# Comparing `tmp/zboxapi-0.0.4.tar.gz` & `tmp/zboxapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zboxapi-0.0.4.tar", max compression
+gzip compressed data, was "zboxapi-0.0.5.tar", max compression
```

## Comparing `zboxapi-0.0.4.tar` & `zboxapi-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      545 2024-05-10 20:21:05.312952 zboxapi-0.0.4/README.md
--rw-r--r--   0        0        0      896 2024-05-15 13:43:43.221360 zboxapi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-15 13:43:43.229360 zboxapi-0.0.4/src/zboxapi/__init__.py
--rw-r--r--   0        0        0     7615 2024-05-15 13:33:43.836917 zboxapi-0.0.4/src/zboxapi/main.py
--rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 zboxapi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      545 2024-05-10 20:21:05.312952 zboxapi-0.0.5/README.md
+-rw-r--r--   0        0        0      896 2024-05-20 15:35:20.449504 zboxapi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-20 15:35:20.457504 zboxapi-0.0.5/src/zboxapi/__init__.py
+-rw-r--r--   0        0        0     7305 2024-05-17 13:55:19.421135 zboxapi-0.0.5/src/zboxapi/main.py
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 zboxapi-0.0.5/PKG-INFO
```

### Comparing `zboxapi-0.0.4/README.md` & `zboxapi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zboxapi-0.0.4/pyproject.toml` & `zboxapi-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zboxapi"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Kelby Valenti <kelby.valenti@gmail.com>", "Timo Sugliani <timo.sugliani@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 zboxapi = "zboxapi.main:launch"
```

### Comparing `zboxapi-0.0.4/src/zboxapi/main.py` & `zboxapi-0.0.5/src/zboxapi/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import contextlib
 import fcntl
 import os
 import re
 import socket
-
-# import ssl
 import subprocess
 import time
 from ipaddress import IPv4Address
 from pathlib import Path
 from typing import IO, Annotated
 
 import uvicorn
 from fastapi import APIRouter, Depends, FastAPI, HTTPException, Security, status
 from fastapi.routing import APIRoute
 from fastapi.security.api_key import APIKey, APIKeyHeader
 from pydantic import AfterValidator, BaseModel
 from pydantic_core import PydanticCustomError
 
+from zboxapi import __version__
+
 api_key_header = APIKeyHeader(name="access_token", auto_error=False)
 
 
 @contextlib.contextmanager
 def get_hosts_file_object():
     pfile = Path("/etc/hosts")
     if not pfile.is_file():
@@ -116,37 +116,25 @@
     """
     for route in api.routes:
         if isinstance(route, APIRoute) and not route.operation_id:
             tag = route.tags[0] if route.tags else "default"
             route.operation_id = f"{tag}_{route.name}"
 
 
-def make_list(obj):
-    return obj if isinstance(obj, list) else [obj]
-
-
-def ip_fqdn_str(obj, ip_key="ip", fqdn_key="fqdn"):
-    return f"ip={getattr(obj, ip_key)}, fqdn={getattr(obj, fqdn_key)}"
-
-
-def ip_fqdn_dict(obj, ip_key="ip", fqdn_key="fqdn"):
-    return {"ip": getattr(obj, ip_key), "fqdn": getattr(obj, fqdn_key)}
-
-
-def RecordNotFound(obj, ip_key="ip", fqdn_key="fqdn"):
+def RecordNotFound(ip, fqdn):
     return HTTPException(
-        status_code=status.HTTP_406_NOT_ACCEPTABLE,
-        detail=f"Record not found: {ip_fqdn_str(obj, ip_key, fqdn_key)}",
+        status_code=status.HTTP_404_NOT_FOUND,
+        detail=f"DNS record not found: ip={ip}, fqdn={fqdn}",
     )
 
 
-def RecordAlreadyPresent(obj, ip_key="ip", fqdn_key="fqdn"):
+def RecordAlreadyPresent(ip, fqdn):
     return HTTPException(
         status_code=status.HTTP_406_NOT_ACCEPTABLE,
-        detail=f"Record already present: {ip_fqdn_str(obj, ip_key, fqdn_key)}",
+        detail=f"DNS record already present: ip={ip}, fqdn={fqdn}",
     )
 
 
 def validate_fqdn(value: str):
     """
     https://en.m.wikipedia.org/wiki/Fully_qualified_domain_name
     """
@@ -172,100 +160,114 @@
         raise PydanticCustomError("value_error", "Invalid fqdn")
     return value
 
 
 FQDN = Annotated[str, AfterValidator(validate_fqdn)]
 
 
-class HostsCreate(BaseModel):
+class DnsCreate(BaseModel):
     ip: IPv4Address
     fqdn: FQDN
 
 
-class HostsDelete(BaseModel):
+class DnsDelete(BaseModel):
     ip: IPv4Address
     fqdn: FQDN
 
 
-class HostsUpdate(BaseModel):
+class DnsUpdate(BaseModel):
     ip: IPv4Address
     fqdn: FQDN
-    new_ip: IPv4Address
-    new_fqdn: FQDN
 
 
-class HostsView(BaseModel):
+class DnsView(BaseModel):
     ip: IPv4Address
     fqdn: str
 
 
-hosts_router = APIRouter(prefix="/hosts", tags=["hosts"])
+dns_router = APIRouter(prefix="/dns", tags=["dns"])
 
 
-@hosts_router.get("")
-def get_hosts(
-    ip: IPv4Address | None = None,
-    fqdn: str | None = None,
-) -> list[HostsView]:
+@dns_router.get("")
+def dns_get_all() -> list[DnsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
-        hosts_lines = filter_hosts_file(hosts_lines, ip, fqdn)
     return hosts_lines
 
 
-@hosts_router.post("")
-def add_hosts(lines_in: list[HostsCreate] | HostsCreate) -> list[HostsView]:
+@dns_router.get("/{ip}/{fqdn}")
+def dns_get(
+    ip: IPv4Address,
+    fqdn: FQDN,
+) -> DnsView:
+    with get_hosts_file_object() as hosts_fo:
+        hosts_lines = get_hosts_lines(hosts_fo)
+        hosts_lines = filter_hosts_file(hosts_lines, ip, fqdn)
+    if not hosts_lines:
+        raise RecordNotFound(ip, fqdn)
+    return hosts_lines[0]
+
+
+@dns_router.post("")
+def dns_add(
+    dns_in: DnsCreate,
+) -> list[DnsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
-        for line in make_list(lines_in):
-            if filter_hosts_file(hosts_lines, line.ip, line.fqdn):
-                raise RecordAlreadyPresent(line)
-            hosts_lines.append(ip_fqdn_dict(line))
+        if filter_hosts_file(hosts_lines, dns_in.ip, dns_in.fqdn):
+            raise RecordAlreadyPresent(dns_in.ip, dns_in.fqdn)
+        hosts_lines.append({"ip": dns_in.ip, "fqdn": dns_in.fqdn})
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
-@hosts_router.put("")
-def update_hosts(lines_in: list[HostsUpdate] | HostsUpdate) -> list[HostsView]:
+@dns_router.put("/{ip}/{fqdn}")
+def dns_update(
+    ip: IPv4Address,
+    fqdn: FQDN,
+    dns_in: DnsUpdate,
+) -> list[DnsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
-        for line in make_list(lines_in):
-            key = ip_fqdn_dict(line)
-            if key not in hosts_lines:
-                raise RecordNotFound(line)
-            ix = hosts_lines.index(key)
-            hosts_lines[ix] = ip_fqdn_dict(line, "new_ip", "new_fqdn")
+        key = {"ip": ip, "fqdn": fqdn}
+        if key not in hosts_lines:
+            raise RecordNotFound(ip, fqdn)
+        ix = hosts_lines.index(key)
+        hosts_lines[ix] = {"ip": dns_in.ip, "fqdn": dns_in.fqdn}
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
-@hosts_router.delete("")
-def delete_hosts(lines_in: list[HostsDelete] | HostsDelete) -> list[HostsView]:
+@dns_router.delete("/{ip}/{fqdn}")
+def dns_delete(
+    ip: IPv4Address,
+    fqdn: FQDN,
+) -> list[DnsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
-        for line in make_list(lines_in):
-            key = ip_fqdn_dict(line)
-            if key not in hosts_lines:
-                raise RecordNotFound(line)
-            hosts_lines.remove(key)
+        key = {"ip": ip, "fqdn": fqdn}
+        if key not in hosts_lines:
+            raise RecordNotFound(ip, fqdn)
+        hosts_lines.remove(key)
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
 zboxapi_root_path = os.getenv("ZBOXAPI_ROOT_PATH", None)
 
 app = FastAPI(
     title="zBox API",
     root_path=zboxapi_root_path,
     dependencies=[Depends(validate_api_key)],
+    version=__version__,
 )
-app.include_router(hosts_router)
+app.include_router(dns_router)
 simplify_operation_ids(app)
 
 ZPOD_PASSWORD = get_zpod_password()
 
 
 def launch():
     uvicorn.run(
```

### Comparing `zboxapi-0.0.4/PKG-INFO` & `zboxapi-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zboxapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Kelby Valenti
 Author-email: kelby.valenti@gmail.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


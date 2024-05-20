# Comparing `tmp/docmesh_cli-0.0.7.tar.gz` & `tmp/docmesh_cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_cli-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_cli-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_cli-0.0.7.tar` & `docmesh_cli-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.7/README.md
--rw-r--r--   0        0        0       83 2024-05-17 06:28:46.358197 docmesh_cli-0.0.7/docmesh_cli/__init__.py
--rw-r--r--   0        0        0     6917 2024-05-17 06:16:22.637165 docmesh_cli-0.0.7/docmesh_cli/client.py
--rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.7/docmesh_cli/logos.py
--rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.8/README.md
+-rw-r--r--   0        0        0       83 2024-05-20 03:20:54.906887 docmesh_cli-0.0.8/docmesh_cli/__init__.py
+-rw-r--r--   0        0        0     8264 2024-05-20 03:20:17.042021 docmesh_cli-0.0.8/docmesh_cli/client.py
+-rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.8/docmesh_cli/logos.py
+-rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.8/PKG-INFO
```

### Comparing `docmesh_cli-0.0.7/docmesh_cli/client.py` & `docmesh_cli-0.0.8/docmesh_cli/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import random
 import requests
 import configparser
+import docmesh_cli
 
 from typing import Any
 
+from packaging.version import Version
 from docmesh_cli.logos import LOGOS
 
 
 RC_FILE = os.path.expanduser("~/.docmeshrc")
 PARSER = configparser.ConfigParser()
 
 ADMIN_SHORTCUTS = {
@@ -53,14 +55,34 @@
 class TermColor:
     blue = "\033[94m"
     green = "\033[92m"
     red = "\033[96m"
     end = "\033[0m"
 
 
+def _check_verseion():
+    current_version = Version(docmesh_cli.__version__)
+
+    # get latest version from pypi
+    pypi_link = f"https://pypi.org/pypi/{docmesh_cli.__name__}/json"
+    rsp = requests.get(pypi_link, timeout=30)
+
+    if rsp.status_code == 200:
+        latest_version = Version(rsp.json()["info"]["version"])
+        if current_version < latest_version:
+            print(
+                f"{TermColor.red}Current client version is {current_version}, the latest verision is {latest_version}."
+                f"You could update the client version using `pip install -U {docmesh_cli.__name__}`. {TermColor.end}"
+            )
+        else:
+            print(f"{TermColor.green}Using the latest client version!{TermColor.end}")
+    else:
+        print(f"{TermColor.red}Check latest client version failed.{TermColor.end}")
+
+
 def _create_profile() -> tuple[str, str]:
     server = input("docmesh server: ")
     access_token = input("docmesh token: ")
     profile = input("profile name: ")
 
     PARSER[profile] = {}
     PARSER[profile]["server"] = server
@@ -143,14 +165,17 @@
 
     return session_id
 
 
 def client() -> None:
     print(random.choice(LOGOS))
 
+    # check client version
+    _check_verseion()
+
     # load server and access_token from profiles
     server, access_token = _profile_management()
 
     # setup headers
     headers = {"Authorization": f"Bearer {access_token}"}
 
     # retreive session_id
@@ -206,16 +231,26 @@
                 _shortcut(server, path, headers, **shortcut_kwargs)
             except Exception:
                 print(f"{TermColor.red}You enter an invalid shortcut {query}\n{_show_shortcut()}{TermColor.end}")
                 continue
         else:
             data = {"session_id": session_id, "query": query}
             if streaming:
+                chunks: list[bytes] = []
                 with requests.post(
                     url=f"{server}/async_agent", headers=headers, json=data, stream=True, timeout=300
                 ) as r:
                     for chunk in r.iter_content(chunk_size=64):
-                        print(chunk.decode(), end="", flush=True)
+                        try:
+                            if chunks:
+                                s = b"".join(chunks.append(chunk)).decode()
+                            else:
+                                s = chunk.decode()
+
+                            chunks = []
+                            print(s, end="", flush=True)
+                        except UnicodeDecodeError:
+                            chunks.append(chunk)
             else:
                 rsp = requests.post(url=f"{server}/agent", headers=headers, json=data, timeout=300)
                 msg = rsp.json()["data"]["msg"]
                 print(msg, end="", flush=True)
```

### Comparing `docmesh_cli-0.0.7/docmesh_cli/logos.py` & `docmesh_cli-0.0.8/docmesh_cli/logos.py`

 * *Files identical despite different names*

### Comparing `docmesh_cli-0.0.7/pyproject.toml` & `docmesh_cli-0.0.8/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/audiconnectpy-2.2.4.tar.gz` & `tmp/audiconnectpy-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.2.4.tar", last modified: Mon May 20 12:50:04 2024, max compression
+gzip compressed data, was "audiconnectpy-2.2.5.tar", last modified: Mon May 20 14:08:07 2024, max compression
```

## Comparing `audiconnectpy-2.2.4.tar` & `audiconnectpy-2.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.990760 audiconnectpy-2.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.990760 audiconnectpy-2.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.990760 audiconnectpy-2.2.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.990760 audiconnectpy-2.2.4/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23323 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:08:07.959404 audiconnectpy-2.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:08:07.951404 audiconnectpy-2.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:08:07.951404 audiconnectpy-2.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:08:07.951404 audiconnectpy-2.2.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 14:08:07.955404 audiconnectpy-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:08:07.955404 audiconnectpy-2.2.5/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23299 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:08:07.955404 audiconnectpy-2.2.5/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 14:08:07.000000 audiconnectpy-2.2.5/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-20 14:08:07.000000 audiconnectpy-2.2.5/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:08:07.000000 audiconnectpy-2.2.5/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:08:07.000000 audiconnectpy-2.2.5/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 14:08:07.000000 audiconnectpy-2.2.5/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 14:08:07.000000 audiconnectpy-2.2.5/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:08:07.959404 audiconnectpy-2.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:08:07.955404 audiconnectpy-2.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:08:07.955404 audiconnectpy-2.2.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-20 14:07:57.000000 audiconnectpy-2.2.5/tests/test_home.py
```

### Comparing `audiconnectpy-2.2.4/.github/dependabot.yml` & `audiconnectpy-2.2.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/.github/workflows/auto-approve.yml` & `audiconnectpy-2.2.5/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.2.5/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.2.5/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/.github/workflows/release.yml` & `audiconnectpy-2.2.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/.gitignore` & `audiconnectpy-2.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/.pre-commit-config.yaml` & `audiconnectpy-2.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/LICENSE` & `audiconnectpy-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/PKG-INFO` & `audiconnectpy-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.4
+Version: 2.2.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.4/README.md` & `audiconnectpy-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/audiconnectpy/api.py` & `audiconnectpy-2.2.5/audiconnectpy/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Audi connect."""
 
 from __future__ import annotations
 
 from collections import namedtuple
 import logging
-from typing import Any, NamedTuple, Self
+from typing import Any, Literal, NamedTuple, Self
 
 from aiohttp import ClientSession
 
 from .auth import Auth
 from .const import (
     URL_HOME_REGION,
     URL_HOME_REGION_SETTER,
     URL_INFO_VEHICLE,
     URL_INFO_VEHICLE_US,
 )
-from .exceptions import AudiException, AuthorizationError
+from .exceptions import AudiException
 from .helpers import ExtendedDict
 from .vehicle import Globals, Vehicle, Vehicles
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AudiConnect:
@@ -28,22 +28,21 @@
     def __init__(
         self,
         session: ClientSession,
         username: str,
         password: str,
         country: str = "DE",
         spin: str | None = None,
+        *,
         unit_system: str = "metric",
+        model: Literal["standard", "e-tron"] = "standard",
     ) -> None:
         """Initialize."""
         Globals(unit_system)
-        self.auth = Auth(session)
-        self.country = country.upper()
-        self._password = password
-        self._username = username
+        self.auth = Auth(session, username, password, country.upper(), model)
         self._spin = spin
         self.vehicles: list[Vehicle] = []
 
     @property
     def is_connected(self) -> bool:
         """Is connected."""
         return self.auth.binded
@@ -53,19 +52,15 @@
         return self.auth.uris
 
     async def async_login(self, vinlist: list[str] | None = None) -> None:
         """Login and retrieve tokens."""
         if self.is_connected:
             return
 
-        # Connect API
-        try:
-            await self.auth.async_connect(self._username, self._password, self.country)
-        except AudiException as error:
-            raise AuthorizationError(error) from error
+        await self.auth.async_connect()
 
         if len(self.vehicles) == 0:
             await self.async_fetch_data(vinlist=vinlist)
 
     async def async_fetch_data(self, vinlist: list[str] | None = None) -> None:
         """Update the state of all vehicles."""
         try:
@@ -95,26 +90,28 @@
                 except AudiException as error:
                     _LOGGER.error(
                         "Error while updating - %s - (%s)", vehicle.vin, error
                     )
 
     async def async_get_information_vehicles(self) -> Any:
         """Get information vehicles."""
+        language = self.uri_services["language"]
+        country = self.uri_services["country"]
+        url = URL_INFO_VEHICLE if country != "US" else URL_INFO_VEHICLE_US
         headers = await self.auth.async_get_headers(
             token_type="audi",
             headers={
-                "Accept-Language": f"{self.uri_services['language']}-{self.country}",
+                "Accept-Language": f"{language}-{country}",
                 "Content-Type": "application/json",
-                "X-User-Country": self.country,
+                "X-User-Country": country,
             },
         )
         data = {
             "query": "query vehicleList {\n userVehicles {\n vin\n mappingVin\n vehicle { core { modelYear\n }\n media { shortName\n longName }\n }\n csid\n commissionNumber\n type\n devicePlatform\n mbbConnect\n userRole {\n role\n }\n vehicle {\n classification {\n driveTrain\n }\n }\n nickname\n }\n}"
         }
-        url = URL_INFO_VEHICLE if self.country != "US" else URL_INFO_VEHICLE_US
 
         response = await self.auth.request(
             "POST", url, json=data, headers=headers, allow_redirects=False
         )
         if "data" not in response:
             raise AudiException("Invalid json in vehicle information")
```

### Comparing `audiconnectpy-2.2.4/audiconnectpy/auth.py` & `audiconnectpy-2.2.5/audiconnectpy/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 import os
 import re
 import socket
 from typing import Any, Literal
 from urllib.parse import parse_qs, urlencode, urlparse
 import uuid
 
-import aiohttp
+from aiohttp import ClientError, ClientSession
 import async_timeout
 from bs4 import BeautifulSoup
 
 from .const import (
-    CLIENT_ID,
+    CLIENT_IDS,
     DELAY,
     HDR_USER_AGENT,
     HDR_XAPP_VERSION,
     MARKET_URL,
     MBB_URL,
     TIMEOUT,
     URL_HERE_COM,
@@ -33,41 +33,51 @@
 from .exceptions import (
     AudiException,
     AuthorizationError,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
 )
-from .helpers import ExtendedDict
+from .helpers import ExtendedDict, retry
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Auth:
     """Authentication."""
 
     def __init__(
-        self, session: aiohttp.ClientSession, proxy: str | None = None
+        self,
+        session: ClientSession,
+        username: str,
+        password: str,
+        country: str,
+        model: Literal["standard", "e-tron"],
+        *,
+        proxy: str | None = None,
     ) -> None:
         """Initialize."""
         self._session = session
+        self._username = username
+        self._password = password
+        self.country = country
+        self.model = model
         self.__proxy: dict[str, str] | None = (
             {"http": proxy, "https": proxy} if proxy else None
         )
 
         self._x_client_id: str | None = None
         self.user_id = ""
         self._mbb_token: dict[str, Any] = {}
         self._here_token: dict[str, Any] = {}
         self._mbb_token_expired: datetime | None = None
         self._idk_token: dict[str, str] = {}
         self._audi_token: dict[str, str] = {}
         self.uris: dict[str, str] = {}
         self.binded: bool = False
-        self.country: str = ""
 
     async def request(
         self,
         method: str,
         url: str,
         raw_reply: bool = False,
         raw_rsp: bool = False,
@@ -80,24 +90,25 @@
                 _LOGGER.debug("REQUEST: %s", url)
                 _LOGGER.debug("REQUEST DATA:%s", kwargs.get("data"))
                 response = await self._session.request(method, url, **kwargs)
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Audi Connect."
             ) from error
-        except (aiohttp.ClientError, socket.gaierror) as error:
+        except (ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with Audi Connect."
             ) from error
 
         content_type = response.headers.get("Content-Type", "")
         contents = (await response.read()).decode("utf8")
 
         _LOGGER.debug("RESPONSE HEADERS: %s", response.headers)
         _LOGGER.debug("RESPONSE: %s ,return_code '%s'", contents, response.status)
+        _LOGGER.debug("---------------------------------------------------------")
 
         if response.status // 100 in [4, 5]:
             response.close()
             if "application/json" in content_type:
                 raise ServiceNotFoundError(response.status, json.loads(contents))
             raise ServiceNotFoundError(response.status, contents)
 
@@ -116,41 +127,31 @@
         else:
             rsp = await response.text()
 
         if raw_reply and raw_rsp:
             return response, rsp
         return rsp
 
-    async def async_connect(
-        self, username: str, password: str, country: str, tries: int = 3
-    ) -> None:
+    async def async_connect(self, tries: int = 3) -> None:
         """Connect to API."""
-        self.country = country
         try:
             await self._async_retrieve_url_service()
         except HttpRequestError as error:
             self.binded = False
-            raise AudiException("Failed retrieve urls service (%s)", error)
+            raise AudiException("Failed retrieve urls service (%s)", error) from error
 
         try:
-            await self._async_login(username, password)
+            await self._async_login()
             self.binded = True
-        except HttpRequestError as error:
-            if tries > 1:
-                _LOGGER.warning(
-                    "Login to Audi service failed, trying again in %s seconds [ERROR:%s]",
-                    DELAY,
-                    str(error),
-                )
-                await asyncio.sleep(DELAY)
-                return await self.async_connect(username, password, country, tries - 1)
+        except AudiException as error:
             self.binded = False
-            raise AuthorizationError("Login to Audi service failed: %s ", error)
+            raise AuthorizationError("Login to Audi service failed") from error
 
-    async def _async_login(self, user: str, password: str) -> None:
+    @retry(exceptions=HttpRequestError, tries=3, delay=DELAY, logger=_LOGGER)
+    async def _async_login(self) -> None:
         """Request login."""
 
         # Generate code_challenge
         code_verifier = str(base64.urlsafe_b64encode(os.urandom(32)), "utf-8").strip(
             "="
         )
         code_challenge = str(
@@ -181,15 +182,17 @@
             headers=headers,
             params=idk_data,
             raw_reply=True,
             raw_rsp=True,
         )
 
         # form_data with email
-        submit_data = self._get_hidden_html_input_form_data(idk_rsptxt, {"email": user})
+        submit_data = self._get_hidden_html_input_form_data(
+            idk_rsptxt, {"email": self._username}
+        )
         submit_url = self._get_post_url(idk_rsptxt, self.uris["authorization_endpoint"])
         # send email
         email_rsptxt = await self.request(
             "POST",
             submit_url,
             data=submit_data,
             headers=headers,
@@ -201,18 +204,18 @@
         # 2022-01-29: new HTML response uses a js two build the html form data + button.
         # Therefore it's not possible to extract hmac and other form data.
         # --> extract hmac from embedded js snippet.
         regex_res = re.findall(r'"hmac"\s*:\s*"[0-9a-fA-F]+"', email_rsptxt)
         if regex_res:
             submit_url = submit_url.replace("identifier", "authenticate")
             submit_data["hmac"] = regex_res[0].split(":")[1].strip('"')
-            submit_data["password"] = password
+            submit_data["password"] = self._password
         else:
             submit_data = self._get_hidden_html_input_form_data(
-                email_rsptxt, {"password": password}
+                email_rsptxt, {"password": self._password}
             )
             submit_url = self._get_post_url(email_rsptxt, submit_url)
 
         # send password
         pw_rsp = await self.request(
             "POST",
             submit_url,
@@ -604,31 +607,30 @@
         )
         _LOGGER.debug("Here Token: %s", hereoauth_json)
         return hereoauth_json
 
     async def _async_retrieve_url_service(self) -> None:
         """Get urls for request."""
         # Get markets to get language
-        country = self.country.upper()
         markets_json = await self.request("GET", f"{MARKET_URL}/markets")
 
         country_spec = ExtendedDict(markets_json).getr(
             "countries.countrySpecifications"
         )
-        if country not in country_spec:
+        if self.country not in country_spec:
             raise AudiException("Country not found")
 
-        language = country_spec[country].get("defaultLanguage")
+        language = country_spec[self.country].get("defaultLanguage")
 
         # Get market config
         services = await self.request(
-            "GET", f"{MARKET_URL}/market/{country}/{language}"
+            "GET", f"{MARKET_URL}/market/{self.country}/{language}"
         )
 
-        client_id = services.get("idkClientIDAndroidLive", CLIENT_ID)
+        client_id = services.get("idkClientIDAndroidLive", CLIENT_IDS[self.model])
         audi_baseurl = services.get(
             "myAudiAuthorizationServerProxyServiceURLProduction"
         )
         profil_url = (
             services.get("idkCustomerProfileMicroserviceBaseURLLive", "") + "/v3"
         )
         mbb_baseurl = services.get("mbbOAuthBaseURLLive", MBB_URL)
@@ -651,11 +653,11 @@
             "here_url": URL_HERE_COM,
             "cv_url": cvvsb_base_url,
             "user_url": URL_INFO_USER,
             "authorization_endpoint": authorization_endpoint_url,
             "token_endpoint": token_endpoint_url,
             "revocation_endpoint": revocation_endpoint_url,
             "language": language,
-            "country": country,
+            "country": self.country,
         }
 
         _LOGGER.debug("Urls of service: %s", self.uris)
```

### Comparing `audiconnectpy-2.2.4/audiconnectpy/const.py` & `audiconnectpy-2.2.5/audiconnectpy/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Constants."""
 
 BRAND = "Audi"
-CLIENT_ID = "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com"
+CLIENT_IDS = {
+    "standard": "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com",
+    "e-tron": "f4d0934f-32bf-4ce4-b3c4-699a7049ad26@apps_vw-dilab_com",
+}
 DELAY = 10
 FAILED = "failed"
 HDR_USER_AGENT = "Android/4.24.2 (Build 800240338.root project 'onetouch-android'.ext.buildTime) Android/11"
 HDR_XAPP_VERSION = "4.24.2"
 MARKET_URL = "https://content.app.my.audi.com/service/mobileapp/configurations"
 MAX_RESPONSE_ATTEMPTS = 10
 MBB_URL = "https://mbboauth-1d.prd.ece.vwg-connect.com/mbbcoauth"
```

### Comparing `audiconnectpy-2.2.4/audiconnectpy/helpers.py` & `audiconnectpy-2.2.5/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/audiconnectpy/model.py` & `audiconnectpy-2.2.5/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/audiconnectpy/vehicle.py` & `audiconnectpy-2.2.5/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.2.5/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.4
+Version: 2.2.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.4/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.2.5/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/example.py` & `audiconnectpy-2.2.5/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/pyproject.toml` & `audiconnectpy-2.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/tests/conftest.py` & `audiconnectpy-2.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/tests/fixtures/audi0.json` & `audiconnectpy-2.2.5/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/tests/fixtures/audi1.json` & `audiconnectpy-2.2.5/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/tests/fixtures/audi2.json` & `audiconnectpy-2.2.5/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.2.5/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/tests/fixtures/location.json` & `audiconnectpy-2.2.5/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.4/tests/test_home.py` & `audiconnectpy-2.2.5/tests/test_home.py`

 * *Files identical despite different names*


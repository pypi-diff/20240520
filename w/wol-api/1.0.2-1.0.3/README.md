# Comparing `tmp/wol_api-1.0.2.tar.gz` & `tmp/wol_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wol_api-1.0.2.tar", last modified: Sun May 19 19:07:10 2024, max compression
+gzip compressed data, was "wol_api-1.0.3.tar", last modified: Mon May 20 09:41:52 2024, max compression
```

## Comparing `wol_api-1.0.2.tar` & `wol_api-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:07:10.197007 wol_api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 19:07:06.000000 wol_api-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 19:07:06.000000 wol_api-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 19:07:10.197007 wol_api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-19 19:07:06.000000 wol_api-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:07:10.197007 wol_api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-19 19:07:06.000000 wol_api-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:07:10.193007 wol_api-1.0.2/wol_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:07:06.000000 wol_api-1.0.2/wol_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:07:10.197007 wol_api-1.0.2/wol_api/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:07:06.000000 wol_api-1.0.2/wol_api/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 19:07:06.000000 wol_api-1.0.2/wol_api/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-19 19:07:06.000000 wol_api-1.0.2/wol_api/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-19 19:07:06.000000 wol_api-1.0.2/wol_api/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:07:10.193007 wol_api-1.0.2/wol_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 19:07:10.000000 wol_api-1.0.2/wol_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-19 19:07:10.000000 wol_api-1.0.2/wol_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:07:10.000000 wol_api-1.0.2/wol_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 19:07:10.000000 wol_api-1.0.2/wol_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:07:10.000000 wol_api-1.0.2/wol_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 19:07:10.000000 wol_api-1.0.2/wol_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 19:07:10.000000 wol_api-1.0.2/wol_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:52.800347 wol_api-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 09:41:44.000000 wol_api-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-20 09:41:52.800347 wol_api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-20 09:41:44.000000 wol_api-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:41:52.800347 wol_api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-20 09:41:44.000000 wol_api-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:52.800347 wol_api-1.0.3/wol_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:52.800347 wol_api-1.0.3/wol_api/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:52.800347 wol_api-1.0.3/wol_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/top_level.txt
```

### Comparing `wol_api-1.0.2/LICENSE` & `wol_api-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.2/PKG-INFO` & `wol_api-1.0.3/wol_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
-Name: wol_api
-Version: 1.0.2
+Name: wol-api
+Version: 1.0.3
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/WakeOnLAN-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 License-File: LICENSE.md
 
 #  WakeOnLAN-API
 
 [![PyPI version](https://badge.fury.io/py/wol-api.svg)](https://badge.fury.io/py/wol-api)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
@@ -29,12 +28,15 @@
 
 ` wol_api --port=8080`
 
 # Docker
 ```
 docker run -d \
   --name="WakeOnLAN-API" \
-  -p port:8080 \
+  -e PORT=8080 \
+  --network host \
   rix1337/docker-wol-api:latest
   ```
 
+The desired port is set by environment variable `PORT` for a reason!
+You must use `--network host`, else the magic packets will not be sent to the correct network.
```

### Comparing `wol_api-1.0.2/setup.py` & `wol_api-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.2/wol_api/providers/version.py` & `wol_api-1.0.3/wol_api/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WakeOnLAN-API
 # Project by https://github.com/rix1337
 
 import re
 
 
 def get_version():
-    return "1.0.2"
+    return "1.0.3"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub(r'[^\d.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `wol_api-1.0.2/wol_api/run.py` & `wol_api-1.0.3/wol_api/run.py`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.2/wol_api.egg-info/PKG-INFO` & `wol_api-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
-Name: wol-api
-Version: 1.0.2
+Name: wol_api
+Version: 1.0.3
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/WakeOnLAN-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 License-File: LICENSE.md
 
 #  WakeOnLAN-API
 
 [![PyPI version](https://badge.fury.io/py/wol-api.svg)](https://badge.fury.io/py/wol-api)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
@@ -29,12 +28,15 @@
 
 ` wol_api --port=8080`
 
 # Docker
 ```
 docker run -d \
   --name="WakeOnLAN-API" \
-  -p port:8080 \
+  -e PORT=8080 \
+  --network host \
   rix1337/docker-wol-api:latest
   ```
 
+The desired port is set by environment variable `PORT` for a reason!
+You must use `--network host`, else the magic packets will not be sent to the correct network.
```


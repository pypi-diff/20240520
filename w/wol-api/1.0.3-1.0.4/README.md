# Comparing `tmp/wol_api-1.0.3.tar.gz` & `tmp/wol_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wol_api-1.0.3.tar", last modified: Mon May 20 09:41:52 2024, max compression
+gzip compressed data, was "wol_api-1.0.4.tar", last modified: Mon May 20 10:33:55 2024, max compression
```

## Comparing `wol_api-1.0.3.tar` & `wol_api-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:52.800347 wol_api-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 09:41:44.000000 wol_api-1.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-20 09:41:52.800347 wol_api-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-20 09:41:44.000000 wol_api-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:41:52.800347 wol_api-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-20 09:41:44.000000 wol_api-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:52.800347 wol_api-1.0.3/wol_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:52.800347 wol_api-1.0.3/wol_api/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-20 09:41:44.000000 wol_api-1.0.3/wol_api/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:41:52.800347 wol_api-1.0.3/wol_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 09:41:52.000000 wol_api-1.0.3/wol_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:55.863291 wol_api-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 10:33:49.000000 wol_api-1.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-20 10:33:55.863291 wol_api-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-20 10:33:49.000000 wol_api-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:33:55.863291 wol_api-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-20 10:33:49.000000 wol_api-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:55.859290 wol_api-1.0.4/wol_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:55.863291 wol_api-1.0.4/wol_api/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-20 10:33:49.000000 wol_api-1.0.4/wol_api/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:33:55.863291 wol_api-1.0.4/wol_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 10:33:55.000000 wol_api-1.0.4/wol_api.egg-info/top_level.txt
```

### Comparing `wol_api-1.0.3/LICENSE.md` & `wol_api-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.3/PKG-INFO` & `wol_api-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wol_api
-Version: 1.0.3
+Version: 1.0.4
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/WakeOnLAN-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wol_api-1.0.3/README.md` & `wol_api-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.3/setup.py` & `wol_api-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # WakeOnLAN-API
-# Projekt by https://github.com/rix1337
+# Project by https://github.com/rix1337
 
 import setuptools
 
 from wol_api.providers.version import get_version
 
 try:
     with open('README.md', encoding='utf-8') as f:
```

### Comparing `wol_api-1.0.3/wol_api/providers/version.py` & `wol_api-1.0.4/wol_api/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # WakeOnLAN-API
 # Project by https://github.com/rix1337
 
 import re
 
 
 def get_version():
-    return "1.0.3"
+    return "1.0.4"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub(r'[^\d.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `wol_api-1.0.3/wol_api/run.py` & `wol_api-1.0.4/wol_api/run.py`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.3/wol_api.egg-info/PKG-INFO` & `wol_api-1.0.4/wol_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wol-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/WakeOnLAN-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```


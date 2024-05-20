# Comparing `tmp/malevich-coretools-0.3.8.tar.gz` & `tmp/malevich-coretools-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malevich-coretools-0.3.8.tar", last modified: Thu Feb 29 13:01:13 2024, max compression
+gzip compressed data, was "malevich-coretools-0.3.9.tar", last modified: Wed Mar 13 23:26:24 2024, max compression
```

## Comparing `malevich-coretools-0.3.8.tar` & `malevich-coretools-0.3.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.214713 malevich-coretools-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-29 13:01:13.214713 malevich-coretools-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-29 13:01:06.000000 malevich-coretools-0.3.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.206713 malevich-coretools-0.3.8/malevich_coretools/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.210713 malevich-coretools-0.3.8/malevich_coretools/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11762 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/abstract/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/abstract/statuses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.210713 malevich-coretools-0.3.8/malevich_coretools/admin/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/admin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.210713 malevich-coretools-0.3.8/malevich_coretools/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/batch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.210713 malevich-coretools-0.3.8/malevich_coretools/funcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/funcs/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    33904 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/funcs/funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/funcs/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.210713 malevich-coretools-0.3.8/malevich_coretools/secondary/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/secondary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/secondary/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/secondary/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/secondary/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/secondary/kafka_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.214713 malevich-coretools-0.3.8/malevich_coretools/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/tools/vast.py
--rw-r--r--   0 runner    (1001) docker     (127)    93382 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/malevich_coretools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:01:13.214713 malevich-coretools-0.3.8/malevich_coretools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-29 13:01:13.000000 malevich-coretools-0.3.8/malevich_coretools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-29 13:01:13.000000 malevich-coretools-0.3.8/malevich_coretools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 13:01:13.000000 malevich-coretools-0.3.8/malevich_coretools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-29 13:01:13.000000 malevich-coretools-0.3.8/malevich_coretools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-29 13:01:13.000000 malevich-coretools-0.3.8/malevich_coretools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 13:01:13.214713 malevich-coretools-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-29 13:00:57.000000 malevich-coretools-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.226301 malevich-coretools-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-13 23:26:24.226301 malevich-coretools-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 23:26:20.000000 malevich-coretools-0.3.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.222301 malevich-coretools-0.3.9/malevich_coretools/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.222301 malevich-coretools-0.3.9/malevich_coretools/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11762 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/abstract/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/abstract/statuses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.222301 malevich-coretools-0.3.9/malevich_coretools/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/admin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.222301 malevich-coretools-0.3.9/malevich_coretools/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/batch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.226301 malevich-coretools-0.3.9/malevich_coretools/funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/funcs/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33904 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/funcs/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/funcs/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.226301 malevich-coretools-0.3.9/malevich_coretools/secondary/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/secondary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/secondary/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/secondary/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/secondary/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/secondary/kafka_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.226301 malevich-coretools-0.3.9/malevich_coretools/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/tools/vast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93382 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/malevich_coretools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 23:26:24.226301 malevich-coretools-0.3.9/malevich_coretools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-13 23:26:24.000000 malevich-coretools-0.3.9/malevich_coretools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-13 23:26:24.000000 malevich-coretools-0.3.9/malevich_coretools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 23:26:24.000000 malevich-coretools-0.3.9/malevich_coretools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-13 23:26:24.000000 malevich-coretools-0.3.9/malevich_coretools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-13 23:26:24.000000 malevich-coretools-0.3.9/malevich_coretools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 23:26:24.226301 malevich-coretools-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-13 23:26:10.000000 malevich-coretools-0.3.9/setup.py
```

### Comparing `malevich-coretools-0.3.8/LICENSE` & `malevich-coretools-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/abstract/abstract.py` & `malevich-coretools-0.3.9/malevich_coretools/abstract/abstract.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/admin/utils.py` & `malevich-coretools-0.3.9/malevich_coretools/admin/utils.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/batch/utils.py` & `malevich-coretools-0.3.9/malevich_coretools/batch/utils.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/funcs/funcs.py` & `malevich-coretools-0.3.9/malevich_coretools/funcs/funcs.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/funcs/helpers.py` & `malevich-coretools-0.3.9/malevich_coretools/funcs/helpers.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/secondary/const.py` & `malevich-coretools-0.3.9/malevich_coretools/secondary/const.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/secondary/helpers.py` & `malevich-coretools-0.3.9/malevich_coretools/secondary/helpers.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/secondary/kafka_utils.py` & `malevich-coretools-0.3.9/malevich_coretools/secondary/kafka_utils.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools/tools/vast.py` & `malevich-coretools-0.3.9/malevich_coretools/tools/vast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import re
 import sys
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 
 def numeric_version(version_str):  # noqa: ANN201
     try:
         # Split the version string by the period
         major, minor, patch = version_str.split(".")
 
@@ -329,15 +329,15 @@
     except ValueError as e:
         print("Error: ", e)
         return None
     return query
 
 
 def vast_settings(
-    id: Optional[int] = None, query: Optional[Union[str, Dict[str, Any]]] = None, api_key: Optional[str] = None, disk: Optional[int] = None
+    id: Optional[int] = None, query: Optional[Union[str, Dict[str, Any]]] = None, api_key: Optional[str] = None, disk: Optional[int] = None, assets: Optional[List[str]] = None
 ) -> str:
     """
     Platform settings for create app:\n
             by nothing - use default query inside\n
             by offer id - try use this id for app\n
             by query - use this query inside\n
 
@@ -360,8 +360,10 @@
             res["query"] = query
     if api_key is not None:
         assert isinstance(api_key, str), "wrong api_key type"
         res["apiKey"] = api_key
     if disk is not None:
         assert isinstance(disk, int), "wrong disk type"
         res["disk"] = disk
+    if assets is not None:
+        res["assets"] = assets
     return json.dumps(res)
```

### Comparing `malevich-coretools-0.3.8/malevich_coretools/utils.py` & `malevich-coretools-0.3.9/malevich_coretools/utils.py`

 * *Files identical despite different names*

### Comparing `malevich-coretools-0.3.8/malevich_coretools.egg-info/SOURCES.txt` & `malevich-coretools-0.3.9/malevich_coretools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


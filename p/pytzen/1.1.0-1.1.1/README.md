# Comparing `tmp/pytzen-1.1.0.tar.gz` & `tmp/pytzen-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytzen-1.1.0.tar", last modified: Sat May 18 16:10:35 2024, max compression
+gzip compressed data, was "pytzen-1.1.1.tar", last modified: Mon May 20 11:40:47 2024, max compression
```

## Comparing `pytzen-1.1.0.tar` & `pytzen-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:10:35.746249 pytzen-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-18 16:10:27.000000 pytzen-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-18 16:10:35.746249 pytzen-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-18 16:10:27.000000 pytzen-1.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-05-18 16:10:27.000000 pytzen-1.1.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      606 2024-05-18 16:10:35.746249 pytzen-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:10:35.746249 pytzen-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:10:35.746249 pytzen-1.1.0/src/pytzen/
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-18 16:10:27.000000 pytzen-1.1.0/src/pytzen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:10:35.746249 pytzen-1.1.0/src/pytzen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-18 16:10:35.000000 pytzen-1.1.0/src/pytzen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-18 16:10:35.000000 pytzen-1.1.0/src/pytzen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:10:35.000000 pytzen-1.1.0/src/pytzen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 16:10:35.000000 pytzen-1.1.0/src/pytzen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:47.752894 pytzen-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-20 11:40:38.000000 pytzen-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-20 11:40:38.000000 pytzen-1.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-20 11:40:47.752894 pytzen-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-20 11:40:38.000000 pytzen-1.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-05-20 11:40:38.000000 pytzen-1.1.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-20 11:40:47.752894 pytzen-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:47.752894 pytzen-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:47.752894 pytzen-1.1.1/src/pytzen/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-20 11:40:38.000000 pytzen-1.1.1/src/pytzen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:47.752894 pytzen-1.1.1/src/pytzen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-20 11:40:47.000000 pytzen-1.1.1/src/pytzen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-20 11:40:47.000000 pytzen-1.1.1/src/pytzen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:40:47.000000 pytzen-1.1.1/src/pytzen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 11:40:47.000000 pytzen-1.1.1/src/pytzen.egg-info/top_level.txt
```

### Comparing `pytzen-1.1.0/LICENSE` & `pytzen-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytzen-1.1.0/PKG-INFO` & `pytzen-1.1.1/src/pytzen/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pytzen
-Version: 1.1.0
-Summary: Software engineering studies
-Home-page: https://pytzen.com
-Author: PYTZEN
-Project-URL: Source Code, https://github.com/pytzen/pytzen
-Project-URL: Code Usage, https://usage.pytzen.com
-Project-URL: Studies Wiki, https://github.com/pytzen/pytzen/wiki
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-```python
 """PYTZEN is designed to sketch out data pipelines.
 """
 
 import json
 import sys
 import importlib.util
 import os
@@ -178,8 +161,7 @@
         """
 
         if hasattr(self, key):
             error = f"Attribute '{key}' already exists and cannot be changed."
             raise AttributeError(error)
         else:
             super().__setattr__(key, value)
-```
```


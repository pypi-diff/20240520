# Comparing `tmp/socketwrench-2.0.1.tar.gz` & `tmp/socketwrench-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-2.0.1.tar", last modified: Sun May 19 01:52:19 2024, max compression
+gzip compressed data, was "socketwrench-2.0.3.tar", last modified: Mon May 20 21:02:12 2024, max compression
```

## Comparing `socketwrench-2.0.1.tar` & `socketwrench-2.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:19.119880 socketwrench-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-19 01:52:14.000000 socketwrench-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 01:52:14.000000 socketwrench-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-19 01:52:19.119880 socketwrench-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-05-19 01:52:14.000000 socketwrench-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-19 01:52:14.000000 socketwrench-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 01:52:19.119880 socketwrench-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:19.111880 socketwrench-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:19.115880 socketwrench-2.0.1/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:19.119880 socketwrench-2.0.1/src/socketwrench/fake_imports/
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_tempfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/fake_imports/fake_traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)    35292 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/public.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:19.119880 socketwrench-2.0.1/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:19.119880 socketwrench-2.0.1/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:19.119880 socketwrench-2.0.1/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/standardlib_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    33772 2024-05-19 01:52:14.000000 socketwrench-2.0.1/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:52:19.119880 socketwrench-2.0.1/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-19 01:52:19.000000 socketwrench-2.0.1/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-19 01:52:19.000000 socketwrench-2.0.1/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 01:52:19.000000 socketwrench-2.0.1/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 01:52:19.000000 socketwrench-2.0.1/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.684836 socketwrench-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-20 21:02:08.000000 socketwrench-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 21:02:08.000000 socketwrench-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-20 21:02:12.684836 socketwrench-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-05-20 21:02:08.000000 socketwrench-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-20 21:02:08.000000 socketwrench-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:02:12.684836 socketwrench-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.676836 socketwrench-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.680836 socketwrench-2.0.3/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.680836 socketwrench-2.0.3/src/socketwrench/fake_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/fake_imports/fake_traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35292 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/public.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.680836 socketwrench-2.0.3/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.680836 socketwrench-2.0.3/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.684836 socketwrench-2.0.3/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/standardlib_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33772 2024-05-20 21:02:08.000000 socketwrench-2.0.3/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:02:12.684836 socketwrench-2.0.3/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-20 21:02:12.000000 socketwrench-2.0.3/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-20 21:02:12.000000 socketwrench-2.0.3/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:02:12.000000 socketwrench-2.0.3/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 21:02:12.000000 socketwrench-2.0.3/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-2.0.1/LICENSE` & `socketwrench-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/PKG-INFO` & `socketwrench-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 2.0.1
+Version: 2.0.3
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-2.0.1/README.md` & `socketwrench-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/pyproject.toml` & `socketwrench-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "2.0.1"
+version = "2.0.3"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-2.0.1/src/socketwrench/__init__.py` & `socketwrench-2.0.3/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/__main__.py` & `socketwrench-2.0.3/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/connection.py` & `socketwrench-2.0.3/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/fake_imports/__init__.py` & `socketwrench-2.0.3/src/socketwrench/fake_imports/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/fake_imports/fake_argparse.py` & `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_argparse.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/fake_imports/fake_datetime.py` & `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_datetime.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/fake_imports/fake_inspect.py` & `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_inspect.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/fake_imports/fake_json.py` & `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_json.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/fake_imports/fake_logging.py` & `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_logging.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/fake_imports/fake_pathlib.py` & `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_pathlib.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/fake_imports/fake_tempfile.py` & `socketwrench-2.0.3/src/socketwrench/fake_imports/fake_tempfile.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/handlers.py` & `socketwrench-2.0.3/src/socketwrench/handlers.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/openapi.py` & `socketwrench-2.0.3/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/public.py` & `socketwrench-2.0.3/src/socketwrench/public.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/resources/favicon.ico` & `socketwrench-2.0.3/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/resources/playground/panels.js` & `socketwrench-2.0.3/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/resources/playground/playground.html` & `socketwrench-2.0.3/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/resources/playground/playground.js` & `socketwrench-2.0.3/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/resources/swagger.html` & `socketwrench-2.0.3/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/samples/file_sample.py` & `socketwrench-2.0.3/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/samples/sample.py` & `socketwrench-2.0.3/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/server.py` & `socketwrench-2.0.3/src/socketwrench/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,20 +246,20 @@
             r = r.rstrip(", ")
             r += ")>"
             self._rep = r
         return self._rep
 
 
     @classmethod
-    def serve_class(cls, c, thread: bool = False, cleanup_event = None, pause_event = None, **kwargs):
+    def serve_class(cls, c, thread: bool = False, cleanup_event = None, pause_event = None, run_in_background=False, **kwargs):
         inst = c()
-        return cls(inst, serve=False, **kwargs).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event)
+        return cls(inst, serve=False, **kwargs).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event, run_in_background=run_in_background)
 
     @classmethod
-    def serve_module(cls, module, thread: bool = False, cleanup_event = None, pause_event = None, **kwargs):
+    def serve_module(cls, module, thread: bool = False, cleanup_event = None, pause_event = None, run_in_background=False, **kwargs):
         if isinstance(module, Path):
             from socketwrench.standardlib_dependencies import importlib, modules
             module = importlib.util.spec_from_file_location("module", module)
             module = importlib.util.module_from_spec(module)
             module.__file__ = module.__spec__.origin
             module.__package__ = module.__spec__.name
             modules[module.__spec__.name] = module
@@ -268,9 +268,9 @@
             try:
                 from socketwrench.standardlib_dependencies import importlib
                 module = importlib.import_module(module)
             except ImportError:
                 parts = module.split(".")
                 module = importlib.import_module(".".join(parts[:-1]))
                 module = getattr(module, parts[-1])
-        return cls(module, **kwargs).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event)
+        return cls(module, **kwargs).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event, run_in_background=run_in_background)
```

### Comparing `socketwrench-2.0.1/src/socketwrench/settings.py` & `socketwrench-2.0.3/src/socketwrench/settings.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/standardlib_dependencies.py` & `socketwrench-2.0.3/src/socketwrench/standardlib_dependencies.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/tags.py` & `socketwrench-2.0.3/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench/types.py` & `socketwrench-2.0.3/src/socketwrench/types.py`

 * *Files identical despite different names*

### Comparing `socketwrench-2.0.1/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-2.0.3/src/socketwrench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 2.0.1
+Version: 2.0.3
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-2.0.1/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-2.0.3/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*


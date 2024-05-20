# Comparing `tmp/dreams_core-0.0.7.tar.gz` & `tmp/dreams_core-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreams_core-0.0.7.tar", last modified: Sat May  4 03:33:46 2024, max compression
+gzip compressed data, was "dreams_core-0.1.0.tar", last modified: Mon May 20 21:47:38 2024, max compression
```

## Comparing `dreams_core-0.0.7.tar` & `dreams_core-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-04 03:33:46.478028 dreams_core-0.0.7/
--rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.0.7/LICENSE
--rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-25 04:05:52.000000 dreams_core-0.0.7/MANIFEST.in
--rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-04 03:33:46.477732 dreams_core-0.0.7/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.0.7/README.md
--rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-05-04 03:33:28.000000 dreams_core-0.0.7/pyproject.toml
--rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-05-04 03:33:46.478079 dreams_core-0.0.7/setup.cfg
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-04 03:33:46.474913 dreams_core-0.0.7/src/
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-04 03:33:46.476703 dreams_core-0.0.7/src/dreams_core/
--rw-r--r--   0 jeremy     (502) staff       (20)       21 2024-04-27 00:22:32.000000 dreams_core-0.0.7/src/dreams_core/__init__.py
--rw-r--r--   0 jeremy     (502) staff       (20)     5233 2024-04-27 00:20:21.000000 dreams_core-0.0.7/src/dreams_core/core.py
--rw-r--r--   0 jeremy     (502) staff       (20)     3897 2024-04-25 04:03:45.000000 dreams_core-0.0.7/src/dreams_core/dune.py
--rw-r--r--   0 jeremy     (502) staff       (20)     4578 2024-05-04 03:33:20.000000 dreams_core-0.0.7/src/dreams_core/googlecloud.py
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-04 03:33:46.477475 dreams_core-0.0.7/src/dreams_core.egg-info/
--rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-04 03:33:46.000000 dreams_core-0.0.7/src/dreams_core.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      369 2024-05-04 03:33:46.000000 dreams_core-0.0.7/src/dreams_core.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-05-04 03:33:46.000000 dreams_core-0.0.7/src/dreams_core.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-05-04 03:33:46.000000 dreams_core-0.0.7/src/dreams_core.egg-info/requires.txt
--rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-05-04 03:33:46.000000 dreams_core-0.0.7/src/dreams_core.egg-info/top_level.txt
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-20 21:47:38.981652 dreams_core-0.1.0/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.1.0/LICENSE
+-rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-25 04:05:52.000000 dreams_core-0.1.0/MANIFEST.in
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-20 21:47:38.981376 dreams_core-0.1.0/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.1.0/README.md
+-rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-05-20 21:47:03.000000 dreams_core-0.1.0/pyproject.toml
+-rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-05-20 21:47:38.981697 dreams_core-0.1.0/setup.cfg
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-20 21:47:38.976592 dreams_core-0.1.0/src/
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-20 21:47:38.978741 dreams_core-0.1.0/src/dreams_core/
+-rw-r--r--   0 jeremy     (502) staff       (20)       21 2024-04-27 00:22:32.000000 dreams_core-0.1.0/src/dreams_core/__init__.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     5233 2024-04-27 00:20:21.000000 dreams_core-0.1.0/src/dreams_core/core.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     3897 2024-04-25 04:03:45.000000 dreams_core-0.1.0/src/dreams_core/dune.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     7234 2024-05-20 21:36:33.000000 dreams_core-0.1.0/src/dreams_core/googlecloud.py
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-20 21:47:38.981062 dreams_core-0.1.0/src/dreams_core.egg-info/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      369 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-05-20 21:47:38.000000 dreams_core-0.1.0/src/dreams_core.egg-info/top_level.txt
```

### Comparing `dreams_core-0.0.7/LICENSE` & `dreams_core-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.7/PKG-INFO` & `dreams_core-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.0.7
+Version: 0.1.0
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dreams_core-0.0.7/pyproject.toml` & `dreams_core-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreams_core"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="tentabs", email="tentabs00@gmail.com" },
 ]
 description = "brought to you by the dreamslabs discord community"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `dreams_core-0.0.7/src/dreams_core/core.py` & `dreams_core-0.1.0/src/dreams_core/core.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.7/src/dreams_core/dune.py` & `dreams_core-0.1.0/src/dreams_core/dune.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.7/src/dreams_core.egg-info/PKG-INFO` & `dreams_core-0.1.0/src/dreams_core.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.0.7
+Version: 0.1.0
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


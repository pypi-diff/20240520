# Comparing `tmp/colalamo-0.1.2101.tar.gz` & `tmp/colalamo-0.1.2102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colalamo-0.1.2101.tar", last modified: Sun May 19 22:14:56 2024, max compression
+gzip compressed data, was "colalamo-0.1.2102.tar", last modified: Sun May 19 22:16:46 2024, max compression
```

## Comparing `colalamo-0.1.2101.tar` & `colalamo-0.1.2102.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:14:56.649026 colalamo-0.1.2101/
--rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-19 22:14:56.648348 colalamo-0.1.2101/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      765 2024-05-19 22:12:15.000000 colalamo-0.1.2101/pyproject.toml
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-19 22:14:56.649133 colalamo-0.1.2101/setup.cfg
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:14:56.639081 colalamo-0.1.2101/src/
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:14:56.643669 colalamo-0.1.2101/src/colalamo/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-05-19 21:41:09.000000 colalamo-0.1.2101/src/colalamo/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5215 2024-05-19 22:14:43.000000 colalamo-0.1.2101/src/colalamo/colalamo.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1152 2024-05-19 01:18:45.000000 colalamo-0.1.2101/src/colalamo/config.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4051 2024-05-19 22:14:50.000000 colalamo-0.1.2101/src/colalamo/shtoken.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:14:56.647713 colalamo-0.1.2101/src/colalamo.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      294 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       52 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        9 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/top_level.txt
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:16:46.236913 colalamo-0.1.2102/
+-rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-19 22:16:46.236073 colalamo-0.1.2102/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      765 2024-05-19 22:15:38.000000 colalamo-0.1.2102/pyproject.toml
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-19 22:16:46.237050 colalamo-0.1.2102/setup.cfg
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:16:46.228646 colalamo-0.1.2102/src/
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:16:46.231502 colalamo-0.1.2102/src/colalamo/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-05-19 21:41:09.000000 colalamo-0.1.2102/src/colalamo/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5215 2024-05-19 22:14:43.000000 colalamo-0.1.2102/src/colalamo/colalamo.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1152 2024-05-19 01:18:45.000000 colalamo-0.1.2102/src/colalamo/config.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4051 2024-05-19 22:14:50.000000 colalamo-0.1.2102/src/colalamo/shtoken.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:16:46.235393 colalamo-0.1.2102/src/colalamo.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-19 22:16:46.000000 colalamo-0.1.2102/src/colalamo.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      294 2024-05-19 22:16:46.000000 colalamo-0.1.2102/src/colalamo.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 22:16:46.000000 colalamo-0.1.2102/src/colalamo.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       52 2024-05-19 22:16:46.000000 colalamo-0.1.2102/src/colalamo.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        9 2024-05-19 22:16:46.000000 colalamo-0.1.2102/src/colalamo.egg-info/top_level.txt
```

### Comparing `colalamo-0.1.2101/pyproject.toml` & `colalamo-0.1.2102/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "colalamo"
-version = "0.1.2101"
+version = "0.1.2102"
 description = "direct api via copilot to its large language models"
 authors = [
     { name = "tolitius" },
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 keywords = ["ai", "copilot", "github", "gpt", "openai", "code generation"]
```

### Comparing `colalamo-0.1.2101/src/colalamo/colalamo.py` & `colalamo-0.1.2102/src/colalamo/colalamo.py`

 * *Files identical despite different names*

### Comparing `colalamo-0.1.2101/src/colalamo/config.py` & `colalamo-0.1.2102/src/colalamo/config.py`

 * *Files identical despite different names*

### Comparing `colalamo-0.1.2101/src/colalamo/shtoken.py` & `colalamo-0.1.2102/src/colalamo/shtoken.py`

 * *Files identical despite different names*

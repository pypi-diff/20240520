# Comparing `tmp/colalamo-0.1.2104.tar.gz` & `tmp/colalamo-0.1.2105.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colalamo-0.1.2104.tar", last modified: Mon May 20 04:28:27 2024, max compression
+gzip compressed data, was "colalamo-0.1.2105.tar", last modified: Mon May 20 05:12:50 2024, max compression
```

## Comparing `colalamo-0.1.2104.tar` & `colalamo-0.1.2105.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-20 04:28:27.394825 colalamo-0.1.2104/
--rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-20 04:28:27.393621 colalamo-0.1.2104/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      765 2024-05-20 04:28:21.000000 colalamo-0.1.2104/pyproject.toml
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-20 04:28:27.395001 colalamo-0.1.2104/setup.cfg
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-20 04:28:27.381188 colalamo-0.1.2104/src/
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-20 04:28:27.385879 colalamo-0.1.2104/src/colalamo/
--rw-r--r--   0 tolitius   (503) staff       (20)       30 2024-05-20 04:10:18.000000 colalamo-0.1.2104/src/colalamo/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5252 2024-05-20 04:27:37.000000 colalamo-0.1.2104/src/colalamo/colalamo.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1152 2024-05-19 01:18:45.000000 colalamo-0.1.2104/src/colalamo/config.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4051 2024-05-19 22:14:50.000000 colalamo-0.1.2104/src/colalamo/shtoken.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-20 04:28:27.392434 colalamo-0.1.2104/src/colalamo.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-20 04:28:27.000000 colalamo-0.1.2104/src/colalamo.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      294 2024-05-20 04:28:27.000000 colalamo-0.1.2104/src/colalamo.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-20 04:28:27.000000 colalamo-0.1.2104/src/colalamo.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       52 2024-05-20 04:28:27.000000 colalamo-0.1.2104/src/colalamo.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        9 2024-05-20 04:28:27.000000 colalamo-0.1.2104/src/colalamo.egg-info/top_level.txt
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-20 05:12:50.519554 colalamo-0.1.2105/
+-rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-20 05:12:50.518518 colalamo-0.1.2105/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      765 2024-05-20 05:12:41.000000 colalamo-0.1.2105/pyproject.toml
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-20 05:12:50.519739 colalamo-0.1.2105/setup.cfg
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-20 05:12:50.509038 colalamo-0.1.2105/src/
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-20 05:12:50.512835 colalamo-0.1.2105/src/colalamo/
+-rw-r--r--   0 tolitius   (503) staff       (20)       30 2024-05-20 04:10:18.000000 colalamo-0.1.2105/src/colalamo/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5252 2024-05-20 04:27:37.000000 colalamo-0.1.2105/src/colalamo/colalamo.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1152 2024-05-19 01:18:45.000000 colalamo-0.1.2105/src/colalamo/config.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4141 2024-05-20 05:12:24.000000 colalamo-0.1.2105/src/colalamo/shtoken.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-20 05:12:50.517648 colalamo-0.1.2105/src/colalamo.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-20 05:12:50.000000 colalamo-0.1.2105/src/colalamo.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      294 2024-05-20 05:12:50.000000 colalamo-0.1.2105/src/colalamo.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-20 05:12:50.000000 colalamo-0.1.2105/src/colalamo.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       52 2024-05-20 05:12:50.000000 colalamo-0.1.2105/src/colalamo.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        9 2024-05-20 05:12:50.000000 colalamo-0.1.2105/src/colalamo.egg-info/top_level.txt
```

### Comparing `colalamo-0.1.2104/pyproject.toml` & `colalamo-0.1.2105/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "colalamo"
-version = "0.1.2104"
+version = "0.1.2105"
 description = "direct api via copilot to its large language models"
 authors = [
     { name = "tolitius" },
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 keywords = ["ai", "copilot", "github", "gpt", "openai", "code generation"]
```

### Comparing `colalamo-0.1.2104/src/colalamo/colalamo.py` & `colalamo-0.1.2105/src/colalamo/colalamo.py`

 * *Files identical despite different names*

### Comparing `colalamo-0.1.2104/src/colalamo/config.py` & `colalamo-0.1.2105/src/colalamo/config.py`

 * *Files identical despite different names*

### Comparing `colalamo-0.1.2104/src/colalamo/shtoken.py` & `colalamo-0.1.2105/src/colalamo/shtoken.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,18 @@
     user_code = parsed.get('user_code')
     verification_uri = parsed.get('verification_uri')
 
     print(f'browse to {verification_uri} and enter this code "{user_code}" to authenticate')
 
     access_token = wait_for_access_token(device_code)
 
+    # don't create an invaid token file
+    if access_token is None:
+        return None
+
     with open(token_file, 'w') as f:
         f.write(access_token)
 
     return access_token
 
 def refresh_token(token_file=None):
```


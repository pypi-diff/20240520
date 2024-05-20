# Comparing `tmp/jupyter_server_globbing-0.1.4.tar.gz` & `tmp/jupyter_server_globbing-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_server_globbing-0.1.4.tar", last modified: Mon May 20 14:33:25 2024, max compression
+gzip compressed data, was "jupyter_server_globbing-0.1.5.tar", last modified: Mon May 20 14:42:49 2024, max compression
```

## Comparing `jupyter_server_globbing-0.1.4.tar` & `jupyter_server_globbing-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.946880 jupyter_server_globbing-0.1.4/
--rw-r--r--   0 tparment (15010) diana    (200036)      143 2024-05-20 14:33:25.946298 jupyter_server_globbing-0.1.4/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      640 2024-05-20 14:30:23.000000 jupyter_server_globbing-0.1.4/README.md
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.942453 jupyter_server_globbing-0.1.4/globbing/
--rw-r--r--   0 tparment (15010) diana    (200036)      380 2024-05-20 14:15:24.000000 jupyter_server_globbing-0.1.4/globbing/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)      852 2024-05-20 14:32:43.000000 jupyter_server_globbing-0.1.4/globbing/handlers.py
--rw-r--r--   0 tparment (15010) diana    (200036)       22 2024-05-20 14:31:14.000000 jupyter_server_globbing-0.1.4/globbing/version.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.939784 jupyter_server_globbing-0.1.4/jupyter-config/
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.942927 jupyter_server_globbing-0.1.4/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 tparment (15010) diana    (200036)      101 2024-05-20 13:09:27.000000 jupyter_server_globbing-0.1.4/jupyter-config/jupyter_server_config.d/globbing.json
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:33:25.945708 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)      143 2024-05-20 14:33:25.000000 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)      321 2024-05-20 14:33:25.000000 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-05-20 14:33:25.000000 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        9 2024-05-20 14:33:25.000000 jupyter_server_globbing-0.1.4/jupyter_server_globbing.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-05-20 14:33:25.947009 jupyter_server_globbing-0.1.4/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)      442 2024-05-20 14:30:56.000000 jupyter_server_globbing-0.1.4/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:42:49.833032 jupyter_server_globbing-0.1.5/
+-rw-r--r--   0 tparment (15010) diana    (200036)      203 2024-05-20 14:42:49.832452 jupyter_server_globbing-0.1.5/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      617 2024-05-20 14:41:01.000000 jupyter_server_globbing-0.1.5/README.md
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:42:49.829111 jupyter_server_globbing-0.1.5/globbing/
+-rw-r--r--   0 tparment (15010) diana    (200036)      380 2024-05-20 14:15:24.000000 jupyter_server_globbing-0.1.5/globbing/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      852 2024-05-20 14:32:43.000000 jupyter_server_globbing-0.1.5/globbing/handlers.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       22 2024-05-20 14:42:19.000000 jupyter_server_globbing-0.1.5/globbing/version.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:42:49.826694 jupyter_server_globbing-0.1.5/jupyter-config/
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:42:49.829563 jupyter_server_globbing-0.1.5/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 tparment (15010) diana    (200036)      101 2024-05-20 13:09:27.000000 jupyter_server_globbing-0.1.5/jupyter-config/jupyter_server_config.d/globbing.json
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-05-20 14:42:49.831877 jupyter_server_globbing-0.1.5/jupyter_server_globbing.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)      203 2024-05-20 14:42:49.000000 jupyter_server_globbing-0.1.5/jupyter_server_globbing.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)      321 2024-05-20 14:42:49.000000 jupyter_server_globbing-0.1.5/jupyter_server_globbing.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-05-20 14:42:49.000000 jupyter_server_globbing-0.1.5/jupyter_server_globbing.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        9 2024-05-20 14:42:49.000000 jupyter_server_globbing-0.1.5/jupyter_server_globbing.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-05-20 14:42:49.833159 jupyter_server_globbing-0.1.5/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)      525 2024-05-20 14:41:40.000000 jupyter_server_globbing-0.1.5/setup.py
```

### Comparing `jupyter_server_globbing-0.1.4/README.md` & `jupyter_server_globbing-0.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# a Jupyter server extension that supports file globbing
+# jupyter-server-globbing
 
-This extension allows you to use file globbing in Jupyter.
+a Jupyter server extension that supports file globbing
 
-You issue a URL like `/api/globbing/some/path/*.ipynb`
+you issue a URL like `/api/globbing/some/path/*.ipynb`  
 and it returns a list of all the files that match the glob pattern
 
 ## Installation
 
 ```bash
 pip install jupyter-server-globbing
 ```
@@ -14,15 +14,18 @@
 ## Usage
 
 ```javascript
 // from the browser console
 response = await fetch("/api/globbing/some/path/*.ipynb")
 files = await response.json()
 ```
+
 the result is a list of objects with the following structure:
 
 ```json
   {
-    "path": "some/path/file1.ipynb",  // relative to the server root
-    "type": "file" // or "directory"
+      "path": "some/path/file1.ipynb",
+    // relative to the server root
+    "type": "file"
+    // or "directory"
   }
 ```
```

### Comparing `jupyter_server_globbing-0.1.4/globbing/handlers.py` & `jupyter_server_globbing-0.1.5/globbing/handlers.py`

 * *Files identical despite different names*


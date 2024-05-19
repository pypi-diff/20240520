# Comparing `tmp/colalamo-0.1.21.tar.gz` & `tmp/colalamo-0.1.2101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colalamo-0.1.21.tar", last modified: Sun May 19 21:29:21 2024, max compression
+gzip compressed data, was "colalamo-0.1.2101.tar", last modified: Sun May 19 22:14:56 2024, max compression
```

## Comparing `colalamo-0.1.21.tar` & `colalamo-0.1.2101.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:29:21.543224 colalamo-0.1.21/
--rw-r--r--   0 tolitius   (503) staff       (20)      507 2024-05-19 21:29:21.542589 colalamo-0.1.21/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      784 2024-05-19 21:29:09.000000 colalamo-0.1.21/pyproject.toml
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-19 21:29:21.543333 colalamo-0.1.21/setup.cfg
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:29:21.533942 colalamo-0.1.21/src/
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:29:21.538007 colalamo-0.1.21/src/colalamo/
--rw-r--r--   0 tolitius   (503) staff       (20)       27 2024-05-19 21:21:19.000000 colalamo-0.1.21/src/colalamo/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5207 2024-05-19 20:54:44.000000 colalamo-0.1.21/src/colalamo/colalamo.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1152 2024-05-19 01:18:45.000000 colalamo-0.1.21/src/colalamo/config.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4050 2024-05-19 01:03:25.000000 colalamo-0.1.21/src/colalamo/shtoken.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:29:21.542034 colalamo-0.1.21/src/colalamo.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      507 2024-05-19 21:29:21.000000 colalamo-0.1.21/src/colalamo.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      294 2024-05-19 21:29:21.000000 colalamo-0.1.21/src/colalamo.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 21:29:21.000000 colalamo-0.1.21/src/colalamo.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       52 2024-05-19 21:29:21.000000 colalamo-0.1.21/src/colalamo.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        9 2024-05-19 21:29:21.000000 colalamo-0.1.21/src/colalamo.egg-info/top_level.txt
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:14:56.649026 colalamo-0.1.2101/
+-rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-19 22:14:56.648348 colalamo-0.1.2101/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      765 2024-05-19 22:12:15.000000 colalamo-0.1.2101/pyproject.toml
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-19 22:14:56.649133 colalamo-0.1.2101/setup.cfg
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:14:56.639081 colalamo-0.1.2101/src/
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:14:56.643669 colalamo-0.1.2101/src/colalamo/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-05-19 21:41:09.000000 colalamo-0.1.2101/src/colalamo/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5215 2024-05-19 22:14:43.000000 colalamo-0.1.2101/src/colalamo/colalamo.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1152 2024-05-19 01:18:45.000000 colalamo-0.1.2101/src/colalamo/config.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4051 2024-05-19 22:14:50.000000 colalamo-0.1.2101/src/colalamo/shtoken.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 22:14:56.647713 colalamo-0.1.2101/src/colalamo.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      509 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      294 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       52 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        9 2024-05-19 22:14:56.000000 colalamo-0.1.2101/src/colalamo.egg-info/top_level.txt
```

### Comparing `colalamo-0.1.21/pyproject.toml` & `colalamo-0.1.2101/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "colalamo"
-version = "0.1.21"
+version = "0.1.2101"
 description = "direct api via copilot to its large language models"
 authors = [
     { name = "tolitius" },
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 keywords = ["ai", "copilot", "github", "gpt", "openai", "code generation"]
 
 dependencies = []
 
-[tool.setuptools]
-package-dir = {"" = "src"}
-packages = ["colalamo"]
+[tool.setuptools.packages.find]
+where = ["src"]
 
 [project.scripts]
 colalamo = "colalamo.colalamo:main"
 
 [project.urls]
 Homepage = "https://github.com/tolitius/colalamo"
 Documentation = "https://github.com/tolitius/colalamo?tab=readme-ov-file#-colalamo"
```

### Comparing `colalamo-0.1.21/src/colalamo/colalamo.py` & `colalamo-0.1.2101/src/colalamo/colalamo.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import json
 
 import http.server
 import socketserver
 import requests
 
-import shtoken
+from . import shtoken
 
-from config import (
+from .config import (
     HEADERS,
     COPILOT_CHAT_HEADERS,
     GITHUB_COPILOT_CHAT_COMPLETIONS_URL
 )
 
 class Copilot():
```

### Comparing `colalamo-0.1.21/src/colalamo/config.py` & `colalamo-0.1.2101/src/colalamo/config.py`

 * *Files identical despite different names*

### Comparing `colalamo-0.1.21/src/colalamo/shtoken.py` & `colalamo-0.1.2101/src/colalamo/shtoken.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import http.server
 import requests
 import json
 import time
 import sys
 import os
 
-from config import (
+from .config import (
     GITHUB_DEVICE_CODE_URL,
     GITHUB_ACCESS_TOKEN_URL,
     GITHUB_COPILOT_TOKEN_URL,
     HEADERS,
     CLIENT_ID,
     DEVICE_CODE_DATA_TEMPLATE,
     ACCESS_TOKEN_DATA_TEMPLATE,
```


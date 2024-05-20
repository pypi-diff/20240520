# Comparing `tmp/fleekapi-0.1.242.tar.gz` & `tmp/fleekapi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.1.242.tar", last modified: Sun May 19 15:11:36 2024, max compression
+gzip compressed data, was "fleekapi-0.2.tar", last modified: Mon May 20 20:53:59 2024, max compression
```

## Comparing `fleekapi-0.1.242.tar` & `fleekapi-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 15:11:36.415739 fleekapi-0.1.242/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     1085 2024-05-19 13:25:10.000000 fleekapi-0.1.242/LICENCE
--rw-r--r--   0 hasan     (1002) hasan     (1002)     7781 2024-05-19 15:11:36.415739 fleekapi-0.1.242/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     6864 2024-05-19 15:03:24.000000 fleekapi-0.1.242/README.md
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 15:11:36.411738 fleekapi-0.1.242/fleekapi/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       26 2024-05-19 13:15:32.000000 fleekapi-0.1.242/fleekapi/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 15:09:00.000000 fleekapi-0.1.242/fleekapi/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      674 2024-05-19 13:15:32.000000 fleekapi-0.1.242/fleekapi/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      972 2024-05-19 13:15:32.000000 fleekapi-0.1.242/fleekapi/response.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 15:11:36.415739 fleekapi-0.1.242/fleekapi.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     7781 2024-05-19 15:11:36.000000 fleekapi-0.1.242/fleekapi.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      266 2024-05-19 15:11:36.000000 fleekapi-0.1.242/fleekapi.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 15:11:36.000000 fleekapi-0.1.242/fleekapi.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-19 15:11:36.000000 fleekapi-0.1.242/fleekapi.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 15:11:36.000000 fleekapi-0.1.242/fleekapi.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 15:11:36.415739 fleekapi-0.1.242/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     4005 2024-05-19 15:11:33.000000 fleekapi-0.1.242/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 20:53:59.029730 fleekapi-0.2/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     1085 2024-05-19 13:25:10.000000 fleekapi-0.2/LICENCE
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2403 2024-05-20 20:53:59.029730 fleekapi-0.2/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     1491 2024-05-20 20:40:44.000000 fleekapi-0.2/README.md
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 20:53:59.025730 fleekapi-0.2/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       26 2024-05-19 13:15:32.000000 fleekapi-0.2/fleekapi/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3803 2024-05-20 20:51:08.000000 fleekapi-0.2/fleekapi/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      674 2024-05-19 13:15:32.000000 fleekapi-0.2/fleekapi/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      972 2024-05-19 13:15:32.000000 fleekapi-0.2/fleekapi/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 20:53:59.025730 fleekapi-0.2/fleekapi.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     2403 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      266 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-20 20:53:59.029730 fleekapi-0.2/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4001 2024-05-20 20:53:32.000000 fleekapi-0.2/setup.py
```

### Comparing `fleekapi-0.1.242/LICENCE` & `fleekapi-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.242/fleekapi/app.py` & `fleekapi-0.2/fleekapi/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
 import os.path
 
 import requests
 import wsgiadapter
-from icecream import ic
 from jinja2 import Environment, FileSystemLoader
 from parse import parse
 from webob import Request
 from whitenoise import WhiteNoise
 
 from .middleware import Middleware
 from .response import Response
@@ -45,15 +44,14 @@
 
         if handler_data is not None:
             handler = handler_data["handler"]
             allowed_methods = handler_data["allowed_methods"]
 
             if inspect.isclass(handler):
                 handler = getattr(handler(), request.method.lower(), None)
-                ic(handler)
 
                 if handler is None:
                     return self.method_not_allowed(response)
             else:
                 if request.method.lower() not in allowed_methods:
                     return self.method_not_allowed(response)
```

### Comparing `fleekapi-0.1.242/fleekapi/middleware.py` & `fleekapi-0.2/fleekapi/middleware.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.242/fleekapi/response.py` & `fleekapi-0.2/fleekapi/response.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.242/setup.py` & `fleekapi-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'fleekapi'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/FleekAPI'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.242'
+VERSION = '0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```


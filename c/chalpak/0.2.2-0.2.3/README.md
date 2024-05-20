# Comparing `tmp/chalpak-0.2.2.tar.gz` & `tmp/chalpak-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalpak-0.2.2.tar", last modified: Sun May 19 17:06:16 2024, max compression
+gzip compressed data, was "chalpak-0.2.3.tar", last modified: Sun May 19 17:12:37 2024, max compression
```

## Comparing `chalpak-0.2.2.tar` & `chalpak-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 17:06:16.715931 chalpak-0.2.2/
--rw-rw-rw-   0        0        0     1758 2024-05-19 17:06:16.714948 chalpak-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2024-05-19 17:02:15.000000 chalpak-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 17:06:16.665125 chalpak-0.2.2/chalpak/
--rw-rw-rw-   0        0        0       63 2024-05-19 16:04:44.000000 chalpak-0.2.2/chalpak/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-05-19 17:05:55.000000 chalpak-0.2.2/chalpak/app.py
--rw-rw-rw-   0        0        0     1419 2024-05-16 14:53:39.000000 chalpak-0.2.2/chalpak/exceptions.py
--rw-rw-rw-   0        0        0     1534 2024-05-19 16:01:52.000000 chalpak-0.2.2/chalpak/response.py
--rw-rw-rw-   0        0        0     1747 2024-05-19 17:06:08.000000 chalpak-0.2.2/chalpak/routes.py
--rw-rw-rw-   0        0        0      996 2024-05-16 14:56:23.000000 chalpak-0.2.2/chalpak/schema.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:06:16.679931 chalpak-0.2.2/chalpak.egg-info/
--rw-rw-rw-   0        0        0     1758 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 17:06:16.717281 chalpak-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     4023 2024-05-19 17:02:03.000000 chalpak-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:12:37.650246 chalpak-0.2.3/
+-rw-rw-rw-   0        0        0     1758 2024-05-19 17:12:37.647091 chalpak-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1103 2024-05-19 17:02:15.000000 chalpak-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 17:12:37.602562 chalpak-0.2.3/chalpak/
+-rw-rw-rw-   0        0        0       63 2024-05-19 16:04:44.000000 chalpak-0.2.3/chalpak/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-05-19 17:05:55.000000 chalpak-0.2.3/chalpak/app.py
+-rw-rw-rw-   0        0        0     1419 2024-05-16 14:53:39.000000 chalpak-0.2.3/chalpak/exceptions.py
+-rw-rw-rw-   0        0        0     1534 2024-05-19 16:01:52.000000 chalpak-0.2.3/chalpak/response.py
+-rw-rw-rw-   0        0        0     1747 2024-05-19 17:06:08.000000 chalpak-0.2.3/chalpak/routes.py
+-rw-rw-rw-   0        0        0      998 2024-05-19 17:11:34.000000 chalpak-0.2.3/chalpak/schema.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:12:37.644044 chalpak-0.2.3/chalpak.egg-info/
+-rw-rw-rw-   0        0        0     1758 2024-05-19 17:12:37.000000 chalpak-0.2.3/chalpak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-19 17:12:37.000000 chalpak-0.2.3/chalpak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:12:37.000000 chalpak-0.2.3/chalpak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-19 17:12:37.000000 chalpak-0.2.3/chalpak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 17:12:37.000000 chalpak-0.2.3/chalpak.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:12:37.650838 chalpak-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     4023 2024-05-19 17:12:30.000000 chalpak-0.2.3/setup.py
```

### Comparing `chalpak-0.2.2/PKG-INFO` & `chalpak-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalpak
-Version: 0.2.2
+Version: 0.2.3
 Summary: Chalpak - mini web framework like fastAPi, flask
 Home-page: https://github.com/me/myproject
 Author: Mehmonov Husniddin
 Author-email: mehmonov.husniddin1@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `chalpak-0.2.2/README.md` & `chalpak-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `chalpak-0.2.2/chalpak/app.py` & `chalpak-0.2.3/chalpak/app.py`

 * *Files identical despite different names*

### Comparing `chalpak-0.2.2/chalpak/exceptions.py` & `chalpak-0.2.3/chalpak/exceptions.py`

 * *Files identical despite different names*

### Comparing `chalpak-0.2.2/chalpak/response.py` & `chalpak-0.2.3/chalpak/response.py`

 * *Files identical despite different names*

### Comparing `chalpak-0.2.2/chalpak/routes.py` & `chalpak-0.2.3/chalpak/routes.py`

 * *Files identical despite different names*

### Comparing `chalpak-0.2.2/chalpak/schema.py` & `chalpak-0.2.3/chalpak/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from exceptions import APIError
-from response import JSONResponse
+from .exceptions import APIError
+from .response import JSONResponse
 
 
 class SchemaModel:
 
     def __init__(self, data: dict):
         self._parse_model(data)
```

### Comparing `chalpak-0.2.2/chalpak.egg-info/PKG-INFO` & `chalpak-0.2.3/chalpak.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalpak
-Version: 0.2.2
+Version: 0.2.3
 Summary: Chalpak - mini web framework like fastAPi, flask
 Home-page: https://github.com/me/myproject
 Author: Mehmonov Husniddin
 Author-email: mehmonov.husniddin1@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `chalpak-0.2.2/setup.py` & `chalpak-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'chalpak'
 DESCRIPTION = 'Chalpak - mini web framework like fastAPi, flask'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'mehmonov.husniddin1@gmail.com'
 AUTHOR = 'Mehmonov Husniddin'
 REQUIRES_PYTHON = '>=3.11.9'
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'aiohttp==3.9.5',
     'aiohttp-jinja2==1.6',
     'watchdog==4.0.0',
     'jurigged==0.5.7',
```


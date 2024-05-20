# Comparing `tmp/fleekapi-0.2.tar.gz` & `tmp/fleekapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.2.tar", last modified: Mon May 20 20:53:59 2024, max compression
+gzip compressed data, was "fleekapi-0.2.1.tar", last modified: Mon May 20 21:11:46 2024, max compression
```

## Comparing `fleekapi-0.2.tar` & `fleekapi-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 20:53:59.029730 fleekapi-0.2/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     1085 2024-05-19 13:25:10.000000 fleekapi-0.2/LICENCE
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2403 2024-05-20 20:53:59.029730 fleekapi-0.2/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     1491 2024-05-20 20:40:44.000000 fleekapi-0.2/README.md
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 20:53:59.025730 fleekapi-0.2/fleekapi/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       26 2024-05-19 13:15:32.000000 fleekapi-0.2/fleekapi/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3803 2024-05-20 20:51:08.000000 fleekapi-0.2/fleekapi/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      674 2024-05-19 13:15:32.000000 fleekapi-0.2/fleekapi/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      972 2024-05-19 13:15:32.000000 fleekapi-0.2/fleekapi/response.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 20:53:59.025730 fleekapi-0.2/fleekapi.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     2403 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      266 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-20 20:53:58.000000 fleekapi-0.2/fleekapi.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-20 20:53:59.029730 fleekapi-0.2/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     4001 2024-05-20 20:53:32.000000 fleekapi-0.2/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:11:46.722355 fleekapi-0.2.1/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)      928 2024-05-20 21:11:46.722355 fleekapi-0.2.1/PKG-INFO
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:11:46.718355 fleekapi-0.2.1/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       26 2024-05-19 13:15:32.000000 fleekapi-0.2.1/fleekapi/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3803 2024-05-20 20:51:08.000000 fleekapi-0.2.1/fleekapi/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      674 2024-05-19 13:15:32.000000 fleekapi-0.2.1/fleekapi/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      972 2024-05-19 13:15:32.000000 fleekapi-0.2.1/fleekapi/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-20 21:11:46.722355 fleekapi-0.2.1/fleekapi.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)      928 2024-05-20 21:11:46.000000 fleekapi-0.2.1/fleekapi.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      248 2024-05-20 21:11:46.000000 fleekapi-0.2.1/fleekapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-20 21:11:46.000000 fleekapi-0.2.1/fleekapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-20 21:11:46.000000 fleekapi-0.2.1/fleekapi.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-20 21:11:46.000000 fleekapi-0.2.1/fleekapi.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-20 21:11:46.722355 fleekapi-0.2.1/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4004 2024-05-20 21:11:38.000000 fleekapi-0.2.1/setup.py
```

### Comparing `fleekapi-0.2/fleekapi/app.py` & `fleekapi-0.2.1/fleekapi/app.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.2/fleekapi/middleware.py` & `fleekapi-0.2.1/fleekapi/middleware.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.2/fleekapi/response.py` & `fleekapi-0.2.1/fleekapi/response.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.2/setup.py` & `fleekapi-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'fleekapi'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/FleekAPI'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.2'
+VERSION = '0.2.01'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```


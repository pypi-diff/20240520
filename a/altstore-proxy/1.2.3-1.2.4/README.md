# Comparing `tmp/altstore_proxy-1.2.3.tar.gz` & `tmp/altstore_proxy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.2.3.tar", last modified: Sun May 19 18:42:51 2024, max compression
+gzip compressed data, was "altstore_proxy-1.2.4.tar", last modified: Sun May 19 19:05:33 2024, max compression
```

## Comparing `altstore_proxy-1.2.3.tar` & `altstore_proxy-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:05:33.342059 altstore_proxy-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 19:05:23.000000 altstore_proxy-1.2.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 19:05:33.342059 altstore_proxy-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-19 19:05:23.000000 altstore_proxy-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:05:33.342059 altstore_proxy-1.2.4/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:05:23.000000 altstore_proxy-1.2.4/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:05:33.342059 altstore_proxy-1.2.4/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:05:23.000000 altstore_proxy-1.2.4/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-19 19:05:23.000000 altstore_proxy-1.2.4/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-19 19:05:23.000000 altstore_proxy-1.2.4/altstore_proxy/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-19 19:05:23.000000 altstore_proxy-1.2.4/altstore_proxy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:05:33.342059 altstore_proxy-1.2.4/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 19:05:33.000000 altstore_proxy-1.2.4/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 19:05:33.000000 altstore_proxy-1.2.4/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:05:33.000000 altstore_proxy-1.2.4/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 19:05:33.000000 altstore_proxy-1.2.4/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:05:33.000000 altstore_proxy-1.2.4/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 19:05:33.000000 altstore_proxy-1.2.4/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 19:05:33.000000 altstore_proxy-1.2.4/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:05:33.342059 altstore_proxy-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-19 19:05:23.000000 altstore_proxy-1.2.4/setup.py
```

### Comparing `altstore_proxy-1.2.3/LICENSE.md` & `altstore_proxy-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.3/PKG-INFO` & `altstore_proxy-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore_proxy
-Version: 1.2.3
+Version: 1.2.4
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.2.3/README.md` & `altstore_proxy-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.3/altstore_proxy/providers/version.py` & `altstore_proxy-1.2.4/altstore_proxy/providers/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # AltStore-Proxy
 # Project by https://github.com/rix1337
 
 import re
 
 
 def get_version():
-    return "1.2.3"
+    return "1.2.4"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub(r'[^\d.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `altstore_proxy-1.2.3/altstore_proxy/run.py` & `altstore_proxy-1.2.4/altstore_proxy/run.py`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.3/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.2.4/altstore_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore-proxy
-Version: 1.2.3
+Version: 1.2.4
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.2.3/setup.py` & `altstore_proxy-1.2.4/setup.py`

 * *Files identical despite different names*


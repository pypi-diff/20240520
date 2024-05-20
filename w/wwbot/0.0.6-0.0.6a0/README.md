# Comparing `tmp/wwbot-0.0.6.tar.gz` & `tmp/wwbot-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwbot-0.0.6.tar", last modified: Mon May 20 01:07:19 2024, max compression
+gzip compressed data, was "wwbot-0.0.6a0.tar", last modified: Mon May 20 02:22:17 2024, max compression
```

## Comparing `wwbot-0.0.6.tar` & `wwbot-0.0.6a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-20 01:07:19.581056 wwbot-0.0.6/
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)      933 2024-05-20 01:07:19.580092 wwbot-0.0.6/PKG-INFO
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)       38 2024-05-20 01:07:19.581056 wwbot-0.0.6/setup.cfg
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)      949 2024-05-20 01:06:39.000000 wwbot-0.0.6/setup.py
-drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-20 01:07:19.557153 wwbot-0.0.6/wwbot/
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)    16313 2024-05-19 09:41:15.000000 wwbot-0.0.6/wwbot/__init__.py
-drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-20 01:07:19.577068 wwbot-0.0.6/wwbot/lib/
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)       53 2024-05-11 11:51:42.000000 wwbot-0.0.6/wwbot/lib/__init__.py
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)     4505 2024-05-20 01:05:40.000000 wwbot-0.0.6/wwbot/lib/logger.py
-drwxrwxrwx   0 uleo      (1000) uleo      (1000)        0 2024-05-20 01:07:19.570087 wwbot-0.0.6/wwbot.egg-info/
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)      933 2024-05-20 01:07:19.000000 wwbot-0.0.6/wwbot.egg-info/PKG-INFO
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)      184 2024-05-20 01:07:19.000000 wwbot-0.0.6/wwbot.egg-info/SOURCES.txt
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)        1 2024-05-20 01:07:19.000000 wwbot-0.0.6/wwbot.egg-info/dependency_links.txt
--rwxrwxrwx   0 uleo      (1000) uleo      (1000)        6 2024-05-20 01:07:19.000000 wwbot-0.0.6/wwbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 02:22:09.000000 wwbot-0.0.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/wwbot/
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-05-20 02:22:09.000000 wwbot-0.0.6a0/wwbot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/wwbot/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 02:22:09.000000 wwbot-0.0.6a0/wwbot/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 02:22:09.000000 wwbot-0.0.6a0/wwbot/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/wwbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 02:22:17.000000 wwbot-0.0.6a0/wwbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 02:22:17.000000 wwbot-0.0.6a0/wwbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:22:17.000000 wwbot-0.0.6a0/wwbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 02:22:17.000000 wwbot-0.0.6a0/wwbot.egg-info/top_level.txt
```

### Comparing `wwbot-0.0.6/PKG-INFO` & `wwbot-0.0.6a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
 
-UNKNOWN
 
+Please refer to the homepage of the library
```

### Comparing `wwbot-0.0.6/wwbot/__init__.py` & `wwbot-0.0.6a0/wwbot/__init__.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.6/wwbot/lib/logger.py` & `wwbot-0.0.6a0/wwbot/lib/logger.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.6/wwbot.egg-info/PKG-INFO` & `wwbot-0.0.6a0/wwbot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
 
-UNKNOWN
 
+Please refer to the homepage of the library
```


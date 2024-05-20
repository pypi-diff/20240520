# Comparing `tmp/wwbot-0.0.6a0.tar.gz` & `tmp/wwbot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwbot-0.0.6a0.tar", last modified: Mon May 20 02:22:17 2024, max compression
+gzip compressed data, was "wwbot-0.0.7.tar", last modified: Mon May 20 02:43:32 2024, max compression
```

## Comparing `wwbot-0.0.6a0.tar` & `wwbot-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 02:22:09.000000 wwbot-0.0.6a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/wwbot/
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-05-20 02:22:09.000000 wwbot-0.0.6a0/wwbot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/wwbot/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 02:22:09.000000 wwbot-0.0.6a0/wwbot/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 02:22:09.000000 wwbot-0.0.6a0/wwbot/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:22:17.640107 wwbot-0.0.6a0/wwbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 02:22:17.000000 wwbot-0.0.6a0/wwbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 02:22:17.000000 wwbot-0.0.6a0/wwbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:22:17.000000 wwbot-0.0.6a0/wwbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 02:22:17.000000 wwbot-0.0.6a0/wwbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:43:32.185217 wwbot-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 02:43:32.185217 wwbot-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:43:32.185217 wwbot-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 02:43:24.000000 wwbot-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:43:32.181217 wwbot-0.0.7/wwbot/
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-05-20 02:43:24.000000 wwbot-0.0.7/wwbot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:43:32.185217 wwbot-0.0.7/wwbot/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 02:43:24.000000 wwbot-0.0.7/wwbot/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 02:43:24.000000 wwbot-0.0.7/wwbot/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:43:32.185217 wwbot-0.0.7/wwbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 02:43:32.000000 wwbot-0.0.7/wwbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 02:43:32.000000 wwbot-0.0.7/wwbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:43:32.000000 wwbot-0.0.7/wwbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 02:43:32.000000 wwbot-0.0.7/wwbot.egg-info/top_level.txt
```

### Comparing `wwbot-0.0.6a0/PKG-INFO` & `wwbot-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.6a0
+Version: 0.0.7
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```

### Comparing `wwbot-0.0.6a0/setup.py` & `wwbot-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = '''
 Please refer to the homepage of the library
 '''
 
 setuptools.setup(
   name="wwbot",
-  version="0.0.6a",
+  version="0.0.7",
   author="tbbatbb",
   author_email="20682299+tbbatbb@users.noreply.github.com",
   description="A library for dealing with messages in WeWork",
   url="https://github.com/tbbatbb/WeWorkBot",
   long_description_content_type='text/markdown',
   long_description=long_description,
   packages=setuptools.find_packages(),
```

### Comparing `wwbot-0.0.6a0/wwbot/__init__.py` & `wwbot-0.0.7/wwbot/__init__.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.6a0/wwbot/lib/logger.py` & `wwbot-0.0.7/wwbot/lib/logger.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.6a0/wwbot.egg-info/PKG-INFO` & `wwbot-0.0.7/wwbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.6a0
+Version: 0.0.7
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```


# Comparing `tmp/wwbot-0.0.7.tar.gz` & `tmp/wwbot-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwbot-0.0.7.tar", last modified: Mon May 20 02:43:32 2024, max compression
+gzip compressed data, was "wwbot-0.0.8a0.tar", last modified: Mon May 20 13:26:05 2024, max compression
```

## Comparing `wwbot-0.0.7.tar` & `wwbot-0.0.8a0.tar`

### file list

```diff
@@ -1,14 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:43:32.185217 wwbot-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 02:43:32.185217 wwbot-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:43:32.185217 wwbot-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 02:43:24.000000 wwbot-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:43:32.181217 wwbot-0.0.7/wwbot/
--rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-05-20 02:43:24.000000 wwbot-0.0.7/wwbot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:43:32.185217 wwbot-0.0.7/wwbot/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 02:43:24.000000 wwbot-0.0.7/wwbot/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 02:43:24.000000 wwbot-0.0.7/wwbot/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:43:32.185217 wwbot-0.0.7/wwbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 02:43:32.000000 wwbot-0.0.7/wwbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 02:43:32.000000 wwbot-0.0.7/wwbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:43:32.000000 wwbot-0.0.7/wwbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 02:43:32.000000 wwbot-0.0.7/wwbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.176415 wwbot-0.0.8a0/wwbot/
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.176415 wwbot-0.0.8a0/wwbot/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/wwbot/msg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/file_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/image_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/link_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/location_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/markdown_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/mpnews_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/news_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/text_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/textcard_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/video_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/voice_msg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/wwbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 13:26:05.000000 wwbot-0.0.8a0/wwbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-20 13:26:05.000000 wwbot-0.0.8a0/wwbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:26:05.000000 wwbot-0.0.8a0/wwbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:26:05.000000 wwbot-0.0.8a0/wwbot.egg-info/top_level.txt
```

### Comparing `wwbot-0.0.7/PKG-INFO` & `wwbot-0.0.8a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.7
+Version: 0.0.8a0
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```

### Comparing `wwbot-0.0.7/setup.py` & `wwbot-0.0.8a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = '''
 Please refer to the homepage of the library
 '''
 
 setuptools.setup(
   name="wwbot",
-  version="0.0.7",
+  version="0.0.8a",
   author="tbbatbb",
   author_email="20682299+tbbatbb@users.noreply.github.com",
   description="A library for dealing with messages in WeWork",
   url="https://github.com/tbbatbb/WeWorkBot",
   long_description_content_type='text/markdown',
   long_description=long_description,
   packages=setuptools.find_packages(),
```

### Comparing `wwbot-0.0.7/wwbot/lib/logger.py` & `wwbot-0.0.8a0/wwbot/lib/logger.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.7/wwbot.egg-info/PKG-INFO` & `wwbot-0.0.8a0/wwbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.7
+Version: 0.0.8a0
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```


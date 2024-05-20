# Comparing `tmp/wwbot-0.0.8a0.tar.gz` & `tmp/wwbot-0.0.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwbot-0.0.8a0.tar", last modified: Mon May 20 13:26:05 2024, max compression
+gzip compressed data, was "wwbot-0.0.8b0.tar", last modified: Mon May 20 13:39:40 2024, max compression
```

## Comparing `wwbot-0.0.8a0.tar` & `wwbot-0.0.8b0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.176415 wwbot-0.0.8a0/wwbot/
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.176415 wwbot-0.0.8a0/wwbot/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/wwbot/msg/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/file_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/image_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/link_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/location_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/markdown_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/mpnews_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/news_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/text_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/textcard_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/video_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-20 13:25:59.000000 wwbot-0.0.8a0/wwbot/msg/voice_msg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:26:05.180415 wwbot-0.0.8a0/wwbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 13:26:05.000000 wwbot-0.0.8a0/wwbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-20 13:26:05.000000 wwbot-0.0.8a0/wwbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:26:05.000000 wwbot-0.0.8a0/wwbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:26:05.000000 wwbot-0.0.8a0/wwbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:39:40.743242 wwbot-0.0.8b0/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 13:39:40.743242 wwbot-0.0.8b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:39:40.743242 wwbot-0.0.8b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:39:40.739242 wwbot-0.0.8b0/wwbot/
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:39:40.739242 wwbot-0.0.8b0/wwbot/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:39:40.743242 wwbot-0.0.8b0/wwbot/msg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/file_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/image_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/link_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/location_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/markdown_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/mpnews_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/news_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/text_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/textcard_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/video_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-20 13:39:36.000000 wwbot-0.0.8b0/wwbot/msg/voice_msg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:39:40.743242 wwbot-0.0.8b0/wwbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 13:39:40.000000 wwbot-0.0.8b0/wwbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-20 13:39:40.000000 wwbot-0.0.8b0/wwbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:39:40.000000 wwbot-0.0.8b0/wwbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:39:40.000000 wwbot-0.0.8b0/wwbot.egg-info/top_level.txt
```

### Comparing `wwbot-0.0.8a0/PKG-INFO` & `wwbot-0.0.8b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.8a0
+Version: 0.0.8b0
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```

### Comparing `wwbot-0.0.8a0/setup.py` & `wwbot-0.0.8b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = '''
 Please refer to the homepage of the library
 '''
 
 setuptools.setup(
   name="wwbot",
-  version="0.0.8a",
+  version="0.0.8b",
   author="tbbatbb",
   author_email="20682299+tbbatbb@users.noreply.github.com",
   description="A library for dealing with messages in WeWork",
   url="https://github.com/tbbatbb/WeWorkBot",
   long_description_content_type='text/markdown',
   long_description=long_description,
   packages=setuptools.find_packages(),
```

### Comparing `wwbot-0.0.8a0/wwbot/__init__.py` & `wwbot-0.0.8b0/wwbot/__init__.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/lib/logger.py` & `wwbot-0.0.8b0/wwbot/lib/logger.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/__init__.py` & `wwbot-0.0.8b0/wwbot/msg/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         pass
 
     @abstractmethod
     def to_json(self) -> str:
         '''Represent the message in JSON format'''
         pass
 
-    @abstractmethod
     @classmethod
+    @abstractmethod
     def from_xml(cls, xml_tree:Element):
         '''Parse different types of messages from XML object'''
         pass 
 
 
 from .text_msg import TextMessage
 from .link_msg import LinkMessage
```

### Comparing `wwbot-0.0.8a0/wwbot/msg/file_msg.py` & `wwbot-0.0.8b0/wwbot/msg/file_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/image_msg.py` & `wwbot-0.0.8b0/wwbot/msg/image_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/link_msg.py` & `wwbot-0.0.8b0/wwbot/msg/link_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/location_msg.py` & `wwbot-0.0.8b0/wwbot/msg/location_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/markdown_msg.py` & `wwbot-0.0.8b0/wwbot/msg/markdown_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/mpnews_msg.py` & `wwbot-0.0.8b0/wwbot/msg/mpnews_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/news_msg.py` & `wwbot-0.0.8b0/wwbot/msg/news_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/text_msg.py` & `wwbot-0.0.8b0/wwbot/msg/text_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/textcard_msg.py` & `wwbot-0.0.8b0/wwbot/msg/textcard_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/video_msg.py` & `wwbot-0.0.8b0/wwbot/msg/video_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot/msg/voice_msg.py` & `wwbot-0.0.8b0/wwbot/msg/voice_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8a0/wwbot.egg-info/PKG-INFO` & `wwbot-0.0.8b0/wwbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.8a0
+Version: 0.0.8b0
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```


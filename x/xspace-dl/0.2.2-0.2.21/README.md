# Comparing `tmp/xspace-dl-0.2.2.tar.gz` & `tmp/xspace-dl-0.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.2.2.tar", last modified: Mon May 20 14:21:30 2024, max compression
+gzip compressed data, was "xspace-dl-0.2.21.tar", last modified: Mon May 20 14:27:12 2024, max compression
```

## Comparing `xspace-dl-0.2.2.tar` & `xspace-dl-0.2.21.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:21:30.901268 xspace-dl-0.2.2/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 14:21:30.901008 xspace-dl-0.2.2/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 14:21:30.901387 xspace-dl-0.2.2/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      855 2024-05-20 14:21:27.000000 xspace-dl-0.2.2/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:21:30.897761 xspace-dl-0.2.2/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:11:45.000000 xspace-dl-0.2.2/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7416 2024-05-20 14:20:51.000000 xspace-dl-0.2.2/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6084 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7061 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:21:30.900358 xspace-dl-0.2.2/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:27:12.661127 xspace-dl-0.2.21/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 14:27:12.660943 xspace-dl-0.2.21/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 14:27:12.661182 xspace-dl-0.2.21/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 14:26:57.000000 xspace-dl-0.2.21/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:27:12.659506 xspace-dl-0.2.21/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      174 2024-05-20 14:24:16.000000 xspace-dl-0.2.21/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7416 2024-05-20 14:23:45.000000 xspace-dl-0.2.21/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6083 2024-05-20 14:23:58.000000 xspace-dl-0.2.21/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7075 2024-05-20 14:26:09.000000 xspace-dl-0.2.21/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:27:12.660713 xspace-dl-0.2.21/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.2.2/LICENSE` & `xspace-dl-0.2.21/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.2/PKG-INFO` & `xspace-dl-0.2.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.2
+Version: 0.2.21
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/rosebabaganoush/xspace-dl
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.2 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.21 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```

### Comparing `xspace-dl-0.2.2/README.md` & `xspace-dl-0.2.21/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.2/pyproject.toml` & `xspace-dl-0.2.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.2/setup.py` & `xspace-dl-0.2.21/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',
-    version='0.2.2',
+    version='0.2.21',
     author='Your Name',
     author_email='your.email@example.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rosebabaganoush/xspace-dl',
     packages=find_packages(),
```

### Comparing `xspace-dl-0.2.2/xspace/api.py` & `xspace-dl-0.2.21/xspace/api.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.2/xspace/cookies.py` & `xspace-dl-0.2.21/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.2/xspace/main.py` & `xspace-dl-0.2.21/xspace/main.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.2/xspace/xspace.py` & `xspace-dl-0.2.21/xspace/xspace.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Provide an interface with twitter spaces"""
+# xspace/xspace.py
+
 import json
 import logging
 import os
 import re
 from collections import defaultdict
 from datetime import datetime
 
 from .api import API
 
-
-class Twspace(dict):
+class Xspace(dict):  # Ensure the class name is Xspace
     """Downloader class for twitter spaces"""
 
     def __init__(self, metadata: dict) -> None:
         dict.__init__(
             self,
             {
                 "id": "",
@@ -82,15 +82,15 @@
 
         # Remove null byte
         value = value.replace("\0", "")
 
         # If the filename starts with a . prepend it with an underscore, so it
         # doesn't become hidden
         if value.startswith("."):
-            value = "_" + value
+            value = "_"+value
 
         # platform.system docs say it could also return "Windows" or "Java".
         # Failsafe and use Windows sanitisation for Java, as it could be any
         # operating system.
         blacklist = r"\/:*?\"<>|"
 
         # Replace every blacklisted character with a underscore
@@ -122,52 +122,52 @@
             "LPT5",
             "LPT6",
             "LPT7",
             "LPT8",
             "LPT9",
         ]
         if value in invalid_filenames:
-            value = "_" + value
+            value = "_"+value
 
         return value + extension
 
     def format(self, format_str: str) -> str:
         """Use metadata to fill in the fields in format str"""
         actual_format_str = os.path.basename(format_str)
         abs_dir = os.path.dirname(format_str) % self
         basename = self.sterilize_fn(actual_format_str % self)
         return os.path.join(abs_dir, basename)
 
     @classmethod
     def from_space_url(cls, url: str):
-        """Create a Twspace instance from a space url"""
+        """Create a Xspace instance from a space url"""
         try:
             space_id = re.findall(r"(?<=spaces/)\w*", url)[0]
         except IndexError as err:
             raise ValueError(
                 (
                     "Input URL is not valid.\n"
                     "The URL format should 'https://twitter.com/i/spaces/<space_id>'"
                 )
             ) from err
         return cls(cls._metadata(space_id))
 
     @classmethod
     def from_user_avatar(cls, user_url: str):
-        """Create a Twspace instance from a twitter user's ongoing space"""
+        """Create a Xspace instance from a twitter user's ongoing space"""
         user_id = API.graphql_api.user_id_from_url(user_url)
         avatar_content = API.fleets_api.avatar_content(user_id)
         try:
             broadcast_id = avatar_content["users"][user_id]["spaces"]["live_content"][
                 "audiospace"
             ]["broadcast_id"]
         except KeyError as err:
             raise ValueError(
                 "Broadcast ID is not available.\nUser is probably not live"
             ) from err
         return cls(cls._metadata(broadcast_id))
 
     @classmethod
     def from_file(cls, path: str):
-        """Create a Twspace instance from a metadata file"""
+        """Create a Xspace instance from a metadata file"""
         with open(path, "r", encoding="utf-8") as metadata_io:
             return cls(json.load(metadata_io))
```

### Comparing `xspace-dl-0.2.2/xspace/xspace_dl.py` & `xspace-dl-0.2.21/xspace/xspace_dl.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import tempfile
 from functools import cached_property
 from urllib.parse import urlparse
 
 from mutagen.mp4 import MP4, MP4Cover
 
 from .api import API
-from .twspace import Twspace
+from .xspace import Xspace  # Updated import
 
 DEFAULT_FNAME_FORMAT = "(%(creator_name)s)%(title)s-%(id)s"
 MP4_COVER_FORMAT_MAP = {"jpg": MP4Cover.FORMAT_JPEG, "png": MP4Cover.FORMAT_PNG}
 
 
-class TwspaceDL:
+class XspaceDL:
     """Downloader class for twitter spaces"""
 
-    def __init__(self, space: Twspace, format_str: str) -> None:
+    def __init__(self, space: Xspace, format_str: str) -> None:
         self.space = space
         self.format_str = format_str or DEFAULT_FNAME_FORMAT
         self._tempdir = ""
 
     @cached_property
     def filename(self) -> str:
         """Returns the formatted filename"""
```

### Comparing `xspace-dl-0.2.2/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.2.21/xspace_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.2
+Version: 0.2.21
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/rosebabaganoush/xspace-dl
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.2 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.21 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```


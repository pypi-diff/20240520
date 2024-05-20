# Comparing `tmp/xspace-dl-0.2.21.tar.gz` & `tmp/xspace-dl-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.2.21.tar", last modified: Mon May 20 14:27:12 2024, max compression
+gzip compressed data, was "xspace-dl-0.2.22.tar", last modified: Mon May 20 14:42:03 2024, max compression
```

## Comparing `xspace-dl-0.2.21.tar` & `xspace-dl-0.2.22.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:27:12.661127 xspace-dl-0.2.21/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 14:27:12.660943 xspace-dl-0.2.21/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 14:27:12.661182 xspace-dl-0.2.21/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 14:26:57.000000 xspace-dl-0.2.21/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:27:12.659506 xspace-dl-0.2.21/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      174 2024-05-20 14:24:16.000000 xspace-dl-0.2.21/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.21/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7416 2024-05-20 14:23:45.000000 xspace-dl-0.2.21/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6083 2024-05-20 14:23:58.000000 xspace-dl-0.2.21/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7075 2024-05-20 14:26:09.000000 xspace-dl-0.2.21/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:27:12.660713 xspace-dl-0.2.21/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 14:27:12.000000 xspace-dl-0.2.21/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:42:03.059161 xspace-dl-0.2.22/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 14:42:03.058979 xspace-dl-0.2.22/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 14:42:03.059211 xspace-dl-0.2.22/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 14:41:29.000000 xspace-dl-0.2.22/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:42:03.057649 xspace-dl-0.2.22/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.2.22/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7359 2024-05-20 14:37:45.000000 xspace-dl-0.2.22/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6083 2024-05-20 14:39:00.000000 xspace-dl-0.2.22/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7074 2024-05-20 14:38:05.000000 xspace-dl-0.2.22/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:42:03.058755 xspace-dl-0.2.22/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 14:42:03.000000 xspace-dl-0.2.22/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.2.21/LICENSE` & `xspace-dl-0.2.22/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.21/PKG-INFO` & `xspace-dl-0.2.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.21
+Version: 0.2.22
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
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.21 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.22 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```

### Comparing `xspace-dl-0.2.21/README.md` & `xspace-dl-0.2.22/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.21/pyproject.toml` & `xspace-dl-0.2.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.21/setup.py` & `xspace-dl-0.2.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',
-    version='0.2.21',
+    version='0.2.22',
     author='Your Name',
     author_email='your.email@example.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rosebabaganoush/xspace-dl',
     packages=find_packages(),
```

### Comparing `xspace-dl-0.2.21/xspace/api.py` & `xspace-dl-0.2.22/xspace/api.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.21/xspace/cookies.py` & `xspace-dl-0.2.22/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.21/xspace/main.py` & `xspace-dl-0.2.22/xspace/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-"""Script designed to help download twitter spaces"""
 import argparse
 import datetime
 import json
 import logging
 import sys
 from types import TracebackType
 from typing import Optional, Type
@@ -12,25 +11,23 @@
 from xspace.xspace import Xspace
 from xspace.xspace_dl import XspaceDL
 
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_ERROR = 1
 EXIT_CODE_MISUSE = 2
 
-
 def exception_hook(
     _: Type[BaseException],
     exc_value: BaseException,
     _t: TracebackType = None,
 ) -> None:
     """Make Exceptions more legible for the end users"""
     # Exception type and value
     print(f"\033[31;1;4mError\033[0m: {exc_value}\nRetry with -v to see more details")
 
-
 def space(args: argparse.Namespace) -> int:
     """Manage the twitter space related function"""
     has_input = (
         args.user_url
         or args.input_url
         or args.input_metadata
         or args.from_dynamic_url
@@ -110,15 +107,14 @@
         except KeyboardInterrupt:
             logging.info("Download Interrupted by user")
         finally:
             if not args.keep_files:
                 xspace_dl.cleanup()
     return EXIT_CODE_SUCCESS
 
-
 def main() -> int:
     """Main function, creates the argument parser"""
     parser = argparse.ArgumentParser(
         description="Script designed to help download twitter spaces"
     )
 
     input_group = parser.add_argument_group("input")
```

### Comparing `xspace-dl-0.2.21/xspace/xspace.py` & `xspace-dl-0.2.22/xspace/xspace.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.21/xspace/xspace_dl.py` & `xspace-dl-0.2.22/xspace/xspace_dl.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from .api import API
 from .xspace import Xspace  # Updated import
 
 DEFAULT_FNAME_FORMAT = "(%(creator_name)s)%(title)s-%(id)s"
 MP4_COVER_FORMAT_MAP = {"jpg": MP4Cover.FORMAT_JPEG, "png": MP4Cover.FORMAT_PNG}
 
-
 class XspaceDL:
     """Downloader class for twitter spaces"""
 
     def __init__(self, space: Xspace, format_str: str) -> None:
         self.space = space
         self.format_str = format_str or DEFAULT_FNAME_FORMAT
         self._tempdir = ""
```

### Comparing `xspace-dl-0.2.21/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.2.22/xspace_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.21
+Version: 0.2.22
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
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.21 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.22 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```


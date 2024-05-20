# Comparing `tmp/xspace-dl-0.1.22.tar.gz` & `tmp/xspace-dl-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.1.22.tar", last modified: Mon May 20 12:58:54 2024, max compression
+gzip compressed data, was "xspace-dl-0.1.23.tar", last modified: Mon May 20 13:03:50 2024, max compression
```

## Comparing `xspace-dl-0.1.22.tar` & `xspace-dl-0.1.23.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:58:54.709654 xspace-dl-0.1.22/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.22/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 12:58:54.709357 xspace-dl-0.1.22/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4104 2024-05-20 12:44:30.000000 xspace-dl-0.1.22/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1082 2024-05-20 12:44:30.000000 xspace-dl-0.1.22/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 12:58:54.709730 xspace-dl-0.1.22/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      980 2024-05-20 12:58:50.000000 xspace-dl-0.1.22/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:58:54.707608 xspace-dl-0.1.22/xspace_dl/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 12:44:30.000000 xspace-dl-0.1.22/xspace_dl/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7364 2024-05-20 12:51:13.000000 xspace-dl-0.1.22/xspace_dl/__main__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16813 2024-05-20 12:44:42.000000 xspace-dl-0.1.22/xspace_dl/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.22/xspace_dl/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6068 2024-05-20 12:48:38.000000 xspace-dl-0.1.22/xspace_dl/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7057 2024-05-20 12:44:30.000000 xspace-dl-0.1.22/xspace_dl/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:58:54.709048 xspace-dl-0.1.22/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      366 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       10 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:03:50.170250 xspace-dl-0.1.23/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.23/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 13:03:50.170072 xspace-dl-0.1.23/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4104 2024-05-20 12:44:30.000000 xspace-dl-0.1.23/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1082 2024-05-20 12:44:30.000000 xspace-dl-0.1.23/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 13:03:50.170296 xspace-dl-0.1.23/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      980 2024-05-20 13:03:15.000000 xspace-dl-0.1.23/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:03:50.168891 xspace-dl-0.1.23/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 12:44:30.000000 xspace-dl-0.1.23/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7352 2024-05-20 13:01:32.000000 xspace-dl-0.1.23/xspace/__main__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16813 2024-05-20 12:44:42.000000 xspace-dl-0.1.23/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.23/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6068 2024-05-20 12:48:38.000000 xspace-dl-0.1.23/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7057 2024-05-20 12:44:30.000000 xspace-dl-0.1.23/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:03:50.169867 xspace-dl-0.1.23/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 13:03:50.000000 xspace-dl-0.1.23/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      348 2024-05-20 13:03:50.000000 xspace-dl-0.1.23/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 13:03:50.000000 xspace-dl-0.1.23/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 13:03:50.000000 xspace-dl-0.1.23/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 13:03:50.000000 xspace-dl-0.1.23/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 13:03:50.000000 xspace-dl-0.1.23/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.1.22/LICENSE` & `xspace-dl-0.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.22/PKG-INFO` & `xspace-dl-0.1.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.1.22
+Version: 0.1.23
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/RoseBabaganoush/xspace-dl
 Author: RoseBabaGanoush
 Author-email: hello@rosebabaganoush.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `xspace-dl-0.1.22/README.md` & `xspace-dl-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.22/pyproject.toml` & `xspace-dl-0.1.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.22/setup.py` & `xspace-dl-0.1.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',  # Updated package name
-    version='0.1.22',  # Increment the version number
+    version='0.1.23',  # Increment the version number
     author='RoseBabaGanoush',
     author_email='hello@rosebabaganoush.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/RoseBabaganoush/xspace-dl',  # Update with your repository URL
     packages=find_packages(),
```

### Comparing `xspace-dl-0.1.22/xspace_dl/__main__.py` & `xspace-dl-0.1.23/xspace/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import datetime
 import json
 import logging
 import sys
 from types import TracebackType
 from typing import Optional, Type
 
-from xspace_dl.api import API
-from xspace_dl.cookies import load_cookies
-from xspace_dl.xspace import xspace
-from xspace_dl.xspace_dl import xspaceDL
+from xspace.api import API
+from xspace.cookies import load_cookies
+from xspace.xspace import xspace
+from xspace.xspace_dl import xspaceDL
 
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_ERROR = 1
 EXIT_CODE_MISUSE = 2
 
 
 def exception_hook(
```

### Comparing `xspace-dl-0.1.22/xspace_dl/api.py` & `xspace-dl-0.1.23/xspace/api.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.22/xspace_dl/cookies.py` & `xspace-dl-0.1.23/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.22/xspace_dl/xspace.py` & `xspace-dl-0.1.23/xspace/xspace.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.22/xspace_dl/xspace_dl.py` & `xspace-dl-0.1.23/xspace/xspace_dl.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.22/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.1.23/xspace_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.1.22
+Version: 0.1.23
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/RoseBabaganoush/xspace-dl
 Author: RoseBabaGanoush
 Author-email: hello@rosebabaganoush.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```


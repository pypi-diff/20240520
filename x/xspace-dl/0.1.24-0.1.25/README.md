# Comparing `tmp/xspace-dl-0.1.24.tar.gz` & `tmp/xspace-dl-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.1.24.tar", last modified: Mon May 20 13:08:49 2024, max compression
+gzip compressed data, was "xspace-dl-0.1.25.tar", last modified: Mon May 20 13:15:38 2024, max compression
```

## Comparing `xspace-dl-0.1.24.tar` & `xspace-dl-0.1.25.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:08:49.984430 xspace-dl-0.1.24/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.24/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 13:08:49.984255 xspace-dl-0.1.24/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4104 2024-05-20 12:44:30.000000 xspace-dl-0.1.24/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1082 2024-05-20 12:44:30.000000 xspace-dl-0.1.24/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 13:08:49.984481 xspace-dl-0.1.24/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      980 2024-05-20 13:08:38.000000 xspace-dl-0.1.24/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:08:49.982932 xspace-dl-0.1.24/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 12:44:30.000000 xspace-dl-0.1.24/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16813 2024-05-20 12:44:42.000000 xspace-dl-0.1.24/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.24/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7352 2024-05-20 13:01:32.000000 xspace-dl-0.1.24/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6068 2024-05-20 12:48:38.000000 xspace-dl-0.1.24/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7057 2024-05-20 12:44:30.000000 xspace-dl-0.1.24/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:08:49.984021 xspace-dl-0.1.24/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 13:08:49.000000 xspace-dl-0.1.24/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 13:08:49.000000 xspace-dl-0.1.24/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 13:08:49.000000 xspace-dl-0.1.24/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 13:08:49.000000 xspace-dl-0.1.24/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 13:08:49.000000 xspace-dl-0.1.24/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 13:08:49.000000 xspace-dl-0.1.24/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:15:38.958950 xspace-dl-0.1.25/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.25/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 13:15:38.958761 xspace-dl-0.1.25/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4104 2024-05-20 12:44:30.000000 xspace-dl-0.1.25/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1082 2024-05-20 12:44:30.000000 xspace-dl-0.1.25/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 13:15:38.959000 xspace-dl-0.1.25/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      980 2024-05-20 13:15:26.000000 xspace-dl-0.1.25/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:15:38.957403 xspace-dl-0.1.25/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:14:45.000000 xspace-dl-0.1.25/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16813 2024-05-20 12:44:42.000000 xspace-dl-0.1.25/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.25/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7352 2024-05-20 13:01:32.000000 xspace-dl-0.1.25/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6068 2024-05-20 12:48:38.000000 xspace-dl-0.1.25/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7057 2024-05-20 12:44:30.000000 xspace-dl-0.1.25/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:15:38.958526 xspace-dl-0.1.25/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.1.24/LICENSE` & `xspace-dl-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.24/PKG-INFO` & `xspace-dl-0.1.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.1.24
+Version: 0.1.25
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/RoseBabaganoush/xspace-dl
 Author: RoseBabaGanoush
 Author-email: hello@rosebabaganoush.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `xspace-dl-0.1.24/README.md` & `xspace-dl-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.24/pyproject.toml` & `xspace-dl-0.1.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.24/setup.py` & `xspace-dl-0.1.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',  # Updated package name
-    version='0.1.24',  # Increment the version number
+    version='0.1.25',  # Increment the version number
     author='RoseBabaGanoush',
     author_email='hello@rosebabaganoush.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/RoseBabaganoush/xspace-dl',  # Update with your repository URL
     packages=find_packages(),
```

### Comparing `xspace-dl-0.1.24/xspace/api.py` & `xspace-dl-0.1.25/xspace/api.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.24/xspace/cookies.py` & `xspace-dl-0.1.25/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.24/xspace/main.py` & `xspace-dl-0.1.25/xspace/main.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.24/xspace/xspace.py` & `xspace-dl-0.1.25/xspace/xspace.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.24/xspace/xspace_dl.py` & `xspace-dl-0.1.25/xspace/xspace_dl.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.24/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.1.25/xspace_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.1.24
+Version: 0.1.25
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/RoseBabaganoush/xspace-dl
 Author: RoseBabaGanoush
 Author-email: hello@rosebabaganoush.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```


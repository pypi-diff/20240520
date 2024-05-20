# Comparing `tmp/xspace-dl-0.1.21.tar.gz` & `tmp/xspace-dl-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.1.21.tar", last modified: Mon May 20 12:51:33 2024, max compression
+gzip compressed data, was "xspace-dl-0.1.22.tar", last modified: Mon May 20 12:58:54 2024, max compression
```

## Comparing `xspace-dl-0.1.21.tar` & `xspace-dl-0.1.22.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:51:33.007001 xspace-dl-0.1.21/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.21/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 12:51:33.006764 xspace-dl-0.1.21/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4104 2024-05-20 12:44:30.000000 xspace-dl-0.1.21/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1082 2024-05-20 12:44:30.000000 xspace-dl-0.1.21/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 12:51:33.007075 xspace-dl-0.1.21/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      963 2024-05-20 12:51:24.000000 xspace-dl-0.1.21/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:51:33.005253 xspace-dl-0.1.21/xspace_dl/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 12:44:30.000000 xspace-dl-0.1.21/xspace_dl/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7364 2024-05-20 12:51:13.000000 xspace-dl-0.1.21/xspace_dl/__main__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16813 2024-05-20 12:44:42.000000 xspace-dl-0.1.21/xspace_dl/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.21/xspace_dl/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6068 2024-05-20 12:48:38.000000 xspace-dl-0.1.21/xspace_dl/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7057 2024-05-20 12:44:30.000000 xspace-dl-0.1.21/xspace_dl/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:51:33.006493 xspace-dl-0.1.21/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 12:51:32.000000 xspace-dl-0.1.21/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      366 2024-05-20 12:51:32.000000 xspace-dl-0.1.21/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 12:51:32.000000 xspace-dl-0.1.21/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 12:51:32.000000 xspace-dl-0.1.21/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        9 2024-05-20 12:51:32.000000 xspace-dl-0.1.21/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       10 2024-05-20 12:51:32.000000 xspace-dl-0.1.21/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:58:54.709654 xspace-dl-0.1.22/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.22/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 12:58:54.709357 xspace-dl-0.1.22/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4104 2024-05-20 12:44:30.000000 xspace-dl-0.1.22/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1082 2024-05-20 12:44:30.000000 xspace-dl-0.1.22/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 12:58:54.709730 xspace-dl-0.1.22/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      980 2024-05-20 12:58:50.000000 xspace-dl-0.1.22/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:58:54.707608 xspace-dl-0.1.22/xspace_dl/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 12:44:30.000000 xspace-dl-0.1.22/xspace_dl/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7364 2024-05-20 12:51:13.000000 xspace-dl-0.1.22/xspace_dl/__main__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16813 2024-05-20 12:44:42.000000 xspace-dl-0.1.22/xspace_dl/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.22/xspace_dl/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6068 2024-05-20 12:48:38.000000 xspace-dl-0.1.22/xspace_dl/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7057 2024-05-20 12:44:30.000000 xspace-dl-0.1.22/xspace_dl/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:58:54.709048 xspace-dl-0.1.22/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      366 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       10 2024-05-20 12:58:54.000000 xspace-dl-0.1.22/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.1.21/LICENSE` & `xspace-dl-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.21/PKG-INFO` & `xspace-dl-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.1.21
+Version: 0.1.22
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/RoseBabaganoush/xspace-dl
 Author: RoseBabaGanoush
 Author-email: hello@rosebabaganoush.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `xspace-dl-0.1.21/README.md` & `xspace-dl-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.21/pyproject.toml` & `xspace-dl-0.1.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.21/setup.py` & `xspace-dl-0.1.22/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',  # Updated package name
-    version='0.1.21',  # Increment the version number
+    version='0.1.22',  # Increment the version number
     author='RoseBabaGanoush',
     author_email='hello@rosebabaganoush.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/RoseBabaganoush/xspace-dl',  # Update with your repository URL
     packages=find_packages(),
     install_requires=[
-        'requests',  # Add other dependencies if any
+        'requests',
+        'mutagen',  # Add mutagen to dependencies
     ],
     entry_points={
         'console_scripts': [
             'xspace-dl=xspace.main:main',  # Adjust as per your CLI entry point
         ],
     },
     classifiers=[
```

### Comparing `xspace-dl-0.1.21/xspace_dl/__main__.py` & `xspace-dl-0.1.22/xspace_dl/__main__.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.21/xspace_dl/api.py` & `xspace-dl-0.1.22/xspace_dl/api.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.21/xspace_dl/cookies.py` & `xspace-dl-0.1.22/xspace_dl/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.21/xspace_dl/xspace.py` & `xspace-dl-0.1.22/xspace_dl/xspace.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.21/xspace_dl/xspace_dl.py` & `xspace-dl-0.1.22/xspace_dl/xspace_dl.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.21/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.1.22/xspace_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.1.21
+Version: 0.1.22
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/RoseBabaganoush/xspace-dl
 Author: RoseBabaGanoush
 Author-email: hello@rosebabaganoush.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```


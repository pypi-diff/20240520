# Comparing `tmp/unique_colorlogger-0.1.0.tar.gz` & `tmp/unique_colorlogger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unique_colorlogger-0.1.0.tar", last modified: Mon May 20 15:59:55 2024, max compression
+gzip compressed data, was "unique_colorlogger-0.1.1.tar", last modified: Mon May 20 16:07:40 2024, max compression
```

## Comparing `unique_colorlogger-0.1.0.tar` & `unique_colorlogger-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 15:59:55.242008 unique_colorlogger-0.1.0/
--rw-rw-rw-   0        0        0     1085 2024-05-20 15:21:41.000000 unique_colorlogger-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3446 2024-05-20 15:59:55.240827 unique_colorlogger-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2535 2024-05-20 15:21:41.000000 unique_colorlogger-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 15:59:55.223043 unique_colorlogger-0.1.0/pycolorlogger/
--rw-rw-rw-   0        0        0       26 2024-05-20 15:28:32.000000 unique_colorlogger-0.1.0/pycolorlogger/__init__.py
--rw-rw-rw-   0        0        0     2418 2024-05-20 15:36:18.000000 unique_colorlogger-0.1.0/pycolorlogger/logger.py
--rw-rw-rw-   0        0        0       42 2024-05-20 15:59:55.242008 unique_colorlogger-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1264 2024-05-20 15:59:19.000000 unique_colorlogger-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 15:59:55.239496 unique_colorlogger-0.1.0/unique_colorlogger.egg-info/
--rw-rw-rw-   0        0        0     3446 2024-05-20 15:59:55.000000 unique_colorlogger-0.1.0/unique_colorlogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-20 15:59:55.000000 unique_colorlogger-0.1.0/unique_colorlogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 15:59:55.000000 unique_colorlogger-0.1.0/unique_colorlogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-20 15:58:58.000000 unique_colorlogger-0.1.0/unique_colorlogger.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-05-20 15:59:55.000000 unique_colorlogger-0.1.0/unique_colorlogger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 16:07:40.630277 unique_colorlogger-0.1.1/
+-rw-rw-rw-   0        0        0     1085 2024-05-20 15:21:41.000000 unique_colorlogger-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3446 2024-05-20 16:07:40.628513 unique_colorlogger-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2535 2024-05-20 15:21:41.000000 unique_colorlogger-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 16:07:40.630277 unique_colorlogger-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2024-05-20 16:06:48.000000 unique_colorlogger-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:07:40.619351 unique_colorlogger-0.1.1/unique_colorlogger/
+-rw-rw-rw-   0        0        0       26 2024-05-20 15:28:32.000000 unique_colorlogger-0.1.1/unique_colorlogger/__init__.py
+-rw-rw-rw-   0        0        0     2418 2024-05-20 15:36:18.000000 unique_colorlogger-0.1.1/unique_colorlogger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:07:40.628513 unique_colorlogger-0.1.1/unique_colorlogger.egg-info/
+-rw-rw-rw-   0        0        0     3446 2024-05-20 16:07:40.000000 unique_colorlogger-0.1.1/unique_colorlogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2024-05-20 16:07:40.000000 unique_colorlogger-0.1.1/unique_colorlogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 16:07:40.000000 unique_colorlogger-0.1.1/unique_colorlogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-20 15:58:58.000000 unique_colorlogger-0.1.1/unique_colorlogger.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2024-05-20 16:07:40.000000 unique_colorlogger-0.1.1/unique_colorlogger.egg-info/top_level.txt
```

### Comparing `unique_colorlogger-0.1.0/LICENSE` & `unique_colorlogger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_colorlogger-0.1.0/PKG-INFO` & `unique_colorlogger-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique-colorlogger
-Version: 0.1.0
+Version: 0.1.1
 Summary: A colorful logging utility for Python applications
 Home-page: https://github.com/idkconsole/ColorLogger
 Author: console
 Author-email: idkconsole@proton.me
 Keywords: logging logger color logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `unique_colorlogger-0.1.0/README.md` & `unique_colorlogger-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unique_colorlogger-0.1.0/pycolorlogger/logger.py` & `unique_colorlogger-0.1.1/unique_colorlogger/logger.py`

 * *Files identical despite different names*

### Comparing `unique_colorlogger-0.1.0/setup.py` & `unique_colorlogger-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='unique-colorlogger',
-    version='0.1.0',
+    version='0.1.1',
     author='console',
     author_email='idkconsole@proton.me',
     description='A colorful logging utility for Python applications',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/idkconsole/ColorLogger',
     packages=find_packages(),
```

### Comparing `unique_colorlogger-0.1.0/unique_colorlogger.egg-info/PKG-INFO` & `unique_colorlogger-0.1.1/unique_colorlogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique-colorlogger
-Version: 0.1.0
+Version: 0.1.1
 Summary: A colorful logging utility for Python applications
 Home-page: https://github.com/idkconsole/ColorLogger
 Author: console
 Author-email: idkconsole@proton.me
 Keywords: logging logger color logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


# Comparing `tmp/mongodriver-1.2.7.tar.gz` & `tmp/mongodriver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.2.7.tar", last modified: Mon May 20 00:32:36 2024, max compression
+gzip compressed data, was "mongodriver-1.3.0.tar", last modified: Mon May 20 00:33:26 2024, max compression
```

## Comparing `mongodriver-1.2.7.tar` & `mongodriver-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:32:36.938899 mongodriver-1.2.7/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.2.7/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)     3451 2024-05-20 00:32:36.938615 mongodriver-1.2.7/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.2.7/README.md
--rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.2.7/pyproject.toml
--rw-r--r--   0 jstrouse   (501) staff       (20)       38 2024-05-20 00:32:36.938976 mongodriver-1.2.7/setup.cfg
--rw-r--r--   0 jstrouse   (501) staff       (20)      952 2024-05-20 00:25:59.000000 mongodriver-1.2.7/setup.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:32:36.934786 mongodriver-1.2.7/src/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:32:36.936588 mongodriver-1.2.7/src/mongodriver/
--rw-r--r--   0 jstrouse   (501) staff       (20)      181 2024-05-20 00:25:59.000000 mongodriver-1.2.7/src/mongodriver/__init__.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     8287 2024-05-20 00:21:38.000000 mongodriver-1.2.7/src/mongodriver/async_mongodriver.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     8086 2023-08-01 14:46:22.000000 mongodriver-1.2.7/src/mongodriver/mongodriver.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:32:36.938159 mongodriver-1.2.7/src/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)     3451 2024-05-20 00:32:36.000000 mongodriver-1.2.7/src/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      331 2024-05-20 00:32:36.000000 mongodriver-1.2.7/src/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:32:36.000000 mongodriver-1.2.7/src/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       68 2024-05-20 00:32:36.000000 mongodriver-1.2.7/src/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       12 2024-05-20 00:32:36.000000 mongodriver-1.2.7/src/mongodriver.egg-info/top_level.txt
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:33:26.417924 mongodriver-1.3.0/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.3.0/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3451 2024-05-20 00:33:26.417645 mongodriver-1.3.0/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.3.0/README.md
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.3.0/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)       38 2024-05-20 00:33:26.417991 mongodriver-1.3.0/setup.cfg
+-rw-r--r--   0 jstrouse   (501) staff       (20)      952 2024-05-20 00:33:22.000000 mongodriver-1.3.0/setup.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:33:26.414212 mongodriver-1.3.0/src/
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:33:26.415888 mongodriver-1.3.0/src/mongodriver/
+-rw-r--r--   0 jstrouse   (501) staff       (20)      181 2024-05-20 00:33:22.000000 mongodriver-1.3.0/src/mongodriver/__init__.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     8287 2024-05-20 00:21:38.000000 mongodriver-1.3.0/src/mongodriver/async_mongodriver.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     8086 2023-08-01 14:46:22.000000 mongodriver-1.3.0/src/mongodriver/mongodriver.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:33:26.417314 mongodriver-1.3.0/src/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3451 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      331 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       68 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       12 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/top_level.txt
```

### Comparing `mongodriver-1.2.7/LICENSE` & `mongodriver-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.7/PKG-INFO` & `mongodriver-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.2.7
+Version: 1.3.0
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mongodriver-1.2.7/README.md` & `mongodriver-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.7/setup.py` & `mongodriver-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Get the long description from the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mongodriver',
-    version='1.2.7',
+    version='1.3.0',
     license='MIT',
     author="Jake Strouse",
     author_email='jstrouse@meh.llc',
     packages=find_packages('src'),
     url='https://github.com/jakestrouse00/mongodriver',
     package_dir={'': 'src'},
     keywords='mongodb',
```

### Comparing `mongodriver-1.2.7/src/mongodriver/async_mongodriver.py` & `mongodriver-1.3.0/src/mongodriver/async_mongodriver.py`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.7/src/mongodriver/mongodriver.py` & `mongodriver-1.3.0/src/mongodriver/mongodriver.py`

 * *Files identical despite different names*

### Comparing `mongodriver-1.2.7/src/mongodriver.egg-info/PKG-INFO` & `mongodriver-1.3.0/src/mongodriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.2.7
+Version: 1.3.0
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
```


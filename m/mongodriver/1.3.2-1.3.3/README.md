# Comparing `tmp/mongodriver-1.3.2.tar.gz` & `tmp/mongodriver-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.3.2.tar", last modified: Mon May 20 00:45:54 2024, max compression
+gzip compressed data, was "mongodriver-1.3.3.tar", last modified: Mon May 20 00:50:06 2024, max compression
```

## Comparing `mongodriver-1.3.2.tar` & `mongodriver-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:45:54.185618 mongodriver-1.3.2/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.3.2/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)     3429 2024-05-20 00:45:54.185324 mongodriver-1.3.2/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2824 2024-05-20 00:45:50.000000 mongodriver-1.3.2/README.md
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:45:54.182539 mongodriver-1.3.2/mongodriver/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:45:54.184991 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)     3429 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      275 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       66 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/top_level.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.3.2/pyproject.toml
--rw-r--r--   0 jstrouse   (501) staff       (20)       38 2024-05-20 00:45:54.185692 mongodriver-1.3.2/setup.cfg
--rw-r--r--   0 jstrouse   (501) staff       (20)      966 2024-05-20 00:45:50.000000 mongodriver-1.3.2/setup.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:50:06.669202 mongodriver-1.3.3/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.3.3/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3429 2024-05-20 00:50:06.669033 mongodriver-1.3.3/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2824 2024-05-20 00:45:50.000000 mongodriver-1.3.3/README.md
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:50:06.667785 mongodriver-1.3.3/mongodriver/
+-rw-r--r--   0 jstrouse   (501) staff       (20)      181 2024-05-20 00:50:04.000000 mongodriver-1.3.3/mongodriver/__init__.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     8287 2024-05-20 00:21:38.000000 mongodriver-1.3.3/mongodriver/async_mongodriver.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     8086 2023-08-01 14:46:22.000000 mongodriver-1.3.3/mongodriver/mongodriver.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:50:06.668835 mongodriver-1.3.3/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3429 2024-05-20 00:50:06.000000 mongodriver-1.3.3/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      299 2024-05-20 00:50:06.000000 mongodriver-1.3.3/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:50:06.000000 mongodriver-1.3.3/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       66 2024-05-20 00:50:06.000000 mongodriver-1.3.3/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       12 2024-05-20 00:50:06.000000 mongodriver-1.3.3/mongodriver.egg-info/top_level.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.3.3/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)       38 2024-05-20 00:50:06.669246 mongodriver-1.3.3/setup.cfg
+-rw-r--r--   0 jstrouse   (501) staff       (20)      916 2024-05-20 00:50:04.000000 mongodriver-1.3.3/setup.py
```

### Comparing `mongodriver-1.3.2/LICENSE` & `mongodriver-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.3.2/PKG-INFO` & `mongodriver-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.3.2
+Version: 1.3.3
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mongodriver-1.3.2/README.md` & `mongodriver-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `mongodriver-1.3.2/mongodriver/mongodriver.egg-info/PKG-INFO` & `mongodriver-1.3.3/mongodriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.3.2
+Version: 1.3.3
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mongodriver-1.3.2/setup.py` & `mongodriver-1.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 # Get the long description from the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mongodriver',
-    version='1.3.2',
+    version='1.3.3',
     license='MIT',
     author="Jake Strouse",
     author_email='jstrouse@meh.llc',
-    packages=find_packages('mongodriver'),
+    packages=find_packages(),
     url='https://github.com/jakestrouse00/mongodriver',
-    package_dir={'': 'mongodriver'},
     keywords='mongodb',
     install_requires=[
         'pymongo==4.4.1',
         'pymongo[srv]==4.4.1',
         'motor==3.2.0',
         'motor[srv]==3.2.0'
     ],
```


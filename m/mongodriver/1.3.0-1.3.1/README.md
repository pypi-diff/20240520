# Comparing `tmp/mongodriver-1.3.0.tar.gz` & `tmp/mongodriver-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.3.0.tar", last modified: Mon May 20 00:33:26 2024, max compression
+gzip compressed data, was "mongodriver-1.3.1.tar", last modified: Mon May 20 00:40:57 2024, max compression
```

## Comparing `mongodriver-1.3.0.tar` & `mongodriver-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:33:26.417924 mongodriver-1.3.0/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.3.0/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)     3451 2024-05-20 00:33:26.417645 mongodriver-1.3.0/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.3.0/README.md
--rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.3.0/pyproject.toml
--rw-r--r--   0 jstrouse   (501) staff       (20)       38 2024-05-20 00:33:26.417991 mongodriver-1.3.0/setup.cfg
--rw-r--r--   0 jstrouse   (501) staff       (20)      952 2024-05-20 00:33:22.000000 mongodriver-1.3.0/setup.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:33:26.414212 mongodriver-1.3.0/src/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:33:26.415888 mongodriver-1.3.0/src/mongodriver/
--rw-r--r--   0 jstrouse   (501) staff       (20)      181 2024-05-20 00:33:22.000000 mongodriver-1.3.0/src/mongodriver/__init__.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     8287 2024-05-20 00:21:38.000000 mongodriver-1.3.0/src/mongodriver/async_mongodriver.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     8086 2023-08-01 14:46:22.000000 mongodriver-1.3.0/src/mongodriver/mongodriver.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:33:26.417314 mongodriver-1.3.0/src/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)     3451 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      331 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       68 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       12 2024-05-20 00:33:26.000000 mongodriver-1.3.0/src/mongodriver.egg-info/top_level.txt
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:40:57.502430 mongodriver-1.3.1/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.3.1/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3449 2024-05-20 00:40:57.502124 mongodriver-1.3.1/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.3.1/README.md
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.3.1/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)       38 2024-05-20 00:40:57.502514 mongodriver-1.3.1/setup.cfg
+-rw-r--r--   0 jstrouse   (501) staff       (20)      950 2024-05-20 00:40:52.000000 mongodriver-1.3.1/setup.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:40:57.498151 mongodriver-1.3.1/src/
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:40:57.500072 mongodriver-1.3.1/src/mongodriver/
+-rw-r--r--   0 jstrouse   (501) staff       (20)      181 2024-05-20 00:40:52.000000 mongodriver-1.3.1/src/mongodriver/__init__.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     8287 2024-05-20 00:21:38.000000 mongodriver-1.3.1/src/mongodriver/async_mongodriver.py
+-rw-r--r--   0 jstrouse   (501) staff       (20)     8086 2023-08-01 14:46:22.000000 mongodriver-1.3.1/src/mongodriver/mongodriver.py
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:40:57.501772 mongodriver-1.3.1/src/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3449 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      331 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       66 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       12 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/top_level.txt
```

### Comparing `mongodriver-1.3.0/LICENSE` & `mongodriver-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.3.0/PKG-INFO` & `mongodriver-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.3.0
+Version: 1.3.1
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pymongo==3.12.0
-Requires-Dist: pymongo[srv]==3.12.0
+Requires-Dist: pymongo==4.4.1
+Requires-Dist: pymongo[srv]==4.4.1
 Requires-Dist: motor==3.2.0
 Requires-Dist: motor[srv]==3.2.0
 
 # MongoDriver
 
 An object-oriented package for interacting with MongoDB documents
```

### Comparing `mongodriver-1.3.0/README.md` & `mongodriver-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mongodriver-1.3.0/setup.py` & `mongodriver-1.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 # Get the long description from the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mongodriver',
-    version='1.3.0',
+    version='1.3.1',
     license='MIT',
     author="Jake Strouse",
     author_email='jstrouse@meh.llc',
     packages=find_packages('src'),
     url='https://github.com/jakestrouse00/mongodriver',
     package_dir={'': 'src'},
     keywords='mongodb',
     install_requires=[
-        'pymongo==3.12.0',
-        'pymongo[srv]==3.12.0',
+        'pymongo==4.4.1',
+        'pymongo[srv]==4.4.1',
         'motor==3.2.0',
         'motor[srv]==3.2.0'
     ],
     description='Object-oriented interactions with MongoDB',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `mongodriver-1.3.0/src/mongodriver/async_mongodriver.py` & `mongodriver-1.3.1/src/mongodriver/async_mongodriver.py`

 * *Files identical despite different names*

### Comparing `mongodriver-1.3.0/src/mongodriver/mongodriver.py` & `mongodriver-1.3.1/src/mongodriver/mongodriver.py`

 * *Files identical despite different names*

### Comparing `mongodriver-1.3.0/src/mongodriver.egg-info/PKG-INFO` & `mongodriver-1.3.1/src/mongodriver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.3.0
+Version: 1.3.1
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pymongo==3.12.0
-Requires-Dist: pymongo[srv]==3.12.0
+Requires-Dist: pymongo==4.4.1
+Requires-Dist: pymongo[srv]==4.4.1
 Requires-Dist: motor==3.2.0
 Requires-Dist: motor[srv]==3.2.0
 
 # MongoDriver
 
 An object-oriented package for interacting with MongoDB documents
```


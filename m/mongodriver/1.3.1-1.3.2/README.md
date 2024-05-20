# Comparing `tmp/mongodriver-1.3.1.tar.gz` & `tmp/mongodriver-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodriver-1.3.1.tar", last modified: Mon May 20 00:40:57 2024, max compression
+gzip compressed data, was "mongodriver-1.3.2.tar", last modified: Mon May 20 00:45:54 2024, max compression
```

## Comparing `mongodriver-1.3.1.tar` & `mongodriver-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:40:57.502430 mongodriver-1.3.1/
--rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.3.1/LICENSE
--rw-r--r--   0 jstrouse   (501) staff       (20)     3449 2024-05-20 00:40:57.502124 mongodriver-1.3.1/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)     2844 2023-07-20 15:38:01.000000 mongodriver-1.3.1/README.md
--rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.3.1/pyproject.toml
--rw-r--r--   0 jstrouse   (501) staff       (20)       38 2024-05-20 00:40:57.502514 mongodriver-1.3.1/setup.cfg
--rw-r--r--   0 jstrouse   (501) staff       (20)      950 2024-05-20 00:40:52.000000 mongodriver-1.3.1/setup.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:40:57.498151 mongodriver-1.3.1/src/
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:40:57.500072 mongodriver-1.3.1/src/mongodriver/
--rw-r--r--   0 jstrouse   (501) staff       (20)      181 2024-05-20 00:40:52.000000 mongodriver-1.3.1/src/mongodriver/__init__.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     8287 2024-05-20 00:21:38.000000 mongodriver-1.3.1/src/mongodriver/async_mongodriver.py
--rw-r--r--   0 jstrouse   (501) staff       (20)     8086 2023-08-01 14:46:22.000000 mongodriver-1.3.1/src/mongodriver/mongodriver.py
-drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:40:57.501772 mongodriver-1.3.1/src/mongodriver.egg-info/
--rw-r--r--   0 jstrouse   (501) staff       (20)     3449 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/PKG-INFO
--rw-r--r--   0 jstrouse   (501) staff       (20)      331 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/SOURCES.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/dependency_links.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       66 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/requires.txt
--rw-r--r--   0 jstrouse   (501) staff       (20)       12 2024-05-20 00:40:57.000000 mongodriver-1.3.1/src/mongodriver.egg-info/top_level.txt
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:45:54.185618 mongodriver-1.3.2/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     1061 2022-08-27 03:52:41.000000 mongodriver-1.3.2/LICENSE
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3429 2024-05-20 00:45:54.185324 mongodriver-1.3.2/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)     2824 2024-05-20 00:45:50.000000 mongodriver-1.3.2/README.md
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:45:54.182539 mongodriver-1.3.2/mongodriver/
+drwxr-xr-x   0 jstrouse   (501) staff       (20)        0 2024-05-20 00:45:54.184991 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/
+-rw-r--r--   0 jstrouse   (501) staff       (20)     3429 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/PKG-INFO
+-rw-r--r--   0 jstrouse   (501) staff       (20)      275 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/SOURCES.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/dependency_links.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       66 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/requires.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)        1 2024-05-20 00:45:54.000000 mongodriver-1.3.2/mongodriver/mongodriver.egg-info/top_level.txt
+-rw-r--r--   0 jstrouse   (501) staff       (20)       80 2023-07-20 15:31:35.000000 mongodriver-1.3.2/pyproject.toml
+-rw-r--r--   0 jstrouse   (501) staff       (20)       38 2024-05-20 00:45:54.185692 mongodriver-1.3.2/setup.cfg
+-rw-r--r--   0 jstrouse   (501) staff       (20)      966 2024-05-20 00:45:50.000000 mongodriver-1.3.2/setup.py
```

### Comparing `mongodriver-1.3.1/LICENSE` & `mongodriver-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodriver-1.3.1/PKG-INFO` & `mongodriver-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.3.1
+Version: 1.3.2
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
@@ -38,27 +38,27 @@
 Quickstart
 ----------
 
 Install MongoDriver
 `python3 -m pip install mongodriver`
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 ```
    
 Examples
 ----------
 Here is a basic example on how to create a new document and then interact it
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 new_document = driver.create({"foo": 1, "bar": 2})
 
@@ -75,44 +75,44 @@
 
 print(new_document.foo)  # 3
 ```
 
 Find a document
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 search_query = {"foo": 1}
 documents = driver.find(search_query)  # returns a list of documents
 for document in documents:
     print(document)
 ```
 
 Load all documents from MongoDB into Document objects
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 documents = driver.load()  # loads all documents from db into local Document objects
 for document in documents:
     print(document)
 ```
 
 Add more keys into a document
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 json_document = {"foo": 1, "bar": 2}
 new_document = driver.create(json_document)
```

### Comparing `mongodriver-1.3.1/README.md` & `mongodriver-1.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 Quickstart
 ----------
 
 Install MongoDriver
 `python3 -m pip install mongodriver`
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 ```
    
 Examples
 ----------
 Here is a basic example on how to create a new document and then interact it
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 new_document = driver.create({"foo": 1, "bar": 2})
 
@@ -55,44 +55,44 @@
 
 print(new_document.foo)  # 3
 ```
 
 Find a document
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 search_query = {"foo": 1}
 documents = driver.find(search_query)  # returns a list of documents
 for document in documents:
     print(document)
 ```
 
 Load all documents from MongoDB into Document objects
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 documents = driver.load()  # loads all documents from db into local Document objects
 for document in documents:
     print(document)
 ```
 
 Add more keys into a document
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 json_document = {"foo": 1, "bar": 2}
 new_document = driver.create(json_document)
```

### Comparing `mongodriver-1.3.1/setup.py` & `mongodriver-1.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 # Get the long description from the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='mongodriver',
-    version='1.3.1',
+    version='1.3.2',
     license='MIT',
     author="Jake Strouse",
     author_email='jstrouse@meh.llc',
-    packages=find_packages('src'),
+    packages=find_packages('mongodriver'),
     url='https://github.com/jakestrouse00/mongodriver',
-    package_dir={'': 'src'},
+    package_dir={'': 'mongodriver'},
     keywords='mongodb',
     install_requires=[
         'pymongo==4.4.1',
         'pymongo[srv]==4.4.1',
         'motor==3.2.0',
         'motor[srv]==3.2.0'
     ],
```

### Comparing `mongodriver-1.3.1/src/mongodriver.egg-info/PKG-INFO` & `mongodriver-1.3.2/mongodriver/mongodriver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodriver
-Version: 1.3.1
+Version: 1.3.2
 Summary: Object-oriented interactions with MongoDB
 Home-page: https://github.com/jakestrouse00/mongodriver
 Author: Jake Strouse
 Author-email: jstrouse@meh.llc
 License: MIT
 Keywords: mongodb
 Classifier: Programming Language :: Python :: 3
@@ -38,27 +38,27 @@
 Quickstart
 ----------
 
 Install MongoDriver
 `python3 -m pip install mongodriver`
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 ```
    
 Examples
 ----------
 Here is a basic example on how to create a new document and then interact it
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 new_document = driver.create({"foo": 1, "bar": 2})
 
@@ -75,44 +75,44 @@
 
 print(new_document.foo)  # 3
 ```
 
 Find a document
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 search_query = {"foo": 1}
 documents = driver.find(search_query)  # returns a list of documents
 for document in documents:
     print(document)
 ```
 
 Load all documents from MongoDB into Document objects
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 documents = driver.load()  # loads all documents from db into local Document objects
 for document in documents:
     print(document)
 ```
 
 Add more keys into a document
 
 ```python
-from mongodriver.src.mongodriver import Driver
+from mongodriver.mongodriver import Driver
 
 driver = Driver(
     connection_url="mongodb+srv://example:SecurePassword@testcluster.e2lhq.mongodb.net/myFirstDatabase?retryWrites=true&w=majority",
     db_name="example_db", collection_name="example_collection")
 
 json_document = {"foo": 1, "bar": 2}
 new_document = driver.create(json_document)
```


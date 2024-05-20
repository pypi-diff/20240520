# Comparing `tmp/simpleai_image-0.1.6.tar.gz` & `tmp/simpleai_image-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleai_image-0.1.6.tar", last modified: Mon May 20 19:03:05 2024, max compression
+gzip compressed data, was "simpleai_image-0.1.7.tar", last modified: Mon May 20 19:09:06 2024, max compression
```

## Comparing `simpleai_image-0.1.6.tar` & `simpleai_image-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:03:05.105821 simpleai_image-0.1.6/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      927 2024-05-20 19:03:05.105547 simpleai_image-0.1.6/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 simpleai_image-0.1.6/README.md
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:03:05.104011 simpleai_image-0.1.6/SimpleAI_Image/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 simpleai_image-0.1.6/SimpleAI_Image/DataProcessor.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 simpleai_image-0.1.6/SimpleAI_Image/DatabaseHandler.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       86 2024-05-20 18:07:54.000000 simpleai_image-0.1.6/SimpleAI_Image/__init__.py
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:03:05.105201 simpleai_image-0.1.6/SimpleAI_Image.egg-info/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      927 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      318 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      129 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/requires.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       21 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/top_level.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 19:03:05.105885 simpleai_image-0.1.6/setup.cfg
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      921 2024-05-20 19:01:37.000000 simpleai_image-0.1.6/setup.py
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:03:05.104971 simpleai_image-0.1.6/tests/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 simpleai_image-0.1.6/tests/__init__.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:09:06.154734 simpleai_image-0.1.7/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      951 2024-05-20 19:09:06.154372 simpleai_image-0.1.7/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 simpleai_image-0.1.7/README.md
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:09:06.152790 simpleai_image-0.1.7/SimpleAI_Image/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 simpleai_image-0.1.7/SimpleAI_Image/DataProcessor.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 simpleai_image-0.1.7/SimpleAI_Image/DatabaseHandler.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       86 2024-05-20 18:07:54.000000 simpleai_image-0.1.7/SimpleAI_Image/__init__.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:09:06.153977 simpleai_image-0.1.7/SimpleAI_Image.egg-info/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      951 2024-05-20 19:09:06.000000 simpleai_image-0.1.7/SimpleAI_Image.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      318 2024-05-20 19:09:06.000000 simpleai_image-0.1.7/SimpleAI_Image.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 19:09:06.000000 simpleai_image-0.1.7/SimpleAI_Image.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      138 2024-05-20 19:09:06.000000 simpleai_image-0.1.7/SimpleAI_Image.egg-info/requires.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       21 2024-05-20 19:09:06.000000 simpleai_image-0.1.7/SimpleAI_Image.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 19:09:06.154801 simpleai_image-0.1.7/setup.cfg
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      957 2024-05-20 19:07:01.000000 simpleai_image-0.1.7/setup.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:09:06.153745 simpleai_image-0.1.7/tests/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 simpleai_image-0.1.7/tests/__init__.py
```

### Comparing `simpleai_image-0.1.6/PKG-INFO` & `simpleai_image-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleAI_Image
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for processing and storing image vectors in PostgreSQL
 Home-page: https://github.com/Tobias2408/bachelorprojekt
 Author: Tobias Poulsen
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Requires-Dist: tensorflow-macos
 Requires-Dist: tensorflow-datasets
 Requires-Dist: tensorflow-metal
 Requires-Dist: scikit-learn
 Requires-Dist: requests
 Requires-Dist: keras
 Requires-Dist: tensorboard
+Requires-Dist: pgvector
 
 # SimpleAI_Image
 
 A package for processing and storing image vectors in PostgreSQL.
 
 ## Installation
```

### Comparing `simpleai_image-0.1.6/SimpleAI_Image/DataProcessor.py` & `simpleai_image-0.1.7/SimpleAI_Image/DataProcessor.py`

 * *Files identical despite different names*

### Comparing `simpleai_image-0.1.6/SimpleAI_Image/DatabaseHandler.py` & `simpleai_image-0.1.7/SimpleAI_Image/DatabaseHandler.py`

 * *Files identical despite different names*

### Comparing `simpleai_image-0.1.6/SimpleAI_Image.egg-info/PKG-INFO` & `simpleai_image-0.1.7/SimpleAI_Image.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleAI_Image
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for processing and storing image vectors in PostgreSQL
 Home-page: https://github.com/Tobias2408/bachelorprojekt
 Author: Tobias Poulsen
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Requires-Dist: tensorflow-macos
 Requires-Dist: tensorflow-datasets
 Requires-Dist: tensorflow-metal
 Requires-Dist: scikit-learn
 Requires-Dist: requests
 Requires-Dist: keras
 Requires-Dist: tensorboard
+Requires-Dist: pgvector
 
 # SimpleAI_Image
 
 A package for processing and storing image vectors in PostgreSQL.
 
 ## Installation
```

### Comparing `simpleai_image-0.1.6/setup.py` & `simpleai_image-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SimpleAI_Image',
-    version='0.1.6',
+    version='0.1.7',
     description='A package for processing and storing image vectors in PostgreSQL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Tobias Poulsen',
     author_email='your.email@example.com',
     url='https://github.com/Tobias2408/bachelorprojekt',
     packages=find_packages(),
@@ -18,14 +18,15 @@
         'tensorflow-macos',
         'tensorflow-datasets',
         'tensorflow-metal',
         'scikit-learn',
         'requests',
         'keras',
         'tensorboard',
+        'pgvector'  # Add this line
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```


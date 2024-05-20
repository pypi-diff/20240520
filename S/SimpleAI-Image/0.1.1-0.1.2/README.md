# Comparing `tmp/SimpleAI_Image-0.1.1.tar.gz` & `tmp/SimpleAI_Image-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleAI_Image-0.1.1.tar", last modified: Mon May 20 16:38:07 2024, max compression
+gzip compressed data, was "SimpleAI_Image-0.1.2.tar", last modified: Mon May 20 18:05:21 2024, max compression
```

## Comparing `SimpleAI_Image-0.1.1.tar` & `SimpleAI_Image-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 16:38:07.908950 SimpleAI_Image-0.1.1/
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 16:38:07.907599 SimpleAI_Image-0.1.1/ImageAI/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 SimpleAI_Image-0.1.1/ImageAI/DataProcessor.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 SimpleAI_Image-0.1.1/ImageAI/DatabaseHandler.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:25:09.000000 SimpleAI_Image-0.1.1/ImageAI/__init__.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 16:38:07.908778 SimpleAI_Image-0.1.1/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 SimpleAI_Image-0.1.1/README.md
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 16:38:07.908359 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      297 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      178 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/requires.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       14 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/top_level.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 16:38:07.909008 SimpleAI_Image-0.1.1/setup.cfg
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1034 2024-05-20 16:35:54.000000 SimpleAI_Image-0.1.1/setup.py
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 16:38:07.908527 SimpleAI_Image-0.1.1/tests/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 SimpleAI_Image-0.1.1/tests/__init__.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:05:21.908446 SimpleAI_Image-0.1.2/
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:05:21.907003 SimpleAI_Image-0.1.2/ImageAI/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 SimpleAI_Image-0.1.2/ImageAI/DataProcessor.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 SimpleAI_Image-0.1.2/ImageAI/DatabaseHandler.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:25:09.000000 SimpleAI_Image-0.1.2/ImageAI/__init__.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 18:05:21.908260 SimpleAI_Image-0.1.2/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 SimpleAI_Image-0.1.2/README.md
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:05:21.907873 SimpleAI_Image-0.1.2/SimpleAI_Image.egg-info/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 18:05:21.000000 SimpleAI_Image-0.1.2/SimpleAI_Image.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      297 2024-05-20 18:05:21.000000 SimpleAI_Image-0.1.2/SimpleAI_Image.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 18:05:21.000000 SimpleAI_Image-0.1.2/SimpleAI_Image.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      211 2024-05-20 18:05:21.000000 SimpleAI_Image-0.1.2/SimpleAI_Image.egg-info/requires.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       14 2024-05-20 18:05:21.000000 SimpleAI_Image-0.1.2/SimpleAI_Image.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 18:05:21.908505 SimpleAI_Image-0.1.2/setup.cfg
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1252 2024-05-20 18:05:12.000000 SimpleAI_Image-0.1.2/setup.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:05:21.908049 SimpleAI_Image-0.1.2/tests/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 SimpleAI_Image-0.1.2/tests/__init__.py
```

### Comparing `SimpleAI_Image-0.1.1/ImageAI/DataProcessor.py` & `SimpleAI_Image-0.1.2/ImageAI/DataProcessor.py`

 * *Files identical despite different names*

### Comparing `SimpleAI_Image-0.1.1/ImageAI/DatabaseHandler.py` & `SimpleAI_Image-0.1.2/ImageAI/DatabaseHandler.py`

 * *Files identical despite different names*

### Comparing `SimpleAI_Image-0.1.1/PKG-INFO` & `SimpleAI_Image-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleAI_Image
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for processing and storing image vectors in PostgreSQL
 Home-page: https://github.com/Tobias2408/bachelorprojekt
 Author: Tobias Poulsen
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/PKG-INFO` & `SimpleAI_Image-0.1.2/SimpleAI_Image.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleAI-Image
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for processing and storing image vectors in PostgreSQL
 Home-page: https://github.com/Tobias2408/bachelorprojekt
 Author: Tobias Poulsen
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SimpleAI_Image-0.1.1/setup.py` & `SimpleAI_Image-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SimpleAI_Image',  # Change this to a unique name
-    version='0.1.1',  # Increment the version number
+    version='0.1.2',  # Increment the version number
     description='A package for processing and storing image vectors in PostgreSQL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Tobias Poulsen',
     author_email='your.email@example.com',
     url='https://github.com/Tobias2408/bachelorprojekt',  # Your package's URL
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'pandas==1.5.3',
         'sqlalchemy==2.0.30',
         'matplotlib==3.6.3',
-        'tensorflow-macos==2.12.0',
+        'tensorflow-macos==2.16.1',
         'tensorflow-datasets==4.9.2',
         'tensorflow-metal==0.8.0',
         'scikit-learn==1.2.2',
-        'requests==2.28.2',
+        'requests==2.31.0',  # Update to the latest version compatible with other packages
+        'keras==3.0.0',  # Update to be compatible with tensorflow 2.16.1
+        'tensorboard==2.16.0',  # Update to be compatible with tensorflow 2.16.1
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```

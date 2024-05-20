# Comparing `tmp/SimpleAI_Image-0.1.0.tar.gz` & `tmp/SimpleAI_Image-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleAI_Image-0.1.0.tar", last modified: Mon May 20 15:44:51 2024, max compression
+gzip compressed data, was "SimpleAI_Image-0.1.1.tar", last modified: Mon May 20 16:38:07 2024, max compression
```

## Comparing `SimpleAI_Image-0.1.0.tar` & `SimpleAI_Image-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 15:44:51.008141 SimpleAI_Image-0.1.0/
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 15:44:51.006411 SimpleAI_Image-0.1.0/ImageAI/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 SimpleAI_Image-0.1.0/ImageAI/DataProcessor.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 SimpleAI_Image-0.1.0/ImageAI/DatabaseHandler.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:25:09.000000 SimpleAI_Image-0.1.0/ImageAI/__init__.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      419 2024-05-20 15:44:51.007881 SimpleAI_Image-0.1.0/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      171 2024-05-20 12:30:35.000000 SimpleAI_Image-0.1.0/README.md
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 15:44:51.007314 SimpleAI_Image-0.1.0/SimpleAI_Image.egg-info/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      419 2024-05-20 15:44:50.000000 SimpleAI_Image-0.1.0/SimpleAI_Image.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      297 2024-05-20 15:44:50.000000 SimpleAI_Image-0.1.0/SimpleAI_Image.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 15:44:50.000000 SimpleAI_Image-0.1.0/SimpleAI_Image.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       68 2024-05-20 15:44:50.000000 SimpleAI_Image-0.1.0/SimpleAI_Image.egg-info/requires.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       14 2024-05-20 15:44:50.000000 SimpleAI_Image-0.1.0/SimpleAI_Image.egg-info/top_level.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 15:44:51.008212 SimpleAI_Image-0.1.0/setup.cfg
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      772 2024-05-20 15:44:40.000000 SimpleAI_Image-0.1.0/setup.py
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 15:44:51.007601 SimpleAI_Image-0.1.0/tests/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 SimpleAI_Image-0.1.0/tests/__init__.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 16:38:07.908950 SimpleAI_Image-0.1.1/
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 16:38:07.907599 SimpleAI_Image-0.1.1/ImageAI/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 SimpleAI_Image-0.1.1/ImageAI/DataProcessor.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 SimpleAI_Image-0.1.1/ImageAI/DatabaseHandler.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:25:09.000000 SimpleAI_Image-0.1.1/ImageAI/__init__.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 16:38:07.908778 SimpleAI_Image-0.1.1/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 SimpleAI_Image-0.1.1/README.md
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 16:38:07.908359 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      297 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      178 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/requires.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       14 2024-05-20 16:38:07.000000 SimpleAI_Image-0.1.1/SimpleAI_Image.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 16:38:07.909008 SimpleAI_Image-0.1.1/setup.cfg
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1034 2024-05-20 16:35:54.000000 SimpleAI_Image-0.1.1/setup.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 16:38:07.908527 SimpleAI_Image-0.1.1/tests/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 SimpleAI_Image-0.1.1/tests/__init__.py
```

### Comparing `SimpleAI_Image-0.1.0/ImageAI/DataProcessor.py` & `SimpleAI_Image-0.1.1/ImageAI/DataProcessor.py`

 * *Files identical despite different names*

### Comparing `SimpleAI_Image-0.1.0/ImageAI/DatabaseHandler.py` & `SimpleAI_Image-0.1.1/ImageAI/DatabaseHandler.py`

 * *Files identical despite different names*

### Comparing `SimpleAI_Image-0.1.0/setup.py` & `SimpleAI_Image-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SimpleAI_Image',  # Change this to a unique name
-    version='0.1.0',
+    version='0.1.1',  # Increment the version number
     description='A package for processing and storing image vectors in PostgreSQL',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author='Tobias Poulsen',
     author_email='your.email@example.com',
     url='https://github.com/Tobias2408/bachelorprojekt',  # Your package's URL
     packages=find_packages(),
     install_requires=[
-        'numpy',
-        'pandas',
-        'sqlalchemy',
-        'pgvector',
-        'matplotlib',
-        'tensorflow',
-        'scikit-learn',
+        'numpy==1.23.5',
+        'pandas==1.5.3',
+        'sqlalchemy==2.0.30',
+        'matplotlib==3.6.3',
+        'tensorflow-macos==2.12.0',
+        'tensorflow-datasets==4.9.2',
+        'tensorflow-metal==0.8.0',
+        'scikit-learn==1.2.2',
+        'requests==2.28.2',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```


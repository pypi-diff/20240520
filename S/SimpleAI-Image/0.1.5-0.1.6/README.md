# Comparing `tmp/SimpleAI_Image-0.1.5.tar.gz` & `tmp/simpleai_image-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleAI_Image-0.1.5.tar", last modified: Mon May 20 18:15:20 2024, max compression
+gzip compressed data, was "simpleai_image-0.1.6.tar", last modified: Mon May 20 19:03:05 2024, max compression
```

## Comparing `SimpleAI_Image-0.1.5.tar` & `simpleai_image-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:15:20.538488 SimpleAI_Image-0.1.5/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 18:15:20.538316 SimpleAI_Image-0.1.5/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 SimpleAI_Image-0.1.5/README.md
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:15:20.537127 SimpleAI_Image-0.1.5/SimpleAI_Image/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 SimpleAI_Image-0.1.5/SimpleAI_Image/DataProcessor.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 SimpleAI_Image-0.1.5/SimpleAI_Image/DatabaseHandler.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       86 2024-05-20 18:07:54.000000 SimpleAI_Image-0.1.5/SimpleAI_Image/__init__.py
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:15:20.537928 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      318 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      129 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/requires.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       21 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/top_level.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 18:15:20.538552 SimpleAI_Image-0.1.5/setup.cfg
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1007 2024-05-20 18:15:13.000000 SimpleAI_Image-0.1.5/setup.py
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:15:20.538095 SimpleAI_Image-0.1.5/tests/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 SimpleAI_Image-0.1.5/tests/__init__.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:03:05.105821 simpleai_image-0.1.6/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      927 2024-05-20 19:03:05.105547 simpleai_image-0.1.6/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 simpleai_image-0.1.6/README.md
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:03:05.104011 simpleai_image-0.1.6/SimpleAI_Image/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 simpleai_image-0.1.6/SimpleAI_Image/DataProcessor.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 simpleai_image-0.1.6/SimpleAI_Image/DatabaseHandler.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       86 2024-05-20 18:07:54.000000 simpleai_image-0.1.6/SimpleAI_Image/__init__.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:03:05.105201 simpleai_image-0.1.6/SimpleAI_Image.egg-info/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      927 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      318 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      129 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/requires.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       21 2024-05-20 19:03:05.000000 simpleai_image-0.1.6/SimpleAI_Image.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 19:03:05.105885 simpleai_image-0.1.6/setup.cfg
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      921 2024-05-20 19:01:37.000000 simpleai_image-0.1.6/setup.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 19:03:05.104971 simpleai_image-0.1.6/tests/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 simpleai_image-0.1.6/tests/__init__.py
```

### Comparing `SimpleAI_Image-0.1.5/SimpleAI_Image/DataProcessor.py` & `simpleai_image-0.1.6/SimpleAI_Image/DataProcessor.py`

 * *Files identical despite different names*

### Comparing `SimpleAI_Image-0.1.5/SimpleAI_Image/DatabaseHandler.py` & `simpleai_image-0.1.6/SimpleAI_Image/DatabaseHandler.py`

 * *Files identical despite different names*

### Comparing `SimpleAI_Image-0.1.5/setup.py` & `simpleai_image-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='SimpleAI_Image',  # Change this to a unique name
-    version='0.1.5',  # Increment the version number
+    name='SimpleAI_Image',
+    version='0.1.6',
     description='A package for processing and storing image vectors in PostgreSQL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Tobias Poulsen',
     author_email='your.email@example.com',
-    url='https://github.com/Tobias2408/bachelorprojekt',  # Your package's URL
+    url='https://github.com/Tobias2408/bachelorprojekt',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'sqlalchemy',
         'matplotlib',
         'tensorflow-macos',
```


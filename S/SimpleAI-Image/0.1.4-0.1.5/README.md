# Comparing `tmp/SimpleAI_Image-0.1.4.tar.gz` & `tmp/SimpleAI_Image-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleAI_Image-0.1.4.tar", last modified: Mon May 20 18:13:42 2024, max compression
+gzip compressed data, was "SimpleAI_Image-0.1.5.tar", last modified: Mon May 20 18:15:20 2024, max compression
```

## Comparing `SimpleAI_Image-0.1.4.tar` & `SimpleAI_Image-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:13:42.583195 SimpleAI_Image-0.1.4/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 18:13:42.583031 SimpleAI_Image-0.1.4/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 SimpleAI_Image-0.1.4/README.md
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:13:42.581797 SimpleAI_Image-0.1.4/SimpleAI_Image/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 SimpleAI_Image-0.1.4/SimpleAI_Image/DataProcessor.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 SimpleAI_Image-0.1.4/SimpleAI_Image/DatabaseHandler.py
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       86 2024-05-20 18:07:54.000000 SimpleAI_Image-0.1.4/SimpleAI_Image/__init__.py
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:13:42.582592 SimpleAI_Image-0.1.4/SimpleAI_Image.egg-info/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 18:13:42.000000 SimpleAI_Image-0.1.4/SimpleAI_Image.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      318 2024-05-20 18:13:42.000000 SimpleAI_Image-0.1.4/SimpleAI_Image.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 18:13:42.000000 SimpleAI_Image-0.1.4/SimpleAI_Image.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      211 2024-05-20 18:13:42.000000 SimpleAI_Image-0.1.4/SimpleAI_Image.egg-info/requires.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       21 2024-05-20 18:13:42.000000 SimpleAI_Image-0.1.4/SimpleAI_Image.egg-info/top_level.txt
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 18:13:42.583250 SimpleAI_Image-0.1.4/setup.cfg
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1132 2024-05-20 18:13:28.000000 SimpleAI_Image-0.1.4/setup.py
-drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:13:42.582784 SimpleAI_Image-0.1.4/tests/
--rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 SimpleAI_Image-0.1.4/tests/__init__.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:15:20.538488 SimpleAI_Image-0.1.5/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 18:15:20.538316 SimpleAI_Image-0.1.5/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      173 2024-05-20 16:02:30.000000 SimpleAI_Image-0.1.5/README.md
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:15:20.537127 SimpleAI_Image-0.1.5/SimpleAI_Image/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     3354 2024-05-19 20:49:16.000000 SimpleAI_Image-0.1.5/SimpleAI_Image/DataProcessor.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1150 2024-05-19 20:48:47.000000 SimpleAI_Image-0.1.5/SimpleAI_Image/DatabaseHandler.py
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       86 2024-05-20 18:07:54.000000 SimpleAI_Image-0.1.5/SimpleAI_Image/__init__.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:15:20.537928 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      633 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      318 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        1 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)      129 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/requires.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       21 2024-05-20 18:15:20.000000 SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)       38 2024-05-20 18:15:20.538552 SimpleAI_Image-0.1.5/setup.cfg
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)     1007 2024-05-20 18:15:13.000000 SimpleAI_Image-0.1.5/setup.py
+drwxr-xr-x   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 18:15:20.538095 SimpleAI_Image-0.1.5/tests/
+-rw-r--r--   0 tobiaspoulsen   (501) staff       (20)        0 2024-05-20 12:26:32.000000 SimpleAI_Image-0.1.5/tests/__init__.py
```

### Comparing `SimpleAI_Image-0.1.4/PKG-INFO` & `SimpleAI_Image-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleAI_Image
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for processing and storing image vectors in PostgreSQL
 Home-page: https://github.com/Tobias2408/bachelorprojekt
 Author: Tobias Poulsen
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SimpleAI_Image-0.1.4/SimpleAI_Image/DataProcessor.py` & `SimpleAI_Image-0.1.5/SimpleAI_Image/DataProcessor.py`

 * *Files identical despite different names*

### Comparing `SimpleAI_Image-0.1.4/SimpleAI_Image/DatabaseHandler.py` & `SimpleAI_Image-0.1.5/SimpleAI_Image/DatabaseHandler.py`

 * *Files identical despite different names*

### Comparing `SimpleAI_Image-0.1.4/SimpleAI_Image.egg-info/PKG-INFO` & `SimpleAI_Image-0.1.5/SimpleAI_Image.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleAI-Image
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for processing and storing image vectors in PostgreSQL
 Home-page: https://github.com/Tobias2408/bachelorprojekt
 Author: Tobias Poulsen
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SimpleAI_Image-0.1.4/setup.py` & `SimpleAI_Image-0.1.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SimpleAI_Image',  # Change this to a unique name
-    version='0.1.4',  # Increment the version number
+    version='0.1.5',  # Increment the version number
     description='A package for processing and storing image vectors in PostgreSQL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Tobias Poulsen',
     author_email='your.email@example.com',
     url='https://github.com/Tobias2408/bachelorprojekt',  # Your package's URL
     packages=find_packages(),
     install_requires=[
-        'numpy==1.23.5',
-        'pandas==1.5.3',
-        'sqlalchemy==2.0.30',
-        'matplotlib==3.6.3',
-        'tensorflow-macos==2.12.0',  # Updated to the latest available version
-        'tensorflow-datasets==4.9.2',
-        'tensorflow-metal==0.8.0',
-        'scikit-learn==1.2.2',
-        'requests==2.31.0',
-        'keras==3.0.0',
-        'tensorboard==2.16.0',
+        'numpy',
+        'pandas',
+        'sqlalchemy',
+        'matplotlib',
+        'tensorflow-macos',
+        'tensorflow-datasets',
+        'tensorflow-metal',
+        'scikit-learn',
+        'requests',
+        'keras',
+        'tensorboard',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```


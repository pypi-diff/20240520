# Comparing `tmp/data_store_connector-0.1.0.tar.gz` & `tmp/data_store_connector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_store_connector-0.1.0.tar", last modified: Mon May 20 12:07:24 2024, max compression
+gzip compressed data, was "data_store_connector-0.1.1.tar", last modified: Mon May 20 12:12:53 2024, max compression
```

## Comparing `data_store_connector-0.1.0.tar` & `data_store_connector-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 chandanikumari   (501) staff       (20)        0 2024-05-20 12:07:24.482637 data_store_connector-0.1.0/
--rw-r--r--   0 chandanikumari   (501) staff       (20)      484 2024-05-20 11:38:09.000000 data_store_connector-0.1.0/LICENSE
--rw-r--r--   0 chandanikumari   (501) staff       (20)      479 2024-05-20 12:07:24.482308 data_store_connector-0.1.0/PKG-INFO
--rw-r--r--   0 chandanikumari   (501) staff       (20)       11 2024-05-20 11:48:04.000000 data_store_connector-0.1.0/README.md
-drwxr-xr-x   0 chandanikumari   (501) staff       (20)        0 2024-05-20 12:07:24.481952 data_store_connector-0.1.0/data_store_connector.egg-info/
--rw-r--r--   0 chandanikumari   (501) staff       (20)      479 2024-05-20 12:07:24.000000 data_store_connector-0.1.0/data_store_connector.egg-info/PKG-INFO
--rw-r--r--   0 chandanikumari   (501) staff       (20)      248 2024-05-20 12:07:24.000000 data_store_connector-0.1.0/data_store_connector.egg-info/SOURCES.txt
--rw-r--r--   0 chandanikumari   (501) staff       (20)        1 2024-05-20 12:07:24.000000 data_store_connector-0.1.0/data_store_connector.egg-info/dependency_links.txt
--rw-r--r--   0 chandanikumari   (501) staff       (20)       10 2024-05-20 12:07:24.000000 data_store_connector-0.1.0/data_store_connector.egg-info/top_level.txt
-drwxr-xr-x   0 chandanikumari   (501) staff       (20)        0 2024-05-20 12:07:24.481289 data_store_connector-0.1.0/my_module/
--rw-r--r--   0 chandanikumari   (501) staff       (20)       39 2024-05-20 11:34:47.000000 data_store_connector-0.1.0/my_module/__init__.py
--rw-r--r--   0 chandanikumari   (501) staff       (20)       38 2024-05-20 12:07:24.482711 data_store_connector-0.1.0/setup.cfg
--rw-r--r--   0 chandanikumari   (501) staff       (20)      763 2024-05-20 12:07:04.000000 data_store_connector-0.1.0/setup.py
-drwxr-xr-x   0 chandanikumari   (501) staff       (20)        0 2024-05-20 12:07:24.481562 data_store_connector-0.1.0/tests/
--rw-r--r--   0 chandanikumari   (501) staff       (20)      150 2024-05-20 11:35:18.000000 data_store_connector-0.1.0/tests/test_my_module.py
+drwxr-xr-x   0 chandanikumari   (501) staff       (20)        0 2024-05-20 12:12:53.182386 data_store_connector-0.1.1/
+-rw-r--r--   0 chandanikumari   (501) staff       (20)      484 2024-05-20 11:38:09.000000 data_store_connector-0.1.1/LICENSE
+-rw-r--r--   0 chandanikumari   (501) staff       (20)      479 2024-05-20 12:12:53.182115 data_store_connector-0.1.1/PKG-INFO
+-rw-r--r--   0 chandanikumari   (501) staff       (20)       11 2024-05-20 11:48:04.000000 data_store_connector-0.1.1/README.md
+drwxr-xr-x   0 chandanikumari   (501) staff       (20)        0 2024-05-20 12:12:53.181801 data_store_connector-0.1.1/data_store_connector.egg-info/
+-rw-r--r--   0 chandanikumari   (501) staff       (20)      479 2024-05-20 12:12:53.000000 data_store_connector-0.1.1/data_store_connector.egg-info/PKG-INFO
+-rw-r--r--   0 chandanikumari   (501) staff       (20)      248 2024-05-20 12:12:53.000000 data_store_connector-0.1.1/data_store_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 chandanikumari   (501) staff       (20)        1 2024-05-20 12:12:53.000000 data_store_connector-0.1.1/data_store_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 chandanikumari   (501) staff       (20)       10 2024-05-20 12:12:53.000000 data_store_connector-0.1.1/data_store_connector.egg-info/top_level.txt
+drwxr-xr-x   0 chandanikumari   (501) staff       (20)        0 2024-05-20 12:12:53.181126 data_store_connector-0.1.1/my_module/
+-rw-r--r--   0 chandanikumari   (501) staff       (20)       39 2024-05-20 11:34:47.000000 data_store_connector-0.1.1/my_module/__init__.py
+-rw-r--r--   0 chandanikumari   (501) staff       (20)       38 2024-05-20 12:12:53.182458 data_store_connector-0.1.1/setup.cfg
+-rw-r--r--   0 chandanikumari   (501) staff       (20)      763 2024-05-20 12:12:05.000000 data_store_connector-0.1.1/setup.py
+drwxr-xr-x   0 chandanikumari   (501) staff       (20)        0 2024-05-20 12:12:53.181442 data_store_connector-0.1.1/tests/
+-rw-r--r--   0 chandanikumari   (501) staff       (20)      150 2024-05-20 11:35:18.000000 data_store_connector-0.1.1/tests/test_my_module.py
```

### Comparing `data_store_connector-0.1.0/setup.py` & `data_store_connector-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='data_store_connector',
-    version='0.1.0',
+    version='0.1.1',
     description='A brief description of your project',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Chandani7250/CONNECTOR',
     author='Chandani Kumari',
     author_email='chandani@chandani.com',
     license='MIT',
```


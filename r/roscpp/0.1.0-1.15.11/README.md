# Comparing `tmp/roscpp-0.1.0.tar.gz` & `tmp/roscpp-1.15.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roscpp-0.1.0.tar", last modified: Mon May 20 16:35:45 2024, max compression
+gzip compressed data, was "roscpp-1.15.11.tar", last modified: Mon May 20 16:42:30 2024, max compression
```

## Comparing `roscpp-0.1.0.tar` & `roscpp-1.15.11.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lupin      (501) staff       (20)        0 2024-05-20 16:35:45.288840 roscpp-0.1.0/
--rw-r--r--   0 lupin      (501) staff       (20)      484 2024-05-20 16:35:45.288745 roscpp-0.1.0/PKG-INFO
--rw-r--r--   0 lupin      (501) staff       (20)       48 2024-05-20 16:35:45.000000 roscpp-0.1.0/README.md
-drwxr-xr-x   0 lupin      (501) staff       (20)        0 2024-05-20 16:35:45.288128 roscpp-0.1.0/roscpp/
--rw-r--r--   0 lupin      (501) staff       (20)       35 2024-05-20 16:35:45.000000 roscpp-0.1.0/roscpp/__init__.py
--rw-r--r--   0 lupin      (501) staff       (20)       46 2024-05-20 16:35:45.000000 roscpp-0.1.0/roscpp/my_module.py
-drwxr-xr-x   0 lupin      (501) staff       (20)        0 2024-05-20 16:35:45.288608 roscpp-0.1.0/roscpp.egg-info/
--rw-r--r--   0 lupin      (501) staff       (20)      484 2024-05-20 16:35:45.000000 roscpp-0.1.0/roscpp.egg-info/PKG-INFO
--rw-r--r--   0 lupin      (501) staff       (20)      177 2024-05-20 16:35:45.000000 roscpp-0.1.0/roscpp.egg-info/SOURCES.txt
--rw-r--r--   0 lupin      (501) staff       (20)        1 2024-05-20 16:35:45.000000 roscpp-0.1.0/roscpp.egg-info/dependency_links.txt
--rw-r--r--   0 lupin      (501) staff       (20)        7 2024-05-20 16:35:45.000000 roscpp-0.1.0/roscpp.egg-info/top_level.txt
--rw-r--r--   0 lupin      (501) staff       (20)       38 2024-05-20 16:35:45.288881 roscpp-0.1.0/setup.cfg
--rw-r--r--   0 lupin      (501) staff       (20)      626 2024-05-20 16:35:45.000000 roscpp-0.1.0/setup.py
+drwxr-xr-x   0 lupin      (501) staff       (20)        0 2024-05-20 16:42:30.692293 roscpp-1.15.11/
+-rw-r--r--   0 lupin      (501) staff       (20)      486 2024-05-20 16:42:30.692201 roscpp-1.15.11/PKG-INFO
+-rw-r--r--   0 lupin      (501) staff       (20)       48 2024-05-20 16:35:45.000000 roscpp-1.15.11/README.md
+drwxr-xr-x   0 lupin      (501) staff       (20)        0 2024-05-20 16:42:30.691659 roscpp-1.15.11/roscpp/
+-rw-r--r--   0 lupin      (501) staff       (20)       35 2024-05-20 16:35:45.000000 roscpp-1.15.11/roscpp/__init__.py
+-rw-r--r--   0 lupin      (501) staff       (20)       46 2024-05-20 16:35:45.000000 roscpp-1.15.11/roscpp/my_module.py
+drwxr-xr-x   0 lupin      (501) staff       (20)        0 2024-05-20 16:42:30.692069 roscpp-1.15.11/roscpp.egg-info/
+-rw-r--r--   0 lupin      (501) staff       (20)      486 2024-05-20 16:42:30.000000 roscpp-1.15.11/roscpp.egg-info/PKG-INFO
+-rw-r--r--   0 lupin      (501) staff       (20)      177 2024-05-20 16:42:30.000000 roscpp-1.15.11/roscpp.egg-info/SOURCES.txt
+-rw-r--r--   0 lupin      (501) staff       (20)        1 2024-05-20 16:42:30.000000 roscpp-1.15.11/roscpp.egg-info/dependency_links.txt
+-rw-r--r--   0 lupin      (501) staff       (20)        7 2024-05-20 16:42:30.000000 roscpp-1.15.11/roscpp.egg-info/top_level.txt
+-rw-r--r--   0 lupin      (501) staff       (20)       38 2024-05-20 16:42:30.692324 roscpp-1.15.11/setup.cfg
+-rw-r--r--   0 lupin      (501) staff       (20)      628 2024-05-20 16:42:12.000000 roscpp-1.15.11/setup.py
```

### Comparing `roscpp-0.1.0/setup.py` & `roscpp-1.15.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 setup(
     name="roscpp",
-    version="0.1.0",
+    version="1.15.11",
     packages=find_packages(),
     author="Your Name",
     author_email="your.email@example.com",
     description="A simple example package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/yourusername/roscpp",
```


# Comparing `tmp/twinlib-0.1.7.tar.gz` & `tmp/twinlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlib-0.1.7.tar", last modified: Sat May 18 16:25:41 2024, max compression
+gzip compressed data, was "twinlib-0.2.0.tar", last modified: Mon May 20 09:00:31 2024, max compression
```

## Comparing `twinlib-0.1.7.tar` & `twinlib-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:25:41.291061 twinlib-0.1.7/
--rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-18 16:25:41.291061 twinlib-0.1.7/PKG-INFO
--rw-r--r--   0 gaia      (1000) gaia      (1000)        0 2024-05-17 10:08:09.000000 twinlib-0.1.7/README.md
--rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-18 16:25:41.291061 twinlib-0.1.7/setup.cfg
--rw-r--r--   0 gaia      (1000) gaia      (1000)      556 2024-05-18 16:25:18.000000 twinlib-0.1.7/setup.py
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:25:41.291061 twinlib-0.1.7/twinlib.egg-info/
--rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/PKG-INFO
--rw-r--r--   0 gaia      (1000) gaia      (1000)      220 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/SOURCES.txt
--rw-r--r--   0 gaia      (1000) gaia      (1000)        1 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/dependency_links.txt
--rw-r--r--   0 gaia      (1000) gaia      (1000)       46 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/entry_points.txt
--rw-r--r--   0 gaia      (1000) gaia      (1000)       12 2024-05-18 16:25:41.000000 twinlib-0.1.7/twinlib.egg-info/top_level.txt
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-18 16:25:41.291061 twinlib-0.1.7/twinlib_pkg/
--rw-r--r--   0 gaia      (1000) gaia      (1000)       23 2024-05-18 16:03:24.000000 twinlib-0.1.7/twinlib_pkg/__init__.py
--rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-18 16:03:05.000000 twinlib-0.1.7/twinlib_pkg/main.py
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 09:00:31.388167 twinlib-0.2.0/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-20 09:00:31.388167 twinlib-0.2.0/PKG-INFO
+-rw-r--r--   0 gaia      (1000) gaia      (1000)        0 2024-05-17 10:08:09.000000 twinlib-0.2.0/README.md
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-20 09:00:31.388167 twinlib-0.2.0/setup.cfg
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      552 2024-05-20 09:00:09.000000 twinlib-0.2.0/setup.py
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 09:00:31.378166 twinlib-0.2.0/twinlib/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       23 2024-05-18 16:03:24.000000 twinlib-0.2.0/twinlib/__init__.py
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-18 16:03:05.000000 twinlib-0.2.0/twinlib/main.py
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 09:00:31.388167 twinlib-0.2.0/twinlib.egg-info/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/PKG-INFO
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      212 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)        1 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       42 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/entry_points.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)        8 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/top_level.txt
```

### Comparing `twinlib-0.1.7/setup.py` & `twinlib-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="twinlib",
-    version="0.1.7",
+    version="0.2.0",
     author="gaiamzz",
     author_email="mzzgai@unife.it",
     description="A library for twin detection",
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'twinlib = twinlib_pkg:hello'
+            'twinlib = twinlib:hello'
         ]
     },
     packages=find_packages(),
     install_requires=[],
     extras_require={},
 )
```


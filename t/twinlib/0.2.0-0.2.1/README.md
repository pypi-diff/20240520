# Comparing `tmp/twinlib-0.2.0.tar.gz` & `tmp/twinlib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlib-0.2.0.tar", last modified: Mon May 20 09:00:31 2024, max compression
+gzip compressed data, was "twinlib-0.2.1.tar", last modified: Mon May 20 11:50:24 2024, max compression
```

## Comparing `twinlib-0.2.0.tar` & `twinlib-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 09:00:31.388167 twinlib-0.2.0/
--rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-20 09:00:31.388167 twinlib-0.2.0/PKG-INFO
--rw-r--r--   0 gaia      (1000) gaia      (1000)        0 2024-05-17 10:08:09.000000 twinlib-0.2.0/README.md
--rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-20 09:00:31.388167 twinlib-0.2.0/setup.cfg
--rw-r--r--   0 gaia      (1000) gaia      (1000)      552 2024-05-20 09:00:09.000000 twinlib-0.2.0/setup.py
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 09:00:31.378166 twinlib-0.2.0/twinlib/
--rw-r--r--   0 gaia      (1000) gaia      (1000)       23 2024-05-18 16:03:24.000000 twinlib-0.2.0/twinlib/__init__.py
--rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-18 16:03:05.000000 twinlib-0.2.0/twinlib/main.py
-drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 09:00:31.388167 twinlib-0.2.0/twinlib.egg-info/
--rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/PKG-INFO
--rw-r--r--   0 gaia      (1000) gaia      (1000)      212 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/SOURCES.txt
--rw-r--r--   0 gaia      (1000) gaia      (1000)        1 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/dependency_links.txt
--rw-r--r--   0 gaia      (1000) gaia      (1000)       42 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/entry_points.txt
--rw-r--r--   0 gaia      (1000) gaia      (1000)        8 2024-05-20 09:00:31.000000 twinlib-0.2.0/twinlib.egg-info/top_level.txt
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 11:50:24.062083 twinlib-0.2.1/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-20 11:50:24.062083 twinlib-0.2.1/PKG-INFO
+-rw-r--r--   0 gaia      (1000) gaia      (1000)        0 2024-05-17 10:08:09.000000 twinlib-0.2.1/README.md
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       38 2024-05-20 11:50:24.062083 twinlib-0.2.1/setup.cfg
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      552 2024-05-20 11:50:06.000000 twinlib-0.2.1/setup.py
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 11:50:24.052082 twinlib-0.2.1/twinlib/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       22 2024-05-20 11:49:58.000000 twinlib-0.2.1/twinlib/__init__.py
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       37 2024-05-20 11:49:51.000000 twinlib-0.2.1/twinlib/main.py
+drwxr-xr-x   0 gaia      (1000) gaia      (1000)        0 2024-05-20 11:50:24.052082 twinlib-0.2.1/twinlib.egg-info/
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      281 2024-05-20 11:50:24.000000 twinlib-0.2.1/twinlib.egg-info/PKG-INFO
+-rw-r--r--   0 gaia      (1000) gaia      (1000)      212 2024-05-20 11:50:24.000000 twinlib-0.2.1/twinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)        1 2024-05-20 11:50:24.000000 twinlib-0.2.1/twinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)       42 2024-05-20 11:50:24.000000 twinlib-0.2.1/twinlib.egg-info/entry_points.txt
+-rw-r--r--   0 gaia      (1000) gaia      (1000)        8 2024-05-20 11:50:24.000000 twinlib-0.2.1/twinlib.egg-info/top_level.txt
```

### Comparing `twinlib-0.2.0/setup.py` & `twinlib-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="twinlib",
-    version="0.2.0",
+    version="0.2.1",
     author="gaiamzz",
     author_email="mzzgai@unife.it",
     description="A library for twin detection",
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```


# Comparing `tmp/spencer_funcs-0.0.2.tar.gz` & `tmp/spencer_funcs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spencer_funcs-0.0.2.tar", last modified: Wed May  8 23:19:47 2024, max compression
+gzip compressed data, was "spencer_funcs-0.0.3.tar", last modified: Mon May 20 20:44:39 2024, max compression
```

## Comparing `spencer_funcs-0.0.2.tar` & `spencer_funcs-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 23:19:47.070735 spencer_funcs-0.0.2/
--rw-rw-rw-   0        0        0    35823 2024-05-08 23:12:58.000000 spencer_funcs-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0      261 2024-05-08 23:19:47.070735 spencer_funcs-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-05-08 23:12:58.000000 spencer_funcs-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-08 23:19:47.071735 spencer_funcs-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-05-08 23:19:46.000000 spencer_funcs-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 23:19:47.062734 spencer_funcs-0.0.2/spencer_funcs/
--rw-rw-rw-   0        0        0       24 2024-05-08 23:14:19.000000 spencer_funcs-0.0.2/spencer_funcs/__init__.py
--rw-rw-rw-   0        0        0     1807 2024-05-08 23:19:46.000000 spencer_funcs-0.0.2/spencer_funcs/autodiscovery.py
-drwxrwxrwx   0        0        0        0 2024-05-08 23:19:47.068735 spencer_funcs-0.0.2/spencer_funcs.egg-info/
--rw-rw-rw-   0        0        0      261 2024-05-08 23:19:46.000000 spencer_funcs-0.0.2/spencer_funcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-08 23:19:46.000000 spencer_funcs-0.0.2/spencer_funcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 23:19:46.000000 spencer_funcs-0.0.2/spencer_funcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 23:19:46.000000 spencer_funcs-0.0.2/spencer_funcs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 20:44:39.282471 spencer_funcs-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2024-05-08 23:12:58.000000 spencer_funcs-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0      261 2024-05-20 20:44:39.281471 spencer_funcs-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-05-08 23:12:58.000000 spencer_funcs-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-20 20:44:39.282471 spencer_funcs-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-05-20 20:44:38.000000 spencer_funcs-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:44:39.272500 spencer_funcs-0.0.3/spencer_funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-20 20:44:38.000000 spencer_funcs-0.0.3/spencer_funcs/__init__.py
+-rw-rw-rw-   0        0        0     1807 2024-05-08 23:19:46.000000 spencer_funcs-0.0.3/spencer_funcs/autodiscovery.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:44:39.279467 spencer_funcs-0.0.3/spencer_funcs.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-05-20 20:44:39.000000 spencer_funcs-0.0.3/spencer_funcs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-20 20:44:39.000000 spencer_funcs-0.0.3/spencer_funcs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 20:44:39.000000 spencer_funcs-0.0.3/spencer_funcs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 20:44:39.000000 spencer_funcs-0.0.3/spencer_funcs.egg-info/top_level.txt
```

### Comparing `spencer_funcs-0.0.2/LICENSE.md` & `spencer_funcs-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spencer_funcs-0.0.2/setup.py` & `spencer_funcs-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `spencer_funcs-0.0.2/spencer_funcs/autodiscovery.py` & `spencer_funcs-0.0.3/spencer_funcs/autodiscovery.py`

 * *Files identical despite different names*


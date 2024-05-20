# Comparing `tmp/godork-1.2.0.tar.gz` & `tmp/godork-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godork-1.2.0.tar", last modified: Mon May 20 12:09:27 2024, max compression
+gzip compressed data, was "godork-1.2.1.tar", last modified: Mon May 20 15:30:12 2024, max compression
```

## Comparing `godork-1.2.0.tar` & `godork-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 12:09:27.232706 godork-1.2.0/
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     1069 2024-05-18 10:22:51.000000 godork-1.2.0/LICENSE
--rw-r--r--   0 thd3r     (1000) thd3r     (1000)     7045 2024-05-20 12:09:27.232706 godork-1.2.0/PKG-INFO
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     6636 2024-05-20 11:27:39.000000 godork-1.2.0/README.md
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 12:09:27.232706 godork-1.2.0/godork.egg-info/
--rw-r--r--   0 thd3r     (1000) thd3r     (1000)     7045 2024-05-20 12:09:27.000000 godork-1.2.0/godork.egg-info/PKG-INFO
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      238 2024-05-20 12:09:27.000000 godork-1.2.0/godork.egg-info/SOURCES.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        1 2024-05-20 12:09:27.000000 godork-1.2.0/godork.egg-info/dependency_links.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       43 2024-05-20 12:09:27.000000 godork-1.2.0/godork.egg-info/entry_points.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       29 2024-05-20 12:09:27.000000 godork-1.2.0/godork.egg-info/requires.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        4 2024-05-20 12:09:27.000000 godork-1.2.0/godork.egg-info/top_level.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       38 2024-05-20 12:09:27.232706 godork-1.2.0/setup.cfg
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      717 2024-05-20 12:07:18.000000 godork-1.2.0/setup.py
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 12:09:27.232706 godork-1.2.0/src/
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       27 2024-05-20 11:35:10.000000 godork-1.2.0/src/__init__.py
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     6710 2024-05-20 11:39:48.000000 godork-1.2.0/src/godork.py
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:30:12.946059 godork-1.2.1/
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     1069 2024-05-20 15:25:46.000000 godork-1.2.1/LICENSE
+-rw-r--r--   0 thd3r     (1000) thd3r     (1000)     3230 2024-05-20 15:30:12.946059 godork-1.2.1/PKG-INFO
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     2822 2024-05-20 15:26:41.000000 godork-1.2.1/README.md
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:30:12.946059 godork-1.2.1/godork.egg-info/
+-rw-r--r--   0 thd3r     (1000) thd3r     (1000)     3230 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/PKG-INFO
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      238 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/SOURCES.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        1 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/dependency_links.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       43 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/entry_points.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       29 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/requires.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        4 2024-05-20 15:30:12.000000 godork-1.2.1/godork.egg-info/top_level.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       38 2024-05-20 15:30:12.946059 godork-1.2.1/setup.cfg
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      717 2024-05-20 15:25:46.000000 godork-1.2.1/setup.py
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-20 15:30:12.946059 godork-1.2.1/src/
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       27 2024-05-20 15:25:46.000000 godork-1.2.1/src/__init__.py
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     6710 2024-05-20 15:26:17.000000 godork-1.2.1/src/godork.py
```

### Comparing `godork-1.2.0/LICENSE` & `godork-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `godork-1.2.0/setup.py` & `godork-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `godork-1.2.0/src/godork.py` & `godork-1.2.1/src/godork.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import asyncio # v3.4.3
 import random
 import time
 import json
 import os
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 class OptionsArgs(object):
     
     def __init__(self):
         self.parser = ArgumentParser(
             prog="godork",
             add_help=False,
```


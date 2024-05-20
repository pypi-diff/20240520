# Comparing `tmp/alist3-1.1.tar.gz` & `tmp/alist3-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alist3-1.1.tar", last modified: Fri May 10 15:38:33 2024, max compression
+gzip compressed data, was "alist3-1.1.1.tar", last modified: Mon May 20 14:49:44 2024, max compression
```

## Comparing `alist3-1.1.tar` & `alist3-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:38:33.436577 alist3-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-10 15:38:11.000000 alist3-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-10 15:38:33.436577 alist3-1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:38:33.436577 alist3-1.1/alist/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 15:38:11.000000 alist3-1.1/alist/Error.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 15:38:11.000000 alist3-1.1/alist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-10 15:38:11.000000 alist3-1.1/alist/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-10 15:38:11.000000 alist3-1.1/alist/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-10 15:38:11.000000 alist3-1.1/alist/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-10 15:38:11.000000 alist3-1.1/alist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:38:33.436577 alist3-1.1/alist3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-10 15:38:33.000000 alist3-1.1/alist3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-10 15:38:33.000000 alist3-1.1/alist3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:38:33.000000 alist3-1.1/alist3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 15:38:33.000000 alist3-1.1/alist3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 15:38:33.000000 alist3-1.1/alist3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:38:33.436577 alist3-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-10 15:38:11.000000 alist3-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:44.285091 alist3-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-20 14:49:33.000000 alist3-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-20 14:49:44.285091 alist3-1.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:44.285091 alist3-1.1.1/alist/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-20 14:49:33.000000 alist3-1.1.1/alist/Error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-20 14:49:33.000000 alist3-1.1.1/alist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-20 14:49:33.000000 alist3-1.1.1/alist/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-20 14:49:33.000000 alist3-1.1.1/alist/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-20 14:49:33.000000 alist3-1.1.1/alist/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-20 14:49:33.000000 alist3-1.1.1/alist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:44.285091 alist3-1.1.1/alist3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-20 14:49:44.000000 alist3-1.1.1/alist3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-20 14:49:44.000000 alist3-1.1.1/alist3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:49:44.000000 alist3-1.1.1/alist3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 14:49:44.000000 alist3-1.1.1/alist3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 14:49:44.000000 alist3-1.1.1/alist3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:49:44.285091 alist3-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-20 14:49:33.000000 alist3-1.1.1/setup.py
```

### Comparing `alist3-1.1/LICENSE` & `alist3-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alist3-1.1/alist/file.py` & `alist3-1.1.1/alist/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import requests as _req
 
 
 class AListFile:
     def __init__(self, path, init):
-        print(init)
         self.path = path
         self.name = init["name"]
         self.provider = init["provider"]
         self.size = init["size"]
         self.modified = init["modified"]
         self.created = init["created"]
         self.url = init["raw_url"]
```

### Comparing `alist3-1.1/alist/main.py` & `alist3-1.1.1/alist/main.py`

 * *Files identical despite different names*

### Comparing `alist3-1.1/alist/utils.py` & `alist3-1.1.1/alist/utils.py`

 * *Files identical despite different names*


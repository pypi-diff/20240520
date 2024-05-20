# Comparing `tmp/mongo_bridge-0.0.4.tar.gz` & `tmp/mongo_bridge-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_bridge-0.0.4.tar", last modified: Mon May 13 06:02:47 2024, max compression
+gzip compressed data, was "mongo_bridge-0.0.5.tar", last modified: Mon May 20 07:26:32 2024, max compression
```

## Comparing `mongo_bridge-0.0.4.tar` & `mongo_bridge-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:02:47.105471 mongo_bridge-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 06:02:26.000000 mongo_bridge-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-13 06:02:47.105471 mongo_bridge-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-13 06:02:26.000000 mongo_bridge-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 06:02:26.000000 mongo_bridge-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-13 06:02:47.105471 mongo_bridge-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-13 06:02:26.000000 mongo_bridge-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:02:47.101471 mongo_bridge-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:02:47.101471 mongo_bridge-0.0.4/src/mongo_bridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-13 06:02:47.000000 mongo_bridge-0.0.4/src/mongo_bridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-13 06:02:47.000000 mongo_bridge-0.0.4/src/mongo_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:02:47.000000 mongo_bridge-0.0.4/src/mongo_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-13 06:02:47.000000 mongo_bridge-0.0.4/src/mongo_bridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 06:02:47.000000 mongo_bridge-0.0.4/src/mongo_bridge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:02:47.101471 mongo_bridge-0.0.4/src/mongodb_connect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:02:26.000000 mongo_bridge-0.0.4/src/mongodb_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-05-13 06:02:26.000000 mongo_bridge-0.0.4/src/mongodb_connect/mongo_crud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:26:32.762884 mongo_bridge-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 07:26:04.000000 mongo_bridge-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-20 07:26:32.762884 mongo_bridge-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-20 07:26:04.000000 mongo_bridge-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-20 07:26:04.000000 mongo_bridge-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 07:26:32.762884 mongo_bridge-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 07:26:04.000000 mongo_bridge-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:26:32.758883 mongo_bridge-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:26:32.758883 mongo_bridge-0.0.5/src/mongo_bridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-20 07:26:32.000000 mongo_bridge-0.0.5/src/mongo_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-20 07:26:32.000000 mongo_bridge-0.0.5/src/mongo_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:26:32.000000 mongo_bridge-0.0.5/src/mongo_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-20 07:26:32.000000 mongo_bridge-0.0.5/src/mongo_bridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 07:26:32.000000 mongo_bridge-0.0.5/src/mongo_bridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:26:32.758883 mongo_bridge-0.0.5/src/mongodb_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:26:04.000000 mongo_bridge-0.0.5/src/mongodb_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-05-20 07:26:04.000000 mongo_bridge-0.0.5/src/mongodb_connect/mongo_crud.py
```

### Comparing `mongo_bridge-0.0.4/LICENSE` & `mongo_bridge-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo_bridge-0.0.4/setup.py` & `mongo_bridge-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()     
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 REPO_NAME = "MongoDB"
 PKG_NAME= "mongo_bridge"
 AUTHOR_USER_NAME = "Vansh353"
 AUTHOR_EMAIL = "vansh.malhotra@seaflux.tech"
 
 setup(
     name=PKG_NAME,
```

### Comparing `mongo_bridge-0.0.4/src/mongodb_connect/mongo_crud.py` & `mongo_bridge-0.0.5/src/mongodb_connect/mongo_crud.py`

 * *Files identical despite different names*


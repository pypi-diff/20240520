# Comparing `tmp/space_exploration_common_lib-0.0.5.tar.gz` & `tmp/space_exploration_common_lib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_exploration_common_lib-0.0.5.tar", last modified: Mon May 20 18:58:45 2024, max compression
+gzip compressed data, was "space_exploration_common_lib-0.0.6.tar", last modified: Mon May 20 19:11:05 2024, max compression
```

## Comparing `space_exploration_common_lib-0.0.5.tar` & `space_exploration_common_lib-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-20 18:58:44.000000 space_exploration_common_lib-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/space_exploration_common_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 18:58:45.000000 space_exploration_common_lib-0.0.5/space_exploration_common_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-20 18:58:45.000000 space_exploration_common_lib-0.0.5/space_exploration_common_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:58:45.000000 space_exploration_common_lib-0.0.5/space_exploration_common_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 18:58:45.000000 space_exploration_common_lib-0.0.5/space_exploration_common_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 18:58:45.000000 space_exploration_common_lib-0.0.5/space_exploration_common_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/model/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/model/Duration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/model/mission/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/model/mission/ProjectMercury.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/model/mission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:45.155718 space_exploration_common_lib-0.0.5/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 18:58:33.000000 space_exploration_common_lib-0.0.5/src/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/space_exploration_common_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 19:11:05.000000 space_exploration_common_lib-0.0.6/space_exploration_common_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-20 19:11:05.000000 space_exploration_common_lib-0.0.6/space_exploration_common_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:11:05.000000 space_exploration_common_lib-0.0.6/space_exploration_common_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 19:11:05.000000 space_exploration_common_lib-0.0.6/space_exploration_common_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 19:11:05.000000 space_exploration_common_lib-0.0.6/space_exploration_common_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/model/Duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/model/mission/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/model/mission/ProjectMercury.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/model/mission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:11:05.720242 space_exploration_common_lib-0.0.6/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 19:10:52.000000 space_exploration_common_lib-0.0.6/src/tests/test_dummy.py
```

### Comparing `space_exploration_common_lib-0.0.5/setup.py` & `space_exploration_common_lib-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import getenv
 
 setup(
     name='space-exploration-common-lib',
-    version=getenv('VERSION', default='v0.0.5'),
+    version=getenv('VERSION', '0.0.1'),
     packages=find_packages(exclude=['tests']),
     package_dir={'space_exploration_common_lib': 'src/space_exploration_common_lib'},
     python_requires='>=3.12, <4',
     include_package_data=True,
     install_requires=[
         'pydantic==2.7.1'
     ],
```

### Comparing `space_exploration_common_lib-0.0.5/space_exploration_common_lib.egg-info/SOURCES.txt` & `space_exploration_common_lib-0.0.6/space_exploration_common_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `space_exploration_common_lib-0.0.5/src/space_exploration_common_lib/model/mission/ProjectMercury.py` & `space_exploration_common_lib-0.0.6/src/space_exploration_common_lib/model/mission/ProjectMercury.py`

 * *Files identical despite different names*


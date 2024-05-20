# Comparing `tmp/shady-island-0.1.8.tar.gz` & `tmp/shady-island-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shady-island-0.1.8.tar", last modified: Mon Feb 12 01:20:46 2024, max compression
+gzip compressed data, was "shady-island-0.1.9.tar", last modified: Mon Feb 19 01:21:23 2024, max compression
```

## Comparing `shady-island-0.1.8.tar` & `shady-island-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 01:20:46.627068 shady-island-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-12 01:20:33.000000 shady-island-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-12 01:20:33.000000 shady-island-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-12 01:20:46.627068 shady-island-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-12 01:20:33.000000 shady-island-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-12 01:20:33.000000 shady-island-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 01:20:46.627068 shady-island-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-12 01:20:33.000000 shady-island-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 01:20:46.627068 shady-island-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 01:20:46.627068 shady-island-0.1.8/src/shady_island/
--rw-r--r--   0 runner    (1001) docker     (127)   301141 2024-02-12 01:20:33.000000 shady-island-0.1.8/src/shady_island/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 01:20:46.627068 shady-island-0.1.8/src/shady_island/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-12 01:20:33.000000 shady-island-0.1.8/src/shady_island/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   519161 2024-02-12 01:20:33.000000 shady-island-0.1.8/src/shady_island/_jsii/shady-island@0.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 01:20:33.000000 shady-island-0.1.8/src/shady_island/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 01:20:46.627068 shady-island-0.1.8/src/shady_island.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-12 01:20:46.000000 shady-island-0.1.8/src/shady_island.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-12 01:20:46.000000 shady-island-0.1.8/src/shady_island.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 01:20:46.000000 shady-island-0.1.8/src/shady_island.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-12 01:20:46.000000 shady-island-0.1.8/src/shady_island.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 01:20:46.000000 shady-island-0.1.8/src/shady_island.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:21:23.254367 shady-island-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-19 01:21:12.000000 shady-island-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-19 01:21:12.000000 shady-island-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-19 01:21:23.254367 shady-island-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-19 01:21:12.000000 shady-island-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-19 01:21:12.000000 shady-island-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 01:21:23.254367 shady-island-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-19 01:21:12.000000 shady-island-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:21:23.250367 shady-island-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:21:23.250367 shady-island-0.1.9/src/shady_island/
+-rw-r--r--   0 runner    (1001) docker     (127)   301141 2024-02-19 01:21:12.000000 shady-island-0.1.9/src/shady_island/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:21:23.250367 shady-island-0.1.9/src/shady_island/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-19 01:21:12.000000 shady-island-0.1.9/src/shady_island/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   519161 2024-02-19 01:21:12.000000 shady-island-0.1.9/src/shady_island/_jsii/shady-island@0.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 01:21:12.000000 shady-island-0.1.9/src/shady_island/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 01:21:23.250367 shady-island-0.1.9/src/shady_island.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-19 01:21:23.000000 shady-island-0.1.9/src/shady_island.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-19 01:21:23.000000 shady-island-0.1.9/src/shady_island.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 01:21:23.000000 shady-island-0.1.9/src/shady_island.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-19 01:21:23.000000 shady-island-0.1.9/src/shady_island.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-19 01:21:23.000000 shady-island-0.1.9/src/shady_island.egg-info/top_level.txt
```

### Comparing `shady-island-0.1.8/LICENSE` & `shady-island-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shady-island-0.1.8/PKG-INFO` & `shady-island-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shady-island
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utilities and constructs for the AWS CDK
 Home-page: https://libreworks.github.io/shady-island/
 Author: LibreWorks Contributors
 License: Apache-2.0
 Project-URL: Source, https://github.com:libreworks/shady-island.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `shady-island-0.1.8/README.md` & `shady-island-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `shady-island-0.1.8/setup.py` & `shady-island-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "shady-island",
-    "version": "0.1.8",
+    "version": "0.1.9",
     "description": "Utilities and constructs for the AWS CDK",
     "license": "Apache-2.0",
     "url": "https://libreworks.github.io/shady-island/",
     "long_description_content_type": "text/markdown",
     "author": "LibreWorks Contributors",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "shady_island",
         "shady_island._jsii"
     ],
     "package_data": {
         "shady_island._jsii": [
-            "shady-island@0.1.8.jsii.tgz"
+            "shady-island@0.1.9.jsii.tgz"
         ],
         "shady_island": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `shady-island-0.1.8/src/shady_island/__init__.py` & `shady-island-0.1.9/src/shady_island/__init__.py`

 * *Files identical despite different names*

### Comparing `shady-island-0.1.8/src/shady_island.egg-info/PKG-INFO` & `shady-island-0.1.9/src/shady_island.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shady-island
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utilities and constructs for the AWS CDK
 Home-page: https://libreworks.github.io/shady-island/
 Author: LibreWorks Contributors
 License: Apache-2.0
 Project-URL: Source, https://github.com:libreworks/shady-island.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


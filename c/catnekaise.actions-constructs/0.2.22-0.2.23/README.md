# Comparing `tmp/catnekaise.actions-constructs-0.2.22.tar.gz` & `tmp/catnekaise.actions-constructs-0.2.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnekaise.actions-constructs-0.2.22.tar", last modified: Fri May 10 11:31:45 2024, max compression
+gzip compressed data, was "catnekaise.actions-constructs-0.2.23.tar", last modified: Mon May 20 12:09:02 2024, max compression
```

## Comparing `catnekaise.actions-constructs-0.2.22.tar` & `catnekaise.actions-constructs-0.2.23.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    29969 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29028 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29969 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 11:31:45.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/
--rw-r--r--   0 runner    (1001) docker     (127)   220715 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:31:45.454337 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   111894 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/_jsii/actions-constructs@0.2.22.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:31:35.000000 catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:09:02.179528 catnekaise.actions-constructs-0.2.23/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 12:08:52.000000 catnekaise.actions-constructs-0.2.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 12:08:52.000000 catnekaise.actions-constructs-0.2.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    29969 2024-05-20 12:09:02.179528 catnekaise.actions-constructs-0.2.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29028 2024-05-20 12:08:52.000000 catnekaise.actions-constructs-0.2.23/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 12:08:52.000000 catnekaise.actions-constructs-0.2.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:09:02.179528 catnekaise.actions-constructs-0.2.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-20 12:08:52.000000 catnekaise.actions-constructs-0.2.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:09:02.179528 catnekaise.actions-constructs-0.2.23/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:09:02.179528 catnekaise.actions-constructs-0.2.23/src/catnekaise.actions_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29969 2024-05-20 12:09:02.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise.actions_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-20 12:09:02.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise.actions_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:09:02.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise.actions_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 12:09:02.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise.actions_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 12:09:02.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise.actions_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:09:02.179528 catnekaise.actions-constructs-0.2.23/src/catnekaise_actions_constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)   220715 2024-05-20 12:08:52.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise_actions_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:09:02.179528 catnekaise.actions-constructs-0.2.23/src/catnekaise_actions_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 12:08:52.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise_actions_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111893 2024-05-20 12:08:51.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise_actions_constructs/_jsii/actions-constructs@0.2.23.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:08:52.000000 catnekaise.actions-constructs-0.2.23/src/catnekaise_actions_constructs/py.typed
```

### Comparing `catnekaise.actions-constructs-0.2.22/LICENSE` & `catnekaise.actions-constructs-0.2.23/LICENSE`

 * *Files identical despite different names*

### Comparing `catnekaise.actions-constructs-0.2.22/PKG-INFO` & `catnekaise.actions-constructs-0.2.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.actions-constructs
-Version: 0.2.22
+Version: 0.2.23
 Summary: CDK Constructs for integrating GitHub Actions and AWS.
 Home-page: https://github.com/catnekaise/actions-constructs.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/actions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.actions-constructs-0.2.22/README.md` & `catnekaise.actions-constructs-0.2.23/README.md`

 * *Files identical despite different names*

### Comparing `catnekaise.actions-constructs-0.2.22/setup.py` & `catnekaise.actions-constructs-0.2.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "catnekaise.actions-constructs",
-    "version": "0.2.22",
+    "version": "0.2.23",
     "description": "CDK Constructs for integrating GitHub Actions and AWS.",
     "license": "Apache-2.0",
     "url": "https://github.com/catnekaise/actions-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel Jonsén<djonser1@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "catnekaise_actions_constructs",
         "catnekaise_actions_constructs._jsii"
     ],
     "package_data": {
         "catnekaise_actions_constructs._jsii": [
-            "actions-constructs@0.2.22.jsii.tgz"
+            "actions-constructs@0.2.23.jsii.tgz"
         ],
         "catnekaise_actions_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/PKG-INFO` & `catnekaise.actions-constructs-0.2.23/src/catnekaise.actions_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.actions-constructs
-Version: 0.2.22
+Version: 0.2.23
 Summary: CDK Constructs for integrating GitHub Actions and AWS.
 Home-page: https://github.com/catnekaise/actions-constructs.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/actions-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.actions-constructs-0.2.22/src/catnekaise.actions_constructs.egg-info/SOURCES.txt` & `catnekaise.actions-constructs-0.2.23/src/catnekaise.actions_constructs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/catnekaise.actions_constructs.egg-info/SOURCES.txt
 src/catnekaise.actions_constructs.egg-info/dependency_links.txt
 src/catnekaise.actions_constructs.egg-info/requires.txt
 src/catnekaise.actions_constructs.egg-info/top_level.txt
 src/catnekaise_actions_constructs/__init__.py
 src/catnekaise_actions_constructs/py.typed
 src/catnekaise_actions_constructs/_jsii/__init__.py
-src/catnekaise_actions_constructs/_jsii/actions-constructs@0.2.22.jsii.tgz
+src/catnekaise_actions_constructs/_jsii/actions-constructs@0.2.23.jsii.tgz
```

### Comparing `catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/__init__.py` & `catnekaise.actions-constructs-0.2.23/src/catnekaise_actions_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `catnekaise.actions-constructs-0.2.22/src/catnekaise_actions_constructs/_jsii/__init__.py` & `catnekaise.actions-constructs-0.2.23/src/catnekaise_actions_constructs/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import catnekaise_cdk_iam_utilities._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@catnekaise/actions-constructs",
-    "0.2.22",
+    "0.2.23",
     __name__[0:-6],
-    "actions-constructs@0.2.22.jsii.tgz",
+    "actions-constructs@0.2.23.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```


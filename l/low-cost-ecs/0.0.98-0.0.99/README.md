# Comparing `tmp/low-cost-ecs-0.0.98.tar.gz` & `tmp/low-cost-ecs-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "low-cost-ecs-0.0.98.tar", last modified: Mon Feb 12 00:19:04 2024, max compression
+gzip compressed data, was "low-cost-ecs-0.0.99.tar", last modified: Mon Feb 19 00:19:07 2024, max compression
```

## Comparing `low-cost-ecs-0.0.98.tar` & `low-cost-ecs-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:19:04.045047 low-cost-ecs-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-02-12 00:19:04.045047 low-cost-ecs-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 00:19:04.045047 low-cost-ecs-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:19:04.041047 low-cost-ecs-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:19:04.045047 low-cost-ecs-0.0.98/src/low_cost_ecs/
--rw-r--r--   0 runner    (1001) docker     (127)    33973 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/src/low_cost_ecs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:19:04.045047 low-cost-ecs-0.0.98/src/low_cost_ecs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/src/low_cost_ecs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34936 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/src/low_cost_ecs/_jsii/low-cost-ecs@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 00:18:52.000000 low-cost-ecs-0.0.98/src/low_cost_ecs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 00:19:04.045047 low-cost-ecs-0.0.98/src/low_cost_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-02-12 00:19:04.000000 low-cost-ecs-0.0.98/src/low_cost_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-12 00:19:04.000000 low-cost-ecs-0.0.98/src/low_cost_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 00:19:04.000000 low-cost-ecs-0.0.98/src/low_cost_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-12 00:19:04.000000 low-cost-ecs-0.0.98/src/low_cost_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-12 00:19:04.000000 low-cost-ecs-0.0.98/src/low_cost_ecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:19:07.491192 low-cost-ecs-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-02-19 00:19:07.491192 low-cost-ecs-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 00:19:07.491192 low-cost-ecs-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:19:07.491192 low-cost-ecs-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:19:07.491192 low-cost-ecs-0.0.99/src/low_cost_ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)    33973 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/src/low_cost_ecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:19:07.491192 low-cost-ecs-0.0.99/src/low_cost_ecs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/src/low_cost_ecs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34938 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/src/low_cost_ecs/_jsii/low-cost-ecs@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 00:18:54.000000 low-cost-ecs-0.0.99/src/low_cost_ecs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:19:07.491192 low-cost-ecs-0.0.99/src/low_cost_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-02-19 00:19:07.000000 low-cost-ecs-0.0.99/src/low_cost_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-19 00:19:07.000000 low-cost-ecs-0.0.99/src/low_cost_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 00:19:07.000000 low-cost-ecs-0.0.99/src/low_cost_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-19 00:19:07.000000 low-cost-ecs-0.0.99/src/low_cost_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-19 00:19:07.000000 low-cost-ecs-0.0.99/src/low_cost_ecs.egg-info/top_level.txt
```

### Comparing `low-cost-ecs-0.0.98/LICENSE` & `low-cost-ecs-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `low-cost-ecs-0.0.98/PKG-INFO` & `low-cost-ecs-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: low-cost-ecs
-Version: 0.0.98
+Version: 0.0.99
 Summary: Easy and low-cost ECS on EC2 server without a load balancer
 Home-page: https://github.com/rajyan/low-cost-ecs.git
 Author: Yohta Kimura<kitakita7617@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/rajyan/low-cost-ecs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `low-cost-ecs-0.0.98/README.md` & `low-cost-ecs-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `low-cost-ecs-0.0.98/setup.py` & `low-cost-ecs-0.0.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "low-cost-ecs",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "Easy and low-cost ECS on EC2 server without a load balancer",
     "license": "MIT",
     "url": "https://github.com/rajyan/low-cost-ecs.git",
     "long_description_content_type": "text/markdown",
     "author": "Yohta Kimura<kitakita7617@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "low_cost_ecs",
         "low_cost_ecs._jsii"
     ],
     "package_data": {
         "low_cost_ecs._jsii": [
-            "low-cost-ecs@0.0.98.jsii.tgz"
+            "low-cost-ecs@0.0.99.jsii.tgz"
         ],
         "low_cost_ecs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `low-cost-ecs-0.0.98/src/low_cost_ecs/__init__.py` & `low-cost-ecs-0.0.99/src/low_cost_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `low-cost-ecs-0.0.98/src/low_cost_ecs.egg-info/PKG-INFO` & `low-cost-ecs-0.0.99/src/low_cost_ecs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: low-cost-ecs
-Version: 0.0.98
+Version: 0.0.99
 Summary: Easy and low-cost ECS on EC2 server without a load balancer
 Home-page: https://github.com/rajyan/low-cost-ecs.git
 Author: Yohta Kimura<kitakita7617@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/rajyan/low-cost-ecs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


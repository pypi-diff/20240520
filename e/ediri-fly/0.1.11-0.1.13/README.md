# Comparing `tmp/ediri_fly-0.1.11.tar.gz` & `tmp/ediri_fly-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_fly-0.1.11.tar", last modified: Sun Mar  3 16:00:39 2024, max compression
+gzip compressed data, was "ediri_fly-0.1.13.tar", last modified: Mon May 20 13:09:04 2024, max compression
```

## Comparing `ediri_fly-0.1.11.tar` & `ediri_fly-0.1.13.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:00:39.897721 ediri_fly-0.1.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-03 16:00:39.897721 ediri_fly-0.1.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:00:39.897721 ediri_fly-0.1.11/ediri_fly/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/cert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:00:39.897721 ediri_fly-0.1.11/ediri_fly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/get_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/get_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    27814 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:00:39.897721 ediri_fly-0.1.11/ediri_fly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/ediri_fly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 16:00:39.897721 ediri_fly-0.1.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-03 16:00:39.000000 ediri_fly-0.1.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:09:04.632824 ediri_fly-0.1.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-20 13:09:04.632824 ediri_fly-0.1.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:09:04.632824 ediri_fly-0.1.13/ediri_fly/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:09:04.632824 ediri_fly-0.1.13/ediri_fly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/get_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/get_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27814 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:09:04.632824 ediri_fly-0.1.13/ediri_fly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/ediri_fly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:09:04.632824 ediri_fly-0.1.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-20 13:09:04.000000 ediri_fly-0.1.13/setup.py
```

### Comparing `ediri_fly-0.1.11/PKG-INFO` & `ediri_fly-0.1.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri_fly
-Version: 0.1.11
+Version: 0.1.13
 Summary: A Pulumi package for creating and managing Fly.io resources.
 Home-page: https://github.com/dirien/pulumi-fly
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-fly
 Keywords: pulumi fly category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `ediri_fly-0.1.11/README.md` & `ediri_fly-0.1.13/README.md`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/__init__.py` & `ediri_fly-0.1.13/ediri_fly/__init__.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/_inputs.py` & `ediri_fly-0.1.13/ediri_fly/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/_utilities.py` & `ediri_fly-0.1.13/ediri_fly/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/app.py` & `ediri_fly-0.1.13/ediri_fly/app.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/cert.py` & `ediri_fly-0.1.13/ediri_fly/cert.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/config/vars.py` & `ediri_fly-0.1.13/ediri_fly/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/get_app.py` & `ediri_fly-0.1.13/ediri_fly/get_app.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/get_cert.py` & `ediri_fly-0.1.13/ediri_fly/get_cert.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/get_ip.py` & `ediri_fly-0.1.13/ediri_fly/get_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/get_volume.py` & `ediri_fly-0.1.13/ediri_fly/get_volume.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/ip.py` & `ediri_fly-0.1.13/ediri_fly/ip.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/machine.py` & `ediri_fly-0.1.13/ediri_fly/machine.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/outputs.py` & `ediri_fly-0.1.13/ediri_fly/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/provider.py` & `ediri_fly-0.1.13/ediri_fly/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly/volume.py` & `ediri_fly-0.1.13/ediri_fly/volume.py`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/ediri_fly.egg-info/PKG-INFO` & `ediri_fly-0.1.13/ediri_fly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri-fly
-Version: 0.1.11
+Version: 0.1.13
 Summary: A Pulumi package for creating and managing Fly.io resources.
 Home-page: https://github.com/dirien/pulumi-fly
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-fly
 Keywords: pulumi fly category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `ediri_fly-0.1.11/ediri_fly.egg-info/SOURCES.txt` & `ediri_fly-0.1.13/ediri_fly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ediri_fly-0.1.11/setup.py` & `ediri_fly-0.1.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.11"
+VERSION = "0.1.13"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "fly Pulumi Package - Development Version"
```


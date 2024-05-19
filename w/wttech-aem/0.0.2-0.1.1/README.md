# Comparing `tmp/wttech_aem-0.0.2.tar.gz` & `tmp/wttech_aem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wttech_aem-0.0.2.tar", last modified: Sun May 19 20:32:42 2024, max compression
+gzip compressed data, was "wttech_aem-0.1.1.tar", last modified: Sun May 19 22:41:43 2024, max compression
```

## Comparing `wttech_aem-0.0.2.tar` & `wttech_aem-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:32:42.363521 wttech_aem-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-19 20:32:42.363521 wttech_aem-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:32:42.363521 wttech_aem-0.0.2/setup.cfg
--rw-------   0 runner    (1001) docker     (127)     1298 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:32:42.359521 wttech_aem-0.0.2/wttech_aem/
--rw-------   0 runner    (1001) docker     (127)      786 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9269 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:32:42.363521 wttech_aem-0.0.2/wttech_aem/compose/
--rw-------   0 runner    (1001) docker     (127)      320 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/compose/__init__.py
--rw-------   0 runner    (1001) docker     (127)    14453 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/compose/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9345 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/compose/instance.py
--rw-------   0 runner    (1001) docker     (127)    13589 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/compose/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2723 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/provider.py
--rw-------   0 runner    (1001) docker     (127)       97 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:32:42.359521 wttech_aem-0.0.2/wttech_aem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 20:32:42.000000 wttech_aem-0.0.2/wttech_aem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:41:43.312013 wttech_aem-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-19 22:41:43.312013 wttech_aem-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:41:43.312013 wttech_aem-0.1.1/setup.cfg
+-rw-------   0 runner    (1001) docker     (127)     1298 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:41:43.308013 wttech_aem-0.1.1/wttech_aem/
+-rw-------   0 runner    (1001) docker     (127)      786 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9269 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:41:43.312013 wttech_aem-0.1.1/wttech_aem/compose/
+-rw-------   0 runner    (1001) docker     (127)      320 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/compose/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    14453 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/compose/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9345 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/compose/instance.py
+-rw-------   0 runner    (1001) docker     (127)    13589 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/compose/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2723 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/provider.py
+-rw-------   0 runner    (1001) docker     (127)       97 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:41:43.312013 wttech_aem-0.1.1/wttech_aem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 22:41:43.000000 wttech_aem-0.1.1/wttech_aem.egg-info/top_level.txt
```

### Comparing `wttech_aem-0.0.2/LICENSE` & `wttech_aem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.0.2/PKG-INFO` & `wttech_aem-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wttech_aem
-Version: 0.0.2
+Version: 0.1.1
 Summary: Easily manage AEM instances in the cloud without a deep dev-ops knowledge
 Home-page: https://github.com/wttech/pulumi-aem
 License: Apache-2.0
 Project-URL: Repository, https://github.com/wttech/pulumi-aem
 Keywords: pulumi aem aemc cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `wttech_aem-0.0.2/README.md` & `wttech_aem-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.0.2/setup.py` & `wttech_aem-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.2"
+VERSION = "0.1.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "aem Pulumi Package - Development Version"
```

### Comparing `wttech_aem-0.0.2/wttech_aem/__init__.py` & `wttech_aem-0.1.1/wttech_aem/__init__.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.0.2/wttech_aem/_utilities.py` & `wttech_aem-0.1.1/wttech_aem/_utilities.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.0.2/wttech_aem/compose/_inputs.py` & `wttech_aem-0.1.1/wttech_aem/compose/_inputs.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.0.2/wttech_aem/compose/instance.py` & `wttech_aem-0.1.1/wttech_aem/compose/instance.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.0.2/wttech_aem/compose/outputs.py` & `wttech_aem-0.1.1/wttech_aem/compose/outputs.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.0.2/wttech_aem/provider.py` & `wttech_aem-0.1.1/wttech_aem/provider.py`

 * *Files identical despite different names*

### Comparing `wttech_aem-0.0.2/wttech_aem.egg-info/PKG-INFO` & `wttech_aem-0.1.1/wttech_aem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wttech-aem
-Version: 0.0.2
+Version: 0.1.1
 Summary: Easily manage AEM instances in the cloud without a deep dev-ops knowledge
 Home-page: https://github.com/wttech/pulumi-aem
 License: Apache-2.0
 Project-URL: Repository, https://github.com/wttech/pulumi-aem
 Keywords: pulumi aem aemc cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```


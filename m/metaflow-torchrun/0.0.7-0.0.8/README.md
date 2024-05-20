# Comparing `tmp/metaflow_torchrun-0.0.7.tar.gz` & `tmp/metaflow_torchrun-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow_torchrun-0.0.7.tar", last modified: Fri May  3 18:40:45 2024, max compression
+gzip compressed data, was "metaflow_torchrun-0.0.8.tar", last modified: Mon May 20 18:54:53 2024, max compression
```

## Comparing `metaflow_torchrun-0.0.7.tar` & `metaflow_torchrun-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.474519 metaflow_torchrun-0.0.7/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.474519 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.474519 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/mfextinit_torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-03 18:40:45.000000 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-03 18:40:45.000000 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:40:45.000000 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 18:40:45.000000 metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:40:45.478519 metaflow_torchrun-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 18:40:37.000000 metaflow_torchrun-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:54:53.523763 metaflow_torchrun-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-20 18:54:53.523763 metaflow_torchrun-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:54:53.519763 metaflow_torchrun-0.0.8/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:54:53.519763 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:54:53.523763 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/mfextinit_torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:54:53.523763 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:54:53.523763 metaflow_torchrun-0.0.8/metaflow_torchrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-20 18:54:53.000000 metaflow_torchrun-0.0.8/metaflow_torchrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-20 18:54:53.000000 metaflow_torchrun-0.0.8/metaflow_torchrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:54:53.000000 metaflow_torchrun-0.0.8/metaflow_torchrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 18:54:53.000000 metaflow_torchrun-0.0.8/metaflow_torchrun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:54:53.523763 metaflow_torchrun-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-20 18:54:44.000000 metaflow_torchrun-0.0.8/setup.py
```

### Comparing `metaflow_torchrun-0.0.7/PKG-INFO` & `metaflow_torchrun-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-torchrun
-Version: 0.0.7
+Version: 0.0.8
 Summary: An EXPERIMENTAL torchrun decorator for Metaflow
 Author: Eddie Mattia
 Author-email: eddie@outerbounds.com
 Description-Content-Type: text/markdown
 
 # Metaflow torchrun decorator
```

### Comparing `metaflow_torchrun-0.0.7/README.md` & `metaflow_torchrun-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py` & `metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py` & `metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py` & `metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         cmd.extend(["--rdzv_endpoint", "%s:%s" % (self.torchrun_args["master_addr"], self.torchrun_args["master_port"])])
 
         # Construct rest of command starting with the entrypoint.
         if entrypoint is not None:
             cmd.append(entrypoint)
         else:
             raise MetaflowException(
-                "current.deepspeed.run(..., entrypoint=<SCRIPT>, ...) arg must be specified."
+                "current.torchrun.run(..., entrypoint=<SCRIPT>, ...) arg must be specified."
             )
         if entrypoint_args is not None and isinstance(entrypoint_args, dict):
             cmd.extend(_dict_to_args(entrypoint_args))
         elif entrypoint_args is not None and isinstance(entrypoint_args, list):
             cmd.extend(entrypoint_args)
 
         # Launch the Torchrun process and stream logs.
```

### Comparing `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py` & `metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/status_notifier.py`

 * *Files identical despite different names*

### Comparing `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py` & `metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/torch_distributed_setup.py`

 * *Files identical despite different names*

### Comparing `metaflow_torchrun-0.0.7/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py` & `metaflow_torchrun-0.0.8/metaflow_extensions/torchrun/plugins/torchrun_libs/torchrun_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/PKG-INFO` & `metaflow_torchrun-0.0.8/metaflow_torchrun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-torchrun
-Version: 0.0.7
+Version: 0.0.8
 Summary: An EXPERIMENTAL torchrun decorator for Metaflow
 Author: Eddie Mattia
 Author-email: eddie@outerbounds.com
 Description-Content-Type: text/markdown
 
 # Metaflow torchrun decorator
```

### Comparing `metaflow_torchrun-0.0.7/metaflow_torchrun.egg-info/SOURCES.txt` & `metaflow_torchrun-0.0.8/metaflow_torchrun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow_torchrun-0.0.7/setup.py` & `metaflow_torchrun-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "0.0.7"
+version = "0.0.8"
 
 setup(
     name="metaflow-torchrun",
     version=version,
     description="An EXPERIMENTAL torchrun decorator for Metaflow",
     author="Eddie Mattia",
     author_email="eddie@outerbounds.com",
```


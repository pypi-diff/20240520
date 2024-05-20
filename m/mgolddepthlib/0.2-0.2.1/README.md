# Comparing `tmp/mgolddepthlib-0.2.tar.gz` & `tmp/mgolddepthlib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgolddepthlib-0.2.tar", last modified: Mon May 20 02:58:37 2024, max compression
+gzip compressed data, was "mgolddepthlib-0.2.1.tar", last modified: Mon May 20 03:33:46 2024, max compression
```

## Comparing `mgolddepthlib-0.2.tar` & `mgolddepthlib-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 02:58:37.061658 mgolddepthlib-0.2/
--rw-r--r--   0 db         (502) staff       (20)      109 2024-05-20 02:58:37.061364 mgolddepthlib-0.2/PKG-INFO
--rw-r--r--   0 db         (502) staff       (20)       51 2024-05-20 01:34:57.000000 mgolddepthlib-0.2/README.md
-drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 02:58:37.059330 mgolddepthlib-0.2/mgolddepthlib.egg-info/
--rw-r--r--   0 db         (502) staff       (20)      109 2024-05-20 02:58:37.000000 mgolddepthlib-0.2/mgolddepthlib.egg-info/PKG-INFO
--rw-r--r--   0 db         (502) staff       (20)      429 2024-05-20 02:58:37.000000 mgolddepthlib-0.2/mgolddepthlib.egg-info/SOURCES.txt
--rw-r--r--   0 db         (502) staff       (20)        1 2024-05-20 02:58:37.000000 mgolddepthlib-0.2/mgolddepthlib.egg-info/dependency_links.txt
--rw-r--r--   0 db         (502) staff       (20)       17 2024-05-20 02:58:37.000000 mgolddepthlib-0.2/mgolddepthlib.egg-info/top_level.txt
-drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 02:58:37.059898 mgolddepthlib-0.2/model/
--rw-rw-r--   0 db         (502) staff       (20)        0 2024-05-20 00:57:45.000000 mgolddepthlib-0.2/model/__init__.py
--rw-rw-r--   0 db         (502) staff       (20)    12142 2024-05-20 00:57:45.000000 mgolddepthlib-0.2/model/marigold_pipeline.py
--rw-rw-r--   0 db         (502) staff       (20)      994 2024-05-20 00:57:45.000000 mgolddepthlib-0.2/model/rgb_encoder.py
--rw-rw-r--   0 db         (502) staff       (20)     1640 2024-05-20 00:57:45.000000 mgolddepthlib-0.2/model/stacked_depth_AE.py
-drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 02:58:37.060109 mgolddepthlib-0.2/mylib/
--rw-rw-r--   0 db         (502) staff       (20)        0 2024-05-20 01:02:58.000000 mgolddepthlib-0.2/mylib/__init__.py
--rw-r--r--   0 db         (502) staff       (20)      360 2024-05-20 01:21:46.000000 mgolddepthlib-0.2/mylib/myfunctions.py
--rw-r--r--   0 db         (502) staff       (20)       38 2024-05-20 02:58:37.061717 mgolddepthlib-0.2/setup.cfg
--rw-r--r--   0 db         (502) staff       (20)      238 2024-05-20 02:58:21.000000 mgolddepthlib-0.2/setup.py
-drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 02:58:37.060242 mgolddepthlib-0.2/tests/
--rw-r--r--   0 db         (502) staff       (20)      186 2024-05-20 01:08:02.000000 mgolddepthlib-0.2/tests/test_mylib.py
-drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 02:58:37.061109 mgolddepthlib-0.2/util/
--rw-rw-r--   0 db         (502) staff       (20)        0 2024-05-20 01:24:40.000000 mgolddepthlib-0.2/util/__init__.py
--rw-rw-r--   0 db         (502) staff       (20)     1205 2024-05-20 00:57:45.000000 mgolddepthlib-0.2/util/batchsize.py
--rw-rw-r--   0 db         (502) staff       (20)     3842 2024-05-20 00:57:45.000000 mgolddepthlib-0.2/util/ensemble.py
--rw-rw-r--   0 db         (502) staff       (20)     2363 2024-05-20 01:37:58.000000 mgolddepthlib-0.2/util/flow_estimation.py
--rw-rw-r--   0 db         (502) staff       (20)     2149 2024-05-20 00:57:45.000000 mgolddepthlib-0.2/util/image_util.py
--rw-rw-r--   0 db         (502) staff       (20)      245 2024-05-20 00:57:45.000000 mgolddepthlib-0.2/util/seed_all.py
+drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 03:33:46.590303 mgolddepthlib-0.2.1/
+-rw-r--r--   0 db         (502) staff       (20)     1073 2024-05-20 03:24:47.000000 mgolddepthlib-0.2.1/LICENSE
+-rw-r--r--   0 db         (502) staff       (20)      150 2024-05-20 03:33:46.590070 mgolddepthlib-0.2.1/PKG-INFO
+drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 03:33:46.587616 mgolddepthlib-0.2.1/mgolddepthlib/
+-rw-rw-r--   0 db         (502) staff       (20)        0 2024-05-20 01:02:58.000000 mgolddepthlib-0.2.1/mgolddepthlib/__init__.py
+drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 03:33:46.588754 mgolddepthlib-0.2.1/mgolddepthlib/model/
+-rw-rw-r--   0 db         (502) staff       (20)        0 2024-05-20 00:57:45.000000 mgolddepthlib-0.2.1/mgolddepthlib/model/__init__.py
+-rw-rw-r--   0 db         (502) staff       (20)    12142 2024-05-20 00:57:45.000000 mgolddepthlib-0.2.1/mgolddepthlib/model/marigold_pipeline.py
+-rw-rw-r--   0 db         (502) staff       (20)      994 2024-05-20 00:57:45.000000 mgolddepthlib-0.2.1/mgolddepthlib/model/rgb_encoder.py
+-rw-rw-r--   0 db         (502) staff       (20)     1640 2024-05-20 00:57:45.000000 mgolddepthlib-0.2.1/mgolddepthlib/model/stacked_depth_AE.py
+drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 03:33:46.589835 mgolddepthlib-0.2.1/mgolddepthlib/util/
+-rw-rw-r--   0 db         (502) staff       (20)        0 2024-05-20 01:24:40.000000 mgolddepthlib-0.2.1/mgolddepthlib/util/__init__.py
+-rw-rw-r--   0 db         (502) staff       (20)     1205 2024-05-20 00:57:45.000000 mgolddepthlib-0.2.1/mgolddepthlib/util/batchsize.py
+-rw-rw-r--   0 db         (502) staff       (20)     3842 2024-05-20 00:57:45.000000 mgolddepthlib-0.2.1/mgolddepthlib/util/ensemble.py
+-rw-rw-r--   0 db         (502) staff       (20)     2363 2024-05-20 01:37:58.000000 mgolddepthlib-0.2.1/mgolddepthlib/util/flow_estimation.py
+-rw-rw-r--   0 db         (502) staff       (20)     2149 2024-05-20 00:57:45.000000 mgolddepthlib-0.2.1/mgolddepthlib/util/image_util.py
+-rw-rw-r--   0 db         (502) staff       (20)      245 2024-05-20 00:57:45.000000 mgolddepthlib-0.2.1/mgolddepthlib/util/seed_all.py
+-rw-r--r--   0 db         (502) staff       (20)      408 2024-05-20 03:32:43.000000 mgolddepthlib-0.2.1/mgolddepthlib/wp.py
+drwxr-xr-x   0 db         (502) staff       (20)        0 2024-05-20 03:33:46.588143 mgolddepthlib-0.2.1/mgolddepthlib.egg-info/
+-rw-r--r--   0 db         (502) staff       (20)      150 2024-05-20 03:33:46.000000 mgolddepthlib-0.2.1/mgolddepthlib.egg-info/PKG-INFO
+-rw-r--r--   0 db         (502) staff       (20)      554 2024-05-20 03:33:46.000000 mgolddepthlib-0.2.1/mgolddepthlib.egg-info/SOURCES.txt
+-rw-r--r--   0 db         (502) staff       (20)        1 2024-05-20 03:33:46.000000 mgolddepthlib-0.2.1/mgolddepthlib.egg-info/dependency_links.txt
+-rw-r--r--   0 db         (502) staff       (20)       14 2024-05-20 03:33:46.000000 mgolddepthlib-0.2.1/mgolddepthlib.egg-info/top_level.txt
+-rw-r--r--   0 db         (502) staff       (20)       38 2024-05-20 03:33:46.590355 mgolddepthlib-0.2.1/setup.cfg
+-rw-r--r--   0 db         (502) staff       (20)      229 2024-05-20 03:31:46.000000 mgolddepthlib-0.2.1/setup.py
```

### Comparing `mgolddepthlib-0.2/model/marigold_pipeline.py` & `mgolddepthlib-0.2.1/mgolddepthlib/model/marigold_pipeline.py`

 * *Files identical despite different names*

### Comparing `mgolddepthlib-0.2/model/rgb_encoder.py` & `mgolddepthlib-0.2.1/mgolddepthlib/model/rgb_encoder.py`

 * *Files identical despite different names*

### Comparing `mgolddepthlib-0.2/model/stacked_depth_AE.py` & `mgolddepthlib-0.2.1/mgolddepthlib/model/stacked_depth_AE.py`

 * *Files identical despite different names*

### Comparing `mgolddepthlib-0.2/util/batchsize.py` & `mgolddepthlib-0.2.1/mgolddepthlib/util/batchsize.py`

 * *Files identical despite different names*

### Comparing `mgolddepthlib-0.2/util/ensemble.py` & `mgolddepthlib-0.2.1/mgolddepthlib/util/ensemble.py`

 * *Files identical despite different names*

### Comparing `mgolddepthlib-0.2/util/flow_estimation.py` & `mgolddepthlib-0.2.1/mgolddepthlib/util/flow_estimation.py`

 * *Files identical despite different names*

### Comparing `mgolddepthlib-0.2/util/image_util.py` & `mgolddepthlib-0.2.1/mgolddepthlib/util/image_util.py`

 * *Files identical despite different names*


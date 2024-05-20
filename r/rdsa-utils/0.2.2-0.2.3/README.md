# Comparing `tmp/rdsa_utils-0.2.2.tar.gz` & `tmp/rdsa_utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdsa_utils-0.2.2.tar", last modified: Tue May 14 11:56:40 2024, max compression
+gzip compressed data, was "rdsa_utils-0.2.3.tar", last modified: Mon May 20 07:46:37 2024, max compression
```

## Comparing `rdsa_utils-0.2.2.tar` & `rdsa_utils-0.2.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/cdp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/hdfs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/impala.py
--rw-r--r--   0 runner    (1001) docker     (127)    23018 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/s3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/cdp/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/cdp/io/pipeline_runlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/gcp/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/helpers/gcp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.268249 rdsa_utils-0.2.2/rdsa_utils/gcp/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/io/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/gcp/io/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/rdsa_utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/helpers/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/helpers/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/rdsa_utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/rdsa_utils/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/methods/averaging_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/rdsa_utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/rdsa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 11:56:40.000000 rdsa_utils-0.2.2/rdsa_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-14 11:56:40.276249 rdsa_utils-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:40.272249 rdsa_utils-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-14 11:56:36.000000 rdsa_utils-0.2.2/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.708737 rdsa_utils-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-20 07:46:37.708737 rdsa_utils-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.700736 rdsa_utils-0.2.3/rdsa_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.700736 rdsa_utils-0.2.3/rdsa_utils/cdp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.700736 rdsa_utils-0.2.3/rdsa_utils/cdp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/helpers/hdfs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/helpers/impala.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23236 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/helpers/s3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/rdsa_utils/cdp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/cdp/io/pipeline_runlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/rdsa_utils/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/gcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/rdsa_utils/gcp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/gcp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/gcp/helpers/gcp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/rdsa_utils/gcp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/gcp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/gcp/io/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/gcp/io/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/rdsa_utils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/helpers/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/helpers/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/rdsa_utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/rdsa_utils/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/methods/averaging_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/rdsa_utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/rdsa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-20 07:46:37.000000 rdsa_utils-0.2.3/rdsa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 07:46:37.000000 rdsa_utils-0.2.3/rdsa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:46:37.000000 rdsa_utils-0.2.3/rdsa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-20 07:46:37.000000 rdsa_utils-0.2.3/rdsa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 07:46:37.000000 rdsa_utils-0.2.3/rdsa_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-20 07:46:37.708737 rdsa_utils-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:46:37.704737 rdsa_utils-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-20 07:46:33.000000 rdsa_utils-0.2.3/tests/test_validation.py
```

### Comparing `rdsa_utils-0.2.2/LICENSE` & `rdsa_utils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/PKG-INFO` & `rdsa_utils-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdsa-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 Home-page: https://github.com/ONSdigital/rdsa-utils
 Author: Reproducible Data Science & Analysis, ONS
 Author-email: Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rdsa_utils-0.2.2/README.md` & `rdsa_utils-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/hdfs_utils.py` & `rdsa_utils-0.2.3/rdsa_utils/cdp/helpers/hdfs_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/impala.py` & `rdsa_utils-0.2.3/rdsa_utils/cdp/helpers/impala.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/cdp/helpers/s3_utils.py` & `rdsa_utils-0.2.3/rdsa_utils/cdp/helpers/s3_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 Note:
 - The `raz-client` library is required only when running in a
   managed Cloudera environment.
 - You can install it using `pip install raz-client` when needed.
 ```
 """
-
 import logging
 from pathlib import Path
 from typing import List, Optional
 
 import boto3
 
 from rdsa_utils.exceptions import InvalidBucketNameError
@@ -34,15 +33,15 @@
 
 
 def remove_leading_slash(text: str) -> str:
     """Remove the leading forward slash from a string if present.
 
     Parameters
     ----------
-    text : str
+    text
         The text from which the leading slash will be removed.
 
     Returns
     -------
     str
         The text stripped of its leading slash.
 
@@ -55,15 +54,15 @@
 
 
 def validate_bucket_name(bucket_name: str) -> str:
     """Validate the format of an AWS S3 bucket name according to AWS rules.
 
     Parameters
     ----------
-    bucket_name : str
+    bucket_name
         The name of the bucket to validate.
 
     Returns
     -------
     str
         The validated bucket name if valid.
 
@@ -106,37 +105,41 @@
     if '/' in bucket_name:
         error_msg = 'Bucket name must not contain forward slashes.'
         raise InvalidBucketNameError(error_msg)
 
     return bucket_name
 
 
-def is_s3_directory(client: boto3.client, bucket_name: str, key: str) -> bool:
+def is_s3_directory(
+    client: boto3.client,
+    bucket_name: str,
+    object_name: str,
+) -> bool:
     """Check if an AWS S3 key is a directory by listing its contents.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    bucket_name : str
+    bucket_name
         The name of the S3 bucket.
-    key : str
-        The S3 object key to check.
+    object_name
+        The S3 object name to check.
 
     Returns
     -------
     bool
         True if the key represents a directory, False otherwise.
     """
-    if not key.endswith('/'):
-        key += '/'
+    if not object_name.endswith('/'):
+        object_name += '/'
     try:
         response = client.list_objects_v2(
             Bucket=bucket_name,
-            Prefix=key,
+            Prefix=object_name,
             Delimiter='/',
             MaxKeys=1,
         )
         if 'Contents' in response or 'CommonPrefixes' in response:
             return True
         else:
             return False
@@ -150,19 +153,19 @@
     bucket_name: str,
     object_name: str,
 ) -> bool:
     """Check if a specific file exists in an AWS S3 bucket.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client.
-    bucket_name : str
+    bucket_name
         The name of the bucket.
-    object_name : str
+    object_name
         The S3 object name to check for existence.
 
     Returns
     -------
     bool
         True if the file exists, otherwise False.
 
@@ -185,32 +188,32 @@
             logger.error(f'Failed to check file existence: {str(e)}')
             return False
 
 
 def upload_file(
     client: boto3.client,
     bucket_name: str,
-    local_file_path: str,
-    s3_object_name: Optional[str] = None,
+    local_path: str,
+    object_name: Optional[str] = None,
     overwrite: bool = False,
 ) -> bool:
     """Upload a file to an Amazon S3 bucket from local directory.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    bucket_name : str
+    bucket_name
         The name of the target S3 bucket.
-    local_file_path : str
+    local_path
         The file path on the local system to upload.
-    s3_object_name : Optional[str]
+    object_name
         The target S3 object name. If None, uses the base name of
         the local file path.
-    overwrite : bool, optional
+    overwrite
         If True, the existing file on S3 will be overwritten.
 
     Returns
     -------
     bool
         True if the file was uploaded successfully, False otherwise.
 
@@ -223,62 +226,62 @@
     ...     '/path/to/file.txt',
     ...     'folder/s3_file.txt'
     ... )
     True
     """
     bucket_name = validate_bucket_name(bucket_name)
 
-    local_file_path = Path(local_file_path)
-    if not local_file_path.exists():
+    local_path = Path(local_path)
+    if not local_path.exists():
         logger.error('Local file does not exist.')
         return False
 
-    if s3_object_name is None:
-        s3_object_name = local_file_path.name
+    if object_name is None:
+        object_name = local_path.name
 
-    s3_object_name = remove_leading_slash(s3_object_name)
+    object_name = remove_leading_slash(object_name)
 
-    if not overwrite and file_exists(client, bucket_name, s3_object_name):
+    if not overwrite and file_exists(client, bucket_name, object_name):
         logger.error('File already exists in the bucket.')
         return False
 
     try:
-        client.upload_file(str(local_file_path), bucket_name, s3_object_name)
+        client.upload_file(str(local_path), bucket_name, object_name)
         logger.info(
-            f'Uploaded {local_file_path} to {bucket_name}/{s3_object_name}',
+            f'Uploaded {local_path} to {bucket_name}/{object_name}',
         )
         return True
     except FileNotFoundError:
         logger.error('The local file was not found.')
         return False
     except client.exceptions.NoCredentialsError:
         logger.error('Credentials not available.')
         return False
 
 
 def download_file(
     client: boto3.client,
     bucket_name: str,
-    s3_object_name: str,
-    local_file_path: str,
+    object_name: str,
+    local_path: str,
     overwrite: bool = False,
 ) -> bool:
     """Download a file from an AWS S3 bucket to a local directory.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    bucket_name : str
+    bucket_name
         The name of the S3 bucket from which to download the file.
-    s3_object_name : str
+    object_name
         The S3 object name of the file to download.
-    local_file_path : str
+    local_path
         The local file path where the downloaded file will be saved.
-    overwrite : bool, optional
+    overwrite
         If True, overwrite the local file if it exists.
 
     Returns
     -------
     bool
         True if the file was downloaded successfully, False otherwise.
 
@@ -291,32 +294,31 @@
     ...     'folder/s3_file.txt',
     ...     '/path/to/download.txt'
     ... )
     True
     """
     bucket_name = validate_bucket_name(bucket_name)
 
-    local_file_path = Path(local_file_path)
+    local_path = Path(local_path)
 
-    if not overwrite and local_file_path.exists():
+    if not overwrite and local_path.exists():
         logger.error('Local file already exists.')
         return False
 
-    s3_object_name = remove_leading_slash(s3_object_name)
+    object_name = remove_leading_slash(object_name)
 
-    if file_exists(client, bucket_name, s3_object_name):
+    if file_exists(client, bucket_name, object_name):
         try:
             client.download_file(
                 bucket_name,
-                s3_object_name,
-                str(local_file_path),
+                object_name,
+                str(local_path),
             )
             logger.info(
-                f'Downloaded {bucket_name}/{s3_object_name} '
-                f'to {local_file_path}',
+                f'Downloaded {bucket_name}/{object_name} to {local_path}',
             )
             return True
         except client.exceptions.ClientError as e:
             logger.error(f'Failed to download file: {str(e)}')
             return False
     else:
         logger.error('File does not exist in the bucket.')
@@ -329,21 +331,21 @@
     object_name: str,
     overwrite: bool = False,
 ) -> bool:
     """Delete a file from an AWS S3 bucket.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    bucket_name : str
+    bucket_name
         The name of the bucket from which the file will be deleted.
-    object_name : str
+    object_name
         The S3 object name of the file to delete.
-    overwrite : bool, optional
+    overwrite
         If False, the function will not delete the file if it does not exist;
         set to True to ignore non-existence on delete.
 
     Returns
     -------
     bool
         True if the file was deleted successfully, otherwise False.
@@ -368,35 +370,35 @@
     except client.exceptions.ClientError as e:
         logger.error(f'Failed to delete file: {str(e)}')
         return False
 
 
 def copy_file(
     client: boto3.client,
-    source_bucket: str,
-    source_key: str,
-    dest_bucket: str,
-    dest_key: str,
+    source_bucket_name: str,
+    source_object_name: str,
+    destination_bucket_name: str,
+    destination_object_name: str,
     overwrite: bool = False,
 ) -> bool:
     """Copy a file from one aWS S3 bucket to another.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    source_bucket : str
+    source_bucket_name
         The name of the source bucket.
-    source_key : str
+    source_object_name
         The S3 object name of the source file.
-    dest_bucket : str
+    destination_bucket_name
         The name of the destination bucket.
-    dest_key : str
+    destination_object_name
         The S3 object name of the destination file.
-    overwrite : bool, optional
+    overwrite
         If True, overwrite the destination file if it already exists.
 
     Returns
     -------
     bool
         True if the file was copied successfully, otherwise False.
 
@@ -404,60 +406,65 @@
     --------
     >>> client = boto3.client('s3')
     >>> copy_file(
     ...     client,
     ...     'source-bucket',
     ...     'source_file.txt',
     ...     'destination-bucket',
-    ...     'dest_file.txt'
+    ...     'destination_file.txt'
     ... )
     True
     """
-    source_bucket = validate_bucket_name(source_bucket)
-    dest_bucket = validate_bucket_name(dest_bucket)
+    source_bucket_name = validate_bucket_name(source_bucket_name)
+    destination_bucket_name = validate_bucket_name(destination_bucket_name)
 
-    source_key = remove_leading_slash(source_key)
-    dest_key = remove_leading_slash(dest_key)
+    source_object_name = remove_leading_slash(source_object_name)
+    destination_object_name = remove_leading_slash(destination_object_name)
 
-    if not overwrite and file_exists(client, dest_bucket, dest_key):
+    if not overwrite and file_exists(
+        client,
+        destination_bucket_name,
+        destination_object_name,
+    ):
         logger.error(
             'Destination file already exists in the destination bucket.',
         )
         return False
 
-    copy_source = {'Bucket': source_bucket, 'Key': source_key}
+    copy_source = {'Bucket': source_bucket_name, 'Key': source_object_name}
     try:
         client.copy_object(
             CopySource=copy_source,
-            Bucket=dest_bucket,
-            Key=dest_key,
+            Bucket=destination_bucket_name,
+            Key=destination_object_name,
         )
         logger.info(
-            f'Copied {source_bucket}/{source_key} to {dest_bucket}/{dest_key}',
+            f'Copied {source_bucket_name}/{source_object_name} to '
+            f'{destination_bucket_name}/{destination_object_name}',
         )
         return True
     except client.exceptions.ClientError as e:
         logger.error(f'Failed to copy file: {str(e)}')
         return False
 
 
 def create_folder_on_s3(
     client: boto3.client,
     bucket_name: str,
-    folder_name: str,
+    folder_path: str,
 ) -> bool:
     """Create a folder in an AWS S3 bucket if it doesn't already exist.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    bucket_name : str
+    bucket_name
         The name of the bucket where the folder will be created.
-    folder_name : str
+    folder_path
         The name of the folder to create.
 
     Returns
     -------
     bool
         True if the folder was created successfully or
         already exists, otherwise False.
@@ -465,58 +472,58 @@
     Examples
     --------
     >>> client = boto3.client('s3')
     >>> create_folder_on_s3(client, 'mybucket', 'new_folder/')
     True
     """
     bucket_name = validate_bucket_name(bucket_name)
-    folder_name = remove_leading_slash(folder_name)
+    folder_path = remove_leading_slash(folder_path)
 
-    if not folder_name.endswith('/'):
-        folder_name += '/'
+    if not folder_path.endswith('/'):
+        folder_path += '/'
 
     try:
-        client.head_object(Bucket=bucket_name, Key=folder_name)
-        logger.info(f"Folder '{folder_name}' already exists on S3.")
+        client.head_object(Bucket=bucket_name, Key=folder_path)
+        logger.info(f"Folder '{folder_path}' already exists on S3.")
         return True
     except client.exceptions.ClientError as e:
         if e.response['Error']['Code'] == '404':
             # Folder does not exist, create it
             try:
-                client.put_object(Bucket=bucket_name, Key=folder_name)
-                logger.info(f"Created folder '{folder_name}' on S3.")
+                client.put_object(Bucket=bucket_name, Key=folder_path)
+                logger.info(f"Created folder '{folder_path}' on S3.")
                 return True
             except client.exceptions.ClientError as e:
                 logger.error(f'Failed to create folder on S3: {str(e)}')
                 return False
         else:
             logger.error(f'Failed to check folder existence on S3: {str(e)}')
             return False
 
 
 def upload_folder(
     client: boto3.client,
     bucket_name: str,
-    local_folder_path: str,
-    s3_prefix: str = '',
+    local_path: str,
+    prefix: str = '',
     overwrite: bool = False,
 ) -> bool:
     """Upload an entire folder from the local file system to an AWS S3 bucket.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    bucket_name : str
+    bucket_name
         The name of the bucket to which the folder will be uploaded.
-    local_folder_path : str
+    local_path
         The path to the local folder to upload.
-    s3_prefix : str, optional
+    prefix
         The prefix to prepend to each object name when uploading to S3.
-    overwrite : bool, optional
+    overwrite
         If True, overwrite existing files in the bucket.
 
     Returns
     -------
     bool
         True if the folder was uploaded successfully, otherwise False.
 
@@ -529,49 +536,47 @@
     ...     '/path/to/local/folder',
     ...     'folder_prefix',
     ...     True
     ... )
     True
     """
     bucket_name = validate_bucket_name(bucket_name)
-    local_folder_path = Path(local_folder_path)
+    local_path = Path(local_path)
 
     # Check if the local folder exists
-    if not local_folder_path.is_dir():
+    if not local_path.is_dir():
         logger.error('Local folder does not exist.')
         return False
 
-    s3_prefix = remove_leading_slash(s3_prefix)
+    prefix = remove_leading_slash(prefix)
 
     # Ensure the folder exists on S3
-    if not create_folder_on_s3(client, bucket_name, s3_prefix):
+    if not create_folder_on_s3(client, bucket_name, prefix):
         logger.error('Failed to create folder on S3.')
         return False
 
     # Iterate over files in the local folder and its subdirectories
-    for file_path in local_folder_path.rglob('*'):
+    for file_path in local_path.rglob('*'):
         if file_path.is_file():
             # Determine the S3 object key
-            s3_object_key = (
-                s3_prefix + '/' + str(file_path.relative_to(local_folder_path))
-            )
+            object_name = prefix + '/' + str(file_path.relative_to(local_path))
             # Check if the file already exists in the bucket
             if not overwrite and file_exists(
                 client,
                 bucket_name,
-                s3_object_key,
+                object_name,
             ):
                 logger.error(
-                    f"File '{s3_object_key}' already exists in the bucket.",
+                    f"File '{object_name}' already exists in the bucket.",
                 )
                 return False
             # Upload the file to S3
             try:
-                client.upload_file(str(file_path), bucket_name, s3_object_key)
-                logger.info(f"Uploaded '{file_path}' to '{s3_object_key}'.")
+                client.upload_file(str(file_path), bucket_name, object_name)
+                logger.info(f"Uploaded '{file_path}' to '{object_name}'.")
             except FileNotFoundError:
                 logger.error(f"The local file '{file_path}' was not found.")
                 return False
             except client.exceptions.NoCredentialsError:
                 logger.error('Credentials not available.')
                 return False
 
@@ -583,19 +588,19 @@
     bucket_name: str,
     prefix: str = '',
 ) -> List[str]:
     """List files in an AWS S3 bucket that match a specific prefix.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client.
-    bucket_name : str
+    bucket_name
         The name of the bucket.
-    prefix : str, optional
+    prefix
         The prefix to filter files, by default "".
 
     Returns
     -------
     List[str]
         A list of S3 object keys matching the prefix.
 
@@ -619,31 +624,31 @@
         logger.error(f'Failed to list files in bucket: {str(e)}')
         return []
 
 
 def download_folder(
     client: boto3.client,
     bucket_name: str,
-    s3_prefix: str,
+    prefix: str,
     local_path: str,
     overwrite: bool = False,
 ) -> bool:
     """Download a folder from an AWS S3 bucket to a local directory.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    bucket_name : str
+    bucket_name
         The name of the S3 bucket from which to download the folder.
-    s3_prefix : str
+    prefix
         The S3 prefix of the folder to download.
-    local_path : str
+    local_path
         The local directory path where the downloaded folder will be saved.
-    overwrite : bool, optional
+    overwrite
         If True, overwrite existing local files if they exist.
 
     Returns
     -------
     bool
         True if the folder was downloaded successfully, False otherwise.
 
@@ -658,29 +663,29 @@
     ...     overwrite=False
     ... )
     True
     """
     bucket_name = validate_bucket_name(bucket_name)
     local_path = Path(local_path)
 
-    s3_prefix = remove_leading_slash(s3_prefix)
-    if not is_s3_directory(client, bucket_name, s3_prefix):
-        logger.error(f'The provided S3 prefix {s3_prefix} is not a directory.')
+    prefix = remove_leading_slash(prefix)
+    if not is_s3_directory(client, bucket_name, prefix):
+        logger.error(f'The provided S3 prefix {prefix} is not a directory.')
         return False
 
     if not local_path.exists():
         local_path.mkdir(parents=True)
 
     try:
         paginator = client.get_paginator('list_objects_v2')
-        for page in paginator.paginate(Bucket=bucket_name, Prefix=s3_prefix):
+        for page in paginator.paginate(Bucket=bucket_name, Prefix=prefix):
             for obj in page.get('Contents', []):
                 if is_s3_directory(client, bucket_name, obj['Key']):
                     continue
-                target = local_path / Path(obj['Key']).relative_to(s3_prefix)
+                target = local_path / Path(obj['Key']).relative_to(prefix)
                 if not overwrite and target.exists():
                     logger.info(f'Skipping {target} as it already exists.')
                     continue
                 if not target.parent.exists():
                     target.parent.mkdir(parents=True)
                 client.download_file(bucket_name, obj['Key'], str(target))
                 logger.info(f'Downloaded {obj["Key"]} to {target}')
@@ -688,33 +693,33 @@
     except client.exceptions.ClientError as e:
         logger.error(f'Failed to download folder: {str(e)}')
         return False
 
 
 def move_file(
     client: boto3.client,
-    src_bucket: str,
-    src_key: str,
-    dest_bucket: str,
-    dest_key: str,
+    source_bucket_name: str,
+    source_object_name: str,
+    destination_bucket_name: str,
+    destination_object_name: str,
 ) -> bool:
     """Move a file within or between AWS S3 buckets.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    src_bucket : str
+    source_bucket_name
         The name of the source S3 bucket.
-    src_key : str
-        The S3 object key of the source file.
-    dest_bucket : str
+    source_object_name
+        The S3 object name of the source file.
+    destination_bucket_name
         The name of the destination S3 bucket.
-    dest_key : str
-        The S3 object key of the destination file.
+    destination_object_name
+        The S3 object name of the destination file.
 
     Returns
     -------
     bool
         True if the file was moved successfully, False otherwise.
 
     Examples
@@ -725,55 +730,74 @@
     ...     'sourcebucket',
     ...     'source_folder/file.txt',
     ...     'destbucket',
     ...     'dest_folder/file.txt'
     ... )
     True
     """
-    src_bucket = validate_bucket_name(src_bucket)
-    dest_bucket = validate_bucket_name(dest_bucket)
+    source_bucket_name = validate_bucket_name(source_bucket_name)
+    destination_bucket_name = validate_bucket_name(destination_bucket_name)
 
-    src_key = remove_leading_slash(src_key)
-    dest_key = remove_leading_slash(dest_key)
+    source_object_name = remove_leading_slash(source_object_name)
+    destination_object_name = remove_leading_slash(destination_object_name)
 
-    if file_exists(client, src_bucket, src_key):
+    if file_exists(client, source_bucket_name, source_object_name):
         try:
-            copy_source = {'Bucket': src_bucket, 'Key': src_key}
-            client.copy(copy_source, dest_bucket, dest_key)
-            client.delete_object(Bucket=src_bucket, Key=src_key)
+            copy_source = {
+                'Bucket': source_bucket_name,
+                'Key': source_object_name,
+            }
+            client.copy(
+                copy_source,
+                destination_bucket_name,
+                destination_object_name,
+            )
+            client.delete_object(
+                Bucket=source_bucket_name,
+                Key=source_object_name,
+            )
             logger.info(
-                f'Moved {src_bucket}/{src_key} to {dest_bucket}/{dest_key}',
+                f'Moved {source_bucket_name}/{source_object_name} to '
+                f'{destination_bucket_name}/{destination_object_name}',
             )
             return True
         except client.exceptions.ClientError as e:
             logger.error(f'Failed to move file: {str(e)}')
             return False
     else:
         logger.error('Source file does not exist.')
         return False
 
 
 def delete_folder(
-    client: boto3.client, bucket_name: str, folder_path: str,
+    client: boto3.client,
+    bucket_name: str,
+    folder_path: str,
 ) -> bool:
     """Delete a folder in an AWS S3 bucket.
 
     Parameters
     ----------
-    client : boto3.client
+    client
         The boto3 S3 client instance.
-    bucket_name : str
+    bucket_name
         The name of the S3 bucket.
-    folder_path : str
+    folder_path
         The path of the folder to delete.
 
     Returns
     -------
     bool
         True if the folder was deleted successfully, otherwise False.
+
+    Examples
+    --------
+    >>> client = boto3.client('s3')
+    >>> delete_folder(client, 'mybucket', 'path/to/folder/')
+    True
     """
     bucket_name = validate_bucket_name(bucket_name)
     folder_path = remove_leading_slash(folder_path)
 
     if not is_s3_directory(client, bucket_name, folder_path):
         logger.error(f'The provided path {folder_path} is not a directory.')
         return False
```

### Comparing `rdsa_utils-0.2.2/rdsa_utils/cdp/io/input.py` & `rdsa_utils-0.2.3/rdsa_utils/cdp/io/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
        the function will use the current database of the SparkSession.
 
     4. For any other incorrectly formatted names, the function will raise
        a ValueError.
 
     Parameters
     ----------
-    spark : SparkSession
+    spark
         Active SparkSession.
-    long_table_name : str
+    long_table_name
         Full name of the table, which can include the GCP project
         and/or database name.
 
     Returns
     -------
     Tuple[str, str]
         A tuple containing the name of the database and the table name.
```

### Comparing `rdsa_utils-0.2.2/rdsa_utils/cdp/io/output.py` & `rdsa_utils-0.2.3/rdsa_utils/cdp/io/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 """Write outputs on CDP."""
 import logging
+import uuid
 from typing import Union
 
+import boto3
 from pyspark.sql import DataFrame as SparkDF
 from pyspark.sql import SparkSession
 from pyspark.sql import functions as F
 from pyspark.sql.utils import AnalysisException
 
 from rdsa_utils.cdp.helpers.hdfs_utils import delete_path, file_exists, rename
+from rdsa_utils.cdp.helpers.s3_utils import (
+    copy_file,
+    delete_folder,
+    list_files,
+    remove_leading_slash,
+    validate_bucket_name,
+)
 from rdsa_utils.cdp.io.input import load_and_validate_table
 from rdsa_utils.exceptions import (
     ColumnNotInDataframeError,
     DataframeEmptyError,
     TableNotFoundError,
 )
 from rdsa_utils.helpers.pyspark import is_df_empty
@@ -119,15 +128,15 @@
         Active SparkSession.
     df
         The SparkDF to be written to the Hive table.
     table_name
         The name of the Hive table to write to and read from.
     database
         The Hive database name.
-    filter_id : Union[int, str]
+    filter_id
         The identifier to filter on when reading data back from the Hive table.
     filter_col
         The column name to use for filtering data when reading back from
         the Hive table, by default 'run_id'.
     fill_missing_cols
         If True, missing columns in the DataFrame will be filled with nulls
         when writing to the Hive table, by default False.
@@ -304,7 +313,140 @@
         raise IOError(error_msg)
 
     logger.info(f'DataFrame successfully saved to {destination_path}')
 
     # Clean up the temporary directory
     delete_path(temp_path)
     logger.info(f'Temporary directory {temp_path} deleted')
+
+
+def save_csv_to_s3(
+    df: SparkDF,
+    bucket_name: str,
+    file_name: str,
+    file_path: str,
+    s3_client: boto3.client,
+    overwrite: bool = True,
+) -> None:
+    """Save DataFrame as CSV on S3, coalescing to a single partition.
+
+    This function saves a PySpark DataFrame to S3 in CSV format. By
+    coalescing the DataFrame into a single partition before saving, it
+    accomplishes two main objectives:
+
+    1. Single Part File: The output is a single CSV file rather than
+       multiple part files. This method reduces complexity and
+       cuts through the clutter of multi-part files, offering users
+       and systems a more cohesive and hassle-free experience.
+
+    2. Preserving Row Order: Coalescing into a single partition maintains
+       the order of rows as they appear in the DataFrame. This is essential
+       when the row order matters for subsequent processing or analysis.
+       It's important to note, however, that coalescing can have performance
+       implications for very large DataFrames by concentrating
+       all data processing on a single node.
+
+    Parameters
+    ----------
+    df
+        PySpark DataFrame to be saved.
+    bucket_name
+        The name of the S3 bucket where the CSV file should be saved.
+    file_name
+        Name of the CSV file. Must include the ".csv" extension.
+    file_path
+        S3 path where the CSV file should be saved.
+    s3_client
+        The boto3 S3 client instance.
+    overwrite
+        If True, overwrite any existing file with the same name. If False
+        and the file exists, the function will raise an error.
+
+    Raises
+    ------
+    ValueError
+        If the file_name does not end with ".csv".
+    IOError
+        If overwrite is False and the target file already exists.
+
+    Examples
+    --------
+    Saving to an S3 bucket:
+
+    ```python
+    # Assume `df` is a pre-defined PySpark DataFrame
+    file_name = "data_output.csv"
+    file_path = "data_folder/"
+    s3_client = boto3.client('s3')
+    save_csv_to_s3(
+        df,
+        'my-bucket',
+        file_name,
+        file_path,
+        s3_client,
+        overwrite=True
+    )
+    ```
+    """
+    bucket_name = validate_bucket_name(bucket_name)
+    file_path = remove_leading_slash(file_path)
+
+    if not file_name.endswith('.csv'):
+        error_msg = "The file_name must end with '.csv' extension."
+        raise ValueError(error_msg)
+
+    destination_path = f"{file_path.rstrip('/')}/{file_name}"
+
+    if not overwrite and file_exists(s3_client, bucket_name, destination_path):
+        error_msg = (
+            f"File '{destination_path}' already exists "
+            "and overwrite is set to False."
+        )
+        raise IOError(error_msg)
+
+    logger.info(
+        f'Saving DataFrame to {file_name} in S3 at s3://{bucket_name}/{file_path}',
+    )
+
+    # Coalesce the DataFrame to a single partition
+    df = df.coalesce(1)
+
+    # Temporary S3 path for saving the single part file
+    temp_path = f"{file_path.rstrip('/')}/temp_{uuid.uuid4().hex}_{file_name}"
+
+    # Save the DataFrame to S3 in CSV format in a temporary directory
+    df.write.csv(
+        f's3a://{bucket_name}/{temp_path}',
+        header=True,
+        mode='overwrite',
+    )
+
+    # Identify the part file using the list_files helper function
+    part_file_prefix = f'{temp_path}/part-00000'
+    part_files = list_files(s3_client, bucket_name, part_file_prefix)
+    if not part_files:
+        error_msg = 'No part files found in the temporary directory.'
+        raise IOError(error_msg)
+
+    # Get the first part file from the list
+    # Since the DataFrame is coalesced to a single partition, there should
+    # only be one part file
+    part_file_key = part_files[0]
+
+    # Rename the part file to the final file name
+    if not copy_file(
+        s3_client,
+        bucket_name,
+        part_file_key,
+        bucket_name,
+        destination_path,
+        overwrite,
+    ):
+        error_msg = f"Failed to rename the part file to '{destination_path}'"
+        raise IOError(error_msg)
+
+    logger.info(
+        f'DataFrame successfully saved to s3://{bucket_name}/{destination_path}',
+    )
+
+    # Clean up the temporary directory
+    delete_folder(s3_client, bucket_name, temp_path)
```

### Comparing `rdsa_utils-0.2.2/rdsa_utils/cdp/io/pipeline_runlog.py` & `rdsa_utils-0.2.3/rdsa_utils/cdp/io/pipeline_runlog.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/exceptions.py` & `rdsa_utils-0.2.3/rdsa_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/gcp/helpers/gcp_utils.py` & `rdsa_utils-0.2.3/rdsa_utils/gcp/helpers/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/gcp/io/inputs.py` & `rdsa_utils-0.2.3/rdsa_utils/gcp/io/inputs.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/gcp/io/outputs.py` & `rdsa_utils-0.2.3/rdsa_utils/gcp/io/outputs.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/helpers/pyspark.py` & `rdsa_utils-0.2.3/rdsa_utils/helpers/pyspark.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/helpers/python.py` & `rdsa_utils-0.2.3/rdsa_utils/helpers/python.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/io/config.py` & `rdsa_utils-0.2.3/rdsa_utils/io/config.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/io/input.py` & `rdsa_utils-0.2.3/rdsa_utils/io/input.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/logging.py` & `rdsa_utils-0.2.3/rdsa_utils/logging.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/methods/averaging_methods.py` & `rdsa_utils-0.2.3/rdsa_utils/methods/averaging_methods.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/test_utils.py` & `rdsa_utils-0.2.3/rdsa_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/typing.py` & `rdsa_utils-0.2.3/rdsa_utils/typing.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils/validation.py` & `rdsa_utils-0.2.3/rdsa_utils/validation.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils.egg-info/PKG-INFO` & `rdsa_utils-0.2.3/rdsa_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdsa-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 Home-page: https://github.com/ONSdigital/rdsa-utils
 Author: Reproducible Data Science & Analysis, ONS
 Author-email: Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rdsa_utils-0.2.2/rdsa_utils.egg-info/SOURCES.txt` & `rdsa_utils-0.2.3/rdsa_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/rdsa_utils.egg-info/requires.txt` & `rdsa_utils-0.2.3/rdsa_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/setup.cfg` & `rdsa_utils-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/tests/test_logging.py` & `rdsa_utils-0.2.3/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.2.2/tests/test_validation.py` & `rdsa_utils-0.2.3/tests/test_validation.py`

 * *Files identical despite different names*


# Comparing `tmp/strangeworks_braket-1.0.8.tar.gz` & `tmp/strangeworks_braket-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_braket-1.0.8.tar", max compression
+gzip compressed data, was "strangeworks_braket-1.0.9.tar", max compression
```

## Comparing `strangeworks_braket-1.0.8.tar` & `strangeworks_braket-1.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      457 2024-01-02 19:08:27.316221 strangeworks_braket-1.0.8/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2024-01-02 19:08:27.316221 strangeworks_braket-1.0.8/LICENSE
--rw-r--r--   0        0        0     1374 2024-01-02 19:08:43.681128 strangeworks_braket-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      286 2024-01-02 19:08:27.316221 strangeworks_braket-1.0.8/strangeworks_braket/__init__.py
--rw-r--r--   0        0        0     7283 2024-01-02 19:08:27.316221 strangeworks_braket-1.0.8/strangeworks_braket/device.py
--rw-r--r--   0        0        0     8503 2024-01-02 19:08:27.316221 strangeworks_braket-1.0.8/strangeworks_braket/job.py
--rw-r--r--   0        0        0    10554 2024-01-02 19:08:27.316221 strangeworks_braket-1.0.8/strangeworks_braket/task.py
--rw-r--r--   0        0        0     1988 2024-01-02 19:08:27.316221 strangeworks_braket-1.0.8/strangeworks_braket/utils/ahs_utils.py
--rw-r--r--   0        0        0      691 2024-01-02 19:08:27.320221 strangeworks_braket-1.0.8/strangeworks_braket/utils/serializer.py
--rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      457 2024-02-16 21:41:40.594308 strangeworks_braket-1.0.9/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2024-02-16 21:41:40.594308 strangeworks_braket-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1372 2024-02-16 21:41:54.698390 strangeworks_braket-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      286 2024-02-16 21:41:40.598308 strangeworks_braket-1.0.9/strangeworks_braket/__init__.py
+-rw-r--r--   0        0        0     7283 2024-02-16 21:41:40.598308 strangeworks_braket-1.0.9/strangeworks_braket/device.py
+-rw-r--r--   0        0        0     8503 2024-02-16 21:41:40.598308 strangeworks_braket-1.0.9/strangeworks_braket/job.py
+-rw-r--r--   0        0        0    10554 2024-02-16 21:41:40.598308 strangeworks_braket-1.0.9/strangeworks_braket/task.py
+-rw-r--r--   0        0        0     1988 2024-02-16 21:41:40.598308 strangeworks_braket-1.0.9/strangeworks_braket/utils/ahs_utils.py
+-rw-r--r--   0        0        0      691 2024-02-16 21:41:40.598308 strangeworks_braket-1.0.9/strangeworks_braket/utils/serializer.py
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.9/PKG-INFO
```

### Comparing `strangeworks_braket-1.0.8/LICENSE` & `strangeworks_braket-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.8/pyproject.toml` & `strangeworks_braket-1.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "strangeworks-braket"
-version = "1.0.8"
+version = "1.0.9"
 description = "Strangeworks Braket SDK extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks_braket"},
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11.4"
+python = ">=3.10,<4.0"
 amazon-braket-sdk = "1.42.1"
 strangeworks-core = "0.2.3"
 python-jose = "3.3.0"
 strangeworks = "0.4.4"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `strangeworks_braket-1.0.8/strangeworks_braket/device.py` & `strangeworks_braket-1.0.9/strangeworks_braket/device.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.8/strangeworks_braket/job.py` & `strangeworks_braket-1.0.9/strangeworks_braket/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.8/strangeworks_braket/task.py` & `strangeworks_braket-1.0.9/strangeworks_braket/task.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.8/strangeworks_braket/utils/ahs_utils.py` & `strangeworks_braket-1.0.9/strangeworks_braket/utils/ahs_utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.8/strangeworks_braket/utils/serializer.py` & `strangeworks_braket-1.0.9/strangeworks_braket/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.8/PKG-INFO` & `strangeworks_braket-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: strangeworks-braket
-Version: 1.0.8
+Version: 1.0.9
 Summary: Strangeworks Braket SDK extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
-Requires-Python: >=3.9,<3.11.4
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: amazon-braket-sdk (==1.42.1)
 Requires-Dist: python-jose (==3.3.0)
 Requires-Dist: strangeworks (==0.4.4)
 Requires-Dist: strangeworks-core (==0.2.3)
 Description-Content-Type: text/markdown
 
 | ⚠️ | This SDK is currently in pre-release alpha state and subject to change. To get
```


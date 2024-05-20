# Comparing `tmp/wizata_dsapi-1.0.3.tar.gz` & `tmp/wizata_dsapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata_dsapi-1.0.3.tar", last modified: Mon May 20 09:11:52 2024, max compression
+gzip compressed data, was "wizata_dsapi-1.0.4.tar", last modified: Mon May 20 09:14:07 2024, max compression
```

## Comparing `wizata_dsapi-1.0.3.tar` & `wizata_dsapi-1.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:11:52.924774 wizata_dsapi-1.0.3/
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.3/LICENSE.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1252 2024-05-20 09:11:52.924595 wizata_dsapi-1.0.3/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.3/README.rst
--rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-05-20 09:11:52.924818 wizata_dsapi-1.0.3/setup.cfg
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1417 2024-05-20 09:08:09.000000 wizata_dsapi-1.0.3/setup.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:11:52.923554 wizata_dsapi-1.0.3/wizata_dsapi/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1557 2024-05-16 13:17:14.000000 wizata_dsapi-1.0.3/wizata_dsapi/__init__.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3875 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/api_config.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1172 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/api_dto.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     9270 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/api_interface.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4151 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/business_label.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10084 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/context.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     8472 2024-05-16 13:17:14.000000 wizata_dsapi-1.0.3/wizata_dsapi/dataframe_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10822 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/datapoint.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2089 2024-03-06 07:51:32.000000 wizata_dsapi-1.0.3/wizata_dsapi/ds_dataframe.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.3/wizata_dsapi/dsapi_json_encoder.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12777 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/execution.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4355 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/experiment.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      807 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/ilogger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    14587 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/mlmodel.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1551 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/model_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1150 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/paged_query_result.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    28788 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/pipeline.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2355 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/plot.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    19308 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12710 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/script.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     7625 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/solution_component.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12451 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/template.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4769 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/trigger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     6291 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/twin.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12865 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/twinregistration.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-05-20 09:08:09.000000 wizata_dsapi-1.0.3/wizata_dsapi/version.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      942 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/wizard_function.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3762 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/wizard_request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    68678 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.3/wizata_dsapi/wizata_dsapi_client.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1535 2024-03-20 11:49:55.000000 wizata_dsapi-1.0.3/wizata_dsapi/words.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:11:52.924267 wizata_dsapi-1.0.3/wizata_dsapi.egg-info/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1252 2024-05-20 09:11:52.000000 wizata_dsapi-1.0.3/wizata_dsapi.egg-info/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1037 2024-05-20 09:11:52.000000 wizata_dsapi-1.0.3/wizata_dsapi.egg-info/SOURCES.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-05-20 09:11:52.000000 wizata_dsapi-1.0.3/wizata_dsapi.egg-info/dependency_links.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      569 2024-05-20 09:11:52.000000 wizata_dsapi-1.0.3/wizata_dsapi.egg-info/requires.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-05-20 09:11:52.000000 wizata_dsapi-1.0.3/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:14:07.409813 wizata_dsapi-1.0.4/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.4/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1252 2024-05-20 09:14:07.409625 wizata_dsapi-1.0.4/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.4/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-05-20 09:14:07.409859 wizata_dsapi-1.0.4/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1417 2024-05-20 09:13:35.000000 wizata_dsapi-1.0.4/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:14:07.408425 wizata_dsapi-1.0.4/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1557 2024-05-16 13:17:14.000000 wizata_dsapi-1.0.4/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3875 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/api_config.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1172 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     9270 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/api_interface.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4151 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/business_label.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10084 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8472 2024-05-16 13:17:14.000000 wizata_dsapi-1.0.4/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10822 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2089 2024-03-06 07:51:32.000000 wizata_dsapi-1.0.4/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.4/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12777 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4355 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      807 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/ilogger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    14587 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1551 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1150 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/paged_query_result.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    28788 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2355 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19308 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12710 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7625 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/solution_component.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12451 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4769 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/trigger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     6291 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12865 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-05-20 09:14:06.000000 wizata_dsapi-1.0.4/wizata_dsapi/version.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      942 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3762 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/wizard_request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    68678 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.4/wizata_dsapi/wizata_dsapi_client.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1535 2024-03-20 11:49:55.000000 wizata_dsapi-1.0.4/wizata_dsapi/words.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:14:07.409261 wizata_dsapi-1.0.4/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1252 2024-05-20 09:14:07.000000 wizata_dsapi-1.0.4/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1037 2024-05-20 09:14:07.000000 wizata_dsapi-1.0.4/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-05-20 09:14:07.000000 wizata_dsapi-1.0.4/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      569 2024-05-20 09:14:07.000000 wizata_dsapi-1.0.4/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-05-20 09:14:07.000000 wizata_dsapi-1.0.4/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata_dsapi-1.0.3/LICENSE.txt` & `wizata_dsapi-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/PKG-INFO` & `wizata_dsapi-1.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: wizata-dsapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: Wizata Data Science Toolkit
 Author: Wizata S.A.
 Author-email: info@wizata.com
 License-File: LICENSE.txt
 Requires-Dist: dill>=0.3.8
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: matplotlib>=3.9.0
-Requires-Dist: protobuf>=5.26.1
+Requires-Dist: protobuf>=3.20.3
 Requires-Dist: tensorflow==2.16.1; sys_platform != "darwin" or platform_machine != "arm64"
 Requires-Dist: tensorflow-macos==2.16.1; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: keras==3.3.3; sys_platform != "darwin" or platform_machine != "arm64"
 Requires-Dist: keras==3.3.3; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: tensorflow_probability>=0.24.0
 Requires-Dist: scikit-learn>=1.4.2
 Requires-Dist: scipy>=1.13.0
```

### Comparing `wizata_dsapi-1.0.3/setup.py` & `wizata_dsapi-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill>=0.3.8',
         'pandas>=2.2.2',
         'numpy>=1.26.4',
         'matplotlib>=3.9.0',
-        'protobuf>=5.26.1',
+        'protobuf>=3.20.3',
         "tensorflow==2.16.1; sys_platform != 'darwin' or platform_machine != 'arm64'",
         "tensorflow-macos==2.16.1; sys_platform == 'darwin' and platform_machine == 'arm64'",
         "keras==3.3.3; sys_platform != 'darwin' or platform_machine != 'arm64'",
         "keras==3.3.3; sys_platform == 'darwin' and platform_machine == 'arm64'",
         'tensorflow_probability>=0.24.0',
         'scikit-learn>=1.4.2',
         'scipy>=1.13.0',
```

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/__init__.py` & `wizata_dsapi-1.0.4/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/api_config.py` & `wizata_dsapi-1.0.4/wizata_dsapi/api_config.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/api_dto.py` & `wizata_dsapi-1.0.4/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/api_interface.py` & `wizata_dsapi-1.0.4/wizata_dsapi/api_interface.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/business_label.py` & `wizata_dsapi-1.0.4/wizata_dsapi/business_label.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/context.py` & `wizata_dsapi-1.0.4/wizata_dsapi/context.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/dataframe_toolkit.py` & `wizata_dsapi-1.0.4/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/datapoint.py` & `wizata_dsapi-1.0.4/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/ds_dataframe.py` & `wizata_dsapi-1.0.4/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/dsapi_json_encoder.py` & `wizata_dsapi-1.0.4/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/execution.py` & `wizata_dsapi-1.0.4/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/experiment.py` & `wizata_dsapi-1.0.4/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/ilogger.py` & `wizata_dsapi-1.0.4/wizata_dsapi/ilogger.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/mlmodel.py` & `wizata_dsapi-1.0.4/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/model_toolkit.py` & `wizata_dsapi-1.0.4/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/paged_query_result.py` & `wizata_dsapi-1.0.4/wizata_dsapi/paged_query_result.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/pipeline.py` & `wizata_dsapi-1.0.4/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/plot.py` & `wizata_dsapi-1.0.4/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/request.py` & `wizata_dsapi-1.0.4/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/script.py` & `wizata_dsapi-1.0.4/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/solution_component.py` & `wizata_dsapi-1.0.4/wizata_dsapi/solution_component.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/template.py` & `wizata_dsapi-1.0.4/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/trigger.py` & `wizata_dsapi-1.0.4/wizata_dsapi/trigger.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/twin.py` & `wizata_dsapi-1.0.4/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/twinregistration.py` & `wizata_dsapi-1.0.4/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/wizard_function.py` & `wizata_dsapi-1.0.4/wizata_dsapi/wizard_function.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/wizard_request.py` & `wizata_dsapi-1.0.4/wizata_dsapi/wizard_request.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/wizata_dsapi_client.py` & `wizata_dsapi-1.0.4/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi/words.py` & `wizata_dsapi-1.0.4/wizata_dsapi/words.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi.egg-info/PKG-INFO` & `wizata_dsapi-1.0.4/wizata_dsapi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: wizata-dsapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: Wizata Data Science Toolkit
 Author: Wizata S.A.
 Author-email: info@wizata.com
 License-File: LICENSE.txt
 Requires-Dist: dill>=0.3.8
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: matplotlib>=3.9.0
-Requires-Dist: protobuf>=5.26.1
+Requires-Dist: protobuf>=3.20.3
 Requires-Dist: tensorflow==2.16.1; sys_platform != "darwin" or platform_machine != "arm64"
 Requires-Dist: tensorflow-macos==2.16.1; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: keras==3.3.3; sys_platform != "darwin" or platform_machine != "arm64"
 Requires-Dist: keras==3.3.3; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: tensorflow_probability>=0.24.0
 Requires-Dist: scikit-learn>=1.4.2
 Requires-Dist: scipy>=1.13.0
```

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi.egg-info/SOURCES.txt` & `wizata_dsapi-1.0.4/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.3/wizata_dsapi.egg-info/requires.txt` & `wizata_dsapi-1.0.4/wizata_dsapi.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 dill>=0.3.8
 pandas>=2.2.2
 numpy>=1.26.4
 matplotlib>=3.9.0
-protobuf>=5.26.1
+protobuf>=3.20.3
 tensorflow_probability>=0.24.0
 scikit-learn>=1.4.2
 scipy>=1.13.0
 plotly>=5.22.0
 adtk>=0.6.2
 xgboost>=2.0.3
 joblib>=1.4.2
```


# Comparing `tmp/WrenchCL-2.1.5.tar.gz` & `tmp/WrenchCL-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrenchCL-2.1.5.tar", last modified: Mon May 20 15:34:51 2024, max compression
+gzip compressed data, was "WrenchCL-2.1.6.tar", last modified: Mon May 20 15:54:52 2024, max compression
```

## Comparing `WrenchCL-2.1.5.tar` & `WrenchCL-2.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.118313 WrenchCL-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-05-20 15:34:51.118313 WrenchCL-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22844 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.110313 WrenchCL-2.1.5/WrenchCL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.114313 WrenchCL-2.1.5/WrenchCL/Connect/
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Connect/AwsClientHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Connect/RdsServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Connect/S3ServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.114313 WrenchCL-2.1.5/WrenchCL/DataFlow/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/DataFlow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/DataFlow/build_return_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/DataFlow/handle_lambda_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/DataFlow/trigger_dataflow_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.114313 WrenchCL-2.1.5/WrenchCL/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Decorators/Retryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Decorators/SingletonClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Decorators/TimedMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.114313 WrenchCL-2.1.5/WrenchCL/Models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.114313 WrenchCL-2.1.5/WrenchCL/Models/OpenAI/
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Models/OpenAI/OpenAIFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    16033 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Models/OpenAI/OpenAIGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Models/OpenAI/_ConversationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Models/OpenAI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.118313 WrenchCL-2.1.5/WrenchCL/Tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/Coalesce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/DictValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/FetchMetaData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/FileTyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/Image2B64.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/JsonSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/MaybeMonad.py
--rw-r--r--   0 runner    (1001) docker     (127)    31356 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/WrenchLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/Tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.118313 WrenchCL-2.1.5/WrenchCL/_Internal/
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/_Internal/_ConfigurationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/_Internal/_SshTunnelManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/_Internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 15:34:28.000000 WrenchCL-2.1.5/WrenchCL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:34:51.114313 WrenchCL-2.1.5/WrenchCL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-05-20 15:34:51.000000 WrenchCL-2.1.5/WrenchCL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-20 15:34:51.000000 WrenchCL-2.1.5/WrenchCL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:34:51.000000 WrenchCL-2.1.5/WrenchCL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 15:34:51.000000 WrenchCL-2.1.5/WrenchCL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 15:34:51.000000 WrenchCL-2.1.5/WrenchCL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:34:51.118313 WrenchCL-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-20 15:34:49.000000 WrenchCL-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.158797 WrenchCL-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-05-20 15:54:52.154797 WrenchCL-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22844 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.150797 WrenchCL-2.1.6/WrenchCL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.150797 WrenchCL-2.1.6/WrenchCL/Connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Connect/AwsClientHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Connect/RdsServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Connect/S3ServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.154797 WrenchCL-2.1.6/WrenchCL/DataFlow/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/DataFlow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/DataFlow/build_return_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/DataFlow/handle_lambda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/DataFlow/trigger_dataflow_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.154797 WrenchCL-2.1.6/WrenchCL/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Decorators/Retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Decorators/SingletonClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Decorators/TimedMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.154797 WrenchCL-2.1.6/WrenchCL/Models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.154797 WrenchCL-2.1.6/WrenchCL/Models/OpenAI/
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Models/OpenAI/OpenAIFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16033 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Models/OpenAI/OpenAIGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Models/OpenAI/_ConversationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Models/OpenAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.154797 WrenchCL-2.1.6/WrenchCL/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/Coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/DictValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/FetchMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/FileTyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/Image2B64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/JsonSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/MaybeMonad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31356 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/WrenchLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/Tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.154797 WrenchCL-2.1.6/WrenchCL/_Internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/_Internal/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/_Internal/_SshTunnelManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/_Internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 15:54:30.000000 WrenchCL-2.1.6/WrenchCL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:54:52.150797 WrenchCL-2.1.6/WrenchCL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-05-20 15:54:52.000000 WrenchCL-2.1.6/WrenchCL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-20 15:54:52.000000 WrenchCL-2.1.6/WrenchCL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:54:52.000000 WrenchCL-2.1.6/WrenchCL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 15:54:52.000000 WrenchCL-2.1.6/WrenchCL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 15:54:52.000000 WrenchCL-2.1.6/WrenchCL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:54:52.158797 WrenchCL-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-20 15:54:50.000000 WrenchCL-2.1.6/setup.py
```

### Comparing `WrenchCL-2.1.5/LICENSE` & `WrenchCL-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/PKG-INFO` & `WrenchCL-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.1.5
+Version: 2.1.6
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.5 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.6 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
```

### Comparing `WrenchCL-2.1.5/README.md` & `WrenchCL-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Connect/AwsClientHub.py` & `WrenchCL-2.1.6/WrenchCL/Connect/AwsClientHub.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Connect/RdsServiceGateway.py` & `WrenchCL-2.1.6/WrenchCL/Connect/RdsServiceGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Connect/S3ServiceGateway.py` & `WrenchCL-2.1.6/WrenchCL/Connect/S3ServiceGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/DataFlow/build_return_json.py` & `WrenchCL-2.1.6/WrenchCL/DataFlow/build_return_json.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/DataFlow/handle_lambda_response.py` & `WrenchCL-2.1.6/WrenchCL/DataFlow/handle_lambda_response.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/DataFlow/trigger_dataflow_metrics.py` & `WrenchCL-2.1.6/WrenchCL/DataFlow/trigger_dataflow_metrics.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Decorators/Retryable.py` & `WrenchCL-2.1.6/WrenchCL/Decorators/Retryable.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Decorators/SingletonClass.py` & `WrenchCL-2.1.6/WrenchCL/Decorators/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Decorators/TimedMethod.py` & `WrenchCL-2.1.6/WrenchCL/Decorators/TimedMethod.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Models/OpenAI/OpenAIFactory.py` & `WrenchCL-2.1.6/WrenchCL/Models/OpenAI/OpenAIFactory.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Models/OpenAI/OpenAIGateway.py` & `WrenchCL-2.1.6/WrenchCL/Models/OpenAI/OpenAIGateway.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Models/OpenAI/_ConversationManager.py` & `WrenchCL-2.1.6/WrenchCL/Models/OpenAI/_ConversationManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Models/OpenAI/__init__.py` & `WrenchCL-2.1.6/WrenchCL/Models/OpenAI/__init__.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Tools/Coalesce.py` & `WrenchCL-2.1.6/WrenchCL/Tools/Coalesce.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Tools/DictValidator.py` & `WrenchCL-2.1.6/WrenchCL/Tools/DictValidator.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Tools/FetchMetaData.py` & `WrenchCL-2.1.6/WrenchCL/Tools/FetchMetaData.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Tools/FileTyper.py` & `WrenchCL-2.1.6/WrenchCL/Tools/FileTyper.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Tools/Image2B64.py` & `WrenchCL-2.1.6/WrenchCL/Tools/Image2B64.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Tools/JsonSerializer.py` & `WrenchCL-2.1.6/WrenchCL/Tools/JsonSerializer.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Tools/MaybeMonad.py` & `WrenchCL-2.1.6/WrenchCL/Tools/MaybeMonad.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/Tools/WrenchLogger.py` & `WrenchCL-2.1.6/WrenchCL/Tools/WrenchLogger.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL/_Internal/_ConfigurationManager.py` & `WrenchCL-2.1.6/WrenchCL/_Internal/_ConfigurationManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         self.openai_api_key = kwargs.get('OPENAI_API_KEY', self.openai_api_key)
         self.ssh_server = kwargs.get('SSH_SERVER', self.ssh_server)
         self.ssh_port = int(kwargs.get('SSH_PORT', self.ssh_port or 0))
         self.ssh_user = kwargs.get('SSH_USER', self.ssh_user)
         self.ssh_password = kwargs.get('SSH_PASSWORD', self.ssh_password)
         self.pem_path = kwargs.get('PEM_PATH', self.pem_path)
         self.db_batch_size = int(kwargs.get('DB_BATCH_OVERRIDE', self.db_batch_size or 10000))
+        logger.error(str(kwargs.get('AWS_DEPLOYMENT', self.aws_deployment)).lower())
         self.aws_deployment = str(kwargs.get('AWS_DEPLOYMENT', self.aws_deployment)).lower() == 'true'
 
     def _init_from_env(self):
         """
         Initializes configuration values from environment variables.
         """
         self.aws_profile = os.getenv('AWS_PROFILE', self.aws_profile)
@@ -159,8 +160,8 @@
         self.openai_api_key = os.getenv('OPENAI_API_KEY', self.openai_api_key)
         self.ssh_server = os.getenv('SSH_SERVER', self.ssh_server)
         self.ssh_port = int(os.getenv('SSH_PORT', self.ssh_port or 0))
         self.ssh_user = os.getenv('SSH_USER', self.ssh_user)
         self.ssh_password = os.getenv('SSH_PASSWORD', self.ssh_password)
         self.pem_path = os.getenv('PEM_PATH', self.pem_path)
         self.db_batch_size = int(os.getenv('DB_BATCH_OVERRIDE', self.db_batch_size or 10000))
-        self.aws_deployment = str(os.getenv('DB_BATCH_OVERRIDE', None)).lower() == 'true'
+        self.aws_deployment = str(os.getenv('AWS_DEPLOYMENT', None)).lower() == 'true'
```

### Comparing `WrenchCL-2.1.5/WrenchCL/_Internal/_SshTunnelManager.py` & `WrenchCL-2.1.6/WrenchCL/_Internal/_SshTunnelManager.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/WrenchCL.egg-info/PKG-INFO` & `WrenchCL-2.1.6/WrenchCL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.1.5
+Version: 2.1.6
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.5 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.6 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
```

### Comparing `WrenchCL-2.1.5/WrenchCL.egg-info/SOURCES.txt` & `WrenchCL-2.1.6/WrenchCL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.1.5/setup.py` & `WrenchCL-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,14 @@
         if os.path.exists(requires_path):
             with open(requires_path, "r", encoding="utf-8") as f:
                 required = f.read().splitlines()
 
 # Define the optional dependencies
 extras = {'libmagic': ['python-magic-bin~=0.4.14']}
 
-setup(name='WrenchCL', version='v2.1.5',
+setup(name='WrenchCL', version='v2.1.6',
       description='WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.',
       long_description=long_description, long_description_content_type="text/markdown",
       url='https://github.com/WrenchAI/WrenchCL', packages=find_packages(), install_requires=required,
       extras_require=extras, python_requires='>=3.11',
       classifiers=['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License',
                    'Operating System :: OS Independent', ], )
```


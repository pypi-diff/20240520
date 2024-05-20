# Comparing `tmp/cogflow-1.9.8.tar.gz` & `tmp/cogflow-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.9.8.tar", last modified: Tue May  7 07:24:58 2024, max compression
+gzip compressed data, was "cogflow-1.9.9.tar", last modified: Thu May 16 13:21:55 2024, max compression
```

## Comparing `cogflow-1.9.8.tar` & `cogflow-1.9.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 07:24:57.966848 cogflow-1.9.8/
--rw-rw-rw-   0        0        0     3230 2024-05-07 07:24:57.934664 cogflow-1.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 07:24:57.715655 cogflow-1.9.8/cogflow/
--rw-rw-rw-   0        0        0     5551 2024-05-06 13:50:23.000000 cogflow-1.9.8/cogflow/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.8/cogflow/cogflow_config.ini
--rw-rw-rw-   0        0        0     6159 2024-05-03 11:09:50.000000 cogflow-1.9.8/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.8/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    15647 2024-05-06 12:36:42.000000 cogflow-1.9.8/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0     3116 2024-05-03 11:02:35.000000 cogflow-1.9.8/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.8/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.8/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.8/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:24:57.794737 cogflow-1.9.8/cogflow.egg-info/
--rw-rw-rw-   0        0        0     3230 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 07:24:57.966848 cogflow-1.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1940 2024-05-07 07:24:47.000000 cogflow-1.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:24:57.925433 cogflow-1.9.8/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.8/tests/__init__.py
--rw-rw-rw-   0        0        0    11566 2024-05-03 11:09:50.000000 cogflow-1.9.8/tests/test_dataset_plugin.py
--rw-rw-rw-   0        0        0     6614 2024-05-03 11:09:50.000000 cogflow-1.9.8/tests/test_kubeflowplugin.py
--rw-rw-rw-   0        0        0    18889 2024-05-06 13:32:38.000000 cogflow-1.9.8/tests/test_mlflowplugin.py
--rw-rw-rw-   0        0        0     4363 2024-05-03 11:09:50.000000 cogflow-1.9.8/tests/test_plugin_manager.py
+drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-05-16 13:21:55.690938 cogflow-1.9.9/
+-rw-r--r--   0 bola      (1000) bola      (1000)     3075 2024-05-16 13:21:55.690938 cogflow-1.9.9/PKG-INFO
+-rw-rw-r--   0 bola      (1000) bola      (1000)     2282 2024-05-16 12:11:27.000000 cogflow-1.9.9/README.md
+drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-05-16 13:21:55.690938 cogflow-1.9.9/cogflow/
+-rw-rw-r--   0 bola      (1000) bola      (1000)     5398 2024-05-16 12:11:27.000000 cogflow-1.9.9/cogflow/__init__.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)      119 2024-05-16 12:11:27.000000 cogflow-1.9.9/cogflow/cogflow_config.ini
+-rw-rw-r--   0 bola      (1000) bola      (1000)     6010 2024-05-16 12:11:27.000000 cogflow-1.9.9/cogflow/dataset_plugin.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)    10114 2024-05-16 13:14:59.000000 cogflow-1.9.9/cogflow/kubeflowplugin.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)    15179 2024-05-16 12:11:27.000000 cogflow-1.9.9/cogflow/mlflowplugin.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)     3050 2024-05-16 12:11:27.000000 cogflow-1.9.9/cogflow/plugin_config.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)      602 2024-05-16 12:11:27.000000 cogflow-1.9.9/cogflow/plugin_status.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)      165 2024-05-16 12:11:27.000000 cogflow-1.9.9/cogflow/pluginerrors.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)     9412 2024-05-16 12:11:27.000000 cogflow-1.9.9/cogflow/pluginmanager.py
+drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-05-16 13:21:55.690938 cogflow-1.9.9/cogflow.egg-info/
+-rw-r--r--   0 bola      (1000) bola      (1000)     3075 2024-05-16 13:21:55.000000 cogflow-1.9.9/cogflow.egg-info/PKG-INFO
+-rw-rw-r--   0 bola      (1000) bola      (1000)      526 2024-05-16 13:21:55.000000 cogflow-1.9.9/cogflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 bola      (1000) bola      (1000)        1 2024-05-16 13:21:55.000000 cogflow-1.9.9/cogflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 bola      (1000) bola      (1000)      214 2024-05-16 13:21:55.000000 cogflow-1.9.9/cogflow.egg-info/requires.txt
+-rw-rw-r--   0 bola      (1000) bola      (1000)       14 2024-05-16 13:21:55.000000 cogflow-1.9.9/cogflow.egg-info/top_level.txt
+-rw-rw-r--   0 bola      (1000) bola      (1000)       38 2024-05-16 13:21:55.690938 cogflow-1.9.9/setup.cfg
+-rw-rw-r--   0 bola      (1000) bola      (1000)     1879 2024-05-16 13:16:13.000000 cogflow-1.9.9/setup.py
+drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-05-16 13:21:55.690938 cogflow-1.9.9/tests/
+-rw-rw-r--   0 bola      (1000) bola      (1000)        0 2024-05-16 12:11:27.000000 cogflow-1.9.9/tests/__init__.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)    11267 2024-05-16 12:11:27.000000 cogflow-1.9.9/tests/test_dataset_plugin.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)     6452 2024-05-16 12:11:27.000000 cogflow-1.9.9/tests/test_kubeflowplugin.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)    18401 2024-05-16 12:11:27.000000 cogflow-1.9.9/tests/test_mlflowplugin.py
+-rw-rw-r--   0 bola      (1000) bola      (1000)     4259 2024-05-16 12:11:27.000000 cogflow-1.9.9/tests/test_plugin_manager.py
```

### Comparing `cogflow-1.9.8/README.md` & `cogflow-1.9.9/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-
-# CogFlow
-
-CogFlow is a versatile framework designed to manage multiple plugins for cognitive and machine learning tasks. It includes several plugins such as `MlflowPlugin`, `KubeflowPlugin`, and `DatasetPlugin`, which can be activated as needed to extend the capabilities of the framework.
-
-## Getting Started
-
-To begin, import cogflow from the CogFlow module:
-
-```python
-import cogflow
-
-```
-
-### Explore the Capabilities of `cogflow`
-
-- **List Attributes and Methods**: Understand the `cogflow` module better with:
-    ```python
-    print(dir(cogflow))
-    ```
-
-- **Get Documentation**: For a comprehensive guide on the `cogflow`, use:
-    ```python
-    help(cogflow)
-    ```
-
-## Environment Variables
-
-To maximize the functionality of CogFlow, set the following environment variables:
-
-- **Mlflow Configuration**:
-    - `MLFLOW_TRACKING_URI`: The URI of the Mlflow tracking server.
-    - `MLFLOW_S3_ENDPOINT_URL`: The endpoint URL for the AWS S3 service.
-    - `ACCESS_KEY_ID`: The access key ID for AWS S3 authentication.
-    - `SECRET_ACCESS_KEY`: The secret access key for AWS S3 authentication.
-
-- **Machine Learning Database**:
-    - `ML_DB_USERNAME`: Username for connecting to the machine learning database.
-    - `ML_DB_PASSWORD`: Password for connecting to the machine learning database.
-    - `ML_DB_HOST`: Host address for the machine learning database.
-    - `ML_DB_PORT`: Port number for the machine learning database.
-    - `ML_DB_NAME`: Name of the machine learning database.
-
-- **CogFlow Database**:
-    - `COGFLOW_DB_USERNAME`: Username for connecting to the CogFlow database.
-    - `COGFLOW_DB_PASSWORD`: Password for connecting to the CogFlow database.
-    - `COGFLOW_DB_HOST`: Host address for the CogFlow database.
-    - `COGFLOW_DB_PORT`: Port number for the CogFlow database.
-    - `COGFLOW_DB_NAME`: Name of the CogFlow database.
-
-- **MinIO Configuration**:
-    - `MINIO_ENDPOINT_URL`: The endpoint URL for the MinIO service.
-    - `MINIO_ACCESS_KEY`: The access key for MinIO authentication.
-    - `MINIO_SECRET_ACCESS_KEY`: The secret access key for MinIO authentication.
-
----
-
+
+# CogFlow
+
+CogFlow is a versatile framework designed to manage multiple plugins for cognitive and machine learning tasks. It includes several plugins such as `MlflowPlugin`, `KubeflowPlugin`, and `DatasetPlugin`, which can be activated as needed to extend the capabilities of the framework.
+
+## Getting Started
+
+To begin, import cogflow from the CogFlow module:
+
+```python
+import cogflow
+
+```
+
+### Explore the Capabilities of `cogflow`
+
+- **List Attributes and Methods**: Understand the `cogflow` module better with:
+    ```python
+    print(dir(cogflow))
+    ```
+
+- **Get Documentation**: For a comprehensive guide on the `cogflow`, use:
+    ```python
+    help(cogflow)
+    ```
+
+## Environment Variables
+
+To maximize the functionality of CogFlow, set the following environment variables:
+
+- **Mlflow Configuration**:
+    - `MLFLOW_TRACKING_URI`: The URI of the Mlflow tracking server.
+    - `MLFLOW_S3_ENDPOINT_URL`: The endpoint URL for the AWS S3 service.
+    - `ACCESS_KEY_ID`: The access key ID for AWS S3 authentication.
+    - `SECRET_ACCESS_KEY`: The secret access key for AWS S3 authentication.
+
+- **Machine Learning Database**:
+    - `ML_DB_USERNAME`: Username for connecting to the machine learning database.
+    - `ML_DB_PASSWORD`: Password for connecting to the machine learning database.
+    - `ML_DB_HOST`: Host address for the machine learning database.
+    - `ML_DB_PORT`: Port number for the machine learning database.
+    - `ML_DB_NAME`: Name of the machine learning database.
+
+- **CogFlow Database**:
+    - `COGFLOW_DB_USERNAME`: Username for connecting to the CogFlow database.
+    - `COGFLOW_DB_PASSWORD`: Password for connecting to the CogFlow database.
+    - `COGFLOW_DB_HOST`: Host address for the CogFlow database.
+    - `COGFLOW_DB_PORT`: Port number for the CogFlow database.
+    - `COGFLOW_DB_NAME`: Name of the CogFlow database.
+
+- **MinIO Configuration**:
+    - `MINIO_ENDPOINT_URL`: The endpoint URL for the MinIO service.
+    - `MINIO_ACCESS_KEY`: The access key for MinIO authentication.
+    - `MINIO_SECRET_ACCESS_KEY`: The secret access key for MinIO authentication.
+
+---
+
 By setting the environment variables correctly, you can fully utilize the features and functionalities of the CogFlow framework for your cognitive and machine learning tasks.
```

### Comparing `cogflow-1.9.8/cogflow/__init__.py` & `cogflow-1.9.9/cogflow/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-"""
-This module provides configurations, utilities, and management for the CogFlow plugins.
-
-Attributes:
-    TRACKING_URI (str): The URI for tracking experiments in the machine learning tool.
-    TIMER_IN_SEC (int): Timer interval in seconds, used for scheduling tasks or operations.
-    ML_TOOL (str): The machine learning tool being used (e.g., "mlflow").
-    ACCESS_KEY_ID (str): Access key ID for authentication, typically for AWS services.
-    SECRET_ACCESS_KEY (str): Secret access key for authentication, typically for AWS services.
-    S3_ENDPOINT_URL (str): Endpoint URL for connecting to Amazon S3.
-
-    ML_DB_USERNAME (str): Username for connecting to the machine learning database.
-    ML_DB_PASSWORD (str): Password for connecting to the machine learning database.
-    ML_DB_HOST (str): Host address for the machine learning database.
-    ML_DB_PORT (str): Port number for the machine learning database.
-    ML_DB_NAME (str): Name of the machine learning database.
-
-    COGFLOW_DB_USERNAME (str): Username for connecting to the CogFlow database.
-    COGFLOW_DB_PASSWORD (str): Password for connecting to the CogFlow database.
-    COGFLOW_DB_HOST (str): Host address for the CogFlow database.
-    COGFLOW_DB_PORT (str): Port number for the CogFlow database.
-    COGFLOW_DB_NAME (str): Name of the CogFlow database.
-
-    MINIO_ENDPOINT_URL (str): Endpoint URL for connecting to the MinIO service.
-    MINIO_ACCESS_KEY (str): Access key for authentication with MinIO.
-    MINIO_SECRET_ACCESS_KEY (str): Secret access key for authentication with MinIO.
-
-Imports:
-    plugin_status: Contains plugin status information and management utilities.
-    PluginErrors: Defines custom exceptions for handling plugin-related errors.
-    PluginManager: Provides the PluginManager class for managing CogFlow plugins.
-
-Usage:
-    This module serves as a central configuration hub for the CogFlow framework,
-    allowing easy access to settings and utilities for managing plugins and their
-    dependencies. The module also includes error handling and plugin status management.
-"""
-
-from .plugin_config import (
-    TRACKING_URI,
-    TIMER_IN_SEC,
-    ML_TOOL,
-    ACCESS_KEY_ID,
-    SECRET_ACCESS_KEY,
-    S3_ENDPOINT_URL,
-    ML_DB_USERNAME,
-    ML_DB_PASSWORD,
-    ML_DB_HOST,
-    ML_DB_PORT,
-    ML_DB_NAME,
-    COGFLOW_DB_USERNAME,
-    COGFLOW_DB_PASSWORD,
-    COGFLOW_DB_HOST,
-    COGFLOW_DB_PORT,
-    COGFLOW_DB_NAME,
-    MINIO_ENDPOINT_URL,
-    MINIO_ACCESS_KEY,
-    MINIO_SECRET_ACCESS_KEY,
-)
-
-
-from .pluginmanager import PluginManager
-from .dataset_plugin import DatasetPlugin
-from .kubeflowplugin import CogContainer, KubeflowPlugin
-from .mlflowplugin import MlflowPlugin
-
-
-delete_registered_model = MlflowPlugin().delete_registered_model
-search_registered_models = MlflowPlugin().search_registered_models
-load_model = MlflowPlugin().load_model
-register_model = MlflowPlugin().register_model
-autolog = MlflowPlugin().autolog
-create_registered_model = MlflowPlugin().create_registered_model
-create_model_version = MlflowPlugin().create_model_version
-set_tracking_uri = MlflowPlugin().set_tracking_uri
-set_experiment = MlflowPlugin().set_experiment
-get_artifact_uri = MlflowPlugin().get_artifact_uri
-start_run = MlflowPlugin().start_run
-end_run = MlflowPlugin().end_run
-log_param = MlflowPlugin().log_param
-log_metric = MlflowPlugin().log_metric
-log_model = MlflowPlugin().log_model
-pyfunc = MlflowPlugin().pyfunc
-mlflow = MlflowPlugin().mlflow
-sklearn = MlflowPlugin().sklearn
-cogclient = MlflowPlugin().cogclient
-tensorflow = MlflowPlugin().tensorflow
-pytorch = MlflowPlugin().pytorch
-models = MlflowPlugin().models
-search_model_versions = MlflowPlugin().search_model_versions
-
-
-add_model_access = CogContainer().add_model_access
-pipeline = KubeflowPlugin().pipeline
-create_component_from_func = KubeflowPlugin().create_component_from_func
-client = KubeflowPlugin().client
-load_component_from_url = KubeflowPlugin().load_component_from_url
-input_path = KubeflowPlugin().input_path
-output_path = KubeflowPlugin().output_path
-serve_model_v2 = KubeflowPlugin().serve_model_v2
-serve_model_v1 = KubeflowPlugin().serve_model_v1
-get_model_url = KubeflowPlugin().get_model_url
-kfp = KubeflowPlugin().kfp
-
-
-create_minio_client = DatasetPlugin().create_minio_client
-query_endpoint_and_download_file = DatasetPlugin().query_endpoint_and_download_file
-save_to_minio = DatasetPlugin().save_to_minio
-delete_from_minio = DatasetPlugin().delete_from_minio
-
-__all__ = [
-    # Methods from MlflowPlugin class
-    "delete_registered_model",
-    "search_registered_models",
-    "load_model",
-    "register_model",
-    "autolog",
-    "create_registered_model",
-    "create_model_version",
-    "set_tracking_uri",
-    "set_experiment",
-    "get_artifact_uri",
-    "start_run",
-    "end_run",
-    "log_param",
-    "log_metric",
-    "log_model",
-    "pyfunc",
-    "mlflow",
-    "sklearn",
-    "cogclient",
-    "tensorflow",
-    "pytorch",
-    "models",
-    # Method from CogContainer class
-    "add_model_access",
-    # Methods from KubeflowPlugin class
-    "pipeline",
-    "create_component_from_func",
-    "client",
-    "load_component_from_url",
-    "input_path",
-    "output_path",
-    "serve_model_v2",
-    "serve_model_v1",
-    "get_model_url",
-    "kfp",
-    # Methods from DatasetPlugin class
-    "create_minio_client",
-    "query_endpoint_and_download_file",
-    "save_to_minio",
-    "delete_from_minio",
-]
+"""
+This module provides configurations, utilities, and management for the CogFlow plugins.
+
+Attributes:
+    TRACKING_URI (str): The URI for tracking experiments in the machine learning tool.
+    TIMER_IN_SEC (int): Timer interval in seconds, used for scheduling tasks or operations.
+    ML_TOOL (str): The machine learning tool being used (e.g., "mlflow").
+    ACCESS_KEY_ID (str): Access key ID for authentication, typically for AWS services.
+    SECRET_ACCESS_KEY (str): Secret access key for authentication, typically for AWS services.
+    S3_ENDPOINT_URL (str): Endpoint URL for connecting to Amazon S3.
+
+    ML_DB_USERNAME (str): Username for connecting to the machine learning database.
+    ML_DB_PASSWORD (str): Password for connecting to the machine learning database.
+    ML_DB_HOST (str): Host address for the machine learning database.
+    ML_DB_PORT (str): Port number for the machine learning database.
+    ML_DB_NAME (str): Name of the machine learning database.
+
+    COGFLOW_DB_USERNAME (str): Username for connecting to the CogFlow database.
+    COGFLOW_DB_PASSWORD (str): Password for connecting to the CogFlow database.
+    COGFLOW_DB_HOST (str): Host address for the CogFlow database.
+    COGFLOW_DB_PORT (str): Port number for the CogFlow database.
+    COGFLOW_DB_NAME (str): Name of the CogFlow database.
+
+    MINIO_ENDPOINT_URL (str): Endpoint URL for connecting to the MinIO service.
+    MINIO_ACCESS_KEY (str): Access key for authentication with MinIO.
+    MINIO_SECRET_ACCESS_KEY (str): Secret access key for authentication with MinIO.
+
+Imports:
+    plugin_status: Contains plugin status information and management utilities.
+    PluginErrors: Defines custom exceptions for handling plugin-related errors.
+    PluginManager: Provides the PluginManager class for managing CogFlow plugins.
+
+Usage:
+    This module serves as a central configuration hub for the CogFlow framework,
+    allowing easy access to settings and utilities for managing plugins and their
+    dependencies. The module also includes error handling and plugin status management.
+"""
+
+from .plugin_config import (
+    TRACKING_URI,
+    TIMER_IN_SEC,
+    ML_TOOL,
+    ACCESS_KEY_ID,
+    SECRET_ACCESS_KEY,
+    S3_ENDPOINT_URL,
+    ML_DB_USERNAME,
+    ML_DB_PASSWORD,
+    ML_DB_HOST,
+    ML_DB_PORT,
+    ML_DB_NAME,
+    COGFLOW_DB_USERNAME,
+    COGFLOW_DB_PASSWORD,
+    COGFLOW_DB_HOST,
+    COGFLOW_DB_PORT,
+    COGFLOW_DB_NAME,
+    MINIO_ENDPOINT_URL,
+    MINIO_ACCESS_KEY,
+    MINIO_SECRET_ACCESS_KEY,
+)
+
+
+from .pluginmanager import PluginManager
+from .dataset_plugin import DatasetPlugin
+from .kubeflowplugin import CogContainer, KubeflowPlugin
+from .mlflowplugin import MlflowPlugin
+
+
+delete_registered_model = MlflowPlugin().delete_registered_model
+search_registered_models = MlflowPlugin().search_registered_models
+load_model = MlflowPlugin().load_model
+register_model = MlflowPlugin().register_model
+autolog = MlflowPlugin().autolog
+create_registered_model = MlflowPlugin().create_registered_model
+create_model_version = MlflowPlugin().create_model_version
+set_tracking_uri = MlflowPlugin().set_tracking_uri
+set_experiment = MlflowPlugin().set_experiment
+get_artifact_uri = MlflowPlugin().get_artifact_uri
+start_run = MlflowPlugin().start_run
+end_run = MlflowPlugin().end_run
+log_param = MlflowPlugin().log_param
+log_metric = MlflowPlugin().log_metric
+log_model = MlflowPlugin().log_model
+pyfunc = MlflowPlugin().pyfunc
+mlflow = MlflowPlugin().mlflow
+sklearn = MlflowPlugin().sklearn
+cogclient = MlflowPlugin().cogclient
+tensorflow = MlflowPlugin().tensorflow
+pytorch = MlflowPlugin().pytorch
+models = MlflowPlugin().models
+search_model_versions = MlflowPlugin().search_model_versions
+
+
+add_model_access = CogContainer().add_model_access
+pipeline = KubeflowPlugin().pipeline
+create_component_from_func = KubeflowPlugin().create_component_from_func
+client = KubeflowPlugin().client
+load_component_from_url = KubeflowPlugin().load_component_from_url
+input_path = KubeflowPlugin().input_path
+output_path = KubeflowPlugin().output_path
+serve_model_v2 = KubeflowPlugin().serve_model_v2
+serve_model_v1 = KubeflowPlugin().serve_model_v1
+get_model_url = KubeflowPlugin().get_model_url
+kfp = KubeflowPlugin().kfp
+
+
+create_minio_client = DatasetPlugin().create_minio_client
+query_endpoint_and_download_file = DatasetPlugin().query_endpoint_and_download_file
+save_to_minio = DatasetPlugin().save_to_minio
+delete_from_minio = DatasetPlugin().delete_from_minio
+
+__all__ = [
+    # Methods from MlflowPlugin class
+    "delete_registered_model",
+    "search_registered_models",
+    "load_model",
+    "register_model",
+    "autolog",
+    "create_registered_model",
+    "create_model_version",
+    "set_tracking_uri",
+    "set_experiment",
+    "get_artifact_uri",
+    "start_run",
+    "end_run",
+    "log_param",
+    "log_metric",
+    "log_model",
+    "pyfunc",
+    "mlflow",
+    "sklearn",
+    "cogclient",
+    "tensorflow",
+    "pytorch",
+    "models",
+    # Method from CogContainer class
+    "add_model_access",
+    # Methods from KubeflowPlugin class
+    "pipeline",
+    "create_component_from_func",
+    "client",
+    "load_component_from_url",
+    "input_path",
+    "output_path",
+    "serve_model_v2",
+    "serve_model_v1",
+    "get_model_url",
+    "kfp",
+    # Methods from DatasetPlugin class
+    "create_minio_client",
+    "query_endpoint_and_download_file",
+    "save_to_minio",
+    "delete_from_minio",
+]
```

### Comparing `cogflow-1.9.8/cogflow/dataset_plugin.py` & `cogflow-1.9.9/cogflow/dataset_plugin.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-"""
-This module provides functionality related to Dataset upload via plugin.
-"""
-
-import io
-import os
-import requests
-from minio import Minio
-from . import plugin_config, PluginManager
-
-
-class DatasetPlugin:
-    """
-    A class to handle dataset-related operations.
-    Attributes:
-        None
-    """
-
-    def __init__(self):
-        """
-        Initializes DatasetPlugin with environment variables.
-        """
-        # Retrieve MinIO connection details from environment variables
-        self.minio_endpoint = os.getenv(plugin_config.MINIO_ENDPOINT_URL)
-        # Check if the environment variable exists and has a value
-        if self.minio_endpoint:
-            # Remove the http:// or https:// prefix using string manipulation
-            if self.minio_endpoint.startswith(("http://", "https://")):
-                # Find the index where the protocol ends
-                protocol_end_index = self.minio_endpoint.find("//") + 2
-                # Get the remaining part of the URL (without the protocol)
-                self.minio_endpoint = self.minio_endpoint[protocol_end_index:]
-        else:
-            print("MINIO_ENDPOINT_URL environment variable is not set.")
-        self.minio_access_key = os.getenv(plugin_config.MINIO_ACCESS_KEY)
-        self.minio_secret_key = os.getenv(plugin_config.MINIO_SECRET_ACCESS_KEY)
-        self.section = "dataset_plugin"
-
-    def create_minio_client(self):
-        """
-        Creates a MinIO client object.
-        Returns:
-            Minio: The MinIO client object.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(self.section)
-        return Minio(
-            self.minio_endpoint,
-            access_key=self.minio_access_key,
-            secret_key=self.minio_secret_key,
-            secure=False,
-        )  # Change to True if using HTTPS
-
-    def query_endpoint_and_download_file(self, url, output_file, bucket_name):
-        """
-        Queries an endpoint and downloads a file from it.
-        Args:
-            url (str): The URL of the endpoint.
-            output_file (str): The name of the output file to save.
-        Returns:
-            tuple: A tuple containing a boolean indicating success and the file URL if successful.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(self.section)
-        try:
-            response = requests.get(url)
-            if response.status_code == 200:
-                self.save_to_minio(response.content, output_file, bucket_name)
-                return True
-            print(f"Request failed with status code {response.status_code}")
-            raise Exception("Request could not be successful due to error")
-        except requests.exceptions.RequestException as exp:
-            print(f"An error occurred: {exp}")
-            raise Exception("Exception occurred during the requested operation")
-
-    def save_to_minio(self, file_content, output_file, bucket_name):
-        """
-        Saves a file to MinIO.
-        Args:
-            file_content (bytes): The content of the file to be uploaded.
-            output_file (str): The name of the file to be uploaded.
-            bucket_name (str): The name of the bucket to upload the file to.
-        Returns:
-            str: The presigned URL of the uploaded file.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(self.section)
-        # Initialize MinIO client
-        minio_client = self.create_minio_client()
-        object_name = output_file
-        # Check if the bucket exists, if not, create it
-        bucket_exists = minio_client.bucket_exists(bucket_name)
-        if not bucket_exists:
-            try:
-                minio_client.make_bucket(bucket_name)
-                print(f"Bucket '{bucket_name}' created successfully.")
-            except Exception as exp:
-                print(f"Bucket '{bucket_name}' couldnot be created.")
-                raise exp
-        # Put file to MinIO
-        try:
-            # Upload content to MinIO bucket
-            minio_client.put_object(
-                bucket_name,
-                object_name,
-                io.BytesIO(file_content),
-                len(file_content),
-            )
-            print(
-                f"File {output_file} uploaded successfully to MinIO bucket"
-                f" {bucket_name} as {object_name}."
-            )
-            presigned_url = minio_client.presigned_get_object(bucket_name, object_name)
-            print(f"Access URL for '{object_name}': {presigned_url}")
-            return presigned_url
-        except Exception as err:
-            print(f"Error uploading file: {err}")
-            raise Exception(f"Error uploading file: {err}")
-
-    def delete_from_minio(self, object_name, bucket_name):
-        """
-        Deletes a file from MinIO.
-        Args:
-            object_name (str): The name of the object (file) to be deleted.
-            bucket_name (str): The name of the bucket containing the file.
-        Returns:
-            bool: True if the file was successfully deleted, False otherwise.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(self.section)
-        # Initialize MinIO client
-        minio_client = self.create_minio_client()
-        try:
-            # Check if the object exists
-            object_exists = minio_client.stat_object(bucket_name, object_name)
-            if object_exists:
-                # Delete the object from the bucket
-                minio_client.remove_object(bucket_name, object_name)
-                print(
-                    f"File '{object_name}' deleted successfully from bucket '{bucket_name}'."
-                )
-                return True
-            print(f"File '{object_name}' does not exist in bucket '{bucket_name}'.")
-            return False
-        except Exception as err:
-            print(
-                f"Error deleting file '{object_name}' from bucket '{bucket_name}': {err}"
-            )
-            return False
+"""
+This module provides functionality related to Dataset upload via plugin.
+"""
+
+import io
+import os
+import requests
+from minio import Minio
+from . import plugin_config, PluginManager
+
+
+class DatasetPlugin:
+    """
+    A class to handle dataset-related operations.
+    Attributes:
+        None
+    """
+
+    def __init__(self):
+        """
+        Initializes DatasetPlugin with environment variables.
+        """
+        # Retrieve MinIO connection details from environment variables
+        self.minio_endpoint = os.getenv(plugin_config.MINIO_ENDPOINT_URL)
+        # Check if the environment variable exists and has a value
+        if self.minio_endpoint:
+            # Remove the http:// or https:// prefix using string manipulation
+            if self.minio_endpoint.startswith(("http://", "https://")):
+                # Find the index where the protocol ends
+                protocol_end_index = self.minio_endpoint.find("//") + 2
+                # Get the remaining part of the URL (without the protocol)
+                self.minio_endpoint = self.minio_endpoint[protocol_end_index:]
+        else:
+            print("MINIO_ENDPOINT_URL environment variable is not set.")
+        self.minio_access_key = os.getenv(plugin_config.MINIO_ACCESS_KEY)
+        self.minio_secret_key = os.getenv(plugin_config.MINIO_SECRET_ACCESS_KEY)
+        self.section = "dataset_plugin"
+
+    def create_minio_client(self):
+        """
+        Creates a MinIO client object.
+        Returns:
+            Minio: The MinIO client object.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(self.section)
+        return Minio(
+            self.minio_endpoint,
+            access_key=self.minio_access_key,
+            secret_key=self.minio_secret_key,
+            secure=False,
+        )  # Change to True if using HTTPS
+
+    def query_endpoint_and_download_file(self, url, output_file, bucket_name):
+        """
+        Queries an endpoint and downloads a file from it.
+        Args:
+            url (str): The URL of the endpoint.
+            output_file (str): The name of the output file to save.
+        Returns:
+            tuple: A tuple containing a boolean indicating success and the file URL if successful.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(self.section)
+        try:
+            response = requests.get(url)
+            if response.status_code == 200:
+                self.save_to_minio(response.content, output_file, bucket_name)
+                return True
+            print(f"Request failed with status code {response.status_code}")
+            raise Exception("Request could not be successful due to error")
+        except requests.exceptions.RequestException as exp:
+            print(f"An error occurred: {exp}")
+            raise Exception("Exception occurred during the requested operation")
+
+    def save_to_minio(self, file_content, output_file, bucket_name):
+        """
+        Saves a file to MinIO.
+        Args:
+            file_content (bytes): The content of the file to be uploaded.
+            output_file (str): The name of the file to be uploaded.
+            bucket_name (str): The name of the bucket to upload the file to.
+        Returns:
+            str: The presigned URL of the uploaded file.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(self.section)
+        # Initialize MinIO client
+        minio_client = self.create_minio_client()
+        object_name = output_file
+        # Check if the bucket exists, if not, create it
+        bucket_exists = minio_client.bucket_exists(bucket_name)
+        if not bucket_exists:
+            try:
+                minio_client.make_bucket(bucket_name)
+                print(f"Bucket '{bucket_name}' created successfully.")
+            except Exception as exp:
+                print(f"Bucket '{bucket_name}' couldnot be created.")
+                raise exp
+        # Put file to MinIO
+        try:
+            # Upload content to MinIO bucket
+            minio_client.put_object(
+                bucket_name,
+                object_name,
+                io.BytesIO(file_content),
+                len(file_content),
+            )
+            print(
+                f"File {output_file} uploaded successfully to MinIO bucket"
+                f" {bucket_name} as {object_name}."
+            )
+            presigned_url = minio_client.presigned_get_object(bucket_name, object_name)
+            print(f"Access URL for '{object_name}': {presigned_url}")
+            return presigned_url
+        except Exception as err:
+            print(f"Error uploading file: {err}")
+            raise Exception(f"Error uploading file: {err}")
+
+    def delete_from_minio(self, object_name, bucket_name):
+        """
+        Deletes a file from MinIO.
+        Args:
+            object_name (str): The name of the object (file) to be deleted.
+            bucket_name (str): The name of the bucket containing the file.
+        Returns:
+            bool: True if the file was successfully deleted, False otherwise.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(self.section)
+        # Initialize MinIO client
+        minio_client = self.create_minio_client()
+        try:
+            # Check if the object exists
+            object_exists = minio_client.stat_object(bucket_name, object_name)
+            if object_exists:
+                # Delete the object from the bucket
+                minio_client.remove_object(bucket_name, object_name)
+                print(
+                    f"File '{object_name}' deleted successfully from bucket '{bucket_name}'."
+                )
+                return True
+            print(f"File '{object_name}' does not exist in bucket '{bucket_name}'.")
+            return False
+        except Exception as err:
+            print(
+                f"Error deleting file '{object_name}' from bucket '{bucket_name}': {err}"
+            )
+            return False
```

### Comparing `cogflow-1.9.8/cogflow/kubeflowplugin.py` & `cogflow-1.9.9/cogflow/kubeflowplugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,314 +1,321 @@
-"""
-This module provides functionality related to Kubeflow Pipelines.
-"""
-
-import os
-import time
-from datetime import datetime
-import kfp
-from kfp import dsl
-from kserve import (
-    KServeClient,
-    V1beta1InferenceService,
-    V1beta1InferenceServiceSpec,
-    V1beta1ModelFormat,
-    V1beta1ModelSpec,
-    V1beta1PredictorSpec,
-    V1beta1SKLearnSpec,
-    constants,
-    utils,
-)
-from kubernetes import client
-from kubernetes.client import V1ObjectMeta
-from kubernetes.client.models import V1EnvVar
-from . import plugin_config, PluginManager
-
-
-class CogContainer(kfp.dsl._container_op.Container):
-    """
-    Subclass of Container to add model access environment variables.
-    """
-
-    def __init__(self):
-        """
-        Initializes the CogContainer class.
-        """
-        super().__init__(image=None, command=None, args=None)
-
-    def add_model_access(self):
-        """
-        Adds model access environment variables to the container.
-
-        Returns:
-            CogContainer: Container instance with added environment variables.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        return (
-            self.add_env_variable(
-                V1EnvVar(
-                    name=plugin_config.TRACKING_URI,
-                    value=os.getenv(plugin_config.TRACKING_URI),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=plugin_config.S3_ENDPOINT_URL,
-                    value=os.getenv(plugin_config.S3_ENDPOINT_URL),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=plugin_config.ACCESS_KEY_ID,
-                    value=os.getenv(plugin_config.ACCESS_KEY_ID),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=plugin_config.SECRET_ACCESS_KEY,
-                    value=os.getenv(plugin_config.SECRET_ACCESS_KEY),
-                )
-            )
-        )
-
-
-class KubeflowPlugin:
-    """
-    Class for defining reusable components.
-    """
-
-    def __init__(self, image=None, command=None, args=None):
-        """
-        Initializes the KubeflowPlugin class.
-        """
-        self.kfp = kfp
-        self.kfp.dsl._container_op.Container.AddModelAccess = (
-            CogContainer.add_model_access
-        )
-        self.kfp.dsl._container_op.ContainerOp.AddModelAccess = (
-            CogContainer.add_model_access
-        )
-        self.config_file_path = os.getenv(plugin_config.COGFLOW_CONFIG_FILE_PATH)
-        self.section = "kubeflow_plugin"
-
-    @staticmethod
-    def pipeline(name=None, description=None):
-        """
-        Decorator function to define Kubeflow Pipelines.
-
-        Args:
-            name (str, optional): Name of the pipeline. Defaults to None.
-            description (str, optional): Description of the pipeline. Defaults to None.
-
-        Returns:
-            Callable: Decorator for defining Kubeflow Pipelines.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        return dsl.pipeline(name=name, description=description)
-
-    def create_component_from_func(
-        self,
-        func,
-        output_component_file=None,
-        base_image=None,
-        packages_to_install=None,
-    ):
-        """
-        Create a component from a Python function.
-
-        Args:
-            func (Callable): Python function to convert into a component.
-            output_component_file (str, optional): Path to save the component YAML file. Defaults
-            to None.
-            base_image (str, optional): Base Docker image for the component. Defaults to None.
-            packages_to_install (List[str], optional): List of additional Python packages
-            to install in the component.
-            Defaults to None.
-
-        Returns:
-            kfp.components.ComponentSpec: Component specification.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        training_var = kfp.components.create_component_from_func(
-            func=func,
-            output_component_file=output_component_file,
-            base_image=base_image,
-            packages_to_install=packages_to_install,
-        )
-        self.kfp.dsl._container_op.ContainerOp.AddModelAccess = (
-            CogContainer.add_model_access
-        )
-        return training_var
-
-    @staticmethod
-    def client():
-        """
-        Get the Kubeflow Pipeline client.
-
-        Returns:
-            kfp.Client: Kubeflow Pipeline client instance.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        return kfp.Client()
-
-    @staticmethod
-    def load_component_from_url(url):
-        """
-        Load a component from a URL.
-
-        Args:
-            url (str): URL to load the component from.
-
-        Returns:
-            kfp.components.ComponentSpec: Loaded component specification.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        return kfp.components.load_component_from_url(url)
-
-    @staticmethod
-    def input_path(label: str):
-        """
-        Create an InputPath component.
-
-        Args:
-            label (str): Label for the input path.
-
-        Returns:
-            InputPath: InputPath component instance.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        return kfp.components.InputPath(label)
-
-    @staticmethod
-    def output_path(label: str):
-        """
-        Create an OutputPath component.
-
-        Args:
-            label (str): Label for the output path.
-
-        Returns:
-            OutputPath: OutputPath component instance.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        return kfp.components.OutputPath(label)
-
-    @staticmethod
-    def serve_model_v2(model_uri: str, name: str = None):
-        """
-        Create a kserve instance.
-
-        Args:
-            model_uri (str): URI of the model.
-            name (str, optional): Name of the kserve instance. If not provided,
-            a default name will be generated.
-
-        Returns:
-            None
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        namespace = utils.get_default_target_namespace()
-        if name is None:
-            now = datetime.now()
-            v = now.strftime("%d%M")
-            name = f"predictor_model{v}"
-        isvc_name = name
-        predictor = V1beta1PredictorSpec(
-            service_account_name="kserve-controller-s3",
-            min_replicas=1,
-            model=V1beta1ModelSpec(
-                model_format=V1beta1ModelFormat(
-                    name=plugin_config.ML_TOOL,
-                ),
-                storage_uri=model_uri,
-                protocol_version="v2",
-            ),
-        )
-
-        isvc = V1beta1InferenceService(
-            api_version=constants.KSERVE_V1BETA1,
-            kind=constants.KSERVE_KIND,
-            metadata=client.V1ObjectMeta(
-                name=isvc_name,
-                namespace=namespace,
-                annotations={"sidecar.istio.io/inject": "false"},
-            ),
-            spec=V1beta1InferenceServiceSpec(predictor=predictor),
-        )
-        kserve = KServeClient()
-        kserve.create(isvc)
-        time.sleep(plugin_config.TIMER_IN_SEC)
-
-    @staticmethod
-    def serve_model_v1(model_uri: str, name: str = None):
-        """
-        Create a kserve instance version1.
-
-        Args:
-            model_uri (str): URI of the model.
-            name (str, optional): Name of the kserve instance. If not provided,
-            a default name will be generated.
-
-        Returns:
-            None
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        isvc_name = name
-        namespace = utils.get_default_target_namespace()
-        isvc = V1beta1InferenceService(
-            api_version=constants.KSERVE_V1BETA1,
-            kind=constants.KSERVE_KIND,
-            metadata=V1ObjectMeta(
-                name=isvc_name,
-                namespace=namespace,
-                annotations={"sidecar.istio.io/inject": "false"},
-            ),
-            spec=V1beta1InferenceServiceSpec(
-                predictor=V1beta1PredictorSpec(
-                    service_account_name="kserve-controller-s3",
-                    sklearn=V1beta1SKLearnSpec(storage_uri=model_uri),
-                )
-            ),
-        )
-
-        kclient = KServeClient()
-        kclient.create(isvc)
-        time.sleep(plugin_config.TIMER_IN_SEC)
-
-    @staticmethod
-    def get_model_url(model_name: str):
-        """
-        Retrieve the URL of a deployed model.
-
-        Args:
-            model_name (str): Name of the deployed model.
-
-        Returns:
-            str: URL of the deployed model.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(KubeflowPlugin().section)
-
-        kclient = KServeClient()
-
-        time.sleep(plugin_config.TIMER_IN_SEC)
-        isvc_resp = kclient.get(model_name)
-        isvc_url = isvc_resp["status"]["address"]["url"]
-        return isvc_url
+"""
+This module provides functionality related to Kubeflow Pipelines.
+"""
+
+import os
+import time
+from datetime import datetime
+import kfp
+from kfp import dsl
+from kserve import (
+    KServeClient,
+    V1beta1InferenceService,
+    V1beta1InferenceServiceSpec,
+    V1beta1ModelFormat,
+    V1beta1ModelSpec,
+    V1beta1PredictorSpec,
+    V1beta1SKLearnSpec,
+    constants,
+    utils,
+)
+from kubernetes import client
+from kubernetes.client import V1ObjectMeta
+from kubernetes.client.models import V1EnvVar
+from . import plugin_config, PluginManager
+
+
+class CogContainer(kfp.dsl._container_op.Container):
+    """
+    Subclass of Container to add model access environment variables.
+    """
+
+    def __init__(self):
+        """
+        Initializes the CogContainer class.
+        """
+        super().__init__(image=None, command=None, args=None)
+
+    def add_model_access(self):
+        """
+        Adds model access environment variables to the container.
+
+        Returns:
+            CogContainer: Container instance with added environment variables.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        return (
+            self.add_env_variable(
+                V1EnvVar(
+                    name=plugin_config.TRACKING_URI,
+                    value=os.getenv(plugin_config.TRACKING_URI),
+                )
+            )
+            .add_env_variable(
+                V1EnvVar(
+                    name=plugin_config.S3_ENDPOINT_URL,
+                    value=os.getenv(plugin_config.S3_ENDPOINT_URL),
+                )
+            )
+            .add_env_variable(
+                V1EnvVar(
+                    name=plugin_config.ACCESS_KEY_ID,
+                    value=os.getenv(plugin_config.ACCESS_KEY_ID),
+                )
+            )
+            .add_env_variable(
+                V1EnvVar(
+                    name=plugin_config.SECRET_ACCESS_KEY,
+                    value=os.getenv(plugin_config.SECRET_ACCESS_KEY),
+                )
+            )
+        )
+
+
+class KubeflowPlugin:
+    """
+    Class for defining reusable components.
+    """
+
+    def __init__(self, image=None, command=None, args=None):
+        """
+        Initializes the KubeflowPlugin class.
+        """
+        self.kfp = kfp
+        self.kfp.dsl._container_op.Container.AddModelAccess = (
+            CogContainer.add_model_access
+        )
+        self.kfp.dsl._container_op.ContainerOp.AddModelAccess = (
+            CogContainer.add_model_access
+        )
+        self.config_file_path = os.getenv(plugin_config.COGFLOW_CONFIG_FILE_PATH)
+        self.section = "kubeflow_plugin"
+
+    @staticmethod
+    def pipeline(name=None, description=None):
+        """
+        Decorator function to define Kubeflow Pipelines.
+
+        Args:
+            name (str, optional): Name of the pipeline. Defaults to None.
+            description (str, optional): Description of the pipeline. Defaults to None.
+
+        Returns:
+            Callable: Decorator for defining Kubeflow Pipelines.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        return dsl.pipeline(name=name, description=description)
+
+    def create_component_from_func(
+        self,
+        func,
+        output_component_file=None,
+        base_image=None,
+        packages_to_install=None,
+    ):
+        """
+        Create a component from a Python function.
+
+        Args:
+            func (Callable): Python function to convert into a component.
+            output_component_file (str, optional): Path to save the component YAML file. Defaults
+            to None.
+            base_image (str, optional): Base Docker image for the component. Defaults to None.
+            packages_to_install (List[str], optional): List of additional Python packages
+            to install in the component.
+            Defaults to None.
+
+        Returns:
+            kfp.components.ComponentSpec: Component specification.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        training_var = kfp.components.create_component_from_func(
+            func=func,
+            output_component_file=output_component_file,
+            base_image=base_image,
+            packages_to_install=packages_to_install,
+        )
+        self.kfp.dsl._container_op.ContainerOp.AddModelAccess = (
+            CogContainer.add_model_access
+        )
+        return training_var
+
+    @staticmethod
+    def client():
+        """
+        Get the Kubeflow Pipeline client.
+
+        Returns:
+            kfp.Client: Kubeflow Pipeline client instance.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        return kfp.Client()
+
+    @staticmethod
+    def load_component_from_url(url):
+        """
+        Load a component from a URL.
+
+        Args:
+            url (str): URL to load the component from.
+
+        Returns:
+            kfp.components.ComponentSpec: Loaded component specification.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        return kfp.components.load_component_from_url(url)
+
+    @staticmethod
+    def input_path(label: str):
+        """
+        Create an InputPath component.
+
+        Args:
+            label (str): Label for the input path.
+
+        Returns:
+            InputPath: InputPath component instance.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        return kfp.components.InputPath(label)
+
+    @staticmethod
+    def output_path(label: str):
+        """
+        Create an OutputPath component.
+
+        Args:
+            label (str): Label for the output path.
+
+        Returns:
+            OutputPath: OutputPath component instance.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        return kfp.components.OutputPath(label)
+
+    @staticmethod
+    def serve_model_v2(model_uri: str, name: str = None):
+        """
+        Create a kserve instance.
+
+        Args:
+            model_uri (str): URI of the model.
+            name (str, optional): Name of the kserve instance. If not provided,
+            a default name will be generated.
+
+        Returns:
+            None
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        namespace = utils.get_default_target_namespace()
+        if name is None:
+            now = datetime.now()
+            v = now.strftime("%d%M")
+            name = f"predictor_model{v}"
+        isvc_name = name
+        predictor = V1beta1PredictorSpec(
+            service_account_name="kserve-controller-s3",
+            min_replicas=1,
+            model=V1beta1ModelSpec(
+                model_format=V1beta1ModelFormat(
+                    name=plugin_config.ML_TOOL,
+                ),
+                storage_uri=model_uri,
+                protocol_version="v2",
+            ),
+        )
+
+        isvc = V1beta1InferenceService(
+            api_version=constants.KSERVE_V1BETA1,
+            kind=constants.KSERVE_KIND,
+            metadata=client.V1ObjectMeta(
+                name=isvc_name,
+                namespace=namespace,
+                annotations={"sidecar.istio.io/inject": "false"},
+            ),
+            spec=V1beta1InferenceServiceSpec(predictor=predictor),
+        )
+        kserve = KServeClient()
+        kserve.create(isvc)
+        time.sleep(plugin_config.TIMER_IN_SEC)
+
+    @staticmethod
+    def serve_model_v1(model_uri: str, name: str = None):
+        """
+        Create a kserve instance version1.
+
+        Args:
+            model_uri (str): URI of the model.
+            name (str, optional): Name of the kserve instance. If not provided,
+            a default name will be generated.
+
+        Returns:
+            None
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        isvc_name = name
+        namespace = utils.get_default_target_namespace()
+        isvc = V1beta1InferenceService(
+            api_version=constants.KSERVE_V1BETA1,
+            kind=constants.KSERVE_KIND,
+            metadata=V1ObjectMeta(
+                name=isvc_name,
+                namespace=namespace,
+                annotations={"sidecar.istio.io/inject": "false"},
+            ),
+            spec=V1beta1InferenceServiceSpec(
+                predictor=V1beta1PredictorSpec(
+                    service_account_name="kserve-controller-s3",
+                    sklearn=V1beta1SKLearnSpec(storage_uri=model_uri),
+                )
+            ),
+        )
+
+        kclient = KServeClient()
+        kclient.create(isvc)
+        time.sleep(plugin_config.TIMER_IN_SEC)
+
+    @staticmethod
+    def get_model_url(model_name: str, max_wait_time: int = 60):
+        """
+        Retrieve the URL of a deployed model.
+
+        Args:
+            model_name (str): Name of the deployed model.
+            max_wait_time (int): Maximum time to wait for the model address, in seconds. Default is 60 seconds.
+        Returns:
+            str: URL of the deployed model if available within the timeout, otherwise None.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(KubeflowPlugin().section)
+
+        kclient = KServeClient()
+
+        start_time = time.time()
+        while time.time() - start_time < max_wait_time:
+            isvc_resp = kclient.get(model_name)
+            if "status" in isvc_resp and "address" in isvc_resp["status"] and "url" in isvc_resp["status"]["address"]:
+                isvc_url = isvc_resp["status"]["address"]["url"]
+                return isvc_url
+            else:
+                time.sleep(1)  # Wait for 1 second before checking again
+
+        # If max_wait_time is reached without getting the address, return timeout message
+        return f"Timeout: Unable to retrieve the URL for model '{model_name}' within {max_wait_time} seconds."
```

### Comparing `cogflow-1.9.8/cogflow/mlflowplugin.py` & `cogflow-1.9.9/cogflow/mlflowplugin.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,468 +1,468 @@
-"""
-This module provides functionality related to Mlflow.
-"""
-
-import os
-from typing import Union, Any, List, Optional
-
-import mlflow as ml
-import numpy as np
-import pandas as pd
-import requests
-from mlflow.models.signature import ModelSignature
-from mlflow.tracking import MlflowClient
-from scipy.sparse import csr_matrix, csc_matrix
-
-from . import plugin_config, PluginManager
-
-
-class CogModel(ml.pyfunc.PythonModel):
-    """
-    A custom Mlflow PythonModel implementation for demonstration purposes.
-    """
-
-    @staticmethod
-    def fit():
-        """
-        Train the model.
-
-        This method is called to train the model.
-        """
-        print("Fitting model...")
-
-    def predict(self, model_input: [str]):  # type: ignore
-        """
-        Generate predictions.
-
-        This method generates predictions based on the input data.
-
-        Parameters:
-            model_input (List[str]): List of input strings for prediction.
-
-        Returns:
-            None: This method prints the predictions instead of returning them.
-        """
-        print(self.get_prediction(model_input))
-
-    def get_prediction(self, model_input: [str]):  # type: ignore
-        """
-        Generate predictions.
-
-        This method generates predictions based on the input data.
-
-        Parameters:
-            model_input (List[str]): List of input strings for prediction.
-
-        Returns:
-            str: The concatenated uppercase version of the input strings.
-        """
-
-        return " ".join([w.upper() for w in model_input])
-
-
-class MlflowPlugin:
-    """
-    Class for defining reusable components.
-    """
-
-    def __init__(self):
-        """
-        Initializes the MlFlowPlugin class.
-        """
-        self.mlflow = ml
-        self.sklearn = ml.sklearn
-        self.cogclient = MlflowClient()
-        self.pyfunc = ml.pyfunc
-        self.tensorflow = ml.tensorflow
-        self.pytorch = ml.pytorch
-        self.models = ml.models
-        self.section = "mlflow_plugin"
-
-    def is_alive(self):
-        """
-        Check if Mlflow UI is accessible.
-
-        Returns:
-            tuple: A tuple containing a boolean indicating if Mlflow UI is accessible
-             and the status code of the response.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        try:
-            response = requests.get(os.getenv(plugin_config.TRACKING_URI))
-
-            if response.status_code == 200:
-                pass
-            else:
-                print(
-                    f"Mlflow UI is not accessible. Status code: {response.status_code}, "
-                    f"Message: {response.text}"
-                )
-            return response.status_code, response.text
-        except Exception as e:
-            print(f"An error occurred while accessing Mlflow UI: {str(e)}, ")
-            raise e
-
-    @staticmethod
-    def version():
-        """
-        Retrieve the version of the Mlflow.
-
-        Returns:
-            str: Version of the Mlflow.
-        """
-        return ml.__version__
-
-    def delete_registered_model(self, model_name):
-        """
-        Deletes a registered model with the given name.
-
-        Args:
-            model_name (str): The name of the registered model to delete.
-
-        Returns:
-            bool: True if the model was successfully deleted, False otherwise.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.cogclient.delete_registered_model(model_name)
-
-    def search_registered_models(self):
-        """
-        Searches for registered models.
-
-        Returns:
-            list: A list of registered model objects matching the search criteria.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        registered_models = self.cogclient.search_registered_models()
-        return registered_models
-
-    def load_model(self, model_uri: str, dst_path=None):
-        """
-        Loads a model from the specified Mlflow model URI.
-
-        Args:
-            model_uri (str): The URI of the Mlflow model to load.
-            dst_path (str, optional): Optional path where the model will be downloaded and saved.
-             If not provided, the model will be loaded without saving.
-
-        Returns:
-            loaded_model: The loaded Mlflow model.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        loaded_model = ml.sklearn.load_model(model_uri, dst_path)
-        return loaded_model
-
-    def register_model(self, model, model_uri):
-        """
-        Registers the given model with Mlflow.
-
-        Args:
-            model: The model object to register.
-            model_uri (str): The Mlflow model URI.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return ml.register_model(model, model_uri)
-
-    def autolog(self):
-        """
-        Enable automatic logging of parameters, metrics, and models with Mlflow.
-
-        Returns:
-            None
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.autolog()
-
-    def create_registered_model(self, name):
-        """
-        Create a registered model.
-
-        Args:
-            name (str): Name of the registered model.
-
-        Returns:
-            str: ID of the created registered model.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.cogclient.create_registered_model(name)
-
-    def create_model_version(self, name, source):
-        """
-        Create a model version for a registered model.
-
-        Args:
-            name (str): Name of the registered model.
-            source (str): Source path or URI of the model.
-
-        Returns:
-            str: ID of the created model version.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.cogclient.create_model_version(name, source)
-
-    def set_tracking_uri(self, tracking_uri):
-        """
-        Set the Mlflow tracking URI.
-
-        Args:
-            tracking_uri (str): The URI of the Mlflow tracking server.
-
-        Returns:
-            None
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.set_tracking_uri(tracking_uri)
-
-    def set_experiment(self, experiment_name):
-        """
-        Set the active Mlflow experiment.
-
-        Args:
-            experiment_name (str): The name of the experiment to set as active.
-
-        Returns:
-            None
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.set_experiment(experiment_name)
-
-    def get_artifact_uri(self, run_id=None):
-        """
-        Get the artifact URI of the current or specified Mlflow run.
-
-        Args:
-            run_id (str, optional): ID of the Mlflow run. If not provided,
-            the current run's artifact URI is returned.
-
-        Returns:
-            str: Artifact URI of the specified Mlflow run.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.get_artifact_uri(run_id)
-
-    def start_run(self, run_name=None):
-        """
-        Start a Mlflow run.
-
-        Args:
-            run_name (str): Name of the Mlflow run.
-
-        Returns:
-            Mlflow Run object
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.start_run(run_name=run_name)
-
-    def end_run(self):
-        """
-        End a Mlflow run.
-
-        Returns:
-            Mlflow Run object
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.end_run()
-
-    def log_param(self, key: str, value: Any, synchronous: bool = True) -> None:
-        """
-        Log a parameter to the Mlflow run.
-
-        Args:
-            key (str): The key of the parameter to log.
-            value (Any): The value of the parameter to log.
-            synchronous (bool, optional): If True, logs the parameter synchronously.
-                Defaults to True.
-
-        Returns:
-            None
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.log_param(key, value, synchronous)
-
-    def log_metric(
-        self,
-        key: str,
-        value: float,
-        step: Optional[int] = None,
-        synchronous: Optional[bool] = None,
-        timestamp: Optional[int] = None,
-        run_id: Optional[str] = None,
-    ) -> None:
-        """
-        Log a metric to the Mlflow run.
-
-        Args:
-            key (str): The name of the metric to log.
-            value (float): The value of the metric to log.
-            step (Optional[int], optional): Step to log the metric at. Defaults to None.
-            synchronous (Optional[bool], optional): Whether to log synchronously. Defaults to True.
-            timestamp (Optional[int], optional): The timestamp of the metric. Defaults to None.
-            run_id (Optional[str], optional): The run ID. Defaults to None.
-
-        Returns:
-            None
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.log_metric(
-            key,
-            value,
-            step=step,
-            synchronous=synchronous,
-            timestamp=timestamp,
-            run_id=run_id,
-        )
-
-    def log_model(
-        self,
-        sk_model,
-        artifact_path,
-        conda_env=None,
-        code_paths=None,
-        serialization_format="cloudpickle",
-        registered_model_name=None,
-        signature: ModelSignature = None,
-        input_example: Union[
-            pd.DataFrame,
-            np.ndarray,
-            dict,
-            list,
-            csr_matrix,
-            csc_matrix,
-            str,
-            bytes,
-            tuple,
-        ] = None,
-        await_registration_for=300,
-        pip_requirements=None,
-        extra_pip_requirements=None,
-        pyfunc_predict_fn="predict",
-        metadata=None,
-    ):
-        """
-        Log a scikit-learn model to Mlflow.
-
-        Args:
-            sk_model: The scikit-learn model to be logged.
-            artifact_path (str): The run-relative artifact path to which the model artifacts will
-            be saved.
-            conda_env (str, optional): The path to a Conda environment YAML file. Defaults to None.
-            code_paths (list, optional): A list of local filesystem paths to Python files that
-            contain code to be
-            included as part of the model's logged artifacts. Defaults to None.
-            serialization_format (str, optional): The format used to serialize the model. Defaults
-            to "cloudpickle".
-            registered_model_name (str, optional): The name under which to register the model with
-            Mlflow. Defaults to None.
-            signature (ModelSignature, optional): The signature defining model input and output
-            data types and shapes. Defaults to None.
-            input_example (Union[pd.DataFrame, np.ndarray, dict, list, csr_matrix, csc_matrix, str,
-            bytes, tuple], optional): An example input to the model. Defaults to None.
-            await_registration_for (int, optional): The duration, in seconds, to wait for the
-            model version to finish being created and is in the READY status. Defaults to 300.
-            pip_requirements (str, optional): A file in pip requirements format specifying
-            additional pip dependencies for the model environment. Defaults to None.
-            extra_pip_requirements (str, optional): A string containing additional pip dependencies
-            that should be added to the environment. Defaults to None.
-            pyfunc_predict_fn (str, optional): The name of the function to invoke for prediction,
-            when the model is a PyFunc model. Defaults to "predict".
-            metadata (dict, optional): A dictionary of metadata to log with the model.
-            Defaults to None.
-
-        Returns:
-            Model: The logged scikit-learn model.
-
-        Raises:
-            Exception: If an error occurs during the logging process.
-
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.sklearn.log_model(
-            sk_model=sk_model,
-            artifact_path=artifact_path,
-            conda_env=conda_env,
-            code_paths=code_paths,
-            serialization_format=serialization_format,
-            registered_model_name=registered_model_name,
-            signature=signature,
-            input_example=input_example,
-            await_registration_for=await_registration_for,
-            pip_requirements=pip_requirements,
-            extra_pip_requirements=extra_pip_requirements,
-            pyfunc_predict_fn=pyfunc_predict_fn,
-            metadata=metadata,
-        )
-
-    def search_model_versions(
-        self,
-        filter_string: Optional[str] = None,
-        order_by: Optional[List[str]] = None,
-    ):
-        """
-        Searches for model versions in the model registry based on the specified
-        filters and ordering.
-
-        Args:
-            filter_string (Optional[str], optional): A string specifying the conditions
-            that the model versions must meet.
-                It is used to filter the model versions. Examples of filter strings
-                include "name='my-model'"
-                or "name='my-model' and version='1'". If not provided, all model
-                versions are returned.
-                Defaults to None.
-            order_by (Optional[List[str]], optional): A list of strings specifying how to
-            order the model versions.
-                Examples of ordering criteria include "name ASC" or "version DESC".
-                If not provided, the model versions are ordered by their creation time in
-                descending order.
-                Defaults to None.
-
-        Returns:
-            List[dict]: A list of dictionaries, each representing a model version that meets
-            the filter and ordering criteria.
-                Each dictionary contains information about the model version, including
-                its name, version number, creation
-                time, run ID, and other metadata.
-
-        Raises:
-            Exception: If the plugin is not activated.
-        """
-        # Verify plugin activation
-        PluginManager().verify_activation(MlflowPlugin().section)
-
-        return self.mlflow.search_model_versions(
-            max_results=None,
-            filter_string=filter_string,
-            order_by=order_by,
-        )
+"""
+This module provides functionality related to Mlflow.
+"""
+
+import os
+from typing import Union, Any, List, Optional
+
+import mlflow as ml
+import numpy as np
+import pandas as pd
+import requests
+from mlflow.models.signature import ModelSignature
+from mlflow.tracking import MlflowClient
+from scipy.sparse import csr_matrix, csc_matrix
+
+from . import plugin_config, PluginManager
+
+
+class CogModel(ml.pyfunc.PythonModel):
+    """
+    A custom Mlflow PythonModel implementation for demonstration purposes.
+    """
+
+    @staticmethod
+    def fit():
+        """
+        Train the model.
+
+        This method is called to train the model.
+        """
+        print("Fitting model...")
+
+    def predict(self, model_input: [str]):  # type: ignore
+        """
+        Generate predictions.
+
+        This method generates predictions based on the input data.
+
+        Parameters:
+            model_input (List[str]): List of input strings for prediction.
+
+        Returns:
+            None: This method prints the predictions instead of returning them.
+        """
+        print(self.get_prediction(model_input))
+
+    def get_prediction(self, model_input: [str]):  # type: ignore
+        """
+        Generate predictions.
+
+        This method generates predictions based on the input data.
+
+        Parameters:
+            model_input (List[str]): List of input strings for prediction.
+
+        Returns:
+            str: The concatenated uppercase version of the input strings.
+        """
+
+        return " ".join([w.upper() for w in model_input])
+
+
+class MlflowPlugin:
+    """
+    Class for defining reusable components.
+    """
+
+    def __init__(self):
+        """
+        Initializes the MlFlowPlugin class.
+        """
+        self.mlflow = ml
+        self.sklearn = ml.sklearn
+        self.cogclient = MlflowClient()
+        self.pyfunc = ml.pyfunc
+        self.tensorflow = ml.tensorflow
+        self.pytorch = ml.pytorch
+        self.models = ml.models
+        self.section = "mlflow_plugin"
+
+    def is_alive(self):
+        """
+        Check if Mlflow UI is accessible.
+
+        Returns:
+            tuple: A tuple containing a boolean indicating if Mlflow UI is accessible
+             and the status code of the response.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        try:
+            response = requests.get(os.getenv(plugin_config.TRACKING_URI))
+
+            if response.status_code == 200:
+                pass
+            else:
+                print(
+                    f"Mlflow UI is not accessible. Status code: {response.status_code}, "
+                    f"Message: {response.text}"
+                )
+            return response.status_code, response.text
+        except Exception as e:
+            print(f"An error occurred while accessing Mlflow UI: {str(e)}, ")
+            raise e
+
+    @staticmethod
+    def version():
+        """
+        Retrieve the version of the Mlflow.
+
+        Returns:
+            str: Version of the Mlflow.
+        """
+        return ml.__version__
+
+    def delete_registered_model(self, model_name):
+        """
+        Deletes a registered model with the given name.
+
+        Args:
+            model_name (str): The name of the registered model to delete.
+
+        Returns:
+            bool: True if the model was successfully deleted, False otherwise.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.cogclient.delete_registered_model(model_name)
+
+    def search_registered_models(self):
+        """
+        Searches for registered models.
+
+        Returns:
+            list: A list of registered model objects matching the search criteria.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        registered_models = self.cogclient.search_registered_models()
+        return registered_models
+
+    def load_model(self, model_uri: str, dst_path=None):
+        """
+        Loads a model from the specified Mlflow model URI.
+
+        Args:
+            model_uri (str): The URI of the Mlflow model to load.
+            dst_path (str, optional): Optional path where the model will be downloaded and saved.
+             If not provided, the model will be loaded without saving.
+
+        Returns:
+            loaded_model: The loaded Mlflow model.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        loaded_model = ml.sklearn.load_model(model_uri, dst_path)
+        return loaded_model
+
+    def register_model(self, model, model_uri):
+        """
+        Registers the given model with Mlflow.
+
+        Args:
+            model: The model object to register.
+            model_uri (str): The Mlflow model URI.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return ml.register_model(model, model_uri)
+
+    def autolog(self):
+        """
+        Enable automatic logging of parameters, metrics, and models with Mlflow.
+
+        Returns:
+            None
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.autolog()
+
+    def create_registered_model(self, name):
+        """
+        Create a registered model.
+
+        Args:
+            name (str): Name of the registered model.
+
+        Returns:
+            str: ID of the created registered model.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.cogclient.create_registered_model(name)
+
+    def create_model_version(self, name, source):
+        """
+        Create a model version for a registered model.
+
+        Args:
+            name (str): Name of the registered model.
+            source (str): Source path or URI of the model.
+
+        Returns:
+            str: ID of the created model version.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.cogclient.create_model_version(name, source)
+
+    def set_tracking_uri(self, tracking_uri):
+        """
+        Set the Mlflow tracking URI.
+
+        Args:
+            tracking_uri (str): The URI of the Mlflow tracking server.
+
+        Returns:
+            None
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.set_tracking_uri(tracking_uri)
+
+    def set_experiment(self, experiment_name):
+        """
+        Set the active Mlflow experiment.
+
+        Args:
+            experiment_name (str): The name of the experiment to set as active.
+
+        Returns:
+            None
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.set_experiment(experiment_name)
+
+    def get_artifact_uri(self, run_id=None):
+        """
+        Get the artifact URI of the current or specified Mlflow run.
+
+        Args:
+            run_id (str, optional): ID of the Mlflow run. If not provided,
+            the current run's artifact URI is returned.
+
+        Returns:
+            str: Artifact URI of the specified Mlflow run.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.get_artifact_uri(run_id)
+
+    def start_run(self, run_name=None):
+        """
+        Start a Mlflow run.
+
+        Args:
+            run_name (str): Name of the Mlflow run.
+
+        Returns:
+            Mlflow Run object
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.start_run(run_name=run_name)
+
+    def end_run(self):
+        """
+        End a Mlflow run.
+
+        Returns:
+            Mlflow Run object
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.end_run()
+
+    def log_param(self, key: str, value: Any, synchronous: bool = True) -> None:
+        """
+        Log a parameter to the Mlflow run.
+
+        Args:
+            key (str): The key of the parameter to log.
+            value (Any): The value of the parameter to log.
+            synchronous (bool, optional): If True, logs the parameter synchronously.
+                Defaults to True.
+
+        Returns:
+            None
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.log_param(key, value, synchronous)
+
+    def log_metric(
+        self,
+        key: str,
+        value: float,
+        step: Optional[int] = None,
+        synchronous: Optional[bool] = None,
+        timestamp: Optional[int] = None,
+        run_id: Optional[str] = None,
+    ) -> None:
+        """
+        Log a metric to the Mlflow run.
+
+        Args:
+            key (str): The name of the metric to log.
+            value (float): The value of the metric to log.
+            step (Optional[int], optional): Step to log the metric at. Defaults to None.
+            synchronous (Optional[bool], optional): Whether to log synchronously. Defaults to True.
+            timestamp (Optional[int], optional): The timestamp of the metric. Defaults to None.
+            run_id (Optional[str], optional): The run ID. Defaults to None.
+
+        Returns:
+            None
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.log_metric(
+            key,
+            value,
+            step=step,
+            synchronous=synchronous,
+            timestamp=timestamp,
+            run_id=run_id,
+        )
+
+    def log_model(
+        self,
+        sk_model,
+        artifact_path,
+        conda_env=None,
+        code_paths=None,
+        serialization_format="cloudpickle",
+        registered_model_name=None,
+        signature: ModelSignature = None,
+        input_example: Union[
+            pd.DataFrame,
+            np.ndarray,
+            dict,
+            list,
+            csr_matrix,
+            csc_matrix,
+            str,
+            bytes,
+            tuple,
+        ] = None,
+        await_registration_for=300,
+        pip_requirements=None,
+        extra_pip_requirements=None,
+        pyfunc_predict_fn="predict",
+        metadata=None,
+    ):
+        """
+        Log a scikit-learn model to Mlflow.
+
+        Args:
+            sk_model: The scikit-learn model to be logged.
+            artifact_path (str): The run-relative artifact path to which the model artifacts will
+            be saved.
+            conda_env (str, optional): The path to a Conda environment YAML file. Defaults to None.
+            code_paths (list, optional): A list of local filesystem paths to Python files that
+            contain code to be
+            included as part of the model's logged artifacts. Defaults to None.
+            serialization_format (str, optional): The format used to serialize the model. Defaults
+            to "cloudpickle".
+            registered_model_name (str, optional): The name under which to register the model with
+            Mlflow. Defaults to None.
+            signature (ModelSignature, optional): The signature defining model input and output
+            data types and shapes. Defaults to None.
+            input_example (Union[pd.DataFrame, np.ndarray, dict, list, csr_matrix, csc_matrix, str,
+            bytes, tuple], optional): An example input to the model. Defaults to None.
+            await_registration_for (int, optional): The duration, in seconds, to wait for the
+            model version to finish being created and is in the READY status. Defaults to 300.
+            pip_requirements (str, optional): A file in pip requirements format specifying
+            additional pip dependencies for the model environment. Defaults to None.
+            extra_pip_requirements (str, optional): A string containing additional pip dependencies
+            that should be added to the environment. Defaults to None.
+            pyfunc_predict_fn (str, optional): The name of the function to invoke for prediction,
+            when the model is a PyFunc model. Defaults to "predict".
+            metadata (dict, optional): A dictionary of metadata to log with the model.
+            Defaults to None.
+
+        Returns:
+            Model: The logged scikit-learn model.
+
+        Raises:
+            Exception: If an error occurs during the logging process.
+
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.sklearn.log_model(
+            sk_model=sk_model,
+            artifact_path=artifact_path,
+            conda_env=conda_env,
+            code_paths=code_paths,
+            serialization_format=serialization_format,
+            registered_model_name=registered_model_name,
+            signature=signature,
+            input_example=input_example,
+            await_registration_for=await_registration_for,
+            pip_requirements=pip_requirements,
+            extra_pip_requirements=extra_pip_requirements,
+            pyfunc_predict_fn=pyfunc_predict_fn,
+            metadata=metadata,
+        )
+
+    def search_model_versions(
+        self,
+        filter_string: Optional[str] = None,
+        order_by: Optional[List[str]] = None,
+    ):
+        """
+        Searches for model versions in the model registry based on the specified
+        filters and ordering.
+
+        Args:
+            filter_string (Optional[str], optional): A string specifying the conditions
+            that the model versions must meet.
+                It is used to filter the model versions. Examples of filter strings
+                include "name='my-model'"
+                or "name='my-model' and version='1'". If not provided, all model
+                versions are returned.
+                Defaults to None.
+            order_by (Optional[List[str]], optional): A list of strings specifying how to
+            order the model versions.
+                Examples of ordering criteria include "name ASC" or "version DESC".
+                If not provided, the model versions are ordered by their creation time in
+                descending order.
+                Defaults to None.
+
+        Returns:
+            List[dict]: A list of dictionaries, each representing a model version that meets
+            the filter and ordering criteria.
+                Each dictionary contains information about the model version, including
+                its name, version number, creation
+                time, run ID, and other metadata.
+
+        Raises:
+            Exception: If the plugin is not activated.
+        """
+        # Verify plugin activation
+        PluginManager().verify_activation(MlflowPlugin().section)
+
+        return self.mlflow.search_model_versions(
+            max_results=None,
+            filter_string=filter_string,
+            order_by=order_by,
+        )
```

### Comparing `cogflow-1.9.8/cogflow/plugin_config.py` & `cogflow-1.9.9/cogflow/plugin_config.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""
-This module defines constants for configuring Mlflow and AWS S3, as well as database credentials
- and MinIO settings.
-
-Attributes:
-    TRACKING_URI (str): The URI of the Mlflow tracking server. Used to specify where Mlflow logs and
-    artifacts should be stored.
-    S3_ENDPOINT_URL (str): The endpoint URL for the AWS S3 service. Needed for accessing and
-     storing data in an S3 bucket.
-    ACCESS_KEY_ID (str): The access key ID for AWS S3 authentication. Used in conjunction with
-     SECRET_ACCESS_KEY for secure access to S3.
-    SECRET_ACCESS_KEY (str): The secret access key for AWS S3 authentication. Paired with
-     ACCESS_KEY_ID for secure access to S3.
-    TIMER_IN_SEC (int): The interval in seconds for operations that require timing, such as
-     periodic checks or updates. Default is set to 10 seconds.
-    ML_TOOL (str): The name of the machine learning tool. Currently set to "mlflow" to
-     specify the use of the Mlflow framework.
-
-    ML_DB_USERNAME (str): Username for connecting to the machine learning database (ML_DB).
-     Essential for database access authentication.
-    ML_DB_PASSWORD (str): Password for connecting to the machine learning database (ML_DB).
-     Should be kept secure.
-    ML_DB_HOST (str): Host address for connecting to the machine learning database (ML_DB).
-    ML_DB_PORT (str): Port number for connecting to the machine learning database (ML_DB).
-    ML_DB_NAME (str): Name of the machine learning database (ML_DB).
-
-    Cogflow_DB_USERNAME (str): Username for connecting to the CogFlow database. Important for
-     authenticating access to the database.
-    Cogflow_DB_PASSWORD (str): Password for connecting to the CogFlow database.
-     Should be stored securely.
-    Cogflow_DB_HOST (str): Host address for connecting to the CogFlow database.
-    Cogflow_DB_PORT (str): Port number for connecting to the CogFlow database.
-    Cogflow_DB_NAME (str): Name of the CogFlow database.
-
-    MINIO_ENDPOINT_URL (str): The endpoint URL for the MinIO service, an alternative to AWS S3.
-     Used for accessing and storing data.
-    MINIO_ACCESS_KEY (str): The access key for MinIO authentication. Used with
-     MINIO_SECRET_ACCESS_KEY for secure access to MinIO.
-    MINIO_SECRET_ACCESS_KEY (str): The secret access key for MinIO authentication. Combined with
-     MINIO_ACCESS_KEY for secure access.
-"""
-
-COGFLOW_CONFIG_FILE_PATH = "COGFLOW_CONFIG_FILE_PATH"
-
-TRACKING_URI = "MLFLOW_TRACKING_URI"
-S3_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
-ACCESS_KEY_ID = "AWS_ACCESS_KEY_ID"
-SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
-TIMER_IN_SEC = 10
-ML_TOOL = "mlflow"
-
-ML_DB_USERNAME = "ML_DB_USERNAME"
-ML_DB_PASSWORD = "ML_DB_PASSWORD"
-ML_DB_HOST = "ML_DB_HOST"
-ML_DB_PORT = "ML_DB_PORT"
-ML_DB_NAME = "ML_DB_NAME"
-
-COGFLOW_DB_USERNAME = "DB_USER"
-COGFLOW_DB_PASSWORD = "DB_PASSWORD"
-COGFLOW_DB_HOST = "DB_HOST"
-COGFLOW_DB_PORT = "DB_PORT"
-COGFLOW_DB_NAME = "DB_NAME"
-
-MINIO_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
-MINIO_ACCESS_KEY = "AWS_ACCESS_KEY_ID"
-MINIO_SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
+"""
+This module defines constants for configuring Mlflow and AWS S3, as well as database credentials
+ and MinIO settings.
+
+Attributes:
+    TRACKING_URI (str): The URI of the Mlflow tracking server. Used to specify where Mlflow logs and
+    artifacts should be stored.
+    S3_ENDPOINT_URL (str): The endpoint URL for the AWS S3 service. Needed for accessing and
+     storing data in an S3 bucket.
+    ACCESS_KEY_ID (str): The access key ID for AWS S3 authentication. Used in conjunction with
+     SECRET_ACCESS_KEY for secure access to S3.
+    SECRET_ACCESS_KEY (str): The secret access key for AWS S3 authentication. Paired with
+     ACCESS_KEY_ID for secure access to S3.
+    TIMER_IN_SEC (int): The interval in seconds for operations that require timing, such as
+     periodic checks or updates. Default is set to 10 seconds.
+    ML_TOOL (str): The name of the machine learning tool. Currently set to "mlflow" to
+     specify the use of the Mlflow framework.
+
+    ML_DB_USERNAME (str): Username for connecting to the machine learning database (ML_DB).
+     Essential for database access authentication.
+    ML_DB_PASSWORD (str): Password for connecting to the machine learning database (ML_DB).
+     Should be kept secure.
+    ML_DB_HOST (str): Host address for connecting to the machine learning database (ML_DB).
+    ML_DB_PORT (str): Port number for connecting to the machine learning database (ML_DB).
+    ML_DB_NAME (str): Name of the machine learning database (ML_DB).
+
+    Cogflow_DB_USERNAME (str): Username for connecting to the CogFlow database. Important for
+     authenticating access to the database.
+    Cogflow_DB_PASSWORD (str): Password for connecting to the CogFlow database.
+     Should be stored securely.
+    Cogflow_DB_HOST (str): Host address for connecting to the CogFlow database.
+    Cogflow_DB_PORT (str): Port number for connecting to the CogFlow database.
+    Cogflow_DB_NAME (str): Name of the CogFlow database.
+
+    MINIO_ENDPOINT_URL (str): The endpoint URL for the MinIO service, an alternative to AWS S3.
+     Used for accessing and storing data.
+    MINIO_ACCESS_KEY (str): The access key for MinIO authentication. Used with
+     MINIO_SECRET_ACCESS_KEY for secure access to MinIO.
+    MINIO_SECRET_ACCESS_KEY (str): The secret access key for MinIO authentication. Combined with
+     MINIO_ACCESS_KEY for secure access.
+"""
+
+COGFLOW_CONFIG_FILE_PATH = "COGFLOW_CONFIG_FILE_PATH"
+
+TRACKING_URI = "MLFLOW_TRACKING_URI"
+S3_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
+ACCESS_KEY_ID = "AWS_ACCESS_KEY_ID"
+SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
+TIMER_IN_SEC = 10
+ML_TOOL = "mlflow"
+
+ML_DB_USERNAME = "ML_DB_USERNAME"
+ML_DB_PASSWORD = "ML_DB_PASSWORD"
+ML_DB_HOST = "ML_DB_HOST"
+ML_DB_PORT = "ML_DB_PORT"
+ML_DB_NAME = "ML_DB_NAME"
+
+COGFLOW_DB_USERNAME = "DB_USER"
+COGFLOW_DB_PASSWORD = "DB_PASSWORD"
+COGFLOW_DB_HOST = "DB_HOST"
+COGFLOW_DB_PORT = "DB_PORT"
+COGFLOW_DB_NAME = "DB_NAME"
+
+MINIO_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
+MINIO_ACCESS_KEY = "AWS_ACCESS_KEY_ID"
+MINIO_SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
```

### Comparing `cogflow-1.9.8/cogflow/plugin_status.py` & `cogflow-1.9.9/cogflow/plugin_status.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""
-Dictionary representing the status of different plugins.
-
-Keys:
-    - "MlflowPlugin": Represents the status of the MLflow plugin.
-    - "KubeflowPlugin": Represents the status of the Kubeflow plugin.
-    - "DatasetPlugin": Represents the status of the Dataset plugin.
-
-Values:
-    - "activated": Indicates that the corresponding plugin is activated and operational.
-    - "deactivated": Indicates that the corresponding plugin is deactivated and not operational.
-"""
-
-plugin_statuses = {
-    "MlflowPlugin": "deactivated",
-    "KubeflowPlugin": "deactivated",
-    "DatasetPlugin": "deactivated",
-}
+"""
+Dictionary representing the status of different plugins.
+
+Keys:
+    - "MlflowPlugin": Represents the status of the MLflow plugin.
+    - "KubeflowPlugin": Represents the status of the Kubeflow plugin.
+    - "DatasetPlugin": Represents the status of the Dataset plugin.
+
+Values:
+    - "activated": Indicates that the corresponding plugin is activated and operational.
+    - "deactivated": Indicates that the corresponding plugin is deactivated and not operational.
+"""
+
+plugin_statuses = {
+    "MlflowPlugin": "deactivated",
+    "KubeflowPlugin": "deactivated",
+    "DatasetPlugin": "deactivated",
+}
```

### Comparing `cogflow-1.9.8/cogflow.egg-info/SOURCES.txt` & `cogflow-1.9.9/cogflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.8/tests/test_dataset_plugin.py` & `cogflow-1.9.9/tests/test_dataset_plugin.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-import unittest
-from unittest.mock import patch, MagicMock
-
-import minio
-import requests
-
-from cogflow.cogflow.dataset_plugin import DatasetPlugin
-
-
-class TestDatasetPlugin(unittest.TestCase):
-    @patch("requests.get")
-    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.save_to_minio")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_query_endpoint_and_download_file_success(
-        self, mock_plugin_activation, mock_save_to_minio, mock_requests_get
-    ):
-        # Arrange
-        url = "http://dataset.com/dataset"
-        output_file = "dataset.csv"
-        bucket_name = "mlpipeline"
-        mock_response = MagicMock()
-        mock_response.status_code = 200
-        mock_response.content = b"Test dataset content"
-        mock_requests_get.return_value = mock_response
-
-        mock_minio_instance = MagicMock()
-        mock_save_to_minio.return_value = "http://dataset.com/dataset.csv"
-
-        # Act
-        success = DatasetPlugin().query_endpoint_and_download_file(
-            url=url, output_file=output_file, bucket_name=bucket_name
-        )
-
-        # Assert
-        self.assertTrue(success)
-        mock_save_to_minio.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("requests.get")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_query_endpoint_and_download_file_failure(
-        self, mock_plugin_activation, mock_requests_get
-    ):
-        # Arrange
-        dataset_plugin = DatasetPlugin()
-        url = "http://dataset.com/dataset"
-        bucket_name = "mlpipeline"
-        output_file = "dataset.csv"
-        mock_response = MagicMock()
-        mock_response.status_code = 404
-        mock_requests_get.return_value = mock_response
-
-        # Act & Assert
-        with self.assertRaises(Exception):
-            dataset_plugin.query_endpoint_and_download_file(
-                url, output_file, bucket_name
-            )
-        mock_plugin_activation.assert_called_once()
-
-    @patch("requests.get")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_request_exception_query_endpoint(
-        self, mock_plugin_activation, mock_requests_get
-    ):
-        # Arrange
-        dataset_plugin = DatasetPlugin()
-        url = "http://dataset.com/dataset"
-        bucket_name = "mlpipeline"
-        output_file = "dataset.csv"
-        # mock_response = MagicMock()
-        # mock_response.status_code = 404
-        # mock_requests_get.return_value = mock_response
-        mock_requests_get.side_effect = requests.exceptions.RequestException(
-            "Request failed"
-        )
-        with self.assertRaises(Exception):
-            dataset_plugin.query_endpoint_and_download_file(
-                url, output_file, bucket_name
-            )
-        mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
-    @patch("os.getenv")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_save_to_minio_success(
-        self, mock_plugin_activation, mock_getenv, mock_create_minio_client
-    ):
-
-        # Arrange
-        mock_minio_client = MagicMock()
-        mock_create_minio_client.return_value = mock_minio_client
-        mock_getenv.side_effect = lambda x: {
-            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
-            "AWS_ACCESS_KEY_ID": "minio",
-            "AWS_SECRET_ACCESS_KEY": "minio123",
-        }[x]
-
-        dataset_plugin = DatasetPlugin()
-        file_content = b"Test dataset content"
-        output_file = "dataset.csv"
-
-        mock_minio_instance = MagicMock()
-        mock_minio_instance.bucket_exists.return_value = True
-        mock_minio_instance.presigned_get_object.return_value = (
-            "http://dataset.com/dataset.csv"
-        )
-
-        # Act
-        dataset_plugin.save_to_minio(
-            file_content, output_file, bucket_name="mlpipeline"
-        )
-        # Assertions
-        mock_minio_client.bucket_exists.assert_called_once_with("mlpipeline")
-        mock_minio_client.presigned_get_object.assert_called_once()
-        mock_minio_client.put_object.assert_called_once()
-        mock_create_minio_client.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
-    @patch("os.getenv")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_minio_bucket_creation(
-        self,
-        mock_plugin_activation,
-        mock_getenv,
-        mock_create_minio_client,
-    ):
-        # Arrange
-        mock_minio_client = MagicMock()
-        mock_create_minio_client.return_value = mock_minio_client
-        mock_getenv.side_effect = lambda x: {
-            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
-            "AWS_ACCESS_KEY_ID": "minio",
-            "AWS_SECRET_ACCESS_KEY": "minio123",
-        }[x]
-
-        dataset_plugin = DatasetPlugin()
-        file_content = b"Test dataset content"
-        output_file = "dataset.csv"
-
-        mock_minio_client.bucket_exists.return_value = False
-        dataset_plugin.save_to_minio(
-            file_content, output_file, bucket_name="bucket_name"
-        )
-        mock_minio_client.make_bucket.assert_called_once()
-        mock_minio_client.make_bucket.assert_called_once_with("bucket_name")
-        mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
-    @patch("os.getenv")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_minio_bucket_creation_exception(
-        self,
-        mock_plugin_activation,
-        mock_getenv,
-        mock_create_minio_client,
-    ):
-        # Arrange
-        mock_minio_client = MagicMock()
-        mock_create_minio_client.return_value = mock_minio_client
-        mock_getenv.side_effect = lambda x: {
-            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
-            "AWS_ACCESS_KEY_ID": "minio",
-            "AWS_SECRET_ACCESS_KEY": "minio123",
-        }[x]
-
-        dataset_plugin = DatasetPlugin()
-        file_content = b"Test dataset content"
-        output_file = "dataset.csv"
-
-        mock_minio_client.bucket_exists.return_value = False
-        mock_minio_client.make_bucket.side_effect = Exception(
-            "Bucket Cannot be created"
-        )
-        with self.assertRaises(Exception):
-            dataset_plugin.save_to_minio(
-                file_content, output_file, bucket_name="bucket_name"
-            )
-        mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
-    @patch("os.getenv")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_save_to_exception(
-        self, mock_plugin_activation, mock_getenv, mock_create_minio_client
-    ):
-        # Arrange
-        mock_minio_client = MagicMock()
-        mock_create_minio_client.return_value = mock_minio_client
-        mock_getenv.side_effect = lambda x: {
-            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
-            "AWS_ACCESS_KEY_ID": "minio",
-            "AWS_SECRET_ACCESS_KEY": "minio123",
-        }[x]
-
-        dataset_plugin = DatasetPlugin()
-        file_content = b"Test dataset content"
-        output_file = "dataset.csv"
-
-        # mock_minio_client.bucket_exists.return_value = False
-        # mock_minio_client.make_bucket.side_effect = Exception("Bucket Cannot be created")
-        mock_minio_client.put_object.side_effect = Exception(
-            "Error while storing object"
-        )
-        with self.assertRaises(Exception):
-            dataset_plugin.save_to_minio(
-                file_content, output_file, bucket_name="bucket_name"
-            )
-        mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_delete_from_minio_success(
-        self, mock_plugin_activation, mock_create_minio_client
-    ):
-        # Arrange
-        dataset_plugin = DatasetPlugin()
-        object_name = "test_object"
-        bucket_name = "test_bucket"
-
-        mock_minio_instance = MagicMock()
-        mock_create_minio_client.return_value = mock_minio_instance
-        mock_minio_instance.stat_object.return_value = True  # Object exists
-
-        # Act
-        result = dataset_plugin.delete_from_minio(object_name, bucket_name)
-
-        # Assert
-        self.assertTrue(result)
-        mock_minio_instance.remove_object.assert_called_once_with(
-            bucket_name, object_name
-        )
-        mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_delete_from_minio_object_not_found(
-        self, mock_plugin_activation, mock_create_minio_client
-    ):
-        # Arrange
-        dataset_plugin = DatasetPlugin()
-        object_name = "test_object"
-        bucket_name = "test_bucket"
-
-        mock_minio_instance = MagicMock()
-        mock_create_minio_client.return_value = mock_minio_instance
-        mock_minio_instance.stat_object.return_value = False  # Object does not exist
-
-        # Act
-        result = dataset_plugin.delete_from_minio(object_name, bucket_name)
-
-        # Assert
-        self.assertFalse(result)
-        mock_minio_instance.remove_object.assert_not_called()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_delete_from_minio_exception(
-        self, mock_plugin_activation, mock_create_minio_client
-    ):
-        # Arrange
-        dataset_plugin = DatasetPlugin()
-        object_name = "test_object"
-        bucket_name = "test_bucket"
-
-        mock_minio_instance = MagicMock()
-        mock_create_minio_client.return_value = mock_minio_instance
-        mock_minio_instance.stat_object.side_effect = Exception("Test error")
-
-        # Act
-        result = dataset_plugin.delete_from_minio(object_name, bucket_name)
-
-        # Assert
-        self.assertFalse(result)
-        mock_minio_instance.remove_object.assert_not_called()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("os.getenv")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_create_minio_client(self, mock_plugin_activation, mock_getenv):
-        # Define test parameters
-        mock_getenv.side_effect = lambda x: {
-            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
-            "AWS_ACCESS_KEY_ID": "minio",
-            "AWS_SECRET_ACCESS_KEY": "minio123",
-        }[x]
-
-        # Create the MinioClient object
-        dataset_plugin = DatasetPlugin()
-        minio_client = dataset_plugin.create_minio_client()
-
-        # Assert that the MinioClient object is created correctly
-        self.assertIsInstance(minio_client, minio.api.Minio)
-        mock_plugin_activation.assert_called_once()
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+from unittest.mock import patch, MagicMock
+
+import minio
+import requests
+
+from cogflow.cogflow.dataset_plugin import DatasetPlugin
+
+
+class TestDatasetPlugin(unittest.TestCase):
+    @patch("requests.get")
+    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.save_to_minio")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_query_endpoint_and_download_file_success(
+        self, mock_plugin_activation, mock_save_to_minio, mock_requests_get
+    ):
+        # Arrange
+        url = "http://dataset.com/dataset"
+        output_file = "dataset.csv"
+        bucket_name = "mlpipeline"
+        mock_response = MagicMock()
+        mock_response.status_code = 200
+        mock_response.content = b"Test dataset content"
+        mock_requests_get.return_value = mock_response
+
+        mock_minio_instance = MagicMock()
+        mock_save_to_minio.return_value = "http://dataset.com/dataset.csv"
+
+        # Act
+        success = DatasetPlugin().query_endpoint_and_download_file(
+            url=url, output_file=output_file, bucket_name=bucket_name
+        )
+
+        # Assert
+        self.assertTrue(success)
+        mock_save_to_minio.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("requests.get")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_query_endpoint_and_download_file_failure(
+        self, mock_plugin_activation, mock_requests_get
+    ):
+        # Arrange
+        dataset_plugin = DatasetPlugin()
+        url = "http://dataset.com/dataset"
+        bucket_name = "mlpipeline"
+        output_file = "dataset.csv"
+        mock_response = MagicMock()
+        mock_response.status_code = 404
+        mock_requests_get.return_value = mock_response
+
+        # Act & Assert
+        with self.assertRaises(Exception):
+            dataset_plugin.query_endpoint_and_download_file(
+                url, output_file, bucket_name
+            )
+        mock_plugin_activation.assert_called_once()
+
+    @patch("requests.get")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_request_exception_query_endpoint(
+        self, mock_plugin_activation, mock_requests_get
+    ):
+        # Arrange
+        dataset_plugin = DatasetPlugin()
+        url = "http://dataset.com/dataset"
+        bucket_name = "mlpipeline"
+        output_file = "dataset.csv"
+        # mock_response = MagicMock()
+        # mock_response.status_code = 404
+        # mock_requests_get.return_value = mock_response
+        mock_requests_get.side_effect = requests.exceptions.RequestException(
+            "Request failed"
+        )
+        with self.assertRaises(Exception):
+            dataset_plugin.query_endpoint_and_download_file(
+                url, output_file, bucket_name
+            )
+        mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
+    @patch("os.getenv")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_save_to_minio_success(
+        self, mock_plugin_activation, mock_getenv, mock_create_minio_client
+    ):
+
+        # Arrange
+        mock_minio_client = MagicMock()
+        mock_create_minio_client.return_value = mock_minio_client
+        mock_getenv.side_effect = lambda x: {
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "AWS_ACCESS_KEY_ID": "minio",
+            "AWS_SECRET_ACCESS_KEY": "minio123",
+        }[x]
+
+        dataset_plugin = DatasetPlugin()
+        file_content = b"Test dataset content"
+        output_file = "dataset.csv"
+
+        mock_minio_instance = MagicMock()
+        mock_minio_instance.bucket_exists.return_value = True
+        mock_minio_instance.presigned_get_object.return_value = (
+            "http://dataset.com/dataset.csv"
+        )
+
+        # Act
+        dataset_plugin.save_to_minio(
+            file_content, output_file, bucket_name="mlpipeline"
+        )
+        # Assertions
+        mock_minio_client.bucket_exists.assert_called_once_with("mlpipeline")
+        mock_minio_client.presigned_get_object.assert_called_once()
+        mock_minio_client.put_object.assert_called_once()
+        mock_create_minio_client.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
+    @patch("os.getenv")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_minio_bucket_creation(
+        self,
+        mock_plugin_activation,
+        mock_getenv,
+        mock_create_minio_client,
+    ):
+        # Arrange
+        mock_minio_client = MagicMock()
+        mock_create_minio_client.return_value = mock_minio_client
+        mock_getenv.side_effect = lambda x: {
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "AWS_ACCESS_KEY_ID": "minio",
+            "AWS_SECRET_ACCESS_KEY": "minio123",
+        }[x]
+
+        dataset_plugin = DatasetPlugin()
+        file_content = b"Test dataset content"
+        output_file = "dataset.csv"
+
+        mock_minio_client.bucket_exists.return_value = False
+        dataset_plugin.save_to_minio(
+            file_content, output_file, bucket_name="bucket_name"
+        )
+        mock_minio_client.make_bucket.assert_called_once()
+        mock_minio_client.make_bucket.assert_called_once_with("bucket_name")
+        mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
+    @patch("os.getenv")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_minio_bucket_creation_exception(
+        self,
+        mock_plugin_activation,
+        mock_getenv,
+        mock_create_minio_client,
+    ):
+        # Arrange
+        mock_minio_client = MagicMock()
+        mock_create_minio_client.return_value = mock_minio_client
+        mock_getenv.side_effect = lambda x: {
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "AWS_ACCESS_KEY_ID": "minio",
+            "AWS_SECRET_ACCESS_KEY": "minio123",
+        }[x]
+
+        dataset_plugin = DatasetPlugin()
+        file_content = b"Test dataset content"
+        output_file = "dataset.csv"
+
+        mock_minio_client.bucket_exists.return_value = False
+        mock_minio_client.make_bucket.side_effect = Exception(
+            "Bucket Cannot be created"
+        )
+        with self.assertRaises(Exception):
+            dataset_plugin.save_to_minio(
+                file_content, output_file, bucket_name="bucket_name"
+            )
+        mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
+    @patch("os.getenv")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_save_to_exception(
+        self, mock_plugin_activation, mock_getenv, mock_create_minio_client
+    ):
+        # Arrange
+        mock_minio_client = MagicMock()
+        mock_create_minio_client.return_value = mock_minio_client
+        mock_getenv.side_effect = lambda x: {
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "AWS_ACCESS_KEY_ID": "minio",
+            "AWS_SECRET_ACCESS_KEY": "minio123",
+        }[x]
+
+        dataset_plugin = DatasetPlugin()
+        file_content = b"Test dataset content"
+        output_file = "dataset.csv"
+
+        # mock_minio_client.bucket_exists.return_value = False
+        # mock_minio_client.make_bucket.side_effect = Exception("Bucket Cannot be created")
+        mock_minio_client.put_object.side_effect = Exception(
+            "Error while storing object"
+        )
+        with self.assertRaises(Exception):
+            dataset_plugin.save_to_minio(
+                file_content, output_file, bucket_name="bucket_name"
+            )
+        mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_delete_from_minio_success(
+        self, mock_plugin_activation, mock_create_minio_client
+    ):
+        # Arrange
+        dataset_plugin = DatasetPlugin()
+        object_name = "test_object"
+        bucket_name = "test_bucket"
+
+        mock_minio_instance = MagicMock()
+        mock_create_minio_client.return_value = mock_minio_instance
+        mock_minio_instance.stat_object.return_value = True  # Object exists
+
+        # Act
+        result = dataset_plugin.delete_from_minio(object_name, bucket_name)
+
+        # Assert
+        self.assertTrue(result)
+        mock_minio_instance.remove_object.assert_called_once_with(
+            bucket_name, object_name
+        )
+        mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_delete_from_minio_object_not_found(
+        self, mock_plugin_activation, mock_create_minio_client
+    ):
+        # Arrange
+        dataset_plugin = DatasetPlugin()
+        object_name = "test_object"
+        bucket_name = "test_bucket"
+
+        mock_minio_instance = MagicMock()
+        mock_create_minio_client.return_value = mock_minio_instance
+        mock_minio_instance.stat_object.return_value = False  # Object does not exist
+
+        # Act
+        result = dataset_plugin.delete_from_minio(object_name, bucket_name)
+
+        # Assert
+        self.assertFalse(result)
+        mock_minio_instance.remove_object.assert_not_called()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.dataset_plugin.DatasetPlugin.create_minio_client")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_delete_from_minio_exception(
+        self, mock_plugin_activation, mock_create_minio_client
+    ):
+        # Arrange
+        dataset_plugin = DatasetPlugin()
+        object_name = "test_object"
+        bucket_name = "test_bucket"
+
+        mock_minio_instance = MagicMock()
+        mock_create_minio_client.return_value = mock_minio_instance
+        mock_minio_instance.stat_object.side_effect = Exception("Test error")
+
+        # Act
+        result = dataset_plugin.delete_from_minio(object_name, bucket_name)
+
+        # Assert
+        self.assertFalse(result)
+        mock_minio_instance.remove_object.assert_not_called()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("os.getenv")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_create_minio_client(self, mock_plugin_activation, mock_getenv):
+        # Define test parameters
+        mock_getenv.side_effect = lambda x: {
+            "MLFLOW_S3_ENDPOINT_URL": "localhost:9000",
+            "AWS_ACCESS_KEY_ID": "minio",
+            "AWS_SECRET_ACCESS_KEY": "minio123",
+        }[x]
+
+        # Create the MinioClient object
+        dataset_plugin = DatasetPlugin()
+        minio_client = dataset_plugin.create_minio_client()
+
+        # Assert that the MinioClient object is created correctly
+        self.assertIsInstance(minio_client, minio.api.Minio)
+        mock_plugin_activation.assert_called_once()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `cogflow-1.9.8/tests/test_mlflowplugin.py` & `cogflow-1.9.9/tests/test_mlflowplugin.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,488 +1,488 @@
-"""
-    Test module for cases related to mlflow_plugin
-"""
-
-import unittest
-from unittest.mock import patch, MagicMock
-import mlflow
-from mlflow.exceptions import MlflowException
-
-import cogflow.cogflow.pluginmanager
-from cogflow.cogflow.mlflowplugin import MlflowPlugin
-
-
-class TestMlflowPlugin(unittest.TestCase):
-    """
-    Test Class for cases related to mlflow_plugin
-    """
-
-    def setUp(self):
-        """
-            Initial setup
-        :return:
-        """
-        self.mlflow_plugin = MlflowPlugin()
-
-    @patch("mlflow.get_artifact_uri")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_get_artifact_uri_with_run_id(
-        self, mock_plugin_activation, mock_get_artifact_uri
-    ):
-        """
-            test for get_artifact_uri_with_run_id
-        :param mock_get_artifact_uri:
-        :return:
-        """
-        # Mocking the mlflow get_artifact_uri method to return a specific URI
-        mock_get_artifact_uri.return_value = "s3://your-bucket/artifacts/123"
-
-        result = self.mlflow_plugin.get_artifact_uri("123")
-
-        # Asserting that the mock method was called with the correct argument
-        mock_get_artifact_uri.assert_called_once_with("123")
-
-        # Asserting that the method returned the expected artifact URI
-        self.assertEqual(result, "s3://your-bucket/artifacts/123")
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.set_experiment")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_set_experiment(self, mock_plugin_activation, mock_set_experiment):
-        """
-            test for set_experiment
-        :param mock_set_experiment:
-        :return:
-        """
-        # Mocking the mlflow set_experiment method to raise an exception
-        mock_set_experiment.side_effect = MlflowException("Failed to set experiment")
-
-        with self.assertRaises(MlflowException):
-            self.mlflow_plugin.set_experiment("experiment_name")
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.set_tracking_uri")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_set_tracking_uri(self, mock_plugin_activation, mock_client):
-        """
-            test for set_tracking_uri
-        :param mock_client:
-        :return:
-        """
-        self.mlflow_plugin.set_tracking_uri("your_tracking_uri")
-
-        mock_client.assert_called_once_with("your_tracking_uri")
-        mock_plugin_activation.assert_called_once()
-
-    def test_version(self):
-        """
-            test for version
-        :return:
-        """
-        version = self.mlflow_plugin.version()
-
-        # Assert that the result matches the mocked version
-        self.assertEqual(version, "2.10.2")
-
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_is_alive(self, mock_plugin_activation):
-        """
-            test for is_alive
-        :return:
-        """
-        # Mock the requests.get function to simulate response
-        with patch("requests.get") as mock_get:
-            mock_response = MagicMock()
-            mock_response.status_code = 200  # Assuming Mlflow UI is accessible
-            mock_response.text = "OK"  # Mock response message
-            mock_get.return_value = mock_response
-
-            mlflow_plugin = MlflowPlugin()  # Create an instance of MlflowPlugin
-
-            status_code, message = mlflow_plugin.is_alive()
-
-            self.assertEqual(status_code, 200)  # Check if status code is 200
-            self.assertEqual(message, "OK")  # Check if response message is "OK"
-            mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_is_alive_request_not_success(self, mock_plugin_activation):
-        """
-            test when there is request not successful in is_alive method
-        :return:
-        """
-        # Mock the requests.get function to simulate response
-        with patch("requests.get") as mock_get:
-            mock_response = MagicMock()
-            mock_response.status_code = 404  # Assuming Mlflow UI is not-accessible
-            mock_response.text = "NOT-FOUND"  # Mock response message
-            mock_get.return_value = mock_response
-
-            mlflow_plugin = MlflowPlugin()  # Create an instance of MlflowPlugin
-
-            status_code, message = mlflow_plugin.is_alive()
-
-            self.assertEqual(status_code, 404)
-            self.assertEqual(message, "NOT-FOUND")
-            mock_plugin_activation.assert_called_once()
-
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_is_alive_request_exception(self, mock_plugin_activation):
-        """
-            test when there is exception occured in is_alive method
-        :return:
-        """
-        # Mock the requests.get function to simulate response
-        with patch("requests.get") as mock_get:
-            mock_get.side_effect = Exception("An error occurred .")
-
-            mlflow_plugin = MlflowPlugin()  # Create an instance of MlflowPlugin
-            with self.assertRaises(Exception):
-                status_code, message = mlflow_plugin.is_alive()
-            mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.tracking.client.MlflowClient.create_model_version")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_create_model_version(self, mock_plugin_activation, mock_client):
-        """
-            test for create_model_version
-        :param mock_client:
-        :return:
-        """
-        mock_client.side_effect = MlflowException("Error occured")
-        # # Call the method under test and expect it to raise an MlflowException
-        with self.assertRaises(MlflowException):
-            result = self.mlflow_plugin.create_model_version("model_name", "source")
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.tracking.client.MlflowClient")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_create_registered_model_exception(
-        self, mock_plugin_activation, mock_client
-    ):
-        """
-            test case when exception occurs in create_registered_model
-        :param mock_client:
-        :return:
-        """
-        # Define the exception to be raised
-        exception_to_raise = MlflowException("API request failed")
-
-        # Mocking the client method to raise the exception
-        mock_client.return_value.create_registered_model.side_effect = (
-            exception_to_raise
-        )
-
-        self.mlflow_plugin.create_registered_model("model_name_4")
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.tracking.client.MlflowClient.create_registered_model")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_create_registered_model(self, mock_plugin_activation, mock_client):
-        """
-            test case for create_registered_model
-        :param mock_client:
-        :return:
-        """
-        self.mlflow_plugin.create_registered_model("model_name")
-        mock_client.assert_called_once_with("model_name")
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.register_model")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_register_model(self, mock_plugin_activation, mock_register_model):
-        """
-            test case for register_model
-        :param mock_register_model:
-        :return:
-        """
-        # Define inputs
-        model = MagicMock()
-        model_uri = "my_model_uri"
-        self.mlflow_plugin.register_model(model, model_uri)
-        mock_register_model.assert_called_once_with(model, model_uri)
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.sklearn.load_model")
-    @patch("mlflow.utils.rest_utils.http_request")
-    def test_load_model_exception(self, mock_http_request, mock_load_model):
-        """
-            test for exception in load_model
-        :param mock_http_request:
-        :param mock_load_model:
-        :return:
-        """
-        # Define inputs
-        model_name = "my_model"
-        model_version = 1
-        expected_model = MagicMock()
-        mock_load_model.return_value = expected_model
-
-        # Mocking the HTTP request to raise MlflowException
-        mock_http_request.side_effect = MlflowException(
-            "API request failed with exception HTTPConnectionPool: "
-            "Max retries exceeded with url: http://127.0.0.1:5001"
-        )
-        try:
-            mock_load_model.assert_not_called()
-        except MlflowException:
-            with self.assertRaises(MlflowException):
-                loaded_model = self.mlflow_plugin.load_model(model_name, model_version)
-
-    @patch("cogflow.cogflow.mlflowplugin.MlflowPlugin.load_model")
-    def test_load_model(self, mock_load_model):
-        """
-        Test load_model method in mlflow_plugin.
-        """
-        # Define inputs
-        model_name = "tracking-quickstart"
-        model_version = 1
-        expected_model = MagicMock()
-
-        # Set the return value of the mocked load_model function
-        mock_load_model.return_value = expected_model
-
-        # Call the load_model method
-        result = self.mlflow_plugin.load_model(model_name, model_version)
-
-        # Verify that the result is equal to the expected model
-        self.assertEqual(result, expected_model)
-
-    @patch("mlflow.autolog")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_autolog(self, mock_plugin_activation, mock_autolog):
-        """
-            test for autolog
-        :param mock_autolog:
-        :return:
-        """
-        # Call the method under test
-        self.mlflow_plugin.autolog()
-
-        # Assert that autolog was called
-        mock_autolog.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.tracking.client.MlflowClient.delete_registered_model")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_delete_registered_model(
-        self, mock_plugin_activation, mock_delete_registered_model
-    ):
-        """
-            test for delete_registered_model
-        :param mock_delete_registered_model:
-        :return:
-        """
-        # Mock successful deletion
-        model_name = "test_model"
-        mock_delete_registered_model.return_value = True
-
-        # Call the method under test
-        result = self.mlflow_plugin.delete_registered_model(model_name)
-
-        # Assert that the method returns True
-        self.assertTrue(result)
-
-        # Assert that delete_registered_model was called with the correct argument
-        mock_delete_registered_model.assert_called_once_with(model_name)
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.search_registered_models")
-    def test_search_registered_models_exception(self, mock_search_registered_models):
-        """
-            test for exception occurs when search for registered model
-        :param mock_search_registered_models:
-        :return:
-        """
-        # Mock any other unexpected exception
-        mock_search_registered_models.side_effect = MlflowException(
-            "API request failed with exception HTTPConnectionPool: "
-            "Max retries exceeded with url: http://127.0.0.1:5001"
-        )
-        # Assert that the method raises the expected exception
-        try:
-            mock_search_registered_models.assert_not_called()
-        except MlflowException:
-            with self.assertRaises(MlflowException):
-                self.mlflow_plugin.search_registered_models()
-
-    @patch("mlflow.tracking.client.MlflowClient.search_registered_models")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_search_registered_models(
-        self, mock_plugin_activation, mock_search_registered_models
-    ):
-        """
-            test for search_registered_model
-        :param mock_search_registered_models:
-        :return:
-        """
-        mock_search_registered_models.return_value = None
-        # Call the method under test
-        self.mlflow_plugin.search_registered_models()
-
-        # Assert that autolog was called
-        mock_search_registered_models.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.start_run")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_start_run_with_experiment_and_run_name(
-        self, mock_plugin_activation, mock_start_run
-    ):
-        """
-            test for start_run_with_experiment with run_name
-        :param mock_start_run:
-        :return:
-        """
-        experiment_name = "test_experiment"
-        run_name = "test_run"
-        self.mlflow_plugin.start_run(run_name=run_name)
-        # Assert that start_run was called with the correct arguments
-        mock_start_run.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.end_run")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_end_run(self, mock_plugin_activation, mock_end_run):
-        """
-            test for end_run
-        :param mock_end_run:
-        :return:
-        """
-        # Call the method under test
-        self.mlflow_plugin.end_run()
-        # Assert that end_run was called
-        mock_end_run.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.log_param")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_log_param(self, mock_plugin_activation, mock_log_param):
-        """
-            test for log_param
-        :param mock_log_param:
-        :return:
-        """
-        # Define inputs
-        run = MagicMock()
-        params = {"param1": 10, "param2": "value"}
-
-        # Call the method under test
-        self.mlflow_plugin.log_param(run, params)
-
-        # Assert that log_param was called with the correct arguments
-        mock_log_param.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.log_metric")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_log_metric(self, mock_plugin_activation, mock_log_metric):
-        """
-            test for log_metric
-        :param mock_log_metric:
-        :return:
-        """
-        # Define inputs
-        run = MagicMock()
-        metrics = {"accuracy": 0.85, "loss": 0.1}
-
-        # Call the method under test
-        self.mlflow_plugin.log_metric(run, metrics)
-
-        # Assert that log_metric was called with the correct arguments
-        mock_log_metric.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.sklearn.log_model")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_log_model(self, mock_plugin_activation, mock_log_model):
-        """
-            test for log_model
-        :param mock_log_model:
-        :return:
-        """
-        # Define inputs
-        sk_model = MagicMock()
-        artifact_path = "model"
-        # Define any other necessary inputs for the log_model method
-
-        # Call the method under test
-        result = self.mlflow_plugin.log_model(
-            sk_model=sk_model, artifact_path=artifact_path
-        )
-        # Assert that log_model was called with the correct arguments
-        mock_log_model.assert_called_once()
-        mock_plugin_activation.assert_called_once()
-
-    @patch("mlflow.sklearn.log_model")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_log_model_exception(self, mock_plugin_activation, mock_log_model):
-        """
-            test log_model when exception occurs
-        :param mock_log_model:
-        :return:
-        """
-        # Define inputs
-        sk_model = MagicMock()
-        artifact_path = "model"
-        # Define any other necessary inputs for the log_model method
-
-        # Set up the side effect to raise MlflowException
-        mock_log_model.side_effect = MlflowException(
-            "API request failed with exception HTTPConnectionPool: "
-            "Max retries exceeded with url: http://127.0.0.1:5001"
-        )
-
-        # Call the method under test and assert that it raises an exception
-        with self.assertRaises(MlflowException):
-            self.mlflow_plugin.log_model(sk_model=sk_model, artifact_path=artifact_path)
-        mock_plugin_activation.assert_called_once()
-
-    def test_log_metric_successful(self):
-        # Use patch to mock PluginManager().verify_activation
-        with patch.object(
-            cogflow.cogflow.pluginmanager.PluginManager, "verify_activation"
-        ) as mock_verify_activation:
-            # Use patch to mock mlflow.log_metric
-            with patch("mlflow.log_metric") as mock_log_metric:
-                # Configure the mock's behavior
-                mock_verify_activation.return_value = None  # Plugin activated
-
-                # Call the method with valid arguments
-                key = "accuracy"
-                value = 0.95
-                step = 1
-                synchronous = True
-                timestamp = None
-                run_id = "run1"
-
-                # Invoke the log_metric method
-                self.mlflow_plugin.log_metric(
-                    key,
-                    value,
-                    step=step,
-                    synchronous=synchronous,
-                    timestamp=timestamp,
-                    run_id=run_id,
-                )
-
-                # Assert that log_metric was called with the expected arguments
-                mock_log_metric.assert_called_once()
-
-    @patch("mlflow.search_model_versions")
-    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
-    def test_search_model_versions(
-        self, mock_verify_activation, mock_search_model_versions
-    ):
-        filter_string = "name='custom_model'"
-        order_by = ["1"]
-
-        # Call the method being tested
-        self.mlflow_plugin.search_model_versions(
-            filter_string=filter_string, order_by=order_by
-        )
-        mock_search_model_versions.assert_called_once()
-        mock_verify_activation.assert_called_once()
-
-
-if __name__ == "__main__":
-    unittest.main()
+"""
+    Test module for cases related to mlflow_plugin
+"""
+
+import unittest
+from unittest.mock import patch, MagicMock
+import mlflow
+from mlflow.exceptions import MlflowException
+
+import cogflow.cogflow.pluginmanager
+from cogflow.cogflow.mlflowplugin import MlflowPlugin
+
+
+class TestMlflowPlugin(unittest.TestCase):
+    """
+    Test Class for cases related to mlflow_plugin
+    """
+
+    def setUp(self):
+        """
+            Initial setup
+        :return:
+        """
+        self.mlflow_plugin = MlflowPlugin()
+
+    @patch("mlflow.get_artifact_uri")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_get_artifact_uri_with_run_id(
+        self, mock_plugin_activation, mock_get_artifact_uri
+    ):
+        """
+            test for get_artifact_uri_with_run_id
+        :param mock_get_artifact_uri:
+        :return:
+        """
+        # Mocking the mlflow get_artifact_uri method to return a specific URI
+        mock_get_artifact_uri.return_value = "s3://your-bucket/artifacts/123"
+
+        result = self.mlflow_plugin.get_artifact_uri("123")
+
+        # Asserting that the mock method was called with the correct argument
+        mock_get_artifact_uri.assert_called_once_with("123")
+
+        # Asserting that the method returned the expected artifact URI
+        self.assertEqual(result, "s3://your-bucket/artifacts/123")
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.set_experiment")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_set_experiment(self, mock_plugin_activation, mock_set_experiment):
+        """
+            test for set_experiment
+        :param mock_set_experiment:
+        :return:
+        """
+        # Mocking the mlflow set_experiment method to raise an exception
+        mock_set_experiment.side_effect = MlflowException("Failed to set experiment")
+
+        with self.assertRaises(MlflowException):
+            self.mlflow_plugin.set_experiment("experiment_name")
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.set_tracking_uri")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_set_tracking_uri(self, mock_plugin_activation, mock_client):
+        """
+            test for set_tracking_uri
+        :param mock_client:
+        :return:
+        """
+        self.mlflow_plugin.set_tracking_uri("your_tracking_uri")
+
+        mock_client.assert_called_once_with("your_tracking_uri")
+        mock_plugin_activation.assert_called_once()
+
+    def test_version(self):
+        """
+            test for version
+        :return:
+        """
+        version = self.mlflow_plugin.version()
+
+        # Assert that the result matches the mocked version
+        self.assertEqual(version, "2.10.2")
+
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_is_alive(self, mock_plugin_activation):
+        """
+            test for is_alive
+        :return:
+        """
+        # Mock the requests.get function to simulate response
+        with patch("requests.get") as mock_get:
+            mock_response = MagicMock()
+            mock_response.status_code = 200  # Assuming Mlflow UI is accessible
+            mock_response.text = "OK"  # Mock response message
+            mock_get.return_value = mock_response
+
+            mlflow_plugin = MlflowPlugin()  # Create an instance of MlflowPlugin
+
+            status_code, message = mlflow_plugin.is_alive()
+
+            self.assertEqual(status_code, 200)  # Check if status code is 200
+            self.assertEqual(message, "OK")  # Check if response message is "OK"
+            mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_is_alive_request_not_success(self, mock_plugin_activation):
+        """
+            test when there is request not successful in is_alive method
+        :return:
+        """
+        # Mock the requests.get function to simulate response
+        with patch("requests.get") as mock_get:
+            mock_response = MagicMock()
+            mock_response.status_code = 404  # Assuming Mlflow UI is not-accessible
+            mock_response.text = "NOT-FOUND"  # Mock response message
+            mock_get.return_value = mock_response
+
+            mlflow_plugin = MlflowPlugin()  # Create an instance of MlflowPlugin
+
+            status_code, message = mlflow_plugin.is_alive()
+
+            self.assertEqual(status_code, 404)
+            self.assertEqual(message, "NOT-FOUND")
+            mock_plugin_activation.assert_called_once()
+
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_is_alive_request_exception(self, mock_plugin_activation):
+        """
+            test when there is exception occured in is_alive method
+        :return:
+        """
+        # Mock the requests.get function to simulate response
+        with patch("requests.get") as mock_get:
+            mock_get.side_effect = Exception("An error occurred .")
+
+            mlflow_plugin = MlflowPlugin()  # Create an instance of MlflowPlugin
+            with self.assertRaises(Exception):
+                status_code, message = mlflow_plugin.is_alive()
+            mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.tracking.client.MlflowClient.create_model_version")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_create_model_version(self, mock_plugin_activation, mock_client):
+        """
+            test for create_model_version
+        :param mock_client:
+        :return:
+        """
+        mock_client.side_effect = MlflowException("Error occured")
+        # # Call the method under test and expect it to raise an MlflowException
+        with self.assertRaises(MlflowException):
+            result = self.mlflow_plugin.create_model_version("model_name", "source")
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.tracking.client.MlflowClient")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_create_registered_model_exception(
+        self, mock_plugin_activation, mock_client
+    ):
+        """
+            test case when exception occurs in create_registered_model
+        :param mock_client:
+        :return:
+        """
+        # Define the exception to be raised
+        exception_to_raise = MlflowException("API request failed")
+
+        # Mocking the client method to raise the exception
+        mock_client.return_value.create_registered_model.side_effect = (
+            exception_to_raise
+        )
+
+        self.mlflow_plugin.create_registered_model("model_name_4")
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.tracking.client.MlflowClient.create_registered_model")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_create_registered_model(self, mock_plugin_activation, mock_client):
+        """
+            test case for create_registered_model
+        :param mock_client:
+        :return:
+        """
+        self.mlflow_plugin.create_registered_model("model_name")
+        mock_client.assert_called_once_with("model_name")
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.register_model")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_register_model(self, mock_plugin_activation, mock_register_model):
+        """
+            test case for register_model
+        :param mock_register_model:
+        :return:
+        """
+        # Define inputs
+        model = MagicMock()
+        model_uri = "my_model_uri"
+        self.mlflow_plugin.register_model(model, model_uri)
+        mock_register_model.assert_called_once_with(model, model_uri)
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.sklearn.load_model")
+    @patch("mlflow.utils.rest_utils.http_request")
+    def test_load_model_exception(self, mock_http_request, mock_load_model):
+        """
+            test for exception in load_model
+        :param mock_http_request:
+        :param mock_load_model:
+        :return:
+        """
+        # Define inputs
+        model_name = "my_model"
+        model_version = 1
+        expected_model = MagicMock()
+        mock_load_model.return_value = expected_model
+
+        # Mocking the HTTP request to raise MlflowException
+        mock_http_request.side_effect = MlflowException(
+            "API request failed with exception HTTPConnectionPool: "
+            "Max retries exceeded with url: http://127.0.0.1:5001"
+        )
+        try:
+            mock_load_model.assert_not_called()
+        except MlflowException:
+            with self.assertRaises(MlflowException):
+                loaded_model = self.mlflow_plugin.load_model(model_name, model_version)
+
+    @patch("cogflow.cogflow.mlflowplugin.MlflowPlugin.load_model")
+    def test_load_model(self, mock_load_model):
+        """
+        Test load_model method in mlflow_plugin.
+        """
+        # Define inputs
+        model_name = "tracking-quickstart"
+        model_version = 1
+        expected_model = MagicMock()
+
+        # Set the return value of the mocked load_model function
+        mock_load_model.return_value = expected_model
+
+        # Call the load_model method
+        result = self.mlflow_plugin.load_model(model_name, model_version)
+
+        # Verify that the result is equal to the expected model
+        self.assertEqual(result, expected_model)
+
+    @patch("mlflow.autolog")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_autolog(self, mock_plugin_activation, mock_autolog):
+        """
+            test for autolog
+        :param mock_autolog:
+        :return:
+        """
+        # Call the method under test
+        self.mlflow_plugin.autolog()
+
+        # Assert that autolog was called
+        mock_autolog.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.tracking.client.MlflowClient.delete_registered_model")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_delete_registered_model(
+        self, mock_plugin_activation, mock_delete_registered_model
+    ):
+        """
+            test for delete_registered_model
+        :param mock_delete_registered_model:
+        :return:
+        """
+        # Mock successful deletion
+        model_name = "test_model"
+        mock_delete_registered_model.return_value = True
+
+        # Call the method under test
+        result = self.mlflow_plugin.delete_registered_model(model_name)
+
+        # Assert that the method returns True
+        self.assertTrue(result)
+
+        # Assert that delete_registered_model was called with the correct argument
+        mock_delete_registered_model.assert_called_once_with(model_name)
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.search_registered_models")
+    def test_search_registered_models_exception(self, mock_search_registered_models):
+        """
+            test for exception occurs when search for registered model
+        :param mock_search_registered_models:
+        :return:
+        """
+        # Mock any other unexpected exception
+        mock_search_registered_models.side_effect = MlflowException(
+            "API request failed with exception HTTPConnectionPool: "
+            "Max retries exceeded with url: http://127.0.0.1:5001"
+        )
+        # Assert that the method raises the expected exception
+        try:
+            mock_search_registered_models.assert_not_called()
+        except MlflowException:
+            with self.assertRaises(MlflowException):
+                self.mlflow_plugin.search_registered_models()
+
+    @patch("mlflow.tracking.client.MlflowClient.search_registered_models")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_search_registered_models(
+        self, mock_plugin_activation, mock_search_registered_models
+    ):
+        """
+            test for search_registered_model
+        :param mock_search_registered_models:
+        :return:
+        """
+        mock_search_registered_models.return_value = None
+        # Call the method under test
+        self.mlflow_plugin.search_registered_models()
+
+        # Assert that autolog was called
+        mock_search_registered_models.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.start_run")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_start_run_with_experiment_and_run_name(
+        self, mock_plugin_activation, mock_start_run
+    ):
+        """
+            test for start_run_with_experiment with run_name
+        :param mock_start_run:
+        :return:
+        """
+        experiment_name = "test_experiment"
+        run_name = "test_run"
+        self.mlflow_plugin.start_run(run_name=run_name)
+        # Assert that start_run was called with the correct arguments
+        mock_start_run.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.end_run")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_end_run(self, mock_plugin_activation, mock_end_run):
+        """
+            test for end_run
+        :param mock_end_run:
+        :return:
+        """
+        # Call the method under test
+        self.mlflow_plugin.end_run()
+        # Assert that end_run was called
+        mock_end_run.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.log_param")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_log_param(self, mock_plugin_activation, mock_log_param):
+        """
+            test for log_param
+        :param mock_log_param:
+        :return:
+        """
+        # Define inputs
+        run = MagicMock()
+        params = {"param1": 10, "param2": "value"}
+
+        # Call the method under test
+        self.mlflow_plugin.log_param(run, params)
+
+        # Assert that log_param was called with the correct arguments
+        mock_log_param.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.log_metric")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_log_metric(self, mock_plugin_activation, mock_log_metric):
+        """
+            test for log_metric
+        :param mock_log_metric:
+        :return:
+        """
+        # Define inputs
+        run = MagicMock()
+        metrics = {"accuracy": 0.85, "loss": 0.1}
+
+        # Call the method under test
+        self.mlflow_plugin.log_metric(run, metrics)
+
+        # Assert that log_metric was called with the correct arguments
+        mock_log_metric.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.sklearn.log_model")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_log_model(self, mock_plugin_activation, mock_log_model):
+        """
+            test for log_model
+        :param mock_log_model:
+        :return:
+        """
+        # Define inputs
+        sk_model = MagicMock()
+        artifact_path = "model"
+        # Define any other necessary inputs for the log_model method
+
+        # Call the method under test
+        result = self.mlflow_plugin.log_model(
+            sk_model=sk_model, artifact_path=artifact_path
+        )
+        # Assert that log_model was called with the correct arguments
+        mock_log_model.assert_called_once()
+        mock_plugin_activation.assert_called_once()
+
+    @patch("mlflow.sklearn.log_model")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_log_model_exception(self, mock_plugin_activation, mock_log_model):
+        """
+            test log_model when exception occurs
+        :param mock_log_model:
+        :return:
+        """
+        # Define inputs
+        sk_model = MagicMock()
+        artifact_path = "model"
+        # Define any other necessary inputs for the log_model method
+
+        # Set up the side effect to raise MlflowException
+        mock_log_model.side_effect = MlflowException(
+            "API request failed with exception HTTPConnectionPool: "
+            "Max retries exceeded with url: http://127.0.0.1:5001"
+        )
+
+        # Call the method under test and assert that it raises an exception
+        with self.assertRaises(MlflowException):
+            self.mlflow_plugin.log_model(sk_model=sk_model, artifact_path=artifact_path)
+        mock_plugin_activation.assert_called_once()
+
+    def test_log_metric_successful(self):
+        # Use patch to mock PluginManager().verify_activation
+        with patch.object(
+            cogflow.cogflow.pluginmanager.PluginManager, "verify_activation"
+        ) as mock_verify_activation:
+            # Use patch to mock mlflow.log_metric
+            with patch("mlflow.log_metric") as mock_log_metric:
+                # Configure the mock's behavior
+                mock_verify_activation.return_value = None  # Plugin activated
+
+                # Call the method with valid arguments
+                key = "accuracy"
+                value = 0.95
+                step = 1
+                synchronous = True
+                timestamp = None
+                run_id = "run1"
+
+                # Invoke the log_metric method
+                self.mlflow_plugin.log_metric(
+                    key,
+                    value,
+                    step=step,
+                    synchronous=synchronous,
+                    timestamp=timestamp,
+                    run_id=run_id,
+                )
+
+                # Assert that log_metric was called with the expected arguments
+                mock_log_metric.assert_called_once()
+
+    @patch("mlflow.search_model_versions")
+    @patch("cogflow.cogflow.pluginmanager.PluginManager.verify_activation")
+    def test_search_model_versions(
+        self, mock_verify_activation, mock_search_model_versions
+    ):
+        filter_string = "name='custom_model'"
+        order_by = ["1"]
+
+        # Call the method being tested
+        self.mlflow_plugin.search_model_versions(
+            filter_string=filter_string, order_by=order_by
+        )
+        mock_search_model_versions.assert_called_once()
+        mock_verify_activation.assert_called_once()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `cogflow-1.9.8/tests/test_plugin_manager.py` & `cogflow-1.9.9/tests/test_plugin_manager.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-"""
-    This file contains unittest for PluginManager methods
-"""
-
-import os
-import unittest
-import configparser
-from unittest.mock import patch, mock_open, MagicMock
-from cogflow.cogflow import PluginManager
-
-
-class TestPluginManager(unittest.TestCase):
-    """
-    Test class for PluginManger
-    """
-
-    def setUp(self):
-        # Set up the file paths and sections to use in the test cases
-        self.config_file_path = os.path.join(
-            os.path.dirname(__file__), "cogflow_config.ini"
-        )
-        # self.config_file_path = "config.ini"
-        self.section = "mlflow_plugin"
-        self.key = "activation_key"
-
-        # Initialize the instance of the class containing the methods to test
-        self.instance = PluginManager()
-
-    def test_get_config_value_activation_status(self):
-        # Prepare a valid configuration file content with the key
-        config_content = """
-        [mlflow_plugin]
-        activation_key = True
-        """
-
-        # Mock open function to simulate reading the file
-        with patch("builtins.open", mock_open(read_data=self.config_file_path)):
-            # Mock configparser to control its behavior
-            with patch("configparser.ConfigParser") as mock_config:
-                # Configure the mock object to return desired values
-                mock_config_instance = mock_config.return_value
-                mock_config_instance.read.return_value = None
-                mock_config_instance.getboolean.return_value = True
-                print("**************", self.config_file_path)
-
-                # Call the method
-
-                with self.assertRaises(Exception) as context:
-                    self.instance.get_config_value(
-                        self.config_file_path, "mlflow_plugin"
-                    )
-
-                # Check that the expected error message is raised
-                expected_message = (
-                    "Section 'mlflow_plugin' not found in the configuration file. "
-                    "Please correct section name in configuration file."
-                )
-                self.assertIn(expected_message, str(context.exception))
-
-    def test_get_config_value_nonexistent_key(self):
-        # Prepare a valid configuration file content without the key
-        config_content = """
-        [mlflow_plugin]
-        other_key = some_value
-        """
-
-        # Mock open function to simulate reading the file
-        with patch("builtins.open", mock_open(read_data=config_content)):
-            # Mock configparser to control its behavior
-            with patch("configparser.ConfigParser") as mock_config:
-                # Configure the mock object to return desired values
-                mock_config_instance = mock_config.return_value
-                mock_config_instance.read.return_value = None
-                mock_config_instance.get.side_effect = configparser.NoOptionError(
-                    "key", self.section
-                )
-
-                # Call the method and expect a KeyError
-                with self.assertRaises(Exception) as cm:
-                    self.instance.get_config_value(
-                        self.config_file_path, self.section, self.key
-                    )
-                self.assertNotIn("Key 'activation_key' not found", str(cm.exception))
-
-    def test_verify_activation_plugin_active(self):
-        # Prepare a valid configuration file content with the key set to True
-        config_content = """
-        [mlflow_plugin]
-        activation_key = true
-        """
-
-        # Mock open function to simulate reading the file
-        with patch("builtins.open", mock_open(read_data=config_content)):
-            # Mock configparser to control its behavior
-            with patch("configparser.ConfigParser") as mock_config:
-                # Configure the mock object to return desired values
-                mock_config_instance = mock_config.return_value
-                mock_config_instance.read.return_value = None
-                mock_config_instance.getboolean.return_value = True
-
-                # Call the method
-                with self.assertRaises(Exception):
-                    self.instance.verify_activation(self.section)
-                # No exception expected if plugin is active
+"""
+    This file contains unittest for PluginManager methods
+"""
+
+import os
+import unittest
+import configparser
+from unittest.mock import patch, mock_open, MagicMock
+from cogflow.cogflow import PluginManager
+
+
+class TestPluginManager(unittest.TestCase):
+    """
+    Test class for PluginManger
+    """
+
+    def setUp(self):
+        # Set up the file paths and sections to use in the test cases
+        self.config_file_path = os.path.join(
+            os.path.dirname(__file__), "cogflow_config.ini"
+        )
+        # self.config_file_path = "config.ini"
+        self.section = "mlflow_plugin"
+        self.key = "activation_key"
+
+        # Initialize the instance of the class containing the methods to test
+        self.instance = PluginManager()
+
+    def test_get_config_value_activation_status(self):
+        # Prepare a valid configuration file content with the key
+        config_content = """
+        [mlflow_plugin]
+        activation_key = True
+        """
+
+        # Mock open function to simulate reading the file
+        with patch("builtins.open", mock_open(read_data=self.config_file_path)):
+            # Mock configparser to control its behavior
+            with patch("configparser.ConfigParser") as mock_config:
+                # Configure the mock object to return desired values
+                mock_config_instance = mock_config.return_value
+                mock_config_instance.read.return_value = None
+                mock_config_instance.getboolean.return_value = True
+                print("**************", self.config_file_path)
+
+                # Call the method
+
+                with self.assertRaises(Exception) as context:
+                    self.instance.get_config_value(
+                        self.config_file_path, "mlflow_plugin"
+                    )
+
+                # Check that the expected error message is raised
+                expected_message = (
+                    "Section 'mlflow_plugin' not found in the configuration file. "
+                    "Please correct section name in configuration file."
+                )
+                self.assertIn(expected_message, str(context.exception))
+
+    def test_get_config_value_nonexistent_key(self):
+        # Prepare a valid configuration file content without the key
+        config_content = """
+        [mlflow_plugin]
+        other_key = some_value
+        """
+
+        # Mock open function to simulate reading the file
+        with patch("builtins.open", mock_open(read_data=config_content)):
+            # Mock configparser to control its behavior
+            with patch("configparser.ConfigParser") as mock_config:
+                # Configure the mock object to return desired values
+                mock_config_instance = mock_config.return_value
+                mock_config_instance.read.return_value = None
+                mock_config_instance.get.side_effect = configparser.NoOptionError(
+                    "key", self.section
+                )
+
+                # Call the method and expect a KeyError
+                with self.assertRaises(Exception) as cm:
+                    self.instance.get_config_value(
+                        self.config_file_path, self.section, self.key
+                    )
+                self.assertNotIn("Key 'activation_key' not found", str(cm.exception))
+
+    def test_verify_activation_plugin_active(self):
+        # Prepare a valid configuration file content with the key set to True
+        config_content = """
+        [mlflow_plugin]
+        activation_key = true
+        """
+
+        # Mock open function to simulate reading the file
+        with patch("builtins.open", mock_open(read_data=config_content)):
+            # Mock configparser to control its behavior
+            with patch("configparser.ConfigParser") as mock_config:
+                # Configure the mock object to return desired values
+                mock_config_instance = mock_config.return_value
+                mock_config_instance.read.return_value = None
+                mock_config_instance.getboolean.return_value = True
+
+                # Call the method
+                with self.assertRaises(Exception):
+                    self.instance.verify_activation(self.section)
+                # No exception expected if plugin is active
```


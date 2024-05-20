# Comparing `tmp/acceldata_airflow_sdk-3.4.0.tar.gz` & `tmp/acceldata_airflow_sdk-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acceldata_airflow_sdk-3.4.0.tar", last modified: Wed May  8 11:07:31 2024, max compression
+gzip compressed data, was "acceldata_airflow_sdk-3.5.0.tar", last modified: Mon May 20 08:41:44 2024, max compression
```

## Comparing `acceldata_airflow_sdk-3.4.0.tar` & `acceldata_airflow_sdk-3.5.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.894420 acceldata_airflow_sdk-3.4.0/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      307 2024-05-08 11:01:16.000000 acceldata_airflow_sdk-3.4.0/CHANGELOG.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/LICENCE.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/MANIFEST.in
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23484 2024-05-08 11:07:31.894071 acceldata_airflow_sdk-3.4.0/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    22515 2024-05-08 11:01:16.000000 acceldata_airflow_sdk-3.4.0/README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/README.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.882429 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3065 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/dag.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.884568 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1100 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/handle_callback.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3935 2024-03-21 11:14:17.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/job.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4254 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/span.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1298 2024-05-08 11:01:16.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/initialiser.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.886524 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4229 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/execute_policy_operator.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6446 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/job_operator.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6143 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/span_operator.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     7017 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.887781 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2270 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/callback.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3477 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3812 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/torch_client.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.893601 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23484 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2029 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       82 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/requires.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       22 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.888012 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2323 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/README.md
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.888409 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/__init__.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.889415 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:28.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      867 2024-02-22 04:32:28.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     5955 2024-05-08 04:50:53.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/events_listener.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    18561 2024-05-08 04:50:53.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/utils.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1215 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener_plugin.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.889859 acceldata_airflow_sdk-3.4.0/docs/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.879725 acceldata_airflow_sdk-3.4.0/docs/_build/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.879796 acceldata_airflow_sdk-3.4.0/docs/_build/html/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.891320 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      492 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       96 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      858 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      720 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      707 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      623 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1950 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/conf.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.891511 acceldata_airflow_sdk-3.4.0/openlineage/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1050 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/airflow_local_settings.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.891693 acceldata_airflow_sdk-3.4.0/openlineage/config/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/config/__init__.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.892305 acceldata_airflow_sdk-3.4.0/openlineage/extractors/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/extractors/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3993 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/extractors/bigquery_insert_job_extractor.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6291 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/extractors/gcs_bigquery_extractor.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.892750 acceldata_airflow_sdk-3.4.0/openlineage/policy/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/policy/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4179 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/policy/config_helper.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.893195 acceldata_airflow_sdk-3.4.0/openlineage/tokenproviders/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/tokenproviders/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10427 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/tokenproviders/access_key_secret_token_provider.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-05-08 11:07:31.894482 acceldata_airflow_sdk-3.4.0/setup.cfg
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      842 2024-05-08 11:01:16.000000 acceldata_airflow_sdk-3.4.0/setup.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.515380 acceldata_airflow_sdk-3.5.0/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      124 2024-05-15 04:39:47.000000 acceldata_airflow_sdk-3.5.0/CHANGELOG.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/LICENCE.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/MANIFEST.in
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23302 2024-05-20 08:41:44.515099 acceldata_airflow_sdk-3.5.0/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    22515 2024-05-08 12:39:35.000000 acceldata_airflow_sdk-3.5.0/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/README.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.503293 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3065 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/dag.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.505346 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/decorators/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/decorators/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1100 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/decorators/handle_callback.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3935 2024-03-21 11:14:17.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/decorators/job.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4254 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/decorators/span.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1298 2024-05-08 12:39:35.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/initialiser.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.506831 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4229 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/execute_policy_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6446 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/job_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6143 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/span_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     7017 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.508034 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/utils/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/utils/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2270 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/utils/callback.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3477 2024-05-15 10:32:15.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/utils/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3812 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/utils/torch_client.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.514676 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk.egg-info/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23302 2024-05-20 08:41:44.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2029 2024-05-20 08:41:44.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-05-20 08:41:44.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       82 2024-05-20 08:41:44.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk.egg-info/requires.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       22 2024-05-20 08:41:44.000000 acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.508331 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2323 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/README.md
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.508755 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/__init__.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.509896 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:28.000000 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      867 2024-02-22 04:32:28.000000 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6182 2024-05-15 04:39:47.000000 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener/events_listener.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23819 2024-05-15 04:39:47.000000 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener/utils.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1215 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener_plugin.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.510419 acceldata_airflow_sdk-3.5.0/docs/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.500698 acceldata_airflow_sdk-3.5.0/docs/_build/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.500765 acceldata_airflow_sdk-3.5.0/docs/_build/html/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.512125 acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      492 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       96 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      858 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      720 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      707 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      623 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1950 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/docs/conf.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.512360 acceldata_airflow_sdk-3.5.0/openlineage/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1050 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/airflow_local_settings.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.512584 acceldata_airflow_sdk-3.5.0/openlineage/config/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/config/__init__.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.513116 acceldata_airflow_sdk-3.5.0/openlineage/extractors/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/extractors/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3993 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/extractors/bigquery_insert_job_extractor.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6291 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/extractors/gcs_bigquery_extractor.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.513615 acceldata_airflow_sdk-3.5.0/openlineage/policy/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/policy/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4179 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/policy/config_helper.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:41:44.514191 acceldata_airflow_sdk-3.5.0/openlineage/tokenproviders/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/tokenproviders/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10427 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.5.0/openlineage/tokenproviders/access_key_secret_token_provider.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-05-20 08:41:44.515432 acceldata_airflow_sdk-3.5.0/setup.cfg
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      842 2024-05-15 04:39:47.000000 acceldata_airflow_sdk-3.5.0/setup.py
```

### Comparing `acceldata_airflow_sdk-3.4.0/LICENCE.txt` & `acceldata_airflow_sdk-3.5.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/PKG-INFO` & `acceldata_airflow_sdk-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_airflow_sdk
-Version: 3.4.0
+Version: 3.5.0
 Summary: Acceldata Airflow SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-airflow
 Classifier: Development Status :: 5 - Production/Stable
@@ -438,14 +438,10 @@
             print("Policy execution encountered an error.")
 
 ```
 
 Version Log
 ==========
 
-3.4.0 (08/05/2024)
+3.5.0 (09/05/2024)
 -------------------
-- Acceldata airflow sdk - Wrapper on apache airflow
-- Acceldata airflow sdk provides support for observability of airflow dags in ADOC catalog. With the use of acceldata airflow SDK, user can e2e observability on airflow dag run in ADOC UI.
-
-
-
+- Improved the ADOC Listener plugin to handle retry behaviour
```

### Comparing `acceldata_airflow_sdk-3.4.0/README.md` & `acceldata_airflow_sdk-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/dag.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/dag.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/handle_callback.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/decorators/handle_callback.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/job.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/decorators/job.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/span.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/decorators/span.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/initialiser.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/initialiser.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/execute_policy_operator.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/execute_policy_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/job_operator.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/job_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/span_operator.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/span_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/callback.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/utils/callback.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/constants.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/utils/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/torch_client.py` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk/utils/torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/PKG-INFO` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_airflow_sdk
-Version: 3.4.0
+Version: 3.5.0
 Summary: Acceldata Airflow SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-airflow
 Classifier: Development Status :: 5 - Production/Stable
@@ -438,14 +438,10 @@
             print("Policy execution encountered an error.")
 
 ```
 
 Version Log
 ==========
 
-3.4.0 (08/05/2024)
+3.5.0 (09/05/2024)
 -------------------
-- Acceldata airflow sdk - Wrapper on apache airflow
-- Acceldata airflow sdk provides support for observability of airflow dags in ADOC catalog. With the use of acceldata airflow SDK, user can e2e observability on airflow dag run in ADOC UI.
-
-
-
+- Improved the ADOC Listener plugin to handle retry behaviour
```

### Comparing `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/SOURCES.txt` & `acceldata_airflow_sdk-3.5.0/acceldata_airflow_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/README.md` & `acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/README.md`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/constants.py` & `acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/events_listener.py` & `acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener/events_listener.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,89 +14,91 @@
 from acceldata_sdk.models.pipeline import PipelineRunResult, PipelineRunStatus
 
 log = logging.getLogger(__name__)
 
 
 @hookimpl
 def on_dag_run_running(dag_run: DagRun, msg: str):
-    log.info("Listener Event==> on_dag_run_running")
+    log.info("Listener Event ==> on_dag_run_running")
     try:
         dag_id = dag_run.dag_id
         if observe_dag_env_variables_detected() and ignore_dag_env_variables_detected():
             log.error(INVALID_ENV_SELECTION_MESSAGE)
             return
 
         if validate_and_auto_instrument_dag(dag_id):
             log.info("Observing the DAG with dag_id  %s ", dag_id)
             create_pipeline_for_dag_run(dag_run, get_torch_client(), msg)
         else:
             log.info("Instrumentation not enabled for the dag with dag_id %s ", dag_id)
     except Exception as e:
-        log.error("Error in on_dag_run_running: %s", e)
+        log.error("Error in on_dag_run_running event : %s", e)
 
 
 @hookimpl
 def on_dag_run_failed(dag_run: DagRun, msg: str):
-    log.info("Listener Event==> on_dag_run_failed")
+    log.info("Listener Event ==> on_dag_run_failed")
     try:
         dag_id = dag_run.dag_id
         if observe_dag_env_variables_detected() and ignore_dag_env_variables_detected():
             log.error(INVALID_ENV_SELECTION_MESSAGE)
             return
 
         if validate_and_auto_instrument_dag(dag_id):
             log.info("Observing the DAG with dag_id  %s ", dag_id)
             end_pipeline_for_dag_run(dag_run, get_torch_client(), PipelineRunResult.FAILURE, PipelineRunStatus.FAILED,
                                      msg)
         else:
             log.info("Instrumentation not enabled for the dag with dag_id %s ", dag_id)
     except Exception as e:
-        log.error("Error in on_dag_run_failed: %s", e)
+        log.error("Error in on_dag_run_failed event : %s", e)
 
 
 @hookimpl
 def on_dag_run_success(dag_run: DagRun, msg: str):
-    log.info("Listener Event==> on_dag_run_success")
+    log.info("Listener Event ==> on_dag_run_success")
     try:
         dag_id = dag_run.dag_id
         if observe_dag_env_variables_detected() and ignore_dag_env_variables_detected():
             log.error(INVALID_ENV_SELECTION_MESSAGE)
             return
 
         if validate_and_auto_instrument_dag(dag_id):
             log.info("Observing the DAG with dag_id  %s ", dag_id)
             end_pipeline_for_dag_run(dag_run, get_torch_client(), PipelineRunResult.SUCCESS,
                                      PipelineRunStatus.COMPLETED, msg)
         else:
             log.info("Instrumentation not enabled for the dag with dag_id %s ", dag_id)
     except Exception as e:
-        log.error("Error in on_dag_run_success: %s", e)
+        log.error("Error in on_dag_run_success event: %s", e)
 
 
 @hookimpl
 def on_task_instance_running(previous_state: TaskInstanceState, task_instance: TaskInstance, session):
-    log.info("Listener Event==> on_task_instance_running")
+    log.info("Listener Event ==> on_task_instance_running")
+    log.info("Task instance state: %s", task_instance.state)
     try:
         dag_id = task_instance.dag_id
         if observe_dag_env_variables_detected() and ignore_dag_env_variables_detected():
             log.error(INVALID_ENV_SELECTION_MESSAGE)
             return
 
         if validate_and_auto_instrument_dag(dag_id):
             log.info("Observing the DAG with dag_id  %s ", dag_id)
             create_job_and_span(task_instance, get_torch_client())
         else:
             log.info("Instrumentation not enabled for the dag with dag_id %s ", dag_id)
     except Exception as e:
-        log.error("Error in on_task_instance_running: %s", e)
+        log.error("Error in on_task_instance_running evnet: %s", e)
 
 
 @hookimpl
 def on_task_instance_success(previous_state: TaskInstanceState, task_instance: TaskInstance, session):
-    log.info("Listener Event==> on_task_instance_success")
+    log.info("Listener Event ==> on_task_instance_success")
+    log.info("Task instance state: %s", task_instance.state)
     try:
         dag_id = task_instance.dag_id
         if observe_dag_env_variables_detected() and ignore_dag_env_variables_detected():
             log.error(INVALID_ENV_SELECTION_MESSAGE)
             return
 
         if validate_and_auto_instrument_dag(dag_id):
@@ -105,20 +107,21 @@
             log.info("Pushed span to Torch Server for success task")
             # Versions prior to 2.5.0 should end pipeline for task with zero downstream events
             end_pipeline_for_older_versions(task_instance, PipelineRunResult.SUCCESS, PipelineRunStatus.COMPLETED,
                                             session)
         else:
             log.info("Instrumentation not enabled for the dag with dag_id %s ", dag_id)
     except Exception as e:
-        log.error("Error in on_task_instance_success: %s", e)
+        log.error("Error in on_task_instance_success event: %s", e)
 
 
 @hookimpl
 def on_task_instance_failed(previous_state: TaskInstanceState, task_instance: TaskInstance, session):
-    log.info("Listener Event==> on_task_instance_failed")
+    log.info("Listener Event ==> on_task_instance_failed")
+    log.info("Task instance state: %s", task_instance.state)
     try:
         dag_id = task_instance.dag_id
         if observe_dag_env_variables_detected() and ignore_dag_env_variables_detected():
             log.error(INVALID_ENV_SELECTION_MESSAGE)
             return
 
         if validate_and_auto_instrument_dag(dag_id):
@@ -126,8 +129,8 @@
             end_job_and_span(task_instance, get_torch_client())
             log.info("Pushed span to Torch Server for failed task")
             # Versions prior to 2.5.0 should end pipeline for events with zero downstream events or upon failure
             end_pipeline_for_older_versions(task_instance, PipelineRunResult.FAILURE, PipelineRunStatus.FAILED, session)
         else:
             log.info("Instrumentation not enabled for the dag with dag_id %s ", dag_id)
     except Exception as e:
-        log.error("Error in on_task_instance_failed: %s", e)
+        log.error("Error in on_task_instance_failed event: %s", e)
```

### Comparing `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/utils.py` & `acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -44,24 +44,24 @@
         self.torchClient = get_or_create_torch_client()
 
     def get_torch_client(self):
         return self.torchClient
 
 
 def get_dag_run_url(dag_run):
-    base_url=conf.get('webserver', 'BASE_URL')
+    base_url = conf.get('webserver', 'BASE_URL')
     import urllib.parse
     execution_date = urllib.parse.quote(dag_run.execution_date.isoformat())
     dag_url = f'{base_url}/graph?root=&dag_id={dag_run.dag_id}&execution_date={execution_date}&arrang=LR'
     log.info(dag_url)
     return dag_url
 
 
 def get_or_create_torch_client():
-    #TODO: Required on Mac else the app crashes
+    # TODO: Required on Mac else the app crashes
     os.environ["no_proxy"] = "*"
     torch_catalog_url = os.environ["TORCH_CATALOG_URL"]
     access_key = os.environ["TORCH_ACCESS_KEY"]
     secret_key = os.environ["TORCH_SECRET_KEY"]
     torch_client = TorchClient(url=torch_catalog_url, access_key=access_key,
                                secret_key=secret_key)
     return torch_client
@@ -153,106 +153,138 @@
     dag_model = DagModel.get_current(task_instance.dag_id, session=session)
     dagbag = DagBag(dag_folder=dag_model.fileloc, read_dags_from_db=True)
     dag = dagbag.get_dag(task_instance.dag_id, session=session)
     task_ids = dag.task_dict[task_instance.task_id].downstream_task_ids
     return task_ids
 
 
-def create_pipeline_for_dag_run(dag_run: DagRun, torch_client, msg: str):
-    log.debug("create_pipeline_for_dag_run invoked")
-    dag_id = dag_run.dag_id
-    pipeline_name = dag_id
-    root_span_uid = dag_id + ROOT_SPAN_SUFFIX
-    dag_url = get_dag_run_url(dag_run)
-    try:
-        # 1. Create Pipeline
-        log.info("Creating pipeline for the DAG with the pipeline_name %s", pipeline_name)
-        pipeline = CreatePipeline(uid=pipeline_name, name=pipeline_name)
-        pipeline_response = torch_client.create_pipeline(pipeline)
-        dag_run_id = dag_run.run_id
+def create_pipeline(pipeline_name, torch_client):
+    log.info("Creating/updating pipeline for the DAG with the pipeline_name %s", pipeline_name)
+    pipeline = CreatePipeline(uid=pipeline_name, name=pipeline_name)
+    return torch_client.create_pipeline(pipeline)
+
+
+def prepare_dag_run_context_data(dag_run, dag_id, dag_run_id, dag_url, msg):
+    log.info("Preparing context data for pipeline run")
+    return {
+        STARTED: str(dag_run.start_date),
+        STATE: str(dag_run.state),
+        DAG_ID: str(dag_id),
+        DAG_RUN_ID: str(dag_run_id),
+        RUN_TYPE: str(dag_run.run_type),
+        DAG_URL: dag_url,
+        SCHEDULE_INTERVAL: str(dag_run.dag.schedule_interval) if dag_run.dag.schedule_interval else None,
+        MESSAGE: msg
+    }
+
+
+def prepare_dag_completion_context_data(dag_run, dag_id, dag_run_id, msg):
+    log.info("Preparing context data for pipeline run")
+    return {
+        STARTED: str(dag_run.start_date),
+        ENDED: str(dag_run.end_date),
+        STATE: str(dag_run.state),
+        DAG_ID: str(dag_id),
+        DAG_RUN_ID: str(dag_run_id),
+        RUN_TYPE: str(dag_run.run_type),
+        MESSAGE: msg
+    }
+
+
+def prepare_task_run_context_data(task_instance):
+    log.info("Preparing context data for task instance run")
+    return {
+        TASK_ID: str(task_instance.task_id),
+        TASK_RUN_ID: str(task_instance.run_id),
+        STARTED: str(task_instance.start_date),
+        OPERATOR: str(task_instance.operator),
+        STATE: str(task_instance.state),
+        TRY_NUMBER: str(task_instance.try_number),
+        OWNER: str(task_instance.task.owner),
+        QUEUE: str(task_instance.task.queue)
+    }
+
+
+def prepare_task_completion_context_data(task_instance, try_number):
+    log.info("Preparing context data for task completion")
+    return {
+        TASK_ID: str(task_instance.task_id),
+        TASK_RUN_ID: str(task_instance.run_id),
+        STARTED: str(task_instance.start_date),
+        ENDED: str(task_instance.start_date),
+        DURATION: str(task_instance.duration) + DURATION_UNIT,
+        OPERATOR: str(task_instance.operator),
+        STATE: str(task_instance.state),
+        TRY_NUMBER: str(try_number)
+    }
 
-        # 2. Create pipeline run
-        log.info("Creating pipeline run for the pipeline with name %s", pipeline_name)
-        log.debug(f"dag run {dag_run}")
-        context_data = {
-            STARTED: str(dag_run.start_date),
-            STATE: str(dag_run.state),
-            DAG_ID: str(dag_id),
-            DAG_RUN_ID: str(dag_run_id),
-            RUN_TYPE: str(dag_run.run_type),
-            DAG_URL: dag_url,
-            # TODO: Code breaks for the older version,
-            # SCHEDULE_INTERVAL: str(dag_run.dag.schedule_interval),
-            MESSAGE: msg}
-
-        log.info("Getting the pipeline run corresponding to dag run based on continuation_id and pipeline_id")
-        continuation_id = f"{dag_id}.{dag_run_id}"
-        pipeline_run = pipeline_response.create_pipeline_run(context_data=context_data, continuation_id=continuation_id)
-        pipeline_run_id = pipeline_run.id
-        log.info("Created pipeline run with the pipeline_run_id: %s", pipeline_run_id)
 
-        # 3. Create root span
-        log.info("Creating the root span")
-        root_span = pipeline_run.create_span(uid=root_span_uid)
-        event_uid = f'{root_span_uid}.start_event'
-        pipeline_start_event = GenericEvent(context_data=context_data,
-                                            event_uid=event_uid)
-        root_span.send_event(span_event=pipeline_start_event)
-    except APIError as api_error:
-        # 2. Pipeline doesn't exist , create pipeline with the dag id as the identity
-        log.error("Pipeline creation for the pipeline : %s  failed with error:  %s", str(pipeline_name), str(api_error))
+def create_pipeline_run(pipeline_response, context_data, dag_id, dag_run_id):
+    continuation_id = f"{dag_id}.{dag_run_id}"
+    log.info("Creating pipeline run for the pipeline with name %s and continuation_id %s", pipeline_response.name)
+    return pipeline_response.create_pipeline_run(context_data=context_data, continuation_id=continuation_id)
+
+
+def create_root_span(pipeline_run, root_span_uid, context_data):
+    log.info("Creating the root span with uid %s", root_span_uid)
+    root_span = pipeline_run.create_span(uid=root_span_uid)
+    event_uid = f'{root_span_uid}.start_event'
+    pipeline_start_event = GenericEvent(context_data=context_data, event_uid=event_uid)
+    root_span.send_event(span_event=pipeline_start_event)
+    return root_span
+
+
+def get_pipeline_by_name(torch_client, pipeline_name):
+    log.debug("Getting the pipeline corresponding to the pipeline name: %s", pipeline_name)
+    return torch_client.get_pipeline(pipeline_name)
+
+
+def get_pipeline_run_by_continuation_id(torch_client, dag_id, run_id, pipeline):
+    continuation_id = f"{dag_id}.{run_id}"
+    log.info("Getting the pipeline run corresponding to dag run based on continuation_id : %s and pipeline_id: %s",
+             continuation_id, pipeline.id)
+    return torch_client.get_pipeline_run(continuation_id=continuation_id, pipeline_id=pipeline.id)
 
 
 def end_pipeline_for_dag_run(dag_run: DagRun, torch_client, pipeline_run_result: PipelineRunResult,
                              pipeline_run_status: PipelineRunStatus, msg: str):
+    log.debug("end_pipeline_for_dag_run called with dag_run: %s", dag_run)
+
     dag_id = dag_run.dag_id
-    pipeline_name = dag_id
     dag_run_id = dag_run.run_id
-    log.debug("end_pipeline_for_dag_run called")
-    # 1. get the pipeline corresponding to the above pipelineName
-    log.debug("Getting the pipeline corresponding to the pipeline name: %s", pipeline_name)
-    pipeline = torch_client.get_pipeline(pipeline_name)
 
+    # 1. get the pipeline corresponding to the above pipelineName
+    pipeline = get_pipeline_by_name(torch_client, dag_id)
     #  2. get the pipeline run for the dag run
-    log.info("Getting the pipeline run corresponding to dag run based on continuation_id and pipeline_id")
-    continuation_id = f"{dag_id}.{dag_run_id}"
-    pipeline_run = torch_client.get_pipeline_run(continuation_id=continuation_id,
-                                                 pipeline_id=pipeline.id)
+    pipeline_run = get_pipeline_run_by_continuation_id(torch_client, dag_id, dag_run_id, pipeline)
 
     # 3. get the root span for the run and mark it as success or failure accordingly
-    log.debug("Getting the root span for the pipeline run with pipeline run id: %s", pipeline_run.id)
     root_span_context = pipeline_run.get_root_span()
     log.debug("Got the root span context %s", root_span_context)
-
-    root_span_uid = dag_run.dag_id + ROOT_SPAN_SUFFIX
-    log.debug("Root span uid: %s", root_span_uid)
+    root_span_uid = dag_id + ROOT_SPAN_SUFFIX
+    log.debug("Root span uid for the pipeline run is : %s", root_span_uid)
     event_uid = f'{root_span_uid}.end_event'
-    context_data = {STARTED: str(dag_run.start_date),
-                    ENDED: str(dag_run.end_date),
-                    DAG_ID: str(dag_run.dag_id),
-                    DAG_RUN_ID: str(dag_run.run_id),
-                    RUN_TYPE: str(dag_run.run_type),
-                    STATE: str(dag_run.state),
-                    MESSAGE: msg}
+    context_data = prepare_dag_completion_context_data(dag_run, dag_id, dag_run_id, msg)
     pipeline_end_event = GenericEvent(context_data=context_data,
                                       event_uid=event_uid)
+    root_span_context.send_event(span_event=pipeline_end_event)
 
-    # 4. Mark the run as success or failure accordingly
+    #  4.Mark the run as success or failure based on run result
     if pipeline_run_result == PipelineRunResult.SUCCESS:
         log.debug("pipeline_run_result is: %s", pipeline_run_result)
         root_span_context.end()
         log.info("Root span has been ended.")
 
     elif pipeline_run_result == PipelineRunResult.FAILURE:
         log.debug("pipeline_run_result is: %s", pipeline_run_result)
         root_span_context.failed()
         log.info("Root span has been Failed.")
 
     log.info("Ending the pipeline run")
-    root_span_context.send_event(span_event=pipeline_end_event)
+    # 5. Terminating the pipeline run
     pipeline_run.update_pipeline_run(context_data=context_data,
                                      result=pipeline_run_result,
                                      status=pipeline_run_status)
 
 
 def validate_and_auto_instrument_dag(dag_id):
     # Observe the given dag if any one of below condition happens:
@@ -269,24 +301,24 @@
     return False
 
 
 def create_job_and_span(task_instance: TaskInstance, torch_client: TorchClient):
     dag_run_id = task_instance.dag_run.run_id
     dag_id = task_instance.dag_id
     pipeline_name = str(task_instance.dag_id)
-    pipeline = torch_client.get_pipeline(pipeline_name)
-    log.info("Getting the pipeline run corresponding to dag run based on continuation_id and pipeline_id")
-    continuation_id = f"{dag_id}.{dag_run_id}"
-    pipeline_run = torch_client.get_pipeline_run(continuation_id=continuation_id,
-                                                 pipeline_id=pipeline.id)
+    pipeline = get_pipeline_by_name(torch_client, pipeline_name)
+    pipeline_run = get_pipeline_run_by_continuation_id(torch_client, dag_id, dag_run_id, pipeline)
     root_span_context = pipeline_run.get_root_span()
     log.debug("Got the root span context %s", root_span_context)
 
     # 1. create a job with  job_uid and inputs based on upstream tasks
-    upstream_list = task_instance.task.upstream_list
+    upstream_list = []
+    if task_instance.task and task_instance.task.upstream_list:
+        upstream_list = task_instance.task.upstream_list
+
     input_nodes = []
     associated_job_uids = []
 
     # Construct node inputs
     log.debug("Constructing the input_nodes from upstream tasks")
     for upstream in upstream_list:
         job_uid = upstream.task_id
@@ -299,91 +331,146 @@
         name=job_uid,
         version=pipeline_run.versionId,
         pipeline_run_id=pipeline_run.id,
         inputs=input_nodes,
         bounded_by_span=False
     )
 
-    log.info("Creating job %s", job)
+    log.info("Creating job: %s", job)
     pipeline.create_job(job)
 
     # 2. get the root span and then create child span on that object using the spanUid above
     # and pass the jobUid as well to this function
+
     log.info("Initiate Child span for job with job_uid %s", job_uid)
     child_span_uid = f'{job_uid}.span'
     log.info("associatedJobUids %s for the child span with child_span_uid %s", associated_job_uids, child_span_uid)
-    child_span = root_span_context.create_child_span(uid=child_span_uid, associatedJobUids=associated_job_uids)
-    log.info("Created span with child_span_uid %s", child_span_uid)
 
-    child_span.start()
-    log.info("Started the child span with child_span_uid %s", child_span_uid)
-    log.info("Sending job start event the child span with child_span_uid %s", child_span_uid)
-
-    event_uid = f'{child_span_uid}.start_event'
-    context_data = {TASK_ID: str(task_instance.task_id),
-                    TASK_RUN_ID: str(task_instance.run_id),
-                    STARTED: str(task_instance.start_date),
-                    OPERATOR: str(task_instance.operator),
-                    STATE: str(task_instance.state),
-                    TRY_NUMBER: str(task_instance.try_number),
-                    OWNER: str(task_instance.task.owner),
-                    QUEUE: str(task_instance.task.queue)}
+    try_number = task_instance.try_number
+    event_uid = f'{child_span_uid}.job.start.try_{try_number}.event'
+    context_data = prepare_task_run_context_data(task_instance)
     job_start_event = GenericEvent(context_data=context_data,
                                    event_uid=event_uid)
 
-    child_span.send_event(span_event=job_start_event)
-    log.info("Successfully sent job start event for the child span with child_span_uid %s", child_span_uid)
+    # 3. Handle the case when the span already exists (retry)
+    try:
+        child_span = pipeline_run.get_span(child_span_uid)
+        log.info("Span already exists with child_span_uid : %s", child_span_uid)
+        # Emit generic events related to the retry here
+        log.info("Sending job retry start event %s for the child span with child_span_uid %s", job_start_event,
+                 child_span_uid)
+        child_span.send_event(span_event=job_start_event)
+        log.info("Successfully sent job start retry event for the child span with child_span_uid %s", child_span_uid)
+        return
+    except Exception as e:
+        # Span doesn't exist, create the span under the root span
+        log.warning("Error while getting span : %s", e)
+        log.info("Span doesn't exist with child_span_uid %s . Create the child span", child_span_uid)
+        child_span = root_span_context.create_child_span(uid=child_span_uid, associatedJobUids=associated_job_uids)
+        log.info("Created span with child_span_uid %s", child_span_uid)
+        child_span.start()
+        log.info("Started the child span with child_span_uid %s", child_span_uid)
+        log.info("Sending job start event %s for the child span with child_span_uid %s", job_start_event,
+                 child_span_uid)
+        child_span.send_event(span_event=job_start_event)
+        log.info("Successfully sent job start event for the child span with child_span_uid %s", child_span_uid)
+
+
+def handle_failed_state(task_instance, child_span_uid, try_number, max_retries, child_span):
+    # Task instance state comes as FAILED, so try_number is incremented by 1, hence, need to reduce by 1
+    # If the TaskInstance is currently running, this will match the column in the database,
+    # in all other cases this will be incremented.
+    task_failure_try_number = try_number - 1
+    context_data = prepare_task_completion_context_data(task_instance, task_failure_try_number)
+    if task_failure_try_number <= max_retries:
+        # Logic to send generic event for job failure if this isn't the last retry
+        log.info("Sending job end event for the child span with child_span_uid %s", child_span_uid)
+        job_fail_event = GenericEvent(context_data=context_data,
+                                      event_uid=f'{child_span_uid}.job.failed.try_{task_failure_try_number}.event')
+        child_span.send_event(span_event=job_fail_event)
+        log.info("Sending failed retry data event for the child span with child_span_uid %s", child_span_uid)
+        return
+
+    # This is the last retry, the span should be ended here
+    log.info("Task instance in failed State and last retry. Sending JobFailEvent")
+    event_uid = f'{child_span_uid}.job.failed.try.{task_failure_try_number}.event'
+    job_fail_event = GenericEvent(context_data=context_data, event_uid=event_uid)
+    child_span.send_event(span_event=job_fail_event)
+    child_span.failed()
+    log.info("Marking child span as failed")
+
+
+def handle_failed_state_listener_bug(task_instance, child_span_uid, try_number, max_retries, child_span):
+    # Task instance state is coming as running for failure callback also, so no need to decrement in this case
+    # If the TaskInstance is currently running, this will match the column in the database,
+    # in all other cases this will be incremented.
+    context_data = prepare_task_completion_context_data(task_instance, try_number)
+    if try_number <= max_retries:
+        log.info("Sending job end event for the child span with child_span_uid %s", child_span_uid)
+        job_fail_event = GenericEvent(context_data=context_data,
+                                      event_uid=f'{child_span_uid}.job.failed.try.{try_number}.event')
+        child_span.send_event(span_event=job_fail_event)
+        log.info("Sending failed retry data event for the child span with child_span_uid %s", child_span_uid)
+        return
+
+    # This is the last retry, the span should be ended here
+    log.info("Task instance in failed State and last retry. Sending JobFailEvent")
+    event_uid = f'{child_span_uid}.job.failed.try.{try_number}.event'
+    job_fail_event = GenericEvent(context_data=context_data, event_uid=event_uid)
+    child_span.send_event(span_event=job_fail_event)
+    child_span.failed()
+    log.info("Marking child span as failed")
+
+
+def handle_success_state(task_instance, child_span, child_span_uid, try_number):
+    # Task instance state comes as SUCCESS, so try_number is incremented by 1, hence, need to reduce by 1
+    # If the TaskInstance is currently running, this will match the column in the database,
+    task_success_try_number = try_number - 1
+    context_data = prepare_task_completion_context_data(task_instance, task_success_try_number)
+    log.info("Task instance in success State. Sending JobEndEvent")
+    event_uid = f'{child_span_uid}.job.success.try.{task_success_try_number}.event'
+    job_end_event = GenericEvent(context_data=context_data, event_uid=event_uid)
+    child_span.send_event(span_event=job_end_event)
+    child_span.end()
+    log.info("Marking child span as success")
 
 
 def end_job_and_span(task_instance: TaskInstance, torch_client: TorchClient, ):
     log.info("TaskInstance State: %s", task_instance.state)
     # 1. Get pipeline for the task
     log.info("Get pipeline for the task")
     dag_id = task_instance.dag_id
     pipeline_name = str(dag_id)
     pipeline = torch_client.get_pipeline(pipeline_name)
 
     #  2. get the pipeline run on the dag run
-    log.info("Getting the pipeline run for the corresponding dag run based on continuation_id and pipeline_id")
     dag_run_id = task_instance.dag_run.run_id
-    continuation_id = f"{dag_id}.{dag_run_id}"
-    pipeline_run = torch_client.get_pipeline_run(continuation_id=continuation_id,
-                                                 pipeline_id=pipeline.id)
+    pipeline_run = get_pipeline_run_by_continuation_id(torch_client, dag_id, dag_run_id, pipeline)
     job_uid = task_instance.task_id
 
     child_span_uid = f'{job_uid}.span'
     log.info("Fetching the child span with child span uid %s", child_span_uid)
-    child_span = pipeline_run.get_span(child_span_uid)
 
     log.info("Triggering job end events based on the task state")
-    context_data = {TASK_ID: str(task_instance.task_id),
-                    TASK_RUN_ID: str(task_instance.run_id),
-                    STARTED: str(task_instance.start_date),
-                    ENDED: str(task_instance.start_date),
-                    DURATION: str(task_instance.duration) + DURATION_UNIT,
-                    OPERATOR: str(task_instance.operator),
-                    STATE: str(task_instance.state),
-                    TRY_NUMBER: str(task_instance.try_number)}
-
-    if str(task_instance.state) == FAILED:
-        # TODO : try to extract failure reason and logs
-        log.info("Task instance in failed State. Sending JobFailEvent")
-        event_uid = f'{child_span_uid}.failed_event'
-        job_fail_event = GenericEvent(context_data=context_data, event_uid=event_uid)
-        child_span.send_event(span_event=job_fail_event)
-        child_span.failed()
-        log.info("Marking child span as failed")
+    try_number = task_instance.try_number
+    log.info("try_number inside task failure/success callback %s", try_number)
+
+    max_retries = task_instance.task.retries
+
+    log.info("max_retries %s", max_retries)
+    child_span = pipeline_run.get_span(child_span_uid)
 
     if str(task_instance.state) == SUCCESS:
-        log.info("Task instance in success State. Sending JobEndEvent")
-        event_uid = f'{child_span_uid}.success_event'
-        job_end_event = GenericEvent(context_data=context_data, event_uid=event_uid)
-        child_span.send_event(span_event=job_end_event)
-        child_span.end()
-        log.info("Marking child span as success")
+        handle_success_state(task_instance, child_span, child_span_uid, try_number)
+    elif str(task_instance.state) == FAILED:
+        handle_failed_state(task_instance, child_span_uid, try_number, max_retries, child_span)
+    else:
+        # Due to a bug in airflow  the task instance state is coming as running for failure callback also,
+        # so no need to decrement the try number and take care of this case
+        handle_failed_state_listener_bug(task_instance, child_span_uid, try_number, max_retries, child_span)
 
 
 def create_pipeline_for_older_versions(task_instance: TaskInstance, session):
     log.info("Checking if pipeline needs to be created for the task_instance : %s", task_instance)
     upstream_size = len(task_instance.task.upstream_list)
     log.debug("Upstream size: %s", upstream_size)
     current_version = airflow.__version__
@@ -413,7 +500,33 @@
                      current_version)
             end_pipeline_for_dag_run(task_instance.dag_run, get_torch_client(), pipelineRunResult,
                                      pipelineRunStatus, msg="")
         else:
             log.debug("task instance completion handling not needed to terminate the pipeline for the newer versions")
     else:
         log.debug("Downstream size is > 0 and task_instance state is not FAILED. Proceeding with the next tasks")
+
+
+def create_pipeline_for_dag_run(dag_run: DagRun, torch_client, msg: str):
+    log.debug("create_pipeline_for_dag_run invoked")
+    dag_id = dag_run.dag_id
+    pipeline_name = dag_id
+    root_span_uid = dag_id + ROOT_SPAN_SUFFIX
+    dag_url = get_dag_run_url(dag_run)
+    try:
+        # 1. Create/Update Pipeline
+        pipeline_response = create_pipeline(pipeline_name, torch_client)
+        dag_run_id = dag_run.run_id
+
+        # 2. Create pipeline run
+        log.debug(f"dag run: {dag_run}")
+        context_data = prepare_dag_run_context_data(dag_run, dag_id, dag_run_id, dag_url, msg)
+        pipeline_run = create_pipeline_run(pipeline_response, context_data, dag_id, dag_run_id)
+        pipeline_run_id = pipeline_run.id
+        log.info("Created pipeline run with the pipeline_run_id: %s", pipeline_run_id)
+
+        # 3. Create root span
+        log.info("Creating the root span")
+        root_span = create_root_span(pipeline_run, root_span_uid, context_data)
+    except APIError as api_error:
+        log.error("Pipeline creation for the pipeline with name : %s  , failed with error:  %s", str(pipeline_name),
+                  str(api_error))
```

### Comparing `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener_plugin.py` & `acceldata_airflow_sdk-3.5.0/adoc_listener_plugin/plugins/listener_plugin.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt` & `acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt` & `acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt` & `acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt` & `acceldata_airflow_sdk-3.5.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/docs/conf.py` & `acceldata_airflow_sdk-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/openlineage/airflow_local_settings.py` & `acceldata_airflow_sdk-3.5.0/openlineage/airflow_local_settings.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/openlineage/extractors/bigquery_insert_job_extractor.py` & `acceldata_airflow_sdk-3.5.0/openlineage/extractors/bigquery_insert_job_extractor.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/openlineage/extractors/gcs_bigquery_extractor.py` & `acceldata_airflow_sdk-3.5.0/openlineage/extractors/gcs_bigquery_extractor.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/openlineage/policy/config_helper.py` & `acceldata_airflow_sdk-3.5.0/openlineage/policy/config_helper.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/openlineage/tokenproviders/access_key_secret_token_provider.py` & `acceldata_airflow_sdk-3.5.0/openlineage/tokenproviders/access_key_secret_token_provider.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.4.0/setup.py` & `acceldata_airflow_sdk-3.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: Apache Software License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='acceldata_airflow_sdk',
-  version='3.4.0',
+  version='3.5.0',
   description='Acceldata Airflow SDK.' + '\n\n' + open('README.txt').read(),
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type="text/markdown",
   url='',
   author='acceldata',
   author_email='apisupport@acceldata.io',
   license='MIT License',
```


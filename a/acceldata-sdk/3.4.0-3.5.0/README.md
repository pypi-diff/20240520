# Comparing `tmp/acceldata_sdk-3.4.0.tar.gz` & `tmp/acceldata_sdk-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acceldata_sdk-3.4.0.tar", last modified: Wed May  8 11:06:44 2024, max compression
+gzip compressed data, was "acceldata_sdk-3.5.0.tar", last modified: Mon May 20 08:40:32 2024, max compression
```

## Comparing `acceldata_sdk-3.4.0.tar` & `acceldata_sdk-3.5.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.560537 acceldata_sdk-3.4.0/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      213 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/CHANGELOG.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/DATASOURCE_README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/LICENCE.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/MANIFEST.in
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23764 2024-05-08 11:06:44.559992 acceldata_sdk-3.4.0/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    18890 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/README.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.536074 acceldata_sdk-3.4.0/acceldata_sdk/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     7776 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/common.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2098 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      329 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/datetime_utils.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/errors.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.538674 acceldata_sdk-3.4.0/acceldata_sdk/events/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      903 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/generic_event.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/job_events.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      826 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/log_events.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1487 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/span_event.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/initialiser.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.552034 acceldata_sdk-3.4.0/acceldata_sdk/models/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6106 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/asset.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/assetType.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10021 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/connection.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3522 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/create_asset.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     8164 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/datasource.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10268 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/dqrule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4599 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/job.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    24639 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/pipeline.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2015 2024-03-21 11:14:24.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/profile.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    11785 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/reconcillationrule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/rule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10102 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/ruleExecutionResult.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2396 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/span.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10582 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/span_context.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/tags.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    15888 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/acceldata_sdk/torch_client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    48151 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/acceldata_sdk/torch_http_client.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.559519 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23764 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1923 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/requires.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.552265 acceldata_sdk-3.4.0/docs/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.531315 acceldata_sdk-3.4.0/docs/_build/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.531392 acceldata_sdk-3.4.0/docs/_build/html/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.556143 acceldata_sdk-3.4.0/docs/_build/html/_sources/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/readme.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/readme_datasource.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/readme_pipeline.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/conf.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.558026 acceldata_sdk-3.4.0/integration_tests/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3765 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_ds_assets.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    11805 2024-03-21 11:14:17.000000 acceldata_sdk-3.4.0/integration_tests/test_external_integration_default_time.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    15535 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_external_integration_explicit_time.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_pipelines.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4386 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_policy.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    27169 2024-05-02 08:45:58.000000 acceldata_sdk-3.4.0/integration_tests/test_torch_client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-05-08 11:06:44.560614 acceldata_sdk-3.4.0/setup.cfg
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/setup.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.696355 acceldata_sdk-3.5.0/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      119 2024-05-15 04:39:47.000000 acceldata_sdk-3.5.0/CHANGELOG.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/DATASOURCE_README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/LICENCE.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/MANIFEST.in
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23670 2024-05-20 08:40:32.696026 acceldata_sdk-3.5.0/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    18890 2024-05-08 12:39:35.000000 acceldata_sdk-3.5.0/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/README.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.677915 acceldata_sdk-3.5.0/acceldata_sdk/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     7776 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/common.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2098 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      329 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/datetime_utils.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/errors.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.680939 acceldata_sdk-3.5.0/acceldata_sdk/events/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/events/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      903 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/events/generic_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/events/job_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      826 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/events/log_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1487 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/events/span_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/initialiser.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.689459 acceldata_sdk-3.5.0/acceldata_sdk/models/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6106 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/assetType.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10021 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/connection.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3522 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/create_asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     8164 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/datasource.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10268 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/dqrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4599 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/job.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    24639 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/pipeline.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2015 2024-03-21 11:14:24.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/profile.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    11785 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/reconcillationrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/rule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10102 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/ruleExecutionResult.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2396 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/span.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10582 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/span_context.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/acceldata_sdk/models/tags.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    15888 2024-05-08 12:39:35.000000 acceldata_sdk-3.5.0/acceldata_sdk/torch_client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    48365 2024-05-20 06:04:31.000000 acceldata_sdk-3.5.0/acceldata_sdk/torch_http_client.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.695609 acceldata_sdk-3.5.0/acceldata_sdk.egg-info/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23670 2024-05-20 08:40:32.000000 acceldata_sdk-3.5.0/acceldata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1923 2024-05-20 08:40:32.000000 acceldata_sdk-3.5.0/acceldata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-05-20 08:40:32.000000 acceldata_sdk-3.5.0/acceldata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2024-05-20 08:40:32.000000 acceldata_sdk-3.5.0/acceldata_sdk.egg-info/requires.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2024-05-20 08:40:32.000000 acceldata_sdk-3.5.0/acceldata_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.689722 acceldata_sdk-3.5.0/docs/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.672914 acceldata_sdk-3.5.0/docs/_build/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.672986 acceldata_sdk-3.5.0/docs/_build/html/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.691884 acceldata_sdk-3.5.0/docs/_build/html/_sources/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/_build/html/_sources/readme.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/_build/html/_sources/readme_datasource.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/_build/html/_sources/readme_pipeline.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/_build/html/_sources/torch_sdk.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/docs/conf.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-20 08:40:32.694964 acceldata_sdk-3.5.0/integration_tests/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/integration_tests/test_constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3765 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/integration_tests/test_ds_assets.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    11805 2024-03-21 11:14:17.000000 acceldata_sdk-3.5.0/integration_tests/test_external_integration_default_time.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    15535 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/integration_tests/test_external_integration_explicit_time.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/integration_tests/test_pipelines.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4386 2024-02-22 04:32:27.000000 acceldata_sdk-3.5.0/integration_tests/test_policy.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    27169 2024-05-02 08:45:58.000000 acceldata_sdk-3.5.0/integration_tests/test_torch_client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-05-20 08:40:32.696419 acceldata_sdk-3.5.0/setup.cfg
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2024-05-15 04:39:47.000000 acceldata_sdk-3.5.0/setup.py
```

### Comparing `acceldata_sdk-3.4.0/DATASOURCE_README.md` & `acceldata_sdk-3.5.0/DATASOURCE_README.md`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/LICENCE.txt` & `acceldata_sdk-3.5.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/PKG-INFO` & `acceldata_sdk-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_sdk
-Version: 3.4.0
+Version: 3.5.0
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -518,13 +518,13 @@
 filter = PolicyFilter(policyType=RuleType.RECONCILIATION, enable=True)
 # List all rules
 recon_rules = torch_client.list_all_policies(filter=filter)
 ```
 
 Version Log
 ==========
-
-3.4.0 (08/05/2024)
+3.5.0 (09/05/2024)
 -------------------
-- Incorporated fix for control plane version compatibility check based apis to handle patch version
-- Disable version compatibility check by default
+- Release for 3.5.0 version of the ADOC control plane
+
+
```

### Comparing `acceldata_sdk-3.4.0/README.md` & `acceldata_sdk-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/client.py` & `acceldata_sdk-3.5.0/acceldata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/common.py` & `acceldata_sdk-3.5.0/acceldata_sdk/common.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/constants.py` & `acceldata_sdk-3.5.0/acceldata_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/events/generic_event.py` & `acceldata_sdk-3.5.0/acceldata_sdk/events/generic_event.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/events/job_events.py` & `acceldata_sdk-3.5.0/acceldata_sdk/events/job_events.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/events/log_events.py` & `acceldata_sdk-3.5.0/acceldata_sdk/events/log_events.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/events/span_event.py` & `acceldata_sdk-3.5.0/acceldata_sdk/events/span_event.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/asset.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/assetType.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/assetType.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/connection.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/connection.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/create_asset.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/create_asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/datasource.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/datasource.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/dqrule.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/dqrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/job.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/job.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/pipeline.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/profile.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/profile.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/reconcillationrule.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/reconcillationrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/rule.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/rule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/ruleExecutionResult.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/ruleExecutionResult.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/span.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/span.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/span_context.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/span_context.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/models/tags.py` & `acceldata_sdk-3.5.0/acceldata_sdk/models/tags.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/torch_client.py` & `acceldata_sdk-3.5.0/acceldata_sdk/torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk/torch_http_client.py` & `acceldata_sdk-3.5.0/acceldata_sdk/torch_http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -704,16 +704,22 @@
         :param uid: uid of an asset
         :return: asset data (Asset)
         """
         if uid is None:
             raise Exception('Asset uid is required')
         url = f'{self._catalog_api_base}/assets?uid={uid}'
         asset = self._get_asset(url)
-        asset['data']['client'] = self
-        return Asset(**asset['data'])
+        if asset is None:
+            return None
+        asset_data = asset['data']
+        if asset_data is None or not asset_data or len(asset_data) == 0:
+            return None
+        asset_res = list(asset_data)[0]
+        asset_res['client'] = self
+        return Asset(**asset_res)
 
     def _get_asset(self, url: str):
         response = self._get(
             url=url
         )
         return response
```

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk.egg-info/PKG-INFO` & `acceldata_sdk-3.5.0/acceldata_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_sdk
-Version: 3.4.0
+Version: 3.5.0
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -518,13 +518,13 @@
 filter = PolicyFilter(policyType=RuleType.RECONCILIATION, enable=True)
 # List all rules
 recon_rules = torch_client.list_all_policies(filter=filter)
 ```
 
 Version Log
 ==========
-
-3.4.0 (08/05/2024)
+3.5.0 (09/05/2024)
 -------------------
-- Incorporated fix for control plane version compatibility check based apis to handle patch version
-- Disable version compatibility check by default
+- Release for 3.5.0 version of the ADOC control plane
+
+
```

### Comparing `acceldata_sdk-3.4.0/acceldata_sdk.egg-info/SOURCES.txt` & `acceldata_sdk-3.5.0/acceldata_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.events.rst.txt` & `acceldata_sdk-3.5.0/docs/_build/html/_sources/torch_sdk.events.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.models.rst.txt` & `acceldata_sdk-3.5.0/docs/_build/html/_sources/torch_sdk.models.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.rst.txt` & `acceldata_sdk-3.5.0/docs/_build/html/_sources/torch_sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/docs/conf.py` & `acceldata_sdk-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/integration_tests/test_constants.py` & `acceldata_sdk-3.5.0/integration_tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/integration_tests/test_ds_assets.py` & `acceldata_sdk-3.5.0/integration_tests/test_ds_assets.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/integration_tests/test_external_integration_default_time.py` & `acceldata_sdk-3.5.0/integration_tests/test_external_integration_default_time.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/integration_tests/test_external_integration_explicit_time.py` & `acceldata_sdk-3.5.0/integration_tests/test_external_integration_explicit_time.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/integration_tests/test_pipelines.py` & `acceldata_sdk-3.5.0/integration_tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/integration_tests/test_policy.py` & `acceldata_sdk-3.5.0/integration_tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/integration_tests/test_torch_client.py` & `acceldata_sdk-3.5.0/integration_tests/test_torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.4.0/setup.py` & `acceldata_sdk-3.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # except (IOError, ImportError):
 #     description = open('README.md').read()
 
 # Change MIN_TORCH_BACKEND_VERSION_SUPPORTED in constants as well if needed while updating version here
 
 setup(
     name='acceldata_sdk',
-    version='3.4.0',
+    version='3.5.0',
     description='Acceldata SDK.' + '\n\n' + open('README.txt').read(),
     long_description=open('README.md').read() + '\n\n' + open('DATASOURCE_README.md').read() + '\n\n'  + open('CHANGELOG.txt').read(),
     long_description_content_type="text/markdown",
     url='',
     author='acceldata',
     author_email='apisupport@acceldata.io',
     license='MIT License',
```


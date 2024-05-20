# Comparing `tmp/cript-2.3.0.tar.gz` & `tmp/cript-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cript-2.3.0.tar", last modified: Mon Apr  1 18:48:28 2024, max compression
+gzip compressed data, was "cript-2.4.0.tar", last modified: Mon May 20 21:16:34 2024, max compression
```

## Comparing `cript-2.3.0.tar` & `cript-2.4.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.763323 cript-2.3.0/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1122 2023-08-30 00:21:45.000000 cript-2.3.0/LICENSE.md
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5659 2024-04-01 18:48:28.763323 cript-2.3.0/PKG-INFO
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5012 2024-02-21 00:00:01.000000 cript-2.3.0/README.md
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      346 2023-08-30 00:21:45.000000 cript-2.3.0/pyproject.toml
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      762 2024-04-01 18:48:28.763323 cript-2.3.0/setup.cfg
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)       69 2023-08-30 00:21:45.000000 cript-2.3.0/setup.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.755323 cript-2.3.0/src/
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.755323 cript-2.3.0/src/cript/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      849 2024-03-25 21:02:04.000000 cript-2.3.0/src/cript/__init__.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/api/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      219 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/__init__.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    40944 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/api/api.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      316 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/api_config.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9155 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/data_schema.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    10793 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/exceptions.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9520 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/paginator.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/api/utils/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      137 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/api/utils/__init__.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1310 2024-02-21 00:00:01.000000 cript-2.3.0/src/cript/api/utils/aws_s3_utils.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1990 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/api/utils/get_host_token.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1302 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/utils/helper_functions.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8399 2024-02-21 21:14:12.000000 cript-2.3.0/src/cript/api/utils/save_helper.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2806 2023-09-11 22:06:53.000000 cript-2.3.0/src/cript/api/utils/web_file_downloader.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1035 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/valid_search_modes.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     3006 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/vocabulary_categories.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      218 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/exceptions.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      615 2024-03-25 21:02:04.000000 cript-2.3.0/src/cript/nodes/__init__.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    27915 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/core.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    14386 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/nodes/exceptions.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2296 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/node_iterator.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/primary_nodes/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      617 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/nodes/primary_nodes/__init__.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9735 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/collection.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    15136 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/computation.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    19308 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/computation_process.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    20789 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/data.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    14052 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/experiment.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     4825 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/inventory.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    21826 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/nodes/primary_nodes/material.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2891 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/nodes/primary_nodes/primary_base_node.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    21207 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/process.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8528 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/nodes/primary_nodes/project.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    19736 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/reference.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/subobjects/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      683 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/nodes/subobjects/__init__.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9286 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/algorithm.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8103 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/citation.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    17261 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/computational_forcefield.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    16294 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/condition.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    10346 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/equipment.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     7580 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/ingredient.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     6017 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/parameter.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    24342 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/property.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     7819 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/quantity.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5126 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/software.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9502 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/software_configuration.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/supporting_nodes/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      132 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/nodes/supporting_nodes/__init__.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    16377 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/supporting_nodes/file.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     4439 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/supporting_nodes/user.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/util/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)      234 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/util/__init__.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     3398 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/nodes/util/core.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    18567 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/util/json.py
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2886 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/uuid_base.py
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript.egg-info/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5659 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/PKG-INFO
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2139 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/SOURCES.txt
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)        1 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/dependency_links.txt
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)       68 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/requires.txt
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)        6 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/top_level.txt
-drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/tests/
--rw-r--r--   0 ludwig    (1000) ludwig    (1000)    14716 2024-04-01 18:45:13.000000 cript-2.3.0/tests/test_node_util.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.828595 cript-2.4.0/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1122 2023-08-30 00:21:45.000000 cript-2.4.0/LICENSE.md
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5663 2024-05-20 21:16:34.828595 cript-2.4.0/PKG-INFO
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5014 2024-05-20 21:09:59.000000 cript-2.4.0/README.md
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      346 2023-08-30 00:21:45.000000 cript-2.4.0/pyproject.toml
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      764 2024-05-20 21:16:34.828595 cript-2.4.0/setup.cfg
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)       69 2023-08-30 00:21:45.000000 cript-2.4.0/setup.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.820595 cript-2.4.0/src/
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.820595 cript-2.4.0/src/cript/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      849 2024-03-25 21:02:04.000000 cript-2.4.0/src/cript/__init__.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.824595 cript-2.4.0/src/cript/api/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      219 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/api/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    40993 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/api/api.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      316 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/api/api_config.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9155 2024-04-05 18:16:05.000000 cript-2.4.0/src/cript/api/data_schema.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    10793 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/api/exceptions.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9907 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/api/paginator.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.824595 cript-2.4.0/src/cript/api/utils/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      137 2023-08-30 00:21:45.000000 cript-2.4.0/src/cript/api/utils/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1310 2024-02-21 00:00:01.000000 cript-2.4.0/src/cript/api/utils/aws_s3_utils.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1990 2023-08-30 00:21:45.000000 cript-2.4.0/src/cript/api/utils/get_host_token.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1302 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/api/utils/helper_functions.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8399 2024-02-21 21:14:12.000000 cript-2.4.0/src/cript/api/utils/save_helper.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2806 2023-09-11 22:06:53.000000 cript-2.4.0/src/cript/api/utils/web_file_downloader.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1035 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/api/valid_search_modes.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     3006 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/api/vocabulary_categories.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      447 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/exceptions.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.824595 cript-2.4.0/src/cript/nodes/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      615 2024-03-25 21:02:04.000000 cript-2.4.0/src/cript/nodes/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    28077 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/nodes/core.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    14438 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/nodes/exceptions.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2296 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/node_iterator.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.824595 cript-2.4.0/src/cript/nodes/primary_nodes/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      617 2023-08-30 00:21:45.000000 cript-2.4.0/src/cript/nodes/primary_nodes/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9735 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/primary_nodes/collection.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    15136 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/primary_nodes/computation.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    19300 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/nodes/primary_nodes/computation_process.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    20789 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/primary_nodes/data.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    14052 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/primary_nodes/experiment.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     4825 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/primary_nodes/inventory.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    21847 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/nodes/primary_nodes/material.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2891 2023-08-30 00:21:45.000000 cript-2.4.0/src/cript/nodes/primary_nodes/primary_base_node.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    21199 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/nodes/primary_nodes/process.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8566 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/nodes/primary_nodes/project.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    19736 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/primary_nodes/reference.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.824595 cript-2.4.0/src/cript/nodes/subobjects/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      683 2023-08-30 00:21:45.000000 cript-2.4.0/src/cript/nodes/subobjects/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9286 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/algorithm.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8103 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/citation.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    17261 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/computational_forcefield.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    16294 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/condition.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    10346 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/equipment.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     7580 2024-04-05 18:16:05.000000 cript-2.4.0/src/cript/nodes/subobjects/ingredient.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     6017 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/parameter.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    24293 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/nodes/subobjects/property.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     7819 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/quantity.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5126 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/software.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9502 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/subobjects/software_configuration.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.824595 cript-2.4.0/src/cript/nodes/supporting_nodes/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      132 2023-08-30 00:21:45.000000 cript-2.4.0/src/cript/nodes/supporting_nodes/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    16377 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/supporting_nodes/file.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     4439 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/supporting_nodes/user.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.828595 cript-2.4.0/src/cript/nodes/util/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      234 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/util/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     3664 2024-05-20 21:09:59.000000 cript-2.4.0/src/cript/nodes/util/core.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    18567 2024-04-24 16:22:05.000000 cript-2.4.0/src/cript/nodes/util/json.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2886 2024-04-01 16:46:26.000000 cript-2.4.0/src/cript/nodes/uuid_base.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.828595 cript-2.4.0/src/cript.egg-info/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5663 2024-05-20 21:16:34.000000 cript-2.4.0/src/cript.egg-info/PKG-INFO
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2139 2024-05-20 21:16:34.000000 cript-2.4.0/src/cript.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)        1 2024-05-20 21:16:34.000000 cript-2.4.0/src/cript.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)       68 2024-05-20 21:16:34.000000 cript-2.4.0/src/cript.egg-info/requires.txt
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)        6 2024-05-20 21:16:34.000000 cript-2.4.0/src/cript.egg-info/top_level.txt
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-05-20 21:16:34.828595 cript-2.4.0/tests/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    15315 2024-05-20 21:09:59.000000 cript-2.4.0/tests/test_node_util.py
```

### Comparing `cript-2.3.0/LICENSE.md` & `cript-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/PKG-INFO` & `cript-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: cript
-Version: 2.3.0
+Version: 2.4.0
 Summary: CRIPT Python SDK
 Home-page: https://github.com/C-Accel-CRIPT/Python-SDK
 Author: CRIPT Development Team
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests==2.31.0
 Requires-Dist: jsonschema>=4.17.3
 Requires-Dist: beartype==0.14.1
 Requires-Dist: boto3==1.28.39
 
 # CRIPT Python SDK
 
 [![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
 
 [![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/Language-Python%203.10+-blue?style=flat-square&logo=python)](https://www.python.org/)
 [![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
 [![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
 [![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
 [![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
 [![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
 [![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
 
@@ -53,15 +53,15 @@
 
 The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
 
 ---
 
 ## Installation
 
-CRIPT Python SDK requires Python 3.8+
+CRIPT Python SDK requires Python 3.10+
 
 The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
 
 ```bash
 pip install cript
 ```
```

### Comparing `cript-2.3.0/README.md` & `cript-2.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # CRIPT Python SDK
 
 [![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
 
 [![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/Language-Python%203.10+-blue?style=flat-square&logo=python)](https://www.python.org/)
 [![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
 [![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
 [![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
 [![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
 [![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
 [![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
 
@@ -32,15 +32,15 @@
 
 The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
 
 ---
 
 ## Installation
 
-CRIPT Python SDK requires Python 3.8+
+CRIPT Python SDK requires Python 3.10+
 
 The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
 
 ```bash
 pip install cript
 ```
```

### Comparing `cript-2.3.0/setup.cfg` & `cript-2.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [metadata]
 name = cript
-version = 2.3.0
+version = 2.4.0
 description = CRIPT Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = CRIPT Development Team
 url = https://github.com/C-Accel-CRIPT/Python-SDK
 license = MIT
 license_files = LICENSE.md
 platforms = any
 classifiers = 
 	Development Status :: 3 - Alpha
 	Topic :: Scientific/Engineering
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.10
 
 [options]
 package_dir = 
 	=src
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.10
 include_package_data = True
 install_requires = 
 	requests==2.31.0
 	jsonschema>=4.17.3
 	beartype==0.14.1
 	boto3==1.28.39
```

### Comparing `cript-2.3.0/src/cript/__init__.py` & `cript-2.4.0/src/cript/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/api.py` & `cript-2.4.0/src/cript/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,17 @@
             The configured logger instance.
         """
         # Create a logger instance associated with the current module
         logger = logging.getLogger(__name__)
 
         logger.setLevel(log_level)
 
+        # Activate Warning handling
+        logging.captureWarnings(True)
+
         # Create a console handler
         console_handler = logging.StreamHandler()
 
         # Create a formatter for log messages (customize the format as desired)
         formatter = logging.Formatter("%(levelname)s: %(message)s")
 
         # Associate the formatter with the console handler
@@ -780,43 +783,40 @@
         [paginator object documentation](../paginator).
         """
 
         # get node typ from class
         node_type = node_type.node_type_snake_case
 
         api_endpoint: str = ""
-        page_number: Union[int, None] = None
-
+        limit_node_fetches: Optional[int] = None
         if search_mode == SearchModes.NODE_TYPE:
             api_endpoint = f"/search/{node_type}"
-            page_number = 0
+            value_to_search = ""
 
         elif search_mode == SearchModes.CONTAINS_NAME:
             api_endpoint = f"/search/{node_type}"
-            page_number = 0
 
         elif search_mode == SearchModes.EXACT_NAME:
             api_endpoint = f"/search/exact/{node_type}"
-            page_number = None
+            limit_node_fetches = 1
 
         elif search_mode == SearchModes.UUID:
             api_endpoint = f"/{node_type}/{value_to_search}"
             # putting the value_to_search in the URL instead of a query
             value_to_search = ""
-            page_number = None
+            limit_node_fetches = 1
 
         elif search_mode == SearchModes.BIGSMILES:
             api_endpoint = "/search/bigsmiles/"
-            page_number = 0
 
         # error handling if none of the API endpoints got hit
         else:
             raise RuntimeError("Internal Error: Failed to recognize any search modes. Please report this bug on https://github.com/C-Accel-CRIPT/Python-SDK/issues.")
 
-        return Paginator(api=self, url_path=api_endpoint, page_number=page_number, query=value_to_search)
+        return Paginator(api=self, url_path=api_endpoint, query=value_to_search, limit_node_fetches=limit_node_fetches)
 
     def delete(self, node) -> None:
         """
         Simply deletes the desired node from the CRIPT API and writes a log in the terminal that the node has been
         successfully deleted.
 
         Examples
```

### Comparing `cript-2.3.0/src/cript/api/data_schema.py` & `cript-2.4.0/src/cript/api/data_schema.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/exceptions.py` & `cript-2.4.0/src/cript/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/paginator.py` & `cript-2.4.0/src/cript/api/paginator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import json
-from typing import Dict, Union
+from typing import Dict, Optional, Tuple
 from urllib.parse import quote
 
 import requests
 from beartype import beartype
 
 from cript.api.exceptions import APIError
 from cript.nodes.util import load_nodes_from_json
 
 
+def _get_uuid_score_from_json(node_dict: Dict) -> Tuple[str, Optional[float]]:
+    """
+    Get the UUID string and search score from a JSON node representation if available.
+    """
+    node_uuid: str = node_dict["uuid"]
+    node_score: Optional[float] = node_dict.get("score", None)
+
+    return node_uuid, node_score
+
+
 class Paginator:
     """
     Paginator is used to flip through different pages of data that the API returns when searching.
     > Instead of the user manipulating the URL and parameters, this object handles all of that for them.
 
     Using the Paginator object, the user can simply and easily flip through the results of the search.
     The details, that results are listed as pages are hidden from the user.
@@ -25,66 +35,60 @@
         Please note that you are not required or advised to create a paginator object, and instead the
         Python SDK API object will create a paginator for you, return it, and let you simply use it
 
     """
 
     _url_path: str
     _query: str
-    _initial_page_number: Union[int, None]
     _current_position: int
     _fetched_nodes: list
+    _uuid_search_score_map: Dict
     _number_fetched_pages: int = 0
-    _limit_page_fetches: Union[int, None] = None
-    _num_skip_pages: int = 0
+    _limit_node_fetches: Optional[int] = None
+    _start_after_uuid: Optional[str] = None
+    _start_after_score: Optional[float] = None
     auto_load_nodes: bool = True
 
     @beartype
-    def __init__(
-        self,
-        api,
-        url_path: str,
-        page_number: Union[int, None],
-        query: str,
-    ):
+    def __init__(self, api, url_path: str, query: str, limit_node_fetches: Optional[int] = None):
         """
         create a paginator
 
         1. set all the variables coming into constructor
         1. then prepare any variable as needed e.g. strip extra spaces or url encode query
 
         Parameters
         ----------
-        http_headers: dict
-            get already created http headers from API and just use them in paginator
-        api_endpoint: str
-            api endpoint to send the search requests to
-            it already contains what node the user is looking for
-        current_page_number: int
-            page number to start from. Keep track of current page for user to flip back and forth between pages of data
+        api: cript.API
+           Object through which the API call is routed.
+        url_path: str
+            query URL used.
         query: str
             the value the user is searching for
+        limit_node_fetches: Optional[int] = None
+            limits the number of nodes fetches through this call.
 
         Returns
         -------
         None
             instantiate a paginator
         """
         self._api = api
-        self._initial_page_number = page_number
-        self._number_fetched_pages = 0
         self._fetched_nodes = []
         self._current_position = 0
+        self._limit_node_fetches = limit_node_fetches
+        self._uuid_search_score_map = {}
 
         # check if it is a string and not None to avoid AttributeError
         try:
-            self._url_path = quote(url_path.rstrip("/").strip())
+            self._url_path = url_path.rstrip("/").strip()
         except Exception as exc:
             raise RuntimeError(f"Invalid type for api_endpoint {self._url_path} for a paginator.") from exc
 
-        self._query = quote(query)
+        self._query = query
 
     @beartype
     def _fetch_next_page(self) -> None:
         """
         1. builds the URL from the query and page number
         1. makes the request to the API
         1. API responds with a JSON that has data or JSON that has data and result
@@ -101,24 +105,44 @@
 
 
         Returns
         -------
              None
         """
 
-        # Check if we are supposed to fetch more pages
-        if self._limit_page_fetches and self._number_fetched_pages >= self._limit_page_fetches:
-            raise StopIteration
-
         # Composition of the query URL
-        temp_url_path: str = self._url_path
-        temp_url_path += f"/?q={self._query}"
-        if self._initial_page_number is not None:
-            temp_url_path += f"&page={self.page_number}"
-        self._number_fetched_pages += 1
+        temp_url_path: str = self._url_path + "/"
+
+        query_list = []
+
+        if len(self._query) > 0:
+            query_list += [f"q={self._query}"]
+
+        if self._limit_node_fetches is None or self._limit_node_fetches > 1:  # This limits these parameters
+            if self._start_after_uuid is not None:
+                query_list += [f"after={self._start_after_uuid}"]
+                if self._start_after_score is not None:  # Always None for none BigSMILES searches
+                    query_list += [f"score={self._start_after_score}"]
+
+                # Reset to allow normal search to continue
+                self._start_after_uuid = None
+                self._start_after_score = None
+
+            elif len(self._fetched_nodes) > 0:  # Use known last element
+                node_uuid, node_score = _get_uuid_score_from_json(self._fetched_nodes[-1])
+                query_list += [f"after={node_uuid}"]
+                if node_score is not None:
+                    query_list += [f"score={node_score}"]
+
+        for i, query in enumerate(query_list):
+            if i == 0:
+                temp_url_path += "?"
+            else:
+                temp_url_path += "&"
+            temp_url_path += quote(query, safe="/=&?")
 
         response: requests.Response = self._api._capsule_request(url_path=temp_url_path, method="GET")
 
         # it is expected that the response will be JSON
         # try to convert response to JSON
         try:
             api_response: Dict = response.json()
@@ -149,26 +173,26 @@
 
         # Here we only load the JSON into the temporary results.
         # This delays error checking, and allows users to disable auto node conversion
         json_list = current_page_results
         self._fetched_nodes += json_list
 
     def __next__(self):
+        if self._limit_node_fetches and self._current_position >= self._limit_node_fetches:
+            raise StopIteration
+
         if self._current_position >= len(self._fetched_nodes):
-            # Without a page number argument, we can only fetch once.
-            if self._initial_page_number is None and self._number_fetched_pages > 0:
-                raise StopIteration
             self._fetch_next_page()
 
         try:
             next_node_json = self._fetched_nodes[self._current_position - 1]
-        except IndexError:  # This is not a random access iteration.
+        except IndexError as exc:  # This is not a random access iteration.
             # So if fetching a next page wasn't enough to get the index inbound,
             # The iteration stops
-            raise StopIteration
+            raise StopIteration from exc
 
         if self.auto_load_nodes:
             return_data = load_nodes_from_json(next_node_json)
         else:
             return_data = next_node_json
 
         # Advance position last, so if an exception occurs, for example when
@@ -177,69 +201,57 @@
 
         return return_data
 
     def __iter__(self):
         self._current_position = 0
         return self
 
-    @property
-    def page_number(self) -> Union[int, None]:
-        """Obtain the current page number the paginator is fetching next.
-
-        Returns
-        -------
-        int
-          positive number of the next page this paginator is fetching.
-        None
-          if no page number is associated with the pagination
-        """
-        page_number = self._num_skip_pages + self._number_fetched_pages
-        if self._initial_page_number is not None:
-            page_number += self._initial_page_number
-        return page_number
-
     @beartype
-    def limit_page_fetches(self, max_num_pages: Union[int, None]) -> None:
+    def limit_node_fetches(self, max_num_nodes: Optional[int]) -> None:
         """Limit pagination to a maximum number of pages.
 
         This can be used for very large searches with the paginator, so the search can be split into
         smaller portions.
 
         Parameters
         ----------
-        max_num_pages: Union[int, None],
+        max_num_nodes: Optional[int],
           positive integer with maximum number of page fetches.
           or None, indicating unlimited number of page fetches are permitted.
         """
-        self._limit_page_fetches = max_num_pages
+        self._limit_node_fetches = max_num_nodes
 
-    def skip_pages(self, skip_pages: int) -> int:
-        """Skip pages in the pagination.
-
-        Warning this function is advanced usage and may not produce the results you expect.
-        In particular, every search is different, even if we search for the same values there is
-        no guarantee that the results are in the same order. (And results can change if data is
-        added or removed from CRIPT.) So if you break up your search with `limit_page_fetches` and
-        `skip_pages` there is no guarantee that it is the same as one continuous search.
-        If the paginator associated search does not accept pages, there is no effect.
+    @beartype
+    def start_after_uuid(self, start_after_uuid: str, start_after_score: Optional[float] = None):
+        """
+        This can be used to continue a search from a last known node.
 
         Parameters
         ----------
-        skip_pages:int
-          Number of pages that the paginator skips now before fetching the next page.
-          The parameter is added to the internal state, so repeated calls skip more pages.
+        start_after_uuid: str
+            UUID string of the last node from a previous search
+        start_after_score: float
+            required for BigSMILES searches, the last score from a BigSMILES search.
+            Must be None if not a BigSMILES search.
 
         Returns
         -------
-        int
-          The number this paginator is skipping. Internal skip count.
+        None
+        """
+        self._start_after_uuid = start_after_uuid
+        self._start_after_score = start_after_score
 
-        Raises
-        ------
-        RuntimeError
-          If the total number of skipped pages is negative.
+    @beartype
+    def get_bigsmiles_search_score(self, uuid: str):
+        """
+        Get the ranking score for nodes from the BigSMILES search.
+        Will return None if not a BigSMILES search or raise an Exception.
         """
-        num_skip_pages = self._num_skip_pages + skip_pages
-        if self._num_skip_pages < 0:
-            RuntimeError(f"Invalid number of skipped pages. The total number of pages skipped is negative {num_skip_pages}, requested to skip {skip_pages}.")
-        self._num_skip_pages = num_skip_pages
-        return self._num_skip_pages
+        if uuid not in self._uuid_search_score_map.keys():
+            start = len(self._uuid_search_score_map.keys())
+            for node_json in self._fetched_nodes[start:]:
+                node_uuid, node_score = _get_uuid_score_from_json(node_json)
+                self._uuid_search_score_map[node_uuid] = node_score
+        try:
+            return self._uuid_search_score_map[uuid]
+        except KeyError as exc:
+            raise RuntimeError(f"The requested UUID {uuid} is not know from the search. Search scores are limited only to current search.") from exc
```

### Comparing `cript-2.3.0/src/cript/api/utils/aws_s3_utils.py` & `cript-2.4.0/src/cript/api/utils/aws_s3_utils.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/utils/get_host_token.py` & `cript-2.4.0/src/cript/api/utils/get_host_token.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/utils/helper_functions.py` & `cript-2.4.0/src/cript/api/utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/utils/save_helper.py` & `cript-2.4.0/src/cript/api/utils/save_helper.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/utils/web_file_downloader.py` & `cript-2.4.0/src/cript/api/utils/web_file_downloader.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/valid_search_modes.py` & `cript-2.4.0/src/cript/api/valid_search_modes.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/api/vocabulary_categories.py` & `cript-2.4.0/src/cript/api/vocabulary_categories.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/__init__.py` & `cript-2.4.0/src/cript/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/core.py` & `cript-2.4.0/src/cript/nodes/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,18 @@
         for field in json_dict:
             try:
                 getattr(default_dataclass, field)
             except AttributeError:
                 pass
             else:
                 arguments[field] = json_dict[field]
+        try:  # TODO remove this hack to work with compatible model versions
+            del arguments["model_version"]
+        except KeyError:
+            pass
 
         # add omitted fields from default (necessary if they are required)
         for field_name in [field.name for field in dataclasses.fields(default_dataclass)]:
             if field_name not in arguments:
                 arguments[field_name] = getattr(default_dataclass, field_name)
 
         try:
```

### Comparing `cript-2.3.0/src/cript/nodes/exceptions.py` & `cript-2.4.0/src/cript/nodes/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import List
 
-from cript.exceptions import CRIPTException
+from cript.exceptions import CRIPTException, CRIPTWarning
 
 
 class CRIPTUUIDException(CRIPTException):
     def __init__(self, uuid: str, old_type: str, new_type: str):
         self.uuid = uuid
         self.old_type = old_type
         self.new_type = new_type
@@ -63,15 +63,15 @@
     def __str__(self) -> str:
         error_message: str = f"JSON database schema validation for node {self.node_type} failed."
         error_message += f"Error: {self.json_schema_validation_error}"
 
         return error_message
 
 
-class CRIPTMaterialIdentifierError(CRIPTException):
+class CRIPTMaterialIdentifierWarning(CRIPTWarning):
     """Every material node needs to have at least one identifier set."""
 
     def __init__(self, material_node):
         self.material_node = material_node
 
     def __str__(self) -> str:
         error_message = "Every Material node needs at least one identifier from "
@@ -277,22 +277,22 @@
         return (
             f"During the construction of a node {self.name_type} an additional attribute {self.extra_attribute} was detected.\n"
             "This might be a typo or an extra delivered argument from the back end.\n"
             f"In the latter case, you can disable this error temporarily by calling `cript.add_tolerated_extra_json('{self.extra_attribute}')`.\n"
         )
 
 
-class CRIPTOrphanedNodesError(CRIPTException, ABC):
+class CRIPTOrphanedNodesWarning(CRIPTWarning, ABC):
     """
     ## Definition
     This error is raised when a child node is not attached to the
     appropriate parent node. For example, all material nodes used
     within a project must belong to the project inventory or are explicitly listed as material of that project.
     If there is a material node that is used within a project but not a part of the
-    inventory and the validation code finds it then it raises an `CRIPTOrphanedNodeError`
+    inventory and the validation code finds it then it raises an `CRIPTOrphanedNodeWarning`
 
     ## Troubleshooting
     Fixing this is simple and easy, just take the node that CRIPT Python SDK
     found a problem with and associate it with the appropriate parent via
 
     ```
     my_project.material += my_orphaned_material_node
@@ -303,18 +303,18 @@
         self.orphaned_node = orphaned_node
 
     @abstractmethod
     def __str__(self):
         pass
 
 
-class CRIPTOrphanedMaterialError(CRIPTOrphanedNodesError):
+class CRIPTOrphanedMaterialWarning(CRIPTOrphanedNodesWarning):
     """
     ## Definition
-    CRIPTOrphanedNodesError, but specific for orphaned materials.
+    CRIPTOrphanedNodesWarning, but specific for orphaned materials.
 
     ## Troubleshooting
     Handle this error by adding the orphaned materials into the parent project or its inventories.
     """
 
     def __init__(self, orphaned_node):
         super().__init__(orphaned_node)
@@ -323,18 +323,18 @@
         ret_string = "While validating a project graph, an orphaned material node was found. "
         ret_string += "This material is present in the graph, but not listed in the project. "
         ret_string += "Please add the node like: `my_project.material += [orphaned_material]`. "
         ret_string += f"The orphaned material was {self.orphaned_node}."
         return ret_string
 
 
-class CRIPTOrphanedExperimentError(CRIPTOrphanedNodesError):
+class CRIPTOrphanedExperimentWarning(CRIPTOrphanedNodesWarning):
     """
     ## Definition
-    CRIPTOrphanedNodesError, but specific for orphaned nodes that should be listed in one of the experiments.
+    CRIPTOrphanedNodesWarning, but specific for orphaned nodes that should be listed in one of the experiments.
 
     ## Troubleshooting
     Handle this error by adding the orphaned node into one the parent project's experiments.
     """
 
     def __init__(self, orphaned_node):
         super().__init__(orphaned_node)
@@ -344,61 +344,61 @@
         ret_string = f"While validating a project graph, an orphaned {node_name} node was found. "
         ret_string += f"This {node_name} node is present in the graph, but not listed in any of the experiments of the  project. "
         ret_string += f"Please add the node like: `your_experiment.{node_name} += [orphaned_{node_name}]`. "
         ret_string += f"The orphaned {node_name} was {self.orphaned_node}."
         return ret_string
 
 
-class CRIPTOrphanedDataError(CRIPTOrphanedExperimentError):
+class CRIPTOrphanedDataWarning(CRIPTOrphanedExperimentWarning):
     """
     ## Definition
-    CRIPTOrphanedExperimentError, but specific for orphaned Data node that should be listed in one of the experiments.
+    CRIPTOrphanedExperimentWarning, but specific for orphaned Data node that should be listed in one of the experiments.
 
     ## Troubleshooting
     Handle this error by adding the orphaned node into one the parent project's experiments `data` attribute.
     """
 
     def __init__(self, orphaned_node):
         super().__init__(orphaned_node)
 
 
-class CRIPTOrphanedProcessError(CRIPTOrphanedExperimentError):
+class CRIPTOrphanedProcessWarning(CRIPTOrphanedExperimentWarning):
     """
     ## Definition
-    CRIPTOrphanedExperimentError, but specific for orphaned Process node that should be
+    CRIPTOrphanedExperimentWarning, but specific for orphaned Process node that should be
     listed in one of the experiments.
 
     ## Troubleshooting
     Handle this error by adding the orphaned node into one the parent project's experiments
     `process` attribute.
     """
 
     def __init__(self, orphaned_node):
         super().__init__(orphaned_node)
 
 
-class CRIPTOrphanedComputationError(CRIPTOrphanedExperimentError):
+class CRIPTOrphanedComputationWarning(CRIPTOrphanedExperimentWarning):
     """
     ## Definition
-    CRIPTOrphanedExperimentError, but specific for orphaned Computation node that should be
+    CRIPTOrphanedExperimentWarning, but specific for orphaned Computation node that should be
     listed in one of the experiments.
 
     ## Troubleshooting
     Handle this error by adding the orphaned node into one the parent project's experiments
     `Computation` attribute.
     """
 
     def __init__(self, orphaned_node):
         super().__init__(orphaned_node)
 
 
-class CRIPTOrphanedComputationalProcessError(CRIPTOrphanedExperimentError):
+class CRIPTOrphanedComputationalProcessWarning(CRIPTOrphanedExperimentWarning):
     """
     ## Definition
-    CRIPTOrphanedExperimentError, but specific for orphaned ComputationalProcess
+    CRIPTOrphanedExperimentWarning, but specific for orphaned ComputationalProcess
     node that should be listed in one of the experiments.
 
     ## Troubleshooting
     Handle this error by adding the orphaned node into one the parent project's experiments
     `ComputationalProcess` attribute.
     """
```

### Comparing `cript-2.3.0/src/cript/nodes/node_iterator.py` & `cript-2.4.0/src/cript/nodes/node_iterator.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/__init__.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/collection.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/collection.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/computation.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/computation.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/computation_process.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/computation_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
     def property(self) -> List[Any]:
         """
         List of properties
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="modulus_shear", type="min", value=1.23, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.23, unit="J")
         >>> my_computation_process.property = [my_property]     # doctest: +SKIP
 
         Returns
         -------
         List[Property]
             list of properties for this computational process node
         """
```

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/data.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/data.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/experiment.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/experiment.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/inventory.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/inventory.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/material.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/material.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import warnings
 from dataclasses import dataclass, field, replace
 from typing import Any, List, Optional, Union
 
 from beartype import beartype
 
-from cript.nodes.exceptions import CRIPTMaterialIdentifierError
+from cript.nodes.exceptions import CRIPTMaterialIdentifierWarning
 from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
 from cript.nodes.primary_nodes.process import Process
 from cript.nodes.util.json import UIDProxy
 
 
 class Material(PrimaryBaseNode):
     """
@@ -214,15 +215,15 @@
             and self.inchi is None
             and self.lot_number is None
             and len(self.names) == 0
             and self.pubchem_cid is None
             and self.smiles is None
             and self.vendor is None
         ):
-            raise CRIPTMaterialIdentifierError(self)
+            warnings.warn(CRIPTMaterialIdentifierWarning(self))
 
     @property
     @beartype
     def amino_acid(self) -> Union[str, None]:
         return self._json_attrs.amino_acid
 
     @amino_acid.setter
@@ -535,15 +536,15 @@
         Examples
         --------
         >>> import cript
         >>> my_material = cript.Material(
         ...     name="my component material 1",
         ...     smiles = "component 1 smiles",
         ... )
-        >>> my_property = cript.Property(key="modulus_shear", type="min", value=1.23, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.23, unit="J")
         >>> my_material.property = [my_property]
 
         Returns
         -------
         List[Property]
             list of property that define this material
         """
```

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/primary_base_node.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/primary_base_node.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/process.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,15 +576,15 @@
         """
         List of [Property nodes](../../subobjects/property) for this process
 
         Examples
         --------
         >>> import cript
         >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_property = cript.Property(key="modulus_shear", type="min", value=1.23, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.23, unit="J")
         >>> my_process.property = [my_property]
 
         Returns
         -------
         List[Property]
             list of properties for this process
         """
```

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/project.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from dataclasses import dataclass, field, replace
 from typing import List, Optional, Union
 
 from beartype import beartype
 
 from cript.nodes.primary_nodes.collection import Collection
 from cript.nodes.primary_nodes.material import Material
@@ -102,15 +103,15 @@
         if material is None:
             material = []
 
         new_json_attrs = replace(self._json_attrs, name=name, collection=collection, material=material)
         self._update_json_attrs_if_valid(new_json_attrs)
 
     def validate(self, api=None, is_patch=False, force_validation: bool = False):
-        from cript.nodes.exceptions import CRIPTOrphanedMaterialError
+        from cript.nodes.exceptions import CRIPTOrphanedMaterialWarning
         from cript.nodes.util.core import get_orphaned_experiment_exception
 
         # First validate like other nodes
         super().validate(api=api, is_patch=is_patch, force_validation=force_validation)
 
         # Check graph for orphaned nodes, that should be listed in project
         # Project.materials should contain all material nodes
@@ -118,15 +119,15 @@
         # Combine all materials listed in the project inventories
         project_inventory_materials = []
         for inventory in self.find_children({"node": ["Inventory"]}):
             for material in inventory.material:
                 project_inventory_materials.append(material)
         for material in project_graph_materials:
             if material not in self.material and material not in project_inventory_materials:
-                raise CRIPTOrphanedMaterialError(material)
+                warnings.warn(CRIPTOrphanedMaterialWarning(material))
 
         # Check graph for orphaned nodes, that should be listed in the experiments
         project_experiments = self.find_children({"node": ["Experiment"]})
         # There are 4 different types of nodes Experiments are collecting.
         node_types = ("Process", "Computation", "ComputationProcess", "Data")
         # We loop over them with the same logic
         for node_type in node_types:
@@ -141,15 +142,15 @@
             # Every node of the graph must be present somewhere in this concatenated list.
             experiment_nodes = []
             for experiment in project_experiments:
                 for ex_node in getattr(experiment, node_type_attr):
                     experiment_nodes.append(ex_node)
             for node in project_graph_nodes:
                 if node not in experiment_nodes:
-                    raise get_orphaned_experiment_exception(node)
+                    warnings.warn(get_orphaned_experiment_exception(node))
 
     @property
     @beartype
     def member(self) -> List[Union[User, UIDProxy]]:
         return self._json_attrs.member.copy()
 
     @property
```

### Comparing `cript-2.3.0/src/cript/nodes/primary_nodes/reference.py` & `cript-2.4.0/src/cript/nodes/primary_nodes/reference.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/__init__.py` & `cript-2.4.0/src/cript/nodes/subobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/algorithm.py` & `cript-2.4.0/src/cript/nodes/subobjects/algorithm.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/citation.py` & `cript-2.4.0/src/cript/nodes/subobjects/citation.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/computational_forcefield.py` & `cript-2.4.0/src/cript/nodes/subobjects/computational_forcefield.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/condition.py` & `cript-2.4.0/src/cript/nodes/subobjects/condition.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/equipment.py` & `cript-2.4.0/src/cript/nodes/subobjects/equipment.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/ingredient.py` & `cript-2.4.0/src/cript/nodes/subobjects/ingredient.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/parameter.py` & `cript-2.4.0/src/cript/nodes/subobjects/parameter.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/property.py` & `cript-2.4.0/src/cript/nodes/subobjects/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     ---
 
     ## Attributes
 
     | attribute          | type              | example                                 | description                                                                  | required | vocab |
     |--------------------|-------------------|-----------------------------------------|------------------------------------------------------------------------------|----------|-------|
-    | key                | str               | modulus_shear                           | type of property                                                             | True     | True  |
+    | key                | str               | enthalpy                                | type of property                                                             | True     | True  |
     | type               | str               | min                                     | type of value stored                                                         | True     | True  |
     | value              | Any               | 1.23                                    | value or quantity                                                            | True     |       |
     | unit               | str               | gram                                    | unit for value                                                               | True     |       |
     | uncertainty        | Number            | 0.1                                     | uncertainty of value                                                         |          |       |
     | uncertainty_type   | str               | standard_deviation                      | type of uncertainty                                                          |          | True  |
     | component          | list[Material]    |                                         | material that the property relates to**                                      |          |       |
     | structure          | str               | {\\[\\]\\[$\\]\\[C:1\\]\\[C:1\\]\\[$\\] | specific chemical structure associate with the property with atom mappings** |          |       |
@@ -54,18 +54,18 @@
     | citation           | list[Citation]    |                                         | reference to a book, paper, or scholarly work                                |          |       |
     | notes              | str               |                                         | miscellaneous information, or custom data structure (e.g.; JSON)             |          |       |
 
 
     ## JSON Representation
     ```json
     {
-       "key":"modulus_shear",
+       "key":"enthalpy",
        "node":["Property"],
        "type":"value",
-       "unit":"GPa",
+       "unit":"J",
        "value":5.0
        "uid":"_:bc3abb68-25b5-4144-aa1b-85d82b7c77e1",
        "uuid":"bc3abb68-25b5-4144-aa1b-85d82b7c77e1",
     }
     ```
     """
 
@@ -145,15 +145,15 @@
         notes : str, optional
             miscellaneous information, or custom data structure (e.g.; JSON), by default ""
 
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
 
         Returns
         -------
         None
             create a Property sub-object
         """
         if component is None:
@@ -193,15 +193,15 @@
     def key(self) -> str:
         """
         Property key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/)
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_property.key = "angle_rdist"
 
         Returns
         -------
         str
             Property Key
         """
@@ -232,15 +232,15 @@
         type of value for this Property sub-object
 
         [property type](https://app.criptapp.org/vocab/) must come from CRIPT controlled vocabulary
 
         Examples
         ---------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_property.type = "max"
 
         Returns
         -------
         str
             type of value for this Property sub-object
         """
@@ -281,15 +281,15 @@
     def set_value(self, new_value: Union[Number, str, None], new_unit: str) -> None:
         """
         set the value attribute of the Property subobject
 
         Examples
         ---------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_property.set_value(new_value=1, new_unit="gram")
 
         Parameters
         ----------
         new_value : Number
             new value
         new_unit : str
@@ -341,15 +341,15 @@
             new uncertainty value
         new_uncertainty_type : str
             new uncertainty type
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_property.set_uncertainty(new_uncertainty=2, new_uncertainty_type="fwhm")
 
         Returns
         -------
         None
         """
         new_attrs = replace(self._json_attrs, uncertainty=new_uncertainty, uncertainty_type=new_uncertainty_type)
@@ -376,15 +376,15 @@
     def component(self) -> List[Union[Material, UIDProxy]]:
         """
         list of Materials that the Property relates to
 
         Examples
         ---------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_material = cript.Material(name="my material", bigsmiles = "123456")
         >>> my_property.component = [my_material]
 
         Returns
         -------
         List[Material]
             list of Materials that the Property relates to
@@ -414,15 +414,15 @@
     def structure(self) -> str:
         """
         specific chemical structure associate with the property with atom mappings
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_property.structure = "{[][$][C:1][C:1][$],[$][C:2][C:2]([C:2])[$][]}"
 
         Returns
         -------
         str
             Property structure string
         """
@@ -453,15 +453,15 @@
         approach or source of property data True sample_preparation Process sample preparation
 
         [Property method](https://app.criptapp.org/vocab/property_method) must come from CRIPT Controlled Vocabulary
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_property.method = "ASTM_D3574_Test_A"
 
         Returns
         -------
         str
             Property method
         """
@@ -490,15 +490,15 @@
     def sample_preparation(self) -> Union[Process, None, UIDProxy]:
         """
         sample_preparation
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_process = cript.Process(name="my process name", type="affinity_pure")
         >>> my_property.sample_preparation = my_process
 
         Returns
         -------
         Union[Process, None]
             Property linking back to the Process that has it as subobject
@@ -528,15 +528,15 @@
     def condition(self) -> List[Union[Condition, UIDProxy]]:
         """
         list of Conditions under which the property was measured
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_condition = cript.Condition(key="atm", type="max", value=1)
         >>> my_property.condition = [my_condition]
 
         Returns
         -------
         List[Condition]
             list of Conditions
@@ -566,15 +566,15 @@
     def data(self) -> List[Union[Data, UIDProxy]]:
         """
         List of Data nodes for this Property subobjects
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_file = cript.File(
         ...     name="my file node name",
         ...     source="https://criptapp.org",
         ...     type="calibration",
         ...     extension=".csv",
         ...     data_dictionary="my file's data dictionary",
         ... )
@@ -611,15 +611,15 @@
     def computation(self) -> List[Union[Computation, UIDProxy]]:
         """
         list of Computation nodes that produced this property
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_computation = cript.Computation(name="my computation name", type="analysis")
         >>> my_property.computation = [my_computation]
 
         Returns
         -------
         List[Computation]
             list of Computation nodes
@@ -649,15 +649,15 @@
     def citation(self) -> List[Union[Citation, UIDProxy]]:
         """
         list of Citation subobjects for this Property subobject
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> title = (
         ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
         ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
         ... )
         >>> my_reference = cript.Reference(
         ...     type="journal_article",
         ...     title=title,
@@ -703,15 +703,15 @@
     def notes(self) -> str:
         """
         notes for this Property subobject
 
         Examples
         --------
         >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property = cript.Property(key="enthalpy", type="min", value=1.00, unit="J")
         >>> my_property.notes = "these are my notes"
 
         Returns
         -------
         str
             notes for this property subobject
         """
```

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/quantity.py` & `cript-2.4.0/src/cript/nodes/subobjects/quantity.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/software.py` & `cript-2.4.0/src/cript/nodes/subobjects/software.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/subobjects/software_configuration.py` & `cript-2.4.0/src/cript/nodes/subobjects/software_configuration.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/supporting_nodes/file.py` & `cript-2.4.0/src/cript/nodes/supporting_nodes/file.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/supporting_nodes/user.py` & `cript-2.4.0/src/cript/nodes/supporting_nodes/user.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/util/core.py` & `cript-2.4.0/src/cript/nodes/util/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import uuid
+import warnings
 
 from cript.nodes.exceptions import (
-    CRIPTOrphanedComputationalProcessError,
-    CRIPTOrphanedComputationError,
-    CRIPTOrphanedDataError,
-    CRIPTOrphanedExperimentError,
-    CRIPTOrphanedMaterialError,
-    CRIPTOrphanedProcessError,
+    CRIPTOrphanedComputationalProcessWarning,
+    CRIPTOrphanedComputationWarning,
+    CRIPTOrphanedDataWarning,
+    CRIPTOrphanedExperimentWarning,
+    CRIPTOrphanedMaterialWarning,
+    CRIPTOrphanedProcessWarning,
 )
 
 
 def get_uuid_from_uid(uid):
     return str(uuid.UUID(uid[2:]))
 
 
@@ -23,54 +24,57 @@
     of the project graph to the `active_experiment`.
     This functions call `project.validate` and might raise Exceptions from there.
     """
     if active_experiment is not None and active_experiment not in project.find_children({"node": ["Experiment"]}):
         raise RuntimeError(f"The provided active experiment {active_experiment} is not part of the project graph. Choose an active experiment that is part of a collection of this project.")
 
     counter = 0
-    while True:
-        if counter > max_iteration >= 0:
-            break  # Emergency stop
-        try:
-            project.validate()
-        except CRIPTOrphanedMaterialError as exc:
-            # because calling the setter calls `validate` we have to force add the material.
-            project._json_attrs.material.append(exc.orphaned_node)
-        except CRIPTOrphanedDataError as exc:
-            active_experiment.data += [exc.orphaned_node]
-        except CRIPTOrphanedProcessError as exc:
-            active_experiment.process += [exc.orphaned_node]
-        except CRIPTOrphanedComputationError as exc:
-            active_experiment.computation += [exc.orphaned_node]
-        except CRIPTOrphanedComputationalProcessError as exc:
-            active_experiment.computation_process += [exc.orphaned_node]
-        else:
-            break
-        counter += 1
+    # Convert Errors into exceptions, so we can catch and fix them
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        while True:
+            if counter > max_iteration >= 0:
+                break  # Emergency stop
+            try:
+                project.validate()
+            except CRIPTOrphanedMaterialWarning as exc:
+                # because calling the setter calls `validate` we have to force add the material.
+                project._json_attrs.material.append(exc.orphaned_node)
+            except CRIPTOrphanedDataWarning as exc:
+                active_experiment.data += [exc.orphaned_node]
+            except CRIPTOrphanedProcessWarning as exc:
+                active_experiment.process += [exc.orphaned_node]
+            except CRIPTOrphanedComputationWarning as exc:
+                active_experiment.computation += [exc.orphaned_node]
+            except CRIPTOrphanedComputationalProcessWarning as exc:
+                active_experiment.computation_process += [exc.orphaned_node]
+            else:
+                break
+            counter += 1
 
 
 def get_orphaned_experiment_exception(orphaned_node):
     """
     Return the correct specific Exception based in the orphaned node type for nodes not correctly listed in experiment.
     """
     from cript.nodes.primary_nodes.computation import Computation
     from cript.nodes.primary_nodes.computation_process import ComputationProcess
     from cript.nodes.primary_nodes.data import Data
     from cript.nodes.primary_nodes.process import Process
 
     if isinstance(orphaned_node, Data):
-        return CRIPTOrphanedDataError(orphaned_node)
+        return CRIPTOrphanedDataWarning(orphaned_node)
     if isinstance(orphaned_node, Process):
-        return CRIPTOrphanedProcessError(orphaned_node)
+        return CRIPTOrphanedProcessWarning(orphaned_node)
     if isinstance(orphaned_node, Computation):
-        return CRIPTOrphanedComputationError(orphaned_node)
+        return CRIPTOrphanedComputationWarning(orphaned_node)
     if isinstance(orphaned_node, ComputationProcess):
-        return CRIPTOrphanedComputationalProcessError(orphaned_node)
+        return CRIPTOrphanedComputationalProcessWarning(orphaned_node)
     # Base case raise the parent exception. TODO add bug warning.
-    return CRIPTOrphanedExperimentError(orphaned_node)
+    return CRIPTOrphanedExperimentWarning(orphaned_node)
 
 
 def iterate_leaves(obj):
     """Helper function that iterates over all leaves of nested dictionaries or lists."""
 
     if isinstance(obj, dict):
         for value in obj.values():
```

### Comparing `cript-2.3.0/src/cript/nodes/util/json.py` & `cript-2.4.0/src/cript/nodes/util/json.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript/nodes/uuid_base.py` & `cript-2.4.0/src/cript/nodes/uuid_base.py`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/src/cript.egg-info/PKG-INFO` & `cript-2.4.0/src/cript.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: cript
-Version: 2.3.0
+Version: 2.4.0
 Summary: CRIPT Python SDK
 Home-page: https://github.com/C-Accel-CRIPT/Python-SDK
 Author: CRIPT Development Team
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests==2.31.0
 Requires-Dist: jsonschema>=4.17.3
 Requires-Dist: beartype==0.14.1
 Requires-Dist: boto3==1.28.39
 
 # CRIPT Python SDK
 
 [![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
 
 [![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/Language-Python%203.10+-blue?style=flat-square&logo=python)](https://www.python.org/)
 [![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
 [![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
 [![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
 [![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
 [![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
 [![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
 
@@ -53,15 +53,15 @@
 
 The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
 
 ---
 
 ## Installation
 
-CRIPT Python SDK requires Python 3.8+
+CRIPT Python SDK requires Python 3.10+
 
 The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
 
 ```bash
 pip install cript
 ```
```

### Comparing `cript-2.3.0/src/cript.egg-info/SOURCES.txt` & `cript-2.4.0/src/cript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cript-2.3.0/tests/test_node_util.py` & `cript-2.4.0/tests/test_node_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import copy
 import json
+import warnings
 from dataclasses import replace
 
 import pytest
 
 import cript
 from cript.nodes.core import get_new_uid
 from cript.nodes.exceptions import (
     CRIPTJsonNodeError,
     CRIPTJsonSerializationError,
     CRIPTNodeSchemaError,
-    CRIPTOrphanedComputationalProcessError,
-    CRIPTOrphanedComputationError,
-    CRIPTOrphanedDataError,
-    CRIPTOrphanedMaterialError,
-    CRIPTOrphanedProcessError,
+    CRIPTOrphanedComputationalProcessWarning,
+    CRIPTOrphanedComputationWarning,
+    CRIPTOrphanedDataWarning,
+    CRIPTOrphanedMaterialWarning,
+    CRIPTOrphanedProcessWarning,
 )
 from tests.utils.util import strip_uid_from_dict
 
 
 def test_removing_nodes(simple_algorithm_node, complex_parameter_node, simple_algorithm_dict):
     a = simple_algorithm_node
     p = complex_parameter_node
@@ -28,16 +29,16 @@
     assert strip_uid_from_dict(json.loads(a.json)) == simple_algorithm_dict
 
 
 def test_uid_deserialization(simple_algorithm_node, complex_parameter_node, simple_algorithm_dict):
     material = cript.Material(name="my material", bigsmiles="{[][$]CC[$][]}")
 
     computation = cript.Computation(name="my computation name", type="analysis")
-    property1 = cript.Property("modulus_shear", "value", 5.0, "GPa", computation=[computation])
-    property2 = cript.Property("modulus_loss", "value", 5.0, "GPa", computation=[computation])
+    property1 = cript.Property("enthalpy", "value", 5.0, "GPa", computation=[computation])
+    property2 = cript.Property("rho_z", "value", 5.0, "GPa", computation=[computation])
     material.property = [property1, property2]
 
     material2 = cript.load_nodes_from_json(material.json)
     assert json.loads(material.json) == json.loads(material2.json)
 
     material3_dict = {
         "node": ["Material"],
@@ -45,25 +46,25 @@
         "uuid": "f6d56fdc-9df7-49a1-a843-cf92681932ad",
         "name": "my material",
         "property": [
             {
                 "node": ["Property"],
                 "uid": "_:82e7270e-9f35-4b35-80a2-faa6e7f670be",
                 "uuid": "82e7270e-9f35-4b35-80a2-faa6e7f670be",
-                "key": "modulus_shear",
+                "key": "enthalpy",
                 "type": "value",
                 "value": 5.0,
                 "unit": "GPa",
                 "computation": [{"uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef"}],
             },
             {
                 "node": ["Property"],
                 "uid": "_:fc4dfa5e-742c-4d0b-bb66-2185461f4582",
                 "uuid": "fc4dfa5e-742c-4d0b-bb66-2185461f4582",
-                "key": "modulus_loss",
+                "key": "rho_z",
                 "type": "value",
                 "value": 5.0,
                 "unit": "GPa",
                 "computation": [
                     {
                         "uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef",
                     }
@@ -87,15 +88,15 @@
     #     "property": [
     #         {
     #             "node": [
     #                 "Property"
     #             ],
     #             "uid": "_:82e7270e-9f35-4b35-80a2-faa6e7f670be",
     #             "uuid": "82e7270e-9f35-4b35-80a2-faa6e7f670be",
-    #             "key": "modulus_shear",
+    #             "key": "enthalpy",
     #             "type": "value",
     #             "value": 5.0,
     #             "unit": "GPa",
     #             "computation": [
     #                 {
     #                     "node": [
     #                         "Computation"
@@ -106,15 +107,15 @@
     #         },
     #         {
     #             "node": [
     #                 "Property"
     #             ],
     #             "uid": "_:fc4dfa5e-742c-4d0b-bb66-2185461f4582",
     #             "uuid": "fc4dfa5e-742c-4d0b-bb66-2185461f4582",
-    #             "key": "modulus_loss",
+    #             "key": "rho_z",
     #             "type": "value",
     #             "value": 5.0,
     #             "unit": "GPa",
     #             "computation": [
     #                 {
     #                     "node": [
     #                         "Computation"
@@ -241,83 +242,97 @@
 
     ingredient = cript.Ingredient(material=material, quantity=[cript.Quantity(key="mass", value=1.23, unit="kg")])
     process.ingredient += [ingredient]
 
     # Add the process to the experiment, but not in inventory or materials
     # Invalid graph
     project.collection[0].experiment[0].process += [process]
-    with pytest.raises(CRIPTOrphanedMaterialError):
+    with pytest.warns(CRIPTOrphanedMaterialWarning):
         project.validate()
 
     # First fix add material to inventory
     project.collection[0].inventory += [cript.Inventory("test_inventory", material=[material])]
-    project.validate()
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        project.validate()
     # Reverse this fix
     project.collection[0].inventory = []
-    with pytest.raises(CRIPTOrphanedMaterialError):
+    with pytest.warns(CRIPTOrphanedMaterialWarning):
         project.validate()
 
     # Fix by add to the materials list instead.
     # Using the util helper function for this.
     cript.add_orphaned_nodes_to_project(project, active_experiment=None, max_iteration=10)
-    project.validate()
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        project.validate()
 
     # Now add an orphan process to the graph
     process2 = copy.deepcopy(simple_process_node)
     process.prerequisite_process += [process2]
-    with pytest.raises(CRIPTOrphanedProcessError):
+    with pytest.warns(CRIPTOrphanedProcessWarning):
         project.validate()
 
     # Wrong fix it helper node
     dummy_experiment = copy.deepcopy(project.collection[0].experiment[0])
     with pytest.raises(RuntimeError):
         cript.add_orphaned_nodes_to_project(project, dummy_experiment)
     # Problem still persists
-    with pytest.raises(CRIPTOrphanedProcessError):
+    with pytest.warns(CRIPTOrphanedProcessWarning):
         project.validate()
     # Fix by using the helper function correctly
     cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
-    project.validate()
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        project.validate()
 
     # We add property to the material, because that adds the opportunity for orphaned data and computation
     property = copy.deepcopy(simple_property_node)
     material.property += [property]
-    project.validate()
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        project.validate()
     # Now add an orphan data
     data = copy.deepcopy(simple_data_node)
     property.data = [data]
 
-    with pytest.raises(CRIPTOrphanedDataError):
+    with pytest.warns(CRIPTOrphanedDataWarning):
         project.validate()
     # Fix with the helper function
     cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
-    project.validate()
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        project.validate()
 
     # Add an orphan Computation
     computation = copy.deepcopy(simple_computation_node)
     property.computation += [computation]
-    with pytest.raises(CRIPTOrphanedComputationError):
+    with pytest.warns(CRIPTOrphanedComputationWarning):
         project.validate()
     # Fix with the helper function
     cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
-    project.validate()
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        project.validate()
 
     # Add orphan computational process
     comp_proc = copy.deepcopy(simple_computation_process_node)
     data.computation_process += [comp_proc]
-    with pytest.raises(CRIPTOrphanedComputationalProcessError):
+    with pytest.raises(CRIPTOrphanedComputationalProcessWarning):
         while True:
-            try:  # Do trigger not orphan materials
-                project.validate()
-            except CRIPTOrphanedMaterialError as exc:
-                project._json_attrs.material.append(exc.orphaned_node)
-            except CRIPTOrphanedProcessError as exc:
-                project.collection[0].experiment[0]._json_attrs.process.append(exc.orphaned_node)
-            else:
-                break
+            with warnings.catch_warnings():
+                warnings.simplefilter("error")
+                try:  # Do trigger not orphan materials
+                    project.validate()
+                except CRIPTOrphanedMaterialWarning as exc:
+                    project._json_attrs.material.append(exc.orphaned_node)
+                except CRIPTOrphanedProcessWarning as exc:
+                    project.collection[0].experiment[0]._json_attrs.process.append(exc.orphaned_node)
+                else:
+                    break
 
     cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
     project.validate()
 
 
 def test_expanded_json(complex_project_node):
     """
```


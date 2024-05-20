# Comparing `tmp/kit4dl-2023.9b1.tar.gz` & `tmp/kit4dl-2023.9b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kit4dl-2023.9b1.tar", last modified: Fri Sep  8 06:28:47 2023, max compression
+gzip compressed data, was "kit4dl-2023.9b2.tar", last modified: Fri Sep 22 12:13:27 2023, max compression
```

## Comparing `kit4dl-2023.9b1.tar` & `kit4dl-2023.9b2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.086979 kit4dl-2023.9b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28923 2023-09-08 06:28:47.086979 kit4dl-2023.9b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26666 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.070979 kit4dl-2023.9b1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.074979 kit4dl-2023.9b1/examples/cnn_mnist_classification/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/examples/cnn_mnist_classification/conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.074979 kit4dl-2023.9b1/examples/cnn_s3dis_segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/examples/cnn_s3dis_segmentation/conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.074979 kit4dl-2023.9b1/kit4dl/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.078979 kit4dl-2023.9b1/kit4dl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.070979 kit4dl-2023.9b1/kit4dl/cli/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.078979 kit4dl-2023.9b1/kit4dl/cli/_templates/project/
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/cli/_templates/project/conf.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/cli/_templates/project/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/cli/_templates/project/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/kit4dl_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.078979 kit4dl-2023.9b1/kit4dl/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15711 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/nn/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/nn/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17385 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/nn/confmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/nn/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/nn/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/kit4dl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.078979 kit4dl-2023.9b1/kit4dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28923 2023-09-08 06:28:47.000000 kit4dl-2023.9b1/kit4dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-09-08 06:28:47.000000 kit4dl-2023.9b1/kit4dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 06:28:47.000000 kit4dl-2023.9b1/kit4dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-09-08 06:28:47.000000 kit4dl-2023.9b1/kit4dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-09-08 06:28:47.000000 kit4dl-2023.9b1/kit4dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-08 06:28:47.000000 kit4dl-2023.9b1/kit4dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 06:28:47.086979 kit4dl-2023.9b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.082979 kit4dl-2023.9b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.082979 kit4dl-2023.9b1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/cli/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/dummy_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/dummy_module2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.086979 kit4dl-2023.9b1/tests/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/nn/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22789 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/nn/test_confmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/nn/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/nn/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 06:28:47.086979 kit4dl-2023.9b1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/resources/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/resources/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/resources/test_file.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-08 06:28:34.000000 kit4dl-2023.9b1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.155733 kit4dl-2023.9b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    31622 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29440 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.143732 kit4dl-2023.9b2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/examples/cnn_mnist_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/examples/cnn_mnist_classification/conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/examples/cnn_s3dis_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/examples/cnn_s3dis_segmentation/conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/kit4dl/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/kit4dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.143732 kit4dl-2023.9b2/kit4dl/cli/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/kit4dl/cli/_templates/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/_templates/project/conf.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/_templates/project/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/_templates/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/kit4dl_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/kit4dl/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16510 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18227 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/confmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/nn/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/kit4dl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.147733 kit4dl-2023.9b2/kit4dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31622 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-22 12:13:27.000000 kit4dl-2023.9b2/kit4dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 12:13:27.155733 kit4dl-2023.9b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/cli/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/dummy_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/dummy_module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/tests/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22823 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/test_confmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/nn/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:13:27.151733 kit4dl-2023.9b2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/resources/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/resources/test_file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-22 12:13:17.000000 kit4dl-2023.9b2/tests/utils.py
```

### Comparing `kit4dl-2023.9b1/LICENSE` & `kit4dl-2023.9b2/LICENSE`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/PKG-INFO` & `kit4dl-2023.9b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kit4dl
-Version: 2023.9b1
+Version: 2023.9b2
 Summary: Kit4DL - A quick way to start with machine and deep learning
 Author: Jakub Walczak, Marco Mancini, Mirko Stojiljkovic, Shahbaz Alvi
 License: MIT License
         
         Copyright (c) 2023 opengeokube
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -69,15 +69,15 @@
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![pydocstyle](https://img.shields.io/badge/pydocstyle-enabled-AD4CD3)](http://www.pydocstyle.org/en/stable/)
 
 [![license](https://img.shields.io/badge/License-MIT-green.svg?labelColor=gray)](https://github.com/opengeokube/kit4dl/blob/main/LICENSE)
 
 [![pytest](https://github.com/opengeokube/kit4dl/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/opengeokube/kit4dl/actions/workflows/test.yml)
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8241376.svg)](https://doi.org/10.5281/zenodo.8241376)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8328176.svg)](https://doi.org/10.5281/zenodo.8328176)
 
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/kit4dl.svg)](https://anaconda.org/conda-forge/kit4dl) 
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/kit4dl.svg)](https://anaconda.org/conda-forge/kit4dl)
 
 [![PyPI version](https://badge.fury.io/py/kit4dl.svg)](https://badge.fury.io/py/kit4dl)
 </div>
 
@@ -95,30 +95,31 @@
 ```bibtex
 @SOFTWARE{kit4dl,
   author = {Walczak, Jakub and
             Mancini, Marco and
             Stojiljković, Mirko and
             Alvi, Shahbaz},
   title = {Kit4DL},
-  month = aug,
+  month = sep,
   year = 2023,
   note = {{Available in GitHub: https://github.com/opengeokube/kit4dl}},
   publisher = {Zenodo},
-  version = {2023.08b0},
-  doi = {10.5281/zenodo.8241376},
-  url = {https://doi.org/10.5281/zenodo.8241376}
+  version = {2023.9b1},
+  doi = {10.5281/zenodo.8328176},
+  url = {https://doi.org/10.5281/zenodo.8328176}
 }
 ```
 ## 🚧 Roadmap
 
 > **Warning**: Kit4DL is currently in its alpha stage. All recommendations are welcomed.
 
 - [ ] add handling sklearn-like models
 - [ ] add functionality to serve the model
 - [x] enable custom metrics
+- [x] enable using callbacks (also custom ones)
 - [ ] write more unit tests
 
 
 ## 🎬 Quickstart
 
 ### Getting started
 
@@ -450,18 +451,91 @@
 #### Configuring training
 Training-related arguments should be defined in the `[training]` section of the configuration file.
 You can define the following arguments.
 
 |   **Property** 	|  **Type**        |         **Details**              |
 |---------------	|----------------- | -------------------------------- | 
 |      `epochs`*    |   `int > 0`      |  number of epochs	              | 
+|      `callbacks`  |   `list`         |  list of callbacks	              | 
 |`epoch_schedulers` |  `list of dict`  |  list of schedulers definitions  |
 
 > **Note**: Arguments marked with `*` are obligatory!
 
+You can define a list of custom callbacks applied in the training process. Your callbacks need to be subclasses of `lightning.pytorch.callbacks.Callback` or `kit4dl.Kit4DLCallback` (for convenience) class and define one/some of the methods indicated in the [PyTorch-Lightning callback API](https://lightning.ai/docs/pytorch/stable/extensions/callbacks.html#callback-api). You can always use one of the [predefined callbacks](https://lightning.ai/docs/pytorch/stable/extensions/callbacks.html#built-in-callbacks).
+
+
+```toml
+[training]
+callbacks = [
+    {target = "./callbacks.py::SaveConfusionMatrixCallback", task="multiclass", num_classes=10, save_dir="{{ PROJECT_DIR }}/cm},
+    {target = "lightning.pytorch.callbacks::DeviceStatsMonitor"}
+]
+```
+
+Where the 1st callback is user-defined and the other - PyTorch-Loghtning built-in. For the custom callback we need to provide a class (here: located in the `callbacks.py` file in the project directory, the class is named `SaveConfusionMatrixCallback`).
+
+```python
+import os
+from typing import Any
+
+import lightning.pytorch as pl
+import torchmetrics as tm
+
+from kit4dl import Kit4DLCallback, StepOutput
+
+
+class SaveConfusionMatrixCallback(Kit4DLCallback):
+    _cm: tm.ConfusionMatrix
+    _num_classes: int
+    _task: str
+    _save_dir: str
+
+    def __init__(self, task: str, num_classes: int, save_dir: str) -> None:
+        super().__init__()
+        self._num_classes = num_classes
+        self._save_dir = save_dir
+        self._task = task
+        os.makedirs(self._save_dir, exist_ok=True)
+
+    def on_validation_epoch_start(
+        self, trainer: pl.Trainer, pl_module: pl.LightningModule
+    ) -> None:
+        self._cm = tm.ConfusionMatrix(
+            task=self._task, num_classes=self._num_classes
+        )
+
+    def on_validation_batch_end(
+        self,
+        trainer: pl.Trainer,
+        pl_module: pl.LightningModule,
+        outputs: StepOutput,
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int = 0,
+    ) -> None:
+        self._cm.update(outputs.predictions, outputs.labels)
+
+    def on_validation_epoch_end(
+        self, trainer: pl.Trainer, pl_module: pl.LightningModule
+    ) -> None:
+        """Called when the val epoch ends."""
+        fig, _ = self._cm.plot()
+        target_file = os.path.join(
+            self._save_dir,
+            f"confusion_matrix_for_epoch_{pl_module.current_epoch}",
+        )
+        fig.savefig(target_file)
+
+```
+
+
+
+
+
+
 Besides those listed in the table above, you can specify PyTorch Lightning-related `Trainer` arguments, like:
 1. `accumulate_grad_batches`
 1. `gradient_clip_val`
 1. `gradient_clip_algorithm`
 1. ...
 
 ##### ✍️ Example
@@ -623,8 +697,9 @@
 
 The constants currently available in `kit4dl` are the following:
 |   **Symbol** 	|            **Meaning of the symbol**                                   	|          **Example**                  |
 |-------------	|-----------------------------------------------------------------------	| -----------------------------------	|
 | `PROJECT_DIR`	| the home directory of the TOML configuration file (project directory) 	| `context.PROJECT_DIR`                 |
 | `LOG_LEVEL`	| logging level as defined in the configuration TOML file                	| `context.LOG_LEVEL`                   |
 | `LOG_FORMAT`	| logging message format as defined in the configuration TOML file      	| `context.LOG_FORMAT`                  |
+|  `VERSION`	| the current version of the package                                      	| `context.VERSION`                     |
```

### Comparing `kit4dl-2023.9b1/README.md` & `kit4dl-2023.9b2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![pydocstyle](https://img.shields.io/badge/pydocstyle-enabled-AD4CD3)](http://www.pydocstyle.org/en/stable/)
 
 [![license](https://img.shields.io/badge/License-MIT-green.svg?labelColor=gray)](https://github.com/opengeokube/kit4dl/blob/main/LICENSE)
 
 [![pytest](https://github.com/opengeokube/kit4dl/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/opengeokube/kit4dl/actions/workflows/test.yml)
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8241376.svg)](https://doi.org/10.5281/zenodo.8241376)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8328176.svg)](https://doi.org/10.5281/zenodo.8328176)
 
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/kit4dl.svg)](https://anaconda.org/conda-forge/kit4dl) 
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/kit4dl.svg)](https://anaconda.org/conda-forge/kit4dl)
 
 [![PyPI version](https://badge.fury.io/py/kit4dl.svg)](https://badge.fury.io/py/kit4dl)
 </div>
 
@@ -36,30 +36,31 @@
 ```bibtex
 @SOFTWARE{kit4dl,
   author = {Walczak, Jakub and
             Mancini, Marco and
             Stojiljković, Mirko and
             Alvi, Shahbaz},
   title = {Kit4DL},
-  month = aug,
+  month = sep,
   year = 2023,
   note = {{Available in GitHub: https://github.com/opengeokube/kit4dl}},
   publisher = {Zenodo},
-  version = {2023.08b0},
-  doi = {10.5281/zenodo.8241376},
-  url = {https://doi.org/10.5281/zenodo.8241376}
+  version = {2023.9b1},
+  doi = {10.5281/zenodo.8328176},
+  url = {https://doi.org/10.5281/zenodo.8328176}
 }
 ```
 ## 🚧 Roadmap
 
 > **Warning**: Kit4DL is currently in its alpha stage. All recommendations are welcomed.
 
 - [ ] add handling sklearn-like models
 - [ ] add functionality to serve the model
 - [x] enable custom metrics
+- [x] enable using callbacks (also custom ones)
 - [ ] write more unit tests
 
 
 ## 🎬 Quickstart
 
 ### Getting started
 
@@ -391,18 +392,91 @@
 #### Configuring training
 Training-related arguments should be defined in the `[training]` section of the configuration file.
 You can define the following arguments.
 
 |   **Property** 	|  **Type**        |         **Details**              |
 |---------------	|----------------- | -------------------------------- | 
 |      `epochs`*    |   `int > 0`      |  number of epochs	              | 
+|      `callbacks`  |   `list`         |  list of callbacks	              | 
 |`epoch_schedulers` |  `list of dict`  |  list of schedulers definitions  |
 
 > **Note**: Arguments marked with `*` are obligatory!
 
+You can define a list of custom callbacks applied in the training process. Your callbacks need to be subclasses of `lightning.pytorch.callbacks.Callback` or `kit4dl.Kit4DLCallback` (for convenience) class and define one/some of the methods indicated in the [PyTorch-Lightning callback API](https://lightning.ai/docs/pytorch/stable/extensions/callbacks.html#callback-api). You can always use one of the [predefined callbacks](https://lightning.ai/docs/pytorch/stable/extensions/callbacks.html#built-in-callbacks).
+
+
+```toml
+[training]
+callbacks = [
+    {target = "./callbacks.py::SaveConfusionMatrixCallback", task="multiclass", num_classes=10, save_dir="{{ PROJECT_DIR }}/cm},
+    {target = "lightning.pytorch.callbacks::DeviceStatsMonitor"}
+]
+```
+
+Where the 1st callback is user-defined and the other - PyTorch-Loghtning built-in. For the custom callback we need to provide a class (here: located in the `callbacks.py` file in the project directory, the class is named `SaveConfusionMatrixCallback`).
+
+```python
+import os
+from typing import Any
+
+import lightning.pytorch as pl
+import torchmetrics as tm
+
+from kit4dl import Kit4DLCallback, StepOutput
+
+
+class SaveConfusionMatrixCallback(Kit4DLCallback):
+    _cm: tm.ConfusionMatrix
+    _num_classes: int
+    _task: str
+    _save_dir: str
+
+    def __init__(self, task: str, num_classes: int, save_dir: str) -> None:
+        super().__init__()
+        self._num_classes = num_classes
+        self._save_dir = save_dir
+        self._task = task
+        os.makedirs(self._save_dir, exist_ok=True)
+
+    def on_validation_epoch_start(
+        self, trainer: pl.Trainer, pl_module: pl.LightningModule
+    ) -> None:
+        self._cm = tm.ConfusionMatrix(
+            task=self._task, num_classes=self._num_classes
+        )
+
+    def on_validation_batch_end(
+        self,
+        trainer: pl.Trainer,
+        pl_module: pl.LightningModule,
+        outputs: StepOutput,
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int = 0,
+    ) -> None:
+        self._cm.update(outputs.predictions, outputs.labels)
+
+    def on_validation_epoch_end(
+        self, trainer: pl.Trainer, pl_module: pl.LightningModule
+    ) -> None:
+        """Called when the val epoch ends."""
+        fig, _ = self._cm.plot()
+        target_file = os.path.join(
+            self._save_dir,
+            f"confusion_matrix_for_epoch_{pl_module.current_epoch}",
+        )
+        fig.savefig(target_file)
+
+```
+
+
+
+
+
+
 Besides those listed in the table above, you can specify PyTorch Lightning-related `Trainer` arguments, like:
 1. `accumulate_grad_batches`
 1. `gradient_clip_val`
 1. `gradient_clip_algorithm`
 1. ...
 
 ##### ✍️ Example
@@ -564,8 +638,9 @@
 
 The constants currently available in `kit4dl` are the following:
 |   **Symbol** 	|            **Meaning of the symbol**                                   	|          **Example**                  |
 |-------------	|-----------------------------------------------------------------------	| -----------------------------------	|
 | `PROJECT_DIR`	| the home directory of the TOML configuration file (project directory) 	| `context.PROJECT_DIR`                 |
 | `LOG_LEVEL`	| logging level as defined in the configuration TOML file                	| `context.LOG_LEVEL`                   |
 | `LOG_FORMAT`	| logging message format as defined in the configuration TOML file      	| `context.LOG_FORMAT`                  |
+|  `VERSION`	| the current version of the package                                      	| `context.VERSION`                     |
```

#### html2text {}

```diff
@@ -11,83 +11,84 @@
 lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![pydocstyle](https://
 img.shields.io/badge/pydocstyle-enabled-AD4CD3)](http://www.pydocstyle.org/en/
         stable/) [![license](https://img.shields.io/badge/License-MIT-
  green.svg?labelColor=gray)](https://github.com/opengeokube/kit4dl/blob/main/
  LICENSE) [![pytest](https://github.com/opengeokube/kit4dl/actions/workflows/
 test.yml/badge.svg?branch=main)](https://github.com/opengeokube/kit4dl/actions/
        workflows/test.yml) [![DOI](https://zenodo.org/badge/DOI/10.5281/
-zenodo.8241376.svg)](https://doi.org/10.5281/zenodo.8241376) [![Conda Version]
+zenodo.8328176.svg)](https://doi.org/10.5281/zenodo.8328176) [![Conda Version]
 (https://img.shields.io/conda/vn/conda-forge/kit4dl.svg)](https://anaconda.org/
 conda-forge/kit4dl) [![Conda Downloads](https://img.shields.io/conda/dn/conda-
  forge/kit4dl.svg)](https://anaconda.org/conda-forge/kit4dl) [![PyPI version]
     (https://badge.fury.io/py/kit4dl.svg)](https://badge.fury.io/py/kit4dl)
 ## ðï¸ Authors OpenGeokube Developers: 1. Jakub Walczak _[_O_R_C_I_D_ _l_o_g_o_]1.
 Marco Macini _[_O_R_C_I_D_ _l_o_g_o_]1. Mirko Stojiljkovic _[_O_R_C_I_D_ _l_o_g_o_]1. Shahbaz Alvi
 _[_O_R_C_I_D_ _l_o_g_o_]## ð Cite Us ```bibtex @SOFTWARE{kit4dl, author = {Walczak,
 Jakub and Mancini, Marco and StojiljkoviÄ, Mirko and Alvi, Shahbaz}, title =
-{Kit4DL}, month = aug, year = 2023, note = {{Available in GitHub: https://
-github.com/opengeokube/kit4dl}}, publisher = {Zenodo}, version = {2023.08b0},
-doi = {10.5281/zenodo.8241376}, url = {https://doi.org/10.5281/zenodo.8241376}
+{Kit4DL}, month = sep, year = 2023, note = {{Available in GitHub: https://
+github.com/opengeokube/kit4dl}}, publisher = {Zenodo}, version = {2023.9b1},
+doi = {10.5281/zenodo.8328176}, url = {https://doi.org/10.5281/zenodo.8328176}
 } ``` ## ð§ Roadmap > **Warning**: Kit4DL is currently in its alpha stage.
 All recommendations are welcomed. - [ ] add handling sklearn-like models - [ ]
-add functionality to serve the model - [x] enable custom metrics - [ ] write
-more unit tests ## ð¬ Quickstart ### Getting started #### Installation
-```bash pip install kit4dl ``` or ```bash conda install -c conda-forge kit4dl
-``` For contributing: Download and install the `make` tool unless it is already
-available in your system. ```text git clone https://github.com/opengeokube/
-kit4dl cd kit4dl conda env create -f dev-env.yaml pip install -e . ``` ####
-Preparing simple project To start the new project in the current working
-directory, just run the following command: ```bash kit4dl init --name=my-new-
-project ``` It will create a directory with the name `my-new-project` where
-you'll find sample files. Implement necessery methods for datamodule
-(`dataset.py`) and network (`model.py`). Then, adjust `conf.toml` according to
-your needs. That's all ð #### Running the training To run the training just
-type the following command: ```bash kit4dl train ``` > **Note**: If you want to
-run also test for best saved weight, use flag `--test` If the `conf.toml` file
-is present in your current working directory, the training will start. If you
-need to specify the path to the configuration file, use `--conf` argument:
-```bash kit4dl train --conf=/path/to/your/conf.toml ``` #### Serving the model
-The packuge does not yet support model serving. ## ðª Playground At first,
-install `kit4dl` package as indicated in the Section [Installation]
-(#installation). #### Handwritten digit recognition Just navigate to the
-directory `/examples/cnn_mnist_classification` and run ```bash kit4dl train ```
-#### Point cloud instance segmentation Just navigate to the directory `/
-examples/cnn_s3dis_segmentation` and run ```bash kit4dl train ``` ## ð¡
-Instruction 1. [Configuring base setup](#configuring-base-setup) 1.
-[Configuring logging](#configuring-logging) 1. [Defining model](#defining-
-model) 1. [Defining datamodule](#defining-datamodule) 1. [Configuring training]
-(#configuring-training) 1. [Configuring optimizer](#configuring-optimizer) 1.
-[Configuring criterion](#configuring-criterion) 1. [Configuring metrics]
-(#configuring-metrics) 1. [Configuring checkpoint](#configuring-checkpoint) 1.
-[Defining `target`](#defining-target) 1. [Substitutable symbols]
-(#substitutable-symbols) 1. [Context constants](#context-constants) ####
-Configuring base setup Most of the training/validation procedure is managed by
-a configuration file in the TOML format (recommended name is `conf.toml`). Each
-aspect is covered by separate sections. The general one is called `[base]`. It
-has the following properties: | **Property** | **Type** | **Details** | |------
---------- |----------------- | ------------------------------------------------
-------------------------------------------------------- | | `seed` | `int` |
-seed of the random numbers generators for `NumPy` and `PyTorch` | | `cuda_id` |
-`int` or `None` | ID of the cuda device (if available) or `None` for `CPU` |
-|`experiment_name`* | `str` | name of the experiment | > **Note**: Arguments
-marked with `*` are obligatory! > **Warning**: Remember to install the version
-of `pytorch-cuda` package compliant to your CUDA Toolkit version. ##### âï¸
-Example ```toml [base] seed = 0 cuda_id = 1 experiment_name =
-"point_clout_segmentation" ``` #### Configuring logging Logging section is
-optional but it provides you with some extra flexibility regarding the logging.
-All configuration related to logging is included in the `[logging]` section of
-the configuration file. You can define following properties: | **Property** |
-**Type** | **Details** | |--------------- |----------------- | ----------------
--------------------------------------------------------------------------------
--------- | | `type` | `str` | type of metric logger (one of the value:
-`"comet"`, `"csv"`, `"mlflow"`, `"neptune"`, `"tensorboard"`, `"wandb"` -
-metric loggers supported by PyTorch Lightning [https://lightning.ai/docs/
-pytorch/stable/api_references.html#loggers](https://lightning.ai/docs/pytorch/
-stable/api_references.html#loggers). **DEFAULT:** `csv`) | | `level` | `str` |
-Python-supported logging levels (i.e. `"DEBUG"`, `"INFO"`, `"WARN"`, `"ERROR"`,
+add functionality to serve the model - [x] enable custom metrics - [x] enable
+using callbacks (also custom ones) - [ ] write more unit tests ## ð¬
+Quickstart ### Getting started #### Installation ```bash pip install kit4dl ```
+or ```bash conda install -c conda-forge kit4dl ``` For contributing: Download
+and install the `make` tool unless it is already available in your system.
+```text git clone https://github.com/opengeokube/kit4dl cd kit4dl conda env
+create -f dev-env.yaml pip install -e . ``` #### Preparing simple project To
+start the new project in the current working directory, just run the following
+command: ```bash kit4dl init --name=my-new-project ``` It will create a
+directory with the name `my-new-project` where you'll find sample files.
+Implement necessery methods for datamodule (`dataset.py`) and network
+(`model.py`). Then, adjust `conf.toml` according to your needs. That's all ð
+#### Running the training To run the training just type the following command:
+```bash kit4dl train ``` > **Note**: If you want to run also test for best
+saved weight, use flag `--test` If the `conf.toml` file is present in your
+current working directory, the training will start. If you need to specify the
+path to the configuration file, use `--conf` argument: ```bash kit4dl train --
+conf=/path/to/your/conf.toml ``` #### Serving the model The packuge does not
+yet support model serving. ## ðª Playground At first, install `kit4dl`
+package as indicated in the Section [Installation](#installation). ####
+Handwritten digit recognition Just navigate to the directory `/examples/
+cnn_mnist_classification` and run ```bash kit4dl train ``` #### Point cloud
+instance segmentation Just navigate to the directory `/examples/
+cnn_s3dis_segmentation` and run ```bash kit4dl train ``` ## ð¡ Instruction 1.
+[Configuring base setup](#configuring-base-setup) 1. [Configuring logging]
+(#configuring-logging) 1. [Defining model](#defining-model) 1. [Defining
+datamodule](#defining-datamodule) 1. [Configuring training](#configuring-
+training) 1. [Configuring optimizer](#configuring-optimizer) 1. [Configuring
+criterion](#configuring-criterion) 1. [Configuring metrics](#configuring-
+metrics) 1. [Configuring checkpoint](#configuring-checkpoint) 1. [Defining
+`target`](#defining-target) 1. [Substitutable symbols](#substitutable-symbols)
+1. [Context constants](#context-constants) #### Configuring base setup Most of
+the training/validation procedure is managed by a configuration file in the
+TOML format (recommended name is `conf.toml`). Each aspect is covered by
+separate sections. The general one is called `[base]`. It has the following
+properties: | **Property** | **Type** | **Details** | |--------------- |-------
+---------- | ------------------------------------------------------------------
+------------------------------------- | | `seed` | `int` | seed of the random
+numbers generators for `NumPy` and `PyTorch` | | `cuda_id` | `int` or `None` |
+ID of the cuda device (if available) or `None` for `CPU` | |`experiment_name`*
+| `str` | name of the experiment | > **Note**: Arguments marked with `*` are
+obligatory! > **Warning**: Remember to install the version of `pytorch-cuda`
+package compliant to your CUDA Toolkit version. ##### âï¸ Example ```toml
+[base] seed = 0 cuda_id = 1 experiment_name = "point_clout_segmentation" ```
+#### Configuring logging Logging section is optional but it provides you with
+some extra flexibility regarding the logging. All configuration related to
+logging is included in the `[logging]` section of the configuration file. You
+can define following properties: | **Property** | **Type** | **Details** | |---
+------------ |----------------- | ---------------------------------------------
+---------------------------------------------------------- | | `type` | `str` |
+type of metric logger (one of the value: `"comet"`, `"csv"`, `"mlflow"`,
+`"neptune"`, `"tensorboard"`, `"wandb"` - metric loggers supported by PyTorch
+Lightning [https://lightning.ai/docs/pytorch/stable/
+api_references.html#loggers](https://lightning.ai/docs/pytorch/stable/
+api_references.html#loggers). **DEFAULT:** `csv`) | | `level` | `str` | Python-
+supported logging levels (i.e. `"DEBUG"`, `"INFO"`, `"WARN"`, `"ERROR"`,
 `"CRITICAL"`) **DEFAULT:** `INFO` | |`format` | `str` | logging message format
 as defined for the Python `logging` package (see [https://docs.python.org/3/
 library/logging.html#logging.LogRecord](https://docs.python.org/3/library/
 logging.html#logging.LogRecord)) | > **Warning**: Logger `level` and `format`
 are related to the Python `logging` Loggers you can use in your model and
 datamodule classes with approperiate methods `self.debure`, `self.info`, etc.
 In `type`, in turn, you just specify the metric logger as used in PyTorch
@@ -195,59 +196,88 @@
 indicated in the PyTorch docs [torch.utils.data.DataLoader](https://
 pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader). > **Warning**:
 You **cannot** specify loader arguments for in the `[dataset.trainval.loader]`.
 Loaders should be defined for each split separately. #### Configuring training
 Training-related arguments should be defined in the `[training]` section of the
 configuration file. You can define the following arguments. | **Property** |
 **Type** | **Details** | |--------------- |----------------- | ----------------
----------------- | | `epochs`* | `int > 0` | number of epochs |
-|`epoch_schedulers` | `list of dict` | list of schedulers definitions | >
-**Note**: Arguments marked with `*` are obligatory! Besides those listed in the
-table above, you can specify PyTorch Lightning-related `Trainer` arguments,
-like: 1. `accumulate_grad_batches` 1. `gradient_clip_val` 1.
-`gradient_clip_algorithm` 1. ... ##### âï¸ Example ```toml [training] epochs
-= 10 epoch_schedulers = [ {target = "torch.optim.lr_scheduler::
-CosineAnnealingLR", T_max = 100} ] accumulate_grad_batches = 2 ``` ####
-Configuring optimizer Optimizer configuration is located in the subsection `
-[training.optimizer]`. There, you should define `target` (see [Defining
-`target`](#defining-target)) and extra keyword arguments passed to the
-optimizer initializer. ##### âï¸ Example ```toml [training.optimizer] target
-= "torch.optim::Adam" lr = 0.001 weight_decay = 0.01 ``` > **Note**: The
-section `[training.optimizer]` is **mandatory**. > **Note**: You can always
-define the custom optimizer. Then, you just need to set the proper `target`
-value. #### Configuring criterion Similarily to the optimizer configuration,
-there is a subsection dedicated for the critarion. You need to specify, at
-least, the `target` (see [Defining `target`](#defining-target)) and other
-mandatory or optional properties of the selected critarion (loss function).
-##### âï¸ Example ```toml [training.criterion] target = "torch.nn::
-CrossEntropyLoss" weight = [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1]
-``` > **Note**: The section `[training.criterion]` is **mandatory**. >
-**Note**: You can always define the custom optimizer. Then, you just need to
-set the proper `target` value. #### Configuring metrics Metrics are configured
-in the section `[metrics]` of the configuration file. You can define several
-metrics (including the custom ones). The only thing you need to do is to define
-all desired metrics. For each metric dictionary, you need to set `target` (see
-Section [Defining `target`](#defining-target)) value and, eventually, extra
-arguments. **REMEMBER** to have metric names (here `MyPrecision` and
-`FBetaScore`) unique! ##### âï¸ Example ```toml [metrics] MyPrecision =
-{target = "torchmetrics::Precision", task = "multiclass", num_classes=10}
-FBetaScore = {target = "torchmetrics::FBetaScore", task = "multiclass",
-num_classes=10, beta = 0.1} ``` > **Note**: You can define custom metrics. Just
-properly set `target` value. **REMEMBER!** The custom metric need to be a
-subclass of `torchmetrics.Metric` class! ```python import torch import
-torchmetrics as tm class MyMetric(tm.Metric): def __init__(self): ... def
-update(self, preds: torch.Tensor, target: torch.Tensor): ... def compute(self):
-... ``` #### Configuring checkpoint If you need to save your intermediate
-weights (do checkpoints) you can configure the optional subsection `
-[training.checkpoint]`. In the section, you can define the following
-proeprties: | **Property** | **Type** | **Details** | |--------------- |-------
----------- | -------------------------------- | | `path`* | `str` | path to a
-directory where checkpoints should be stored | |`monitor`* | `dict` | a
-dictionary with two keys: `metric` and `stage`. `metrics` is a metric name as
-defined in the `[metrics]` section ([Configuring metrics](#configuring-
+---------------- | | `epochs`* | `int > 0` | number of epochs | | `callbacks` |
+`list` | list of callbacks | |`epoch_schedulers` | `list of dict` | list of
+schedulers definitions | > **Note**: Arguments marked with `*` are obligatory!
+You can define a list of custom callbacks applied in the training process. Your
+callbacks need to be subclasses of `lightning.pytorch.callbacks.Callback` or
+`kit4dl.Kit4DLCallback` (for convenience) class and define one/some of the
+methods indicated in the [PyTorch-Lightning callback API](https://lightning.ai/
+docs/pytorch/stable/extensions/callbacks.html#callback-api). You can always use
+one of the [predefined callbacks](https://lightning.ai/docs/pytorch/stable/
+extensions/callbacks.html#built-in-callbacks). ```toml [training] callbacks =
+[ {target = "./callbacks.py::SaveConfusionMatrixCallback", task="multiclass",
+num_classes=10, save_dir="{{ PROJECT_DIR }}/cm}, {target =
+"lightning.pytorch.callbacks::DeviceStatsMonitor"} ] ``` Where the 1st callback
+is user-defined and the other - PyTorch-Loghtning built-in. For the custom
+callback we need to provide a class (here: located in the `callbacks.py` file
+in the project directory, the class is named `SaveConfusionMatrixCallback`).
+```python import os from typing import Any import lightning.pytorch as pl
+import torchmetrics as tm from kit4dl import Kit4DLCallback, StepOutput class
+SaveConfusionMatrixCallback(Kit4DLCallback): _cm: tm.ConfusionMatrix
+_num_classes: int _task: str _save_dir: str def __init__(self, task: str,
+num_classes: int, save_dir: str) -> None: super().__init__() self._num_classes
+= num_classes self._save_dir = save_dir self._task = task os.makedirs
+(self._save_dir, exist_ok=True) def on_validation_epoch_start( self, trainer:
+pl.Trainer, pl_module: pl.LightningModule ) -> None: self._cm =
+tm.ConfusionMatrix( task=self._task, num_classes=self._num_classes ) def
+on_validation_batch_end( self, trainer: pl.Trainer, pl_module:
+pl.LightningModule, outputs: StepOutput, batch: Any, batch_idx: int,
+dataloader_idx: int = 0, ) -> None: self._cm.update(outputs.predictions,
+outputs.labels) def on_validation_epoch_end( self, trainer: pl.Trainer,
+pl_module: pl.LightningModule ) -> None: """Called when the val epoch ends."""
+fig, _ = self._cm.plot() target_file = os.path.join( self._save_dir,
+f"confusion_matrix_for_epoch_{pl_module.current_epoch}", ) fig.savefig
+(target_file) ``` Besides those listed in the table above, you can specify
+PyTorch Lightning-related `Trainer` arguments, like: 1.
+`accumulate_grad_batches` 1. `gradient_clip_val` 1. `gradient_clip_algorithm`
+1. ... ##### âï¸ Example ```toml [training] epochs = 10 epoch_schedulers =
+[ {target = "torch.optim.lr_scheduler::CosineAnnealingLR", T_max = 100} ]
+accumulate_grad_batches = 2 ``` #### Configuring optimizer Optimizer
+configuration is located in the subsection `[training.optimizer]`. There, you
+should define `target` (see [Defining `target`](#defining-target)) and extra
+keyword arguments passed to the optimizer initializer. ##### âï¸ Example
+```toml [training.optimizer] target = "torch.optim::Adam" lr = 0.001
+weight_decay = 0.01 ``` > **Note**: The section `[training.optimizer]` is
+**mandatory**. > **Note**: You can always define the custom optimizer. Then,
+you just need to set the proper `target` value. #### Configuring criterion
+Similarily to the optimizer configuration, there is a subsection dedicated for
+the critarion. You need to specify, at least, the `target` (see [Defining
+`target`](#defining-target)) and other mandatory or optional properties of the
+selected critarion (loss function). ##### âï¸ Example ```toml
+[training.criterion] target = "torch.nn::CrossEntropyLoss" weight = [0.1, 0.1,
+0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1] ``` > **Note**: The section `
+[training.criterion]` is **mandatory**. > **Note**: You can always define the
+custom optimizer. Then, you just need to set the proper `target` value. ####
+Configuring metrics Metrics are configured in the section `[metrics]` of the
+configuration file. You can define several metrics (including the custom ones).
+The only thing you need to do is to define all desired metrics. For each metric
+dictionary, you need to set `target` (see Section [Defining `target`]
+(#defining-target)) value and, eventually, extra arguments. **REMEMBER** to
+have metric names (here `MyPrecision` and `FBetaScore`) unique! ##### âï¸
+Example ```toml [metrics] MyPrecision = {target = "torchmetrics::Precision",
+task = "multiclass", num_classes=10} FBetaScore = {target = "torchmetrics::
+FBetaScore", task = "multiclass", num_classes=10, beta = 0.1} ``` > **Note**:
+You can define custom metrics. Just properly set `target` value. **REMEMBER!**
+The custom metric need to be a subclass of `torchmetrics.Metric` class!
+```python import torch import torchmetrics as tm class MyMetric(tm.Metric): def
+__init__(self): ... def update(self, preds: torch.Tensor, target:
+torch.Tensor): ... def compute(self): ... ``` #### Configuring checkpoint If
+you need to save your intermediate weights (do checkpoints) you can configure
+the optional subsection `[training.checkpoint]`. In the section, you can define
+the following proeprties: | **Property** | **Type** | **Details** | |----------
+----- |----------------- | -------------------------------- | | `path`* | `str`
+| path to a directory where checkpoints should be stored | |`monitor`* | `dict`
+| a dictionary with two keys: `metric` and `stage`. `metrics` is a metric name
+as defined in the `[metrics]` section ([Configuring metrics](#configuring-
 metrics)), `stage` is one of the following: [`train`, `val`] | | `filename`* |
 `str` | filename pattern of the checkpoint (see (PyTorch Lightning
 `ModelCheckpoint`)[https://lightning.ai/docs/pytorch/stable/api/
 lightning.pytorch.callbacks.ModelCheckpoint.html]) you can use value of the
 defined metric for the stage. if you want `MyPrecision` score for the
 validation stage, use `{val_myprecision}` in the filename | | `mode` | `min` |
 `max` | to save checkpoint for `min`imum or `max`imum value of the metric being
@@ -307,8 +337,9 @@
 (context.PROJECT_DIR) ``` The constants currently available in `kit4dl` are the
 following: | **Symbol** | **Meaning of the symbol** | **Example** | |----------
 --- |----------------------------------------------------------------------- |
 ----------------------------------- | | `PROJECT_DIR` | the home directory of
 the TOML configuration file (project directory) | `context.PROJECT_DIR` | |
 `LOG_LEVEL` | logging level as defined in the configuration TOML file |
 `context.LOG_LEVEL` | | `LOG_FORMAT` | logging message format as defined in the
-configuration TOML file | `context.LOG_FORMAT` |
+configuration TOML file | `context.LOG_FORMAT` | | `VERSION` | the current
+version of the package | `context.VERSION` |
```

### Comparing `kit4dl-2023.9b1/examples/cnn_mnist_classification/conf.toml` & `kit4dl-2023.9b2/examples/cnn_mnist_classification/conf.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,64 +23,77 @@
 00000160: 6e69 6e67 5d0d 0a65 706f 6368 7320 3d20  ning]..epochs = 
 00000170: 3130 0d0a 6570 6f63 685f 7363 6865 6475  10..epoch_schedu
 00000180: 6c65 7273 203d 205b 0d0a 2020 2020 7b74  lers = [..    {t
 00000190: 6172 6765 7420 3d20 2274 6f72 6368 2e6f  arget = "torch.o
 000001a0: 7074 696d 2e6c 725f 7363 6865 6475 6c65  ptim.lr_schedule
 000001b0: 723a 3a43 6f73 696e 6541 6e6e 6561 6c69  r::CosineAnneali
 000001c0: 6e67 4c52 222c 2054 5f6d 6178 203d 2031  ngLR", T_max = 1
-000001d0: 3030 7d0d 0a5d 0d0a 0d0a 5b74 7261 696e  00}..]....[train
-000001e0: 696e 672e 6368 6563 6b70 6f69 6e74 5d0d  ing.checkpoint].
-000001f0: 0a70 6174 6820 3d20 2263 6863 6b70 7422  .path = "chckpt"
-00000200: 0d0a 6d6f 6e69 746f 7220 3d20 7b22 6d65  ..monitor = {"me
-00000210: 7472 6963 2220 3d20 224d 7950 7265 6369  tric" = "MyPreci
-00000220: 7369 6f6e 222c 2022 7374 6167 6522 203d  sion", "stage" =
-00000230: 2022 7661 6c22 7d0d 0a66 696c 656e 616d   "val"}..filenam
-00000240: 6520 3d20 227b 6570 6f63 687d 5f7b 7661  e = "{epoch}_{va
-00000250: 6c5f 6d79 7072 6563 6973 696f 6e3a 2e32  l_myprecision:.2
-00000260: 667d 5f63 6e6e 220d 0a6d 6f64 6520 3d20  f}_cnn"..mode = 
-00000270: 226d 6178 220d 0a73 6176 655f 746f 705f  "max"..save_top_
-00000280: 6b20 3d20 310d 0a0d 0a5b 7472 6169 6e69  k = 1....[traini
-00000290: 6e67 2e6f 7074 696d 697a 6572 5d0d 0a74  ng.optimizer]..t
-000002a0: 6172 6765 7420 3d20 2274 6f72 6368 2e6f  arget = "torch.o
-000002b0: 7074 696d 3a3a 4164 616d 220d 0a6c 7220  ptim::Adam"..lr 
-000002c0: 3d20 302e 3030 310d 0a77 6569 6768 745f  = 0.001..weight_
-000002d0: 6465 6361 7920 3d20 302e 3031 0d0a 0d0a  decay = 0.01....
-000002e0: 5b74 7261 696e 696e 672e 6372 6974 6572  [training.criter
-000002f0: 696f 6e5d 0d0a 7461 7267 6574 203d 2022  ion]..target = "
-00000300: 746f 7263 682e 6e6e 3a3a 4372 6f73 7345  torch.nn::CrossE
-00000310: 6e74 726f 7079 4c6f 7373 220d 0a77 6569  ntropyLoss"..wei
-00000320: 6768 7420 3d20 5b30 2e31 2c20 302e 312c  ght = [0.1, 0.1,
-00000330: 2030 2e31 2c20 302e 312c 2030 2e31 2c20   0.1, 0.1, 0.1, 
-00000340: 302e 312c 2030 2e31 2c20 302e 312c 2030  0.1, 0.1, 0.1, 0
-00000350: 2e31 2c20 302e 315d 0d0a 0d0a 5b76 616c  .1, 0.1]....[val
-00000360: 6964 6174 696f 6e5d 0d0a 7275 6e5f 6576  idation]..run_ev
-00000370: 6572 795f 6570 6f63 6820 3d20 310d 0a0d  ery_epoch = 1...
-00000380: 0a5b 6461 7461 7365 745d 0d0a 7461 7267  .[dataset]..targ
-00000390: 6574 203d 2022 2e2f 6461 7461 6d6f 6475  et = "./datamodu
-000003a0: 6c65 2e70 793a 3a4d 4e49 5354 4375 7374  le.py::MNISTCust
-000003b0: 6f6d 4461 7461 6d6f 6475 6c65 220d 0a0d  omDatamodule"...
-000003c0: 0a5b 6461 7461 7365 742e 7472 6169 6e76  .[dataset.trainv
-000003d0: 616c 5d0d 0a72 6f6f 745f 6469 7220 3d20  al]..root_dir = 
-000003e0: 222e 2f6d 6e69 7374 220d 0a0d 0a5b 6461  "./mnist"....[da
-000003f0: 7461 7365 742e 7472 6169 6e2e 6c6f 6164  taset.train.load
-00000400: 6572 5d0d 0a62 6174 6368 5f73 697a 6520  er]..batch_size 
-00000410: 3d20 3135 300d 0a73 6875 6666 6c65 203d  = 150..shuffle =
-00000420: 2074 7275 650d 0a6e 756d 5f77 6f72 6b65   true..num_worke
-00000430: 7273 203d 2034 0d0a 0d0a 5b64 6174 6173  rs = 4....[datas
-00000440: 6574 2e76 616c 6964 6174 696f 6e2e 6c6f  et.validation.lo
-00000450: 6164 6572 5d0d 0a62 6174 6368 5f73 697a  ader]..batch_siz
-00000460: 6520 3d20 3135 300d 0a73 6875 6666 6c65  e = 150..shuffle
-00000470: 203d 2066 616c 7365 0d0a 6e75 6d5f 776f   = false..num_wo
-00000480: 726b 6572 7320 3d20 340d 0a0d 0a5b 6d65  rkers = 4....[me
-00000490: 7472 6963 735d 0d0a 4d79 5072 6563 6973  trics]..MyPrecis
-000004a0: 696f 6e20 3d20 7b74 6172 6765 7420 3d20  ion = {target = 
-000004b0: 2274 6f72 6368 6d65 7472 6963 733a 3a50  "torchmetrics::P
-000004c0: 7265 6369 7369 6f6e 222c 2074 6173 6b20  recision", task 
-000004d0: 3d20 226d 756c 7469 636c 6173 7322 2c20  = "multiclass", 
-000004e0: 6e75 6d5f 636c 6173 7365 733d 3130 7d0d  num_classes=10}.
-000004f0: 0a46 4265 7461 5363 6f72 6520 3d20 7b74  .FBetaScore = {t
-00000500: 6172 6765 7420 3d20 2274 6f72 6368 6d65  arget = "torchme
-00000510: 7472 6963 733a 3a46 4265 7461 5363 6f72  trics::FBetaScor
-00000520: 6522 2c20 7461 736b 203d 2022 6d75 6c74  e", task = "mult
-00000530: 6963 6c61 7373 222c 206e 756d 5f63 6c61  iclass", num_cla
-00000540: 7373 6573 3d31 302c 2062 6574 6120 3d20  sses=10, beta = 
-00000550: 302e 317d                                0.1}
+000001d0: 3030 7d0d 0a5d 0d0a 6361 6c6c 6261 636b  00}..]..callback
+000001e0: 7320 3d20 5b0d 0a20 2020 207b 7461 7267  s = [..    {targ
+000001f0: 6574 203d 2022 2e2f 6361 6c6c 6261 636b  et = "./callback
+00000200: 732e 7079 3a3a 5361 7665 436f 6e66 7573  s.py::SaveConfus
+00000210: 696f 6e4d 6174 7269 7843 616c 6c62 6163  ionMatrixCallbac
+00000220: 6b22 2c20 2074 6173 6b3d 226d 756c 7469  k",  task="multi
+00000230: 636c 6173 7322 2c20 6e75 6d5f 636c 6173  class", num_clas
+00000240: 7365 7320 3d20 3130 2c20 7361 7665 5f64  ses = 10, save_d
+00000250: 6972 203d 2022 7b7b 2050 524f 4a45 4354  ir = "{{ PROJECT
+00000260: 5f44 4952 207d 7d2f 636d 227d 2c0d 0a20  _DIR }}/cm"},.. 
+00000270: 2020 207b 7461 7267 6574 203d 2022 6c69     {target = "li
+00000280: 6768 746e 696e 672e 7079 746f 7263 682e  ghtning.pytorch.
+00000290: 6361 6c6c 6261 636b 733a 3a44 6576 6963  callbacks::Devic
+000002a0: 6553 7461 7473 4d6f 6e69 746f 7222 7d0d  eStatsMonitor"}.
+000002b0: 0a5d 0d0a 0d0a 5b74 7261 696e 696e 672e  .]....[training.
+000002c0: 6368 6563 6b70 6f69 6e74 5d0d 0a70 6174  checkpoint]..pat
+000002d0: 6820 3d20 2263 6863 6b70 7422 0d0a 6d6f  h = "chckpt"..mo
+000002e0: 6e69 746f 7220 3d20 7b22 6d65 7472 6963  nitor = {"metric
+000002f0: 2220 3d20 224d 7950 7265 6369 7369 6f6e  " = "MyPrecision
+00000300: 222c 2022 7374 6167 6522 203d 2022 7661  ", "stage" = "va
+00000310: 6c22 7d0d 0a66 696c 656e 616d 6520 3d20  l"}..filename = 
+00000320: 227b 6570 6f63 687d 5f7b 7661 6c5f 6d79  "{epoch}_{val_my
+00000330: 7072 6563 6973 696f 6e3a 2e32 667d 5f63  precision:.2f}_c
+00000340: 6e6e 220d 0a6d 6f64 6520 3d20 226d 6178  nn"..mode = "max
+00000350: 220d 0a73 6176 655f 746f 705f 6b20 3d20  "..save_top_k = 
+00000360: 310d 0a0d 0a5b 7472 6169 6e69 6e67 2e6f  1....[training.o
+00000370: 7074 696d 697a 6572 5d0d 0a74 6172 6765  ptimizer]..targe
+00000380: 7420 3d20 2274 6f72 6368 2e6f 7074 696d  t = "torch.optim
+00000390: 3a3a 4164 616d 220d 0a6c 7220 3d20 302e  ::Adam"..lr = 0.
+000003a0: 3030 310d 0a77 6569 6768 745f 6465 6361  001..weight_deca
+000003b0: 7920 3d20 302e 3031 0d0a 0d0a 5b74 7261  y = 0.01....[tra
+000003c0: 696e 696e 672e 6372 6974 6572 696f 6e5d  ining.criterion]
+000003d0: 0d0a 7461 7267 6574 203d 2022 746f 7263  ..target = "torc
+000003e0: 682e 6e6e 3a3a 4372 6f73 7345 6e74 726f  h.nn::CrossEntro
+000003f0: 7079 4c6f 7373 220d 0a77 6569 6768 7420  pyLoss"..weight 
+00000400: 3d20 5b30 2e31 2c20 302e 312c 2030 2e31  = [0.1, 0.1, 0.1
+00000410: 2c20 302e 312c 2030 2e31 2c20 302e 312c  , 0.1, 0.1, 0.1,
+00000420: 2030 2e31 2c20 302e 312c 2030 2e31 2c20   0.1, 0.1, 0.1, 
+00000430: 302e 315d 0d0a 0d0a 5b76 616c 6964 6174  0.1]....[validat
+00000440: 696f 6e5d 0d0a 7275 6e5f 6576 6572 795f  ion]..run_every_
+00000450: 6570 6f63 6820 3d20 310d 0a0d 0a5b 6461  epoch = 1....[da
+00000460: 7461 7365 745d 0d0a 7461 7267 6574 203d  taset]..target =
+00000470: 2022 2e2f 6461 7461 6d6f 6475 6c65 2e70   "./datamodule.p
+00000480: 793a 3a4d 4e49 5354 4375 7374 6f6d 4461  y::MNISTCustomDa
+00000490: 7461 6d6f 6475 6c65 220d 0a0d 0a5b 6461  tamodule"....[da
+000004a0: 7461 7365 742e 7472 6169 6e76 616c 5d0d  taset.trainval].
+000004b0: 0a72 6f6f 745f 6469 7220 3d20 222e 2f6d  .root_dir = "./m
+000004c0: 6e69 7374 220d 0a0d 0a5b 6461 7461 7365  nist"....[datase
+000004d0: 742e 7472 6169 6e2e 6c6f 6164 6572 5d0d  t.train.loader].
+000004e0: 0a62 6174 6368 5f73 697a 6520 3d20 3135  .batch_size = 15
+000004f0: 300d 0a73 6875 6666 6c65 203d 2074 7275  0..shuffle = tru
+00000500: 650d 0a6e 756d 5f77 6f72 6b65 7273 203d  e..num_workers =
+00000510: 2034 0d0a 0d0a 5b64 6174 6173 6574 2e76   4....[dataset.v
+00000520: 616c 6964 6174 696f 6e2e 6c6f 6164 6572  alidation.loader
+00000530: 5d0d 0a62 6174 6368 5f73 697a 6520 3d20  ]..batch_size = 
+00000540: 3135 300d 0a73 6875 6666 6c65 203d 2066  150..shuffle = f
+00000550: 616c 7365 0d0a 6e75 6d5f 776f 726b 6572  alse..num_worker
+00000560: 7320 3d20 340d 0a0d 0a5b 6d65 7472 6963  s = 4....[metric
+00000570: 735d 0d0a 4d79 5072 6563 6973 696f 6e20  s]..MyPrecision 
+00000580: 3d20 7b74 6172 6765 7420 3d20 2274 6f72  = {target = "tor
+00000590: 6368 6d65 7472 6963 733a 3a50 7265 6369  chmetrics::Preci
+000005a0: 7369 6f6e 222c 2074 6173 6b20 3d20 226d  sion", task = "m
+000005b0: 756c 7469 636c 6173 7322 2c20 6e75 6d5f  ulticlass", num_
+000005c0: 636c 6173 7365 733d 3130 7d0d 0a46 4265  classes=10}..FBe
+000005d0: 7461 5363 6f72 6520 3d20 7b74 6172 6765  taScore = {targe
+000005e0: 7420 3d20 2274 6f72 6368 6d65 7472 6963  t = "torchmetric
+000005f0: 733a 3a46 4265 7461 5363 6f72 6522 2c20  s::FBetaScore", 
+00000600: 7461 736b 203d 2022 6d75 6c74 6963 6c61  task = "multicla
+00000610: 7373 222c 206e 756d 5f63 6c61 7373 6573  ss", num_classes
+00000620: 3d31 302c 2062 6574 6120 3d20 302e 317d  =10, beta = 0.1}
```

### Comparing `kit4dl-2023.9b1/examples/cnn_s3dis_segmentation/conf.toml` & `kit4dl-2023.9b2/examples/cnn_s3dis_segmentation/conf.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/cli/_templates/project/conf.toml` & `kit4dl-2023.9b2/kit4dl/cli/_templates/project/conf.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/cli/_templates/project/datamodule.py` & `kit4dl-2023.9b2/kit4dl/cli/_templates/project/datamodule.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/cli/_templates/project/model.py` & `kit4dl-2023.9b2/kit4dl/cli/_templates/project/model.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/cli/app.py` & `kit4dl-2023.9b2/kit4dl/cli/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     import tomllib as toml
 except ModuleNotFoundError:
     import toml  # type: ignore[no-redef]
 
 import typer
 from typing_extensions import Annotated
 
-from kit4dl import context
+from kit4dl import _version, context
 from kit4dl.formatting import escape_os_sep, substitute_symbols
 from kit4dl.nn.confmodels import Conf
 from kit4dl.nn.trainer import Trainer
 
 # ##############################
 #         CREATE CLI
 # ##############################
@@ -43,14 +43,19 @@
 log = logging.getLogger("Kit4DL.CLI")
 _configure_logger(log)
 
 
 # ##############################
 #         UTILS METHODS
 # ##############################
+def update_context_from_static() -> None:
+    """Update context from static attributes."""
+    context.VERSION = _version.__version__
+
+
 def update_context_from_runtime(
     prj_dir: str | None = None,
 ) -> None:
     """Update context properties from the runtime variables."""
     context.PROJECT_DIR = prj_dir
 
 
@@ -75,14 +80,18 @@
     return os.path.join(os.getcwd(), "conf.toml")
 
 
 def _remove_redundant_items(path):
     shutil.rmtree(os.path.join(path, "__pycache__"), ignore_errors=True)
 
 
+def _is_test_allowed(trainer: Trainer) -> bool:
+    return trainer.is_finished
+
+
 # ##############################
 #      COMMANDS DEFINITIONS
 # ##############################
 @_app.command()
 def init(
     name: Annotated[
         str, typer.Option(help="The name of your new project")
@@ -146,23 +155,32 @@
         raise RuntimeError(
             f"the conf file: {conf} does not exist. ensure the default"
             " configuration file exist or specify --conf argument to a valid"
             " configuration file."
         )
     prj_dir = os.path.join(os.getcwd(), root_dir)
     sys.path.append(prj_dir)
+    update_context_from_static()
     update_context_from_runtime(prj_dir=prj_dir)
     conf_ = _get_conf_from_file(conf, root_dir=root_dir)
     update_context_from_conf(conf=conf_)
     log.info("Running trainer \U0001f3ac")
     trainer = Trainer(conf=conf_).prepare()
     trainer.fit()
     log.info("Training finished \U00002728")
     if test:
+        if not _is_test_allowed(trainer):
+            return
         log.info("Running testing \U00002728")
         trainer.test()
         log.info("Testing finished \U00002728")
 
 
+@_app.command()
+def version() -> None:
+    """Display Kit4DL version."""
+    print(_version.__version__)
+
+
 def run():
     """Run the CLI app."""
     _app()
```

### Comparing `kit4dl-2023.9b1/kit4dl/context.py` & `kit4dl-2023.9b2/kit4dl/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,28 +20,30 @@
 
 
 # NOTE: below definitions will not be used, they are required
 # just for suntax suggestions and to avoid mypy [attr-defined] error
 PROJECT_DIR: Any
 LOG_LEVEL: Any
 LOG_FORMAT: Any
+VERSION: Any
 
 
 def get_dict():
     """Get dictionary of all available context-defined properties."""
 
 
 class Context:
     """Current Python session."""
 
     PROJECT_DIR: _ImmutableAttribute = _ImmutableAttribute(default=".")
     LOG_LEVEL: _ImmutableAttribute = _ImmutableAttribute(default="INFO")
     LOG_FORMAT: _ImmutableAttribute = _ImmutableAttribute(
         default="%(asctime)s - %(levelname)s - %(message)s"
     )
+    VERSION: _ImmutableAttribute = _ImmutableAttribute(default=None)
 
     def get_dict(self) -> dict:
         """Get dictionary of all available context-defined properties."""
         return {
             key: getattr(self, key)
             for key, value in type(self).__dict__.items()
             if isinstance(value, _ImmutableAttribute)
```

### Comparing `kit4dl-2023.9b1/kit4dl/dataset.py` & `kit4dl-2023.9b2/kit4dl/dataset.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/formatting.py` & `kit4dl-2023.9b2/kit4dl/formatting.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/io.py` & `kit4dl-2023.9b2/kit4dl/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 import os
 import sys
 from typing import Any
 
 from kit4dl.kit4dl_types import FullyQualifiedName
 
 _TARGET_SPLIT = "::"
+_MODULE_SEP = ".py::"
 PROJECT_DIR = "PROJECT_DIR"
 
 
+def _does_path_contain_module_file(target: str | FullyQualifiedName):
+    return target.strip().endswith(".py") or _MODULE_SEP in target
+
+
 def split_target(target: str | FullyQualifiedName) -> tuple[str, str]:
     """Split target name or fully qualified name by `::` to get the path and the attribute.
 
     Parameters
     ----------
     target : str or FullyQualifiedName
         The value of the class or Python module path
@@ -90,25 +95,27 @@
 
     ```
     >>> maybe_get_abs_target("os::PathLike", "/work/usr")
     os::PathLike
     ```
 
     """
-    if ".py" not in target:
+    if not _does_path_contain_module_file(target):
         return target
     path, attr_name = split_target(target)
     if os.path.isabs(path):
         return target
     return connect_target(os.path.join(root_dir, path), attr_name)
 
 
 def import_module_from_file(path: str, exec_module: bool = False):
     """Import module from file indicated by the relative path."""
-    assert ".py" in path, f"path: {path} is not a Python module"
+    assert _does_path_contain_module_file(
+        path
+    ), f"path: {path} is not a Python module"
     assert os.path.exists(path), f"module: {path} does not exist"
     spec = importlib.util.spec_from_file_location(
         "_file_imported_module", path
     )
     if spec is None:
         raise RuntimeError(f"module {path} is not defined")
     _file_imported_module = importlib.util.module_from_spec(spec)
@@ -187,14 +194,14 @@
         raise ValueError(
             f"missing `::` in the name: `{name}`. remember to put the double"
             " colon `::` between: \n a) the fully qualified name and the"
             " class, like `package.module::MyClass` \n 2) the module path and"
             " the class, like `/usr/my_user/my_module.py::MyClass`"
         )
     path, attr_name = split_target(name)
-    if ".py" in path:
+    if _does_path_contain_module_file(path):
         return get_class_from_py_file(path, attr_name)
     if importlib.util.find_spec(path):
         return getattr(importlib.import_module(path), attr_name)
     raise ModuleNotFoundError(
         f"module defined as `{path}` cannot be imported or found in the system"
     )
```

### Comparing `kit4dl-2023.9b1/kit4dl/metric.py` & `kit4dl-2023.9b2/kit4dl/metric.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/mixins.py` & `kit4dl-2023.9b2/kit4dl/mixins.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/nn/base.py` & `kit4dl-2023.9b2/kit4dl/nn/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,41 @@
 
 from kit4dl.metric import MetricStore
 from kit4dl.mixins import LoggerMixin
 from kit4dl.nn.confmodels import Conf
 from kit4dl.stages import Stage
 
 
+class StepOutput(dict):
+    """Output of the single train/val/test step."""
+
+    def __init__(
+        self, *, pred: torch.Tensor, true: torch.Tensor, loss: torch.Tensor
+    ):
+        super().__init__()
+        self["pred"] = pred
+        self["true"] = true
+        self["loss"] = loss
+
+    @property
+    def loss(self) -> torch.Tensor:
+        """Get loss value."""
+        return self["loss"]
+
+    @property
+    def predictions(self) -> torch.Tensor:
+        """Get predictions."""
+        return self["pred"]
+
+    @property
+    def labels(self) -> torch.Tensor:
+        """Get ground-turth labels."""
+        return self["true"]
+
+
 class Kit4DLAbstractModule(
     ABC, pl.LightningModule, LoggerMixin
 ):  # pylint: disable=too-many-ancestors
     """Base abstract class for Kit4DL modules."""
 
     def __init__(self, *, conf: Conf) -> None:
         super().__init__()
@@ -389,15 +416,15 @@
                 loss = self.compute_loss(y_scores, y_true)
             case (y_true, y_scores, loss):
                 pass
             case _:
                 self.error("wrong size of tuple returned by `run_step`")
                 raise ValueError("wrong size of tuple returned by `run_step`")
         self.update_train_metrics(true=y_true, predictions=y_scores, loss=loss)
-        return loss
+        return StepOutput(pred=y_scores, true=y_true, loss=loss)
 
     def validation_step(
         self, batch, batch_idx
     ):  # pylint: disable=arguments-differ
         """Carry out a single validation step."""
         res = self.run_val_step(batch, batch_idx)
         match res:
@@ -405,22 +432,22 @@
                 loss = self.compute_loss(y_scores, y_true)
             case (y_true, y_scores, loss):
                 pass
             case _:
                 self.error("wrong size of tuple returned by `run_step`")
                 raise ValueError("wrong size of tuple returned by `run_step`")
         self.update_val_metrics(true=y_true, predictions=y_scores, loss=loss)
-        return loss
+        return StepOutput(pred=y_scores, true=y_true, loss=loss)
 
     def test_step(self, batch, batch_idx):  # pylint: disable=arguments-differ
         """Carry out a single test step."""
         res = self.run_test_step(batch, batch_idx)
         match res:
             case (y_true, y_scores):
                 loss = self.compute_loss(y_scores, y_true)
             case (y_true, y_scores, loss):
                 pass
             case _:
                 self.error("wrong size of tuple returned by `run_step`")
                 raise ValueError("wrong size of tuple returned by `run_step`")
         self.update_test_metrics(true=y_true, predictions=y_scores, loss=loss)
-        return loss
+        return StepOutput(pred=y_scores, true=y_true, loss=loss)
```

### Comparing `kit4dl-2023.9b1/kit4dl/nn/callbacks.py` & `kit4dl-2023.9b2/kit4dl/nn/callbacks.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl/nn/confmodels.py` & `kit4dl-2023.9b2/kit4dl/nn/confmodels.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A module with configuration classes."""
 import os
 import warnings
-from functools import partial
+from functools import partial as func_partial
 from inspect import signature
 from typing import Any, Callable, Literal
 
 import lightning.pytorch.loggers as pl_logs
 import torch
 import torchmetrics as tm
 from pydantic import (
@@ -16,31 +16,34 @@
     field_validator,
     model_validator,
 )
 from pydantic.fields import FieldInfo
 from typing_extensions import Annotated
 
 import kit4dl.io as io_
+from kit4dl import Kit4DLCallback
 from kit4dl import utils as ut
 from kit4dl.kit4dl_types import FullyQualifiedName
 from kit4dl.nn.validators import (
+    validate_callback,
     validate_class_exists,
     validate_cuda_device_exists,
     validate_lr_scheduler,
     validate_metric,
 )
 
 Target = Annotated[
     FullyQualifiedName | str, AfterValidator(validate_class_exists)
 ]
 CudaDevice = Annotated[int | None, AfterValidator(validate_cuda_device_exists)]
 SchedulerDict = Annotated[
     dict[str, Any], AfterValidator(validate_lr_scheduler)
 ]
 MetricDict = Annotated[dict[str, Any], AfterValidator(validate_metric)]
+CallbackDict = Annotated[dict[str, Any], AfterValidator(validate_callback)]
 
 
 def split_extra_arguments(
     values: dict, fields: dict[str, FieldInfo], *, consider_alias: bool = False
 ) -> tuple[dict, dict]:
     """Split arguments to field-related and auxiliary."""
     extra_args: dict = {}
@@ -58,14 +61,28 @@
                 extra_args.update({key: value})
     else:
         extra_args = {k: v for k, v in values.items() if k not in fields}
         field_args = {k: v for k, v in values.items() if k in fields}
     return (field_args, extra_args)
 
 
+def create_obj_from_conf(obj_conf: dict, partial: bool = False) -> Any:
+    """Initialize object or prepared `partial` object based on configuration."""
+    obj_conf_copy = obj_conf.copy()
+    class_ = io_.import_and_get_attr_from_fully_qualified_name(
+        obj_conf_copy.pop("target")
+    )
+    if partial:
+        return func_partial(
+            class_,
+            **obj_conf_copy,
+        )
+    return class_(**obj_conf_copy)
+
+
 # ################################
 #           ABSTRACT
 # ################################
 class _AbstractClassWithArgumentsConf(BaseModel):
     model_config = ConfigDict(extra="allow", frozen=True)
     target: Target
     arguments: dict[str, Any] = Field(default_factory=dict)
@@ -155,15 +172,15 @@
 
     @property
     def optimizer(self) -> Callable[..., torch.optim.Optimizer]:
         """Get `partial` object of the preconfigured optimizer."""
         target_class = io_.import_and_get_attr_from_fully_qualified_name(
             self.target
         )
-        return partial(
+        return func_partial(
             target_class,
             lr=self.lr,
             **self.arguments,  # pylint: disable=not-a-mapping
         )
 
 
 # ################################
@@ -255,43 +272,44 @@
 # ################################
 class TrainingConf(BaseModel):
     """Training procedure configuration class."""
 
     epochs: int = Field(gt=0)
     epoch_schedulers: list[SchedulerDict] = Field(default_factory=list)
     checkpoint: CheckpointConf | None = None
+    callbacks: list[CallbackDict] = Field(default_factory=list)
     optimizer: OptimizerConf
     criterion: CriterionConf
     arguments: dict[str, Any]
 
     @model_validator(mode="before")
     def _build_model_arguments(cls, values: dict[str, Any]) -> dict[str, Any]:
         field_args, extra_args = split_extra_arguments(
             values, cls.model_fields, consider_alias=False
         )
         field_args["arguments"] = extra_args
         return field_args
 
     @property
+    def preconfigured_callbacks(self) -> list[Kit4DLCallback]:
+        """Get list of all preconfigured callbacks."""
+        callbacks: list[Kit4DLCallback] = []
+        for clb in self.callbacks:  # pylint: disable=not-an-iterable
+            callbacks.append(create_obj_from_conf(clb, partial=False))
+        return callbacks
+
+    @property
     def preconfigured_schedulers_classes(
         self,
     ) -> list[Callable]:
         """Get a list of preconfigured schedulers."""
         schedulers: list[Callable] = []
 
         for sch in self.epoch_schedulers:  # pylint: disable=not-an-iterable
-            sch_copy = sch.copy()
-            schedulers.append(
-                partial(
-                    io_.import_and_get_attr_from_fully_qualified_name(
-                        sch_copy.pop("target")
-                    ),
-                    **sch_copy,
-                )
-            )
+            schedulers.append(create_obj_from_conf(sch, partial=True))
         return schedulers
 
 
 # ################################
 #     Validation configuration
 # ################################
 class ValidationConf(BaseModel):
@@ -475,15 +493,15 @@
             raise ValueError("metrics are not defined!")
         metric_obj: dict = {}
         for metric_name, metric_args in self.metrics.items():
             metric_args_copy = metric_args.copy()
             metric_obj[metric_name.lower()] = (
                 io_.import_and_get_attr_from_fully_qualified_name(
                     metric_args_copy.pop("target")
-                )(**metric_args_copy)
+                )(**metric_args_copy).to(self.base.device)
             )
         return metric_obj
 
     @classmethod
     def override_with_abs_target(cls, root_dir: str, entries: dict) -> dict:
         """Replace in-place `target` valuesof the `entries`.
 
@@ -495,12 +513,14 @@
             Dictionary of values to replace `target` key
 
         Returns
         -------
         replaced : dict
             In-place modified `entries` dictionary
         """
-        replace_logic = partial(io_.maybe_get_abs_target, root_dir=root_dir)
+        replace_logic = func_partial(
+            io_.maybe_get_abs_target, root_dir=root_dir
+        )
         entries = ut.replace_item_recursively(
             entries, key="target", replace=replace_logic
         )
         return entries
```

### Comparing `kit4dl-2023.9b1/kit4dl/nn/trainer.py` & `kit4dl-2023.9b2/kit4dl/nn/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,34 @@
 
 
 class Trainer(LoggerMixin):
     """Class managing the training procedure."""
 
     _model: Kit4DLAbstractModule
     _datamodule: Kit4DLAbstractDataModule
-    _trainer: pl.Trainer
+    _pl_trainer: pl.Trainer
     _conf: Conf
     _metric_logger: Any
 
     def __init__(self, conf: Conf) -> None:
         self._logger = logging.getLogger("lightning.pytorch")
         self._conf = conf
         self._device = self._conf.base.device
         self._metric_logger = self._new_metric_logger()
         set_seed(self._conf.base.seed)
 
+    @property
+    def is_finished(self) -> bool:
+        """Check if training routing finished."""
+        return self._pl_trainer.state.finished
+
     def prepare(self) -> "Trainer":
         """Prepare trainer by configuring the model and data modules."""
         self._model = self._configure_model()
-        self._trainer = self._configure_trainer()
+        self._pl_trainer = self._configure_trainer()
         self._datamodule = self._configure_datamodule()
         self._log_hparams()
         return self
 
     def _log_hparams(self) -> None:
         self._metric_logger.log_hyperparams(self._conf.dict())
         self._metric_logger.log_hyperparams(
@@ -53,39 +58,39 @@
     def load_checkpoint(self, path: str) -> "Trainer":
         """Load model weights from the checkpoint."""
         self._model = type(self._model).load_from_checkpoint(path)
         return self
 
     def fit(self) -> "Trainer":
         """Fit the trainer making use of `lightning.pytorch.Trainer`."""
-        assert self._trainer, (
+        assert self._pl_trainer, (
             "trainer is not configured. did you forget to call `prepare()`"
             " method first?"
         )
-        self._trainer.fit(self._model, datamodule=self._datamodule)
+        self._pl_trainer.fit(self._model, datamodule=self._datamodule)
         return self
 
     def test(self) -> "Trainer":
         """Test the model."""
-        assert self._trainer, (
+        assert self._pl_trainer, (
             "trainer is not configured. did you forget to call `prepare()`"
             " method first?"
         )
-        self._trainer.test(
+        self._pl_trainer.test(
             self._model, datamodule=self._datamodule, ckpt_path="best"
         )
         return self
 
     def predict(self) -> "Trainer":
         """Predict values for the model."""
-        assert self._trainer, (
+        assert self._pl_trainer, (
             "trainer is not configured. did you forget to call `prepare()`"
             " method first?"
         )
-        self._trainer.predict(self._model, datamodule=self._datamodule)
+        self._pl_trainer.predict(self._model, datamodule=self._datamodule)
         return self
 
     def _new_metric_logger(self) -> pl_log.Logger:
         return self._conf.logging.metric_logger_type(
             **self._conf.logging.arguments
         )
 
@@ -116,15 +121,17 @@
             save_weights_only=chkp_conf.save_weights_only,
             every_n_epochs=chkp_conf.every_n_epochs,
             save_on_train_epoch_end=chkp_conf.save_on_train_epoch_end,
         )
 
     def _configure_trainer(self) -> pl.Trainer:
         accelerator_device, device = self._conf.base.accelerator_device_and_id
-        callbacks: list[pl_callbacks.Callback] = [MetricCallback()]
+        callbacks: list[pl_callbacks.Callback] = [
+            MetricCallback()
+        ] + self._conf.training.preconfigured_callbacks
         if self._conf.training.checkpoint:
             callbacks.append(self._get_model_checkpoint())
         return pl.Trainer(
             accelerator=accelerator_device,
             devices=device,
             max_epochs=self._conf.training.epochs,
             check_val_every_n_epoch=self._conf.validation.run_every_epoch,
```

### Comparing `kit4dl-2023.9b1/kit4dl/nn/validators.py` & `kit4dl-2023.9b2/kit4dl/nn/validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,32 @@
 """A module with resuable validators."""
 import warnings
 
 import torch
 import torchmetrics as tm
 
 import kit4dl.io as io_
+from kit4dl import Kit4DLCallback
 from kit4dl.io import import_and_get_attr_from_fully_qualified_name
 from kit4dl.kit4dl_types import FullyQualifiedName
 
 
+def validate_callback(conf: dict):
+    """Assert callback exists."""
+    assert "target" in conf, "`target` is not defined for some callbacks"
+    target_class = io_.import_and_get_attr_from_fully_qualified_name(
+        conf["target"]
+    )
+    assert issubclass(target_class, Kit4DLCallback), (
+        "custom callbacks need to be subclasses of `kit4dl.Kit4DLCallback`"
+        " class!"
+    )
+    return conf
+
+
 def validate_metric(conf: dict):
     """Assert metric exists."""
     assert "target" in conf, "`target` is not defined for some metric"
     target_class = io_.import_and_get_attr_from_fully_qualified_name(
         conf["target"]
     )
     # TODO: issubclass for torchmetrics metric does not work
```

### Comparing `kit4dl-2023.9b1/kit4dl/utils.py` & `kit4dl-2023.9b2/kit4dl/utils.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/kit4dl.egg-info/PKG-INFO` & `kit4dl-2023.9b2/kit4dl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kit4dl
-Version: 2023.9b1
+Version: 2023.9b2
 Summary: Kit4DL - A quick way to start with machine and deep learning
 Author: Jakub Walczak, Marco Mancini, Mirko Stojiljkovic, Shahbaz Alvi
 License: MIT License
         
         Copyright (c) 2023 opengeokube
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -69,15 +69,15 @@
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![pydocstyle](https://img.shields.io/badge/pydocstyle-enabled-AD4CD3)](http://www.pydocstyle.org/en/stable/)
 
 [![license](https://img.shields.io/badge/License-MIT-green.svg?labelColor=gray)](https://github.com/opengeokube/kit4dl/blob/main/LICENSE)
 
 [![pytest](https://github.com/opengeokube/kit4dl/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/opengeokube/kit4dl/actions/workflows/test.yml)
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8241376.svg)](https://doi.org/10.5281/zenodo.8241376)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8328176.svg)](https://doi.org/10.5281/zenodo.8328176)
 
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/kit4dl.svg)](https://anaconda.org/conda-forge/kit4dl) 
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/kit4dl.svg)](https://anaconda.org/conda-forge/kit4dl)
 
 [![PyPI version](https://badge.fury.io/py/kit4dl.svg)](https://badge.fury.io/py/kit4dl)
 </div>
 
@@ -95,30 +95,31 @@
 ```bibtex
 @SOFTWARE{kit4dl,
   author = {Walczak, Jakub and
             Mancini, Marco and
             Stojiljković, Mirko and
             Alvi, Shahbaz},
   title = {Kit4DL},
-  month = aug,
+  month = sep,
   year = 2023,
   note = {{Available in GitHub: https://github.com/opengeokube/kit4dl}},
   publisher = {Zenodo},
-  version = {2023.08b0},
-  doi = {10.5281/zenodo.8241376},
-  url = {https://doi.org/10.5281/zenodo.8241376}
+  version = {2023.9b1},
+  doi = {10.5281/zenodo.8328176},
+  url = {https://doi.org/10.5281/zenodo.8328176}
 }
 ```
 ## 🚧 Roadmap
 
 > **Warning**: Kit4DL is currently in its alpha stage. All recommendations are welcomed.
 
 - [ ] add handling sklearn-like models
 - [ ] add functionality to serve the model
 - [x] enable custom metrics
+- [x] enable using callbacks (also custom ones)
 - [ ] write more unit tests
 
 
 ## 🎬 Quickstart
 
 ### Getting started
 
@@ -450,18 +451,91 @@
 #### Configuring training
 Training-related arguments should be defined in the `[training]` section of the configuration file.
 You can define the following arguments.
 
 |   **Property** 	|  **Type**        |         **Details**              |
 |---------------	|----------------- | -------------------------------- | 
 |      `epochs`*    |   `int > 0`      |  number of epochs	              | 
+|      `callbacks`  |   `list`         |  list of callbacks	              | 
 |`epoch_schedulers` |  `list of dict`  |  list of schedulers definitions  |
 
 > **Note**: Arguments marked with `*` are obligatory!
 
+You can define a list of custom callbacks applied in the training process. Your callbacks need to be subclasses of `lightning.pytorch.callbacks.Callback` or `kit4dl.Kit4DLCallback` (for convenience) class and define one/some of the methods indicated in the [PyTorch-Lightning callback API](https://lightning.ai/docs/pytorch/stable/extensions/callbacks.html#callback-api). You can always use one of the [predefined callbacks](https://lightning.ai/docs/pytorch/stable/extensions/callbacks.html#built-in-callbacks).
+
+
+```toml
+[training]
+callbacks = [
+    {target = "./callbacks.py::SaveConfusionMatrixCallback", task="multiclass", num_classes=10, save_dir="{{ PROJECT_DIR }}/cm},
+    {target = "lightning.pytorch.callbacks::DeviceStatsMonitor"}
+]
+```
+
+Where the 1st callback is user-defined and the other - PyTorch-Loghtning built-in. For the custom callback we need to provide a class (here: located in the `callbacks.py` file in the project directory, the class is named `SaveConfusionMatrixCallback`).
+
+```python
+import os
+from typing import Any
+
+import lightning.pytorch as pl
+import torchmetrics as tm
+
+from kit4dl import Kit4DLCallback, StepOutput
+
+
+class SaveConfusionMatrixCallback(Kit4DLCallback):
+    _cm: tm.ConfusionMatrix
+    _num_classes: int
+    _task: str
+    _save_dir: str
+
+    def __init__(self, task: str, num_classes: int, save_dir: str) -> None:
+        super().__init__()
+        self._num_classes = num_classes
+        self._save_dir = save_dir
+        self._task = task
+        os.makedirs(self._save_dir, exist_ok=True)
+
+    def on_validation_epoch_start(
+        self, trainer: pl.Trainer, pl_module: pl.LightningModule
+    ) -> None:
+        self._cm = tm.ConfusionMatrix(
+            task=self._task, num_classes=self._num_classes
+        )
+
+    def on_validation_batch_end(
+        self,
+        trainer: pl.Trainer,
+        pl_module: pl.LightningModule,
+        outputs: StepOutput,
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int = 0,
+    ) -> None:
+        self._cm.update(outputs.predictions, outputs.labels)
+
+    def on_validation_epoch_end(
+        self, trainer: pl.Trainer, pl_module: pl.LightningModule
+    ) -> None:
+        """Called when the val epoch ends."""
+        fig, _ = self._cm.plot()
+        target_file = os.path.join(
+            self._save_dir,
+            f"confusion_matrix_for_epoch_{pl_module.current_epoch}",
+        )
+        fig.savefig(target_file)
+
+```
+
+
+
+
+
+
 Besides those listed in the table above, you can specify PyTorch Lightning-related `Trainer` arguments, like:
 1. `accumulate_grad_batches`
 1. `gradient_clip_val`
 1. `gradient_clip_algorithm`
 1. ...
 
 ##### ✍️ Example
@@ -623,8 +697,9 @@
 
 The constants currently available in `kit4dl` are the following:
 |   **Symbol** 	|            **Meaning of the symbol**                                   	|          **Example**                  |
 |-------------	|-----------------------------------------------------------------------	| -----------------------------------	|
 | `PROJECT_DIR`	| the home directory of the TOML configuration file (project directory) 	| `context.PROJECT_DIR`                 |
 | `LOG_LEVEL`	| logging level as defined in the configuration TOML file                	| `context.LOG_LEVEL`                   |
 | `LOG_FORMAT`	| logging message format as defined in the configuration TOML file      	| `context.LOG_FORMAT`                  |
+|  `VERSION`	| the current version of the package                                      	| `context.VERSION`                     |
```

### Comparing `kit4dl-2023.9b1/kit4dl.egg-info/SOURCES.txt` & `kit4dl-2023.9b2/kit4dl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 examples/cnn_mnist_classification/conf.toml
 examples/cnn_s3dis_segmentation/conf.toml
 kit4dl/__init__.py
+kit4dl/_version.py
 kit4dl/context.py
 kit4dl/dataset.py
 kit4dl/formatting.py
 kit4dl/io.py
 kit4dl/kit4dl_types.py
 kit4dl/metric.py
 kit4dl/mixins.py
```

### Comparing `kit4dl-2023.9b1/pyproject.toml` & `kit4dl-2023.9b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kit4dl"
-version = "2023.9b1"
 description = "Kit4DL - A quick way to start with machine and deep learning"
 requires-python = ">=3.10"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["deep learning", "training pipeline"]
+dynamic = ["version"]
 authors = [
     {name = "Jakub Walczak"},
     {name = "Marco Mancini"},
     {name = "Mirko Stojiljkovic"},
     {name = "Shahbaz Alvi"},
 ]
 classifiers = [
@@ -44,14 +44,17 @@
     "tqdm>=4.57.0,<4.67.0",
     "typing-extensions>=4.0.0,<4.8.0; python_version<='3.11'",
     "Jinja2<3.2.0",
     "typer[all]",
     "toml; python_version<'3.11'"
 ]
 
+[tool.setuptools.dynamic]
+version = {attr = "kit4dl._version.__version__"}
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["examples*"]
```

### Comparing `kit4dl-2023.9b1/tests/cli/test_app.py` & `kit4dl-2023.9b2/tests/cli/test_app.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/dummy_module.py` & `kit4dl-2023.9b2/tests/dummy_module.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/fixtures.py` & `kit4dl-2023.9b2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/nn/test_base.py` & `kit4dl-2023.9b2/tests/nn/test_base.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/nn/test_confmodels.py` & `kit4dl-2023.9b2/tests/nn/test_confmodels.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     experiment_name = "handwritten_digit_classification"
         """
         conf = BaseConf(**toml.loads(load))
         assert conf.seed == 0
         assert conf.cuda_id is None
         assert conf.experiment_name == "handwritten_digit_classification"
 
+    @skipnocuda
     def test_base_conf_failed_on_missing_exp_name(self):
         load = """
     seed = 10
     cuda_id = 1
         """
         with pytest.raises(ValidationError):
             _ = BaseConf(**toml.loads(load))
@@ -83,14 +84,15 @@
     def test_base_conf_failed_on_wrong_seed(self):
         load = """
     seed_id = -10
         """
         with pytest.raises(ValidationError):
             _ = BaseConf(**toml.loads(load))
 
+    @skipnocuda
     def test_base_conf_failed_on_wrong_cuda_id(self):
         load = """
     cuda_id = -1
         """
         with pytest.raises(ValidationError):
             _ = BaseConf(**toml.loads(load))
```

### Comparing `kit4dl-2023.9b1/tests/nn/test_trainer.py` & `kit4dl-2023.9b2/tests/nn/test_trainer.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/nn/test_validators.py` & `kit4dl-2023.9b2/tests/nn/test_validators.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/resources/dataset.py` & `kit4dl-2023.9b2/tests/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/resources/model.py` & `kit4dl-2023.9b2/tests/resources/model.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/resources/test_file.toml` & `kit4dl-2023.9b2/tests/resources/test_file.toml`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/test_context.py` & `kit4dl-2023.9b2/tests/test_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 
 class TestSession:
     @pytest.fixture(autouse=True, scope="class")
     def set_session_attributes(self):
         context.LOG_LEVEL = "INFO"
         context.LOG_FORMAT = "%(asctime)s"
         context.PROJECT_DIR = "/work/my_dir"
+        context.VERSION = "0.0.1"
         yield
 
     @pytest.mark.parametrize(
-        "session_attr", ["LOG_LEVEL", "LOG_FORMAT", "PROJECT_DIR"]
+        "session_attr", ["LOG_LEVEL", "LOG_FORMAT", "PROJECT_DIR", "VERSION"]
     )
     def test_fail_on_successive_session_attribute_set(self, session_attr):
         with pytest.raises(
             RuntimeError, match=r"Session properties can be set only once"
         ):
             setattr(context, session_attr, "new_value")
```

### Comparing `kit4dl-2023.9b1/tests/test_formatting.py` & `kit4dl-2023.9b2/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/test_io.py` & `kit4dl-2023.9b2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kit4dl-2023.9b1/tests/test_metrics.py` & `kit4dl-2023.9b2/tests/test_metrics.py`

 * *Files identical despite different names*


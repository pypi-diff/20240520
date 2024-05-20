# Comparing `tmp/vvdutils-0.0.3.tar.gz` & `tmp/vvdutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvdutils-0.0.3.tar", last modified: Thu May 16 10:01:12 2024, max compression
+gzip compressed data, was "vvdutils-0.0.4.tar", last modified: Mon May 20 03:54:16 2024, max compression
```

## Comparing `vvdutils-0.0.3.tar` & `vvdutils-0.0.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     1068 2024-05-10 03:45:03.000000 vvdutils-0.0.3/LICENSE
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      283 2024-05-16 10:01:12.197102 vvdutils-0.0.3/PKG-INFO
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      256 2024-05-10 03:50:57.000000 vvdutils-0.0.3/README.md
--rw-rw-r--   0 vvd       (1000) vvd       (1000)       38 2024-05-16 10:01:12.197102 vvdutils-0.0.3/setup.cfg
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     1316 2024-05-16 10:00:59.000000 vvdutils-0.0.3/setup.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.193102 vvdutils-0.0.3/vvdutils/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)       52 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/__init__.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.193102 vvdutils-0.0.3/vvdutils/assets/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/assets/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     4792 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/assets/color_list.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    66531 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/assets/det.json
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.193102 vvdutils-0.0.3/vvdutils/assets/evaluator/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/assets/evaluator/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     9331 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/assets/everytime3p.jpg
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     6723 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/assets/mc.json
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     7736 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/assets/ml.json
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.193102 vvdutils-0.0.3/vvdutils/lib/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      364 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/__init__.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.193102 vvdutils-0.0.3/vvdutils/lib/data/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      157 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/data/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    19146 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/data/base.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     4829 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/data/builder.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     3185 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/data/class_mapper.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    11810 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/data/format.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     6745 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/data/info.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     3595 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/data/saver.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/lib/evaluator/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      227 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/evaluator/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     7067 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/evaluator/base.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    13953 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/evaluator/detection.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     2127 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/evaluator/multi_class.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    13625 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/evaluator/multi_label.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/lib/labelme/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)       79 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/labelme/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     3133 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/labelme/labelme.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      595 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/labelme/main.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     3503 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/labelme/polygon.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     1449 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/labelme/utils.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/lib/mario/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      155 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/mario/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      621 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/mario/databus.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      457 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/mario/hook.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    12293 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/mario/pipeline.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      330 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/mario/register.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     3620 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/mario/utils.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/lib/processing/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      253 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/processing/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     5003 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/processing/array_processing.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     8642 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/processing/box_processing.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    12696 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/processing/circle_processing.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      296 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/processing/feature_processing.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    60581 2024-05-16 09:49:07.000000 vvdutils-0.0.3/vvdutils/lib/processing/image_processing.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     7264 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/processing/math_processing.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     7499 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/processing/multi_processing.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      374 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/processing/net_processing.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/lib/utils/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      458 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     2132 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/add_utils.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)       98 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    32284 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/eval_metrics.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     4376 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/example.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     3023 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/plot_confusion_matrix.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     2789 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/tmp_file.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     1088 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/utils.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     2145 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/coding_related.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     1434 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/eva_utils.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      632 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/id_related.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    18521 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/mean_ap.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     1289 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/path_related.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     8880 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/register.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     1276 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/torch_utils.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    51445 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/lib/utils/utils.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      162 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/mttest.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/tests/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/tests/__init__.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/tests/test_data/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/tests/test_data/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     6024 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/tests/test_data/test_data.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils/tests/test_utils/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/tests/test_utils/__init__.py
--rw-rw-r--   0 vvd       (1000) vvd       (1000)    13721 2024-05-10 09:26:38.000000 vvdutils-0.0.3/vvdutils/tests/test_utils/test_utils.py
-drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-16 10:01:12.197102 vvdutils-0.0.3/vvdutils.egg-info/
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      283 2024-05-16 10:01:12.000000 vvdutils-0.0.3/vvdutils.egg-info/PKG-INFO
--rw-rw-r--   0 vvd       (1000) vvd       (1000)     2504 2024-05-16 10:01:12.000000 vvdutils-0.0.3/vvdutils.egg-info/SOURCES.txt
--rw-rw-r--   0 vvd       (1000) vvd       (1000)        1 2024-05-16 10:01:12.000000 vvdutils-0.0.3/vvdutils.egg-info/dependency_links.txt
--rw-rw-r--   0 vvd       (1000) vvd       (1000)        1 2024-05-16 09:59:48.000000 vvdutils-0.0.3/vvdutils.egg-info/not-zip-safe
--rw-rw-r--   0 vvd       (1000) vvd       (1000)      106 2024-05-16 10:01:12.000000 vvdutils-0.0.3/vvdutils.egg-info/requires.txt
--rw-rw-r--   0 vvd       (1000) vvd       (1000)        9 2024-05-16 10:01:12.000000 vvdutils-0.0.3/vvdutils.egg-info/top_level.txt
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     1068 2024-05-10 03:45:03.000000 vvdutils-0.0.4/LICENSE
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      283 2024-05-20 03:54:16.742244 vvdutils-0.0.4/PKG-INFO
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      256 2024-05-10 03:50:57.000000 vvdutils-0.0.4/README.md
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)       38 2024-05-20 03:54:16.742244 vvdutils-0.0.4/setup.cfg
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     1316 2024-05-20 03:54:00.000000 vvdutils-0.0.4/setup.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)       52 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/__init__.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/assets/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/assets/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     4792 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/assets/color_list.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    66531 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/assets/det.json
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/assets/evaluator/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/assets/evaluator/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     9331 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/assets/everytime3p.jpg
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     6723 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/assets/mc.json
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     7736 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/assets/ml.json
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/lib/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      364 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/__init__.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/lib/data/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      157 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/data/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    19146 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/data/base.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     4829 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/data/builder.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     3185 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/data/class_mapper.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    11810 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/data/format.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     6745 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/data/info.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     3595 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/data/saver.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/lib/evaluator/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      227 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/evaluator/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     7067 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/evaluator/base.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    13953 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/evaluator/detection.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     2127 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/evaluator/multi_class.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    13625 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/evaluator/multi_label.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/lib/labelme/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)       79 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/labelme/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     3133 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/labelme/labelme.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      595 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/labelme/main.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     3503 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/labelme/polygon.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     1449 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/labelme/utils.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/lib/mario/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      155 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/mario/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      621 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/mario/databus.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      457 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/mario/hook.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    12293 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/mario/pipeline.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      330 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/mario/register.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     3620 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/mario/utils.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/lib/processing/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      253 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/processing/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     5003 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/processing/array_processing.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     8642 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/processing/box_processing.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    12696 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/processing/circle_processing.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      296 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/processing/feature_processing.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    60581 2024-05-16 09:49:07.000000 vvdutils-0.0.4/vvdutils/lib/processing/image_processing.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     8100 2024-05-20 03:52:29.000000 vvdutils-0.0.4/vvdutils/lib/processing/math_processing.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     7499 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/processing/multi_processing.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      374 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/processing/net_processing.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/lib/utils/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      458 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     2132 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/add_utils.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)       98 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    32284 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/eval_metrics.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     4376 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/example.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     3023 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/plot_confusion_matrix.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     2789 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/tmp_file.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     1088 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/utils.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     2145 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/coding_related.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     1434 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/eva_utils.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      632 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/id_related.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    18521 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/mean_ap.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     1289 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/path_related.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     8880 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/register.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     1276 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/torch_utils.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    51445 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/lib/utils/utils.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      162 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/mttest.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/tests/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/tests/__init__.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/tests/test_data/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/tests/test_data/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     6024 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/tests/test_data/test_data.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils/tests/test_utils/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)        0 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/tests/test_utils/__init__.py
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)    13721 2024-05-10 09:26:38.000000 vvdutils-0.0.4/vvdutils/tests/test_utils/test_utils.py
+drwxrwxr-x   0 vvd       (1000) vvd       (1000)        0 2024-05-20 03:54:16.742244 vvdutils-0.0.4/vvdutils.egg-info/
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      283 2024-05-20 03:54:16.000000 vvdutils-0.0.4/vvdutils.egg-info/PKG-INFO
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)     2504 2024-05-20 03:54:16.000000 vvdutils-0.0.4/vvdutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)        1 2024-05-20 03:54:16.000000 vvdutils-0.0.4/vvdutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)        1 2024-05-20 03:54:16.000000 vvdutils-0.0.4/vvdutils.egg-info/not-zip-safe
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)      106 2024-05-20 03:54:16.000000 vvdutils-0.0.4/vvdutils.egg-info/requires.txt
+-rw-rw-r--   0 vvd       (1000) vvd       (1000)        9 2024-05-20 03:54:16.000000 vvdutils-0.0.4/vvdutils.egg-info/top_level.txt
```

### Comparing `vvdutils-0.0.3/LICENSE` & `vvdutils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/setup.py` & `vvdutils-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import setuptools
 from setuptools import find_packages, setup
 from numpy.distutils.core import setup
 from numpy.distutils.misc_util import Configuration
 from os.path import join, dirname, realpath
 
-str_version = '0.0.3'
+str_version = '0.0.4'
 
 
 
 def configuration(parent_package='', top_path=''):
     # this will automatically build the scattering extensions, using the
     # setup.py files located in their subdirectories
     config = Configuration(None, parent_package, top_path)
```

### Comparing `vvdutils-0.0.3/vvdutils/assets/color_list.py` & `vvdutils-0.0.4/vvdutils/assets/color_list.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/assets/det.json` & `vvdutils-0.0.4/vvdutils/assets/det.json`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/assets/everytime3p.jpg` & `vvdutils-0.0.4/vvdutils/assets/everytime3p.jpg`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/assets/mc.json` & `vvdutils-0.0.4/vvdutils/assets/mc.json`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/assets/ml.json` & `vvdutils-0.0.4/vvdutils/assets/ml.json`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/data/base.py` & `vvdutils-0.0.4/vvdutils/lib/data/base.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/data/builder.py` & `vvdutils-0.0.4/vvdutils/lib/data/builder.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/data/class_mapper.py` & `vvdutils-0.0.4/vvdutils/lib/data/class_mapper.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/data/format.py` & `vvdutils-0.0.4/vvdutils/lib/data/format.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/data/info.py` & `vvdutils-0.0.4/vvdutils/lib/data/info.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/data/saver.py` & `vvdutils-0.0.4/vvdutils/lib/data/saver.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/evaluator/base.py` & `vvdutils-0.0.4/vvdutils/lib/evaluator/base.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/evaluator/detection.py` & `vvdutils-0.0.4/vvdutils/lib/evaluator/detection.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/evaluator/multi_class.py` & `vvdutils-0.0.4/vvdutils/lib/evaluator/multi_class.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/evaluator/multi_label.py` & `vvdutils-0.0.4/vvdutils/lib/evaluator/multi_label.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/labelme/labelme.py` & `vvdutils-0.0.4/vvdutils/lib/labelme/labelme.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/labelme/main.py` & `vvdutils-0.0.4/vvdutils/lib/labelme/main.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/labelme/polygon.py` & `vvdutils-0.0.4/vvdutils/lib/labelme/polygon.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/labelme/utils.py` & `vvdutils-0.0.4/vvdutils/lib/labelme/utils.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/mario/databus.py` & `vvdutils-0.0.4/vvdutils/lib/mario/databus.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/mario/pipeline.py` & `vvdutils-0.0.4/vvdutils/lib/mario/pipeline.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/mario/utils.py` & `vvdutils-0.0.4/vvdutils/lib/mario/utils.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/processing/array_processing.py` & `vvdutils-0.0.4/vvdutils/lib/processing/array_processing.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/processing/box_processing.py` & `vvdutils-0.0.4/vvdutils/lib/processing/box_processing.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/processing/circle_processing.py` & `vvdutils-0.0.4/vvdutils/lib/processing/circle_processing.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/processing/image_processing.py` & `vvdutils-0.0.4/vvdutils/lib/processing/image_processing.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/processing/math_processing.py` & `vvdutils-0.0.4/vvdutils/lib/processing/math_processing.py`

 * *Files 19% similar despite different names*

```diff
@@ -268,8 +268,29 @@
 
     mean_x = np.mean(point_array[:, 0])
     mean_y = np.mean(point_array[:, 1])
     sigma_x = np.std(point_array[:, 0])
     sigma_y = np.std(point_array[:, 1])
 
     rho = ((point_array[:, 0] * point_array[:, 1]).mean() - mean_x * mean_y) / (sigma_x * sigma_y)
-    return mean_x, mean_y, sigma_x, sigma_y, rho
+    return mean_x, mean_y, sigma_x, sigma_y, rho
+
+# 计算距离
+def getDistance(latA, lonA, latB, lonB):
+    ra = 6378140  # 赤道半径
+    rb = 6356755  # 极半径
+    flatten = (ra - rb) / ra  # Partial rate of the earth
+    # change angle to radians
+    radLatA = math.radians(latA)
+    radLonA = math.radians(lonA)
+    radLatB = math.radians(latB)
+    radLonB = math.radians(lonB)
+ 
+    pA = math.atan(rb / ra * math.tan(radLatA))
+    pB = math.atan(rb / ra * math.tan(radLatB))
+    x = math.acos(math.sin(pA) * math.sin(pB) + math.cos(pA) * math.cos(pB) * math.cos(radLonA - radLonB))
+    c1 = (math.sin(x) - x) * (math.sin(pA) + math.sin(pB)) ** 2 / math.cos(x / 2) ** 2
+    c2 = (math.sin(x) + x) * (math.sin(pA) - math.sin(pB)) ** 2 / math.sin(x / 2) ** 2
+    dr = flatten / 8 * (c1 - c2)
+    distance = ra * (x + dr)
+    distance = round(distance , 4)
+    return distance
```

### Comparing `vvdutils-0.0.3/vvdutils/lib/processing/multi_processing.py` & `vvdutils-0.0.4/vvdutils/lib/processing/multi_processing.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/add_utils.py` & `vvdutils-0.0.4/vvdutils/lib/utils/add_utils.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/eval_metrics.py` & `vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/example.py` & `vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/example.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/plot_confusion_matrix.py` & `vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/plot_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/tmp_file.py` & `vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/tmp_file.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/classifier_eval/utils.py` & `vvdutils-0.0.4/vvdutils/lib/utils/classifier_eval/utils.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/coding_related.py` & `vvdutils-0.0.4/vvdutils/lib/utils/coding_related.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/eva_utils.py` & `vvdutils-0.0.4/vvdutils/lib/utils/eva_utils.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/id_related.py` & `vvdutils-0.0.4/vvdutils/lib/utils/id_related.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/mean_ap.py` & `vvdutils-0.0.4/vvdutils/lib/utils/mean_ap.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/path_related.py` & `vvdutils-0.0.4/vvdutils/lib/utils/path_related.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/register.py` & `vvdutils-0.0.4/vvdutils/lib/utils/register.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/torch_utils.py` & `vvdutils-0.0.4/vvdutils/lib/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/lib/utils/utils.py` & `vvdutils-0.0.4/vvdutils/lib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/tests/test_data/test_data.py` & `vvdutils-0.0.4/vvdutils/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils/tests/test_utils/test_utils.py` & `vvdutils-0.0.4/vvdutils/tests/test_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `vvdutils-0.0.3/vvdutils.egg-info/SOURCES.txt` & `vvdutils-0.0.4/vvdutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*


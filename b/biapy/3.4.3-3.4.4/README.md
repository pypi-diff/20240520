# Comparing `tmp/biapy-3.4.3.tar.gz` & `tmp/biapy-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biapy-3.4.3.tar", last modified: Thu May 16 10:34:24 2024, max compression
+gzip compressed data, was "biapy-3.4.4.tar", last modified: Mon May 20 13:25:06 2024, max compression
```

## Comparing `biapy-3.4.3.tar` & `biapy-3.4.4.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.306904 biapy-3.4.3/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1079 2023-03-09 07:44:00.000000 biapy-3.4.3/LICENSE.md
--rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23500 2024-05-16 10:34:24.306904 biapy-3.4.3/PKG-INFO
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    20933 2024-02-13 08:39:35.000000 biapy-3.4.3/README.md
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.294904 biapy-3.4.3/biapy/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2097 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19898 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/_biapy.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.294904 biapy-3.4.3/biapy/config/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       22 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/config/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    75082 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/config/config.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/data/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        0 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/data/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    45284 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/data_2D_manipulation.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    66558 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/data_3D_manipulation.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/data/generators/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    27960 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    66734 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/augmentors.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    69136 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/pair_base_data_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5616 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/pair_data_2D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7835 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/pair_data_3D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22270 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/single_base_data_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1612 2024-01-10 14:29:17.000000 biapy-3.4.3/biapy/data/generators/single_data_2D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2864 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/data/generators/single_data_3D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19467 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/test_pair_data_generators.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10987 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/test_single_data_generator.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/data/post_processing/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3028 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/data/post_processing/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    76226 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/post_processing/post_processing.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10434 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/data/post_processing/smooth_tiled_predictions.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    59305 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/pre_processing.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/engine/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2606 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/engine/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    91979 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/base_workflow.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    60972 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/check_configuration.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    16287 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/classification.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22609 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/engine/denoising.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    53230 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/detection.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13410 2024-04-14 17:17:46.000000 biapy-3.4.3/biapy/engine/image_to_image.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    48723 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/instance_seg.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    25026 2024-04-14 17:17:46.000000 biapy-3.4.3/biapy/engine/metrics.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/engine/schedulers/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      956 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/engine/schedulers/warmup_cosine_decay.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21105 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/engine/self_supervised.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11246 2024-04-14 17:17:46.000000 biapy-3.4.3/biapy/engine/semantic_seg.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13055 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/engine/super_resolution.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4952 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/train_engine.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.302904 biapy-3.4.3/biapy/models/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11931 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/models/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7576 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/attention_unet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    17636 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/models/blocks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3637 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/dfcan.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3305 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/edsr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1221 2024-02-08 07:25:10.000000 biapy-3.4.3/biapy/models/efficientnet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18966 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/models/mae.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13552 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/multiresunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2732 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/rcan.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     9139 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/resunet++.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7451 2024-02-26 08:40:58.000000 biapy-3.4.3/biapy/models/resunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7231 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/seunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2998 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/models/simple_cnn.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1734 2024-02-15 12:34:02.000000 biapy-3.4.3/biapy/models/tr_layers.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7186 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/unet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10300 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/models/unetr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3592 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/models/vit.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2982 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/wdsr.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.302904 biapy-3.4.3/biapy/utils/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4243 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/callbacks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    12958 2024-04-13 10:16:32.000000 biapy-3.4.3/biapy/utils/matching.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    14861 2024-02-15 12:34:02.000000 biapy-3.4.3/biapy/utils/misc.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.302904 biapy-3.4.3/biapy/utils/scripts/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3617 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/calculate_detection_metrics.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5803 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/calculate_metrics_3D.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5021 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/create_probability_csv.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1808 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/crop_2D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1171 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/crop_3D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1828 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/crop_and_discard_3D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1726 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/detection_plots.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4873 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/detection_probs_to_points.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2374 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/fill_holes_in_seg_masks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3864 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/filter_close_points.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1895 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/from_class_csv_to_folders.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      674 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/h5_to_tif.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1212 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/h5_to_zarr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2328 2024-04-27 18:57:13.000000 biapy-3.4.3/biapy/utils/scripts/lightmycell_data_preparation.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      920 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/merge_dataset_channels.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2538 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/order_axes.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)   118081 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/utils/scripts/run_checks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      966 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/tif_to_h5.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    57739 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/utils/util.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.302904 biapy-3.4.3/biapy.egg-info/
--rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23500 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/PKG-INFO
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2737 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/SOURCES.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        1 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/dependency_links.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       37 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/entry_points.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      348 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/requires.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        6 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/top_level.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1718 2024-05-16 10:34:12.000000 biapy-3.4.3/pyproject.toml
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       38 2024-05-16 10:34:24.306904 biapy-3.4.3/setup.cfg
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.881924 biapy-3.4.4/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1079 2023-03-09 07:44:00.000000 biapy-3.4.4/LICENSE.md
+-rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23500 2024-05-20 13:25:06.881924 biapy-3.4.4/PKG-INFO
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    20933 2024-02-13 08:39:35.000000 biapy-3.4.4/README.md
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.869923 biapy-3.4.4/biapy/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2097 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19898 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/_biapy.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.873924 biapy-3.4.4/biapy/config/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       22 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/config/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    77124 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/config/config.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.873924 biapy-3.4.4/biapy/data/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        0 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/data/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    45284 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/data/data_2D_manipulation.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    69029 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/data/data_3D_manipulation.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.873924 biapy-3.4.4/biapy/data/generators/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    28052 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/data/generators/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    66734 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/data/generators/augmentors.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    67906 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/data/generators/pair_base_data_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5616 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/data/generators/pair_data_2D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7835 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/data/generators/pair_data_3D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22270 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/data/generators/single_base_data_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1612 2024-01-10 14:29:17.000000 biapy-3.4.4/biapy/data/generators/single_data_2D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2864 2024-04-12 16:11:48.000000 biapy-3.4.4/biapy/data/generators/single_data_3D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19467 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/data/generators/test_pair_data_generators.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10987 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/data/generators/test_single_data_generator.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.873924 biapy-3.4.4/biapy/data/post_processing/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3028 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/data/post_processing/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    76226 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/data/post_processing/post_processing.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10434 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/data/post_processing/smooth_tiled_predictions.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    65651 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/data/pre_processing.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.877924 biapy-3.4.4/biapy/engine/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2606 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/engine/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    94472 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/engine/base_workflow.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    62642 2024-05-20 13:24:05.000000 biapy-3.4.4/biapy/engine/check_configuration.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    16287 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/engine/classification.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22609 2024-04-12 16:11:48.000000 biapy-3.4.4/biapy/engine/denoising.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    53230 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/engine/detection.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13410 2024-04-14 17:17:46.000000 biapy-3.4.4/biapy/engine/image_to_image.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    52821 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/engine/instance_seg.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    25026 2024-04-14 17:17:46.000000 biapy-3.4.4/biapy/engine/metrics.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.877924 biapy-3.4.4/biapy/engine/schedulers/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      956 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/engine/schedulers/warmup_cosine_decay.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21105 2024-04-12 16:11:48.000000 biapy-3.4.4/biapy/engine/self_supervised.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11246 2024-04-14 17:17:46.000000 biapy-3.4.4/biapy/engine/semantic_seg.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13055 2024-04-12 16:11:48.000000 biapy-3.4.4/biapy/engine/super_resolution.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4952 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/engine/train_engine.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.877924 biapy-3.4.4/biapy/models/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11931 2024-04-12 16:11:48.000000 biapy-3.4.4/biapy/models/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7576 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/attention_unet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    17636 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/models/blocks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3637 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/dfcan.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3305 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/edsr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1221 2024-02-08 07:25:10.000000 biapy-3.4.4/biapy/models/efficientnet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18966 2024-05-16 10:33:18.000000 biapy-3.4.4/biapy/models/mae.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13552 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/multiresunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2732 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/rcan.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     9139 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/resunet++.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7451 2024-02-26 08:40:58.000000 biapy-3.4.4/biapy/models/resunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7231 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/seunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2998 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/models/simple_cnn.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1734 2024-02-15 12:34:02.000000 biapy-3.4.4/biapy/models/tr_layers.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7186 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/unet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10300 2024-04-12 16:11:48.000000 biapy-3.4.4/biapy/models/unetr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3592 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/models/vit.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2982 2024-02-25 18:32:47.000000 biapy-3.4.4/biapy/models/wdsr.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.881924 biapy-3.4.4/biapy/utils/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4243 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/callbacks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    12958 2024-04-13 10:16:32.000000 biapy-3.4.4/biapy/utils/matching.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    14861 2024-02-15 12:34:02.000000 biapy-3.4.4/biapy/utils/misc.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.881924 biapy-3.4.4/biapy/utils/scripts/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3617 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/calculate_detection_metrics.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5803 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/calculate_metrics_3D.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5021 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/create_probability_csv.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1808 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/crop_2D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1171 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/crop_3D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1828 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/crop_and_discard_3D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1726 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/detection_plots.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4873 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/detection_probs_to_points.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2374 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/fill_holes_in_seg_masks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3864 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/filter_close_points.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1895 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/from_class_csv_to_folders.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      674 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/h5_to_tif.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1212 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/h5_to_zarr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2328 2024-04-27 18:57:13.000000 biapy-3.4.4/biapy/utils/scripts/lightmycell_data_preparation.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      920 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/merge_dataset_channels.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2538 2024-01-04 12:54:41.000000 biapy-3.4.4/biapy/utils/scripts/order_axes.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)   134975 2024-05-20 13:24:05.000000 biapy-3.4.4/biapy/utils/scripts/run_checks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      967 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/utils/scripts/tif_to_h5.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1293 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/utils/scripts/tif_to_zarr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    58763 2024-05-19 17:17:27.000000 biapy-3.4.4/biapy/utils/util.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-20 13:25:06.881924 biapy-3.4.4/biapy.egg-info/
+-rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23500 2024-05-20 13:25:06.000000 biapy-3.4.4/biapy.egg-info/PKG-INFO
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2772 2024-05-20 13:25:06.000000 biapy-3.4.4/biapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        1 2024-05-20 13:25:06.000000 biapy-3.4.4/biapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       37 2024-05-20 13:25:06.000000 biapy-3.4.4/biapy.egg-info/entry_points.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      348 2024-05-20 13:25:06.000000 biapy-3.4.4/biapy.egg-info/requires.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        6 2024-05-20 13:25:06.000000 biapy-3.4.4/biapy.egg-info/top_level.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1718 2024-05-20 13:24:05.000000 biapy-3.4.4/pyproject.toml
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       38 2024-05-20 13:25:06.881924 biapy-3.4.4/setup.cfg
```

### Comparing `biapy-3.4.3/LICENSE.md` & `biapy-3.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/PKG-INFO` & `biapy-3.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biapy
-Version: 3.4.3
+Version: 3.4.4
 Summary: BiaPy: Bioimage analysis pipelines in Python
 Author-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 Maintainer-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 License: MIT License
         
         Copyright (c) 2022 Daniel Franco-Barranco
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biapy Version: 3.4.3 Summary: BiaPy: Bioimage
+Metadata-Version: 2.1 Name: biapy Version: 3.4.4 Summary: BiaPy: Bioimage
 analysis pipelines in Python Author-email: Daniel Franco-Barranco
 dipc.org> Maintainer-email: Daniel Franco-Barranco
 dipc.org> License: MIT License Copyright (c) 2022 Daniel Franco-Barranco
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `biapy-3.4.3/README.md` & `biapy-3.4.4/README.md`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/__init__.py` & `biapy-3.4.4/biapy/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/_biapy.py` & `biapy-3.4.4/biapy/_biapy.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/config/config.py` & `biapy-3.4.4/biapy/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,21 @@
         # Train
         _C.DATA.TRAIN = CN()
         # Whether to check if the data mask contains correct values, e.g. same classes as defined
         _C.DATA.TRAIN.CHECK_DATA = True
         _C.DATA.TRAIN.IN_MEMORY = True
         _C.DATA.TRAIN.PATH = os.path.join("user_data", 'train', 'x')
         _C.DATA.TRAIN.GT_PATH = os.path.join("user_data", 'train', 'y')
+        # Whether if your input Zarr contains the raw images and labels together or not. Use 'DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH'
+        # and 'DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_GT_PATH' to determine the tag to find within the Zarr
+        _C.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA = False
+        # Paths to the raw and gt within the Zarr file. Only used when 'DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA' is True.
+        # E.g. 'volumes.raw' for raw and 'volumes.labels.neuron_ids' for GT path. 
+        _C.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH = ''
+        _C.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_GT_PATH = ''
         # File to load/save data prepared with the appropiate channels in a instance segmentation problem.
         # E.g. _C.PROBLEM.TYPE ='INSTANCE_SEG' and _C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS != 'B'
         _C.DATA.TRAIN.INSTANCE_CHANNELS_DIR = os.path.join("user_data", 'train', 'x_'+_C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS)
         _C.DATA.TRAIN.INSTANCE_CHANNELS_MASK_DIR = os.path.join("user_data", 'train', 'y_'+_C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS)
         # Path to load/save detection masks prepared. 
         _C.DATA.TRAIN.DETECTION_MASK_DIR = os.path.join("user_data", 'train', 'y_detection_masks')
         # Path to load/save SSL target prepared. 
@@ -236,17 +243,17 @@
         # Train data resolution. It is not completely necessary but when configured it is taken into account when
         # performing some augmentations, e.g. cutout. If defined it need to be (y,x)/(z,y,x) and needs to be to be a 2D
         # tuple when using _C.PROBLEM.NDIM='2D' and 3D tuple when using _C.PROBLEM.NDIM='3D'
         _C.DATA.TRAIN.RESOLUTION = (-1,)
         # Minimum foreground percentage that each image loaded need to have to not discard it (only used when TRAIN.IN_MEMORY == True). 
         # This option is only valid for SEMANTIC_SEG, INSTANCE_SEG and DETECTION. 
         _C.DATA.TRAIN.MINIMUM_FOREGROUND_PER = -1.
-        # Order of the axes of the image when using Zarr/H5 images to train
+        # Order of the axes of the image when using Zarr/H5 images in train data.
         _C.DATA.TRAIN.INPUT_IMG_AXES_ORDER = 'TZCYX'
-        # Order of the axes of the mask when using Zarr/H5 images to train
+        # Order of the axes of the mask when using Zarr/H5 images in train data.
         _C.DATA.TRAIN.INPUT_MASK_AXES_ORDER = 'TZCYX'
 
         # PREPROCESSING
         # Same preprocessing will be applied to all selected datasets
         _C.DATA.PREPROCESS = CN()
         # Apply preprocessing to training dataset
         _C.DATA.PREPROCESS.TRAIN = False
@@ -366,14 +373,21 @@
         _C.DATA.VAL.RANDOM = True
         # Used when _C.DATA.VAL.FROM_TRAIN = False, as DATA.VAL.FROM_TRAIN = True always implies DATA.VAL.IN_MEMORY = True
         _C.DATA.VAL.IN_MEMORY = True
         # Path to the validation data. Used when _C.DATA.VAL.FROM_TRAIN = False
         _C.DATA.VAL.PATH = os.path.join("user_data", 'val', 'x')
         # Path to the validation data mask. Used when _C.DATA.VAL.FROM_TRAIN = False
         _C.DATA.VAL.GT_PATH = os.path.join("user_data", 'val', 'y')
+        # Whether if your input Zarr contains the raw images and labels together or not. Use 'DATA.VAL.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH'
+        # and 'DATA.VAL.INPUT_ZARR_MULTIPLE_DATA_GT_PATH' to determine the tag to find within the Zarr
+        _C.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA = False
+        # Paths to the raw and gt within the Zarr file. Only used when 'DATA.VAL.INPUT_ZARR_MULTIPLE_DATA' is True.
+        # E.g. 'volumes.raw' for raw and 'volumes.labels.neuron_ids' for GT path. 
+        _C.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH = ''
+        _C.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA_GT_PATH = ''
         # File to load/save data prepared with the appropiate channels in a instance segmentation problem.
         # E.g. _C.PROBLEM.TYPE ='INSTANCE_SEG' and _C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS != 'B'
         _C.DATA.VAL.INSTANCE_CHANNELS_DIR = os.path.join("user_data", 'val', 'x_'+_C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS)
         _C.DATA.VAL.INSTANCE_CHANNELS_MASK_DIR = os.path.join("user_data", 'val', 'y_'+_C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS)
         # Path to load/save detection masks prepared. 
         _C.DATA.VAL.DETECTION_MASK_DIR = os.path.join("user_data", 'val', 'y_detection_masks')
         # Path to load/save SSL target prepared. 
@@ -384,18 +398,17 @@
         # not extracted from training. 
         _C.DATA.VAL.OVERLAP = (0,0)
         # Padding to be done in (y,x)/(z,y,x) when cropping validation data. Useful to avoid patch 'border effect'. This 
         # is only used when the validation is loaded from disk, and thus, not extracted from training. 
         _C.DATA.VAL.PADDING = (0,0)
         # Not used yet.
         _C.DATA.VAL.RESOLUTION = (-1,)
-        # Order of the axes of the image when using Zarr/H5 images to train
+        # Order of the axes of the image when using Zarr/H5 images in validation data.
         _C.DATA.VAL.INPUT_IMG_AXES_ORDER = 'TZCYX'
-        # Order of the axes of the mask when using Zarr/H5 images to train. 
-        # detection the mask
+        # Order of the axes of the mask when using Zarr/H5 images in validation data.
         _C.DATA.VAL.INPUT_MASK_AXES_ORDER = 'TZCYX'
 
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         # Data augmentation (DA)
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         _C.AUGMENTOR = CN()
         # Flag to activate DA
@@ -816,14 +829,24 @@
         # In the process of 'TEST.BY_CHUNKS' you can enable this variable to save the reconstructed prediction as a TIF too. 
         # Be aware of this option and be sure that the prediction can fit in you memory entirely, as it is needed for saving as TIF.
         _C.TEST.BY_CHUNKS.SAVE_OUT_TIF = False
         # In how many iterations the H5 writer needs to flush the data. No need to do so with Zarr files.
         _C.TEST.BY_CHUNKS.FLUSH_EACH = 100
         # Input Numpy/Zarr/H5 image's axes order. Options: ['TZCYX', 'TZYXC', 'ZCYX', 'ZYXC']
         _C.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER = 'TZCYX'
+        # Input Numpy/Zarr/H5 image's axes order. Options: ['TZCYX', 'TZYXC', 'ZCYX', 'ZYXC']
+        _C.TEST.BY_CHUNKS.INPUT_MASK_AXES_ORDER = 'TZCYX'
+        # Whether if your input Zarr contains the raw images and labels together or not. Use 'TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH'
+        # and 'TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_GT_PATH' to determine the tag to find within the Zarr
+        _C.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA = False
+        # Paths to the raw and gt within the Zarr file. Only used when 'TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA' is True.
+        # E.g. 'volumes.raw' for raw and 'volumes.labels.neuron_ids' for GT path. 
+        _C.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH = ''
+        _C.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_GT_PATH = ''
+        
         # Whether if after reconstructing the prediction the pipeline will continue each workflow specific steps. For this process
         # the prediction image needs to be loaded into memory so be sure that it can fit in you memory. E.g. in instance 
         # segmentation the instances will be created from the prediction.
         _C.TEST.BY_CHUNKS.WORKFLOW_PROCESS = CN() 
         _C.TEST.BY_CHUNKS.WORKFLOW_PROCESS.ENABLE = True
         # How the workflow process is going to be done. There are two options:
         #    * 'chunk_by_chunk' : each chunk will be considered as an individual file. Select this operation if you have not enough
```

### Comparing `biapy-3.4.3/biapy/data/data_2D_manipulation.py` & `biapy-3.4.4/biapy/data/data_2D_manipulation.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/data_3D_manipulation.py` & `biapy-3.4.4/biapy/data/data_3D_manipulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import h5py
 import numpy as np
 from skimage.io import imread
 from tqdm import tqdm
 from sklearn.model_selection import train_test_split, StratifiedKFold
 
-from biapy.utils.util import load_3d_images_from_dir, order_dimensions, read_chunked_data
+from biapy.utils.util import load_3d_images_from_dir, order_dimensions, read_chunked_data, read_chunked_nested_data
 from biapy.utils.misc import is_main_process
 
 def load_and_prepare_3D_data(train_path, train_mask_path, cross_val=False, cross_val_nsplits=5, cross_val_fold=1, 
     val_split=0.1, seed=0, shuffle_val=True, crop_shape=(80, 80, 80, 1), y_upscaling=(1,1,1), random_crops_in_DA=False, 
     ov=(0,0,0), padding=(0,0,0), minimum_foreground_perc=-1, reflect_to_complete_shape=False, convert_to_rgb=False,
     preprocess_cfg=None, is_y_mask=False, preprocess_f=None):
     """
@@ -377,15 +377,15 @@
         if Y_train is not None:
             print("*** Loaded train GT shape is: {}".format(Y_train.shape))
         return X_train, Y_train, t_filenames
 
 
 def load_and_prepare_3D_efficient_format_data(train_path, train_mask_path, input_img_axes, input_mask_axes=None, cross_val=False, 
     cross_val_nsplits=5, cross_val_fold=1, val_split=0.1, seed=0, shuffle_val=True, crop_shape=(80, 80, 80, 1), y_upscaling=(1,1,1), 
-    ov=(0,0,0), padding=(0,0,0), minimum_foreground_perc=-1):
+    ov=(0,0,0), padding=(0,0,0), minimum_foreground_perc=-1, multiple_data_within_zarr=None):
     """
     Load train and validation images from the given paths to create 3D data.
 
     Parameters
     ----------
     train_path : str
         Path to the training data.
@@ -429,14 +429,17 @@
 
     padding : Tuple of ints, optional
         Size of padding to be added on each axis ``(z, y, x)``. E.g. ``(24, 24, 24)``.
 
     minimum_foreground_perc : float, optional
         Minimum percetnage of foreground that a sample need to have no not be discarded. 
 
+    multiple_data_within_zarr : dict, optional
+        Additional information of where to find the data within the Zarr files.
+
     Returns
     -------
     X_train : 5D Numpy array
         Train images. E.g. ``(num_of_images, z, y, x, channels)``.
 
     Y_train : 5D Numpy array
         Train images' mask. E.g. ``(num_of_images, z, y, x, channels)``.
@@ -453,24 +456,29 @@
     # Check validation
     if val_split > 0 or cross_val:
         create_val = True  
     else:
         create_val = False
 
     print("0) Loading train image information . . .")
-    X_train, X_train_total_patches = load_3D_efficient_files(train_path, input_img_axes, crop_shape, ov, padding)
+    data_within_zarr_path = multiple_data_within_zarr['raw_path'] if multiple_data_within_zarr is not None else None
+    X_train, X_train_total_patches = load_3D_efficient_files(train_path, input_img_axes, crop_shape, ov, padding,
+        data_within_zarr_path=data_within_zarr_path)
 
     if train_mask_path is not None:
         if input_mask_axes is None:
             raise ValueError("input_mask_axes need to be provided")
 
         print("0) Loading train GT information . . .")
         scrop = (crop_shape[0]*y_upscaling[0], crop_shape[1]*y_upscaling[1], crop_shape[2]*y_upscaling[2], crop_shape[3])
+        data_within_zarr_path = None
+        if multiple_data_within_zarr is not None and multiple_data_within_zarr['use_gt_path']:
+            data_within_zarr_path = multiple_data_within_zarr['gt_path']
         Y_train, Y_train_total_patches = load_3D_efficient_files(train_mask_path, input_mask_axes, scrop, ov, padding, 
-            check_channel=False)
+            check_channel=False, data_within_zarr_path=data_within_zarr_path)
 
         for i in range(len(Y_train_total_patches)):
             if Y_train_total_patches[i] != X_train_total_patches[i]:
                 raise ValueError(f"Seems that the image {X_train[i]['filepath']} and its mask pair {Y_train[i]['filepath']} have "
                     f"different data, as they led to different total amount of patches ({Y_train_total_patches[i]} vs {X_train_total_patches[i]})")
                     
     # Discard images that do not surpass the foreground percentage threshold imposed 
@@ -625,15 +633,16 @@
             return X_train, Y_train, X_val, Y_val, test_index
     else:
         print("*** Loaded train data shape is: {}".format(shape))
         if Y_train is not None:
             print("*** Loaded train GT shape is: {}".format(yshape))
         return X_train, Y_train
 
-def load_3D_efficient_files(data_path, input_axes, crop_shape, overlap, padding, check_channel=True):
+def load_3D_efficient_files(data_path, input_axes, crop_shape, overlap, padding, check_channel=True, 
+    data_within_zarr_path=None):
     """
     Load information of all patches that can be extracted from all the Zarr/H5 samples in ``data_path``.
 
     Parameters
     ----------
     data_path : str
         Path to the training data.
@@ -650,14 +659,17 @@
 
     padding : Tuple of ints, optional
         Size of padding to be added on each axis ``(z, y, x)``. E.g. ``(24, 24, 24)``.
 
     check_channel : bool, optional
         Whether to check if the crop_shape channel matches with the loaded images' one. 
         
+    data_within_zarr_path : str, optional
+        Path to find the data within the Zarr file. E.g. 'volumes.labels.neuron_ids'.
+
     Returns
     -------
     data_info : dict
         All patch info that can be extracted from all the Zarr/H5 samples in ``data_path``.
 
     data_info_total_patches : List of ints
         Amount of patches extracted from each sample in ``data_path``.
@@ -665,16 +677,19 @@
     data_info = {}
     data_total_patches = []
     c = 0
     assert len(crop_shape) == 4, f"Provided crop_shape is not a 4D tuple: {crop_shape}"
 
     for i, filename in enumerate(data_path):
         print(f"Reading Zarr/H5 file: {filename}")
-        file, data = read_chunked_data(filename)
-
+        if data_within_zarr_path:
+            file, data = read_chunked_nested_data(filename, data_within_zarr_path)
+        else:
+            file, data = read_chunked_data(filename)
+        
         # Modify crop_shape with the channel
         c_index = -1
         try:
             c_index = input_axes.index("C")
             crop_shape = crop_shape[:-1]+(data.shape[c_index],)
         except:
             pass 
@@ -710,14 +725,61 @@
         if isinstance(file, h5py.File):
             file.close()
             
         data_total_patches.append(total_patches)
     
     return data_info, data_total_patches
 
+def load_img_part_from_efficient_file(filepath, patch_coords, data_axis_order="ZYXC", data_path=None):
+    """
+    Loads from ``filepath`` the patch determined by ``patch_coords``.
+
+    Parameters
+    ----------
+    filepath : str
+        Path to the Zarr/H5 file to read the patch from. 
+
+    patch_coords : Tuple of tuples of ints
+        Coordinates of patch to extract. 
+        
+    data_axis_order : str
+        Order of axes of ``data``. E.g. 'TZCYX', 'TZYXC', 'ZCYX', 'ZYXC'. 
+
+    data_path : str, optional
+        Path to find the data within the Zarr file. E.g. 'volumes.labels.neuron_ids'.
+        
+    Returns
+    -------
+    img : Numpy array
+        Extracted patch. E.g. ``(z, y, x, channels)``.
+    """
+    if data_path is not None:
+        imgfile, img = read_chunked_nested_data(filepath, data_path)
+    else:
+        imgfile, img = read_chunked_data(filepath)
+
+    # Prepare slices to extract the patch
+    slices = []
+    for j in range(len(patch_coords)):
+        if isinstance(patch_coords[j], int):
+            # +1 to prevent 0 length axes that can not be removed with np.squeeze later
+            slices.append(slice(0,patch_coords[j]+1)) 
+        else:
+            slices.append(slice(patch_coords[j][0],patch_coords[j][1]))
+
+    slices = tuple(slices)
+    data_ordered_slices = tuple(order_dimensions(slices, input_order="ZYXC", output_order=data_axis_order,
+            default_value=0))
+    img = np.squeeze(np.array(img[data_ordered_slices]))
+    
+    if isinstance(imgfile, h5py.File):
+        imgfile.close()
+
+    return img 
+
 def crop_3D_data_with_overlap(data, vol_shape, data_mask=None, overlap=(0,0,0), padding=(0,0,0), verbose=True,
     median_padding=False):
     """Crop 3D data into smaller volumes with a defined overlap. The opposite function is :func:`~merge_3D_data_with_overlap`.
 
        Parameters
        ----------
        data : 4D Numpy array
```

### Comparing `biapy-3.4.3/biapy/data/generators/__init__.py` & `biapy-3.4.4/biapy/data/generators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,17 @@
         data_paths = [cfg.DATA.TRAIN.PATH, cfg.DATA.TRAIN.GT_PATH] 
     else:
         data_paths = [cfg.DATA.TRAIN.PATH] 
     
     if cfg.DATA.TRAIN.IN_MEMORY:
         data_mode = "in_memory"
     else:
-        if cfg.PROBLEM.NDIM == '3D' and X_train is not None and isinstance(X_train, list) and isinstance(X_train[0], dict) and \
-            'filepath' in X_train[0] and ('.zarr' in X_train[0]['filepath'] or '.h5' in X_train[0]['filepath']):
+        if cfg.PROBLEM.NDIM == '3D' and X_train is not None and (isinstance(X_train, list) or isinstance(X_train, dict)) and \
+            isinstance(X_train[0], dict) and 'filepath' in X_train[0] and ('.zarr' in X_train[0]['filepath'] or \
+            '.h5' in X_train[0]['filepath']):
             data_mode = "chunked_data"
         else:
             data_mode = "not_in_memory"
     norm_dict['enable'] = False if cfg.MODEL.SOURCE in ["bmz", "torchvision"] else True
     if cfg.PROBLEM.TYPE == 'CLASSIFICATION' or \
         (cfg.PROBLEM.TYPE == 'SELF_SUPERVISED' and cfg.PROBLEM.SELF_SUPERVISED.PRETEXT_TASK == "masking"):
         r_shape = cfg.DATA.PATCH_SIZE
@@ -222,16 +223,17 @@
             val_data_mode = "chunked_data"
         else:
             val_data_mode = "in_memory"
     else:
         if cfg.DATA.VAL.IN_MEMORY:
             val_data_mode = "in_memory"
         else:
-            if cfg.PROBLEM.NDIM == '3D' and X_val is not None and isinstance(X_val, list) and isinstance(X_val[0], dict) and \
-                'filepath' in X_val[0] and ('.zarr' in X_val[0]['filepath'] or '.h5' in X_val[0]['filepath']):
+            if cfg.PROBLEM.NDIM == '3D' and X_val is not None and (isinstance(X_val, list) or isinstance(X_val, dict)) and \
+                isinstance(X_val[0], dict) and 'filepath' in X_val[0] and ('.zarr' in X_val[0]['filepath'] or \
+                '.h5' in X_val[0]['filepath']):
                 val_data_mode = "chunked_data"
             else:
                 val_data_mode = "not_in_memory"
 
     if norm_dict['mask_norm'] == 'as_image' and cfg.DATA.NORMALIZATION.PERC_CLIP and \
         cfg.DATA.NORMALIZATION.APPLICATION_MODE == "dataset":
         X_val, _, _ = percentile_clip(X_val, lwr_perc_val=norm_dict['dataset_X_lower_value'],
```

### Comparing `biapy-3.4.3/biapy/data/generators/augmentors.py` & `biapy-3.4.4/biapy/data/generators/augmentors.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/generators/pair_base_data_generator.py` & `biapy-3.4.4/biapy/data/generators/pair_base_data_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from abc import ABCMeta, abstractmethod
 from torch.utils.data import Dataset                 
 
 from biapy.utils.util import img_to_onehot_encoding, pad_and_reflect, read_chunked_data
 from biapy.data.generators.augmentors import *
 from biapy.data.pre_processing import normalize, norm_range01, percentile_clip
 from biapy.utils.misc import is_main_process
+from biapy.data.data_3D_manipulation import load_img_part_from_efficient_file 
 
 class PairBaseDataGenerator(Dataset, metaclass=ABCMeta):
     """
     Custom BaseDataGenerator based on `imgaug <https://github.com/aleju/imgaug-doc>`_
     and our own `augmentors.py <https://github.com/BiaPyX/BiaPy/blob/master/biapy/data/generators/augmentors.py>`_
     transformations. 
 
@@ -828,47 +829,17 @@
                     img = imread(os.path.join(self.paths[0], self.data_paths[idx]))
                     if self.Y_provided:
                         mask = imread(os.path.join(self.paths[1], self.data_mask_path[idx]))
                 img = np.squeeze(img)
                 if self.Y_provided:
                     mask = np.squeeze(mask)
         else: # self.data_mode == "chunked_data"
-            imgfile, img = read_chunked_data(self.X[idx]['filepath'])
-
-            # Prepare slices to extract the patch
-            slices = []
-            for j in range(len(self.X[idx]['patch_coords'])):
-                if isinstance(self.X[idx]['patch_coords'][j], int):
-                    # +1 to prevent 0 length axes that can not be removed with np.squeeze later
-                    slices.append(slice(0,self.X[idx]['patch_coords'][j]+1)) 
-                else:
-                    slices.append(slice(self.X[idx]['patch_coords'][j][0],self.X[idx]['patch_coords'][j][1]))
-
-            img = np.squeeze(np.array(img[tuple(slices)]))
-            
-            if isinstance(imgfile, h5py.File):
-                imgfile.close()
-
+            img = load_img_part_from_efficient_file(self.X[idx]['filepath'], self.X[idx]['patch_coords'])
             if self.Y_provided:
-                maskfile, mask = read_chunked_data(self.Y[idx]['filepath'])
-
-                # Prepare slices to extract the patch
-                slices = []
-                for j in range(len(self.Y[idx]['patch_coords'])):
-                    if isinstance(self.Y[idx]['patch_coords'][j], int):
-                        # +1 to prevent 0 length axes that can not be removed with np.squeeze later
-                        slices.append(slice(0,self.Y[idx]['patch_coords'][j]+1)) 
-                    else:
-                        slices.append(slice(self.Y[idx]['patch_coords'][j][0],self.Y[idx]['patch_coords'][j][1]))
-
-                mask = np.squeeze(np.array(mask[tuple(slices)]))
-
-                if isinstance(maskfile, h5py.File):
-                    maskfile.close()
-                
+                mask = load_img_part_from_efficient_file(self.Y[idx]['filepath'], self.Y[idx]['patch_coords'])
         if self.Y_provided:
             img, mask = self.ensure_shape(img, mask)
         else:
             img = self.ensure_shape(img, None)
 
         img = self.norm_X(img)
         if self.Y_provided:
```

### Comparing `biapy-3.4.3/biapy/data/generators/pair_data_2D_generator.py` & `biapy-3.4.4/biapy/data/generators/pair_data_2D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/generators/pair_data_3D_generator.py` & `biapy-3.4.4/biapy/data/generators/pair_data_3D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/generators/single_base_data_generator.py` & `biapy-3.4.4/biapy/data/generators/single_base_data_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/generators/single_data_2D_generator.py` & `biapy-3.4.4/biapy/data/generators/single_data_2D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/generators/single_data_3D_generator.py` & `biapy-3.4.4/biapy/data/generators/single_data_3D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/generators/test_pair_data_generators.py` & `biapy-3.4.4/biapy/data/generators/test_pair_data_generators.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/generators/test_single_data_generator.py` & `biapy-3.4.4/biapy/data/generators/test_single_data_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/post_processing/__init__.py` & `biapy-3.4.4/biapy/data/post_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/post_processing/post_processing.py` & `biapy-3.4.4/biapy/data/post_processing/post_processing.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/post_processing/smooth_tiled_predictions.py` & `biapy-3.4.4/biapy/data/post_processing/smooth_tiled_predictions.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/data/pre_processing.py` & `biapy-3.4.4/biapy/data/pre_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import torch
 import scipy
 import h5py
+import zarr
 import numpy as np
 from tqdm import tqdm
 import pandas as pd
 from skimage.segmentation import clear_border, find_boundaries
 from skimage.io import imread
 from scipy.ndimage.morphology import binary_dilation  as binary_dilation_scipy
 from scipy.ndimage.measurements import center_of_mass                                                  
@@ -13,16 +14,18 @@
 from skimage.measure import label, regionprops
 from skimage.transform import resize
 from skimage.feature import peak_local_max, canny
 from skimage.exposure import equalize_adapthist
 from skimage.color import rgb2gray
 from skimage.filters import gaussian, median
 
-from biapy.utils.util import load_data_from_dir, load_3d_images_from_dir, save_tif, write_chunked_data, read_chunked_data
+from biapy.utils.util import (load_data_from_dir, load_3d_images_from_dir, save_tif, write_chunked_data, read_chunked_data,
+    order_dimensions)
 from biapy.utils.misc import is_main_process
+from biapy.data.data_3D_manipulation import load_3D_efficient_files, load_img_part_from_efficient_file
 
 #########################
 # INSTANCE SEGMENTATION #
 #########################
 def create_instance_channels(cfg, data_type='train'):
     """Create training and validation new data with appropiate channels based on ``PROBLEM.INSTANCE_SEG.DATA_CHANNELS`` for instance
        segmentation.
@@ -38,18 +41,49 @@
        Returns
        -------
        filenames: List of str
            Image paths.
     """
 
     assert data_type in ['train', 'val']
-
-    f_name = load_data_from_dir if cfg.PROBLEM.NDIM == '2D' else load_3d_images_from_dir
     tag = "TRAIN" if data_type == "train" else "VAL"
-    Y, _, _, filenames = f_name(getattr(cfg.DATA, tag).GT_PATH, check_drange=False, return_filenames=True)
+
+    # Checking if the user inputted Zarr/H5 files 
+    if getattr(cfg.DATA, tag).INPUT_ZARR_MULTIPLE_DATA:
+        zarr_files = sorted(next(os.walk(getattr(cfg.DATA, tag).PATH))[1])
+        h5_files = sorted(next(os.walk(getattr(cfg.DATA, tag).PATH))[2])
+    else:
+        zarr_files = sorted(next(os.walk(getattr(cfg.DATA, tag).GT_PATH))[1])
+        h5_files = sorted(next(os.walk(getattr(cfg.DATA, tag).GT_PATH))[2])
+    
+    # Find patches info so we can iterate over them to create the instance mask
+    working_with_zarr_h5_files = False
+    if cfg.PROBLEM.NDIM == '3D' and (len(zarr_files) > 0 and '.zarr' in zarr_files[0]) or \
+        (len(h5_files) > 0 and '.h5' in h5_files[0]):
+        working_with_zarr_h5_files = True
+        # Check if the raw images and labels are within the same file 
+        mult_dat = None
+        data_path = getattr(cfg.DATA, tag).GT_PATH
+        if getattr(cfg.DATA, tag).INPUT_ZARR_MULTIPLE_DATA:
+            data_path = getattr(cfg.DATA, tag).PATH
+        
+        if len(zarr_files) > 0 and '.zarr' in zarr_files[0]:
+            print("Working with Zarr files . . .")
+            img_files = [os.path.join(data_path, x) for x in zarr_files]
+        elif len(h5_files) > 0 and '.h5' in h5_files[0]:
+            print("Working with H5 files . . .")
+            img_files = [os.path.join(data_path, x) for x in h5_files]
+        
+        Y, Y_total_patches = load_3D_efficient_files(img_files, input_axes=getattr(cfg.DATA, tag).INPUT_IMG_AXES_ORDER, 
+            crop_shape=cfg.DATA.PATCH_SIZE, overlap=getattr(cfg.DATA, tag).OVERLAP, padding=getattr(cfg.DATA, tag).PADDING)
+    else:
+        f_name = load_data_from_dir if cfg.PROBLEM.NDIM == '2D' else load_3d_images_from_dir
+        Y, _, _, filenames = f_name(getattr(cfg.DATA, tag).GT_PATH, check_drange=False, return_filenames=True)
+    del zarr_files, h5_files
+
     print("Creating Y_{} channels . . .".format(data_type))
     if isinstance(Y, list):
         for i in tqdm(range(len(Y)), disable=not is_main_process()):
             if cfg.MODEL.N_CLASSES > 2:
                 if Y[i].shape[-1] != 2:
                     raise ValueError("In instance segmentation, when 'MODEL.N_CLASSES' are more than 2 labels need to have two channels, "
                         "e.g. (256,256,2), containing the instance segmentation map (first channel) and classification map (second channel).")
@@ -57,39 +91,112 @@
                     class_channel = np.expand_dims(Y[i,...,1].copy(),-1)
                     Y[i] = labels_into_channels(Y[i], mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS, save_dir=getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'),
                         fb_mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE)
                     Y[i] = np.concatenate([Y[i],class_channel],axis=-1)
             else:
                 Y[i] = labels_into_channels(Y[i], mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS, save_dir=getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'),
                     fb_mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE)
+    # Create the mask patch by patch (Zarr/H5)
+    elif working_with_zarr_h5_files and isinstance(Y, dict):
+        savepath = data_path+'_'+cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS+'_'+cfg.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE
+        if 'D' in cfg.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE:
+            dtype_str = "float32"
+            raise ValueError("Currently distance creation using Zarr by chunks is not implemented.")
+        else:
+            dtype_str = "uint8"  
+            
+        mask = None
+        last_zarr_file = None 
+        for i in tqdm(range(len(Y.keys())), disable=not is_main_process()):
+            # Extract the patch to process
+            patch_coords = Y[i]['patch_coords']
+            img = load_img_part_from_efficient_file(Y[i]['filepath'], patch_coords, 
+                data_axis_order=getattr(cfg.DATA, tag).INPUT_IMG_AXES_ORDER,
+                data_path=getattr(cfg.DATA, tag).INPUT_ZARR_MULTIPLE_DATA_GT_PATH)
+            if img.ndim == 3: img = np.expand_dims(img,-1)
+            if img.ndim == 4: img = np.expand_dims(img,0)
+
+            # Create the instance mask
+            if cfg.MODEL.N_CLASSES > 2:
+                if img.shape[-1] != 2:
+                    raise ValueError("In instance segmentation, when 'MODEL.N_CLASSES' are more than 2 labels need to have two channels, "
+                        "e.g. (256,256,2), containing the instance segmentation map (first channel) and classification map (second channel).")
+                else:
+                    class_channel = np.expand_dims(img[...,1].copy(),-1)
+                    img = labels_into_channels(img, mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS, save_dir=getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'),
+                        fb_mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE)
+                    img = np.concatenate([img,class_channel],axis=-1)
+            else:
+                img = labels_into_channels(img, mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS, save_dir=getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'),
+                    fb_mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE)
+            img = img[0]
+
+            # Create the Zarr file where the mask will be placed 
+            if mask is None or os.path.basename(Y[i]['filepath']) != last_zarr_file: 
+                last_zarr_file = os.path.basename(Y[i]['filepath'])
+                imgfile, data = read_chunked_data(Y[i]['filepath'])
+                fname = os.path.join(savepath, os.path.basename(Y[i]['filepath']))
+                fid_mask = zarr.open_group(fname, mode="w")
+
+                # Determine data shape
+                out_data_shape = np.array(data.shape)
+                if "C" not in getattr(cfg.DATA, tag).INPUT_IMG_AXES_ORDER:
+                    out_data_shape = tuple(out_data_shape) + (img.shape[-1],)
+                    out_data_order = getattr(cfg.DATA, tag).INPUT_IMG_AXES_ORDER + "C"
+                    channel_pos = -1
+                else:
+                    out_data_shape[getattr(cfg.DATA, tag).INPUT_IMG_AXES_ORDER.index("C")] = 1
+                    out_data_shape = tuple(out_data_shape)
+                    out_data_order = getattr(cfg.DATA, tag).INPUT_IMG_AXES_ORDER
+                    channel_pos = getattr(cfg.DATA, tag).INPUT_IMG_AXES_ORDER.index("C")
+
+                mask = fid_mask.create_dataset("data", shape=out_data_shape, dtype=dtype_str)
+                del data, imgfile, fname
+            
+            # Adjust slices to calculate where to insert the predicted patch. This slice does not have into account the 
+            # channel so any of them can be inserted 
+            slices = (slice(patch_coords[0][0],patch_coords[0][1]), slice(patch_coords[1][0],patch_coords[1][1]),
+                slice(patch_coords[2][0],patch_coords[2][1]), slice(0,out_data_shape[channel_pos]))
+            data_ordered_slices = tuple(order_dimensions(slices, input_order="ZYXC", 
+                output_order=out_data_order, default_value=0))
+
+            # Adjust patch slice to transpose it before inserting intop the final data 
+            current_order = np.array(range(len(img.shape)))
+            transpose_order = order_dimensions(current_order, input_order="ZYXC", output_order=out_data_order,
+                default_value=np.nan)
+            transpose_order = [x for x in transpose_order if not np.isnan(x)]
+
+            # Place the patch into the Zarr
+            mask[data_ordered_slices] = img.transpose(transpose_order)        
     else:
         if cfg.MODEL.N_CLASSES > 2:
             if Y.shape[-1] != 2:
                 raise ValueError("In instance segmentation, when 'MODEL.N_CLASSES' are more than 2 labels need to have two channels, "
                     "e.g. (256,256,2), containing the instance segmentation map (first channel) and classification map (second channel).")
             else:
                 class_channel = np.expand_dims(Y[...,1].copy(),-1)
                 Y = labels_into_channels(Y, mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS, save_dir=getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'),
                     fb_mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE)
                 Y = np.concatenate([Y, class_channel], axis=-1)
         else:
             Y = labels_into_channels(Y, mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS, save_dir=getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'),
                 fb_mode=cfg.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE)
     
-    save_tif(Y, data_dir=getattr(cfg.DATA, tag).INSTANCE_CHANNELS_MASK_DIR, filenames=filenames, verbose=cfg.TEST.VERBOSE)
-    X, _, _, filenames = f_name(getattr(cfg.DATA, tag).PATH, return_filenames=True)
-    print("Creating X_{} channels . . .".format(data_type))
-    save_tif(X, data_dir=getattr(cfg.DATA, tag).INSTANCE_CHANNELS_DIR, filenames=filenames, verbose=cfg.TEST.VERBOSE)
-    
-    # Save original X data with the labels 
-    for i in range(min(3,len(X))):
-        if isinstance(X, list):
-            save_tif(X[i], getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'), filenames=['vol'+str(i)+".tif"], verbose=False)
-        else:
-            save_tif(np.expand_dims(X[i],0), getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'), filenames=['vol'+str(i)+".tif"], verbose=False)
+    if not working_with_zarr_h5_files:
+        save_tif(Y, data_dir=getattr(cfg.DATA, tag).INSTANCE_CHANNELS_MASK_DIR, filenames=filenames, verbose=cfg.TEST.VERBOSE)
+        X, _, _, filenames = f_name(getattr(cfg.DATA, tag).PATH, return_filenames=True)
+        print("Creating X_{} channels . . .".format(data_type))
+        save_tif(X, data_dir=getattr(cfg.DATA, tag).INSTANCE_CHANNELS_DIR, filenames=filenames, verbose=cfg.TEST.VERBOSE)
+
+        # Save original X data with the labels 
+        for i in range(min(3,len(X))):
+            if isinstance(X, list):
+                save_tif(X[i], getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'), filenames=['vol'+str(i)+".tif"], verbose=False)
+            else:
+                save_tif(np.expand_dims(X[i],0), getattr(cfg.PATHS, tag+'_INSTANCE_CHANNELS_CHECK'), filenames=['vol'+str(i)+".tif"], verbose=False)
 
 def create_test_instance_channels(cfg):
     """Create test new data with appropiate channels based on ``PROBLEM.INSTANCE_SEG.DATA_CHANNELS`` for instance segmentation.
 
        Parameters
        ----------
        cfg : YACS CN object
```

### Comparing `biapy-3.4.3/biapy/engine/__init__.py` & `biapy-3.4.4/biapy/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/base_workflow.py` & `biapy-3.4.4/biapy/engine/base_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,23 +256,33 @@
                     del zarr_files, h5_files
 
                     if self.cfg.DATA.EXTRACT_RANDOM_PATCH:
                         print("WARNING: 'DATA.EXTRACT_RANDOM_PATCH' not taken into account when working with Zarr/H5 images")
                     if self.cfg.DATA.FORCE_RGB:
                         print("WARNING: 'DATA.FORCE_RGB' not taken into account when working with Zarr/H5 images")
 
+                    # When the labels and raw images are within the same Zarr file
+                    mult_dat = None
+                    if self.cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA:
+                        mult_dat = {
+                            'raw_path': self.cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH,
+                            'gt_path': self.cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_GT_PATH,
+                            'use_gt_path': self.cfg.PROBLEM.TYPE != 'INSTANCE_SEG'
+                        }
+
                     objs = load_and_prepare_3D_efficient_format_data(
                         img_files, mask_files, input_img_axes=self.cfg.DATA.TRAIN.INPUT_IMG_AXES_ORDER, 
                         input_mask_axes=self.cfg.DATA.TRAIN.INPUT_MASK_AXES_ORDER, 
                         cross_val=self.cfg.DATA.VAL.CROSS_VAL, cross_val_nsplits=self.cfg.DATA.VAL.CROSS_VAL_NFOLD, 
                         cross_val_fold=self.cfg.DATA.VAL.CROSS_VAL_FOLD, val_split=val_split, seed=self.cfg.SYSTEM.SEED, 
                         shuffle_val=self.cfg.DATA.VAL.RANDOM, crop_shape=self.cfg.DATA.PATCH_SIZE, 
                         y_upscaling=self.cfg.PROBLEM.SUPER_RESOLUTION.UPSCALING, 
                         ov=self.cfg.DATA.TRAIN.OVERLAP, padding=self.cfg.DATA.TRAIN.PADDING, 
-                        minimum_foreground_perc=self.cfg.DATA.TRAIN.MINIMUM_FOREGROUND_PER)
+                        minimum_foreground_perc=self.cfg.DATA.TRAIN.MINIMUM_FOREGROUND_PER,
+                        multiple_data_within_zarr=mult_dat)
                     
                     if self.cfg.DATA.VAL.FROM_TRAIN:
                         if self.cfg.DATA.VAL.CROSS_VAL:
                             self.X_train, self.Y_train, self.X_val, self.Y_val, self.cross_val_samples_ids = objs
                         else:
                             self.X_train, self.Y_train, self.X_val, self.Y_val = objs
                     else:
@@ -330,29 +340,37 @@
                             img_files = [os.path.join(self.cfg.DATA.VAL.PATH, x) for x in h5_files]
                             mask_files = [os.path.join(self.mask_path, x) for x in sorted(next(os.walk(self.mask_path))[2])]
                         del zarr_files, h5_files
 
                         if self.cfg.DATA.FORCE_RGB:
                             print("WARNING: 'DATA.FORCE_RGB' not taken into account when working with Zarr/H5 images")
 
+                        data_within_zarr_path, data_within_zarr_mask_path = None, None
+                        if self.cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA:
+                            data_within_zarr_path = self.cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH
+                            if self.cfg.PROBLEM.TYPE != 'INSTANCE_SEG':
+                                data_within_zarr_mask_path = self.cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH
+
                         self.X_val, _ = load_3D_efficient_files(data_path=img_files, input_axes=self.cfg.DATA.VAL.INPUT_IMG_AXES_ORDER,
-                            crop_shape=self.cfg.DATA.PATCH_SIZE, overlap=self.cfg.DATA.VAL.OVERLAP, padding=self.cfg.DATA.VAL.PADDING)
+                            crop_shape=self.cfg.DATA.PATCH_SIZE, overlap=self.cfg.DATA.VAL.OVERLAP, padding=self.cfg.DATA.VAL.PADDING,
+                            data_within_zarr_path=data_within_zarr_path)
 
                         if self.cfg.PROBLEM.NDIM == '2D':
                             crop_shape = (self.cfg.DATA.PATCH_SIZE[0]*self.cfg.PROBLEM.SUPER_RESOLUTION.UPSCALING[0],
                                 self.cfg.DATA.PATCH_SIZE[1]*self.cfg.PROBLEM.SUPER_RESOLUTION.UPSCALING[1], self.cfg.DATA.PATCH_SIZE[2])
                         else:
                             crop_shape = (self.cfg.DATA.PATCH_SIZE[0], self.cfg.DATA.PATCH_SIZE[1]*self.cfg.PROBLEM.SUPER_RESOLUTION.UPSCALING[0],
                                 self.cfg.DATA.PATCH_SIZE[2]*self.cfg.PROBLEM.SUPER_RESOLUTION.UPSCALING[1],
                                 self.cfg.DATA.PATCH_SIZE[3]*self.cfg.PROBLEM.SUPER_RESOLUTION.UPSCALING[2])
 
                         if self.load_Y_val:
                             print("1) Loading validation GT information . . .")
-                            self.Y_val, _ = load_3D_efficient_files(data_path=img_files, input_axes=self.cfg.DATA.VAL.INPUT_IMG_AXES_ORDER,
-                                crop_shape=crop_shape, overlap=self.cfg.DATA.VAL.OVERLAP, padding=self.cfg.DATA.VAL.PADDING, check_channel=False)                          
+                            self.Y_val, _ = load_3D_efficient_files(data_path=mask_files, input_axes=self.cfg.DATA.VAL.INPUT_MASK_AXES_ORDER,
+                                crop_shape=crop_shape, overlap=self.cfg.DATA.VAL.OVERLAP, padding=self.cfg.DATA.VAL.PADDING, check_channel=False,
+                                data_within_zarr_path=data_within_zarr_mask_path)                          
                         else:
                             self.Y_val = None
                         if self.Y_val is not None and len(self.X_val) != len(self.Y_val):
                             raise ValueError("Different number of raw and ground truth items ({} vs {}). "
                                 "Please check the data!".format(len(self.X_val), len(self.Y_val)))
 
                     else:        
@@ -721,16 +739,20 @@
                     else:
                         self.Y_test = None
                 else:
                     self.X_test, self.Y_test = None, None
 
                 if self.original_test_path is None:
                     self.test_filenames = sorted(next(os.walk(self.cfg.DATA.TEST.PATH))[2])
+                    if len(self.test_filenames) == 0:
+                        self.test_filenames = sorted(next(os.walk(self.cfg.DATA.TEST.PATH))[1]) 
                 else:
                     self.test_filenames = sorted(next(os.walk(self.original_test_path))[2])
+                    if len(self.test_filenames) == 0:
+                        self.test_filenames = sorted(next(os.walk(self.original_test_path))[1])    
             else:
                 # The test is the validation, and as it is only available when validation is obtained from train and when 
                 # cross validation is enabled, the test set files reside in the train folder
                 self.test_filenames = sorted(next(os.walk(self.cfg.DATA.TRAIN.PATH))[2])
                 self.X_test, self.Y_test = None, None
                 if self.cross_val_samples_ids is None:                      
                     # Split the test as it was the validation when train is not enabled 
@@ -908,259 +930,262 @@
 
         Parameters
         ----------
         filenames : List of str
             Filenames fo the samples to process. 
         """
         filename, file_extension = os.path.splitext(filenames)
-        if file_extension not in ['.hdf5', '.h5', ".zarr"]:
-            print("WARNING: you could have saved more memory by converting input test images into H5 file format (.h5) "
-                  "or Zarr (.zarr) as with 'TEST.BY_CHUNKS.ENABLE' option enabled H5/Zarr files will be processed by chunks")
-        # Load data
-        if file_extension in ['.hdf5', '.h5', ".zarr"]:
-            self._X_file, self._X = read_chunked_data(self._X)
-        else: # Numpy array
-            if self._X.ndim == 3:
-                c_pos = -1 if self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER[-1] == 'C' else 1
-                self._X = np.expand_dims(self._X, c_pos)
+        ext = ".h5" if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5" else ".zarr"
+        out_data_div_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+ext)
 
-        if is_main_process():
-            print(f"Loaded image shape is {self._X.shape}")
+        if not self.cfg.TEST.REUSE_PREDICTIONS:    
+            if file_extension not in ['.hdf5', '.h5', ".zarr"]:
+                print("WARNING: you could have saved more memory by converting input test images into H5 file format (.h5) "
+                    "or Zarr (.zarr) as with 'TEST.BY_CHUNKS.ENABLE' option enabled H5/Zarr files will be processed by chunks")
+            # Load data
+            if file_extension in ['.hdf5', '.h5', ".zarr"]:
+                self._X_file, self._X = read_chunked_data(self._X)
+            else: # Numpy array
+                if self._X.ndim == 3:
+                    c_pos = -1 if self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER[-1] == 'C' else 1
+                    self._X = np.expand_dims(self._X, c_pos)
 
-        data_shape = self._X.shape
+            if is_main_process():
+                print(f"Loaded image shape is {self._X.shape}")
 
-        if self._X.ndim < 3:
-            raise ValueError("Loaded image need to have at least 3 dimensions: {} (ndim: {})".format(self._X.shape, self._X.ndim))
-        
-        if len(self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER) != self._X.ndim:
-            raise ValueError("'TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER' value {} does not match the number of dimensions of the loaded H5/Zarr "
-                "file {} (ndim: {})".format(self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER, self._X.shape, self._X.ndim))
+            data_shape = self._X.shape
 
-        # Data paths
-        os.makedirs(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, exist_ok=True)
-        ext = ".h5" if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5" else ".zarr"
-        if self.cfg.SYSTEM.NUM_GPUS > 1:
-            out_data_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+"_part"+str(get_rank())+ext)
-            out_data_mask_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+"_part"+str(get_rank())+"_mask"+ext)
-        else:
-            out_data_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+"_nodiv"+ext)
-            out_data_mask_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+"_mask"+ext)
-        out_data_div_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+ext)
-        in_data = self._X
+            if self._X.ndim < 3:
+                raise ValueError("Loaded image need to have at least 3 dimensions: {} (ndim: {})".format(self._X.shape, self._X.ndim))
+            
+            if len(self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER) != self._X.ndim:
+                raise ValueError("'TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER' value {} does not match the number of dimensions of the loaded H5/Zarr "
+                    "file {} (ndim: {})".format(self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER, self._X.shape, self._X.ndim))
 
-        # Process in charge of processing one predicted patch
-        output_handle_proc = mp.Process(target=insert_patch_into_dataset, args=(out_data_filename, out_data_mask_filename, 
-            data_shape, self.output_queue, self.extract_info_queue, self.cfg, self.dtype_str, self.dtype, 
-            self.cfg.TEST.BY_CHUNKS.FORMAT, self.cfg.TEST.VERBOSE))
-        output_handle_proc.daemon=True
-        output_handle_proc.start()
-        
-        # Process in charge of loading part of the data 
-        load_data_process = mp.Process(target=extract_patch_from_dataset, args=(in_data, self.cfg, self.input_queue, 
-            self.extract_info_queue, self.cfg.TEST.VERBOSE))
-        load_data_process.daemon=True
-        load_data_process.start()
-
-        if '_X_file' in locals() and isinstance(self._X_file, h5py.File):
-            self._X_file.close()
-        del self._X, in_data
- 
-        # Lock the thread inferring until no more patches 
-        if self.cfg.TEST.VERBOSE and self.cfg.SYSTEM.NUM_GPUS > 1:
-            print(f"[Rank {get_rank()} ({os.getpid()})] Doing inference ")
-        while True:
-            obj = self.input_queue.get(timeout=60)
-            if obj == None: break
-
-            img, patch_coords = obj
-            img, _ = self.test_generator.norm_X(img)
-            if self.cfg.TEST.AUGMENTATION:
-                p = ensemble16_3d_predictions(img[0], batch_size_value=self.cfg.TRAIN.BATCH_SIZE,
-                    axis_order_back=self.axis_order_back, pred_func=self.model_call_func, 
-                    axis_order=self.axis_order, device=self.device)
+            # Data paths
+            os.makedirs(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, exist_ok=True)
+            if self.cfg.SYSTEM.NUM_GPUS > 1:
+                out_data_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+"_part"+str(get_rank())+ext)
+                out_data_mask_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+"_part"+str(get_rank())+"_mask"+ext)
             else:
-                with torch.cuda.amp.autocast():
-                    p = self.model_call_func(img)
-            p = self.apply_model_activations(p)
-            # Multi-head concatenation
-            if isinstance(p, list):
-                p = torch.cat((p[0], torch.argmax(p[1], axis=1).unsqueeze(1)), dim=1)
-            p = to_numpy_format(p, self.axis_order_back)
-
-            # Create a mask with the overlap. Calculate the exact part of the patch that will be inserted in the 
-            # final H5/Zarr file
-            p = p[0, self.cfg.DATA.TEST.PADDING[0]:p.shape[1]-self.cfg.DATA.TEST.PADDING[0],
-                self.cfg.DATA.TEST.PADDING[1]:p.shape[2]-self.cfg.DATA.TEST.PADDING[1],
-                self.cfg.DATA.TEST.PADDING[2]:p.shape[3]-self.cfg.DATA.TEST.PADDING[2]]
-            m = np.ones(p.shape, dtype=np.uint8)
+                out_data_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+"_nodiv"+ext)
+                out_data_mask_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+"_mask"+ext)
+            in_data = self._X
+
+            # Process in charge of processing one predicted patch
+            output_handle_proc = mp.Process(target=insert_patch_into_dataset, args=(out_data_filename, out_data_mask_filename, 
+                data_shape, self.output_queue, self.extract_info_queue, self.cfg, self.dtype_str, self.dtype, 
+                self.cfg.TEST.BY_CHUNKS.FORMAT, self.cfg.TEST.VERBOSE))
+            output_handle_proc.daemon=True
+            output_handle_proc.start()
+            
+            # Process in charge of loading part of the data 
+            load_data_process = mp.Process(target=extract_patch_from_dataset, args=(in_data, self.cfg, self.input_queue, 
+                self.extract_info_queue, self.cfg.TEST.VERBOSE))
+            load_data_process.daemon=True
+            load_data_process.start()
+
+            if '_X_file' in locals() and isinstance(self._X_file, h5py.File):
+                self._X_file.close()
+            del self._X, in_data
+    
+            # Lock the thread inferring until no more patches 
+            if self.cfg.TEST.VERBOSE and self.cfg.SYSTEM.NUM_GPUS > 1:
+                print(f"[Rank {get_rank()} ({os.getpid()})] Doing inference ")
+            while True:
+                obj = self.input_queue.get(timeout=60)
+                if obj == None: break
+
+                img, patch_coords = obj
+                img, _ = self.test_generator.norm_X(img)
+                if self.cfg.TEST.AUGMENTATION:
+                    p = ensemble16_3d_predictions(img[0], batch_size_value=self.cfg.TRAIN.BATCH_SIZE,
+                        axis_order_back=self.axis_order_back, pred_func=self.model_call_func, 
+                        axis_order=self.axis_order, device=self.device)
+                else:
+                    with torch.cuda.amp.autocast():
+                        p = self.model_call_func(img)
+                p = self.apply_model_activations(p)
+                # Multi-head concatenation
+                if isinstance(p, list):
+                    p = torch.cat((p[0], torch.argmax(p[1], axis=1).unsqueeze(1)), dim=1)
+                p = to_numpy_format(p, self.axis_order_back)
+
+                # Create a mask with the overlap. Calculate the exact part of the patch that will be inserted in the 
+                # final H5/Zarr file
+                p = p[0, self.cfg.DATA.TEST.PADDING[0]:p.shape[1]-self.cfg.DATA.TEST.PADDING[0],
+                    self.cfg.DATA.TEST.PADDING[1]:p.shape[2]-self.cfg.DATA.TEST.PADDING[1],
+                    self.cfg.DATA.TEST.PADDING[2]:p.shape[3]-self.cfg.DATA.TEST.PADDING[2]]
+                m = np.ones(p.shape, dtype=np.uint8)
 
-            # Put the prediction into queue
-            self.output_queue.put([p, m, patch_coords])         
+                # Put the prediction into queue
+                self.output_queue.put([p, m, patch_coords])         
 
-        # Get some auxiliar variables
-        self.stats['patch_counter'] = self.extract_info_queue.get(timeout=60)
-        if is_main_process():
-            z_vol_info = self.extract_info_queue.get(timeout=60)
-            list_of_vols_in_z  = self.extract_info_queue.get(timeout=60)
-        load_data_process.join()
-        output_handle_proc.join()
+            # Get some auxiliar variables
+            self.stats['patch_counter'] = self.extract_info_queue.get(timeout=60)
+            if is_main_process():
+                z_vol_info = self.extract_info_queue.get(timeout=60)
+                list_of_vols_in_z  = self.extract_info_queue.get(timeout=60)
+            load_data_process.join()
+            output_handle_proc.join()
 
         # Wait until all threads are done so the main thread can create the full size image 
         if self.cfg.SYSTEM.NUM_GPUS > 1 :
             if self.cfg.TEST.VERBOSE:
                 print(f"[Rank {get_rank()} ({os.getpid()})] Finish sample inference ")
             if is_dist_avail_and_initialized():
                 dist.barrier()
 
         # Create the final H5/Zarr file that contains all the individual parts 
         if is_main_process():
-            if "C" not in self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER:
-                out_data_order = self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER + "C"
-                c_index = -1
-            else:
-                out_data_order = self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER
-                c_index = out_data_order.index("C")
-                
-            if self.cfg.SYSTEM.NUM_GPUS > 1:
-                # Obtain parts of the data created by all GPUs
-                if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
-                    data_parts_filenames = sorted(next(os.walk(self.cfg.PATHS.RESULT_DIR.PER_IMAGE))[2])
-                else: 
-                    data_parts_filenames = sorted(next(os.walk(self.cfg.PATHS.RESULT_DIR.PER_IMAGE))[1])
-                parts = []
-                mask_parts = []
-                for x in data_parts_filenames:
-                    if filename+"_part" in x and x.endswith(self.cfg.TEST.BY_CHUNKS.FORMAT):
-                        if "_mask" not in x:
-                            parts.append(x)
-                        else:
-                            mask_parts.append(x)
-                data_parts_filenames = parts 
-                data_parts_mask_filenames = mask_parts
-                del parts, mask_parts
-
-                if max(1,self.cfg.SYSTEM.NUM_GPUS) != len(data_parts_filenames) != len(list_of_vols_in_z):
-                    raise ValueError("Number of data parts is not the same as number of GPUs")
-
-                # Compose the large image 
-                for i, data_part_fname in enumerate(data_parts_filenames):
-                    print("Reading {}".format(os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, data_part_fname)))
-                    data_part_file, data_part = read_chunked_data(os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, data_part_fname))
-                    data_mask_part_file, data_mask_part = read_chunked_data(os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, data_parts_mask_filenames[i]))
+            if not self.cfg.TEST.REUSE_PREDICTIONS:
+                if "C" not in self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER:
+                    out_data_order = self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER + "C"
+                    c_index = -1
+                else:
+                    out_data_order = self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER
+                    c_index = out_data_order.index("C")
+                    
+                if self.cfg.SYSTEM.NUM_GPUS > 1:
+                    # Obtain parts of the data created by all GPUs
+                    if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
+                        data_parts_filenames = sorted(next(os.walk(self.cfg.PATHS.RESULT_DIR.PER_IMAGE))[2])
+                    else: 
+                        data_parts_filenames = sorted(next(os.walk(self.cfg.PATHS.RESULT_DIR.PER_IMAGE))[1])
+                    parts = []
+                    mask_parts = []
+                    for x in data_parts_filenames:
+                        if filename+"_part" in x and x.endswith(self.cfg.TEST.BY_CHUNKS.FORMAT):
+                            if "_mask" not in x:
+                                parts.append(x)
+                            else:
+                                mask_parts.append(x)
+                    data_parts_filenames = parts 
+                    data_parts_mask_filenames = mask_parts
+                    del parts, mask_parts
+
+                    if max(1,self.cfg.SYSTEM.NUM_GPUS) != len(data_parts_filenames) != len(list_of_vols_in_z):
+                        raise ValueError("Number of data parts is not the same as number of GPUs")
+
+                    # Compose the large image 
+                    for i, data_part_fname in enumerate(data_parts_filenames):
+                        print("Reading {}".format(os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, data_part_fname)))
+                        data_part_file, data_part = read_chunked_data(os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, data_part_fname))
+                        data_mask_part_file, data_mask_part = read_chunked_data(os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, data_parts_mask_filenames[i]))
+
+                        if 'data' not in locals():
+                            all_data_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+ext)
+                            if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
+                                allfile = h5py.File(all_data_filename,'w')
+                                data = allfile.create_dataset("data", data_part.shape, dtype=self.dtype_str, compression="gzip")
+                            else:
+                                allfile = zarr.open_group(all_data_filename, mode="w")
+                                data = allfile.create_dataset("data", shape=data_part.shape, dtype=self.dtype_str, compression="gzip")
 
-                    if 'data' not in locals():
-                        all_data_filename = os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+ext)
-                        if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
-                            allfile = h5py.File(all_data_filename,'w')
-                            data = allfile.create_dataset("data", data_part.shape, dtype=self.dtype_str, compression="gzip")
-                        else:
-                            allfile = zarr.open_group(all_data_filename, mode="w")
-                            data = allfile.create_dataset("data", shape=data_part.shape, dtype=self.dtype_str, compression="gzip")
+                        for j, k in enumerate(list_of_vols_in_z[i]):
+                            
+                            slices = (
+                                slice(z_vol_info[k][0],z_vol_info[k][1]), # z (only z axis is distributed across GPUs)
+                                slice(None), # y
+                                slice(None), # x
+                                slice(None), # Channel
+                            )
+                            
+                            data_ordered_slices = order_dimensions(
+                                slices,
+                                input_order="ZYXC",
+                                output_order=out_data_order,
+                                default_value=0)
+
+                            if self.cfg.TEST.VERBOSE:
+                                print(f"Filling {k} [{z_vol_info[k][0]}:{z_vol_info[k][1]}]")
+                            data[data_ordered_slices] = data_part[data_ordered_slices] / data_mask_part[data_ordered_slices]
 
-                    for j, k in enumerate(list_of_vols_in_z[i]):
-                        
-                        slices = (
-                            slice(z_vol_info[k][0],z_vol_info[k][1]), # z (only z axis is distributed across GPUs)
-                            slice(None), # y
-                            slice(None), # x
-                            slice(None), # Channel
-                        )
-                        
-                        data_ordered_slices = order_dimensions(
-                            slices,
-                            input_order="ZYXC",
-                            output_order=out_data_order,
-                            default_value=0)
-
-                        if self.cfg.TEST.VERBOSE:
-                            print(f"Filling {k} [{z_vol_info[k][0]}:{z_vol_info[k][1]}]")
-                        data[data_ordered_slices] = data_part[data_ordered_slices] / data_mask_part[data_ordered_slices]
+                            if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
+                                allfile.flush() 
 
                         if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
-                            allfile.flush() 
-
-                    if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
-                        data_part_file.close()
-                        data_mask_part_file.close()
+                            data_part_file.close()
+                            data_mask_part_file.close()
 
-                # Save image
-                if self.cfg.TEST.BY_CHUNKS.SAVE_OUT_TIF and self.cfg.PATHS.RESULT_DIR.PER_IMAGE != "":
-                    current_order = np.array(range(len(data.shape)))
-                    transpose_order = order_dimensions(current_order, input_order=out_data_order,
-                        output_order="TZYXC", default_value=np.nan)
-                    transpose_order = [x for x in transpose_order if not np.isnan(x)]
-                    data = np.array(data, dtype=self.dtype).transpose(transpose_order)
-                    if "T" not in out_data_order:
-                        data = np.expand_dims(data,0)
+                    # Save image
+                    if self.cfg.TEST.BY_CHUNKS.SAVE_OUT_TIF and self.cfg.PATHS.RESULT_DIR.PER_IMAGE != "":
+                        current_order = np.array(range(len(data.shape)))
+                        transpose_order = order_dimensions(current_order, input_order=out_data_order,
+                            output_order="TZYXC", default_value=np.nan)
+                        transpose_order = [x for x in transpose_order if not np.isnan(x)]
+                        data = np.array(data, dtype=self.dtype).transpose(transpose_order)
+                        if "T" not in out_data_order:
+                            data = np.expand_dims(data,0)
 
-                    save_tif(data, self.cfg.PATHS.RESULT_DIR.PER_IMAGE, [filename+".tif"], verbose=self.cfg.TEST.VERBOSE)
+                        save_tif(data, self.cfg.PATHS.RESULT_DIR.PER_IMAGE, [filename+".tif"], verbose=self.cfg.TEST.VERBOSE)
 
-                if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
-                    allfile.close()      
+                    if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
+                        allfile.close()      
 
-            # Just make the division with the overlap
-            else:
-                # Load predictions and overlapping mask
-                pred_file, pred = read_chunked_data(out_data_filename)
-                mask_file, mask = read_chunked_data(out_data_mask_filename)
-
-                # Create new file
-                if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
-                    fid_div = h5py.File(out_data_div_filename,'w')
-                    pred_div = fid_div.create_dataset("data", pred.shape, dtype=pred.dtype, compression="gzip")
+                # Just make the division with the overlap
                 else:
-                    fid_div = zarr.open_group(out_data_div_filename, mode="w")
-                    pred_div = fid_div.create_dataset("data", shape=pred.shape, dtype=pred.dtype)
-                    
-                t_dim, z_dim, c_dim, y_dim, x_dim = order_dimensions(
-                    data_shape, self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER)
-                
-                # Fill the new data
-                z_vols = math.ceil(z_dim/self.cfg.DATA.PATCH_SIZE[0])
-                y_vols = math.ceil(y_dim/self.cfg.DATA.PATCH_SIZE[1])
-                x_vols = math.ceil(x_dim/self.cfg.DATA.PATCH_SIZE[2])
-                for z in tqdm(range(z_vols), disable=not is_main_process()):
-                    for y in range(y_vols):
-                        for x in range(x_vols):
+                    # Load predictions and overlapping mask
+                    pred_file, pred = read_chunked_data(out_data_filename)
+                    mask_file, mask = read_chunked_data(out_data_mask_filename)
 
-                            slices = (
-                                slice(z*self.cfg.DATA.PATCH_SIZE[0], min(z_dim,self.cfg.DATA.PATCH_SIZE[0]*(z+1))),
-                                slice(y*self.cfg.DATA.PATCH_SIZE[1], min(y_dim,self.cfg.DATA.PATCH_SIZE[1]*(y+1))),
-                                slice(x*self.cfg.DATA.PATCH_SIZE[2], min(x_dim,self.cfg.DATA.PATCH_SIZE[2]*(x+1))),
-                                slice(0,pred.shape[c_index]), # Channel
-                            )
-
-                            data_ordered_slices = order_dimensions(
-                                slices,
-                                input_order = "ZYXC",
-                                output_order = out_data_order,
-                                default_value = 0,
+                    # Create new file
+                    if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
+                        fid_div = h5py.File(out_data_div_filename,'w')
+                        pred_div = fid_div.create_dataset("data", pred.shape, dtype=pred.dtype, compression="gzip")
+                    else:
+                        fid_div = zarr.open_group(out_data_div_filename, mode="w")
+                        pred_div = fid_div.create_dataset("data", shape=pred.shape, dtype=pred.dtype)
+                        
+                    t_dim, z_dim, c_dim, y_dim, x_dim = order_dimensions(
+                        data_shape, self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER)
+                    
+                    # Fill the new data
+                    z_vols = math.ceil(z_dim/self.cfg.DATA.PATCH_SIZE[0])
+                    y_vols = math.ceil(y_dim/self.cfg.DATA.PATCH_SIZE[1])
+                    x_vols = math.ceil(x_dim/self.cfg.DATA.PATCH_SIZE[2])
+                    for z in tqdm(range(z_vols), disable=not is_main_process()):
+                        for y in range(y_vols):
+                            for x in range(x_vols):
+
+                                slices = (
+                                    slice(z*self.cfg.DATA.PATCH_SIZE[0], min(z_dim,self.cfg.DATA.PATCH_SIZE[0]*(z+1))),
+                                    slice(y*self.cfg.DATA.PATCH_SIZE[1], min(y_dim,self.cfg.DATA.PATCH_SIZE[1]*(y+1))),
+                                    slice(x*self.cfg.DATA.PATCH_SIZE[2], min(x_dim,self.cfg.DATA.PATCH_SIZE[2]*(x+1))),
+                                    slice(0,pred.shape[c_index]), # Channel
                                 )
-                            pred_div[data_ordered_slices] = pred[data_ordered_slices] / mask[data_ordered_slices]
 
-                    if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
-                        fid_div.flush()
+                                data_ordered_slices = order_dimensions(
+                                    slices,
+                                    input_order = "ZYXC",
+                                    output_order = out_data_order,
+                                    default_value = 0,
+                                    )
+                                pred_div[data_ordered_slices] = pred[data_ordered_slices] / mask[data_ordered_slices]
 
-                # Save image
-                if self.cfg.TEST.BY_CHUNKS.SAVE_OUT_TIF and self.cfg.PATHS.RESULT_DIR.PER_IMAGE != "":
-                    current_order = np.array(range(len(pred_div.shape)))
-                    transpose_order = order_dimensions(current_order, input_order=out_data_order,
-                        output_order="TZYXC", default_value=np.nan)
-                    transpose_order = [x for x in transpose_order if not np.isnan(x)]
-                    pred_div = np.array(pred_div, dtype=self.dtype).transpose(transpose_order)
-                    if "T" not in out_data_order:
-                        pred_div = np.expand_dims(pred_div,0)
+                        if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
+                            fid_div.flush()
 
-                    save_tif(pred_div, self.cfg.PATHS.RESULT_DIR.PER_IMAGE, [os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+".tif")],
-                        verbose=self.cfg.TEST.VERBOSE)
+                    # Save image
+                    if self.cfg.TEST.BY_CHUNKS.SAVE_OUT_TIF and self.cfg.PATHS.RESULT_DIR.PER_IMAGE != "":
+                        current_order = np.array(range(len(pred_div.shape)))
+                        transpose_order = order_dimensions(current_order, input_order=out_data_order,
+                            output_order="TZYXC", default_value=np.nan)
+                        transpose_order = [x for x in transpose_order if not np.isnan(x)]
+                        pred_div = np.array(pred_div, dtype=self.dtype).transpose(transpose_order)
+                        if "T" not in out_data_order:
+                            pred_div = np.expand_dims(pred_div,0)
 
-                if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
-                    pred_file.close()
-                    mask_file.close()
-                    fid_div.close()
+                        save_tif(pred_div, self.cfg.PATHS.RESULT_DIR.PER_IMAGE, [os.path.join(self.cfg.PATHS.RESULT_DIR.PER_IMAGE, filename+".tif")],
+                            verbose=self.cfg.TEST.VERBOSE)
+
+                    if self.cfg.TEST.BY_CHUNKS.FORMAT == "h5":
+                        pred_file.close()
+                        mask_file.close()
+                        fid_div.close()
 
             if self.cfg.TEST.BY_CHUNKS.WORKFLOW_PROCESS:
                 if self.cfg.TEST.BY_CHUNKS.WORKFLOW_PROCESS.TYPE == "chunk_by_chunk":
                     self.after_merge_patches_by_chunks_proccess_patch(out_data_div_filename) 
                 else:            
                     self.after_merge_patches_by_chunks_proccess_entire_pred(out_data_div_filename) 
                     
@@ -1551,14 +1576,17 @@
         else:
             min_val = min(pred.shape)
             channel_pos = pred.shape.index(min_val)
             if channel_pos != 3 and pred.shape[channel_pos] <= 4:
                 new_pos = [x for x in range(4) if x != channel_pos]+[channel_pos,]
                 pred = pred.transpose(new_pos)
 
+        if pred.ndim == 4: 
+            pred = np.expand_dims(pred, 0)
+
         fname, file_extension = os.path.splitext(os.path.basename(filename))
         self.processing_filenames = [fname+".tif"]
         self.after_merge_patches(pred)
 
     @abstractmethod
     def after_merge_patches_by_chunks_proccess_patch(self, filename):
         """
```

### Comparing `biapy-3.4.3/biapy/engine/check_configuration.py` & `biapy-3.4.4/biapy/engine/check_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,16 +393,14 @@
         if cfg.PROBLEM.IMAGE_TO_IMAGE.MULTIPLE_RAW_ONE_TARGET_LOADER:
             if cfg.DATA.TRAIN.IN_MEMORY:
                 raise ValueError("'PROBLEM.IMAGE_TO_IMAGE.MULTIPLE_RAW_ONE_TARGET_LOADER' can only be used if 'DATA.TRAIN.IN_MEMORY' == 'False'")
             if cfg.DATA.VAL.IN_MEMORY:
                 raise ValueError("'PROBLEM.IMAGE_TO_IMAGE.MULTIPLE_RAW_ONE_TARGET_LOADER' can only be used if 'DATA.VAL.IN_MEMORY' == 'False'")
             if cfg.DATA.TEST.IN_MEMORY:
                 raise ValueError("'PROBLEM.IMAGE_TO_IMAGE.MULTIPLE_RAW_ONE_TARGET_LOADER' can only be used if 'DATA.TEST.IN_MEMORY' == 'False'")
-        if cfg.PROBLEM.NDIM == '3D':
-            raise ValueError("3D workflow not available for 'IMAGE_TO_IMAGE' yet")
             
     if cfg.DATA.EXTRACT_RANDOM_PATCH and cfg.DATA.PROBABILITY_MAP:
         if cfg.DATA.W_FOREGROUND+cfg.DATA.W_BACKGROUND != 1:
             raise ValueError("cfg.DATA.W_FOREGROUND+cfg.DATA.W_BACKGROUND need to sum 1. E.g. 0.94 and 0.06 respectively.")
     if not cfg.DATA.TRAIN.IN_MEMORY and cfg.DATA.PREPROCESS.TRAIN:
         raise ValueError('To use preprocessing DATA.TRAIN.IN_MEMORY needs to be True.')
     if not cfg.DATA.VAL.IN_MEMORY and cfg.DATA.PREPROCESS.VAL:
@@ -435,55 +433,76 @@
         if not cfg.DATA.PREPROCESS.VAL and cfg.DATA.VAL.FROM_TRAIN and cfg.DATA.PREPROCESS.TRAIN:
             raise ValueError("When 'DATA.VAL.FROM_TRAIN' is True and 'DATA.PREPROCESS.TRAIN' is True, 'DATA.PREPROCESS.VAL' also needs to be True.")
         if cfg.DATA.PREPROCESS.MATCH_HISTOGRAM.ENABLE:
             if not os.path.exists(cfg.DATA.PREPROCESS.MATCH_HISTOGRAM.REFERENCE_PATH):
                 raise ValueError(f"Path pointed by 'DATA.PREPROCESS.MATCH_HISTOGRAM.REFERENCE_PATH' does not exist: {cfg.DATA.PREPROCESS.MATCH_HISTOGRAM.REFERENCE_PATH}")
 
     #### Data #### 
-    if cfg.TRAIN.ENABLE and check_data_paths:
-        if not os.path.exists(cfg.DATA.TRAIN.PATH):
-            raise ValueError("Train data dir not found: {}".format(cfg.DATA.TRAIN.PATH))
-        if not os.path.exists(cfg.DATA.TRAIN.GT_PATH) and cfg.PROBLEM.TYPE not in ['DENOISING', "CLASSIFICATION", "SELF_SUPERVISED"]:
-            raise ValueError("Train mask data dir not found: {}".format(cfg.DATA.TRAIN.GT_PATH))
-        if not cfg.DATA.VAL.FROM_TRAIN and not cfg.DATA.VAL.IN_MEMORY:
-            if not os.path.exists(cfg.DATA.VAL.PATH):
-                raise ValueError("Validation data dir not found: {}".format(cfg.DATA.VAL.PATH))
-            if not os.path.exists(cfg.DATA.VAL.GT_PATH) and cfg.PROBLEM.TYPE not in ['DENOISING', "CLASSIFICATION", "SELF_SUPERVISED"]:
-                raise ValueError("Validation mask data dir not found: {}".format(cfg.DATA.VAL.GT_PATH))
+    if cfg.TRAIN.ENABLE:
+        if check_data_paths:
+            if not os.path.exists(cfg.DATA.TRAIN.PATH):
+                raise ValueError("Train data dir not found: {}".format(cfg.DATA.TRAIN.PATH))
+            if not os.path.exists(cfg.DATA.TRAIN.GT_PATH) and cfg.PROBLEM.TYPE not in ['DENOISING', "CLASSIFICATION", "SELF_SUPERVISED"] and\
+            not cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA:
+                raise ValueError("Train mask data dir not found: {}".format(cfg.DATA.TRAIN.GT_PATH))
+            if not cfg.DATA.VAL.FROM_TRAIN and not cfg.DATA.VAL.IN_MEMORY:
+                if not os.path.exists(cfg.DATA.VAL.PATH):
+                    raise ValueError("Validation data dir not found: {}".format(cfg.DATA.VAL.PATH))
+                if not os.path.exists(cfg.DATA.VAL.GT_PATH) and cfg.PROBLEM.TYPE not in ['DENOISING', "CLASSIFICATION", "SELF_SUPERVISED"] and\
+                not cfg.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA:
+                    raise ValueError("Validation mask data dir not found: {}".format(cfg.DATA.VAL.GT_PATH))
+        if cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA:
+            if cfg.PROBLEM.NDIM != '3D':
+                raise ValueError("'DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA' to True is only implemented in 3D workflows")
+            if cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH == '' or cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_GT_PATH == '':
+                raise ValueError("'DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH' and 'DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA_GT_PATH' "
+                    "need to be set when 'DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA' is used.")
+        if cfg.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA:
+            if cfg.PROBLEM.NDIM != '3D':
+                raise ValueError("'DATA.VAL.INPUT_ZARR_MULTIPLE_DATA' to True is only implemented in 3D workflows")
+            if cfg.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH == '' or cfg.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA_GT_PATH == '':
+                raise ValueError("'DATA.VAL.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH' and 'DATA.VAL.INPUT_ZARR_MULTIPLE_DATA_GT_PATH' "
+                    "need to be set when 'DATA.VAL.INPUT_ZARR_MULTIPLE_DATA' is used.")
+
     if cfg.TEST.ENABLE and not cfg.DATA.TEST.USE_VAL_AS_TEST and check_data_paths:
         if not os.path.exists(cfg.DATA.TEST.PATH):
             raise ValueError("Test data not found: {}".format(cfg.DATA.TEST.PATH))
-        if cfg.DATA.TEST.LOAD_GT and not os.path.exists(cfg.DATA.TEST.GT_PATH) and cfg.PROBLEM.TYPE not in ["CLASSIFICATION", "SELF_SUPERVISED"]:
+        if cfg.DATA.TEST.LOAD_GT and not os.path.exists(cfg.DATA.TEST.GT_PATH) and cfg.PROBLEM.TYPE not in ["CLASSIFICATION", "SELF_SUPERVISED"] and\
+        not cfg.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA:
             raise ValueError("Test data mask not found: {}".format(cfg.DATA.TEST.GT_PATH))
-    if cfg.TEST.BY_CHUNKS.ENABLE:
+    if cfg.TEST.ENABLE and cfg.TEST.BY_CHUNKS.ENABLE:
         if cfg.PROBLEM.NDIM == '2D':
             raise ValueError("'TEST.BY_CHUNKS' can not be activated when 'PROBLEM.NDIM' is 2D")
         assert cfg.TEST.BY_CHUNKS.FORMAT.lower() in ["h5", "zarr"], "'TEST.BY_CHUNKS.FORMAT' needs to be one between ['H5', 'Zarr']"
         opts.extend(['TEST.BY_CHUNKS.FORMAT', cfg.TEST.BY_CHUNKS.FORMAT.lower()])
         if cfg.TEST.BY_CHUNKS.WORKFLOW_PROCESS.ENABLE:     
             assert cfg.TEST.BY_CHUNKS.WORKFLOW_PROCESS.TYPE in ["chunk_by_chunk", "entire_pred"], \
                 "'TEST.BY_CHUNKS.WORKFLOW_PROCESS.TYPE' needs to be one between ['chunk_by_chunk', 'entire_pred']"
         if len(cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER) < 3:
             raise ValueError("'TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER' needs to be at least of length 3, e.g., 'ZYX'")
         if cfg.MODEL.N_CLASSES > 2:
             raise ValueError("Not implemented pipeline option: 'MODEL.N_CLASSES' > 2 and 'TEST.BY_CHUNKS'")
+        if cfg.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA and (cfg.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH == '' or \
+            cfg.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_GT_PATH == ''):
+            raise ValueError("'TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_RAW_PATH' and 'TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_GT_PATH' "
+                "need to be set when 'TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA' is used.")
 
     if cfg.TRAIN.ENABLE:
         if cfg.DATA.EXTRACT_RANDOM_PATCH and cfg.DATA.PROBABILITY_MAP:
             if not cfg.PROBLEM.TYPE == 'SEMANTIC_SEG':
                 raise ValueError("'DATA.PROBABILITY_MAP' can only be selected when 'PROBLEM.TYPE' is 'SEMANTIC_SEG'")
 
         if cfg.DATA.VAL.FROM_TRAIN and not cfg.DATA.VAL.CROSS_VAL and cfg.DATA.VAL.SPLIT_TRAIN <= 0:
             raise ValueError("'DATA.VAL.SPLIT_TRAIN' needs to be > 0 when 'DATA.VAL.FROM_TRAIN' == True")
         
         if cfg.DATA.VAL.FROM_TRAIN and not cfg.DATA.TRAIN.IN_MEMORY:
             zarr_files = sorted(next(os.walk(cfg.DATA.TRAIN.PATH))[1])
             if len(zarr_files) == 0:
                 raise ValueError("Validation can only be extracted from train, when 'DATA.TRAIN.IN_MEMORY' == False, if 'DATA.TRAIN.PATH' "
-                    " contain Zarr files. If it's not your case, please, set 'DATA.VAL.FROM_TRAIN' to False and configure "
+                    "contains Zarr files. If it's not your case, please, set 'DATA.VAL.FROM_TRAIN' to False and configure "
                     "'DATA.VAL.PATH'/'DATA.VAL.GT_PATH'")
         if cfg.PROBLEM.NDIM == '2D' and cfg.DATA.TRAIN.INPUT_IMG_AXES_ORDER != 'TZCYX':
             raise ValueError("'DATA.TRAIN.INPUT_IMG_AXES_ORDER' can not be set in 2D problems")
         if cfg.PROBLEM.NDIM == '2D' and cfg.DATA.TRAIN.INPUT_MASK_AXES_ORDER != 'TZCYX':
             raise ValueError("'DATA.TRAIN.INPUT_MASK_AXES_ORDER' can not be set in 2D problems")
         if len(cfg.DATA.TRAIN.INPUT_IMG_AXES_ORDER) < 3:
             raise ValueError("'DATA.TRAIN.INPUT_IMG_AXES_ORDER' needs to be at least of length 3, e.g., 'ZYX'")
@@ -616,15 +635,15 @@
         opts.extend(['PROBLEM.SUPER_RESOLUTION.UPSCALING', (1,)*dim_count])
 
     if len(opts) > 0:
         cfg.merge_from_list(opts)
 
     if cfg.MODEL.SOURCE == "biapy":
         assert cfg.MODEL.LAST_ACTIVATION.lower() in ["relu", "tanh", "leaky_relu", "elu", "gelu", "silu", "sigmoid","softmax", "linear", "none"], \
-            "Get unknown activation key {}".format(activation)
+            "Get unknown activation key {}".format(cfg.MODEL.LAST_ACTIVATION.lower())
     
         if cfg.MODEL.UPSAMPLE_LAYER.lower() not in ["upsampling", "convtranspose"]:
             raise ValueError("cfg.MODEL.UPSAMPLE_LAYER' needs to be one between ['upsampling', 'convtranspose']. Provided {}"
                             .format(cfg.MODEL.UPSAMPLE_LAYER))
         if cfg.PROBLEM.TYPE in ["SEMANTIC_SEG", "INSTANCE_SEG", "DETECTION", "DENOISING"]:
             if model_arch not in ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']:
                 raise ValueError("Architectures available for {} are: ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']"
@@ -634,15 +653,15 @@
                 raise ValueError("Architectures available for 2D 'SUPER_RESOLUTION' are: ['edsr', 'rcan', 'dfcan', 'wdsr', 'unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'multiresunet']")
             elif cfg.PROBLEM.NDIM == '3D':
                 if model_arch not in ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'multiresunet']:
                     raise ValueError("Architectures available for 3D 'SUPER_RESOLUTION' are: ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'multiresunet']")
                 assert cfg.MODEL.UNET_SR_UPSAMPLE_POSITION in ["pre", "post"], "'MODEL.UNET_SR_UPSAMPLE_POSITION' not in ['pre', 'post']"
         elif cfg.PROBLEM.TYPE == 'IMAGE_TO_IMAGE':
             if model_arch not in ['edsr', 'rcan', 'dfcan', 'wdsr', 'unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']:
-                raise ValueError("Architectures available for 2D 'SUPER_RESOLUTION' are: ['edsr', 'rcan', 'dfcan', 'wdsr', 'unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']")
+                raise ValueError("Architectures available for 2D 'IMAGE_TO_IMAGE' are: ['edsr', 'rcan', 'dfcan', 'wdsr', 'unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']")
         elif cfg.PROBLEM.TYPE == 'SELF_SUPERVISED':
             if model_arch not in ['unet', 'resunet', 'resunet++', 'attention_unet', 'multiresunet', 'seunet',  
                 'unetr', 'edsr', 'rcan', 'dfcan', 'wdsr', 'vit', 'mae']:
                 raise ValueError("'SELF_SUPERVISED' models available are these: ['unet', 'resunet', 'resunet++', 'attention_unet', 'multiresunet', 'seunet', " 
                     "'unetr', 'edsr', 'rcan', 'dfcan', 'wdsr', 'vit', 'mae']")
         elif cfg.PROBLEM.TYPE == 'CLASSIFICATION':
             if model_arch not in ['simple_cnn', 'vit'] and 'efficientnet' not in model_arch:
@@ -656,17 +675,17 @@
                 raise ValueError("'MODEL.VIT_EMBED_DIM' should be divisible by 'MODEL.VIT_NUM_HEADS'")
             if not all([i == cfg.DATA.PATCH_SIZE[0] for i in cfg.DATA.PATCH_SIZE[:-1]]):      
                 raise ValueError("'unetr', 'vit' 'mae' models need to have same shape in all dimensions (e.g. DATA.PATCH_SIZE = (80,80,80,1) )")
         # Check that the input patch size is divisible in every level of the U-Net's like architectures, as the model
         # will throw an error not very clear for users
         if model_arch in ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'multiresunet']:
             z_size = cfg.DATA.PATCH_SIZE[0]
+            sizes = cfg.DATA.PATCH_SIZE[1:-1]
             for i in range(len(cfg.MODEL.FEATURE_MAPS)-1):
-                sizes = cfg.DATA.PATCH_SIZE[:-1]
-                if not all([False for x in sizes if x%(np.power(2,(i+1))) != 0 and z_size % cfg.MODEL.Z_DOWN[i] != 0 or x == 0]):
+                if not all([False for x in sizes if x%(np.power(2,(i+1))) != 0 or z_size % cfg.MODEL.Z_DOWN[i] != 0]):
                     m = "The 'DATA.PATCH_SIZE' provided is not divisible by 2 in each of the U-Net's levels. You can:\n 1) Reduce the number " + \
                             "of levels (by reducing 'cfg.MODEL.FEATURE_MAPS' array's length)\n 2) Increase 'DATA.PATCH_SIZE'"
                     if cfg.PROBLEM.NDIM == '3D':
                         m += "\n 3) If the Z axis is the problem, as the patch size is normally less than in other axis due to resolution, you " + \
                             "can tune 'MODEL.Z_DOWN' variable to not downsample the image in all U-Net levels"
                     raise ValueError(m)
                 z_size = z_size // cfg.MODEL.Z_DOWN[i]
```

### Comparing `biapy-3.4.3/biapy/engine/classification.py` & `biapy-3.4.4/biapy/engine/classification.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/denoising.py` & `biapy-3.4.4/biapy/engine/denoising.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/detection.py` & `biapy-3.4.4/biapy/engine/detection.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/image_to_image.py` & `biapy-3.4.4/biapy/engine/image_to_image.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/instance_seg.py` & `biapy-3.4.4/biapy/engine/instance_seg.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from skimage.segmentation import clear_border
 from skimage.transform import resize
 import torch.distributed as dist
 
 from biapy.data.post_processing.post_processing import (watershed_by_channels, voronoi_on_mask, 
     measure_morphological_props_and_filter, repare_large_blobs, apply_binary_mask)
 from biapy.data.pre_processing import create_instance_channels, create_test_instance_channels, norm_range01
-from biapy.utils.util import save_tif
+from biapy.utils.util import save_tif, read_chunked_data, read_chunked_nested_data
 from biapy.utils.matching import matching, wrapper_matching_dataset_lazy
 from biapy.engine.metrics import jaccard_index, instance_segmentation_loss, instance_metrics
 from biapy.engine.base_workflow import Base_Workflow
 from biapy.utils.misc import is_main_process, is_dist_avail_and_initialized
 
 
 class Instance_Segmentation_Workflow(Base_Workflow):
@@ -213,15 +213,14 @@
         """
         assert pred.ndim == 4, "Prediction doesn't have 4 dim: {pred.shape}"
 
         #############################
         ### INSTANCE SEGMENTATION ###
         #############################
         if not self.instances_already_created: 
-
             # Multi-head: instances + classification
             if self.cfg.MODEL.N_CLASSES > 2:
                 class_channel = np.expand_dims(pred[...,-1], -1)
                 pred = pred[...,:-1] 
 
             print("Creating instances with watershed . . .")
             w_dir = os.path.join(self.cfg.PATHS.WATERSHED_DIR, filenames[0])
@@ -280,15 +279,22 @@
                 del self._Y
                 _Y = np.zeros(w_pred.shape, dtype=w_pred.dtype)
                 for i in range(len(self.test_filenames)):
                     test_file = os.path.join(self.original_test_mask_path, self.test_filenames[i])
                     _Y[i] = imread(test_file).squeeze()
             else:
                 test_file = os.path.join(self.original_test_mask_path, self.test_filenames[self.f_numbers[0]])
-                _Y = imread(test_file).squeeze()
+                if test_file.endswith('.zarr'):
+                    if self.cfg.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA:
+                        _, _Y = read_chunked_nested_data(test_file, self.cfg.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA_GT_PATH)
+                    else:
+                        _, _Y = read_chunked_data(test_file)
+                    _Y = np.squeeze(np.array(_Y))
+                else:
+                    _Y = imread(test_file).squeeze()
 
             # Multi-head: instances + classification
             if self.cfg.MODEL.N_CLASSES > 2:
                 # Channel check
                 error_shape = None
                 if self.cfg.PROBLEM.NDIM == "2D" and _Y.ndim != 3:
                     error_shape = (256,256,2)
@@ -754,69 +760,128 @@
 
     def prepare_instance_data(self):
         """
         Creates instance segmentation ground truth images to train the model based on the ground truth instances provided.
         They will be saved in a separate folder in the root path of the ground truth. 
         """
         original_test_path, original_test_mask_path = None, None
+        train_channel_dir = self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_DIR
+        train_channel_mask_dir = self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_MASK_DIR
+        val_channel_dir = self.cfg.DATA.VAL.INSTANCE_CHANNELS_DIR
+        val_channel_mask_dir = self.cfg.DATA.VAL.INSTANCE_CHANNELS_MASK_DIR
+        test_channel_dir = self.cfg.DATA.TEST.INSTANCE_CHANNELS_DIR
+        test_channel_mask_dir = self.cfg.DATA.TEST.INSTANCE_CHANNELS_MASK_DIR
+        test_instance_mask_dir = self.cfg.DATA.TEST.GT_PATH
+        opts = []
 
-        if is_main_process():
-            print("###########################")
-            print("#  PREPARE INSTANCE DATA  #")
-            print("###########################")
-
-            # Create selected channels for train data
-            if (self.cfg.TRAIN.ENABLE or self.cfg.DATA.TEST.USE_VAL_AS_TEST) and (not os.path.isdir(self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_DIR) or \
-                not os.path.isdir(self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_MASK_DIR)):
+        print("###########################")
+        print("#  PREPARE INSTANCE DATA  #")
+        print("###########################")
+
+        # Create selected channels for train data
+        if (self.cfg.TRAIN.ENABLE or self.cfg.DATA.TEST.USE_VAL_AS_TEST) and (not os.path.isdir(self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_DIR) or \
+            not os.path.isdir(self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_MASK_DIR)):
+            do_mask = True
+            if self.cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA:
+                do_mask = not os.path.isdir(self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_DIR)
+                train_channel_dir = self.cfg.DATA.TRAIN.PATH
+                train_channel_mask_dir = self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_DIR
+            
+            if do_mask and is_main_process():
                 print("You select to create {} channels from given instance labels and no file is detected in {}. "
                         "So let's prepare the data. Notice that, if you do not modify 'DATA.TRAIN.INSTANCE_CHANNELS_DIR' "
                         "path, this process will be done just once!".format(self.cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS,
                         self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_DIR))
                 create_instance_channels(self.cfg)
-
-            # Create selected channels for val data
-            if self.cfg.TRAIN.ENABLE and not self.cfg.DATA.VAL.FROM_TRAIN and (not os.path.isdir(self.cfg.DATA.VAL.INSTANCE_CHANNELS_DIR) or \
-                not os.path.isdir(self.cfg.DATA.VAL.INSTANCE_CHANNELS_MASK_DIR)):
+            
+            # Change the value of DATA.TRAIN.INPUT_MASK_AXES_ORDER as we have created the instance mask and maybe the user doesn't 
+            # know the data order that is created.
+            if self.cfg.DATA.TRAIN.INPUT_ZARR_MULTIPLE_DATA:
+                out_data_order = self.cfg.DATA.TRAIN.INPUT_IMG_AXES_ORDER
+                if "C" not in self.cfg.DATA.TRAIN.INPUT_IMG_AXES_ORDER:
+                    out_data_order += "C"
+                print("DATA.TRAIN.INPUT_MASK_AXES_ORDER changed from {} to {}".format(self.cfg.DATA.TRAIN.INPUT_MASK_AXES_ORDER, out_data_order))
+                opts.extend([f"DATA.TRAIN.INPUT_MASK_AXES_ORDER", out_data_order])
+
+        # Create selected channels for val data
+        if self.cfg.TRAIN.ENABLE and not self.cfg.DATA.VAL.FROM_TRAIN and (not os.path.isdir(self.cfg.DATA.VAL.INSTANCE_CHANNELS_DIR) or \
+            not os.path.isdir(self.cfg.DATA.VAL.INSTANCE_CHANNELS_MASK_DIR)):
+            do_mask = True
+            if self.cfg.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA:
+                do_mask = not os.path.isdir(self.cfg.DATA.VAL.INSTANCE_CHANNELS_DIR)
+                val_channel_dir = self.cfg.DATA.VAL.PATH
+                val_channel_mask_dir = self.cfg.DATA.VAL.INSTANCE_CHANNELS_DIR
+            
+            if do_mask and is_main_process():
                 print("You select to create {} channels from given instance labels and no file is detected in {}. "
                         "So let's prepare the data. Notice that, if you do not modify 'DATA.VAL.INSTANCE_CHANNELS_DIR' "
                         "path, this process will be done just once!".format(self.cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS,
                         self.cfg.DATA.VAL.INSTANCE_CHANNELS_DIR))
                 create_instance_channels(self.cfg, data_type='val')
 
-            # Create selected channels for test data once
-            if self.cfg.TEST.ENABLE and not self.cfg.DATA.TEST.USE_VAL_AS_TEST and (not os.path.isdir(self.cfg.DATA.TEST.INSTANCE_CHANNELS_DIR) or \
-                (not os.path.isdir(self.cfg.DATA.TEST.INSTANCE_CHANNELS_MASK_DIR) and self.cfg.DATA.TEST.LOAD_GT)) and not self.cfg.TEST.BY_CHUNKS.ENABLE:
+            # Change the value of DATA.VAL.INPUT_MASK_AXES_ORDER as we have created the instance mask and maybe the user doesn't 
+            # know the data order that is created.
+            if self.cfg.DATA.VAL.INPUT_ZARR_MULTIPLE_DATA:
+                out_data_order = self.cfg.DATA.VAL.INPUT_IMG_AXES_ORDER
+                if "C" not in self.cfg.DATA.VAL.INPUT_IMG_AXES_ORDER:
+                    out_data_order += "C"
+                print("DATA.VAL.INPUT_MASK_AXES_ORDER changed from {} to {}".format(self.cfg.DATA.VAL.INPUT_MASK_AXES_ORDER, out_data_order))
+                opts.extend([f"DATA.VAL.INPUT_MASK_AXES_ORDER", out_data_order])
+
+        # Create selected channels for test data once
+        if self.cfg.TEST.ENABLE and not self.cfg.DATA.TEST.USE_VAL_AS_TEST and (not os.path.isdir(self.cfg.DATA.TEST.INSTANCE_CHANNELS_DIR) or \
+            (not os.path.isdir(self.cfg.DATA.TEST.INSTANCE_CHANNELS_MASK_DIR) and self.cfg.DATA.TEST.LOAD_GT)):
+            do_mask = True
+            if self.cfg.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA:
+                do_mask = not os.path.isdir(self.cfg.DATA.TEST.INSTANCE_CHANNELS_DIR)                    
+                test_channel_dir = self.cfg.DATA.TEST.PATH
+                test_channel_mask_dir = self.cfg.DATA.TEST.INSTANCE_CHANNELS_DIR
+                test_instance_mask_dir = self.cfg.DATA.TEST.PATH
+                
+            if do_mask and is_main_process():
                 print("You select to create {} channels from given instance labels and no file is detected in {}. "
                         "So let's prepare the data. Notice that, if you do not modify 'DATA.TEST.INSTANCE_CHANNELS_DIR' "
                         "path, this process will be done just once!".format(self.cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS,
                         self.cfg.DATA.TEST.INSTANCE_CHANNELS_MASK_DIR))
                 create_test_instance_channels(self.cfg)
 
+            # Change the value of TEST.BY_CHUNKS.INPUT_MASK_AXES_ORDER as we have created the instance mask and maybe the user doesn't 
+            # know the data order that is created.
+            if self.cfg.TEST.BY_CHUNKS.INPUT_ZARR_MULTIPLE_DATA:
+                out_data_order = self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER
+                if "C" not in self.cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER:
+                    out_data_order += "C"
+                print("TEST.BY_CHUNKS.INPUT_MASK_AXES_ORDER changed from {} to {}".format(self.cfg.TEST.BY_CHUNKS.INPUT_MASK_AXES_ORDER, out_data_order))
+                opts.extend([f"TEST.BY_CHUNKS.INPUT_MASK_AXES_ORDER", out_data_order])
+
         if is_dist_avail_and_initialized():
             dist.barrier()
 
-        opts = []
         if self.cfg.TRAIN.ENABLE:
-            print("DATA.TRAIN.PATH changed from {} to {}".format(self.cfg.DATA.TRAIN.PATH, self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_DIR))
-            print("DATA.TRAIN.GT_PATH changed from {} to {}".format(self.cfg.DATA.TRAIN.GT_PATH, self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_MASK_DIR))
-            opts.extend(['DATA.TRAIN.PATH', self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_DIR,
-                        'DATA.TRAIN.GT_PATH', self.cfg.DATA.TRAIN.INSTANCE_CHANNELS_MASK_DIR])
+            if self.cfg.DATA.TRAIN.PATH != train_channel_dir:
+                print("DATA.TRAIN.PATH changed from {} to {}".format(self.cfg.DATA.TRAIN.PATH, train_channel_dir))
+            if self.cfg.DATA.TRAIN.GT_PATH != train_channel_mask_dir:
+                print("DATA.TRAIN.GT_PATH changed from {} to {}".format(self.cfg.DATA.TRAIN.GT_PATH, train_channel_mask_dir))
+            opts.extend(['DATA.TRAIN.PATH', train_channel_dir, 'DATA.TRAIN.GT_PATH', train_channel_mask_dir])
         if not self.cfg.DATA.VAL.FROM_TRAIN:
-            print("DATA.VAL.PATH changed from {} to {}".format(self.cfg.DATA.VAL.PATH, self.cfg.DATA.VAL.INSTANCE_CHANNELS_DIR))
-            print("DATA.VAL.GT_PATH changed from {} to {}".format(self.cfg.DATA.VAL.GT_PATH, self.cfg.DATA.VAL.INSTANCE_CHANNELS_MASK_DIR))
-            opts.extend(['DATA.VAL.PATH', self.cfg.DATA.VAL.INSTANCE_CHANNELS_DIR,
-                        'DATA.VAL.GT_PATH', self.cfg.DATA.VAL.INSTANCE_CHANNELS_MASK_DIR])
-        if self.cfg.TEST.ENABLE and not self.cfg.DATA.TEST.USE_VAL_AS_TEST and not self.cfg.TEST.BY_CHUNKS.ENABLE:
-            print("DATA.TEST.PATH changed from {} to {}".format(self.cfg.DATA.TEST.PATH, self.cfg.DATA.TEST.INSTANCE_CHANNELS_DIR))
-            opts.extend(['DATA.TEST.PATH', self.cfg.DATA.TEST.INSTANCE_CHANNELS_DIR])
+            if self.cfg.DATA.VAL.PATH != val_channel_dir:
+                print("DATA.VAL.PATH changed from {} to {}".format(self.cfg.DATA.VAL.PATH, val_channel_dir))
+            if self.cfg.DATA.VAL.GT_PATH != val_channel_mask_dir:
+                print("DATA.VAL.GT_PATH changed from {} to {}".format(self.cfg.DATA.VAL.GT_PATH, val_channel_mask_dir))
+            opts.extend(['DATA.VAL.PATH', val_channel_dir, 'DATA.VAL.GT_PATH', val_channel_mask_dir])
+        if self.cfg.TEST.ENABLE and not self.cfg.DATA.TEST.USE_VAL_AS_TEST:
+            if self.cfg.DATA.TEST.PATH != test_channel_dir:
+                print("DATA.TEST.PATH changed from {} to {}".format(self.cfg.DATA.TEST.PATH, test_channel_dir))
+                opts.extend(['DATA.TEST.PATH', test_channel_dir])
             if self.cfg.DATA.TEST.LOAD_GT:
-                print("DATA.TEST.GT_PATH changed from {} to {}".format(self.cfg.DATA.TEST.GT_PATH, self.cfg.DATA.TEST.INSTANCE_CHANNELS_MASK_DIR))
-                opts.extend(['DATA.TEST.GT_PATH', self.cfg.DATA.TEST.INSTANCE_CHANNELS_MASK_DIR])
+                if self.cfg.DATA.TEST.GT_PATH != test_channel_mask_dir:
+                    print("DATA.TEST.GT_PATH changed from {} to {}".format(self.cfg.DATA.TEST.GT_PATH, test_channel_mask_dir))
+                    opts.extend(['DATA.TEST.GT_PATH', test_channel_mask_dir])
         original_test_path = self.cfg.DATA.TEST.PATH
-        original_test_mask_path = self.cfg.DATA.TEST.GT_PATH
+        original_test_mask_path = test_instance_mask_dir
         self.cfg.merge_from_list(opts)
 
         return original_test_path, original_test_mask_path
 
     def torchvision_model_call(self, in_img, is_train=False):
         """
         Call a regular Pytorch model.
```

### Comparing `biapy-3.4.3/biapy/engine/metrics.py` & `biapy-3.4.4/biapy/engine/metrics.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/schedulers/warmup_cosine_decay.py` & `biapy-3.4.4/biapy/engine/schedulers/warmup_cosine_decay.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/self_supervised.py` & `biapy-3.4.4/biapy/engine/self_supervised.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/semantic_seg.py` & `biapy-3.4.4/biapy/engine/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/super_resolution.py` & `biapy-3.4.4/biapy/engine/super_resolution.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/engine/train_engine.py` & `biapy-3.4.4/biapy/engine/train_engine.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/__init__.py` & `biapy-3.4.4/biapy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/attention_unet.py` & `biapy-3.4.4/biapy/models/attention_unet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/blocks.py` & `biapy-3.4.4/biapy/models/blocks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/dfcan.py` & `biapy-3.4.4/biapy/models/dfcan.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/edsr.py` & `biapy-3.4.4/biapy/models/edsr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/efficientnet.py` & `biapy-3.4.4/biapy/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/mae.py` & `biapy-3.4.4/biapy/models/mae.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/multiresunet.py` & `biapy-3.4.4/biapy/models/multiresunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/rcan.py` & `biapy-3.4.4/biapy/models/rcan.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/resunet++.py` & `biapy-3.4.4/biapy/models/resunet++.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/resunet.py` & `biapy-3.4.4/biapy/models/resunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/seunet.py` & `biapy-3.4.4/biapy/models/seunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/simple_cnn.py` & `biapy-3.4.4/biapy/models/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/tr_layers.py` & `biapy-3.4.4/biapy/models/tr_layers.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/unet.py` & `biapy-3.4.4/biapy/models/unet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/unetr.py` & `biapy-3.4.4/biapy/models/unetr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/vit.py` & `biapy-3.4.4/biapy/models/vit.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/models/wdsr.py` & `biapy-3.4.4/biapy/models/wdsr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/callbacks.py` & `biapy-3.4.4/biapy/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/matching.py` & `biapy-3.4.4/biapy/utils/matching.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/misc.py` & `biapy-3.4.4/biapy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/calculate_detection_metrics.py` & `biapy-3.4.4/biapy/utils/scripts/calculate_detection_metrics.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/calculate_metrics_3D.py` & `biapy-3.4.4/biapy/utils/scripts/calculate_metrics_3D.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/create_probability_csv.py` & `biapy-3.4.4/biapy/utils/scripts/create_probability_csv.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/crop_2D_dataset.py` & `biapy-3.4.4/biapy/utils/scripts/crop_2D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/crop_3D_dataset.py` & `biapy-3.4.4/biapy/utils/scripts/crop_3D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/crop_and_discard_3D_dataset.py` & `biapy-3.4.4/biapy/utils/scripts/crop_and_discard_3D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/detection_plots.py` & `biapy-3.4.4/biapy/utils/scripts/detection_plots.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/detection_probs_to_points.py` & `biapy-3.4.4/biapy/utils/scripts/detection_probs_to_points.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/fill_holes_in_seg_masks.py` & `biapy-3.4.4/biapy/utils/scripts/fill_holes_in_seg_masks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/filter_close_points.py` & `biapy-3.4.4/biapy/utils/scripts/filter_close_points.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/from_class_csv_to_folders.py` & `biapy-3.4.4/biapy/utils/scripts/from_class_csv_to_folders.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/h5_to_tif.py` & `biapy-3.4.4/biapy/utils/scripts/h5_to_tif.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/h5_to_zarr.py` & `biapy-3.4.4/biapy/utils/scripts/h5_to_zarr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/lightmycell_data_preparation.py` & `biapy-3.4.4/biapy/utils/scripts/lightmycell_data_preparation.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/merge_dataset_channels.py` & `biapy-3.4.4/biapy/utils/scripts/merge_dataset_channels.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/order_axes.py` & `biapy-3.4.4/biapy/utils/scripts/order_axes.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.3/biapy/utils/scripts/run_checks.py` & `biapy-3.4.4/biapy/utils/scripts/run_checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,181 +10,17 @@
 from zipfile import ZipFile 
 from subprocess import Popen, PIPE
 from time import sleep
 import numpy as np
 
 gpu = "0"
 gpus = "0,1" # For those tests that use more than one 
-
 data_folder = "/data/dfranco/biapy_checks"
-results_folder = os.path.join(data_folder,  "output")
 biapy_folder = "/data/dfranco/BiaPy"
 
-###############
-# Semantic seg.
-###############
-semantic_folder = os.path.join(data_folder, "semantic_seg")
-
-# 2D
-semantic_2d_data_drive_link = "https://drive.google.com/uc?id=1DfUoVHf__xk-s4BWSKbkfKYMnES-9RJt"
-semantic_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/semantic_segmentation/2d_semantic_segmentation.yaml"
-semantic_2d_template_local = os.path.join(semantic_folder, "2d_semantic_segmentation.yaml")
-semantic_2d_data_filename = "fibsem_epfl_2D.zip"
-semantic_2d_data_outpath = os.path.join(semantic_folder, "fibsem_epfl_2D")
-# 3D
-semantic_3d_data_drive_link = "https://drive.google.com/uc?id=10Cf11PtERq4pDHCJroekxu_hf10EZzwG"
-semantic_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/semantic_segmentation/3d_semantic_segmentation.yaml"
-semantic_3d_template_local = os.path.join(semantic_folder, "3d_semantic_segmentation.yaml")
-semantic_3d_data_filename = "fibsem_epfl_3D.zip"
-semantic_3d_data_outpath = os.path.join(semantic_folder, "fibsem_epfl_3D")
-
-###############
-# Instance seg.
-###############
-inst_seg_folder = os.path.join(data_folder, "instance_seg")
-
-# 2D
-instance_seg_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/instance_segmentation/2d_instance_segmentation.yaml"
-instance_seg_2d_template_local = os.path.join(inst_seg_folder, "2d_instance_segmentation.yaml")
-instance_seg_2d_data_drive_link = "https://drive.google.com/uc?id=1b7_WDDGEEaEoIpO_1EefVr0w0VQaetmg"
-instance_seg_2d_data_filename = "Stardist_v2_2D.zip"
-instance_seg_2d_data_outpath = os.path.join(inst_seg_folder, "Stardist_v2_2D")
-# 3D
-instance_seg_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/instance_segmentation/3d_instance_segmentation.yaml"
-instance_seg_3d_template_local = os.path.join(inst_seg_folder, "3d_instance_segmentation.yaml")
-instance_seg_3d_data_drive_link = "https://drive.google.com/uc?id=1fdL35ZTNw5hhiKau1gadaGu-rc5ZU_C7"
-instance_seg_3d_data_filename = "demo3D_3D.zip"
-instance_seg_3d_data_outpath = os.path.join(inst_seg_folder, "demo3D_3D")
-
-instance_seg_cyst_data_zenodo_link = "https://zenodo.org/records/10973241/files/CartoCell.zip?download=1"
-instance_seg_cyst_data_filename = "CartoCell.zip"
-instance_seg_cyst_data_outpath = os.path.join(inst_seg_folder, "CartoCell")
-
-###########
-# Detection
-###########
-detection_folder = os.path.join(data_folder, "detection")
-
-# 2D
-detection_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/detection/2d_detection.yaml"
-detection_2d_template_local = os.path.join(detection_folder, "2d_detection.yaml")
-detection_2d_data_drive_link = "https://drive.google.com/uc?id=1pWqQhcWY15b5fVLZDkPS-vnE-RU6NlYf"
-detection_2d_data_filename = "Stardist_v2_detection.zip"
-detection_2d_data_outpath = os.path.join(detection_folder, "Stardist_v2_detection")
-# 3D
-detection_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/detection/3d_detection.yaml"
-detection_3d_template_local = os.path.join(detection_folder, "3d_detection.yaml")
-detection_3d_data_drive_link = "https://drive.google.com/uc?id=19P4AcvBPJXeW7QRj92Jh1keunGa5fi8d"
-detection_3d_data_filename = "NucMM-Z_training.zip"
-detection_3d_data_outpath = os.path.join(detection_folder, "NucMM-Z_training")
-
-detection_3d_brainglobe_data_drive_link = "https://drive.google.com/uc?id=1veBueUuYi_mWbSky_4mtzfKBpO00SvWR"
-detection_3d_brainglobe_data_filename = "brainglobe_small_data.zip"
-detection_3d_brainglobe_data_outpath = os.path.join(detection_folder, "brainglobe_small_data")
-
-###########
-# Denoising
-###########
-denoising_folder = os.path.join(data_folder, "denoising")
-
-# 2D
-denoising_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/denoising/2d_denoising.yaml"
-denoising_2d_template_local = os.path.join(denoising_folder, "2d_denoising.yaml")
-denoising_2d_data_drive_link = "https://drive.google.com/uc?id=1TFvOySOiIgVIv9p4pbHdEbai-d2YGDvV"
-denoising_2d_data_filename = "convallaria2D.zip"
-denoising_2d_data_outpath = os.path.join(denoising_folder, "convallaria2D")
-# 3D
-denoising_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/denoising/3d_denoising.yaml"
-denoising_3d_template_local = os.path.join(denoising_folder, "3d_denoising.yaml")
-denoising_3d_data_drive_link = "https://drive.google.com/uc?id=1OIjnUoJKdnbClBlpzk7V5R8wtoLont-r"
-denoising_3d_data_filename = "flywing3D.zip"
-denoising_3d_data_outpath = os.path.join(denoising_folder, "flywing3D")
-
-###########
-# SR
-###########
-super_resolution_folder = os.path.join(data_folder, "sr")
-
-# 2D
-super_resolution_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/super-resolution/2d_super-resolution.yaml"
-super_resolution_2d_template_local = os.path.join(super_resolution_folder, "2d_super_resolution.yaml")
-super_resolution_2d_data_drive_link = "https://drive.google.com/uc?id=1rtrR_jt8hcBEqvwx_amFBNR7CMP5NXLo"
-super_resolution_2d_data_filename = "sr_data_2D.zip"
-super_resolution_2d_data_outpath = os.path.join(super_resolution_folder, "sr_data_2D")
-# 3D
-super_resolution_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/super-resolution/3d_super-resolution.yaml"
-super_resolution_3d_template_local = os.path.join(super_resolution_folder, "3d_super_resolution.yaml")
-super_resolution_3d_data_drive_link = "https://drive.google.com/uc?id=1TfQVK7arJiRAVmKHRebsfi8NEas8ni4s"
-super_resolution_3d_data_filename = "sr_data_3D.zip"
-super_resolution_3d_data_outpath = os.path.join(super_resolution_folder, "sr_data_3D")
-
-###########
-# SSL
-###########
-self_supervision_folder = os.path.join(data_folder, "ssl")
-
-# 2D
-self_supervision_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/self-supervised/2d_self-supervised.yaml"
-self_supervision_2d_template_local = os.path.join(self_supervision_folder, "2d_self_supervision.yaml")
-self_supervision_2d_data_drive_link = semantic_2d_data_drive_link
-self_supervision_2d_data_filename = "fibsem_epfl_2D.zip"
-self_supervision_2d_data_outpath = os.path.join(self_supervision_folder, "fibsem_epfl_2D")
-# 3D
-self_supervision_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/self-supervised/3d_self-supervised.yaml"
-self_supervision_3d_template_local = os.path.join(self_supervision_folder, "3d_self_supervision.yaml")
-self_supervision_3d_data_drive_link = semantic_3d_data_drive_link
-self_supervision_3d_data_filename = "fibsem_epfl_3D.zip"
-self_supervision_3d_data_outpath = os.path.join(self_supervision_folder, "fibsem_epfl_3D")
-
-
-###########
-# Classification
-###########
-classification_folder = os.path.join(data_folder, "classification")
-
-# 2D
-classification_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/classification/2d_classification.yaml"
-classification_2d_template_local = os.path.join(classification_folder, "2d_classification.yaml")
-classification_2d_data_drive_link = "https://drive.google.com/uc?id=15_pnH4_tJcwhOhNqFsm26NQuJbNbFSIN"
-classification_2d_data_filename = "DermaMNIST_2D.zip"
-classification_2d_data_outpath = os.path.join(classification_folder, "DermaMNIST_2D")
-
-# 2D (natural images)
-classification_butterfly_2d_data_drive_link = "https://drive.google.com/uc?id=1m4_3UAgUsZ8FDjB4HyfA50Sht7_XkfdB"
-classification_butterfly_2d_data_filename = "butterfly_data.zip"
-classification_butterfly_2d_data_outpath = os.path.join(classification_folder, "butterfly_data")
-
-# 3D
-classification_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/classification/3d_classification.yaml"
-classification_3d_template_local = os.path.join(classification_folder, "3d_classification.yaml")
-classification_3d_data_drive_link = "https://drive.google.com/uc?id=1pypWJ4Z9sRLPlVHbG6zpwmS6COkm3wUg"
-classification_3d_data_filename = "DermaMNIST_3D.zip"
-classification_3d_data_outpath = os.path.join(classification_folder, "DermaMNIST_3D")
-
-
-###########
-# I2I
-###########
-image_to_image_folder = os.path.join(data_folder, "image_to_image")
-
-# 2D
-image_to_image_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/image-to-image/lightmycells/lightmycells_actin.yaml"
-image_to_image_2d_template_local = os.path.join(image_to_image_folder, "2d_image_to_image.yaml")
-image_to_image_2d_data_drive_link = "https://drive.google.com/uc?id=1L8AXNjh0_updVI3-v1duf6CbcZb8uZK7"
-image_to_image_2d_data_filename = "Dapi_dataset.zip"
-image_to_image_2d_data_outpath = os.path.join(image_to_image_folder, "Dapi_dataset")
-
-# 2D ligthmycells
-image_to_image_light_2d_data_drive_link = "https://drive.google.com/uc?id=1SU4u-bcM1ZaDzEYg-d8W3zP6Yq2o8eKV"
-image_to_image_light_2d_data_filename = "reduced_actin_lightmycells.zip"
-image_to_image_light_2d_data_outpath = os.path.join(classification_folder, "reduced_actin_lightmycells")
-
-if not os.path.exists(biapy_folder): 
-    raise ValueError(f"BiaPy not found in: {biapy_folder}")
-
 all_test_info = {}
 all_test_info["Test1"] = {
     "enable": False,
     "run_experiment": False,
     "jobname": "test1",
     "description": "2D Semantic seg. Lucchi++. Basic DA. Extract random crops (probability map). unet. 2D stack as 3D. Post-proc: z-filtering.",
     "yaml": "test_1.yaml",
@@ -197,15 +33,15 @@
 all_test_info["Test2"] = {
     "enable": False,
     "run_experiment": False,
     "jobname": "test2",
     "description": "3D Semantic seg. Lucchi++. attention_unet. Basic DA.",
     "yaml": "test_2.yaml",
     "internal_checks": [
-        {"pattern": "Test Foreground IoU (merge patches)", "gt": True, "value": 0.7},
+        {"pattern": "Test Foreground IoU (merge patches)", "gt": True, "value": 0.55},
     ]
 }
 
 all_test_info["Test3"] = {
     "enable": False,
     "run_experiment": False,
     "jobname": "test3",
@@ -433,26 +269,26 @@
     ]
 }
 
 all_test_info["Test22"] = {
     "enable": False,
     "run_experiment": False,
     "jobname": "test22",
-    "description": "3D classification. DermaMNIST 3D data. preprocess: resize, Cross-val. Basic DA. ViT",
+    "description": "3D classification. DermaMNIST 3D data. preprocess: resize, Cross-val. Basic DA. simple_cnn",
     "yaml": "test22.yaml",
     "internal_checks": [
         {"type": "regular", "pattern": "Validation top-5-accuracy:", "gt": True, "value": 0.7},
     ]
 }
 
 all_test_info["Test23"] = {
     "enable": False,
     "run_experiment": False,
     "jobname": "test23",
-    "description": "2D image to image. DermaMNIST 3D data. preprocess: resize, Cross-val. Basic DA. ViT",
+    "description": "3D classification. DermaMNIST 3D data. preprocess: resize. Basic DA. simple_cnn",
     "yaml": "test23.yaml",
     "internal_checks": [
         {"type": "regular", "pattern": "Validation top-5-accuracy:", "gt": True, "value": 0.7},
     ]
 }
 
 all_test_info["Test24"] = {
@@ -473,14 +309,229 @@
     "description": "2D image to image. lighmycells 2D data. preprocess: resize, Cross-val. Basic DA. ViT",
     "yaml": "test25.yaml",
     "internal_checks": [
         {"type": "regular", "pattern": "Validation PSNR:", "gt": True, "value": 22.0},
     ]
 }
 
+all_test_info["Test26"] = {
+    "enable": False,
+    "run_experiment": False,
+    "jobname": "test26",
+    "description": "3D Detection. Zarr 3D data (Brainglobe). in memory false. custom norm, percentile norm, per image. "
+        "MINIMUM_FOREGROUND_PER. warmupcosine. Basic DA. resunet. test by chunks: Zarr. Post-proc: remove close points",
+    "yaml": "test_26.yaml",
+    "internal_checks": [
+        {"type": "regular", "pattern": "Detection - Test F1 (per image)", "gt": True, "value": 0.15},
+    ]
+}
+
+all_test_info["Test27"] = {
+    "enable": False,
+    "run_experiment": False,
+    "jobname": "test27",
+    "description": "3D Instance seg. Zarr 3D data SNEMI. in memory false. input zarr multiple data raw: 'volumes.raw'"
+        "warmupcosine. inference, by chunks, zarr multiple data, workflow process: entire pred.",
+    "yaml": "test_27.yaml",
+    "internal_checks": [
+        {"type": "DatasetMatching", "pattern": "DatasetMatching(criterion='iou', thresh=0.3,", "nApparition": 1, "metric": "f1", 
+            "gt": True, "value": 0.3},
+    ]
+}
+
+all_test_info["Test28"] = {
+    "enable": True,
+    "run_experiment": True,
+    "jobname": "test28",
+    "description": "3D Image to image. Nuclear_Pore_complex_3D data. in memory true. val 0.1 of train.",
+    "yaml": "test_28.yaml",
+    "internal_checks": [
+        {"type": "regular", "pattern": "Validation PSNR:", "gt": True, "value": 20.0},
+    ]
+}
+
+################################################
+# NO-DEVS: DO NOT TOUCH BELOW THIS LINE 
+################################################
+
+results_folder = os.path.join(data_folder,  "output")
+
+###############
+# Semantic seg.
+###############
+semantic_folder = os.path.join(data_folder, "semantic_seg")
+
+# 2D
+semantic_2d_data_drive_link = "https://drive.google.com/uc?id=1DfUoVHf__xk-s4BWSKbkfKYMnES-9RJt"
+semantic_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/semantic_segmentation/2d_semantic_segmentation.yaml"
+semantic_2d_template_local = os.path.join(semantic_folder, "2d_semantic_segmentation.yaml")
+semantic_2d_data_filename = "fibsem_epfl_2D.zip"
+semantic_2d_data_outpath = os.path.join(semantic_folder, "fibsem_epfl_2D")
+# 3D
+semantic_3d_data_drive_link = "https://drive.google.com/uc?id=10Cf11PtERq4pDHCJroekxu_hf10EZzwG"
+semantic_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/semantic_segmentation/3d_semantic_segmentation.yaml"
+semantic_3d_template_local = os.path.join(semantic_folder, "3d_semantic_segmentation.yaml")
+semantic_3d_data_filename = "fibsem_epfl_3D.zip"
+semantic_3d_data_outpath = os.path.join(semantic_folder, "fibsem_epfl_3D")
+
+###############
+# Instance seg.
+###############
+inst_seg_folder = os.path.join(data_folder, "instance_seg")
+
+# 2D
+instance_seg_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/instance_segmentation/2d_instance_segmentation.yaml"
+instance_seg_2d_template_local = os.path.join(inst_seg_folder, "2d_instance_segmentation.yaml")
+instance_seg_2d_data_drive_link = "https://drive.google.com/uc?id=1b7_WDDGEEaEoIpO_1EefVr0w0VQaetmg"
+instance_seg_2d_data_filename = "Stardist_v2_2D.zip"
+instance_seg_2d_data_outpath = os.path.join(inst_seg_folder, "Stardist_v2_2D")
+# 3D
+instance_seg_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/instance_segmentation/3d_instance_segmentation.yaml"
+instance_seg_3d_template_local = os.path.join(inst_seg_folder, "3d_instance_segmentation.yaml")
+instance_seg_3d_data_drive_link = "https://drive.google.com/uc?id=1fdL35ZTNw5hhiKau1gadaGu-rc5ZU_C7"
+instance_seg_3d_data_filename = "demo3D_3D.zip"
+instance_seg_3d_data_outpath = os.path.join(inst_seg_folder, "demo3D_3D")
+
+instance_seg_cyst_data_zenodo_link = "https://zenodo.org/records/10973241/files/CartoCell.zip?download=1"
+instance_seg_cyst_data_filename = "CartoCell.zip"
+instance_seg_cyst_data_outpath = os.path.join(inst_seg_folder, "CartoCell")
+
+instance_seg_snemi_zarr_data_drive_link = "https://drive.google.com/uc?id=1Ralex5SvYUZbXoDkWoaCjb6d_iWuuOHp"
+instance_seg_snemi_zarr_data_filename = "snemi_zarr.zip"
+instance_seg_snemi_zarr_data_outpath = os.path.join(inst_seg_folder, "snemi_zarr")
+
+###########
+# Detection
+###########
+detection_folder = os.path.join(data_folder, "detection")
+
+# 2D
+detection_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/detection/2d_detection.yaml"
+detection_2d_template_local = os.path.join(detection_folder, "2d_detection.yaml")
+detection_2d_data_drive_link = "https://drive.google.com/uc?id=1pWqQhcWY15b5fVLZDkPS-vnE-RU6NlYf"
+detection_2d_data_filename = "Stardist_v2_detection.zip"
+detection_2d_data_outpath = os.path.join(detection_folder, "Stardist_v2_detection")
+# 3D
+detection_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/detection/3d_detection.yaml"
+detection_3d_template_local = os.path.join(detection_folder, "3d_detection.yaml")
+detection_3d_data_drive_link = "https://drive.google.com/uc?id=19P4AcvBPJXeW7QRj92Jh1keunGa5fi8d"
+detection_3d_data_filename = "NucMM-Z_training.zip"
+detection_3d_data_outpath = os.path.join(detection_folder, "NucMM-Z_training")
+
+detection_3d_brainglobe_data_drive_link = "https://drive.google.com/uc?id=1veBueUuYi_mWbSky_4mtzfKBpO00SvWR"
+detection_3d_brainglobe_data_filename = "brainglobe_small_data.zip"
+detection_3d_brainglobe_data_outpath = os.path.join(detection_folder, "brainglobe_small_data")
+
+###########
+# Denoising
+###########
+denoising_folder = os.path.join(data_folder, "denoising")
+
+# 2D
+denoising_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/denoising/2d_denoising.yaml"
+denoising_2d_template_local = os.path.join(denoising_folder, "2d_denoising.yaml")
+denoising_2d_data_drive_link = "https://drive.google.com/uc?id=1TFvOySOiIgVIv9p4pbHdEbai-d2YGDvV"
+denoising_2d_data_filename = "convallaria2D.zip"
+denoising_2d_data_outpath = os.path.join(denoising_folder, "convallaria2D")
+# 3D
+denoising_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/denoising/3d_denoising.yaml"
+denoising_3d_template_local = os.path.join(denoising_folder, "3d_denoising.yaml")
+denoising_3d_data_drive_link = "https://drive.google.com/uc?id=1OIjnUoJKdnbClBlpzk7V5R8wtoLont-r"
+denoising_3d_data_filename = "flywing3D.zip"
+denoising_3d_data_outpath = os.path.join(denoising_folder, "flywing3D")
+
+###########
+# SR
+###########
+super_resolution_folder = os.path.join(data_folder, "sr")
+
+# 2D
+super_resolution_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/super-resolution/2d_super-resolution.yaml"
+super_resolution_2d_template_local = os.path.join(super_resolution_folder, "2d_super_resolution.yaml")
+super_resolution_2d_data_drive_link = "https://drive.google.com/uc?id=1rtrR_jt8hcBEqvwx_amFBNR7CMP5NXLo"
+super_resolution_2d_data_filename = "sr_data_2D.zip"
+super_resolution_2d_data_outpath = os.path.join(super_resolution_folder, "sr_data_2D")
+# 3D
+super_resolution_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/super-resolution/3d_super-resolution.yaml"
+super_resolution_3d_template_local = os.path.join(super_resolution_folder, "3d_super_resolution.yaml")
+super_resolution_3d_data_drive_link = "https://drive.google.com/uc?id=1TfQVK7arJiRAVmKHRebsfi8NEas8ni4s"
+super_resolution_3d_data_filename = "sr_data_3D.zip"
+super_resolution_3d_data_outpath = os.path.join(super_resolution_folder, "sr_data_3D")
+
+###########
+# SSL
+###########
+self_supervision_folder = os.path.join(data_folder, "ssl")
+
+# 2D
+self_supervision_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/self-supervised/2d_self-supervised.yaml"
+self_supervision_2d_template_local = os.path.join(self_supervision_folder, "2d_self_supervision.yaml")
+self_supervision_2d_data_drive_link = semantic_2d_data_drive_link
+self_supervision_2d_data_filename = "fibsem_epfl_2D.zip"
+self_supervision_2d_data_outpath = os.path.join(self_supervision_folder, "fibsem_epfl_2D")
+# 3D
+self_supervision_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/self-supervised/3d_self-supervised.yaml"
+self_supervision_3d_template_local = os.path.join(self_supervision_folder, "3d_self_supervision.yaml")
+self_supervision_3d_data_drive_link = semantic_3d_data_drive_link
+self_supervision_3d_data_filename = "fibsem_epfl_3D.zip"
+self_supervision_3d_data_outpath = os.path.join(self_supervision_folder, "fibsem_epfl_3D")
+
+
+###########
+# Classification
+###########
+classification_folder = os.path.join(data_folder, "classification")
+
+# 2D
+classification_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/classification/2d_classification.yaml"
+classification_2d_template_local = os.path.join(classification_folder, "2d_classification.yaml")
+classification_2d_data_drive_link = "https://drive.google.com/uc?id=15_pnH4_tJcwhOhNqFsm26NQuJbNbFSIN"
+classification_2d_data_filename = "DermaMNIST_2D.zip"
+classification_2d_data_outpath = os.path.join(classification_folder, "DermaMNIST_2D")
+
+# 2D (natural images)
+classification_butterfly_2d_data_drive_link = "https://drive.google.com/uc?id=1m4_3UAgUsZ8FDjB4HyfA50Sht7_XkfdB"
+classification_butterfly_2d_data_filename = "butterfly_data.zip"
+classification_butterfly_2d_data_outpath = os.path.join(classification_folder, "butterfly_data")
+
+# 3D
+classification_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/classification/3d_classification.yaml"
+classification_3d_template_local = os.path.join(classification_folder, "3d_classification.yaml")
+classification_3d_data_drive_link = "https://drive.google.com/uc?id=1pypWJ4Z9sRLPlVHbG6zpwmS6COkm3wUg"
+classification_3d_data_filename = "DermaMNIST_3D.zip"
+classification_3d_data_outpath = os.path.join(classification_folder, "DermaMNIST_3D")
+
+
+###########
+# I2I
+###########
+image_to_image_folder = os.path.join(data_folder, "image_to_image")
+
+# 2D
+image_to_image_2d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/image-to-image/2d_image-to-image.yaml"
+image_to_image_2d_template_local = os.path.join(image_to_image_folder, "2d_image_to_image.yaml")
+image_to_image_2d_data_drive_link = "https://drive.google.com/uc?id=1L8AXNjh0_updVI3-v1duf6CbcZb8uZK7"
+image_to_image_2d_data_filename = "Dapi_dataset.zip"
+image_to_image_2d_data_outpath = os.path.join(image_to_image_folder, "Dapi_dataset")
+
+# 2D ligthmycells
+image_to_image_light_2d_data_drive_link = "https://drive.google.com/uc?id=1SU4u-bcM1ZaDzEYg-d8W3zP6Yq2o8eKV"
+image_to_image_light_2d_data_filename = "reduced_actin_lightmycells.zip"
+image_to_image_light_2d_data_outpath = os.path.join(image_to_image_folder, "reduced_actin_lightmycells")
+
+# 3D
+image_to_image_3d_template = "https://raw.githubusercontent.com/BiaPyX/BiaPy/master/templates/image-to-image/3d_image-to-image.yaml"
+image_to_image_3d_template_local = os.path.join(image_to_image_folder, "3d_image_to_image.yaml")
+image_to_image_3d_data_drive_link = "https://drive.google.com/uc?id=1jL0bn2X3OFaV5T-6KR1g6fPDllH-LWzm"
+image_to_image_3d_data_filename = "Nuclear_Pore_complex_3D.zip"
+image_to_image_3d_data_outpath = os.path.join(image_to_image_folder, "Nuclear_Pore_complex_3D")
+
+if not os.path.exists(biapy_folder): 
+    raise ValueError(f"BiaPy not found in: {biapy_folder}")
+
 ###################
 # Semantic seg.
 ###################
 
 # General things: 2D Data + YAML donwload
 if not os.path.exists(semantic_2d_data_outpath) and (all_test_info["Test1"]["enable"] or\
     all_test_info["Test3"]["enable"]):
@@ -557,14 +608,29 @@
     with ZipFile(os.path.join(inst_seg_folder, instance_seg_cyst_data_filename), 'r') as zObject: 
         zObject.extractall(path=inst_seg_folder) 
 
     if not os.path.exists(instance_seg_3d_template_local):
         print("Downloading instance seg. YAML . . .") 
         _, _ = urllib.request.urlretrieve(instance_seg_3d_template, filename=instance_seg_3d_template_local)
 
+# General things: SNEMI 3D Data + YAML donwload
+if not os.path.exists(instance_seg_snemi_zarr_data_outpath) and all_test_info["Test27"]["enable"]:
+    print("Downloading 3D snemi zarr data . . .")
+    
+    os.makedirs(inst_seg_folder, exist_ok=True)
+    os.chdir(inst_seg_folder)
+    gdown.download(instance_seg_snemi_zarr_data_drive_link, instance_seg_snemi_zarr_data_filename, quiet=True)
+
+    with ZipFile(os.path.join(inst_seg_folder, instance_seg_snemi_zarr_data_filename), 'r') as zObject: 
+        zObject.extractall(path=instance_seg_snemi_zarr_data_outpath) 
+
+    if not os.path.exists(instance_seg_3d_template_local):
+        print("Downloading instance seg. YAML . . .") 
+        _, _ = urllib.request.urlretrieve(instance_seg_3d_template, filename=instance_seg_3d_template_local)
+
 ###########
 # Detection
 ###########
 
 # General things: 2D Data + YAML donwload
 if not os.path.exists(detection_2d_data_outpath) and all_test_info["Test7"]["enable"]:
     print("Downloading 2D detection data . . .")
@@ -592,15 +658,16 @@
         zObject.extractall(path=detection_3d_data_outpath) 
 
     if not os.path.exists(detection_3d_template_local):
         print("Downloading detection YAML . . .") 
         _, _ = urllib.request.urlretrieve(detection_3d_template, filename=detection_3d_template_local)
 
 # General things: 3D Brainglobe Data + YAML donwload
-if not os.path.exists(detection_3d_brainglobe_data_outpath) and all_test_info["Test11"]["enable"]:
+if not os.path.exists(detection_3d_brainglobe_data_outpath) and (all_test_info["Test11"]["enable"] or\
+    all_test_info["Test26"]["enable"]):
     print("Downloading 3D Brainglobe detection data . . .")
     
     os.makedirs(detection_folder, exist_ok=True)
     os.chdir(detection_folder)
     gdown.download(detection_3d_brainglobe_data_drive_link, detection_3d_brainglobe_data_filename, quiet=True)
 
     with ZipFile(os.path.join(detection_folder, detection_3d_brainglobe_data_filename), 'r') as zObject: 
@@ -779,14 +846,29 @@
     with ZipFile(os.path.join(image_to_image_folder, image_to_image_light_2d_data_filename), 'r') as zObject: 
         zObject.extractall(path=image_to_image_light_2d_data_outpath) 
 
     if not os.path.exists(image_to_image_2d_template_local):
         print("Downloading image_to_image YAML . . .") 
         _, _ = urllib.request.urlretrieve(image_to_image_2d_template, filename=image_to_image_2d_template_local)
 
+# General things: 3D Data + YAML donwload
+if not os.path.exists(image_to_image_3d_data_outpath) and all_test_info["Test28"]["enable"]:
+    print("Downloading 3D image to image data . . .")
+    
+    os.makedirs(image_to_image_folder, exist_ok=True)
+    os.chdir(image_to_image_folder)
+    gdown.download(image_to_image_3d_data_drive_link, image_to_image_3d_data_filename, quiet=True)
+
+    with ZipFile(os.path.join(image_to_image_folder, image_to_image_3d_data_filename), 'r') as zObject: 
+        zObject.extractall(path=image_to_image_3d_data_outpath) 
+
+    if not os.path.exists(image_to_image_3d_template_local):
+        print("Downloading image to image YAML . . .") 
+        _, _ = urllib.request.urlretrieve(image_to_image_3d_template, filename=image_to_image_3d_template_local)
+
 
 def print_inventory(dct): 
     for item, amount in dct.items():  # dct.iteritems() in Python 2
         if not isinstance(amount, list):
             print("{}: {}".format(item, amount))
         else:
             print("{}:".format(item))
@@ -2579,20 +2661,16 @@
     biapy_config['DATA']['PREPROCESS']['RESIZE']['OUTPUT_SHAPE'] = "(56,56,56)"
 
     biapy_config['DATA']['PATCH_SIZE'] = "(56,56,56,1)"
     
     biapy_config['DATA']['TRAIN']['PATH'] = os.path.join(classification_3d_data_outpath, "data", "train")
     biapy_config['DATA']['TRAIN']['IN_MEMORY'] = True
     biapy_config['DATA']['VAL']['FROM_TRAIN'] = True
-    biapy_config['DATA']['VAL']['CROSS_VAL'] = True
-    biapy_config['DATA']['VAL']['CROSS_VAL_NFOLD'] = 5
-    biapy_config['DATA']['VAL']['CROSS_VAL_FOLD'] = 3
     biapy_config['DATA']['TEST']['PATH'] = os.path.join(classification_3d_data_outpath, "data", "test")
     biapy_config['DATA']['TEST']['IN_MEMORY'] = True
-    biapy_config['DATA']['TEST']['USE_VAL_AS_TEST'] = True
 
     biapy_config['TRAIN']['ENABLE'] = True
     biapy_config['TRAIN']['EPOCHS'] = 5
     biapy_config['TRAIN']['PATIENCE'] = -1 
     
     biapy_config['MODEL']['ARCHITECTURE'] = 'simple_cnn'
     biapy_config['MODEL']['LOAD_CHECKPOINT'] = False
@@ -2781,8 +2859,293 @@
         if not results[-1]:
             print("Internal check not passed: {} {} {}".format(checks["pattern"], checks["gt"], checks["value"]))
 
     # Test result  
     print_result(results, all_test_info["Test25"]["jobname"], int_checks)
 
 
+#~~~~~~~~~~~~
+# Test 26 
+#~~~~~~~~~~~~
+if all_test_info["Test26"]["enable"]:
+    print("######")
+    print("Running Test 26")
+    print_inventory(all_test_info["Test26"])
+
+    #*******************
+    # File preparation 
+    #*******************
+    # Open config file
+    with open(detection_3d_template_local, 'r') as stream:
+        try:
+            biapy_config = yaml.safe_load(stream)
+        except yaml.YAMLError as exc:
+            raise ValueError(exc)
+
+    biapy_config['PROBLEM']['DETECTION'] = {}
+    biapy_config['PROBLEM']['DETECTION']['CENTRAL_POINT_DILATION'] = 2
+    biapy_config['PROBLEM']['DETECTION']['CHECK_POINTS_CREATED'] = False
+
+    biapy_config['DATA']['PATCH_SIZE'] = "(20, 128, 128, 2)"
+    biapy_config['DATA']['NORMALIZATION'] = {}
+    biapy_config['DATA']['NORMALIZATION']['PERC_CLIP'] = True
+    biapy_config['DATA']['NORMALIZATION']['PERC_LOWER'] = 0.1
+    biapy_config['DATA']['NORMALIZATION']['PERC_UPPER'] = 99.8
+    biapy_config['DATA']['NORMALIZATION']['APPLICATION_MODE'] = 'image'
+
+    biapy_config['DATA']['TRAIN']['INPUT_IMG_AXES_ORDER'] = 'ZYXC'
+    biapy_config['DATA']['TRAIN']['INPUT_MASK_AXES_ORDER'] = 'TZCYX'
+    biapy_config['DATA']['TRAIN']['MINIMUM_FOREGROUND_PER'] = 0.0000000000000000000001
+    biapy_config['DATA']['TRAIN']['PATH'] = os.path.join(detection_3d_brainglobe_data_outpath, "data", "3D_ch2ch4_Zarr")
+    biapy_config['DATA']['TRAIN']['GT_PATH'] = os.path.join(detection_3d_brainglobe_data_outpath, "data", "y")
+    biapy_config['DATA']['TRAIN']['IN_MEMORY'] = False
+    biapy_config['DATA']['VAL']['FROM_TRAIN'] = False
+    biapy_config['DATA']['VAL']['PATH'] = os.path.join(detection_3d_brainglobe_data_outpath, "data", "3D_ch2ch4_Zarr")
+    biapy_config['DATA']['VAL']['GT_PATH'] = os.path.join(detection_3d_brainglobe_data_outpath, "data", "y")
+    biapy_config['DATA']['VAL']['IN_MEMORY'] = False
+    biapy_config['DATA']['VAL']['INPUT_IMG_AXES_ORDER'] = 'ZYXC'
+    biapy_config['DATA']['VAL']['INPUT_MASK_AXES_ORDER'] = 'TZCYX'
+    biapy_config['DATA']['TEST']['PATH'] = os.path.join(detection_3d_brainglobe_data_outpath, "data", "3D_ch2ch4_Zarr")
+    biapy_config['DATA']['TEST']['GT_PATH'] = os.path.join(detection_3d_brainglobe_data_outpath, "data", "y")
+    biapy_config['DATA']['TEST']['IN_MEMORY'] = False
+    biapy_config['DATA']['TEST']['LOAD_GT'] = True
+    biapy_config['DATA']['TEST']['PADDING'] = "(0,18,18)"
+
+    biapy_config['TRAIN']['ENABLE'] = True
+    biapy_config['TRAIN']['EPOCHS'] = 100
+    biapy_config['TRAIN']['BATCH_SIZE'] = 1
+    biapy_config['TRAIN']['PATIENCE'] = 20 
+    biapy_config['TRAIN']['LR_SCHEDULER'] = {} 
+    biapy_config['TRAIN']['LR_SCHEDULER']['NAME'] = 'warmupcosine'  
+    biapy_config['TRAIN']['LR_SCHEDULER']['MIN_LR'] = 5.E-6  
+    biapy_config['TRAIN']['LR_SCHEDULER']['WARMUP_COSINE_DECAY_EPOCHS'] = 15
+
+    biapy_config['MODEL']['ARCHITECTURE'] = 'resunet'
+    biapy_config['MODEL']['Z_DOWN'] = [1,1,1,1]
+    del biapy_config['MODEL']['FEATURE_MAPS']
+    biapy_config['MODEL']['LOAD_CHECKPOINT'] = False
+
+    biapy_config['AUGMENTOR']['RANDOM_ROT'] = True
+    biapy_config['AUGMENTOR']['AFFINE_MODE'] = 'reflect'
+    biapy_config['AUGMENTOR']['ZFLIP'] = True
+
+    biapy_config['TEST']['ENABLE'] = True
+    biapy_config['TEST']['FULL_IMG'] = False
+    biapy_config['TEST']['DET_MIN_TH_TO_BE_PEAK'] = [0.2]
+    biapy_config['TEST']['DET_TOLERANCE'] = [8]
+    biapy_config['TEST']['VERBOSE'] = True
+
+    biapy_config['TEST']['BY_CHUNKS'] = {}
+    biapy_config['TEST']['BY_CHUNKS']['ENABLE'] = True
+    biapy_config['TEST']['BY_CHUNKS']['FORMAT'] = "Zarr"
+    biapy_config['TEST']['BY_CHUNKS']['SAVE_OUT_TIF'] = True
+    biapy_config['TEST']['BY_CHUNKS']['INPUT_IMG_AXES_ORDER'] = 'ZYXC'
+    biapy_config['TEST']['BY_CHUNKS']['WORKFLOW_PROCESS'] = {}
+    biapy_config['TEST']['BY_CHUNKS']['WORKFLOW_PROCESS']['ENABLE'] = True
+    biapy_config['TEST']['BY_CHUNKS']['WORKFLOW_PROCESS']['TYPE'] = "chunk_by_chunk" 
+
+    biapy_config['TEST']['POST_PROCESSING'] = {}
+    biapy_config['TEST']['POST_PROCESSING']['REMOVE_CLOSE_POINTS'] = True
+    biapy_config['TEST']['POST_PROCESSING']['REMOVE_CLOSE_POINTS_RADIUS'] = [3]
+
+    # Save file
+    test_file = os.path.join(detection_folder, all_test_info["Test26"]["yaml"])
+    with open(test_file, 'w') as outfile:
+        yaml.dump(biapy_config, outfile, default_flow_style=False)
+
+    # Run  
+    if all_test_info["Test26"]["run_experiment"]:
+        runjob(all_test_info["Test26"], results_folder, test_file, biapy_folder, multigpu=True)
+
+    # Check  
+    results = []
+    res, last_lines = check_finished(all_test_info["Test26"], "Test 26")
+    if not res:
+        print("Internal check not passed: seems that it didn't finish")
+    results.append(res)
+    int_checks = 1
+    for checks in all_test_info["Test26"]["internal_checks"]: 
+        if checks["type"] == "regular":
+            results.append(check_value(last_lines, checks["pattern"], checks["value"], checks["gt"]))
+        else:
+            results.append(check_DatasetMatching(last_lines, checks["pattern"], checks["value"], gt=checks["gt"], 
+                value_to_check=checks["nApparition"], metric=checks["metric"]))
+        int_checks += 1
+        if not results[-1]:
+            print("Internal check not passed: {} {} {}".format(checks["pattern"], checks["gt"], checks["value"]))
+
+    # Test result  
+    print_result(results, all_test_info["Test26"]["jobname"], int_checks)
+
+
+#~~~~~~~~~~~~
+# Test 27 
+#~~~~~~~~~~~~
+if all_test_info["Test27"]["enable"]:
+    print("######")
+    print("Running Test 27")
+    print_inventory(all_test_info["Test27"])
+
+    #*******************
+    # File preparation 
+    #*******************
+    # Open config file
+    with open(instance_seg_3d_template_local, 'r') as stream:
+        try:
+            biapy_config = yaml.safe_load(stream)
+        except yaml.YAMLError as exc:
+            raise ValueError(exc)
+
+    biapy_config['PROBLEM']['INSTANCE_SEG']['DATA_CHANNELS'] = 'BC'
+    biapy_config['PROBLEM']['INSTANCE_SEG']['DATA_MW_TH_TYPE'] = "manual"
+    biapy_config['PROBLEM']['INSTANCE_SEG']['DATA_MW_TH_BINARY_MASK'] = 0.9
+    biapy_config['PROBLEM']['INSTANCE_SEG']['DATA_MW_TH_CONTOUR'] = 0.1
+    biapy_config['PROBLEM']['INSTANCE_SEG']['DATA_MW_TH_CONTOUR'] = 0.1
+    biapy_config['PROBLEM']['INSTANCE_SEG']['DATA_REMOVE_SMALL_OBJ_BEFORE'] = 20
+    biapy_config['PROBLEM']['INSTANCE_SEG']['DATA_REMOVE_BEFORE_MW'] = True
+    biapy_config['PROBLEM']['INSTANCE_SEG']['DATA_CHANNEL_WEIGHTS'] = "(0.3, 1)"
+
+    biapy_config['DATA']['PATCH_SIZE'] = "(20, 256, 256, 1)"
+    biapy_config['DATA']['TRAIN']['PATH'] = os.path.join(instance_seg_snemi_zarr_data_outpath, "data", "train", "zarr")
+    biapy_config['DATA']['TRAIN']['IN_MEMORY'] = False
+    biapy_config['DATA']['TRAIN']['INPUT_IMG_AXES_ORDER'] = 'ZYX'
+    biapy_config['DATA']['TRAIN']['INPUT_MASK_AXES_ORDER'] = 'ZYX'
+    biapy_config['DATA']['TRAIN']['INPUT_ZARR_MULTIPLE_DATA'] = True
+    biapy_config['DATA']['TRAIN']['INPUT_ZARR_MULTIPLE_DATA_RAW_PATH'] = 'volumes.raw'
+    biapy_config['DATA']['TRAIN']['INPUT_ZARR_MULTIPLE_DATA_GT_PATH'] = 'volumes.labels.neuron_ids'
+    biapy_config['DATA']['VAL']['FROM_TRAIN'] = True
+    biapy_config['DATA']['VAL']['IN_MEMORY'] = False
+    biapy_config['DATA']['VAL']['SPLIT_TRAIN'] = 0.1
+    biapy_config['DATA']['TEST']['PATH'] = os.path.join(instance_seg_snemi_zarr_data_outpath, "data", "train", "zarr")
+    biapy_config['DATA']['TEST']['IN_MEMORY'] = False
+    biapy_config['DATA']['TEST']['LOAD_GT'] = True
+
+    biapy_config['TRAIN']['ENABLE'] = True
+    biapy_config['TRAIN']['EPOCHS'] = 80
+    biapy_config['TRAIN']['PATIENCE'] = -1 
+    biapy_config['TRAIN']['OPTIMIZER'] = "ADAMW" 
+    biapy_config['TRAIN']['LR'] = 1.E-4 
+    biapy_config['TRAIN']['LR_SCHEDULER'] = {} 
+    biapy_config['TRAIN']['LR_SCHEDULER']['NAME'] = 'warmupcosine'  
+    biapy_config['TRAIN']['LR_SCHEDULER']['MIN_LR'] = 5.E-6  
+    biapy_config['TRAIN']['LR_SCHEDULER']['WARMUP_COSINE_DECAY_EPOCHS'] = 15
+
+    biapy_config['MODEL']['ARCHITECTURE'] = 'resunet'
+    biapy_config['AUGMENTOR']['BRIGHTNESS'] = True
+    biapy_config['AUGMENTOR']['CONTRAST'] = True
+    biapy_config['AUGMENTOR']['MISALIGNMENT'] = True
+    biapy_config['AUGMENTOR']['MISSING_SECTIONS'] = True
+    biapy_config['AUGMENTOR']['ELASTIC'] = True
+
+    biapy_config['TEST']['ENABLE'] = True
+    biapy_config['TEST']['BY_CHUNKS'] = {}
+    biapy_config['TEST']['BY_CHUNKS']['ENABLE'] = True
+    biapy_config['TEST']['BY_CHUNKS']['FORMAT'] = "Zarr"
+    biapy_config['TEST']['BY_CHUNKS']['SAVE_OUT_TIF'] = False
+    biapy_config['TEST']['BY_CHUNKS']['INPUT_IMG_AXES_ORDER'] = 'ZYX'
+    biapy_config['TEST']['BY_CHUNKS']['INPUT_ZARR_MULTIPLE_DATA'] = True
+    biapy_config['TEST']['BY_CHUNKS']['INPUT_ZARR_MULTIPLE_DATA_RAW_PATH'] = 'volumes.raw'
+    biapy_config['TEST']['BY_CHUNKS']['INPUT_ZARR_MULTIPLE_DATA_GT_PATH'] = 'volumes.labels.neuron_ids'
+    biapy_config['TEST']['BY_CHUNKS']['WORKFLOW_PROCESS'] = {}
+    biapy_config['TEST']['BY_CHUNKS']['WORKFLOW_PROCESS']['ENABLE'] = True
+    biapy_config['TEST']['BY_CHUNKS']['WORKFLOW_PROCESS']['TYPE'] = "entire_pred" 
+
+    # Save file
+    test_file = os.path.join(inst_seg_folder, all_test_info["Test27"]["yaml"])
+    with open(test_file, 'w') as outfile:
+        yaml.dump(biapy_config, outfile, default_flow_style=False)
+
+    # Run  
+    if all_test_info["Test27"]["run_experiment"]:
+        runjob(all_test_info["Test27"], results_folder, test_file, biapy_folder)
+
+    # Check  
+    results = []
+    res, last_lines = check_finished(all_test_info["Test27"], "Test 27")
+    if not res:
+        print("Internal check not passed: seems that it didn't finish")
+    results.append(res)
+    int_checks = 1
+    for checks in all_test_info["Test27"]["internal_checks"]: 
+        if checks["type"] == "regular":
+            results.append(check_value(last_lines, checks["pattern"], checks["value"], checks["gt"]))
+        else:
+            results.append(check_DatasetMatching(last_lines, checks["pattern"], checks["value"], gt=checks["gt"], 
+                value_to_check=checks["nApparition"], metric=checks["metric"]))
+        int_checks += 1
+        if not results[-1]:
+            print("Internal check not passed: {} {} {}".format(checks["pattern"], checks["gt"], checks["value"]))
+
+    # Test result  
+    print_result(results, all_test_info["Test27"]["jobname"], int_checks)
+
+
+#~~~~~~~~~~~~
+# Test 28
+#~~~~~~~~~~~~
+if all_test_info["Test28"]["enable"]:
+    print("######")
+    print("Running Test 28")
+    print_inventory(all_test_info["Test28"])
+
+    #*******************
+    # File preparation 
+    #*******************
+    # Open config file
+    with open(image_to_image_3d_template_local, 'r') as stream:
+        try:
+            biapy_config = yaml.safe_load(stream)
+        except yaml.YAMLError as exc:
+            raise ValueError(exc)
+
+    biapy_config['DATA']['PATCH_SIZE'] = "(6,128,128,1)"
+    biapy_config['DATA']['TRAIN']['PATH'] = os.path.join(image_to_image_3d_data_outpath, "data", "train", "x")
+    biapy_config['DATA']['TRAIN']['GT_PATH'] = os.path.join(image_to_image_3d_data_outpath, "data", "train", "y")
+    biapy_config['DATA']['TRAIN']['IN_MEMORY'] = True
+    biapy_config['DATA']['VAL']['FROM_TRAIN'] = True
+    biapy_config['DATA']['VAL']['SPLIT_TRAIN'] = 0.1
+    biapy_config['DATA']['TEST']['PATH'] = os.path.join(image_to_image_3d_data_outpath, "data", "test", "x")
+    biapy_config['DATA']['TEST']['GT_PATH'] = os.path.join(image_to_image_3d_data_outpath, "data", "test", "y")
+    biapy_config['DATA']['TEST']['IN_MEMORY'] = False
+    biapy_config['DATA']['TEST']['PADDING'] = "(0,24,24)"
+ 
+    biapy_config['TRAIN']['ENABLE'] = True
+    biapy_config['TRAIN']['EPOCHS'] = 15
+    biapy_config['TRAIN']['PATIENCE'] = -1 
+
+    biapy_config['MODEL']['ARCHITECTURE'] = 'resunet'
+    biapy_config['MODEL']['Z_DOWN'] = [1,1,1,1]
+    biapy_config['MODEL']['LOAD_CHECKPOINT'] = False
+
+    biapy_config['TEST']['ENABLE'] = True
+
+    # Save file
+    test_file = os.path.join(image_to_image_folder, all_test_info["Test28"]["yaml"])
+    with open(test_file, 'w') as outfile:
+        yaml.dump(biapy_config, outfile, default_flow_style=False)
+
+    # Run  
+    if all_test_info["Test28"]["run_experiment"]:
+        runjob(all_test_info["Test28"], results_folder, test_file, biapy_folder)
+
+    # Check  
+    results = []
+    res, last_lines = check_finished(all_test_info["Test28"], "Test 28")
+    if not res:
+        print("Internal check not passed: seems that it didn't finish")
+    results.append(res)
+    int_checks = 1
+    for checks in all_test_info["Test28"]["internal_checks"]: 
+        if checks["type"] == "regular":
+            results.append(check_value(last_lines, checks["pattern"], checks["value"], checks["gt"]))
+        else:
+            results.append(check_DatasetMatching(last_lines, checks["pattern"], checks["value"], gt=checks["gt"], 
+                value_to_check=checks["nApparition"], metric=checks["metric"]))
+        int_checks += 1
+        if not results[-1]:
+            print("Internal check not passed: {} {} {}".format(checks["pattern"], checks["gt"], checks["value"]))
+
+    # Test result  
+    print_result(results, all_test_info["Test28"]["jobname"], int_checks)
+
+
 print("Finish tests!!")
```

### Comparing `biapy-3.4.3/biapy/utils/scripts/tif_to_h5.py` & `biapy-3.4.4/biapy/utils/scripts/tif_to_h5.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tqdm import tqdm
 from skimage import measure, feature
 from scipy import ndimage
 from PIL import ImageEnhance, Image
 from os import path
 
 img_shape = (4096, 4096)
-nput_dir = "/home/user/input"
+input_dir = "/home/user/input"
 output_dir = "/home/user/output"
 h5_filename = '0_human_instance_seg_pred.h5'
 #h5_filename = '1_rat_instance_seg_pred.h5'
 
 input_ids = sorted(next(os.walk(input_dir))[2])
 h5file_name = os.path.join(output_dir, h5_filename)
 os.makedirs(output_dir, exist_ok=True)
```

### Comparing `biapy-3.4.3/biapy/utils/util.py` & `biapy-3.4.4/biapy/utils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1481,14 +1481,47 @@
             else: 
                 data = fid
         else:
             raise ValueError(f"File extension {filename} not recognized")
 
         return fid, data
 
+def read_chunked_nested_data(zarrfile, data_path=""):
+    """
+    Find recursively raw and ground truth data within a Zarr file.
+    """
+    if not zarrfile.endswith('.zarr'):
+        raise ValueError("Not implemented for other filetypes than Zarr")
+    fid = zarr.open(zarrfile,'r')
+
+    def find_obj(path, fid):
+        obj = None
+        rpath = path.split('.')
+        if len(rpath) == 0: 
+            return None
+        else:
+            if len(rpath) > 1:
+                groups = list(fid.group_keys())
+                if rpath[0] not in groups:
+                    return None
+                obj = find_obj('.'.join(rpath[1:]), fid[rpath[0]])
+            else:
+                arrays = list(fid.array_keys())
+                if rpath[0] not in arrays:
+                    return None
+                return fid[rpath[0]]
+        return obj
+
+    data = find_obj(data_path, fid)
+
+    if data is None:
+        raise ValueError(f"No data found within the Zarr file in the path: '{data_path}'.")
+
+    return fid, data
+
 def write_chunked_data(data, data_dir, filename, dtype_str="float32", verbose=True):
     """
     Save images in the given directory.
 
     Parameters
     ----------
     data : 5D numpy array
```

### Comparing `biapy-3.4.3/biapy.egg-info/PKG-INFO` & `biapy-3.4.4/biapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biapy
-Version: 3.4.3
+Version: 3.4.4
 Summary: BiaPy: Bioimage analysis pipelines in Python
 Author-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 Maintainer-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 License: MIT License
         
         Copyright (c) 2022 Daniel Franco-Barranco
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biapy Version: 3.4.3 Summary: BiaPy: Bioimage
+Metadata-Version: 2.1 Name: biapy Version: 3.4.4 Summary: BiaPy: Bioimage
 analysis pipelines in Python Author-email: Daniel Franco-Barranco
 dipc.org> Maintainer-email: Daniel Franco-Barranco
 dipc.org> License: MIT License Copyright (c) 2022 Daniel Franco-Barranco
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `biapy-3.4.3/biapy.egg-info/SOURCES.txt` & `biapy-3.4.4/biapy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -77,8 +77,9 @@
 biapy/utils/scripts/from_class_csv_to_folders.py
 biapy/utils/scripts/h5_to_tif.py
 biapy/utils/scripts/h5_to_zarr.py
 biapy/utils/scripts/lightmycell_data_preparation.py
 biapy/utils/scripts/merge_dataset_channels.py
 biapy/utils/scripts/order_axes.py
 biapy/utils/scripts/run_checks.py
-biapy/utils/scripts/tif_to_h5.py
+biapy/utils/scripts/tif_to_h5.py
+biapy/utils/scripts/tif_to_zarr.py
```

### Comparing `biapy-3.4.3/pyproject.toml` & `biapy-3.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biapy"
-version = "3.4.3"
+version = "3.4.4"
 description = "BiaPy: Bioimage analysis pipelines in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{ name = "Daniel Franco-Barranco", email = "daniel.franco@dipc.org" }]
 maintainers = [{ name = "Daniel Franco-Barranco", email = "daniel.franco@dipc.org" }]
 license = { file = "LICENSE.md" }
 classifiers = [
```


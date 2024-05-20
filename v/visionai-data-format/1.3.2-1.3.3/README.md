# Comparing `tmp/visionai_data_format-1.3.2.tar.gz` & `tmp/visionai_data_format-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai_data_format-1.3.2.tar", last modified: Tue Apr 16 08:41:44 2024, max compression
+gzip compressed data, was "visionai_data_format-1.3.3.tar", last modified: Mon May 20 06:25:36 2024, max compression
```

## Comparing `visionai_data_format-1.3.2.tar` & `visionai_data_format-1.3.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.305475 visionai_data_format-1.3.2/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    23694 2024-04-16 08:41:44.305170 visionai_data_format-1.3.2/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    23316 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/README.md
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-04-16 08:41:44.305540 visionai_data_format-1.3.2/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      753 2024-04-16 08:33:06.000000 visionai_data_format-1.3.2/setup.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.295613 visionai_data_format-1.3.2/tests/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2176 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/tests/test_schemas.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     8449 2024-02-06 03:21:26.000000 visionai_data_format-1.3.2/tests/test_validators.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.296661 visionai_data_format-1.3.2/visionai_data_format/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     6751 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/convert_dataset.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.299739 visionai_data_format-1.3.2/visionai_data_format/converters/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      173 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/converters/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1729 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/converters/base.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    16423 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/converters/bdd_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     9363 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/converters/coco_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    16685 2024-03-19 08:30:06.000000 visionai_data_format-1.3.2/visionai_data_format/converters/kitti_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     9675 2024-03-19 09:51:26.000000 visionai_data_format-1.3.2/visionai_data_format/converters/vai_to_coco.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.300718 visionai_data_format-1.3.2/visionai_data_format/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      156 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1405 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/exceptions/constants.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5564 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/exceptions/error_messages.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1322 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/exceptions/visionai.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.301902 visionai_data_format-1.3.2/visionai_data_format/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2586 2024-04-16 07:37:46.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      679 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1727 2024-02-06 03:21:26.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/common.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      994 2024-04-16 08:33:06.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.302461 visionai_data_format-1.3.2/visionai_data_format/schemas/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    50408 2024-04-16 07:40:00.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    32093 2024-04-16 08:33:06.000000 visionai_data_format-1.3.2/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.304303 visionai_data_format-1.3.2/visionai_data_format/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1692 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/calculation.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10506 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/checker.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      761 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/classes.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      585 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/common.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4571 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/converter.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4059 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/resize.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4588 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/utils/validator.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2308 2023-12-21 03:02:35.000000 visionai_data_format-1.3.2/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5917 2023-07-06 06:50:32.000000 visionai_data_format-1.3.2/visionai_data_format/vai_to_bdd_v2.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-04-16 08:41:44.304560 visionai_data_format-1.3.2/visionai_data_format.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    23694 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1548 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       45 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       21 2024-04-16 08:41:44.000000 visionai_data_format-1.3.2/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.727065 visionai_data_format-1.3.3/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    25808 2024-05-20 06:25:36.726787 visionai_data_format-1.3.3/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    25408 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/README.md
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-05-20 06:25:36.727112 visionai_data_format-1.3.3/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      763 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.717931 visionai_data_format-1.3.3/tests/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2176 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/tests/test_schemas.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     8449 2024-02-06 03:21:26.000000 visionai_data_format-1.3.3/tests/test_validators.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.718830 visionai_data_format-1.3.3/visionai_data_format/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     7698 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/visionai_data_format/convert_dataset.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.721424 visionai_data_format-1.3.3/visionai_data_format/converters/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      206 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/visionai_data_format/converters/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1729 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/converters/base.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    16423 2024-03-19 09:51:26.000000 visionai_data_format-1.3.3/visionai_data_format/converters/bdd_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     9405 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/visionai_data_format/converters/coco_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    16685 2024-03-19 08:30:06.000000 visionai_data_format-1.3.3/visionai_data_format/converters/kitti_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     9965 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/visionai_data_format/converters/vai_to_coco.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10099 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/visionai_data_format/converters/yolo_to_vai.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.722430 visionai_data_format-1.3.3/visionai_data_format/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      156 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1405 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/exceptions/constants.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5564 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/exceptions/error_messages.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1322 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/exceptions/visionai.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.723630 visionai_data_format-1.3.3/visionai_data_format/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2586 2024-04-16 07:37:46.000000 visionai_data_format-1.3.3/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      679 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1745 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/visionai_data_format/schemas/common.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      994 2024-04-16 08:33:06.000000 visionai_data_format-1.3.3/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.724283 visionai_data_format-1.3.3/visionai_data_format/schemas/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    50408 2024-04-16 07:40:00.000000 visionai_data_format-1.3.3/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    32093 2024-04-16 08:33:06.000000 visionai_data_format-1.3.3/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.726052 visionai_data_format-1.3.3/visionai_data_format/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1692 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10506 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/utils/checker.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      761 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/utils/classes.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      593 2024-05-20 06:25:16.000000 visionai_data_format-1.3.3/visionai_data_format/utils/common.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4571 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/utils/converter.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4059 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/utils/resize.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4588 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/utils/validator.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2308 2023-12-21 03:02:35.000000 visionai_data_format-1.3.3/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5917 2023-07-06 06:50:32.000000 visionai_data_format-1.3.3/visionai_data_format/vai_to_bdd_v2.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-20 06:25:36.726289 visionai_data_format-1.3.3/visionai_data_format.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    25808 2024-05-20 06:25:36.000000 visionai_data_format-1.3.3/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1595 2024-05-20 06:25:36.000000 visionai_data_format-1.3.3/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-05-20 06:25:36.000000 visionai_data_format-1.3.3/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       52 2024-05-20 06:25:36.000000 visionai_data_format-1.3.3/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       21 2024-05-20 06:25:36.000000 visionai_data_format-1.3.3/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai_data_format-1.3.2/PKG-INFO` & `visionai_data_format-1.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: visionai-data-format
-Version: 1.3.2
-Summary: converter tool for visionai format
-Home-page: 
-Author: LinkerVision
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-Requires-Dist: pydantic==1.*
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: mock; extra == "test"
-Requires-Dist: pre-commit; extra == "test"
-
 # visionai-data-format
 
 `VisionAI` format is [Dataverse](https://www.linkervision.com/visionai-platform-dataverse) standardized annotation format to label objects and sequences in the context of Autonomous Driving System(ADS). `VisionAI` provides consistent and effective driving environment description and categorization in the real-world case.
 
 This tool provides validator of `VisionAI` format schema. Currently, the library supports:
   - Validate created `VisionAI` data format
   - Validate `VisionAI` data attributes with given `Ontology` information.
@@ -579,21 +565,21 @@
 - `--copy_sensor_data` : enable to copy image/lidar data
 
 
 ### Convert `COCO` format data to `VisionAI` format
 
 ```
 python3 visionai_data_format/convert_dataset.py -input_format coco -output_format vision_ai -image_annotation_type 2d_bounding_box -input_annotation_path ./coco_instance.json -source_data_root ./coco_images/ -output_dest_folder ~/visionai_output_dir -uri_root http://storage_test -n_frame 5 -sequence_idx_start 0 -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg --copy_sensor_data
-
 ```
 
 Arguments :
 - `-input_format`  : input format (use coco for COCO format)
 - `-output_format`  : output format (vision_ai)
 - `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
+- `-input_annotation_path` : input annotation path for coco-label.json file
 - `-source_data_root`  : image data folder
 - `-output_dest_folder` : output root folder (VisionAI local root folder)
 - `-uri_root` : uri root for target upload VisionAI storage i.e: https://azuresorate/vai_dataset
 - `-n_frame`  : number of frame to be converted (-1 means all), by default -1
 - `-sequence_idx_start `  : sequence start id, by default 0
 - `-camera_sensor_name`  : camera sensor name (default: "", specified it if need to convert camera data)
 - `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
@@ -601,29 +587,69 @@
 - `--copy_sensor_data` : enable to copy image data
 
 
 ### Convert `VisionAI` format data to `COCO` format
 
 ```
 python3 visionai_data_format/convert_dataset.py -input_format vision_ai -output_format coco -image_annotation_type 2d_bounding_box -source_data_root ./visionai_data_root -output_dest_folder ~/coco_output_dir -uri_root http://storage_test -n_frame 5 -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg --copy_sensor_data
-
 ```
 Arguments :
 - `-input_format`  : input format (vision_ai)
 - `-output_format`  : output format (use coco for COCO format)
 - `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
 - `-source_data_root`  : visionai local data root folder
 - `-output_dest_folder` : output root folder (COCO local root folder)
 - `-uri_root` : uri root for target upload for coco i.e: https://azuresorate/coco_dataset
 - `-n_frame`  : number of frame to be converted (-1 means all), by default -1
 - `-camera_sensor_name`  : camera sensor name (required for getting the target camera sensor data)
 - `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
 - `-img_extension` : image file extension (default: ".jpg")
 - `--copy_sensor_data` : enable to copy image data
 
+### Convert `YOLO` format data to `VisionAI` format
+
+```
+python3 visionai_data_format/convert_dataset.py -input_format yolo -output_format vision_ai -image_annotation_type 2d_bounding_box -source_data_root ./path_to_yolo_format_dir -output_dest_folder ./output_visionai_dir -n_frame -1 -sequence_idx_start 0 -uri_root http://storage_test -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg  --copy_sensor_data -classes_file category.txt
+```
+
+Arguments :
+- `-input_format`  : input format (use yolo for YOLO format)
+- `-output_format`  : output format (vision_ai)
+- `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
+- `-source_data_root`  : data root folder of yolo format
+- `-output_dest_folder` : output root folder (VisionAI local root folder)
+- `-uri_root` : uri root for target upload VisionAI storage i.e: https://azuresorate/vai_dataset
+- `-n_frame`  : number of frame to be converted (-1 means all), by default -1
+- `-sequence_idx_start `  : sequence start id, by default 0
+- `-camera_sensor_name`  : camera sensor name (default: "", specified it if need to convert camera data)
+- `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
+- `-img_extension` : image file extension (default: ".jpg")
+- `--copy_sensor_data` : enable to copy image data
+- `-classes_file` : txt file contain category names in each line, by default "classes.txt"
+- `-img_height` : image height for all images (default: None, which will read the image and get the size)
+- `-img_width` : image width for all images (default: None, which will read the image and get the size)
+
+
+* The `YOLO` dataset should follow the data structure as below:
+```bash
+.yolo-format-root_folder
+├── classes.txt
+├── images
+│   ├── 000000.png
+│   ├── 000001.png
+│   ├── 000002.png
+│   └── 000003.png
+├── labels
+│   ├── 000000.txt
+│   ├── 000001.txt
+│   ├── 000002.txt
+│   ├── 000003.txt
+```
+
+
 ## Troubleshooting
 
 (WIP)
 
 ## Next steps
 
 (WIP)
```

### Comparing `visionai_data_format-1.3.2/README.md` & `visionai_data_format-1.3.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: visionai-data-format
+Version: 1.3.3
+Summary: converter tool for visionai format
+Home-page: 
+Author: LinkerVision
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+Requires-Dist: pydantic==1.*
+Requires-Dist: pillow
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: mock; extra == "test"
+Requires-Dist: pre-commit; extra == "test"
+
 # visionai-data-format
 
 `VisionAI` format is [Dataverse](https://www.linkervision.com/visionai-platform-dataverse) standardized annotation format to label objects and sequences in the context of Autonomous Driving System(ADS). `VisionAI` provides consistent and effective driving environment description and categorization in the real-world case.
 
 This tool provides validator of `VisionAI` format schema. Currently, the library supports:
   - Validate created `VisionAI` data format
   - Validate `VisionAI` data attributes with given `Ontology` information.
@@ -565,21 +580,21 @@
 - `--copy_sensor_data` : enable to copy image/lidar data
 
 
 ### Convert `COCO` format data to `VisionAI` format
 
 ```
 python3 visionai_data_format/convert_dataset.py -input_format coco -output_format vision_ai -image_annotation_type 2d_bounding_box -input_annotation_path ./coco_instance.json -source_data_root ./coco_images/ -output_dest_folder ~/visionai_output_dir -uri_root http://storage_test -n_frame 5 -sequence_idx_start 0 -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg --copy_sensor_data
-
 ```
 
 Arguments :
 - `-input_format`  : input format (use coco for COCO format)
 - `-output_format`  : output format (vision_ai)
 - `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
+- `-input_annotation_path` : input annotation path for coco-label.json file
 - `-source_data_root`  : image data folder
 - `-output_dest_folder` : output root folder (VisionAI local root folder)
 - `-uri_root` : uri root for target upload VisionAI storage i.e: https://azuresorate/vai_dataset
 - `-n_frame`  : number of frame to be converted (-1 means all), by default -1
 - `-sequence_idx_start `  : sequence start id, by default 0
 - `-camera_sensor_name`  : camera sensor name (default: "", specified it if need to convert camera data)
 - `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
@@ -587,29 +602,69 @@
 - `--copy_sensor_data` : enable to copy image data
 
 
 ### Convert `VisionAI` format data to `COCO` format
 
 ```
 python3 visionai_data_format/convert_dataset.py -input_format vision_ai -output_format coco -image_annotation_type 2d_bounding_box -source_data_root ./visionai_data_root -output_dest_folder ~/coco_output_dir -uri_root http://storage_test -n_frame 5 -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg --copy_sensor_data
-
 ```
 Arguments :
 - `-input_format`  : input format (vision_ai)
 - `-output_format`  : output format (use coco for COCO format)
 - `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
 - `-source_data_root`  : visionai local data root folder
 - `-output_dest_folder` : output root folder (COCO local root folder)
 - `-uri_root` : uri root for target upload for coco i.e: https://azuresorate/coco_dataset
 - `-n_frame`  : number of frame to be converted (-1 means all), by default -1
 - `-camera_sensor_name`  : camera sensor name (required for getting the target camera sensor data)
 - `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
 - `-img_extension` : image file extension (default: ".jpg")
 - `--copy_sensor_data` : enable to copy image data
 
+### Convert `YOLO` format data to `VisionAI` format
+
+```
+python3 visionai_data_format/convert_dataset.py -input_format yolo -output_format vision_ai -image_annotation_type 2d_bounding_box -source_data_root ./path_to_yolo_format_dir -output_dest_folder ./output_visionai_dir -n_frame -1 -sequence_idx_start 0 -uri_root http://storage_test -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg  --copy_sensor_data -classes_file category.txt
+```
+
+Arguments :
+- `-input_format`  : input format (use yolo for YOLO format)
+- `-output_format`  : output format (vision_ai)
+- `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
+- `-source_data_root`  : data root folder of yolo format
+- `-output_dest_folder` : output root folder (VisionAI local root folder)
+- `-uri_root` : uri root for target upload VisionAI storage i.e: https://azuresorate/vai_dataset
+- `-n_frame`  : number of frame to be converted (-1 means all), by default -1
+- `-sequence_idx_start `  : sequence start id, by default 0
+- `-camera_sensor_name`  : camera sensor name (default: "", specified it if need to convert camera data)
+- `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
+- `-img_extension` : image file extension (default: ".jpg")
+- `--copy_sensor_data` : enable to copy image data
+- `-classes_file` : txt file contain category names in each line, by default "classes.txt"
+- `-img_height` : image height for all images (default: None, which will read the image and get the size)
+- `-img_width` : image width for all images (default: None, which will read the image and get the size)
+
+
+* The `YOLO` dataset should follow the data structure as below:
+```bash
+.yolo-format-root_folder
+├── classes.txt
+├── images
+│   ├── 000000.png
+│   ├── 000001.png
+│   ├── 000002.png
+│   └── 000003.png
+├── labels
+│   ├── 000000.txt
+│   ├── 000001.txt
+│   ├── 000002.txt
+│   ├── 000003.txt
+```
+
+
 ## Troubleshooting
 
 (WIP)
 
 ## Next steps
 
 (WIP)
```

### Comparing `visionai_data_format-1.3.2/setup.py` & `visionai_data_format-1.3.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.3.2"
+PACKAGE_VERSION = "1.3.3"
 DESC = "converter tool for visionai format"
-REQUIRED = ["pydantic==1.*"]
+REQUIRED = ["pydantic==1.*", "pillow"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
         "pre-commit",
     ],
```

### Comparing `visionai_data_format-1.3.2/tests/test_schemas.py` & `visionai_data_format-1.3.3/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/tests/test_validators.py` & `visionai_data_format-1.3.3/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/convert_dataset.py` & `visionai_data_format-1.3.3/visionai_data_format/convert_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,17 @@
         input_annotation_path: Optional[str] = None,
         sequence_idx_start: int = 0,
         copy_sensor_data: bool = True,
         n_frame: int = -1,
         annotation_name: str = "groundtruth",
         img_extension: str = ".jpg",
         ontology_classes: str = "",
+        classes_file_name: str = "classes.txt",
+        img_height: Optional[int] = None,
+        img_width: Optional[int] = None,
     ):
         """Run Dataset Converter
 
         Parameters
         ----------
         input_format : str
         output_format : str
@@ -51,14 +54,19 @@
             whether copy sensor files or not, by default True
         n_frame : int, optional
             number of frame to be converted (-1 means all), by default -1
         annotation_name : str, optional
             output annotation name, by default "groundtruth"
         img_extension : str, optional
             img file extension, by default ".jpg"
+        ontology_classes: str, by default: ""
+        classes_file_name: str, by default: "classes.txt",
+        img_height: int, optional
+        img_width: int, optional
+
 
         Raises
         ------
         ValueError
             If the selected convert case is not provided
         """
         input_format = AnnotationFormat(input_format)
@@ -80,14 +88,17 @@
             sequence_idx_start=sequence_idx_start,
             copy_sensor_data=copy_sensor_data,
             source_data_root=source_data_root,
             n_frame=n_frame,
             annotation_name=annotation_name,
             img_extension=img_extension,
             ontology_classes=ontology_classes,
+            classes_file_name=classes_file_name,
+            img_height=img_height,
+            img_width=img_width,
         )
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-input_format",
@@ -103,15 +114,14 @@
     )
     parser.add_argument(
         "-image_annotation_type",
         type=str,
         required=True,
         help="2d_bounding_box",
     )
-
     parser.add_argument(
         "-input_annotation_path",
         type=str,
         default="",
         help="BDD json path or coco annotation dir",
     )
     parser.add_argument(
@@ -134,50 +144,66 @@
     )
     parser.add_argument(
         "-camera_sensor_name",
         type=str,
         help="Camera Sensor name, i.e : `camera1`",
         default="",
     )
-
     parser.add_argument(
         "-lidar_sensor_name",
         type=str,
         help="Lidar Sensor name, i.e : `lidar1`",
         default="",
     )
     parser.add_argument(
         "-sequence_idx_start", type=int, help="sequence id start number", default=0
     )
-
     parser.add_argument(
         "-annotation_name",
         type=str,
         default="groundtruth",
         help=" annotation folder name (default: 'groundtruth')",
     )
     parser.add_argument(
         "-img_extension",
         type=str,
         default=".jpg",
         help="image extention (default: .jpg)",
     )
     parser.add_argument(
+        "-img_width",
+        type=int,
+        required=False,
+        help="image width",
+    )
+    parser.add_argument(
+        "-img_height",
+        type=int,
+        required=False,
+        help="image height",
+    )
+    parser.add_argument(
         "-n_frame",
         type=int,
         help="target convert frame number, -1 means all",
         default=-1,
     )
     parser.add_argument(
         "--ontology_classes",
         type=str,
         default="",
         help="','.join(ontology_classes_list), add this if we required category id follow the specified order ",
     )
     parser.add_argument(
+        "-classes_file",
+        type=str,
+        default="classes.txt",
+        help="file for store category names for yolo format",
+    )
+    parser.add_argument(
         "--copy_sensor_data",
         action="store_true",
         help="enable to copy image/lidar data",
     )
     FORMAT = "%(asctime)s[%(process)d][%(levelname)s] %(name)-16s : %(message)s"
     DATEFMT = "[%d-%m-%Y %H:%M:%S]"
 
@@ -187,15 +213,14 @@
         datefmt=DATEFMT,
     )
 
     args = parser.parse_args()
 
     if not args.camera_sensor_name and not args.lidar_sensor_name:
         raise VisionAIException(error_code=VisionAIErrorCode.VAI_ERR_002)
-
     DatasetConverter.run(
         input_format=args.input_format,
         output_format=args.output_format,
         image_annotation_type=args.image_annotation_type,
         input_annotation_path=args.input_annotation_path,
         source_data_root=args.source_data_root,
         output_dest_folder=args.output_dest_folder,
@@ -204,8 +229,11 @@
         camera_sensor_name=args.camera_sensor_name,
         lidar_sensor_name=args.lidar_sensor_name,
         annotation_name=args.annotation_name,
         img_extension=args.img_extension,
         n_frame=args.n_frame,
         copy_sensor_data=args.copy_sensor_data,
         ontology_classes=args.ontology_classes,
+        classes_file_name=args.classes_file,
+        img_width=args.img_width,
+        img_height=args.img_height,
     )
```

### Comparing `visionai_data_format-1.3.2/visionai_data_format/converters/base.py` & `visionai_data_format-1.3.3/visionai_data_format/converters/base.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/converters/bdd_to_vai.py` & `visionai_data_format-1.3.3/visionai_data_format/converters/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/converters/coco_to_vai.py` & `visionai_data_format-1.3.3/visionai_data_format/converters/coco_to_vai.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,28 +88,37 @@
                     n_frame -= 1
                 dest_sequence_name = f"{sequence_idx:012d}"
                 image_path = image_data["file_name"]
                 old_sequence_idx = os.path.splitext(image_path)[0].split(os.sep)[-1]
                 logger.info(
                     f"convert sequence {old_sequence_idx} to {dest_sequence_name}"
                 )
-                cls.convert_coco_to_vai(
+                vai_data = cls.convert_coco_to_vai(
                     image_data=image_data,
                     img_name_id_map=img_name_id_map,
                     vai_dest_folder=output_dest_folder,
                     camera_sensor_name=camera_sensor_name,
                     dest_sequence_name=dest_sequence_name,
                     uri_root=uri_root,
-                    annotation_name=annotation_name,
                     img_extension=img_extension,
                     copy_sensor_data=copy_sensor_data,
                     source_data_root=source_data_root,
                     class_id_name_map=class_id_name_map,
                     img_id_annotations_map=img_id_annotations_map,
                 )
+                save_as_json(
+                    vai_data,
+                    folder_name=os.path.join(
+                        output_dest_folder,
+                        dest_sequence_name,
+                        "annotations",
+                        annotation_name,
+                    ),
+                    file_name="visionai.json",
+                )
                 if n_frame == 0:
                     break
 
         except VisionAIException:
             logger.exception("Convert coco to vai format error")
             raise VisionAIException(
                 error_code=VisionAIErrorCode.VAI_ERR_041,
@@ -130,18 +139,17 @@
         camera_sensor_name: str,
         dest_sequence_name: str,
         uri_root: str,
         img_name_id_map: dict,
         source_data_root: str,
         class_id_name_map: dict[str, str],
         img_id_annotations_map: dict[str, list[dict]],
-        annotation_name: str = "groundtruth",
         img_extension: str = ".jpg",
         copy_sensor_data: bool = True,
-    ) -> None:
+    ) -> dict:
         try:
             image_file_name = image_data["file_name"]
             image_file_path = os.path.join(source_data_root, image_file_name)
 
             logger.info(
                 f"[convert_coco_to_vai] Convert started (copy sensor data is {copy_sensor_data})"
             )
@@ -234,19 +242,11 @@
                     "metadata": {"schema_version": "1.0.0"},
                 }
             }
             if not objects:
                 vai_data["visionai"].pop("objects")
 
             vai_data = validate_vai(vai_data).dict(exclude_none=True)
-
-            save_as_json(
-                vai_data,
-                folder_name=os.path.join(
-                    vai_dest_folder, dest_sequence_name, "annotations", annotation_name
-                ),
-                file_name="visionai.json",
-            )
-
             logger.info("[convert_coco_to_vai] Convert finished")
+            return vai_data
         except Exception as e:
             logger.error("[convert_coco_to_vai] Convert failed : " + str(e))
```

### Comparing `visionai_data_format-1.3.2/visionai_data_format/converters/kitti_to_vai.py` & `visionai_data_format-1.3.3/visionai_data_format/converters/kitti_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/converters/vai_to_coco.py` & `visionai_data_format-1.3.3/visionai_data_format/converters/vai_to_coco.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from visionai_data_format.converters.base import Converter, ConverterFactory
 from visionai_data_format.schemas.coco_schema import COCO, Annotation, Category, Image
 from visionai_data_format.schemas.common import AnnotationFormat, OntologyImageType
 from visionai_data_format.utils.classes import gen_ontology_classes_dict
 from visionai_data_format.utils.common import (
     ANNOT_PATH,
+    COCO_IMAGE_PATH,
     COCO_LABEL_FILE,
-    DATA_PATH,
     IMAGE_EXT,
     VISIONAI_JSON,
 )
 
 __all__ = ["VAItoCOCO"]
 
 logger = logging.getLogger(__name__)
@@ -48,28 +48,33 @@
         )
         category_map = gen_ontology_classes_dict(ontology_classes)
 
         sequence_folder_list = os.listdir(source_data_root)
         visionai_dict_list = []
         logger.info("retrieve visionai annotations started")
         for sequence in sequence_folder_list:
+            if not os.path.isdir(os.path.join(source_data_root, sequence)):
+                logger.info(
+                    f"file {sequence} is ignore since it is not a sequence folder"
+                )
+                continue
             annotation_path = os.path.join(
                 source_data_root,
                 sequence,
                 "annotations",
                 annotation_name,
                 VISIONAI_JSON,
             )
             logger.info(f"retrieve annotation from {annotation_path}")
             with open(annotation_path) as f:
                 visionai_dict_list.append(json.load(f))
 
         logger.info("retrieve visionai annotations finished")
 
-        dest_img_folder = os.path.join(output_dest_folder, DATA_PATH)
+        dest_img_folder = os.path.join(output_dest_folder, COCO_IMAGE_PATH)
         dest_json_folder = os.path.join(output_dest_folder, ANNOT_PATH)
         if copy_sensor_data:
             # create {dest}/data folder #
             os.makedirs(dest_img_folder, exist_ok=True)
         # create {dest}/annotations folder #
         os.makedirs(dest_json_folder, exist_ok=True)
 
@@ -150,15 +155,17 @@
         images = []
         annotations = []
         image_id = image_id_start
         anno_id = anno_id_start
         for frame_data in visionai_dict["visionai"]["frames"].values():
             if len(images) == n_frame:
                 break
-            dest_coco_url = os.path.join(uri_root, f"{image_id:012d}{img_extension}")
+            dest_coco_url = os.path.join(
+                uri_root, COCO_IMAGE_PATH, f"{image_id:012d}{img_extension}"
+            )
             dest_coco_img = os.path.join(
                 dest_img_folder, f"{image_id:012d}{img_extension}"
             )
             img_url = (
                 frame_data["frame_properties"]
                 .get("streams", {})
                 .get(camera_sensor_name, {})
```

### Comparing `visionai_data_format-1.3.2/visionai_data_format/exceptions/constants.py` & `visionai_data_format-1.3.3/visionai_data_format/exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/exceptions/error_messages.py` & `visionai_data_format-1.3.3/visionai_data_format/exceptions/error_messages.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/exceptions/visionai.py` & `visionai_data_format-1.3.3/visionai_data_format/exceptions/visionai.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/schemas/bdd_schema.py` & `visionai_data_format-1.3.3/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/schemas/coco_schema.py` & `visionai_data_format-1.3.3/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/schemas/common.py` & `visionai_data_format-1.3.3/visionai_data_format/schemas/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 class AnnotationFormat(str, Enum, metaclass=BaseEnumMeta):
     VISION_AI = "vision_ai"
     COCO = "coco"
     BDDP = "bddp"
     IMAGE = "image"
     KITTI = "kitti"
+    YOLO = "yolo"
 
 
 class DatasetType(str, Enum, metaclass=BaseEnumMeta):
     ANNOTATED_DATA = "annotated_data"
     RAW_DATA = "raw_data"
```

### Comparing `visionai_data_format-1.3.2/visionai_data_format/schemas/ontology.py` & `visionai_data_format-1.3.3/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/schemas/utils/validators.py` & `visionai_data_format-1.3.3/visionai_data_format/schemas/utils/validators.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/schemas/visionai_schema.py` & `visionai_data_format-1.3.3/visionai_data_format/schemas/visionai_schema.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/utils/calculation.py` & `visionai_data_format-1.3.3/visionai_data_format/utils/calculation.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/utils/checker.py` & `visionai_data_format-1.3.3/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/utils/classes.py` & `visionai_data_format-1.3.3/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/utils/common.py` & `visionai_data_format-1.3.3/visionai_data_format/utils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ANNOT_PATH = "annotations"
-DATA_PATH = "data"
+COCO_IMAGE_PATH = "images"
 GROUND_TRUTH_FOLDER = "annotations/groundtruth/"
 BBOX_NAME = "bbox_shape"
 IMAGE_EXT = ".jpg"
 COCO_LABEL_FILE = "labels.json"
 
 LOGGING_FORMAT = "%(asctime)s[%(process)d][%(levelname)s] %(name)-16s : %(message)s"
 LOGGING_DATEFMT = "[%d-%m-%Y %H:%M:%S]"
```

### Comparing `visionai_data_format-1.3.2/visionai_data_format/utils/converter.py` & `visionai_data_format-1.3.3/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/utils/resize.py` & `visionai_data_format-1.3.3/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/utils/validator.py` & `visionai_data_format-1.3.3/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/vai_to_bdd.py` & `visionai_data_format-1.3.3/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format/vai_to_bdd_v2.py` & `visionai_data_format-1.3.3/visionai_data_format/vai_to_bdd_v2.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.2/visionai_data_format.egg-info/PKG-INFO` & `visionai_data_format-1.3.3/visionai_data_format.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.3.2
+Version: 1.3.3
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
+Requires-Dist: pillow
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 
 # visionai-data-format
 
@@ -579,21 +580,21 @@
 - `--copy_sensor_data` : enable to copy image/lidar data
 
 
 ### Convert `COCO` format data to `VisionAI` format
 
 ```
 python3 visionai_data_format/convert_dataset.py -input_format coco -output_format vision_ai -image_annotation_type 2d_bounding_box -input_annotation_path ./coco_instance.json -source_data_root ./coco_images/ -output_dest_folder ~/visionai_output_dir -uri_root http://storage_test -n_frame 5 -sequence_idx_start 0 -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg --copy_sensor_data
-
 ```
 
 Arguments :
 - `-input_format`  : input format (use coco for COCO format)
 - `-output_format`  : output format (vision_ai)
 - `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
+- `-input_annotation_path` : input annotation path for coco-label.json file
 - `-source_data_root`  : image data folder
 - `-output_dest_folder` : output root folder (VisionAI local root folder)
 - `-uri_root` : uri root for target upload VisionAI storage i.e: https://azuresorate/vai_dataset
 - `-n_frame`  : number of frame to be converted (-1 means all), by default -1
 - `-sequence_idx_start `  : sequence start id, by default 0
 - `-camera_sensor_name`  : camera sensor name (default: "", specified it if need to convert camera data)
 - `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
@@ -601,29 +602,69 @@
 - `--copy_sensor_data` : enable to copy image data
 
 
 ### Convert `VisionAI` format data to `COCO` format
 
 ```
 python3 visionai_data_format/convert_dataset.py -input_format vision_ai -output_format coco -image_annotation_type 2d_bounding_box -source_data_root ./visionai_data_root -output_dest_folder ~/coco_output_dir -uri_root http://storage_test -n_frame 5 -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg --copy_sensor_data
-
 ```
 Arguments :
 - `-input_format`  : input format (vision_ai)
 - `-output_format`  : output format (use coco for COCO format)
 - `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
 - `-source_data_root`  : visionai local data root folder
 - `-output_dest_folder` : output root folder (COCO local root folder)
 - `-uri_root` : uri root for target upload for coco i.e: https://azuresorate/coco_dataset
 - `-n_frame`  : number of frame to be converted (-1 means all), by default -1
 - `-camera_sensor_name`  : camera sensor name (required for getting the target camera sensor data)
 - `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
 - `-img_extension` : image file extension (default: ".jpg")
 - `--copy_sensor_data` : enable to copy image data
 
+### Convert `YOLO` format data to `VisionAI` format
+
+```
+python3 visionai_data_format/convert_dataset.py -input_format yolo -output_format vision_ai -image_annotation_type 2d_bounding_box -source_data_root ./path_to_yolo_format_dir -output_dest_folder ./output_visionai_dir -n_frame -1 -sequence_idx_start 0 -uri_root http://storage_test -camera_sensor_name camera1 -annotation_name groundtruth -img_extension .jpg  --copy_sensor_data -classes_file category.txt
+```
+
+Arguments :
+- `-input_format`  : input format (use yolo for YOLO format)
+- `-output_format`  : output format (vision_ai)
+- `-image_annotation_type`  : label annotation type for image (2d_bounding_box for box2D)
+- `-source_data_root`  : data root folder of yolo format
+- `-output_dest_folder` : output root folder (VisionAI local root folder)
+- `-uri_root` : uri root for target upload VisionAI storage i.e: https://azuresorate/vai_dataset
+- `-n_frame`  : number of frame to be converted (-1 means all), by default -1
+- `-sequence_idx_start `  : sequence start id, by default 0
+- `-camera_sensor_name`  : camera sensor name (default: "", specified it if need to convert camera data)
+- `-annotation_name` : VisionAI annotation folder name (default: "groundtruth")
+- `-img_extension` : image file extension (default: ".jpg")
+- `--copy_sensor_data` : enable to copy image data
+- `-classes_file` : txt file contain category names in each line, by default "classes.txt"
+- `-img_height` : image height for all images (default: None, which will read the image and get the size)
+- `-img_width` : image width for all images (default: None, which will read the image and get the size)
+
+
+* The `YOLO` dataset should follow the data structure as below:
+```bash
+.yolo-format-root_folder
+├── classes.txt
+├── images
+│   ├── 000000.png
+│   ├── 000001.png
+│   ├── 000002.png
+│   └── 000003.png
+├── labels
+│   ├── 000000.txt
+│   ├── 000001.txt
+│   ├── 000002.txt
+│   ├── 000003.txt
+```
+
+
 ## Troubleshooting
 
 (WIP)
 
 ## Next steps
 
 (WIP)
```

### Comparing `visionai_data_format-1.3.2/visionai_data_format.egg-info/SOURCES.txt` & `visionai_data_format-1.3.3/visionai_data_format.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 visionai_data_format.egg-info/top_level.txt
 visionai_data_format/converters/__init__.py
 visionai_data_format/converters/base.py
 visionai_data_format/converters/bdd_to_vai.py
 visionai_data_format/converters/coco_to_vai.py
 visionai_data_format/converters/kitti_to_vai.py
 visionai_data_format/converters/vai_to_coco.py
+visionai_data_format/converters/yolo_to_vai.py
 visionai_data_format/exceptions/__init__.py
 visionai_data_format/exceptions/constants.py
 visionai_data_format/exceptions/error_messages.py
 visionai_data_format/exceptions/visionai.py
 visionai_data_format/schemas/__init__.py
 visionai_data_format/schemas/bdd_schema.py
 visionai_data_format/schemas/coco_schema.py
```


# Comparing `tmp/vistudio-1.0.1.8-py3-none-any.whl.zip` & `tmp/vistudio-1.0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,44 +1,77 @@
-Zip file size: 42238 bytes, number of entries: 42
--rw-r--r--  2.0 unx      173 b- defN 24-May-20 06:29 vistudio/__init__.py
--rw-r--r--  2.0 unx      329 b- defN 24-May-20 06:29 vistudio/annotation/__init__.py
--rw-r--r--  2.0 unx      341 b- defN 24-May-20 06:29 vistudio/annotation/api/__init__.py
--rw-r--r--  2.0 unx     4100 b- defN 24-May-20 06:29 vistudio/annotation/api/annotation.py
--rw-r--r--  2.0 unx      113 b- defN 24-May-20 06:29 vistudio/annotation/client/__init__.py
--rw-r--r--  2.0 unx     5454 b- defN 24-May-20 06:29 vistudio/annotation/client/annotation_client.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/config/__init__.py
--rw-r--r--  2.0 unx     5329 b- defN 24-May-20 06:29 vistudio/annotation/config/arg_parser.py
--rw-r--r--  2.0 unx     3011 b- defN 24-May-20 06:29 vistudio/annotation/config/config.py
--rw-r--r--  2.0 unx      250 b- defN 24-May-20 06:29 vistudio/annotation/datasource/__init__.py
--rw-r--r--  2.0 unx     6988 b- defN 24-May-20 06:29 vistudio/annotation/datasource/image_datasource.py
--rw-r--r--  2.0 unx     6773 b- defN 24-May-20 06:29 vistudio/annotation/datasource/mongo_query_pipeline.py
--rw-r--r--  2.0 unx    16328 b- defN 24-May-20 06:29 vistudio/annotation/datasource/sharded_mongo_datasource.py
--rw-r--r--  2.0 unx     2844 b- defN 24-May-20 06:29 vistudio/annotation/datasource/xml_datasource.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/__init__.py
--rw-r--r--  2.0 unx     7193 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/base_export_pipeline.py
--rw-r--r--  2.0 unx     5220 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/base_import_pipeline.py
--rw-r--r--  2.0 unx     3544 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/export_coco_pipeline.py
--rw-r--r--  2.0 unx     3836 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/export_paddleclas_pipeline.py
--rw-r--r--  2.0 unx     3881 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/export_paddleseg_pipeline.py
--rw-r--r--  2.0 unx     6554 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/import_cityscapes_pipeline.py
--rw-r--r--  2.0 unx     5859 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/import_coco_pipeline.py
--rw-r--r--  2.0 unx     4441 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/import_cvat_pipeline.py
--rw-r--r--  2.0 unx     6044 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/import_imagenet_pipeline.py
--rw-r--r--  2.0 unx     4810 b- defN 24-May-20 06:29 vistudio/annotation/pipeline/import_vistudio_pipeline.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/processor/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/processor/exporter/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/processor/exporter/coco/__init__.py
--rw-r--r--  2.0 unx     1680 b- defN 24-May-20 06:29 vistudio/annotation/processor/exporter/coco/coco_preprocessor.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/processor/exporter/paddleclas/__init__.py
--rw-r--r--  2.0 unx     2097 b- defN 24-May-20 06:29 vistudio/annotation/processor/exporter/paddleclas/paddleclas_preprocessor.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/processor/exporter/paddleseg/__init__.py
--rw-r--r--  2.0 unx     2308 b- defN 24-May-20 06:29 vistudio/annotation/processor/exporter/paddleseg/cityscape_preprocessor.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/processor/importer/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 06:29 vistudio/annotation/util/__init__.py
--rw-r--r--  2.0 unx      359 b- defN 24-May-20 06:29 vistudio/annotation/util/file.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-20 06:29 vistudio/annotation/util/polygon.py
--rw-r--r--  2.0 unx     1311 b- defN 24-May-20 06:29 vistudio/annotation/util/string.py
--rw-r--r--  2.0 unx      841 b- defN 24-May-20 06:29 vistudio-1.0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 06:29 vistudio-1.0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-May-20 06:29 vistudio-1.0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4269 b- defN 24-May-20 06:29 vistudio-1.0.1.8.dist-info/RECORD
-42 files, 120258 bytes uncompressed, 35090 bytes compressed:  70.8%
+Zip file size: 80553 bytes, number of entries: 75
+-rw-r--r--  2.0 unx      173 b- defN 24-May-20 07:33 vistudio/__init__.py
+-rw-r--r--  2.0 unx      329 b- defN 24-May-20 07:33 vistudio/annotation/__init__.py
+-rw-r--r--  2.0 unx      341 b- defN 24-May-20 07:33 vistudio/annotation/api/__init__.py
+-rw-r--r--  2.0 unx     4100 b- defN 24-May-20 07:33 vistudio/annotation/api/annotation.py
+-rw-r--r--  2.0 unx      113 b- defN 24-May-20 07:33 vistudio/annotation/client/__init__.py
+-rw-r--r--  2.0 unx     5454 b- defN 24-May-20 07:33 vistudio/annotation/client/annotation_client.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/config/__init__.py
+-rw-r--r--  2.0 unx     5329 b- defN 24-May-20 07:33 vistudio/annotation/config/arg_parser.py
+-rw-r--r--  2.0 unx     2926 b- defN 24-May-20 07:33 vistudio/annotation/config/config.py
+-rw-r--r--  2.0 unx      250 b- defN 24-May-20 07:33 vistudio/annotation/datasource/__init__.py
+-rw-r--r--  2.0 unx     6988 b- defN 24-May-20 07:33 vistudio/annotation/datasource/image_datasource.py
+-rw-r--r--  2.0 unx     6773 b- defN 24-May-20 07:33 vistudio/annotation/datasource/mongo_query_pipeline.py
+-rw-r--r--  2.0 unx    16724 b- defN 24-May-20 07:33 vistudio/annotation/datasource/sharded_mongo_datasource.py
+-rw-r--r--  2.0 unx     2844 b- defN 24-May-20 07:33 vistudio/annotation/datasource/xml_datasource.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/operator/__init__.py
+-rw-r--r--  2.0 unx     1860 b- defN 24-May-20 07:33 vistudio/annotation/operator/annotation_state_updater.py
+-rw-r--r--  2.0 unx     6590 b- defN 24-May-20 07:33 vistudio/annotation/operator/cityscapes_formatter.py
+-rw-r--r--  2.0 unx    11496 b- defN 24-May-20 07:33 vistudio/annotation/operator/coco_formatter.py
+-rw-r--r--  2.0 unx     7822 b- defN 24-May-20 07:33 vistudio/annotation/operator/cvat_formatter.py
+-rw-r--r--  2.0 unx     3105 b- defN 24-May-20 07:33 vistudio/annotation/operator/filter.py
+-rw-r--r--  2.0 unx     1488 b- defN 24-May-20 07:33 vistudio/annotation/operator/image_created_at_updater.py
+-rw-r--r--  2.0 unx     2241 b- defN 24-May-20 07:33 vistudio/annotation/operator/image_formatter.py
+-rw-r--r--  2.0 unx     3159 b- defN 24-May-20 07:33 vistudio/annotation/operator/imagenet_formatter.py
+-rw-r--r--  2.0 unx     4796 b- defN 24-May-20 07:33 vistudio/annotation/operator/label_formatter.py
+-rw-r--r--  2.0 unx     2558 b- defN 24-May-20 07:33 vistudio/annotation/operator/paddleclas_formatter.py
+-rw-r--r--  2.0 unx     5906 b- defN 24-May-20 07:33 vistudio/annotation/operator/paddleseg_formatter.py
+-rw-r--r--  2.0 unx     7893 b- defN 24-May-20 07:33 vistudio/annotation/operator/reader.py
+-rw-r--r--  2.0 unx     4012 b- defN 24-May-20 07:33 vistudio/annotation/operator/thumbnail_generator.py
+-rw-r--r--  2.0 unx     1594 b- defN 24-May-20 07:33 vistudio/annotation/operator/thumbnail_state_updater.py
+-rw-r--r--  2.0 unx     5150 b- defN 24-May-20 07:33 vistudio/annotation/operator/vistudio_formatter.py
+-rw-r--r--  2.0 unx     4412 b- defN 24-May-20 07:33 vistudio/annotation/operator/webp_generator.py
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-20 07:33 vistudio/annotation/operator/webp_state_updater.py
+-rw-r--r--  2.0 unx     2170 b- defN 24-May-20 07:33 vistudio/annotation/operator/zip_formatter.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/__init__.py
+-rw-r--r--  2.0 unx     7130 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/base_export_pipeline.py
+-rw-r--r--  2.0 unx     5220 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/base_import_pipeline.py
+-rw-r--r--  2.0 unx     3491 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/export_coco_pipeline.py
+-rw-r--r--  2.0 unx     3836 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/export_paddleclas_pipeline.py
+-rw-r--r--  2.0 unx     3881 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/export_paddleseg_pipeline.py
+-rw-r--r--  2.0 unx     2923 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/generate_thumbnail_pipeline.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/generate_webp_pipeline.py
+-rw-r--r--  2.0 unx     6554 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/import_cityscapes_pipeline.py
+-rw-r--r--  2.0 unx     5859 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/import_coco_pipeline.py
+-rw-r--r--  2.0 unx     4441 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/import_cvat_pipeline.py
+-rw-r--r--  2.0 unx     6044 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/import_imagenet_pipeline.py
+-rw-r--r--  2.0 unx     4810 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/import_vistudio_pipeline.py
+-rw-r--r--  2.0 unx     3174 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/update_annotation_state_pipeline.py
+-rw-r--r--  2.0 unx     2351 b- defN 24-May-20 07:33 vistudio/annotation/pipeline/update_image_created_at_pipeline.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/processor/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/processor/exporter/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/processor/exporter/coco/__init__.py
+-rw-r--r--  2.0 unx     1680 b- defN 24-May-20 07:33 vistudio/annotation/processor/exporter/coco/coco_preprocessor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/processor/exporter/paddleclas/__init__.py
+-rw-r--r--  2.0 unx     2097 b- defN 24-May-20 07:33 vistudio/annotation/processor/exporter/paddleclas/paddleclas_preprocessor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/processor/exporter/paddleseg/__init__.py
+-rw-r--r--  2.0 unx     2308 b- defN 24-May-20 07:33 vistudio/annotation/processor/exporter/paddleseg/cityscape_preprocessor.py
+-rw-r--r--  2.0 unx      113 b- defN 24-May-20 07:33 vistudio/annotation/processor/generator/__init__.py
+-rw-r--r--  2.0 unx     1141 b- defN 24-May-20 07:33 vistudio/annotation/processor/generator/thumbnail_preprocessor.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-20 07:33 vistudio/annotation/processor/generator/webp_preprocessor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/processor/importer/__init__.py
+-rw-r--r--  2.0 unx      113 b- defN 24-May-20 07:33 vistudio/annotation/processor/updater/__init__.py
+-rw-r--r--  2.0 unx     1123 b- defN 24-May-20 07:33 vistudio/annotation/processor/updater/annotation_state_preprocessor.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-20 07:33 vistudio/annotation/processor/updater/image_created_at_preprocessor.py
+-rw-r--r--  2.0 unx     1116 b- defN 24-May-20 07:33 vistudio/annotation/processor/updater/thumbnail_state_preprocessor.py
+-rw-r--r--  2.0 unx     1081 b- defN 24-May-20 07:33 vistudio/annotation/processor/updater/webp_state_preprocessor.py
+-rw-r--r--  2.0 unx      113 b- defN 24-May-20 07:33 vistudio/annotation/serve/__init__.py
+-rw-r--r--  2.0 unx     5644 b- defN 24-May-20 07:33 vistudio/annotation/serve/server.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 07:33 vistudio/annotation/util/__init__.py
+-rw-r--r--  2.0 unx      359 b- defN 24-May-20 07:33 vistudio/annotation/util/file.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-20 07:33 vistudio/annotation/util/polygon.py
+-rw-r--r--  2.0 unx     1311 b- defN 24-May-20 07:33 vistudio/annotation/util/string.py
+-rw-r--r--  2.0 unx      841 b- defN 24-May-20 07:33 vistudio-1.0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 07:33 vistudio-1.0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-20 07:33 vistudio-1.0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7872 b- defN 24-May-20 07:33 vistudio-1.0.1.9.dist-info/RECORD
+75 files, 225345 bytes uncompressed, 67443 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -36,14 +36,71 @@
 
 Filename: vistudio/annotation/datasource/sharded_mongo_datasource.py
 Comment: 
 
 Filename: vistudio/annotation/datasource/xml_datasource.py
 Comment: 
 
+Filename: vistudio/annotation/operator/__init__.py
+Comment: 
+
+Filename: vistudio/annotation/operator/annotation_state_updater.py
+Comment: 
+
+Filename: vistudio/annotation/operator/cityscapes_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/coco_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/cvat_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/filter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/image_created_at_updater.py
+Comment: 
+
+Filename: vistudio/annotation/operator/image_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/imagenet_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/label_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/paddleclas_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/paddleseg_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/reader.py
+Comment: 
+
+Filename: vistudio/annotation/operator/thumbnail_generator.py
+Comment: 
+
+Filename: vistudio/annotation/operator/thumbnail_state_updater.py
+Comment: 
+
+Filename: vistudio/annotation/operator/vistudio_formatter.py
+Comment: 
+
+Filename: vistudio/annotation/operator/webp_generator.py
+Comment: 
+
+Filename: vistudio/annotation/operator/webp_state_updater.py
+Comment: 
+
+Filename: vistudio/annotation/operator/zip_formatter.py
+Comment: 
+
 Filename: vistudio/annotation/pipeline/__init__.py
 Comment: 
 
 Filename: vistudio/annotation/pipeline/base_export_pipeline.py
 Comment: 
 
 Filename: vistudio/annotation/pipeline/base_import_pipeline.py
@@ -54,14 +111,20 @@
 
 Filename: vistudio/annotation/pipeline/export_paddleclas_pipeline.py
 Comment: 
 
 Filename: vistudio/annotation/pipeline/export_paddleseg_pipeline.py
 Comment: 
 
+Filename: vistudio/annotation/pipeline/generate_thumbnail_pipeline.py
+Comment: 
+
+Filename: vistudio/annotation/pipeline/generate_webp_pipeline.py
+Comment: 
+
 Filename: vistudio/annotation/pipeline/import_cityscapes_pipeline.py
 Comment: 
 
 Filename: vistudio/annotation/pipeline/import_coco_pipeline.py
 Comment: 
 
 Filename: vistudio/annotation/pipeline/import_cvat_pipeline.py
@@ -69,14 +132,20 @@
 
 Filename: vistudio/annotation/pipeline/import_imagenet_pipeline.py
 Comment: 
 
 Filename: vistudio/annotation/pipeline/import_vistudio_pipeline.py
 Comment: 
 
+Filename: vistudio/annotation/pipeline/update_annotation_state_pipeline.py
+Comment: 
+
+Filename: vistudio/annotation/pipeline/update_image_created_at_pipeline.py
+Comment: 
+
 Filename: vistudio/annotation/processor/__init__.py
 Comment: 
 
 Filename: vistudio/annotation/processor/exporter/__init__.py
 Comment: 
 
 Filename: vistudio/annotation/processor/exporter/coco/__init__.py
@@ -93,35 +162,65 @@
 
 Filename: vistudio/annotation/processor/exporter/paddleseg/__init__.py
 Comment: 
 
 Filename: vistudio/annotation/processor/exporter/paddleseg/cityscape_preprocessor.py
 Comment: 
 
+Filename: vistudio/annotation/processor/generator/__init__.py
+Comment: 
+
+Filename: vistudio/annotation/processor/generator/thumbnail_preprocessor.py
+Comment: 
+
+Filename: vistudio/annotation/processor/generator/webp_preprocessor.py
+Comment: 
+
 Filename: vistudio/annotation/processor/importer/__init__.py
 Comment: 
 
+Filename: vistudio/annotation/processor/updater/__init__.py
+Comment: 
+
+Filename: vistudio/annotation/processor/updater/annotation_state_preprocessor.py
+Comment: 
+
+Filename: vistudio/annotation/processor/updater/image_created_at_preprocessor.py
+Comment: 
+
+Filename: vistudio/annotation/processor/updater/thumbnail_state_preprocessor.py
+Comment: 
+
+Filename: vistudio/annotation/processor/updater/webp_state_preprocessor.py
+Comment: 
+
+Filename: vistudio/annotation/serve/__init__.py
+Comment: 
+
+Filename: vistudio/annotation/serve/server.py
+Comment: 
+
 Filename: vistudio/annotation/util/__init__.py
 Comment: 
 
 Filename: vistudio/annotation/util/file.py
 Comment: 
 
 Filename: vistudio/annotation/util/polygon.py
 Comment: 
 
 Filename: vistudio/annotation/util/string.py
 Comment: 
 
-Filename: vistudio-1.0.1.8.dist-info/METADATA
+Filename: vistudio-1.0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: vistudio-1.0.1.8.dist-info/WHEEL
+Filename: vistudio-1.0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: vistudio-1.0.1.8.dist-info/top_level.txt
+Filename: vistudio-1.0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: vistudio-1.0.1.8.dist-info/RECORD
+Filename: vistudio-1.0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vistudio/annotation/config/config.py

```diff
@@ -1,27 +1,20 @@
 # !/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 #
 # Copyright (c) 2024 Baidu.com, Inc. All Rights Reserved
 """
 Vistudio Spec
 """
-
-from windmillcomputev1.client.compute_api_compute import parse_compute_name
 from windmillcomputev1.client.compute_api_filesystem import parse_filesystem_name
 from windmillcomputev1.client.compute_client import ComputeClient
 from windmilltrainingv1.client.training_api_job import parse_job_name
 from windmilltrainingv1.client.training_client import TrainingClient
 
 from pydantic import BaseModel
-import logit
-
-logit.base_logger.setup_logger({})
-
-image_extensions = ('.jpeg', '.jpg', '.png', '.bmp')
 
 
 class Config(BaseModel):
     """
     定义基础变量
     """
     filesystem: dict = None
@@ -37,21 +30,21 @@
     job_name: str = ""
 
     org_id: str = ""
     user_id: str = ""
 
     def __init__(self, args: dict()):
         super().__init__(
-            job_name=args.get('job_name'),
-            mongodb_database=args.get('mongo_database'),
-            mongodb_collection=args.get('mongo_collection'),
-            windmill_endpoint=args.get('windmill_endpoint'),
-            windmill_ak=args.get('windmill_ak'),
-            windmill_sk=args.get('windmill_sk'),
-            vistudio_endpoint=args.get('vistudio_endpoint')
+            job_name=args.get('job_name', ''),
+            mongodb_database=args.get('mongo_database', ''),
+            mongodb_collection=args.get('mongo_collection', ''),
+            windmill_endpoint=args.get('windmill_endpoint', ''),
+            windmill_ak=args.get('windmill_ak', ''),
+            windmill_sk=args.get('windmill_sk', ''),
+            vistudio_endpoint=args.get('vistudio_endpoint', '')
         )
 
         self.parse_args(args)
 
     def parse_args(self, args: dict()):
         """
         parse_args
@@ -65,14 +58,17 @@
         self.mongo_uri = "mongodb://{}:{}@{}:{}".format(
             mongo_user,
             mongo_password,
             mongo_host,
             mongo_port
         )
 
+        if args.get('filesystem_name') is None:
+           return
+
         fsName = parse_filesystem_name(args.get('filesystem_name'))
         compute_client = ComputeClient(endpoint=self.windmill_endpoint,
                                        ak=self.windmill_ak,
                                        sk=self.windmill_sk)
 
         fs_res = compute_client.get_filesystem_credential(fsName.workspace_id,
                                                           fsName.local_name)
```

## vistudio/annotation/datasource/sharded_mongo_datasource.py

```diff
@@ -9,26 +9,24 @@
 import logging
 import re
 from typing import Dict, List, Optional, Callable
 import bson
 import pymongo
 import pymongoarrow.api
 import re
-
+from ray.data.datasource.datasource import Datasource
 from pymongo import MongoClient
 from ray.util.annotations import PublicAPI
 from ray.data.block import Block, BlockMetadata
 from ray.data.datasource.datasource import ReadTask
 from ray.data.datasource.mongo_datasource import MongoDatasource, _validate_database_collection_exist
 
 from vistudio.annotation.config.config import Config
 
-import logit
-
-logit.base_logger.setup_logger({})
+import bcelogger
 
 
 @PublicAPI(stability="alpha")
 class ShardedMongoDatasource(MongoDatasource):
     """Datasource for reading from and writing to MongoDB."""
 
     def __init__(
@@ -362,15 +360,15 @@
     query = {
         "annotation_set_id": annotation_set_id,
         "data_type": "Image"
     }
     exist_images = mongodb.find(query, ["image_id"])
     for image in exist_images:
         exist_images_set.add(image["image_id"])
-    logit.info("exist_images_set:{}".format(exist_images_set))
+    bcelogger.info("exist_images_set:{}".format(exist_images_set))
     return exist_images_set
 
 def _get_exist_annoation(config: Config, annotation_set_id: str):
     """
     获取当前标注集已有的标注信息
     :return:
     """
@@ -380,18 +378,30 @@
         "annotation_set_id": annotation_set_id,
         "data_type": "Annotation"
     }
     exist_anno = mongodb.find(query, ["image_id"])
     for anno in exist_anno:
         exist_annoation_set.add(anno["image_id"])
 
-    logit.info("exist_annoation_set:{}".format(exist_annoation_set))
+    bcelogger.info("exist_annoation_set:{}".format(exist_annoation_set))
     return exist_annoation_set
 
-
+def get_mongo_datasource(config: Config, pipeline, schema) -> Datasource:
+    """
+    get mongo datasource
+    :return: Datasource
+    """
+    source = ShardedMongoDatasource(
+        uri=config.mongo_uri,
+        database=config.mongodb_database,
+        collection=config.mongodb_collection,
+        pipeline=pipeline,
+        schema=schema,
+    )
+    return source
 
 def _example_read(item):
     """Example for reading data from ShardedMongoDatasource."""
     name = item["name"]
     float_field = item["float_field"]
     int_field = item["int_field"]
     print(f"name: {name}, float_field: {float_field}, int_field: {int_field}")
```

## vistudio/annotation/pipeline/base_export_pipeline.py

```diff
@@ -1,37 +1,37 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 """
 @File    :   base_pipeline.py
 """
 import os
 import re
-
 import json
-import logit
+import bcelogger
+
 from windmillcomputev1.filesystem import blobstore
 from windmilltrainingv1.client.training_client import TrainingClient
 
 from vistudio.annotation.client.annotation_client import AnnotationClient
-from vistudio.annotation.config import config
 from vistudio.annotation.config.config import Config
 from ray.data.datasource.datasource import Datasource
 from vistudio.annotation.datasource import mongo_query_pipeline
 from vistudio.annotation.datasource.sharded_mongo_datasource import ShardedMongoDatasource, parse_mongo_uri, \
     get_mongo_collection
 from vistudio.annotation.util import string
 
-logit.base_logger.setup_logger({})
 
 annotationset_name_pattern = r"workspaces/(?P<workspace_id>[^/]+)/projects/(?P<project_name>[^/]+)/annotationsets/" \
                              r"(?P<annotationset_local_name>[^/]+)$"
 
 ANNOTATION_FORMAT_COCO = 'COCO'
 ANNOTATION_FORMAT_IMAGENET = 'ImageNet'
 ANNOTATION_FORMAT_CITYSCAPES = 'Cityscapes'
+
+
 class BaseExportPipeline(object):
     """
     BaseExportPipeline
     """
     def __init__(self, args):
         self.args = args
         self.config = Config(args=args)
@@ -79,15 +79,15 @@
         :return:
         """
         if self.args.get('q') is not None and self.args.get('q') != '':
             mongo_pipeline = json.loads(string.decode_from_base64(self.args.get('q')))
         else:
             mongo_pipeline = None
 
-        logit.info("mongo_pipeline:{}".format(mongo_pipeline))
+        bcelogger.info("mongo_pipeline:{}".format(mongo_pipeline))
         return mongo_pipeline
 
     def _get_labels(self):
         """
         get labels
         :return:
         """
@@ -102,15 +102,15 @@
             annotationset_workspace_id = annotationset_name_dict.get("workspace_id")
             annotationset_project_name = annotationset_name_dict.get("project_name")
             annotationset_local_name = annotationset_name_dict.get("annotationset_local_name")
             anno_res = annotation_client.get_annotation_set(workspace_id=annotationset_workspace_id,
                                                             project_name=annotationset_project_name,
                                                             local_name=annotationset_local_name)
         except Exception as e:
-            logit.error("get annotation info exception.annotation_name:{}"
+            bcelogger.error("get annotation info exception.annotation_name:{}"
                          .format(annotation_set_name), e)
             raise Exception("Get annotation set info exception.annotation_set_name:{}".format(annotation_set_name))
 
         self.annotation_set_id = anno_res.id
         annotation_labels = anno_res.labels
         labels = {}
         if annotation_labels is not None:
@@ -154,15 +154,15 @@
             data_type=dataset.get('dataType', 'Image'),
             annotation_format=annotation_format,
             artifact_description=artifact.get('description', ''),
             artifact_alias=artifact.get('alias', []),
             artifact_tags=artifact.get('tags', []),
             artifact_metadata={'paths': [location + "/"]},
         )
-        logit.info("create dataset resp is {}".format(dataset_resp))
+        bcelogger.info("create dataset resp is {}".format(dataset_resp))
 
     def save_label_file(self, file_path: str, labels: dict(), start_index: int = 0):
         """
         save_label_file
         :param file_path:
         :param labels:
         :param start_index:
```

## vistudio/annotation/pipeline/export_coco_pipeline.py

```diff
@@ -1,32 +1,29 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 """
 @File    :   export_pipeline.py
 """
 
-from ray.data.read_api import read_datasource
-import ray
 import sys
 import os
+import bcelogger
+from ray.data.read_api import read_datasource
 
 __work_dir__ = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
 sys.path.insert(0, __work_dir__)
 from windmillartifactv1.client.artifact_client import ArtifactClient
 from windmillcomputev1.filesystem import init_py_filesystem
+from windmilltrainingv1.client.training_api_dataset import DatasetName
 
 from vistudio.annotation.datasink.filename_provider import MultiFilenameProvider
-from sdk.python.vistudio.annotation.config.arg_parser import ArgParser
-from windmilltrainingv1.client.training_api_dataset import DatasetName
-from base_export_pipeline import BaseExportPipeline
+from vistudio.annotation.config.arg_parser import ArgParser
 from vistudio.annotation.processor.exporter.coco.coco_preprocessor import CocoFormatPreprocessor, CocoMergePreprocessor
-import argparse
-import logit
 
-logit.base_logger.setup_logger({})
+from base_export_pipeline import BaseExportPipeline
 
 
 class ExportCocoPipeline(BaseExportPipeline):
     """
     exporter coco pipeline
     """
 
@@ -42,35 +39,35 @@
     def run(self, parallelism: int = 10):
         """
         pipeline_coco
         :return:
         """
         # step 1: datasource
         ds = read_datasource(self.datasource, parallelism=parallelism)
-        logit.info("read data from mongo.dataset count = {}".format(ds.count()))
+        bcelogger.info("read data from mongo.dataset count = {}".format(ds.count()))
         if ds.count() <= 0:
             return
 
         coco_format_preprocessor = CocoFormatPreprocessor(labels=self.labels, merge_labels=self.merge_labels)
         coco_merge_preprocessor = CocoMergePreprocessor(labels=self.labels)
         format_ds = coco_format_preprocessor.transform(ds)
-        logit.info("format dataset.dataset count = {}".format(format_ds.count()))
+        bcelogger.info("format dataset.dataset count = {}".format(format_ds.count()))
         merge_ds = coco_merge_preprocessor.fit(format_ds).stats_
-        logit.info("merge dataset.dataset count = {}".format(merge_ds.count()))
+        bcelogger.info("merge dataset.dataset count = {}".format(merge_ds.count()))
 
         # setp 3: writer
         dataset_name = DatasetName(workspace_id=self.dataset.get('workspaceID'),
                                    project_name=self.dataset.get('projectName'),
                                    local_name=self.dataset.get('localName'))
         object_name = dataset_name.get_name()
         location_resp = self.artifact_client.create_location(
             object_name=object_name
         )
         path = location_resp.location[len("s3://"):].strip("/")
-        logit.info("create windmill location. location= {}".format(path))
+        bcelogger.info("create windmill location. location= {}".format(path))
 
         annotation_filename_provider = MultiFilenameProvider(file_name="annotation.json")
         merge_ds.write_json(path=path,
                             filesystem=self._py_fs,
                             filename_provider=annotation_filename_provider)
         label_txt_full_path = os.path.join(location_resp.location, "labels.txt")
         self.save_label_file(file_path=label_txt_full_path, labels=self.labels, start_index=0)
```

## Comparing `vistudio-1.0.1.8.dist-info/METADATA` & `vistudio-1.0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vistudio
-Version: 1.0.1.8
+Version: 1.0.1.9
 Summary: sdk in python for annotation
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/bce-vistudio/vistudio-annotation/tree/master/sdk
 Author: yangtingyu01
 Author-email: yangtingyu01@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```


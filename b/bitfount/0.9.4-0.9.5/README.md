# Comparing `tmp/bitfount-0.9.4.tar.gz` & `tmp/bitfount-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitfount-0.9.4.tar", last modified: Tue Feb 20 16:11:05 2024, max compression
+gzip compressed data, was "bitfount-0.9.5.tar", last modified: Fri Feb 23 16:04:39 2024, max compression
```

## Comparing `bitfount-0.9.4.tar` & `bitfount-0.9.5.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.650738 bitfount-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-02-20 16:10:51.000000 bitfount-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-20 16:10:51.000000 bitfount-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    30153 2024-02-20 16:11:05.646738 bitfount-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-02-20 16:10:51.000000 bitfount-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.474735 bitfount-0.9.4/bitfount/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.478736 bitfount-0.9.4/bitfount/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.478736 bitfount-0.9.4/bitfount/backends/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/_torch_shims.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.482735 bitfount-0.9.4/bitfount/backends/pytorch/data/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/data/datafactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/data/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/epoch_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.482735 bitfount-0.9.4/bitfount/backends/pytorch/federated/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/federated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/federated/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/federated/shim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.486735 bitfount-0.9.4/bitfount/backends/pytorch/models/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69282 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/models/base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    25215 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/models/bitfount_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26374 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/models/nn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.486735 bitfount-0.9.4/bitfount/backends/pytorch/models/torch_functions/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/models/torch_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/models/torch_functions/mish.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/backends/pytorch/weight_clipper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.490736 bitfount-0.9.4/bitfount/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/databunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datafactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    28171 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.498736 bitfount-0.9.4/bitfount/data/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87068 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/base_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/csv_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    16230 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/database_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/dataframe_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/dicom_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/empty_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/excel_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/view_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasources/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    18637 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datasplitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    33259 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/datastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.498736 bitfount-0.9.4/bitfount/data/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/huggingface/datafactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/huggingface/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/huggingface/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/huggingface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.498736 bitfount-0.9.4/bitfount/data/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/persistence/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21249 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/persistence/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    52427 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    21411 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.506736 bitfount-0.9.4/bitfount/federated/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.510736 bitfount-0.9.4/bitfount/federated/aggregators/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/aggregators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14130 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/aggregators/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/aggregators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/aggregators/secure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.510736 bitfount-0.9.4/bitfount/federated/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/column_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)    19589 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/compute_intersection_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/csv_report_algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.514736 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_image_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18108 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_text_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_text_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_zero_shot_image_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    35510 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/timm_fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/timm_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.518736 bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/federated_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/train_and_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/private_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/algorithms/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    31813 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/authorisation_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)    16842 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/keys_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    35921 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/model_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/modeller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.518736 bitfount-0.9.4/bitfount/federated/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/monitoring/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/monitoring/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/monitoring/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/monitoring/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    68410 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)    41238 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/pod_db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/pod_response_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/pod_vitals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.518736 bitfount-0.9.4/bitfount/federated/privacy/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/privacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/privacy/differential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.518736 bitfount-0.9.4/bitfount/federated/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.522736 bitfount-0.9.4/bitfount/federated/protocols/model_protocols/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/model_protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23768 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/model_protocols/federated_averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/model_protocols/inference_csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/model_protocols/instrumented_inference_csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/psi.py
--rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/protocols/results_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/shim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/task_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.526736 bitfount-0.9.4/bitfount/federated/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50863 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/base_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23176 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.526736 bitfount-0.9.4/bitfount/federated/transport/identity_verification/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/identity_verification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20375 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/identity_verification/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/identity_verification/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/identity_verification/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    47276 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/message_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    41920 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/modeller_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/pod_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.530736 bitfount-0.9.4/bitfount/federated/transport/protos/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/protos/messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32420 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/protos/messages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/protos/messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/protos/messages_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/transport/worker_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31179 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/federated/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    24520 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.530736 bitfount-0.9.4/bitfount/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51905 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hub/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hub/authentication_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hub/authentication_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hub/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hub/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hub/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/hub/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.534736 bitfount-0.9.4/bitfount/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32398 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/models/base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/models/bitfount_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/models/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.538736 bitfount-0.9.4/bitfount/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48784 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/runners/config_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/runners/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/runners/modeller_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/runners/pod_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/runners/upload_task_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/runners/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.538736 bitfount-0.9.4/bitfount/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/schemas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/schemas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.542736 bitfount-0.9.4/bitfount/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/scripts/generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/scripts/generate_yaml_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/scripts/run_modeller.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/scripts/run_pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/scripts/run_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/scripts/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.546736 bitfount-0.9.4/bitfount/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/base_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/batch_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/binary_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/dataset_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22144 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/references.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/torchio_batch_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/unary_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/transformations/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.546736 bitfount-0.9.4/bitfount/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    34243 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/utils/concurrency_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/utils/db_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/utils/ssl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20213 2024-02-20 16:10:51.000000 bitfount-0.9.4/bitfount/utils/web_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.558736 bitfount-0.9.4/bitfount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30153 2024-02-20 16:11:05.000000 bitfount-0.9.4/bitfount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9551 2024-02-20 16:11:05.000000 bitfount-0.9.4/bitfount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:11:05.000000 bitfount-0.9.4/bitfount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-20 16:11:05.000000 bitfount-0.9.4/bitfount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-02-20 16:11:05.000000 bitfount-0.9.4/bitfount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-20 16:11:05.000000 bitfount-0.9.4/bitfount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-02-20 16:10:51.000000 bitfount-0.9.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.550736 bitfount-0.9.4/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.550736 bitfount-0.9.4/requirements/310/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/310/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/310/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/310/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/310/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/310/requirements-tutorial.in
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/310/requirements-tutorial.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.554736 bitfount-0.9.4/requirements/38/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.558736 bitfount-0.9.4/requirements/38/differential_privacy/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/differential_privacy/constraints-dp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/differential_privacy/requirements-dp-test.in
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/differential_privacy/requirements-dp.in
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/requirements-tutorial.in
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/38/requirements-tutorial.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.558736 bitfount-0.9.4/requirements/39/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:11:05.558736 bitfount-0.9.4/requirements/39/differential_privacy/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/differential_privacy/constraints-dp.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/differential_privacy/requirements-dp-test.in
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/differential_privacy/requirements-dp.in
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/requirements-tutorial.in
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/39/requirements-tutorial.txt
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/constraints-compatibility.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/constraints-direct.txt
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/constraints-security.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-02-20 16:10:51.000000 bitfount-0.9.4/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:11:05.650738 bitfount-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-02-20 16:10:51.000000 bitfount-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.865490 bitfount-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-02-23 16:04:30.000000 bitfount-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-23 16:04:30.000000 bitfount-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30153 2024-02-23 16:04:39.865490 bitfount-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-02-23 16:04:30.000000 bitfount-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.785489 bitfount-0.9.5/bitfount/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.785489 bitfount-0.9.5/bitfount/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.785489 bitfount-0.9.5/bitfount/backends/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/_torch_shims.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.789489 bitfount-0.9.5/bitfount/backends/pytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/data/datafactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/data/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/epoch_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.789489 bitfount-0.9.5/bitfount/backends/pytorch/federated/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/federated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/federated/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/federated/shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.789489 bitfount-0.9.5/bitfount/backends/pytorch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69282 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/models/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25215 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/models/bitfount_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26374 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/models/nn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.789489 bitfount-0.9.5/bitfount/backends/pytorch/models/torch_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/models/torch_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/models/torch_functions/mish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/backends/pytorch/weight_clipper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.789489 bitfount-0.9.5/bitfount/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/databunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datafactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28316 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.793489 bitfount-0.9.5/bitfount/data/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91927 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/base_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/csv_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16230 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/database_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/dataframe_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/dicom_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/empty_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/excel_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/view_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22163 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasources/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18637 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datasplitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33259 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.793489 bitfount-0.9.5/bitfount/data/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/huggingface/datafactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/huggingface/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/huggingface/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/huggingface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.793489 bitfount-0.9.5/bitfount/data/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/persistence/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/persistence/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52428 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21411 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.797489 bitfount-0.9.5/bitfount/federated/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.797489 bitfount-0.9.5/bitfount/federated/aggregators/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/aggregators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14130 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/aggregators/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/aggregators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/aggregators/secure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.797489 bitfount-0.9.5/bitfount/federated/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/column_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19589 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/compute_intersection_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/csv_report_algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.801489 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_text_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_zero_shot_image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35763 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/timm_fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/timm_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.801489 bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/federated_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/train_and_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/private_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/algorithms/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31813 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/authorisation_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16842 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/keys_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35921 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/model_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/modeller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.801489 bitfount-0.9.5/bitfount/federated/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/monitoring/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/monitoring/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/monitoring/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/monitoring/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69274 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41238 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/pod_db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/pod_response_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/pod_vitals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.801489 bitfount-0.9.5/bitfount/federated/privacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/privacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/privacy/differential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.801489 bitfount-0.9.5/bitfount/federated/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.801489 bitfount-0.9.5/bitfount/federated/protocols/model_protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/model_protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23768 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/model_protocols/federated_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/model_protocols/inference_csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/model_protocols/instrumented_inference_csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/psi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/protocols/results_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/task_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.805489 bitfount-0.9.5/bitfount/federated/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52121 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/base_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23176 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.805489 bitfount-0.9.5/bitfount/federated/transport/identity_verification/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/identity_verification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20375 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/identity_verification/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/identity_verification/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/identity_verification/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47276 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41920 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/modeller_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/pod_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.805489 bitfount-0.9.5/bitfount/federated/transport/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/protos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/protos/messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32420 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/protos/messages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/protos/messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/protos/messages_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/transport/worker_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31179 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/federated/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24520 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.805489 bitfount-0.9.5/bitfount/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51905 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hub/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hub/authentication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hub/authentication_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hub/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hub/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hub/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/hub/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.809489 bitfount-0.9.5/bitfount/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32398 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/models/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/models/bitfount_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26302 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/models/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.809489 bitfount-0.9.5/bitfount/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48784 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/runners/config_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/runners/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/runners/modeller_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/runners/pod_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/runners/upload_task_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/runners/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.809489 bitfount-0.9.5/bitfount/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/schemas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/schemas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.809489 bitfount-0.9.5/bitfount/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/scripts/generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/scripts/generate_yaml_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/scripts/run_modeller.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/scripts/run_pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/scripts/run_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/scripts/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.809489 bitfount-0.9.5/bitfount/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/base_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/batch_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/binary_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/dataset_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22144 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/torchio_batch_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/unary_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/transformations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.813489 bitfount-0.9.5/bitfount/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    34243 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/utils/concurrency_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/utils/db_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/utils/ssl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20213 2024-02-23 16:04:30.000000 bitfount-0.9.5/bitfount/utils/web_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.817489 bitfount-0.9.5/bitfount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30153 2024-02-23 16:04:39.000000 bitfount-0.9.5/bitfount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9551 2024-02-23 16:04:39.000000 bitfount-0.9.5/bitfount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 16:04:39.000000 bitfount-0.9.5/bitfount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-23 16:04:39.000000 bitfount-0.9.5/bitfount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-02-23 16:04:39.000000 bitfount-0.9.5/bitfount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 16:04:39.000000 bitfount-0.9.5/bitfount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-02-23 16:04:30.000000 bitfount-0.9.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.813489 bitfount-0.9.5/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.813489 bitfount-0.9.5/requirements/310/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/310/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/310/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/310/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/310/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/310/requirements-tutorial.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/310/requirements-tutorial.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.813489 bitfount-0.9.5/requirements/38/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.813489 bitfount-0.9.5/requirements/38/differential_privacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/differential_privacy/constraints-dp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/differential_privacy/requirements-dp-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/differential_privacy/requirements-dp.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/requirements-tutorial.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/38/requirements-tutorial.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.813489 bitfount-0.9.5/requirements/39/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 16:04:39.817489 bitfount-0.9.5/requirements/39/differential_privacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/differential_privacy/constraints-dp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/differential_privacy/requirements-dp-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/differential_privacy/requirements-dp.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/requirements-tutorial.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/39/requirements-tutorial.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/constraints-compatibility.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/constraints-direct.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/constraints-security.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-02-23 16:04:30.000000 bitfount-0.9.5/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 16:04:39.865490 bitfount-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-02-23 16:04:30.000000 bitfount-0.9.5/setup.py
```

### Comparing `bitfount-0.9.4/LICENSE` & `bitfount-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/MANIFEST.in` & `bitfount-0.9.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/PKG-INFO` & `bitfount-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitfount
-Version: 0.9.4
+Version: 0.9.5
 Summary: Machine Learning and Federated Learning Library.
 Home-page: https://github.com/bitfount/bitfount
 Author: Bitfount
 Author-email: info@bitfount.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.bitfount.com/
 Project-URL: Homepage, https://bitfount.com
```

### Comparing `bitfount-0.9.4/README.md` & `bitfount-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/__init__.py` & `bitfount-0.9.5/bitfount/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/__version__.py` & `bitfount-0.9.5/bitfount/__version__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 
 __author__ = "Bitfount"
 __author_email__ = "info@bitfount.com"
 __copyright__ = "Copyright 2021 Bitfount Ltd"
 __description__ = "Machine Learning and Federated Learning Library."
 __title__ = "bitfount"
 __url__ = "https://github.com/bitfount/bitfount"
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 __yaml_versions__ = ["2.0.0"]  # major for bitfount breaking changes,
 # minor for non-breaking changes,
 # patch for plugins versioning
```

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/__init__.py` & `bitfount-0.9.5/bitfount/backends/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/_torch_shims.py` & `bitfount-0.9.5/bitfount/backends/pytorch/_torch_shims.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/data/datafactory.py` & `bitfount-0.9.5/bitfount/backends/pytorch/data/datafactory.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/data/dataloaders.py` & `bitfount-0.9.5/bitfount/backends/pytorch/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/data/datasets.py` & `bitfount-0.9.5/bitfount/backends/pytorch/data/datasets.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/data/utils.py` & `bitfount-0.9.5/bitfount/backends/pytorch/data/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/epoch_callbacks.py` & `bitfount-0.9.5/bitfount/backends/pytorch/epoch_callbacks.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/federated/mixins.py` & `bitfount-0.9.5/bitfount/backends/pytorch/federated/mixins.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/federated/shim.py` & `bitfount-0.9.5/bitfount/backends/pytorch/federated/shim.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/loss.py` & `bitfount-0.9.5/bitfount/backends/pytorch/loss.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/models/base_models.py` & `bitfount-0.9.5/bitfount/backends/pytorch/models/base_models.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/models/bitfount_model.py` & `bitfount-0.9.5/bitfount/backends/pytorch/models/bitfount_model.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/models/models.py` & `bitfount-0.9.5/bitfount/backends/pytorch/models/models.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/models/nn.py` & `bitfount-0.9.5/bitfount/backends/pytorch/models/nn.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/models/torch_functions/mish.py` & `bitfount-0.9.5/bitfount/backends/pytorch/models/torch_functions/mish.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/types.py` & `bitfount-0.9.5/bitfount/backends/pytorch/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/utils.py` & `bitfount-0.9.5/bitfount/backends/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/backends/pytorch/weight_clipper.py` & `bitfount-0.9.5/bitfount/backends/pytorch/weight_clipper.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/config.py` & `bitfount-0.9.5/bitfount/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dealing with interactions with configuration and environment variables."""
+
 from importlib import util
 from importlib.machinery import ModuleSpec
 from functools import lru_cache
 import logging
 import os
 from pathlib import Path
 from typing import Callable, Dict, Final, List, Optional, Tuple, cast
@@ -39,14 +40,21 @@
     "BITFOUNT_DEFAULT_BATCHED_EXECUTION",
     # Backend engine
     "BITFOUNT_ENGINE",
     # GPU
     "get_gpu_metadata",
     # YAML versioning
     "_BITFOUNT_COMPATIBLE_YAML_VERSIONS",
+    # Environment
+    "_get_environment",
+    # DP Support
+    "DP_AVAILABLE",
+    # Shutdown variables
+    "POD_HEARTBEAT_SHUTDOWN_TIMEOUT",
+    "POD_VITALS_HANDLER_SHUTDOWN_TIMEOUT",
 ]
 
 from marshmallow import ValidationError
 
 logger = logging.getLogger(__name__)
 
 
@@ -163,14 +171,18 @@
 _SANDBOX_ENVIRONMENT: Final[str] = "sandbox"
 _ENVIRONMENT_CANDIDATES: Tuple[str, ...] = (
     _PRODUCTION_ENVIRONMENT,
     _STAGING_ENVIRONMENT,
     _DEVELOPMENT_ENVIRONMENT,
     _SANDBOX_ENVIRONMENT,
 )
+# A Bitfount child process is a process that is spawned by the main Bitfount process
+# to perform a specific task. This is used to determine if the current process is a
+# child process or not and therefore if certain actions should be taken or not.
+_BITFOUNT_CHILD_PROCESS: bool = env.bool("_BITFOUNT_CHILD_PROCESS", default=False)
 
 
 def _get_compatible_yaml_versions() -> Optional[List[str]]:
     """Get the compatible yaml versions.
 
     If plugins are used, they need to contain the compatible
     version in the plugins directory in a __version__.py file.
@@ -271,21 +283,26 @@
     if BITFOUNT_ENGINE not in _ENGINE_CANDIDATES:
         raise ValueError(
             f"The backend engine specified by the environment variable "
             f"BITFOUNT_ENGINE ({BITFOUNT_ENGINE}) is not in the supported list of "
             f"backends ({_ENGINE_CANDIDATES})"
         )
 except KeyError:
-    # Otherwise, if PyTorch is installed use PYTORCH_ENGINE
-    try:
-        import torch  # noqa: F401
-
-        BITFOUNT_ENGINE = _PYTORCH_ENGINE
-    except ImportError:
-        pass
+    # Don't import pytorch if in a child process
+    if not _BITFOUNT_CHILD_PROCESS:
+        # Otherwise, if PyTorch is installed use PYTORCH_ENGINE
+        try:
+            import torch  # noqa: F401
+
+            BITFOUNT_ENGINE = _PYTORCH_ENGINE
+        except ImportError:
+            pass
+    else:
+        logger.warning("Not importing PyTorch in a child process.")
+
 #########################
 # End of Backend Engine #
 #########################
 
 ##############
 # DP Support #
 ##############
```

### Comparing `bitfount-0.9.4/bitfount/data/__init__.py` & `bitfount-0.9.5/bitfount/data/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/databunch.py` & `bitfount-0.9.5/bitfount/data/databunch.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datafactory.py` & `bitfount-0.9.5/bitfount/data/datafactory.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/dataloaders.py` & `bitfount-0.9.5/bitfount/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasets.py` & `bitfount-0.9.5/bitfount/data/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes concerning datasets."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from functools import cached_property
 import logging
 from typing import (
     TYPE_CHECKING,
@@ -225,17 +226,19 @@
         imgs: Tuple[np.ndarray, ...] = tuple(
             imread(image, plugin="pil")
             for image in img_features
             if image is not pd.NA and image is not np.nan
         )
         if self.auto_convert_grayscale_images:
             imgs = tuple(
-                gray2rgb(image_array)
-                if len(image_array.squeeze().shape) < 3
-                else image_array
+                (
+                    gray2rgb(image_array)
+                    if len(image_array.squeeze().shape) < 3
+                    else image_array
+                )
                 for image_array in imgs
             )
         imgs = tuple(
             self._transform_image(image_array, i) for i, image_array in enumerate(imgs)
         )
 
         if len(img_features) == 1:
@@ -633,17 +636,19 @@
         imgs: Tuple[np.ndarray, ...] = tuple(
             image
             for image in img_features
             if image is not pd.NA and image is not np.nan
         )
         if self.auto_convert_grayscale_images:
             imgs = tuple(
-                gray2rgb(image_array)
-                if len(image_array.squeeze().shape) < 3
-                else image_array
+                (
+                    gray2rgb(image_array)
+                    if len(image_array.squeeze().shape) < 3
+                    else image_array
+                )
                 for image_array in imgs
             )
         imgs = tuple(
             self._transform_image(image_array, i) for i, image_array in enumerate(imgs)
         )
 
         if len(img_features) == 1:
@@ -710,17 +715,19 @@
         imgs: Tuple[np.ndarray, ...] = tuple(
             image
             for image in img_features
             if image is not pd.NA and image is not np.nan
         )
         if self.auto_convert_grayscale_images:
             imgs = tuple(
-                gray2rgb(image_array)
-                if len(image_array.squeeze().shape) < 3
-                else image_array
+                (
+                    gray2rgb(image_array)
+                    if len(image_array.squeeze().shape) < 3
+                    else image_array
+                )
                 for image_array in imgs
             )
         imgs = tuple(
             self._transform_image(image_array, i) for i, image_array in enumerate(imgs)
         )
 
         if len(img_features) == 1:
```

### Comparing `bitfount-0.9.4/bitfount/data/datasources/__init__.py` & `bitfount-0.9.5/bitfount/data/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/base_source.py` & `bitfount-0.9.5/bitfount/data/datasources/base_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module containing BaseSource class.
 
 BaseSource is the abstract data source class from which all concrete data sources
 must inherit.
 """
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from datetime import date, datetime
 import functools
 from functools import cached_property
@@ -34,14 +35,15 @@
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 from filetype import guess_extension
+import methodtools
 from mypy_extensions import Arg, DefaultNamedArg, KwArg, VarArg
 import numpy as np
 import pandas as pd
 from pandas.core.dtypes.cast import (  # type: ignore[attr-defined] # Reason: this function _is_ defined but is technically private # noqa: B950
     find_common_type,
 )
 from pandas.core.dtypes.common import is_datetime64_any_dtype as is_datetime
@@ -55,14 +57,15 @@
     ORIGINAL_FILENAME_METADATA_COLUMN,
     _modify_column,
     _modify_file_paths,
 )
 from bitfount.data.datasplitters import DatasetSplitter, SplitterDefinedInData
 from bitfount.data.exceptions import DataNotLoadedError, IterableDataSourceError
 from bitfount.data.persistence.base import DataPersister
+from bitfount.data.persistence.sqlite import SQLiteDataPersister
 from bitfount.data.types import (
     DataPathModifiers,
     _Column,
     _GetColumnCallable,
     _GetDtypesCallable,
     _SingleOrMulti,
 )
@@ -136,14 +139,19 @@
     Attributes:
         data: A Dataframe-type object which contains the data.
         data_splitter: Approach used for splitting the data into training, test,
             validation.
         seed: Random number seed. Used for setting random seed for all libraries.
     """
 
+    # TODO: [BIT-3722] Method Resolution Order appears to be broken such that if methods
+    # that are defined in a base class are overridden in a subclass, the base class
+    # implementation is preferentially called over the subclass implementation. Be
+    # mindful of this when overriding methods.
+
     def __init__(
         self,
         data_splitter: Optional[DatasetSplitter] = None,
         seed: Optional[int] = None,
         modifiers: Optional[Dict[str, DataPathModifiers]] = None,
         ignore_cols: Optional[Union[str, Sequence[str]]] = None,
         **kwargs: Any,
@@ -171,14 +179,19 @@
             self._ignore_cols = list(ignore_cols)
 
         for unexpected_kwarg in kwargs:
             logger.warning(f"Ignoring unexpected keyword argument {unexpected_kwarg}")
 
         super().__init__()
 
+    @abstractmethod
+    def get_dtypes(self, **kwargs: Any) -> _Dtypes:
+        """Implement this method to get the columns and column types from dataset."""
+        raise NotImplementedError
+
     def __init_subclass__(cls, **kwargs: Any) -> None:
         if not (inspect.isabstract(cls) or ABC in cls.__bases__):
             cls.get_dtypes = cls._get_dtypes()  # type: ignore[method-assign] # reason: wrap subclass get_dtypes # noqa: B950
             cls.get_column = cls._get_column()  # type: ignore[method-assign] # reason: wrap subclass get_column # noqa: B950
 
     @classmethod
     def _get_dtypes(cls) -> _GetDtypesCallable:
@@ -364,18 +377,14 @@
         return self.data[col_name]
 
     @abstractmethod
     def get_data(self, **kwargs: Any) -> Optional[pd.DataFrame]:
         """Implement this method to load and return dataset."""
         raise NotImplementedError
 
-    def get_dtypes(self, **kwargs: Any) -> _Dtypes:
-        """Get the columns and column types from dataset."""
-        return self._get_data_dtypes(self.data)
-
     def __len__(self) -> int:
         """Get the number of rows in the dataset."""
         return len(self.data)
 
     @property
     def multi_table(self) -> bool:
         """This returns False if the DataSource does not subclass `MultiTableSource`.
@@ -623,26 +632,14 @@
         )
         return col
 
     def _get_column_noniteratively(self, col_name: str, **kwargs: Any) -> _Column:
         """Get column for non-iterable datasource."""
         return self.data[col_name]
 
-    def get_dtypes(self, **kwargs: Any) -> _Dtypes:
-        """Get the columns and column types from dataset.
-
-        Note: iterable=True and iterable=False may return different dtypes for the
-              columns, as with iterable=False we are able to infer pandas dtypes
-              from the whole dataset in one go.
-        """
-        if self.iterable:
-            return self._get_dtypes_iteratively(**kwargs)
-        else:
-            return self._get_dtypes_noniteratively(**kwargs)
-
     def _get_dtypes_iteratively(self, **kwargs: Any) -> _Dtypes:
         """Get dtypes for iterable datasource."""
         dtypes: _Dtypes = {}
 
         # We iterate through each chunk, finding the common type that best
         # expresses the dtype for a column from all the chunks seen so far
         for chunk in self.yield_data(**kwargs):
@@ -675,22 +672,66 @@
         return len(self.data)
 
 
 class MultiProcessingMixIn:
     """MixIn class for multiprocessing of `_get_data`."""
 
     skipped_files: Set[str]
+    data_cache: Optional[DataPersister]
 
     @abstractmethod
     def _get_data(
-        self, file_names: Optional[List[str]] = None, **kwargs: Any
+        self,
+        file_names: Optional[List[str]] = None,
+        use_cache: bool = True,
+        **kwargs: Any,
     ) -> pd.DataFrame:
         ...
 
     @staticmethod
+    def get_num_workers(file_names: List[str]) -> int:
+        """Gets the number of workers to use for multiprocessing.
+
+        Ensures that the number of workers is at least 1 and at most equal to
+        MAX_NUM_MULTIPROCESSING_WORKERS. If the number of files is less than
+        MAX_NUM_MULTIPROCESSING_WORKERS, then we use the number of files as the
+        number of workers. Unless the number of machine cores is also less than
+        MAX_NUM_MULTIPROCESSING_WORKERS, in which case we use the lower of the
+        two.
+
+        Args:
+            file_names: The list of file names to load.
+
+        Returns:
+            The number of workers to use for multiprocessing.
+        """
+        return min(
+            max(1, len(file_names)),
+            # Make sure we don't use all the available cores
+            max(1, psutil.cpu_count(logical=False) - 1),
+            MAX_NUM_MULTIPROCESSING_WORKERS,
+        )
+
+    def use_file_multiprocessing(self, file_names: List[str]) -> bool:
+        """Check if file multiprocessing should be used.
+
+        Returns True if file multiprocessing has been enabled by the environment
+        variable and the number of workers would be greater than 1, otherwise False.
+        There is no need to use file multiprocessing if we are just going to use one
+        worker - it would be slower than just loading the data in the main process.
+
+        Returns:
+            True if file multiprocessing should be used, otherwise False.
+        """
+        # TODO: [BIT-3597] Remove this feature flag
+        if os.environ.get("BITFOUNT_FILE_MULTIPROCESSING_ENABLED"):
+            return self.get_num_workers(file_names) > 1
+        return False
+
+    @staticmethod
     def _mp_configure_listener_logger(log_file_name: str) -> None:
         """Configure the logger for the listener process.
 
         Adds the same handlers as the main process logger to the listener process
         logger. This requires passing the name of the log file to use to the listener
         because otherwise it can't be found because it has a timestamp in the name.
 
@@ -745,46 +786,75 @@
             _logger.addHandler(h)
             _logger.propagate = False
 
     def _mp_worker_get_data_process(
         self,
         queue: Queue,
         file_names: Optional[List[str]] = None,
+        use_cache: bool = True,
         **kwargs: Any,
     ) -> Tuple[pd.DataFrame, List[str]]:
         """Process that calls `_get_data` to load data.
 
         This is called by the main process to load data in parallel. This method
         configures the logger for the worker process and calls `_get_data`.
 
         Args:
             queue: The queue to send log messages to.
             file_names: The list of file names to load.
+            use_cache: Whether the cache should be used to retrieve data for these
+                files. Note that cached data may have some elements, particularly
+                image-related fields such as image data or file paths, replaced
+                with placeholder values when stored in the cache.
+
+                If data_cache is set on the instance, data will be _set_ in the
+                cache, regardless of this argument.
             kwargs: Keyword arguments to pass to `_get_data`.
 
         Returns:
             The loaded data as a dataframe and a list of skipped files. The skipped
             files are returned so that they can be added to the `skipped_files` set
             in the main process - otherwise this information would be lost when the
             worker process is terminated. The skipped files are returned as a list
             rather than a set because sets are not pickleable.
         """
+        logger.debug(f"Using cache: {use_cache}")
         self._mp_configure_worker_logger(queue)
-        data = self._get_data(file_names=file_names, **kwargs)
+        data = self._get_data(file_names=file_names, use_cache=use_cache, **kwargs)
         return data, list(self.skipped_files)
 
-    def _mp_get_data(self, file_names: List[str], **kwargs: Any) -> pd.DataFrame:
+    def _mp_init(self, sqlite_path: Optional[Path]) -> None:
+        """Initialise the multiprocessing environment for loading data.
+
+        This method is called by the worker processes to set up the environment for
+        loading data in parallel. It recreates the data cache if it was set on the
+        instance.
+        """
+        if sqlite_path:
+            logger.debug(f"Recreating data cache from {sqlite_path}.")
+            self.data_cache = SQLiteDataPersister(sqlite_path)
+
+    def _mp_get_data(
+        self, file_names: List[str], use_cache: bool = True, **kwargs: Any
+    ) -> pd.DataFrame:
         """Call `_get_data` in parallel.
 
         This method sets up the multiprocessing queue and processes and calls
         `_get_data` in parallel. It also sets up the listener process to handle log
         messages from the worker processes.
 
         Args:
             file_names: The list of file names to load.
+            use_cache: Whether the cache should be used to retrieve data for these
+                files. Note that cached data may have some elements, particularly
+                image-related fields such as image data or file paths, replaced
+                with placeholder values when stored in the cache.
+
+                If data_cache is set on the instance, data will be _set_ in the
+                cache, regardless of this argument.
             kwargs: Keyword arguments to pass to `_get_data`.
 
         Returns:
             The loaded data as a dataframe.
         """
         from concurrent.futures import Future, ProcessPoolExecutor, as_completed
         from multiprocessing import Manager, Process
@@ -800,37 +870,49 @@
 
         if not log_file_name:
             # If there is no file handler, then there is no need for this message
             # to be logged any higher than debug anyway
             logger.debug("No existing file handler found for logger.")
 
         try:
+            # Set environment variable to indicate that the spawned processes are
+            # child processes since they will inherit the environment from the parent
+            os.environ["_BITFOUNT_CHILD_PROCESS"] = "True"
+
+            # Initialization must be done before creating the process
+            data_cache_sqlite_path: Optional[Path] = None
+            data_cache: Optional[DataPersister] = self.data_cache
+            if self.data_cache and isinstance(self.data_cache, SQLiteDataPersister):
+                data_cache_sqlite_path = self.data_cache._sqlite_path
+                # TODO: [BIT-3723] There may be a better way to pass the data cache to
+                # the worker processes by disposing of the connection pool rather than
+                # having to recreate the cache in each worker process
+                self.data_cache = None
+
             log_queue = Manager().Queue(-1)
             log_listener = Process(
                 target=self._mp_listener_process, args=(log_queue, log_file_name)
             )
             log_listener.start()
 
-            # Ensure that the number of workers is at least 1 and at most equal to
-            # MAX_NUM_MULTIPROCESSING_WORKERS. If the number of files is less than
-            # MAX_NUM_MULTIPROCESSING_WORKERS, then we use the number of files as the
-            # number of workers. Unless the number of machine cores is also less than
-            # MAX_NUM_MULTIPROCESSING_WORKERS, in which case we use the lower of the
-            # two.
-            max_workers = min(
-                max(1, len(file_names)),
-                # Make sure we don't use all the available cores
-                max(1, psutil.cpu_count(logical=False) - 1),
-                MAX_NUM_MULTIPROCESSING_WORKERS,
-            )
+            # Create a pool of worker processes
+            max_workers = self.get_num_workers(file_names)
             logger.info(f"Multiprocessing max workers: {max_workers}")
-            executor = ProcessPoolExecutor(max_workers=max_workers)
+            executor = ProcessPoolExecutor(
+                max_workers=max_workers,
+                initializer=self._mp_init,
+                initargs=(data_cache_sqlite_path,),
+            )
             futures: List[Future] = [
                 executor.submit(
-                    self._mp_worker_get_data_process, log_queue, [i], **kwargs
+                    self._mp_worker_get_data_process,
+                    log_queue,
+                    [i],
+                    use_cache,
+                    **kwargs,
                 )
                 for i in file_names
             ]
 
             total_num_files = len(file_names)
             dfs: List[pd.DataFrame] = []
             # Wait for the results to come in one by one as they complete
@@ -842,15 +924,26 @@
                         file_num=i + 1,
                         total_num_files=total_num_files,
                     )
                 data, skipped_files = future.result()
                 self.skipped_files.update(set(cast(List[str], skipped_files)))
                 dfs.append(cast(pd.DataFrame, data))
 
+            logger.debug("Finished loading data in parallel using multiprocessing.")
         finally:
+            logger.debug("Cleaning up multiprocessing environment.")
+
+            # Reset environment variable to indicate that this is not a child process
+            os.environ["_BITFOUNT_CHILD_PROCESS"] = "False"
+
+            # Reset the data cache if it was set in the first place
+            if data_cache:
+                logger.debug("Reverting data cache to original state.")
+                self.data_cache = data_cache
+
             log_queue.put_nowait(None)  # Send sentinel to tell listener to quit
             # Wait for listener to quit. Must be done before terminating the process
             # to ensure all the log messages continue to get processed
             log_listener.join()
             # Terminate listener process
             log_listener.terminate()
 
@@ -1028,15 +1121,15 @@
         """
         return Path(self._unsanitized_path).absolute().resolve()
 
     @property
     def _sampled_data(self) -> pd.DataFrame:
         """Subset of data, as loaded by fast load."""
         if self._sampled_data_priv is None:
-            self._fast_load_data()
+            self._fast_load_data(use_cache=False)
         # We can make this cast as the above `is None` check causes data to be loaded
         return cast(pd.DataFrame, self._sampled_data_priv)
 
     @_sampled_data.setter
     def _sampled_data(self, data: pd.DataFrame) -> None:
         """Setter for sampled data."""
         self._sampled_data_priv = data
@@ -1194,14 +1287,15 @@
         )
         if ignored_file_types:
             logger.info(
                 f"Ignoring {number_of_ignored_files} files with file types "
                 f"{ignored_file_types}."
             )
 
+        # TODO: [BIT-3721] Move this sorting by hash to `file_names` property
         # Fix for shuffling so that data is mapped correctly
         matched_files.sort(key=lambda x: hash(x))
         return [str(x.resolve()) for x in matched_files]
 
     @staticmethod
     def _get_date_from_date_components(
         cutoff_type: Literal["creation", "modification"],
@@ -1482,15 +1576,18 @@
                 "consecutive files without finding new fields."
             )
 
         # Save onto _sampled_data, not main `.data`
         self._sampled_data = pd.concat(dfs, axis=0, ignore_index=True)
 
     def get_data(
-        self, file_names: Optional[List[str]] = None, **kwargs: Any
+        self,
+        file_names: Optional[List[str]] = None,
+        use_cache: bool = True,
+        **kwargs: Any,
     ) -> Optional[pd.DataFrame]:
         """Returns data if the datasource is not iterable, otherwise None.
 
         We don't reload the data if it has already been loaded. We are assuming that
         files are only added, not removed, meaning we can rely on simply matching the
         number of files detected with the length of the dataframe to ascertain whether
         the data has already been loaded.
@@ -1511,70 +1608,82 @@
         for hook in get_hooks(HookType.POD):
             # Signal file processing start
             hook.on_file_process_start(
                 self, file_num=0, total_num_files=len(file_names)
             )
 
         if len(file_names) == 1:
-            result = self._get_data(file_names=file_names, **kwargs)
+            result = self._get_data(
+                file_names=file_names, use_cache=use_cache, **kwargs
+            )
             for hook in get_hooks(HookType.POD):
                 hook.on_file_process_end(self, file_num=1, total_num_files=1)
 
             return result
 
-        # TODO: [BIT-3597] Remove this feature flag and the corresponding
-        # `else` block.
-        if os.environ.get("BITFOUNT_FILE_MULTIPROCESSING_ENABLED"):
-            return self._mp_get_data(file_names, **kwargs)
+        if self.use_file_multiprocessing(file_names):
+            return self._mp_get_data(file_names, use_cache=use_cache, **kwargs)
         else:
             dfs = []
             for idx, file_name in enumerate(file_names):
-                dfs.append(self._get_data([file_name], **kwargs))
+                dfs.append(self._get_data([file_name], use_cache=use_cache, **kwargs))
                 for hook in get_hooks(HookType.POD):
                     hook.on_file_process_end(
                         self,
                         file_num=idx + 1,
                         total_num_files=len(file_names),
                     )
 
             return pd.concat(dfs, axis=0, ignore_index=True) if dfs else pd.DataFrame()
 
     @abstractmethod
     def _get_data(
         self,
         file_names: Optional[List[str]] = None,
+        use_cache: bool = True,
         **kwargs: Any,
     ) -> pd.DataFrame:
         """Implement to return data corresponding to the provided file names.
 
         This method is called under the hood by `get_data` and `yield_data`. This
         method must return a dataframe with the columns `_original_filename` and
         `_last_modified` containing the original file name of each row, and the
         timestamp when the file was last modified in ISO 8601 format, respectively.
 
         Args:
             file_names: List of file names to load. If None, all files should be
                 loaded.
+            use_cache: Whether the cache should be used to retrieve data for these
+                files. Note that cached data may have some elements, particularly
+                image-related fields such as image data or file paths, replaced
+                with placeholder values when stored in the cache.
+
+                If data_cache is set on the instance, data will be _set_ in the
+                cache, regardless of this argument.
 
         Returns:
             A dataframe containing the data.
         """
         raise NotImplementedError
 
     def yield_data(
-        self, file_names: Optional[List[str]] = None, **kwargs: Any
+        self,
+        file_names: Optional[List[str]] = None,
+        use_cache: bool = True,
+        **kwargs: Any,
     ) -> Iterator[pd.DataFrame]:
         """Yields data in batches from files that match the given file names.
 
         Args:
             file_names: An optional list of file names to use for yielding data.
                 Otherwise, all files that have already been found will be used.
                 `file_names` is always provided when this method is called from the
                 Dataset as part of a task.
 
+
         Raises:
             ValueError: If no file names provided and no files have been found.
         """
         if not file_names and not self.file_names:
             logger.warning("No files found to yield data from.")
             # if there are no files, log a warning, and yield an empty dataframe
             yield pd.DataFrame()
@@ -1584,20 +1693,22 @@
 
         for idx, file_names_partition in enumerate(
             self.partition(file_names_, self.partition_size)
         ):
             try:
                 file_names_partition = cast(List[str], file_names_partition)
                 logger.debug(f"Yielding partition {idx} from {self}")
-                # TODO: [BIT-3597] Remove this feature flag and the corresponding
-                # `else` block.
-                if os.environ.get("BITFOUNT_FILE_MULTIPROCESSING_ENABLED"):
-                    yield self._mp_get_data(file_names_partition, **kwargs)
+                if self.use_file_multiprocessing(file_names_partition):
+                    yield self._mp_get_data(
+                        file_names_partition, use_cache=use_cache, **kwargs
+                    )
                 else:
-                    yield self._get_data(file_names_partition, **kwargs)
+                    yield self._get_data(
+                        file_names_partition, use_cache=use_cache, **kwargs
+                    )
                     file_num = idx * self.partition_size + len(file_names_partition)
                     for hook in get_hooks(HookType.POD):
                         hook.on_file_process_end(
                             self,
                             file_num=file_num,
                             total_num_files=len(file_names_),
                         )
@@ -1712,14 +1823,15 @@
 
         return self.data[col_name]
 
     def _get_column_fast_load(self, col_name: str, **kwargs: Any) -> _Column:
         """Get column for fast-load datasource."""
         return self._sampled_data[col_name]
 
+    @methodtools.lru_cache(maxsize=1)
     def get_dtypes(self, **kwargs: Any) -> _Dtypes:
         """Loads and returns the column names and types of the dataframe.
 
         If `fast_load` is set to True and the data is stale, only the first file will
         be loaded to get the column names and types. Otherwise, all files will be
         loaded. We only perform this optimisation if the data is stale because if it's
         not, it's faster to just return the dtypes of the already loaded data.
@@ -1728,21 +1840,19 @@
             **kwargs: Additional keyword arguments to pass to the `load_data` method
                 if the data is stale.
 
         Returns:
             A mapping from column names to column types.
         """
         if self.fast_load:
-            if self.stale:
-                data = self._get_data(file_names=[self.file_names[0]], **kwargs)
-                return self._get_data_dtypes(data)
-            else:
-                return self._get_data_dtypes(self._sampled_data)
+            return self._get_data_dtypes(self._sampled_data)
+        elif self.iterable:
+            return self._get_dtypes_iteratively(**kwargs)
         else:
-            return super().get_dtypes(**kwargs)
+            return self._get_dtypes_noniteratively(**kwargs)
 
     def _get_dtypes_noniteratively(self, **kwargs: Any) -> _Dtypes:
         """Get dtypes non-iteratively, loading data if it is stale."""
         if self.stale:
             self.load_data(**kwargs)
 
         return self._get_data_dtypes(self.data)
```

### Comparing `bitfount-0.9.4/bitfount/data/datasources/csv_source.py` & `bitfount-0.9.5/bitfount/data/datasources/csv_source.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/database_source.py` & `bitfount-0.9.5/bitfount/data/datasources/database_source.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/dataframe_source.py` & `bitfount-0.9.5/bitfount/data/datasources/dataframe_source.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/dicom_source.py` & `bitfount-0.9.5/bitfount/data/datasources/dicom_source.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/empty_source.py` & `bitfount-0.9.5/bitfount/data/datasources/empty_source.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/excel_source.py` & `bitfount-0.9.5/bitfount/data/datasources/excel_source.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/types.py` & `bitfount-0.9.5/bitfount/data/datasources/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/utils.py` & `bitfount-0.9.5/bitfount/data/datasources/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/view_configs.py` & `bitfount-0.9.5/bitfount/data/datasources/view_configs.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasources/views.py` & `bitfount-0.9.5/bitfount/data/datasources/views.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datasplitters.py` & `bitfount-0.9.5/bitfount/data/datasplitters.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/datastructure.py` & `bitfount-0.9.5/bitfount/data/datastructure.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/exceptions.py` & `bitfount-0.9.5/bitfount/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/helper.py` & `bitfount-0.9.5/bitfount/data/helper.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/huggingface/datafactory.py` & `bitfount-0.9.5/bitfount/data/huggingface/datafactory.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/huggingface/dataloaders.py` & `bitfount-0.9.5/bitfount/data/huggingface/dataloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """HuggingFace compatible dataloaders."""
+
+from __future__ import annotations
+
 import math
 import random
 import secrets
 from typing import Any, Iterator, List, Union, cast
 
 import numpy as np
-import torch
-from torch.utils.data import DataLoader as PyTorchDataLoader
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import torch
+    from torch.utils.data import DataLoader as PyTorchDataLoader
 
 from bitfount.backends.pytorch import DEFAULT_BUFFER_SIZE
 from bitfount.backends.pytorch.data.utils import _convert_batch_to_tensor
 from bitfount.data.dataloaders import BitfountDataLoader
 from bitfount.data.datasets import _IterableBitfountDataset
 from bitfount.data.huggingface.datasets import (
     _HuggingFaceDataset,
@@ -63,15 +70,15 @@
     """
 
     def __init__(
         self,
         dataset: Union[_HuggingFaceDataset, _IterableHuggingFaceDataset],
         batch_size: int = 1,
         shuffle: bool = False,
-        **kwargs: Any
+        **kwargs: Any,
     ):
         self.dataset = cast(_HuggingFaceDataset, dataset)
         super().__init__(dataset=dataset, batch_size=batch_size, shuffle=shuffle)
         self.dataloader = self.get_pytorch_dataloader()
 
     def get_pytorch_dataloader(self, **kwargs: Any) -> PyTorchDataLoader:
         """Return a PyTorch DataLoader for `self.dataset`.
@@ -111,15 +118,15 @@
 
     def __init__(
         self,
         dataset: _IterableBitfountDataset,
         batch_size: int = 1,
         shuffle: bool = False,
         secure_rng: bool = False,
-        **kwargs: Any
+        **kwargs: Any,
     ):
         # _PytorchIterableDataset is a wrapper around of
         # _IterableBitfountDataset so this cast is safe.
         dataset = cast(_IterableHuggingFaceDataset, dataset)
         super().__init__(dataset=dataset, batch_size=batch_size, shuffle=shuffle)
         self.secure_rng = secure_rng
         self.batch_size = batch_size
```

### Comparing `bitfount-0.9.4/bitfount/data/huggingface/datasets.py` & `bitfount-0.9.5/bitfount/data/huggingface/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Hugging Face Datasets."""
 
+from __future__ import annotations
+
 from typing import Any, Iterator, Mapping, Optional, Sequence, Tuple, Union, cast
 
 import numpy as np
 import pandas as pd
-import torch
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import torch
 
 from bitfount.data.datasets import (
     _BaseBitfountDataset,
     _BitfountDataset,
     _FileSystemBitfountDataset,
     _FileSystemIterableBitfountDataset,
     _IterableBitfountDataset,
```

### Comparing `bitfount-0.9.4/bitfount/data/huggingface/utils.py` & `bitfount-0.9.5/bitfount/data/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/persistence/base.py` & `bitfount-0.9.5/bitfount/data/persistence/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base interface for data persistence implementations."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 import logging
 from pathlib import Path
 from typing import TYPE_CHECKING
 
@@ -10,14 +11,15 @@
 
 if TYPE_CHECKING:
     from typing import Collection, Final, Optional, Union
 
 
 _IMAGE_COL_PLACEHOLDER: Final = "<Image Data or File Path>"
 
+
 _logger = logging.getLogger(__name__)
 
 
 class DataPersister(ABC):
     """Abstract interface for data persistence/caching implementations."""
 
     def get(self, file: Union[str, Path]) -> Optional[pd.DataFrame]:
```

### Comparing `bitfount-0.9.4/bitfount/data/persistence/sqlite.py` & `bitfount-0.9.5/bitfount/data/persistence/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A data persistance implementation backed by an SQLite database."""
+
 from __future__ import annotations
 
 from datetime import datetime
 import logging
 import os.path
 from pathlib import Path
 from typing import Any, Optional, Set, Type, Union
```

### Comparing `bitfount-0.9.4/bitfount/data/schema.py` & `bitfount-0.9.5/bitfount/data/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes concerning data schemas."""
+
 from __future__ import annotations
 
 import collections
 import contextlib
 import copy
 import logging
 from os import PathLike
```

### Comparing `bitfount-0.9.4/bitfount/data/types.py` & `bitfount-0.9.5/bitfount/data/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/data/utils.py` & `bitfount-0.9.5/bitfount/data/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/exceptions.py` & `bitfount-0.9.5/bitfount/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/__init__.py` & `bitfount-0.9.5/bitfount/federated/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/aggregators/__init__.py` & `bitfount-0.9.5/bitfount/federated/aggregators/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/aggregators/aggregator.py` & `bitfount-0.9.5/bitfount/federated/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/aggregators/base.py` & `bitfount-0.9.5/bitfount/federated/aggregators/base.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/aggregators/secure.py` & `bitfount-0.9.5/bitfount/federated/aggregators/secure.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/__init__.py` & `bitfount-0.9.5/bitfount/federated/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/base.py` & `bitfount-0.9.5/bitfount/federated/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/column_avg.py` & `bitfount-0.9.5/bitfount/federated/algorithms/column_avg.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/compute_intersection_rsa.py` & `bitfount-0.9.5/bitfount/federated/algorithms/compute_intersection_rsa.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/csv_report_algorithm.py` & `bitfount-0.9.5/bitfount/federated/algorithms/csv_report_algorithm.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_image_classification.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_image_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """Hugging Face Image Classification Algorithm."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Mapping, Optional
 
 from marshmallow import fields
 import pandas as pd
-import torch
-from transformers import AutoImageProcessor, AutoModelForImageClassification, set_seed
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import torch
+    from transformers import (
+        AutoImageProcessor,
+        AutoModelForImageClassification,
+        set_seed,
+    )
 
 from bitfount.data.huggingface.utils import get_data_factory_dataset
 from bitfount.data.types import DataSplit, _SemanticTypeValue
 from bitfount.federated.algorithms.base import (
     BaseAlgorithmFactory,
     BaseModellerAlgorithm,
     BaseWorkerAlgorithm,
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_image_segmentation.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_image_segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 
 import PIL
 import cv2  # type: ignore[import] # Reason: No Stubs for module
 from marshmallow import fields
 from marshmallow.validate import OneOf
 import numpy as np
 import pandas as pd
-import torch
-from transformers import AutoImageProcessor, AutoModelForImageSegmentation, set_seed
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import torch
+    from transformers import AutoImageProcessor, AutoModelForImageSegmentation, set_seed
 
 from bitfount.config import BITFOUNT_OUTPUT_DIR
 from bitfount.data.datasources.base_source import BaseSource, FileSystemIterableSource
 from bitfount.data.datasources.utils import ORIGINAL_FILENAME_METADATA_COLUMN
 from bitfount.data.datasources.views import _DataViewFromFileIterableSource
 from bitfount.data.huggingface.utils import get_data_factory_dataset
 from bitfount.data.types import DataSplit, _SemanticTypeValue
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_perplexity.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_perplexity.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 Reference:
 https://huggingface.co/docs/transformers/perplexity#example-calculating-perplexity-with-gpt2-in-transformers
 """
 from typing import Any, ClassVar, Dict, Mapping, Optional
 
 from marshmallow import fields
 import pandas as pd
-import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer, set_seed
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import torch
+    from transformers import AutoModelForCausalLM, AutoTokenizer, set_seed
 
 from bitfount.data.datasources.base_source import BaseSource
 from bitfount.federated.algorithms.base import (
     BaseAlgorithmFactory,
     BaseModellerAlgorithm,
     BaseWorkerAlgorithm,
 )
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_text_classification.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_text_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,20 @@
     Optional,
     Union,
 )
 
 from marshmallow import fields
 import numpy as np
 import pandas as pd
-import torch
-from transformers import AutoModelForSequenceClassification, AutoTokenizer, set_seed
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import torch
+    from transformers import AutoModelForSequenceClassification, AutoTokenizer, set_seed
 
 from bitfount.data.datasources.base_source import BaseSource
 from bitfount.data.huggingface.utils import get_data_factory_dataset
 from bitfount.data.types import DataSplit, _SemanticTypeValue
 from bitfount.federated.algorithms.base import (
     BaseAlgorithmFactory,
     BaseModellerAlgorithm,
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_text_generation.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_text_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hugging Face Text Generation Algorithm."""
+
 from __future__ import annotations
 
 from functools import partial
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
@@ -12,16 +13,29 @@
     Optional,
     Union,
     overload,
 )
 
 from marshmallow import fields
 import pandas as pd
-import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer, pipeline, set_seed
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import torch
+    from transformers import AutoModelForCausalLM, AutoTokenizer, pipeline, set_seed
+
+    # This is currently semi-duplicated from `bitfount.backends.pytorch.utils` as it is
+    # not possible to import it from there without creating a circular dependency.
+    _TORCH_DTYPES: Dict[str, torch.dtype] = {
+        "bfloat16": torch.bfloat16,
+        "float16": torch.float16,
+        "float32": torch.float32,
+        "float64": torch.float64,
+    }
 
 from bitfount.config import BITFOUNT_DEFAULT_TORCH_DEVICE
 from bitfount.data.datasources.base_source import BaseSource
 from bitfount.federated.algorithms.base import (
     BaseAlgorithmFactory,
     BaseModellerAlgorithm,
     BaseWorkerAlgorithm,
@@ -30,22 +44,14 @@
 from bitfount.federated.types import TextGenerationDefaultReturnType
 from bitfount.types import T_FIELDS_DICT
 from bitfount.utils import DEFAULT_SEED, delegates
 
 if TYPE_CHECKING:
     from bitfount.federated.privacy.differential import DPPodConfig
 
-# This is currently semi-duplicated from `bitfount.backends.pytorch.utils` as it is not
-# possible to import it from there without creating a circular dependency.
-_TORCH_DTYPES: Dict[str, torch.dtype] = {
-    "bfloat16": torch.bfloat16,
-    "float16": torch.float16,
-    "float32": torch.float32,
-    "float64": torch.float64,
-}
 
 DEFAULT_MAX_LENGTH = 50
 DEFAULT_NUM_RETURN_SEQUENCES = 1
 DEFAULT_MIN_NEW_TOKENS = 1
 DEFAULT_REPETITION_PENALTY = 1.0
 DEFAULT_NUM_BEAMS = 1
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_zero_shot_image_classification.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/hugging_face_zero_shot_image_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,25 @@
     Optional,
     Union,
     cast,
 )
 
 from marshmallow import fields
 import pandas as pd
-from transformers import (
-    AutoImageProcessor,
-    AutoModelForZeroShotImageClassification,
-    AutoTokenizer,
-    pipeline,
-    set_seed,
-)
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    from transformers import (
+        AutoImageProcessor,
+        AutoModelForZeroShotImageClassification,
+        AutoTokenizer,
+        pipeline,
+        set_seed,
+    )
 
 from bitfount.data.datasources.base_source import BaseSource
 from bitfount.federated.algorithms.base import (
     BaseAlgorithmFactory,
     BaseModellerAlgorithm,
     BaseWorkerAlgorithm,
 )
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/timm_fine_tuning.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/timm_fine_tuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,65 @@
 """HuggingFace TIMM fine-tuning Algorithm.
 
 Borrowed with permission from https://github.com/huggingface/pytorch-image-models.
 Copyright 2020 Ross Wightman (https://github.com/rwightman)
 """
+
 from contextlib import suppress
 from dataclasses import asdict
 from functools import partial
 import logging
 import os
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, Literal, Mapping, Optional, Union
 import warnings
 
 import desert
 from marshmallow import fields
 from marshmallow.validate import OneOf
-from timm import utils as timm_utils
-from timm.data import Mixup
-from timm.layers import convert_splitbn_model, convert_sync_batchnorm, set_fast_norm
-from timm.loss import (
-    BinaryCrossEntropy,
-    JsdCrossEntropy,
-    LabelSmoothingCrossEntropy,
-    SoftTargetCrossEntropy,
-)
-from timm.models import create_model, safe_model_name
-from timm.optim import create_optimizer_v2, optimizer_kwargs
-from timm.scheduler import create_scheduler_v2, scheduler_kwargs
-from timm.utils import ApexScaler, NativeScaler
-import torch
-import torch.nn as nn
-from torch.nn.parallel import DistributedDataParallel as NativeDDP
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    from timm import utils as timm_utils
+    from timm.data import Mixup
+    from timm.layers import convert_splitbn_model, convert_sync_batchnorm, set_fast_norm
+    from timm.loss import (
+        BinaryCrossEntropy,
+        JsdCrossEntropy,
+        LabelSmoothingCrossEntropy,
+        SoftTargetCrossEntropy,
+    )
+    from timm.models import create_model, safe_model_name
+    from timm.optim import create_optimizer_v2, optimizer_kwargs
+    from timm.scheduler import create_scheduler_v2, scheduler_kwargs
+    from timm.utils import ApexScaler, NativeScaler
+    import torch
+    import torch.nn as nn
+    from torch.nn.parallel import DistributedDataParallel as NativeDDP
+
+    try:
+        from apex import amp
+        from apex.parallel import (
+            DistributedDataParallel as ApexDDP,
+            convert_syncbn_model,
+        )
+
+        has_apex = True
+    except ImportError:
+        has_apex = False
+
+    try:
+        if torch.cuda.amp.autocast is not None:
+            has_native_amp = True
+    except AttributeError:
+        has_native_amp = False
+
+    has_compile = hasattr(torch, "compile")
+
 import yaml
 
 from bitfount.config import BITFOUNT_OUTPUT_DIR
 from bitfount.data.databunch import BitfountDataBunch
 from bitfount.data.datasources.base_source import BaseSource
 from bitfount.data.datastructure import (
     DEFAULT_IMAGE_TRANSFORMATIONS,
@@ -57,30 +82,14 @@
 from bitfount.federated.logging import _get_federated_logger
 from bitfount.federated.privacy.differential import DPPodConfig
 from bitfount.hooks import HookType, get_hooks
 from bitfount.runners.utils import setup_loggers
 from bitfount.types import T_FIELDS_DICT, T_NESTED_FIELDS, _JSONDict
 from bitfount.utils import delegates
 
-try:
-    from apex import amp
-    from apex.parallel import DistributedDataParallel as ApexDDP, convert_syncbn_model
-
-    has_apex = True
-except ImportError:
-    has_apex = False
-
-try:
-    if torch.cuda.amp.autocast is not None:
-        has_native_amp = True
-except AttributeError:
-    has_native_amp = False
-
-has_compile = hasattr(torch, "compile")
-
 logger = _get_federated_logger(__name__)
 
 # Enable logging for timm checkpoint saver
 timm_logger = logging.getLogger("timm.utils.checkpoint_saver")
 setup_loggers([timm_logger])
 _TimmBatchTransformationStep = Literal["train", "validation"]
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/timm_inference.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/timm_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 Adapted from: https://github.com/huggingface/api-inference-community/
 """
 import os
 from typing import Any, ClassVar, Dict, List, Mapping, Optional, Union
 
 from marshmallow import fields
 import pandas as pd
-import timm
-from timm.data import (
-    CustomDatasetInfo,
-    ImageNetInfo,
-    create_transform,
-    infer_imagenet_subset,
-    resolve_model_data_config,
-)
-import torch
+
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import timm
+    from timm.data import (
+        CustomDatasetInfo,
+        ImageNetInfo,
+        create_transform,
+        infer_imagenet_subset,
+        resolve_model_data_config,
+    )
+    import torch
 
 from bitfount.data.datasources.base_source import BaseSource
 from bitfount.data.datastructure import DEFAULT_IMAGE_TRANSFORMATIONS
 from bitfount.data.huggingface.utils import get_data_factory_dataset
 from bitfount.data.types import DataSplit, _SemanticTypeValue
 from bitfount.federated.algorithms.base import (
     BaseAlgorithmFactory,
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/hugging_face_algorithms/utils.py` & `bitfount-0.9.5/bitfount/federated/algorithms/hugging_face_algorithms/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 from contextlib import AbstractContextManager, suppress
 from dataclasses import dataclass, field
 import logging
 import os
 import time
 from typing import Any, Dict, List, Literal, Optional, Tuple
 
-from timm import utils
-from timm.data import Mixup
-from timm.models import model_parameters
-from timm.utils import ApexScaler
-import torch
-import torch.nn as nn
-from torch.utils.data import DataLoader
-import torchvision.utils
+from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    from timm import utils
+    from timm.data import Mixup
+    from timm.models import model_parameters
+    from timm.utils import ApexScaler
+    import torch
+    import torch.nn as nn
+    from torch.utils.data import DataLoader
+    import torchvision.utils
 
 from bitfount.transformations.base_transformation import Transformation
 from bitfount.transformations.parser import TransformationsParser
 from bitfount.types import _JSONDict
 
 _logger = logging.getLogger(__name__)
```

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/base.py` & `bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/base.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/evaluate.py` & `bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/evaluate.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/federated_training.py` & `bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/federated_training.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/inference.py` & `bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/inference.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/model_algorithms/train_and_evaluate.py` & `bitfount-0.9.5/bitfount/federated/algorithms/model_algorithms/train_and_evaluate.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/private_sql_query.py` & `bitfount-0.9.5/bitfount/federated/algorithms/private_sql_query.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/algorithms/sql_query.py` & `bitfount-0.9.5/bitfount/federated/algorithms/sql_query.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/authorisation_checkers.py` & `bitfount-0.9.5/bitfount/federated/authorisation_checkers.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/early_stopping.py` & `bitfount-0.9.5/bitfount/federated/early_stopping.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/encryption.py` & `bitfount-0.9.5/bitfount/federated/encryption.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/exceptions.py` & `bitfount-0.9.5/bitfount/federated/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/helper.py` & `bitfount-0.9.5/bitfount/federated/helper.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/keys_setup.py` & `bitfount-0.9.5/bitfount/federated/keys_setup.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/logging.py` & `bitfount-0.9.5/bitfount/federated/logging.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/mixins.py` & `bitfount-0.9.5/bitfount/federated/mixins.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/model_reference.py` & `bitfount-0.9.5/bitfount/federated/model_reference.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/modeller.py` & `bitfount-0.9.5/bitfount/federated/modeller.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/monitoring/__init__.py` & `bitfount-0.9.5/bitfount/federated/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/monitoring/decorators.py` & `bitfount-0.9.5/bitfount/federated/monitoring/decorators.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/monitoring/exceptions.py` & `bitfount-0.9.5/bitfount/federated/monitoring/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/monitoring/monitor.py` & `bitfount-0.9.5/bitfount/federated/monitoring/monitor.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/monitoring/types.py` & `bitfount-0.9.5/bitfount/federated/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/pod.py` & `bitfount-0.9.5/bitfount/federated/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pods for responding to tasks."""
+
 import asyncio
 from contextlib import nullcontext
 from dataclasses import dataclass
 import os
 import threading
 from typing import (
     Any,
@@ -301,14 +302,32 @@
             datasource=datasource,
             pod_name=name,
             datasource_details=self._pod_details_config,
             data_config=data_config,
             schema=schema,
         )
 
+        # Establish Bitfount Hub and access manager connection details
+        for hook in get_hooks(HookType.POD):
+            hook.on_pod_init_progress(self, "Establishing connection with Hub")
+
+        self._hub = (
+            hub
+            if hub is not None
+            else _create_bitfounthub(username=username, secrets=secrets)
+        )
+        self._session = self._hub.session
+        self._access_manager = (
+            access_manager
+            if access_manager is not None
+            else _create_access_manager(self._session)
+        )
+        self._access_manager_public_key = self._access_manager.get_access_manager_key()
+
+        # Start processing dataset configurations
         for hook in get_hooks(HookType.POD):
             hook.on_pod_init_progress(
                 self,
                 "Processed configurations",
                 base_datasource_names=list(ds.name for ds in base_datasource_configs),
                 views_datasource_names=list(ds.name for ds in view_datasource_configs),
                 pod_db_enabled=False if self.pod_db_connector is None else True,
@@ -366,31 +385,14 @@
 
         self.show_datapoints_with_results_in_db = (
             show_datapoints_with_results_in_db
             if self.pod_db_connector is not None
             else False
         )
 
-        # Establish Bitfount Hub and access manager connection details
-        for hook in get_hooks(HookType.POD):
-            hook.on_pod_init_progress(self, "Establishing connection with Hub")
-
-        self._hub = (
-            hub
-            if hub is not None
-            else _create_bitfounthub(username=username, secrets=secrets)
-        )
-        self._session = self._hub.session
-        self._access_manager = (
-            access_manager
-            if access_manager is not None
-            else _create_access_manager(self._session)
-        )
-        self._access_manager_public_key = self._access_manager.get_access_manager_key()
-
         # Get RSA keys for pod
         self.private_key, self.pod_public_key = self._get_default_pod_keys(pod_keys)
 
         # Establish identifiers for pod and datasets
         # and ensure these are added to the auto-approved "pods" list
         self.pod_identifier = f"{self._session.username}/{self.name}"  # TODO: [NO_TICKET: Temporary] maybe need to get rid of this, at least inside Workers? # noqa: B950
         dataset_identifiers = [
@@ -490,14 +492,17 @@
         # Load existing schemas if needed
         schema: Optional[BitfountSchema] = None
         if ds.schema:
             if isinstance(ds.schema, BitfountSchema):
                 schema = ds.schema
             else:
                 schema = BitfountSchema.load_from_file(ds.schema)
+        # TODO: [BIT-3720] Consider calling `get_pod_schema` to retrieve the schema
+        # from the hub if it's not provided
+
         # Validate database connection if exists
         if isinstance(ds.datasource, DatabaseSource):
             ds.datasource.validate()
 
         # Check if we need to update the provided schema. This may be needed if:
         #   - the datasource is multi-table and references tables not in the schema
         #   - auto-tidy is requested
@@ -633,56 +638,64 @@
         pod_name: str,
         pod_db_connector: Optional[PodDbConnector] = None,
         schema: Optional[BitfountSchema] = None,
     ) -> BitfountSchema:
         """Generate pod schema."""
         logger.info(f"Generating schema for {datasource_name}...")
         # Create schema if not provided
-        if not schema:
+        if schema:
+            schema.unfreeze()
+        else:
+            logger.debug("No existing schema provided, generating schema...")
             schema = BitfountSchema()
         if not pod_db_connector:
+            logger.debug("No pod database, generating schema from datasource...")
             datasource.load_data()
 
             # Check if we need to auto-tidy
             if data_config.auto_tidy and datasource.multi_table:
                 logger.warning("Can't autotidy multi-table data.")
             elif datasource.iterable:
                 # TODO: [BIT-3486] Do we need to do batch-level tidying?
-                logger.warning("Can't autotidy to iterable datasource.")
+                logger.warning("Can't autotidy iterable datasource.")
             elif data_config.auto_tidy:
                 clean_data = CleanDataTransformation()
                 # Normalization is applied to all float columns if `auto-tidy` is true
                 normalize = NormalizeDataTransformation()
                 processor = TransformationProcessor(
                     [clean_data, normalize],
                 )
                 datasource.data = processor.transform(datasource.data)
             # Add BaseSource to schema again because features will have changed by
             # auto-tidying
+            logger.debug("Adding datasource tables to schema...")
             schema.add_datasource_tables(
                 datasource=datasource,
                 table_name=datasource_name,
                 table_descriptions=data_config.table_descriptions,
                 column_descriptions=data_config.column_descriptions,
                 ignore_cols=data_config.ignore_cols,
                 force_stypes=data_config.force_stypes,
             )
         else:
+            logger.debug("Pod database exists, generating schema from database...")
             if datasource.multi_table:
                 schema_tables = cast(MultiTableSource, datasource).table_names
             else:
                 schema_tables = [datasource_name]
+            logger.debug("Adding datasource tables to schema...")
             schema.add_tables_from_pod_database(
                 pod_db_connector=pod_db_connector,
                 pod_name=pod_name,
                 datasource_tables=schema_tables,
                 ignore_cols=data_config.ignore_cols,
                 force_stypes=data_config.force_stypes,
             )
         # Freeze schema
+        logger.debug("Freezing schema...")
         schema.freeze()
         return schema
 
     def _get_default_pod_details_config(
         self, name: Optional[str] = None
     ) -> PodDetailsConfig:
         """Get default pod details config."""
@@ -1039,14 +1052,15 @@
                 if worker_mailbox.task_id:
                     logger.error(
                         f"Exception whilst running task {worker_mailbox.task_id}."
                     )
                 else:
                     logger.error("Exception whilst running task.")
             finally:
+                logger.debug("Updating pod database and schemas.")
                 worker_datasource.is_task_running = False
                 # Find the underlying datasource that was used in the task and update it
                 # if it is a FileSystemIterableSource or a view datasource with a
                 # FileSystemIterableSource as its base.
                 base_source_name: str = ""
                 if isinstance(worker_datasource, FileSystemIterableSource):
                     base_source_name = worker_datasource_name
@@ -1097,14 +1111,15 @@
                             if (
                                 isinstance(view.datasource, ViewDatasourceConfig)
                                 and view.datasource.source_dataset_name == source_name
                             ):
                                 self._update_schema(view.name, is_view=True)
 
             # Run post-task hooks
+            logger.debug("Running post-task hooks.")
             for hook in get_hooks(HookType.POD):
                 hook.on_task_end(self, task_id=worker_mailbox.task_id)
 
         logger.info("Ready for next task...")
 
     def _update_schema(self, datasource_name: str, is_view: bool) -> None:
         """Updates the schema corresponding to the given datasource name.
@@ -1122,14 +1137,16 @@
                 BaseSource, datasource_container.datasource
             )
             schema = self._setup_schema(
                 datasource_name=datasource_name,
                 datasource=datasource_container.datasource,
                 data_config=datasource_container.data_config,
                 pod_name=self.name,
+                pod_db_connector=self.pod_db_connector,
+                schema=datasource_container.schema,
             )
 
         # Update the schema on the hub
         try:
             public_metadata = self._get_public_metadata(
                 datasource_name,
                 datasource_container.datasource_details,
```

### Comparing `bitfount-0.9.4/bitfount/federated/pod_db_utils.py` & `bitfount-0.9.5/bitfount/federated/pod_db_utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/pod_response_message.py` & `bitfount-0.9.5/bitfount/federated/pod_response_message.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/pod_vitals.py` & `bitfount-0.9.5/bitfount/federated/pod_vitals.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/privacy/differential.py` & `bitfount-0.9.5/bitfount/federated/privacy/differential.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/protocols/__init__.py` & `bitfount-0.9.5/bitfount/federated/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/protocols/base.py` & `bitfount-0.9.5/bitfount/federated/protocols/base.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/protocols/conversation.py` & `bitfount-0.9.5/bitfount/federated/protocols/conversation.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/protocols/model_protocols/federated_averaging.py` & `bitfount-0.9.5/bitfount/federated/protocols/model_protocols/federated_averaging.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/protocols/model_protocols/inference_csv_report.py` & `bitfount-0.9.5/bitfount/federated/protocols/model_protocols/inference_csv_report.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/protocols/model_protocols/instrumented_inference_csv_report.py` & `bitfount-0.9.5/bitfount/federated/protocols/model_protocols/instrumented_inference_csv_report.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/protocols/psi.py` & `bitfount-0.9.5/bitfount/federated/protocols/psi.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/protocols/results_only.py` & `bitfount-0.9.5/bitfount/federated/protocols/results_only.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/roles.py` & `bitfount-0.9.5/bitfount/federated/roles.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/secure.py` & `bitfount-0.9.5/bitfount/federated/secure.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/shim.py` & `bitfount-0.9.5/bitfount/federated/shim.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/task_requests.py` & `bitfount-0.9.5/bitfount/federated/task_requests.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/base_transport.py` & `bitfount-0.9.5/bitfount/federated/transport/base_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 from bitfount.config import _BITFOUNT_MULTITHREADING_DEBUG
 from bitfount.exceptions import BitfountError
 from bitfount.federated.exceptions import (
     MessageHandlerNotFoundError,
     MessageRetrievalError,
     MessageTypeSpecificHandlerNotFoundError,
+    TaskAbortError,
 )
 from bitfount.federated.logging import _get_federated_logger
 from bitfount.federated.transport.handlers import _PriorityHandler, _TemporaryHandler
 from bitfount.federated.transport.message_service import (
     _BitfountMessage,
     _BitfountMessageType,
     _MessageEncryption,
@@ -491,14 +492,25 @@
                         f"No mailbox exists for '{self.mailbox_id}', "
                         f"ensure connect_pod() or send_task_requests() is called first."
                     )
                 raise MessageRetrievalError(
                     f"An error occurred when trying to communicate"
                     f" with the messaging service: {err}"
                 ) from err
+            except TaskAbortError as tae:
+                logger.info(
+                    f"Received TASK_ABORT request from handler. Aborting: {tae}"
+                )
+                raise
+            except BaseException as e:
+                # Want to ensure we log out whatever happened
+                logger.error(
+                    f"Unexpected error in message retrieval: {e}", exc_info=True
+                )
+                raise
             finally:
                 # Cancel outstanding dispatch tasks
                 if len(running_dispatch_tasks) > 0:
                     cancelled_tasks: Set[str] = set()
 
                     for task in running_dispatch_tasks:
                         task.cancel()
@@ -1234,14 +1246,24 @@
                     error_msg += (
                         f" Exception was: {exc}. This has been passed to the task"
                         f" to handle."
                     )
                     logger.error(error_msg)
                     logger.exception(exc)
 
+                    # TODO: [BIT-3718] This approach to propagating the exception
+                    #       from the mailbox to the task is not really supported
+                    #       in Python; whilst it _will_ cause the task to raise
+                    #       the exception it will likely cause RuntimeErrors related
+                    #       to the coroutine being awaited multiple times.
+                    #       The issue is that throwing an exception into the underlying
+                    #       coroutine does nothing to mark the wrapping Task as
+                    #       cancelled/done and so it can continue to attempt to
+                    #       use the coroutine without knowing it has already had
+                    #       an exception raised/been awaited.
                     # Pass to task to handle then await on task
                     cast(Coroutine, run_task.get_coro()).throw(exc)
                     return await run_task
                 else:
                     # Otherwise, log that something went wrong and wait on the run_task
                     # to "finish"
                     logger.error(error_msg)
```

### Comparing `bitfount-0.9.4/bitfount/federated/transport/config.py` & `bitfount-0.9.5/bitfount/federated/transport/config.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/handlers.py` & `bitfount-0.9.5/bitfount/federated/transport/handlers.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/identity_verification/oidc.py` & `bitfount-0.9.5/bitfount/federated/transport/identity_verification/oidc.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/identity_verification/saml.py` & `bitfount-0.9.5/bitfount/federated/transport/identity_verification/saml.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/identity_verification/types.py` & `bitfount-0.9.5/bitfount/federated/transport/identity_verification/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/message_service.py` & `bitfount-0.9.5/bitfount/federated/transport/message_service.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/modeller_transport.py` & `bitfount-0.9.5/bitfount/federated/transport/modeller_transport.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/opentelemetry.py` & `bitfount-0.9.5/bitfount/federated/transport/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/pod_transport.py` & `bitfount-0.9.5/bitfount/federated/transport/pod_transport.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/protos/messages_pb2.py` & `bitfount-0.9.5/bitfount/federated/transport/protos/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/protos/messages_pb2.pyi` & `bitfount-0.9.5/bitfount/federated/transport/protos/messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/protos/messages_pb2_grpc.py` & `bitfount-0.9.5/bitfount/federated/transport/protos/messages_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/protos/messages_pb2_grpc.pyi` & `bitfount-0.9.5/bitfount/federated/transport/protos/messages_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/types.py` & `bitfount-0.9.5/bitfount/federated/transport/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/utils.py` & `bitfount-0.9.5/bitfount/federated/transport/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/transport/worker_transport.py` & `bitfount-0.9.5/bitfount/federated/transport/worker_transport.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/types.py` & `bitfount-0.9.5/bitfount/federated/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/utils.py` & `bitfount-0.9.5/bitfount/federated/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/federated/worker.py` & `bitfount-0.9.5/bitfount/federated/worker.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/hooks.py` & `bitfount-0.9.5/bitfount/hooks.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/hub/__init__.py` & `bitfount-0.9.5/bitfount/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/hub/api.py` & `bitfount-0.9.5/bitfount/hub/api.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/hub/authentication_flow.py` & `bitfount-0.9.5/bitfount/hub/authentication_flow.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/hub/authentication_handlers.py` & `bitfount-0.9.5/bitfount/hub/authentication_handlers.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/hub/exceptions.py` & `bitfount-0.9.5/bitfount/hub/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/hub/helper.py` & `bitfount-0.9.5/bitfount/hub/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper functions related to hub and AM interactions."""
+
 from __future__ import annotations
 
 import logging
 import os
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Iterable, Mapping, Optional, Union, cast
 
@@ -369,33 +370,36 @@
 
 def get_pod_schema(
     pod_identifier: str,
     save_file_path: Optional[Union[str, Path]] = None,
     hub: Optional[BitfountHub] = None,
     username: Optional[str] = None,
     project_id: Optional[str] = None,
+    secrets: Optional[Union[APIKeys, JWT]] = None,
 ) -> BitfountSchema:
     """Get a pod's schema from the hub.
 
     Args:
         pod_identifier: The identifier of the pod. If supplied with only pod name
             assumes the namespace is the current user.
         save_file_path: Optional. Path to save the downloaded schema to. Won't save
             if not provided.
         hub: Optional. The BitfountHub to connect to. The default hub will be
              used if not provided.
         username: The username to use when connecting to the hub if a hub instance is
             not provided.
+        project_id: The project ID to use when connecting to the hub.
+        secrets: Optional. Either APIKeys or JWT to use for authentication.
 
     Returns:
         The loaded BitfountSchema object.
     """
     # Generate default hub if not provided
     if not hub:
-        hub = _create_bitfounthub(username=username)
+        hub = _create_bitfounthub(username=username, secrets=secrets)
     elif username:
         logger.warning("Ignoring username argument as hub was provided.")
 
     # Check if full pod_identifier or pod name only
     if "/" not in pod_identifier:
         # Construct full pod identifier if needed
         pod_identifier = f"{hub.username}/{pod_identifier}"
```

### Comparing `bitfount-0.9.4/bitfount/hub/types.py` & `bitfount-0.9.5/bitfount/hub/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/hub/utils.py` & `bitfount-0.9.5/bitfount/hub/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/metrics.py` & `bitfount-0.9.5/bitfount/metrics.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/models/__init__.py` & `bitfount-0.9.5/bitfount/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/models/base_models.py` & `bitfount-0.9.5/bitfount/models/base_models.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/models/bitfount_model.py` & `bitfount-0.9.5/bitfount/models/bitfount_model.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/models/models.py` & `bitfount-0.9.5/bitfount/models/models.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/models/nn.py` & `bitfount-0.9.5/bitfount/models/nn.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/runners/config_schemas.py` & `bitfount-0.9.5/bitfount/runners/config_schemas.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/runners/modeller_runner.py` & `bitfount-0.9.5/bitfount/runners/modeller_runner.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/runners/pod_runner.py` & `bitfount-0.9.5/bitfount/runners/pod_runner.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/runners/upload_task_templates.py` & `bitfount-0.9.5/bitfount/runners/upload_task_templates.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/runners/utils.py` & `bitfount-0.9.5/bitfount/runners/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/schemas/utils.py` & `bitfount-0.9.5/bitfount/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/scripts/generate_schema.py` & `bitfount-0.9.5/bitfount/scripts/generate_schema.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/scripts/generate_yaml_specs.py` & `bitfount-0.9.5/bitfount/scripts/generate_yaml_specs.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/scripts/run_modeller.py` & `bitfount-0.9.5/bitfount/scripts/run_modeller.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/scripts/run_pod.py` & `bitfount-0.9.5/bitfount/scripts/run_pod.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/scripts/run_testing.py` & `bitfount-0.9.5/bitfount/scripts/run_testing.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/scripts/script_runner.py` & `bitfount-0.9.5/bitfount/scripts/script_runner.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/storage.py` & `bitfount-0.9.5/bitfount/storage.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/__init__.py` & `bitfount-0.9.5/bitfount/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/base_transformation.py` & `bitfount-0.9.5/bitfount/transformations/base_transformation.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/batch_operations.py` & `bitfount-0.9.5/bitfount/transformations/batch_operations.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/binary_operations.py` & `bitfount-0.9.5/bitfount/transformations/binary_operations.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/dataset_operations.py` & `bitfount-0.9.5/bitfount/transformations/dataset_operations.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/exceptions.py` & `bitfount-0.9.5/bitfount/transformations/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/parser.py` & `bitfount-0.9.5/bitfount/transformations/parser.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/processor.py` & `bitfount-0.9.5/bitfount/transformations/processor.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/references.py` & `bitfount-0.9.5/bitfount/transformations/references.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/torchio_batch_operations.py` & `bitfount-0.9.5/bitfount/transformations/torchio_batch_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import inspect
 from typing import Any, Dict, List, Protocol, Type, Union, cast
 
 import attr
 from marshmallow import fields, post_load
 from marshmallow_union import Union as M_Union
 import numpy as np
-import torchio as tio
 
 from bitfount.config import _PYTORCH_ENGINE, BITFOUNT_ENGINE
+
+if BITFOUNT_ENGINE == _PYTORCH_ENGINE:
+    import torchio as tio
+
 from bitfount.data.types import DataSplit
 from bitfount.transformations.base_transformation import _TransformationSchema
 from bitfount.transformations.batch_operations import BatchTimeOperation
 from bitfount.transformations.exceptions import TransformationParsingError
 from bitfount.types import _JSONDict
 
 #: Dictionary of available image transformations and their corresponding classes.
```

### Comparing `bitfount-0.9.4/bitfount/transformations/unary_operations.py` & `bitfount-0.9.5/bitfount/transformations/unary_operations.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/transformations/utils.py` & `bitfount-0.9.5/bitfount/transformations/utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/types.py` & `bitfount-0.9.5/bitfount/types.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/utils/__init__.py` & `bitfount-0.9.5/bitfount/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/utils/concurrency_utils.py` & `bitfount-0.9.5/bitfount/utils/concurrency_utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/utils/db_connector.py` & `bitfount-0.9.5/bitfount/utils/db_connector.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/utils/logging_utils.py` & `bitfount-0.9.5/bitfount/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/utils/pandas_utils.py` & `bitfount-0.9.5/bitfount/utils/pandas_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions for interacting with pandas."""
+
 import logging
 from typing import Callable, Generator, Iterable
 
 from pandas import RangeIndex
 import pandas as pd
 
 _logger = logging.getLogger(__name__)
@@ -44,15 +45,15 @@
             )
             continue
         else:
             new_rows = len(tmp_df)
             next_idx = curr_idx + new_rows
 
             if reset_index:
-                print(f"{curr_idx=}, {new_rows=}")
+                _logger.debug(f"{curr_idx=}, {new_rows=}")
                 idx = RangeIndex(curr_idx, next_idx)
                 tmp_df = tmp_df.set_index(idx)
 
             yield tmp_df
 
             curr_idx = next_idx
```

### Comparing `bitfount-0.9.4/bitfount/utils/ssl_utils.py` & `bitfount-0.9.5/bitfount/utils/ssl_utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount/utils/web_utils.py` & `bitfount-0.9.5/bitfount/utils/web_utils.py`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount.egg-info/PKG-INFO` & `bitfount-0.9.5/bitfount.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitfount
-Version: 0.9.4
+Version: 0.9.5
 Summary: Machine Learning and Federated Learning Library.
 Home-page: https://github.com/bitfount/bitfount
 Author: Bitfount
 Author-email: info@bitfount.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.bitfount.com/
 Project-URL: Homepage, https://bitfount.com
```

### Comparing `bitfount-0.9.4/bitfount.egg-info/SOURCES.txt` & `bitfount-0.9.5/bitfount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/bitfount.egg-info/requires.txt` & `bitfount-0.9.5/bitfount.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/pyproject.toml` & `bitfount-0.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/310/requirements-dev.in` & `bitfount-0.9.5/requirements/310/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/310/requirements-dev.txt` & `bitfount-0.9.5/requirements/310/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/310/requirements-test.txt` & `bitfount-0.9.5/requirements/310/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/310/requirements-tutorial.in` & `bitfount-0.9.5/requirements/310/requirements-tutorial.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/310/requirements-tutorial.txt` & `bitfount-0.9.5/requirements/310/requirements-tutorial.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/38/differential_privacy/requirements-dp.in` & `bitfount-0.9.5/requirements/38/differential_privacy/requirements-dp.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/38/requirements-dev.in` & `bitfount-0.9.5/requirements/38/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/38/requirements-dev.txt` & `bitfount-0.9.5/requirements/38/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/38/requirements-test.txt` & `bitfount-0.9.5/requirements/38/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/38/requirements-tutorial.in` & `bitfount-0.9.5/requirements/38/requirements-tutorial.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/38/requirements-tutorial.txt` & `bitfount-0.9.5/requirements/38/requirements-tutorial.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/39/differential_privacy/requirements-dp.in` & `bitfount-0.9.5/requirements/39/differential_privacy/requirements-dp.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/39/requirements-dev.in` & `bitfount-0.9.5/requirements/39/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/39/requirements-dev.txt` & `bitfount-0.9.5/requirements/39/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/39/requirements-test.txt` & `bitfount-0.9.5/requirements/39/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/39/requirements-tutorial.in` & `bitfount-0.9.5/requirements/39/requirements-tutorial.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/39/requirements-tutorial.txt` & `bitfount-0.9.5/requirements/39/requirements-tutorial.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/constraints-compatibility.txt` & `bitfount-0.9.5/requirements/constraints-compatibility.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/constraints-security.txt` & `bitfount-0.9.5/requirements/constraints-security.txt`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/requirements/requirements.in` & `bitfount-0.9.5/requirements/requirements.in`

 * *Files identical despite different names*

### Comparing `bitfount-0.9.4/setup.py` & `bitfount-0.9.5/setup.py`

 * *Files identical despite different names*


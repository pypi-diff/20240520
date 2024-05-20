# Comparing `tmp/datatransfer_client-2.10.8.tar.gz` & `tmp/datatransfer_client-2.10.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransfer_client-2.10.8.tar", last modified: Mon Feb 19 06:40:30 2024, max compression
+gzip compressed data, was "datatransfer_client-2.10.9.tar", last modified: Thu Mar  7 11:02:47 2024, max compression
```

## Comparing `datatransfer_client-2.10.8.tar` & `datatransfer_client-2.10.9.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.075271 datatransfer_client-2.10.8/
--rw-r--r--   0 toor      (1000) toor      (1000)      153 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)      683 2024-02-19 06:40:30.075271 datatransfer_client-2.10.8/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      859 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/README.md
--rw-r--r--   0 toor      (1000) toor      (1000)       91 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/REQUIREMENTS
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-02-19 06:40:30.075271 datatransfer_client-2.10.8/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     1221 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.025271 datatransfer_client-2.10.8/src/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.027271 datatransfer_client-2.10.8/src/datatransfer/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.029271 datatransfer_client-2.10.8/src/datatransfer/common/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1036 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/configuration.py
--rw-r--r--   0 toor      (1000) toor      (1000)      576 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/constants.py
--rw-r--r--   0 toor      (1000) toor      (1000)    12475 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.029271 datatransfer_client-2.10.8/src/datatransfer/common/mapping/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/mapping/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    70170 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/mapping/enum.py
--rw-r--r--   0 toor      (1000) toor      (1000)       89 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/messages.py
--rw-r--r--   0 toor      (1000) toor      (1000)      429 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/smev256.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.030271 datatransfer_client-2.10.8/src/datatransfer/common/utils/
--rw-r--r--   0 toor      (1000) toor      (1000)     3651 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/utils/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9256 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/utils/test.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.031271 datatransfer_client-2.10.8/src/datatransfer/common/xml/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/xml/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3284 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/common/xml/parser.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.033271 datatransfer_client-2.10.8/src/datatransfer/source/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3651 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      414 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/app_meta.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.036271 datatransfer_client-2.10.8/src/datatransfer/source/catalog/
--rw-r--r--   0 toor      (1000) toor      (1000)       24 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16069 2024-02-19 06:40:21.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      352 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)      979 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)      340 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/exceptions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.036271 datatransfer_client-2.10.8/src/datatransfer/source/catalog/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     3868 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)      468 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/migrations/0002_feedback_comment_update_charfield_to_textfield.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2968 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/model_views.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3137 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)      818 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/permissions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      269 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/plugin_meta.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.037271 datatransfer_client-2.10.8/src/datatransfer/source/catalog/project_models/
--rw-r--r--   0 toor      (1000) toor      (1000)     1344 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/project_models/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      189 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/project_models/common.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.038271 datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/
--rw-r--r--   0 toor      (1000) toor      (1000)       24 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1016 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/builder.py
--rw-r--r--   0 toor      (1000) toor      (1000)      894 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/provider.py
--rw-r--r--   0 toor      (1000) toor      (1000)      461 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/report.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9216 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/report.xls
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.039271 datatransfer_client-2.10.8/src/datatransfer/source/catalog/south_migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     5212 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/south_migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2889 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/south_migrations/0002_feedback_comment_update_charfield_to_textfield.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/south_migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4405 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.018271 datatransfer_client-2.10.8/src/datatransfer/source/catalog/templates/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.040271 datatransfer_client-2.10.8/src/datatransfer/source/catalog/templates/ui-js/
--rw-r--r--   0 toor      (1000) toor      (1000)     1312 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/templates/ui-js/feedback-list-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     2906 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/templates/ui-js/feedback-view-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     6749 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2377 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/catalog/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.041271 datatransfer_client-2.10.8/src/datatransfer/source/common/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/common/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.041271 datatransfer_client-2.10.8/src/datatransfer/source/common/configuration/
--rw-r--r--   0 toor      (1000) toor      (1000)     2826 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/common/configuration/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16164 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/common/configuration/configuration.py
--rw-r--r--   0 toor      (1000) toor      (1000)      710 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/common/constants.py
--rw-r--r--   0 toor      (1000) toor      (1000)      607 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/common/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5399 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/common/tasks.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4601 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/configs.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.043271 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1008 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2841 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/client.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.043271 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.043271 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.044271 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/extractor/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/extractor/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.044271 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/extractor/common/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/extractor/common/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      175 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/extractor/common/mapping.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.045271 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/loader/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/loader/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8560 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/loader/mapping.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.045271 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)    16565 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9979 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/models.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.046271 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/service/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/service/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      512 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/service/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3606 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/service/service.py
--rw-r--r--   0 toor      (1000) toor      (1000)    18368 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/tasks.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2211 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.046271 datatransfer_client-2.10.8/src/datatransfer/source/etl/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/etl/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.046271 datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.047271 datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/extractor/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/extractor/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.047271 datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/extractor/common/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/extractor/common/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      995 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/extractor/common/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      440 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/extractor/common/mapping.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.051271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/
--rw-r--r--   0 toor      (1000) toor      (1000)     1866 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    14323 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)      974 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/apps.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.052271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/
--rw-r--r--   0 toor      (1000) toor      (1000)     1341 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11363 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/changes.py
--rw-r--r--   0 toor      (1000) toor      (1000)      367 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/constants.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1209 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/extensions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5128 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4721 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6861 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/wrappers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      315 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/constants.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.053271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.053271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.053271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/extractor/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/extractor/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.054271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/extractor/common/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/extractor/common/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      168 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/extractor/common/mapping.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.055271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/loader/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/loader/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6708 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/loader/mapping.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.055271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.055271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      643 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/management/commands/contingent_get_data.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.056271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)    18269 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)      717 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/migrations/0002_auto_20161209_1332.py
--rw-r--r--   0 toor      (1000) toor      (1000)      814 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/migrations/0003_auto_20191219_0759.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4195 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/model_views.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13019 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)      268 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/plugin_meta.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.057271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/portfolio_tab/
--rw-r--r--   0 toor      (1000) toor      (1000)      159 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/portfolio_tab/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4320 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/portfolio_tab/actions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.058271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/service/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/service/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2834 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/service/client.py
--rw-r--r--   0 toor      (1000) toor      (1000)      542 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/service/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3276 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/service/service.py
--rw-r--r--   0 toor      (1000) toor      (1000)      557 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.059271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/south_migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)    19422 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/south_migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/south_migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16034 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.023271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.060271 datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/
--rw-r--r--   0 toor      (1000) toor      (1000)     2544 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/changes-edit-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     1784 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/get-data-list-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     6409 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/multiselect-page-fix.js
--rw-r--r--   0 toor      (1000) toor      (1000)     2786 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/person-data-list-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)      996 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/statistics-list-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)    10297 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5389 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_data/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.062271 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/
--rw-r--r--   0 toor      (1000) toor      (1000)       74 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)       68 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/const.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.062271 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.063271 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/packet/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/packet/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.063271 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/packet/extractor/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/packet/extractor/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.063271 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/packet/extractor/common/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/packet/extractor/common/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      229 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/etl/packet/extractor/common/mapping.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.064271 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     4404 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1331 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/migrations/0002_auto_20210315_0922.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2207 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)      227 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/plugin_meta.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.065271 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/service/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/service/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2869 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/service/client.py
--rw-r--r--   0 toor      (1000) toor      (1000)      544 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/service/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3347 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/service/service.py
--rw-r--r--   0 toor      (1000) toor      (1000)      556 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11784 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/tasks.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6906 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)      528 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/permissions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      227 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/plugin_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)      219 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.066271 datatransfer_client-2.10.8/src/datatransfer/source/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)      500 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/templates/select-organization-window.js
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.066271 datatransfer_client-2.10.8/src/datatransfer/source/transport/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.066271 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.067271 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/client/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/client/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1810 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/client/base.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.068271 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datapush/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datapush/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      876 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datapush/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6014 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datapush/service.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.069271 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datatransfer/
--rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datatransfer/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3358 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datatransfer/client.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.070271 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/kte/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/kte/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7481 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/kte/client.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11456 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/kte/tasks.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1269 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2981 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/source/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-02-19 06:40:29.000000 datatransfer_client-2.10.8/src/datatransfer/version.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.074271 datatransfer_client-2.10.8/src/datatransfer_client.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)      683 2024-02-19 06:40:29.000000 datatransfer_client-2.10.8/src/datatransfer_client.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     8868 2024-02-19 06:40:30.000000 datatransfer_client-2.10.8/src/datatransfer_client.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-02-19 06:40:29.000000 datatransfer_client-2.10.8/src/datatransfer_client.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       92 2024-02-19 06:40:29.000000 datatransfer_client-2.10.8/src/datatransfer_client.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2024-02-19 06:40:29.000000 datatransfer_client-2.10.8/src/datatransfer_client.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-19 06:40:30.073271 datatransfer_client-2.10.8/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)     3391 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/tests/test_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11129 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/tests/test_from_rs.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7063 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/tests/test_test_utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3003 2023-09-18 12:40:29.000000 datatransfer_client-2.10.8/tests/test_to_rs.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.530502 datatransfer_client-2.10.9/
+-rw-r--r--   0 toor      (1000) toor      (1000)      153 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)      683 2024-03-07 11:02:47.529502 datatransfer_client-2.10.9/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      859 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/README.md
+-rw-r--r--   0 toor      (1000) toor      (1000)       91 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/REQUIREMENTS
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-03-07 11:02:47.530502 datatransfer_client-2.10.9/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     1221 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.335502 datatransfer_client-2.10.9/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.340502 datatransfer_client-2.10.9/src/datatransfer/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.346502 datatransfer_client-2.10.9/src/datatransfer/common/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1036 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/configuration.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      576 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/constants.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12475 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.348502 datatransfer_client-2.10.9/src/datatransfer/common/mapping/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/mapping/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    70170 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/mapping/enum.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       89 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/messages.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      429 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/smev256.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.352502 datatransfer_client-2.10.9/src/datatransfer/common/utils/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3651 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/utils/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9256 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/utils/test.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.355502 datatransfer_client-2.10.9/src/datatransfer/common/xml/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/xml/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3284 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/common/xml/parser.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.365502 datatransfer_client-2.10.9/src/datatransfer/source/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3651 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      414 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/app_meta.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.376502 datatransfer_client-2.10.9/src/datatransfer/source/catalog/
+-rw-r--r--   0 toor      (1000) toor      (1000)       24 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16069 2024-03-07 11:02:41.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      352 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      979 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      340 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/exceptions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.379502 datatransfer_client-2.10.9/src/datatransfer/source/catalog/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3868 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      468 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/migrations/0002_feedback_comment_update_charfield_to_textfield.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2968 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/model_views.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3137 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      818 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/permissions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      269 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/plugin_meta.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.381502 datatransfer_client-2.10.9/src/datatransfer/source/catalog/project_models/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1344 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/project_models/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      189 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/project_models/common.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.391502 datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/
+-rw-r--r--   0 toor      (1000) toor      (1000)       24 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1016 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/builder.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      894 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/provider.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      461 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/report.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9216 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/report.xls
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.395502 datatransfer_client-2.10.9/src/datatransfer/source/catalog/south_migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5212 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/south_migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2889 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/south_migrations/0002_feedback_comment_update_charfield_to_textfield.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/south_migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4405 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.321502 datatransfer_client-2.10.9/src/datatransfer/source/catalog/templates/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.397502 datatransfer_client-2.10.9/src/datatransfer/source/catalog/templates/ui-js/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1312 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/templates/ui-js/feedback-list-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     2906 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/templates/ui-js/feedback-view-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     6749 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2377 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/catalog/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.401502 datatransfer_client-2.10.9/src/datatransfer/source/common/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/common/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.402502 datatransfer_client-2.10.9/src/datatransfer/source/common/configuration/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3059 2024-03-07 11:02:41.000000 datatransfer_client-2.10.9/src/datatransfer/source/common/configuration/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16164 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/common/configuration/configuration.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      710 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/common/constants.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      607 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/common/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5399 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/common/tasks.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4601 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/configs.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.409502 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1008 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2841 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/client.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.410502 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.411502 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.412502 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/extractor/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/extractor/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.415502 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/extractor/common/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/extractor/common/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      175 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/extractor/common/mapping.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.417502 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/loader/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/loader/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8560 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/loader/mapping.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.424502 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)    16565 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9979 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/models.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.427502 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/service/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/service/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      512 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/service/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3606 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/service/service.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    18368 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/tasks.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2211 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.428502 datatransfer_client-2.10.9/src/datatransfer/source/etl/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/etl/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.429502 datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.431502 datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/extractor/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/extractor/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.435502 datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/extractor/common/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/extractor/common/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      995 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/extractor/common/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      440 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/extractor/common/mapping.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.445502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1866 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14323 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      974 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/apps.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.457502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1341 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11363 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/changes.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      367 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/constants.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1209 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/extensions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5128 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4721 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6861 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/wrappers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      315 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/constants.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.458502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.458502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.460502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/extractor/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/extractor/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.461502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/extractor/common/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/extractor/common/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      168 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/extractor/common/mapping.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.463502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/loader/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/loader/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6708 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/loader/mapping.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.465502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.465502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      643 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/management/commands/contingent_get_data.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.469502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)    18269 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      717 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/migrations/0002_auto_20161209_1332.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      814 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/migrations/0003_auto_20191219_0759.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4195 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/model_views.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    13019 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      268 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/plugin_meta.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.471502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/portfolio_tab/
+-rw-r--r--   0 toor      (1000) toor      (1000)      159 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/portfolio_tab/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4320 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/portfolio_tab/actions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.478502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/service/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/service/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2834 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/service/client.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      542 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/service/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3276 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/service/service.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      557 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.480502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/south_migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)    19422 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/south_migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/south_migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16034 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.330502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.486502 datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2544 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/changes-edit-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     1784 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/get-data-list-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     6409 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/multiselect-page-fix.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     2786 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/person-data-list-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)      996 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/statistics-list-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)    10297 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5389 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_data/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.494502 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/
+-rw-r--r--   0 toor      (1000) toor      (1000)       74 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       68 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/const.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.495502 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.495502 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/packet/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/packet/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.497502 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/packet/extractor/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/packet/extractor/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.499502 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/packet/extractor/common/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/packet/extractor/common/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      229 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/etl/packet/extractor/common/mapping.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.502502 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4404 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1331 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/migrations/0002_auto_20210315_0922.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2207 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      227 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/plugin_meta.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.505502 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/service/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/service/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2869 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/service/client.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      544 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/service/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3347 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/service/service.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      556 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11784 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/tasks.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6906 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      528 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/permissions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      227 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/plugin_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      219 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.506502 datatransfer_client-2.10.9/src/datatransfer/source/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)      500 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/templates/select-organization-window.js
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.507502 datatransfer_client-2.10.9/src/datatransfer/source/transport/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.507502 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.509502 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/client/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/client/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1810 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/client/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.514502 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datapush/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datapush/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      876 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datapush/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6014 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datapush/service.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.516502 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datatransfer/
+-rw-r--r--   0 toor      (1000) toor      (1000)       16 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datatransfer/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3358 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datatransfer/client.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.519502 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/kte/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/kte/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7481 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/kte/client.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11456 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/kte/tasks.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1269 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2981 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/src/datatransfer/source/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-03-07 11:02:47.000000 datatransfer_client-2.10.9/src/datatransfer/version.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.528502 datatransfer_client-2.10.9/src/datatransfer_client.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)      683 2024-03-07 11:02:47.000000 datatransfer_client-2.10.9/src/datatransfer_client.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     8868 2024-03-07 11:02:47.000000 datatransfer_client-2.10.9/src/datatransfer_client.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-03-07 11:02:47.000000 datatransfer_client-2.10.9/src/datatransfer_client.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       92 2024-03-07 11:02:47.000000 datatransfer_client-2.10.9/src/datatransfer_client.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2024-03-07 11:02:47.000000 datatransfer_client-2.10.9/src/datatransfer_client.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-07 11:02:47.526502 datatransfer_client-2.10.9/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3391 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/tests/test_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11129 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/tests/test_from_rs.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7063 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/tests/test_test_utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3003 2023-09-18 12:40:29.000000 datatransfer_client-2.10.9/tests/test_to_rs.py
```

### Comparing `datatransfer_client-2.10.8/PKG-INFO` & `datatransfer_client-2.10.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransfer_client
-Version: 2.10.8
+Version: 2.10.9
 Author: BARS Group
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `datatransfer_client-2.10.8/README.md` & `datatransfer_client-2.10.9/README.md`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/setup.py` & `datatransfer_client-2.10.9/setup.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/common/configuration.py` & `datatransfer_client-2.10.9/src/datatransfer/common/configuration.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/common/constants.py` & `datatransfer_client-2.10.9/src/datatransfer/common/constants.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/common/helpers.py` & `datatransfer_client-2.10.9/src/datatransfer/common/helpers.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/common/mapping/enum.py` & `datatransfer_client-2.10.9/src/datatransfer/common/mapping/enum.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/common/utils/__init__.py` & `datatransfer_client-2.10.9/src/datatransfer/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/common/utils/test.py` & `datatransfer_client-2.10.9/src/datatransfer/common/utils/test.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/common/xml/parser.py` & `datatransfer_client-2.10.9/src/datatransfer/common/xml/parser.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/actions.py` & `datatransfer_client-2.10.9/src/datatransfer/source/actions.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/actions.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/actions.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/apps.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/apps.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/migrations/0001_initial.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/model_views.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/model_views.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/permissions.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/permissions.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/project_models/__init__.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/project_models/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/builder.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/builder.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/provider.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/provider.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/report/report.xls` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/report/report.xls`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/south_migrations/0001_initial.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/south_migrations/0002_feedback_comment_update_charfield_to_textfield.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/south_migrations/0002_feedback_comment_update_charfield_to_textfield.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/tasks.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/tasks.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/templates/ui-js/feedback-list-window.js` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/templates/ui-js/feedback-list-window.js`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/templates/ui-js/feedback-view-window.js` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/templates/ui-js/feedback-view-window.js`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/ui.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/ui.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/catalog/utils.py` & `datatransfer_client-2.10.9/src/datatransfer/source/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/common/configuration/__init__.py` & `datatransfer_client-2.10.9/src/datatransfer/source/common/configuration/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # coding: utf-8
 
 
 from __future__ import absolute_import
+
+
 class ProductConfiguration(object):
 
     u"""Класс конфигурации."""
 
     known_attrs = (
         'log_model',
         'client_class',
@@ -31,15 +33,15 @@
         'enroll_get_data_mapping_rules',
     )
 
     active = False
 
     def __getattr__(self, name):
         # fixme: убрать "active" после отказа от yadic
-        if name != 'active' and not hasattr(self, name):
+        if name != 'active' and name not in self.__dict__:
             raise AttributeError("Parameter {} is not set".format(name))
         return super(ProductConfiguration, self).__getattribute__(name)
 
     def __setattr__(self, name, value):
         assert name in self.known_attrs, (
             'Parameter {} is not registered'.format(name)
         )
@@ -71,11 +73,15 @@
 def get_object(name):
     u"""Возвращает требуемый объект, используя конфигурацию РИС.
 
     :param string name: Имя объекта из РИС.
     :return: Объект из РИС.
     """
     if product_configuration.active:
-        return getattr(product_configuration, name)
+        try:
+            return getattr(product_configuration, name)
+        except AttributeError:
+            # если именно этот параметр отсутствует в product_configuration, то fallback на следующий вариант
+            pass
     if hasattr(settings, 'SYSTEM_NAME'):
         return container.get(name, settings.SYSTEM_NAME)
     raise AssertionError("Datatransfer-client is not configured")
```

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/common/configuration/configuration.py` & `datatransfer_client-2.10.9/src/datatransfer/source/common/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/common/constants.py` & `datatransfer_client-2.10.9/src/datatransfer/source/common/constants.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/common/helpers.py` & `datatransfer_client-2.10.9/src/datatransfer/source/common/helpers.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/common/tasks.py` & `datatransfer_client-2.10.9/src/datatransfer/source/common/tasks.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/configs.py` & `datatransfer_client-2.10.9/src/datatransfer/source/configs.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/apps.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/apps.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/client.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/client.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/etl/packet/loader/mapping.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/etl/packet/loader/mapping.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/migrations/0001_initial.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/service/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/service/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/service/service.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/service/service.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/tasks.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/tasks.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/enroll_get_data/utils.py` & `datatransfer_client-2.10.9/src/datatransfer/source/enroll_get_data/utils.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/etl/packet/extractor/common/helpers.py` & `datatransfer_client-2.10.9/src/datatransfer/source/etl/packet/extractor/common/helpers.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/__init__.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/actions.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/actions.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/apps.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/apps.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/__init__.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/changes.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/changes.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/extensions.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/extensions.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/utils.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/utils.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/changes/wrappers.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/changes/wrappers.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/etl/packet/loader/mapping.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/etl/packet/loader/mapping.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/management/commands/contingent_get_data.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/management/commands/contingent_get_data.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/migrations/0001_initial.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/migrations/0002_auto_20161209_1332.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/migrations/0002_auto_20161209_1332.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/migrations/0003_auto_20191219_0759.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/migrations/0003_auto_20191219_0759.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/model_views.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/model_views.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/portfolio_tab/actions.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/portfolio_tab/actions.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/service/client.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/service/client.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/service/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/service/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/service/service.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/service/service.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/settings.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/settings.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/south_migrations/0001_initial.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/tasks.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/tasks.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/changes-edit-window.js` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/changes-edit-window.js`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/get-data-list-window.js` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/get-data-list-window.js`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/multiselect-page-fix.js` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/multiselect-page-fix.js`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/person-data-list-window.js` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/person-data-list-window.js`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/templates/get_data/statistics-list-window.js` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/templates/get_data/statistics-list-window.js`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/ui.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/ui.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_data/utils.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_data/utils.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/migrations/0001_initial.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/migrations/0002_auto_20210315_0922.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/migrations/0002_auto_20210315_0922.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/service/client.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/service/client.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/service/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/service/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/service/service.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/service/service.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/settings.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/settings.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/tasks.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/tasks.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/get_privilege/utils.py` & `datatransfer_client-2.10.9/src/datatransfer/source/get_privilege/utils.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/permissions.py` & `datatransfer_client-2.10.9/src/datatransfer/source/permissions.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/client/base.py` & `datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/client/base.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datapush/models.py` & `datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datapush/models.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datapush/service.py` & `datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datapush/service.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/datatransfer/client.py` & `datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/datatransfer/client.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/kte/client.py` & `datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/kte/client.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/transport/smev/kte/tasks.py` & `datatransfer_client-2.10.9/src/datatransfer/source/transport/smev/kte/tasks.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/ui.py` & `datatransfer_client-2.10.9/src/datatransfer/source/ui.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer/source/utils.py` & `datatransfer_client-2.10.9/src/datatransfer/source/utils.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/src/datatransfer_client.egg-info/PKG-INFO` & `datatransfer_client-2.10.9/src/datatransfer_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransfer_client
-Version: 2.10.8
+Version: 2.10.9
 Author: BARS Group
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `datatransfer_client-2.10.8/src/datatransfer_client.egg-info/SOURCES.txt` & `datatransfer_client-2.10.9/src/datatransfer_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/tests/test_common.py` & `datatransfer_client-2.10.9/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/tests/test_from_rs.py` & `datatransfer_client-2.10.9/tests/test_from_rs.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/tests/test_test_utils.py` & `datatransfer_client-2.10.9/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `datatransfer_client-2.10.8/tests/test_to_rs.py` & `datatransfer_client-2.10.9/tests/test_to_rs.py`

 * *Files identical despite different names*


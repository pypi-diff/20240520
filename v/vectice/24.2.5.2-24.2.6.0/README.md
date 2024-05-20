# Comparing `tmp/vectice-24.2.5.2.tar.gz` & `tmp/vectice-24.2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-24.2.5.2.tar", last modified: Wed May 15 13:40:15 2024, max compression
+gzip compressed data, was "vectice-24.2.6.0.tar", last modified: Mon May 20 08:13:37 2024, max compression
```

## Comparing `vectice-24.2.5.2.tar` & `vectice-24.2.6.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:15.003021 vectice-24.2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 13:40:07.000000 vectice-24.2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-15 13:40:15.003021 vectice-24.2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-15 13:40:07.000000 vectice-24.2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-15 13:40:07.000000 vectice-24.2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 13:40:15.003021 vectice-24.2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-15 13:40:07.000000 vectice-24.2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.959021 vectice-24.2.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.963021 vectice-24.2.5.2/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.971021 vectice-24.2.5.2/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.975021 vectice-24.2.5.2/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/json_to_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/section.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.979021 vectice-24.2.5.2/src/vectice/autolog/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.979021 vectice-24.2.5.2/src/vectice/autolog/asset_services/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/catboost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/keras_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/lightgbm_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/pandas_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/pyspark_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/pytorch_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/sklearn_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/asset_services/vectice_asset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/autolog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/autolog_asset_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    31444 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/autolog_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/autolog/model_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    22308 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.983021 vectice-24.2.5.2/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/model_exp_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/model_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.983021 vectice-24.2.5.2/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.987021 vectice-24.2.5.2/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.987021 vectice-24.2.5.2/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/pyspark_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/no_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/resource/snowflake_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.987021 vectice-24.2.5.2/src/vectice/models/test_library/
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/test_library/binary_classification_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.991021 vectice-24.2.5.2/src/vectice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/services/iteration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/services/phase_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.991021 vectice-24.2.5.2/src/vectice/types/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.991021 vectice-24.2.5.2/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 13:40:07.000000 vectice-24.2.5.2/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:40:14.991021 vectice-24.2.5.2/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-15 13:40:14.000000 vectice-24.2.5.2/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-15 13:40:14.000000 vectice-24.2.5.2/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:40:14.000000 vectice-24.2.5.2/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-15 13:40:14.000000 vectice-24.2.5.2/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 13:40:14.000000 vectice-24.2.5.2/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.068563 vectice-24.2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 08:13:27.000000 vectice-24.2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-20 08:13:37.068563 vectice-24.2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 08:13:27.000000 vectice-24.2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-20 08:13:27.000000 vectice-24.2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 08:13:37.068563 vectice-24.2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-20 08:13:27.000000 vectice-24.2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.028563 vectice-24.2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.028563 vectice-24.2.6.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.036563 vectice-24.2.6.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21452 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.040563 vectice-24.2.6.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/json_to_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.044563 vectice-24.2.6.0/src/vectice/autolog/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.044563 vectice-24.2.6.0/src/vectice/autolog/asset_services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/catboost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/keras_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/lightgbm_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/pandas_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/pyspark_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/pytorch_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/sklearn_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/asset_services/vectice_asset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/autolog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/autolog_asset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31444 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/autolog_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/autolog/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22308 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.048563 vectice-24.2.6.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.048563 vectice-24.2.6.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.052563 vectice-24.2.6.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.052563 vectice-24.2.6.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/pyspark_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/no_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/resource/snowflake_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice/models/test_library/
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/test_library/binary_classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/services/iteration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/services/phase_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 08:13:27.000000 vectice-24.2.6.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:13:37.056563 vectice-24.2.6.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 08:13:37.000000 vectice-24.2.6.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-24.2.5.2/LICENSE` & `vectice-24.2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/PKG-INFO` & `vectice-24.2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.5.2
+Version: 24.2.6.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-24.2.5.2/pyproject.toml` & `vectice-24.2.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/setup.py` & `vectice-24.2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/__init__.py` & `vectice-24.2.6.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/_auth.py` & `vectice-24.2.6.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/attachment.py` & `vectice-24.2.6.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/client.py` & `vectice-24.2.6.0/src/vectice/api/client.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_api.py` & `vectice-24.2.6.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_attachment.py` & `vectice-24.2.6.0/src/vectice/api/gql_attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_dataset.py` & `vectice-24.2.6.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_entity_file.py` & `vectice-24.2.6.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_feature_flag.py` & `vectice-24.2.6.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_metric.py` & `vectice-24.2.6.0/src/vectice/api/gql_metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_model.py` & `vectice-24.2.6.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_organization.py` & `vectice-24.2.6.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_property.py` & `vectice-24.2.6.0/src/vectice/api/gql_property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/gql_user_workspace_api.py` & `vectice-24.2.6.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/http_error.py` & `vectice-24.2.6.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/http_error_handlers.py` & `vectice-24.2.6.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/iteration.py` & `vectice-24.2.6.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/__init__.py` & `vectice-24.2.6.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/artifact_version.py` & `vectice-24.2.6.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/code.py` & `vectice-24.2.6.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/code_version.py` & `vectice-24.2.6.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/dataset_register.py` & `vectice-24.2.6.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/dataset_representation.py` & `vectice-24.2.6.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/dataset_version.py` & `vectice-24.2.6.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/dataset_version_representation.py` & `vectice-24.2.6.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/files_metadata.py` & `vectice-24.2.6.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/iteration.py` & `vectice-24.2.6.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/json_to_class.py` & `vectice-24.2.6.0/src/vectice/api/json/json_to_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/last_assets.py` & `vectice-24.2.6.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/metric.py` & `vectice-24.2.6.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/model.py` & `vectice-24.2.6.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/model_register.py` & `vectice-24.2.6.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/model_representation.py` & `vectice-24.2.6.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/model_version.py` & `vectice-24.2.6.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/model_version_representation.py` & `vectice-24.2.6.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/paged_response.py` & `vectice-24.2.6.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/phase.py` & `vectice-24.2.6.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/project.py` & `vectice-24.2.6.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/property.py` & `vectice-24.2.6.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/public_config.py` & `vectice-24.2.6.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/requirement.py` & `vectice-24.2.6.0/src/vectice/api/json/requirement.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/user_and_workspace.py` & `vectice-24.2.6.0/src/vectice/api/json/user_and_workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/json/workspace.py` & `vectice-24.2.6.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/phase.py` & `vectice-24.2.6.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/project.py` & `vectice-24.2.6.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/rest_api.py` & `vectice-24.2.6.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/version.py` & `vectice-24.2.6.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/api/workspace.py` & `vectice-24.2.6.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/asset_services/__init__.py` & `vectice-24.2.6.0/src/vectice/autolog/asset_services/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/asset_services/catboost_service.py` & `vectice-24.2.6.0/src/vectice/autolog/asset_services/catboost_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/asset_services/keras_service.py` & `vectice-24.2.6.0/src/vectice/autolog/asset_services/keras_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/asset_services/lightgbm_service.py` & `vectice-24.2.6.0/src/vectice/autolog/asset_services/lightgbm_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/asset_services/metric_service.py` & `vectice-24.2.6.0/src/vectice/autolog/asset_services/metric_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/asset_services/pytorch_service.py` & `vectice-24.2.6.0/src/vectice/autolog/asset_services/pytorch_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/asset_services/sklearn_service.py` & `vectice-24.2.6.0/src/vectice/autolog/asset_services/sklearn_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/asset_services/vectice_asset_service.py` & `vectice-24.2.6.0/src/vectice/autolog/asset_services/vectice_asset_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/autolog.py` & `vectice-24.2.6.0/src/vectice/autolog/autolog.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/autolog_asset_factory.py` & `vectice-24.2.6.0/src/vectice/autolog/autolog_asset_factory.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/autolog/autolog_class.py` & `vectice-24.2.6.0/src/vectice/autolog/autolog_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/connection.py` & `vectice-24.2.6.0/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/__init__.py` & `vectice-24.2.6.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/additional_info.py` & `vectice-24.2.6.0/src/vectice/models/additional_info.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/attachment_container.py` & `vectice-24.2.6.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/code_version.py` & `vectice-24.2.6.0/src/vectice/models/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/dataset.py` & `vectice-24.2.6.0/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/iteration.py` & `vectice-24.2.6.0/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/metric.py` & `vectice-24.2.6.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/model.py` & `vectice-24.2.6.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/model_exp_tracker.py` & `vectice-24.2.6.0/src/vectice/models/model_exp_tracker.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/model_mlflow.py` & `vectice-24.2.6.0/src/vectice/models/model_mlflow.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/phase.py` & `vectice-24.2.6.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/project.py` & `vectice-24.2.6.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/property.py` & `vectice-24.2.6.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/representation/dataset_representation.py` & `vectice-24.2.6.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/representation/dataset_version_representation.py` & `vectice-24.2.6.0/src/vectice/models/representation/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/representation/model_representation.py` & `vectice-24.2.6.0/src/vectice/models/representation/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/representation/model_version_representation.py` & `vectice-24.2.6.0/src/vectice/models/representation/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/__init__.py` & `vectice-24.2.6.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/base.py` & `vectice-24.2.6.0/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/bigquery_resource.py` & `vectice-24.2.6.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/databricks_table_resource.py` & `vectice-24.2.6.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/description.py` & `vectice-24.2.6.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/file_resource.py` & `vectice-24.2.6.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/gcs_resource.py` & `vectice-24.2.6.0/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/__init__.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/base.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/metadata/source.py` & `vectice-24.2.6.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/no_resource.py` & `vectice-24.2.6.0/src/vectice/models/resource/no_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/s3_resource.py` & `vectice-24.2.6.0/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/resource/snowflake_resource.py` & `vectice-24.2.6.0/src/vectice/models/resource/snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/table.py` & `vectice-24.2.6.0/src/vectice/models/table.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/test_library/binary_classification_test.py` & `vectice-24.2.6.0/src/vectice/models/test_library/binary_classification_test.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/validation.py` & `vectice-24.2.6.0/src/vectice/models/validation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/models/workspace.py` & `vectice-24.2.6.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/services/iteration_service.py` & `vectice-24.2.6.0/src/vectice/services/iteration_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/services/phase_service.py` & `vectice-24.2.6.0/src/vectice/services/phase_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/types/version.py` & `vectice-24.2.6.0/src/vectice/types/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/utils/code_parser.py` & `vectice-24.2.6.0/src/vectice/utils/code_parser.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/utils/common_utils.py` & `vectice-24.2.6.0/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/utils/configuration.py` & `vectice-24.2.6.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/utils/dataframe_utils.py` & `vectice-24.2.6.0/src/vectice/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/utils/deprecation.py` & `vectice-24.2.6.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/utils/instance_helper.py` & `vectice-24.2.6.0/src/vectice/utils/instance_helper.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/utils/last_assets.py` & `vectice-24.2.6.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice/utils/logging_utils.py` & `vectice-24.2.6.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice.egg-info/PKG-INFO` & `vectice-24.2.6.0/src/vectice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.5.2
+Version: 24.2.6.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-24.2.5.2/src/vectice.egg-info/SOURCES.txt` & `vectice-24.2.6.0/src/vectice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vectice-24.2.5.2/src/vectice.egg-info/requires.txt` & `vectice-24.2.6.0/src/vectice.egg-info/requires.txt`

 * *Files identical despite different names*


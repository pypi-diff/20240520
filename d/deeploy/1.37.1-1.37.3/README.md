# Comparing `tmp/deeploy-1.37.1.tar.gz` & `tmp/deeploy-1.37.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeploy-1.37.1.tar", last modified: Wed Apr  3 13:41:30 2024, max compression
+gzip compressed data, was "deeploy-1.37.3.tar", last modified: Mon May 20 11:32:39 2024, max compression
```

## Comparing `deeploy-1.37.1.tar` & `deeploy-1.37.3.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.552092 deeploy-1.37.1/
--rw-rw-rw-   0 root         (0) root         (0)    11346 2024-04-03 13:31:52.000000 deeploy-1.37.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      926 2024-04-03 13:41:30.552092 deeploy-1.37.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1900 2024-04-03 13:31:52.000000 deeploy-1.37.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.528092 deeploy-1.37.1/deeploy/
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.532092 deeploy-1.37.1/deeploy/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.532092 deeploy-1.37.1/deeploy/cli/custom_instances/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3608 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/model.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/model_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     7147 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deeploycli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.532092 deeploy-1.37.1/deeploy/cli/deploy_instances/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deploy_instances/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     4894 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/parsers/parser_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/parsers/parser_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/parsers/parser_transformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/templates/explainer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/templates/explainer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/templates/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/templates/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/templates/transformer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/templates/transformer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/wrappers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/wrappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/wrappers/explainer_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/wrappers/model_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1748 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/wrappers/transformer_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)    20741 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/common/
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/common/constants/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/constants/pytorch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/common/functions/
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/functions/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.540092 deeploy-1.37.1/deeploy/deepfair/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/deepfair/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6549 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/deepfair/fair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.540092 deeploy-1.37.1/deeploy/enums/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/algo.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/auth_type.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/explainer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/prediction_version.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/qf.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/query_param.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/transformer_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.544092 deeploy-1.37.1/deeploy/fairsd/
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30522 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/algorithms.py
--rw-rw-rw-   0 root         (0) root         (0)    13196 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/discretization.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/qualitymeasures.py
--rw-rw-rw-   0 root         (0) root         (0)     8381 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/searchspace.py
--rw-rw-rw-   0 root         (0) root         (0)     7701 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/sgdescription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.548092 deeploy-1.37.1/deeploy/models/
--rw-rw-rw-   0 root         (0) root         (0)     1543 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/actual_response.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/client_options.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_actuals.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_azure_ml_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     6088 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_deployment_base.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_explainer_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2295 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_model_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_sagemaker_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_transformer_reference.py
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/feature.py
--rw-rw-rw-   0 root         (0) root         (0)     3455 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/get_prediction_logs_options.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/metadata_json.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/prediction_log.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/reference_json.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_azure_ml_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_deployment_base.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_deployment_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_sagemaker_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.548092 deeploy-1.37.1/deeploy/services/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16781 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/deeploy_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4727 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainer_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.548092 deeploy-1.37.1/deeploy/services/explainers/
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/alibi.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/base_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1382 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/omni_tabular.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/shap.py
--rw-rw-rw-   0 root         (0) root         (0)     3432 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/file_service.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/git_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3369 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/model_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.552092 deeploy-1.37.1/deeploy/services/models/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/onnx.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/pytorch.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/sklearn.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/tensorflow.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/triton.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/xgboost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.528092 deeploy-1.37.1/deeploy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      926 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3647 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      200 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 13:41:30.552092 deeploy-1.37.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1806 2024-04-03 13:31:52.000000 deeploy-1.37.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.552092 deeploy-1.37.1/test/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-03 13:31:52.000000 deeploy-1.37.1/test/test_deeploy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2024-05-20 11:32:37.000000 deeploy-1.37.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-20 11:32:39.220363 deeploy-1.37.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2024-05-20 11:32:37.000000 deeploy-1.37.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy/
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy/cli/custom_instances/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/model_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/custom_instances/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7165 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deeploycli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy/cli/deploy_instances/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deploy_instances/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4894 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/parsers/parser_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/parsers/parser_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/parsers/parser_transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/templates/explainer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/templates/explainer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/templates/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/templates/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/templates/transformer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/templates/transformer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/cli/wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/wrappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/wrappers/explainer_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/wrappers/model_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/cli/wrappers/transformer_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)    20741 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/common/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/common/constants/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/constants/pytorch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/common/functions/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/common/functions/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/deepfair/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/deepfair/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6549 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/deepfair/fair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.212363 deeploy-1.37.3/deeploy/enums/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/algo.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/auth_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/explainer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/prediction_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/qf.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/query_param.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/enums/transformer_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.216363 deeploy-1.37.3/deeploy/fairsd/
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30522 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/algorithms.py
+-rw-rw-rw-   0 root         (0) root         (0)    13196 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/discretization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/qualitymeasures.py
+-rw-rw-rw-   0 root         (0) root         (0)     8381 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/searchspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     7701 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/fairsd/sgdescription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/deeploy/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/actual_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/client_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_actuals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_azure_ml_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     6608 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_deployment_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_explainer_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2295 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_model_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_sagemaker_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/create_transformer_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/get_prediction_logs_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/metadata_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/prediction_log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/reference_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_azure_ml_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     6807 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_deployment_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_deployment_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/update_sagemaker_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/models/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/deeploy/services/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16781 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/deeploy_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainer_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/deeploy/services/explainers/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/alibi.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/base_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/omni_tabular.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/explainers/shap.py
+-rw-rw-rw-   0 root         (0) root         (0)     3432 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/file_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/git_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/model_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/deeploy/services/models/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/onnx.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/pytorch.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/sklearn.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/tensorflow.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/triton.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-20 11:32:37.000000 deeploy-1.37.3/deeploy/services/models/xgboost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.208363 deeploy-1.37.3/deeploy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3647 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-20 11:32:39.000000 deeploy-1.37.3/deeploy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 11:32:39.224363 deeploy-1.37.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2024-05-20 11:32:37.000000 deeploy-1.37.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:32:39.220363 deeploy-1.37.3/test/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-20 11:32:37.000000 deeploy-1.37.3/test/test_deeploy.py
```

### Comparing `deeploy-1.37.1/LICENSE` & `deeploy-1.37.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/PKG-INFO` & `deeploy-1.37.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeploy
-Version: 1.37.1
+Version: 1.37.3
 Summary: The official Deeploy client for Python
 Home-page: https://gitlab.com/deeploy-ml/deeploy-python-client
 Author: Tim Kleinloog
 Author-email: opensource@deeploy.ml
 License: UNKNOWN
 Project-URL: Documentation, https://deeploy-ml.gitlab.io/deeploy-python-client/
 Project-URL: Deeploy website, https://deeploy.ml
```

### Comparing `deeploy-1.37.1/README.md` & `deeploy-1.37.3/README.md`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/__init__.py` & `deeploy-1.37.3/deeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/custom_instances/explainer.py` & `deeploy-1.37.3/deeploy/cli/custom_instances/explainer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/custom_instances/model.py` & `deeploy-1.37.3/deeploy/cli/custom_instances/model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/custom_instances/model_repository.py` & `deeploy-1.37.3/deeploy/cli/custom_instances/model_repository.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/custom_instances/transformer.py` & `deeploy-1.37.3/deeploy/cli/custom_instances/transformer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/deeploycli.py` & `deeploy-1.37.3/deeploy/cli/deeploycli.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from enum import Enum
 from typing import Dict
 
 import click
 from jinja2 import Environment, PackageLoader
 
 from deeploy._version import __version__
+from deeploy.cli.utils import validate_project_name
 
 ALLOWED_TYPES = ["model", "explainer", "transformer"]
 
 env = Environment(loader=PackageLoader("deeploy", "cli/templates"), autoescape=True)
 
 
 class Instances(Enum):
@@ -31,43 +32,48 @@
 
 @cli.command()
 @click.option(
     "--name",
     "-n",
     prompt="Name of Project",
     help="Provide name of the project to be initialized.",
+    callback=validate_project_name
 )
 @click.option(
     "--initialization",
     "-i",
     default=["model"],
-    help="Provide initialization types,\
-          eg. -i model -i transformer -> For just model and transformer, \
-            -i model -i explainer -i transformer -> For all three",
+    help="State for which components the templates should be generated.\n\
+        Three options: -i model -i transformer -i explainer.\n\
+        Select one or more.",
     multiple=True,
 )
 def generate_template(name, initialization):
     """Generates Sample Docker Image Template for Custom Docker Image"""
     # catch unknown type
     if not set(initialization).issubset(set(ALLOWED_TYPES)):
         raise RuntimeError("Initialization types can only be model, explainer or transformer.")
+    
+    projectname = name
 
-    projectname = "custom_" + name
-    click.echo(f"Creating Project '{name}'.")
+    click.echo(f"Creating Project '{projectname}'.")
     os.makedirs(projectname, exist_ok=True)
 
     template_vars = {
         "projectname": projectname,
         "model": True if Instances.model.value in initialization else False,
         "explainer": True if Instances.explainer.value in initialization else False,
         "transformer": True if Instances.transformer.value in initialization else False,
     }
     generate_readme(projectname, template_vars)
     click.echo("Generated README.")
 
+    generate_metadata(projectname)
+    click.echo("Generated metadata.")
+
     generate_script(projectname, template_vars)
     click.echo("Generated build script.")
 
     if Instances.explainer.value in initialization:
         response = generate_instance(projectname, template_vars, Instances.explainer.value)
         if response:
             click.echo("Docker Image Template for explainer is generated.")
@@ -84,15 +90,22 @@
     if Instances.transformer.value in initialization:
         response = generate_instance(projectname, template_vars, Instances.transformer.value)
         if response:
             click.echo(f"Docker Image Template for {Instances.transformer.value} is generated.")
         else:
             click.echo(f"Skipping {Instances.transformer.value} since the files already exists")
 
-    click.echo(f"All templates for project '{name}' have been created!")
+    click.echo(f"All templates for project '{projectname}' have been created!")
+
+def generate_metadata(projectname: str):
+    """Generates metadata.json file"""
+    templates_metadata = env.get_template("metadata.json.j2")
+    content_metadata = templates_metadata.render({})
+    with open(os.path.join(projectname, "metadata.json"), "w+") as metadata_file:
+        metadata_file.write(content_metadata)
 
 
 def generate_readme(projectname: str, template_vars: Dict):
     """Generates Primary Readme file"""
     templates_readme = env.get_template("README.md.j2")
     content_readme = templates_readme.render(template_vars)
     with open(os.path.join(projectname, "README.md"), "w+") as readme_file:
@@ -112,84 +125,75 @@
     template_vars["instance"] = instance_type
     generate_folder = projectname + "_" + instance_type
     if not os.path.exists(os.path.join(projectname, generate_folder)):
         os.mkdir(os.path.join(projectname, generate_folder))
     else:
         return False
 
-    if not os.path.exists(
-        os.path.join(projectname, generate_folder, f"{instance_type}_" + projectname)
-    ):
-        os.mkdir(os.path.join(projectname, generate_folder, f"{instance_type}_" + projectname))
 
     # generate sample files
-    templates_dockerfile = env.get_template(f"{instance_type}/DOCKERFILE.j2")
+    templates_dockerfile = env.get_template(f"{instance_type}/Dockerfile.j2")
     templates_main = env.get_template(f"{instance_type}/__main__.py.j2")
     templates_sample_wrapper = env.get_template(f"{instance_type}/sample_{instance_type}.py.j2")
     templates_requirements = env.get_template(f"{instance_type}/requirements.txt.j2")
 
     content_dockerfile = templates_dockerfile.render(template_vars)
-    with open(os.path.join(projectname, generate_folder, "DOCKERFILE"), "w+") as file:
+    with open(os.path.join(projectname, generate_folder, "Dockerfile"), "w+") as file:
         file.write(content_dockerfile)
 
     content_requirements = templates_requirements.render(template_vars)
     with open(
         os.path.join(
             projectname,
             generate_folder,
-            f"{instance_type}_" + projectname,
             "requirements.txt",
         ),
         "w+",
     ) as file:
         file.write(content_requirements)
 
     content_main = templates_main.render(template_vars)
     with open(
         os.path.join(
             projectname,
             generate_folder,
-            f"{instance_type}_" + projectname,
             "__main__.py",
         ),
         "w+",
     ) as file:
         file.write(content_main)
 
     content_sample_wrapper = templates_sample_wrapper.render(template_vars)
     with open(
         os.path.join(
             projectname,
             generate_folder,
-            f"{instance_type}_" + projectname,
             f"sample_{instance_type}.py",
         ),
         "w+",
     ) as file:
         file.write(content_sample_wrapper)
 
     # copy model and explainer objects
     pkgdir = sys.modules[str(sys.modules[__name__].__name__).split(".")[0]].__path__[0]
     if instance_type == Instances.explainer.value:
         shutil.copy(
             pkgdir + f"/cli/templates/{instance_type}/{instance_type}.dill",
             os.path.join(
                 projectname,
                 generate_folder,
-                f"{instance_type}_" + projectname,
                 f"{instance_type}.dill",
             ),
         )
     if instance_type == Instances.model.value:
         shutil.copy(
             pkgdir + f"/cli/templates/{instance_type}/{instance_type}.bst",
             os.path.join(
                 projectname,
                 generate_folder,
-                f"{instance_type}_" + projectname,
                 f"{instance_type}.bst",
             ),
         )
 
     # generate reference
     if not os.path.exists(os.path.join(projectname, instance_type)):
         os.mkdir(os.path.join(projectname, instance_type))
```

### Comparing `deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_explainer.py` & `deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_explainer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_model.py` & `deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_transformer.py` & `deeploy-1.37.3/deeploy/cli/deploy_instances/deeploy_transformer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/interface.py` & `deeploy-1.37.3/deeploy/cli/interface.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/parsers/parser_explainer.py` & `deeploy-1.37.3/deeploy/cli/parsers/parser_explainer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/parsers/parser_model.py` & `deeploy-1.37.3/deeploy/cli/parsers/parser_model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/parsers/parser_transformer.py` & `deeploy-1.37.3/deeploy/cli/parsers/parser_transformer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/utils.py` & `deeploy-1.37.3/deeploy/cli/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import re
+
+import click
+
+
 class Model:
     def __init__(self, f, out_names):
         self.f = f
         self.out_names = out_names
 
 
 def convert_to_model(val):
@@ -21,7 +26,13 @@
 
 def use_transformer(predictor_host: str):
     return predictor_host.replace("predictor", "transformer")
 
 
 def use_predictor(predictor_host: str):
     return predictor_host.replace("transformer", "predictor")
+
+def validate_project_name(ctx, param, project_name):
+    if re.match(r'\w+$', project_name):
+        return project_name
+    else:
+        raise click.BadParameter("Name can only include alphanumeric characters and underscores")
```

### Comparing `deeploy-1.37.1/deeploy/cli/wrappers/explainer_wrapper.py` & `deeploy-1.37.3/deeploy/cli/wrappers/explainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/wrappers/model_wrapper.py` & `deeploy-1.37.3/deeploy/cli/wrappers/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/cli/wrappers/transformer_wrapper.py` & `deeploy-1.37.3/deeploy/cli/wrappers/transformer_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/client.py` & `deeploy-1.37.3/deeploy/client.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/common/constants/pytorch.py` & `deeploy-1.37.3/deeploy/common/constants/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/common/functions/functions.py` & `deeploy-1.37.3/deeploy/common/functions/functions.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/deepfair/fair.py` & `deeploy-1.37.3/deeploy/deepfair/fair.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/fairsd/algorithms.py` & `deeploy-1.37.3/deeploy/fairsd/algorithms.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/fairsd/discretization.py` & `deeploy-1.37.3/deeploy/fairsd/discretization.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/fairsd/qualitymeasures.py` & `deeploy-1.37.3/deeploy/fairsd/qualitymeasures.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/fairsd/searchspace.py` & `deeploy-1.37.3/deeploy/fairsd/searchspace.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/fairsd/sgdescription.py` & `deeploy-1.37.3/deeploy/fairsd/sgdescription.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/__init__.py` & `deeploy-1.37.3/deeploy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/client_options.py` & `deeploy-1.37.3/deeploy/models/client_options.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_actuals.py` & `deeploy-1.37.3/deeploy/models/create_actuals.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_azure_ml_deployment.py` & `deeploy-1.37.3/deeploy/models/create_azure_ml_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_deployment.py` & `deeploy-1.37.3/deeploy/models/create_deployment.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 
 class CreateDeployment(CreateDeploymentBase):
     """Class that contains the options for creating a deployment"""
 
     model_serverless: bool = False
     """bool, optional: whether to deploy the model in a serverless fashion. Defaults to False"""
-    model_credentials_id: Optional[str] = None
-    """str, optional: uuid of credentials generated in Deeploy to access private Blob storage or Docker repo"""
+    model_blob_credentials_id: Optional[str] = None
+    """str, optional: uuid of credentials generated in Deeploy to access private Blob storage"""
+    model_docker_credentials_id: Optional[str] = None
+    """str, optional: uuid of credentials generated in Deeploy to access private Docker repo"""
     model_instance_type: Optional[str] = None
     """str, optional: the preferred instance type for the model"""
     model_mem_request: Optional[int] = None
     """int, optional: RAM request of model pod, in Megabytes."""
     model_mem_limit: Optional[int] = None
     """int, optional: RAM limit of model pod, in Megabytes."""
     model_cpu_request: Optional[float] = None
@@ -24,16 +26,18 @@
     """float, optional: GPU request of model pod, in number of GPUs."""
     model_env: Optional[dict] = None
     """dict, optional: env variables to pass to model container key is env var name, value is env var value"""
     model_args: Optional[dict] = None
     """dict, optional: arguments to pass to model container key is argument name, value is argument value"""
     explainer_serverless: bool = False
     """bool, optional: whether to deploy the explainer in a serverless fashion. Defaults to False"""
-    explainer_credentials_id: Optional[str] = None
-    """str, optional: Credential id of credential generated in Deeploy to access private Blob storage or Docker repo"""
+    explainer_blob_credentials_id: Optional[str] = None
+    """str, optional: Credential id of credential generated in Deeploy to access private Blob storage"""
+    explainer_docker_credentials_id: Optional[str] = None
+    """str, optional: Credential id of credential generated in Deeploy to access private Docker repo"""
     explainer_instance_type: Optional[str] = None
     """str, optional: The preferred instance type for the explainer pod."""
     explainer_mem_request: Optional[int] = None
     """int, optional: RAM request of explainer pod, in Megabytes."""
     explainer_mem_limit: Optional[int] = None
     """int, optional: RAM limit of explainer pod, in Megabytes."""
     explainer_cpu_request: Optional[float] = None
@@ -44,16 +48,16 @@
     """float, optional: GPU request of explainer pod, in number of GPUs."""
     explainer_env: Optional[dict] = None
     """dict, optional: env variables to pass to explainer container key is env var name, value is env var value"""
     explainer_args: Optional[dict] = None
     """dict, optional: arguments to pass to explainer container key is argument name, value is argument value"""
     transformer_serverless: bool = False
     """bool, optional: whether to deploy the transformer in a serverless fashion. Defaults to False"""
-    transformer_credentials_id: Optional[str] = None
-    """str, optional: Credential id of credential generated in Deeploy to access private Blob storage or Docker repo"""
+    transformer_docker_credentials_id: Optional[str] = None
+    """str, optional: Credential id of credential generated in Deeploy to access private Docker repo"""
     transformer_instance_type: Optional[str] = None
     """str, optional: The preferred instance type for the transformer pod."""
     transformer_mem_request: Optional[int] = None
     """int, optional: RAM request of transformer pod, in Megabytes."""
     transformer_mem_limit: Optional[int] = None
     """int, optional: RAM limit of transformer pod, in Megabytes."""
     transformer_cpu_request: Optional[float] = None
@@ -67,35 +71,38 @@
     transformer_args: Optional[dict] = None
     """dict, optional: arguments to pass to transformer container key is argument name, value is argument value"""
 
     def to_request_body(self) -> Dict:
         return {
             **super().to_request_body(),
             "modelServerless": self.model_serverless,
-            "modelCredentialsId": self.model_credentials_id,
+            "modelBlobCredentialsId": self.model_blob_credentials_id,
+            "modelDockerCredentialsId": self.model_docker_credentials_id,
             "modelInstanceType": self.model_instance_type,
             "modelMemRequest": self.model_mem_request,
             "modelMemLimit": self.model_mem_limit,
             "modelCpuRequest": self.model_cpu_request,
             "modelCpuLimit": self.model_cpu_limit,
             "modelGpuRequest": self.model_gpu_request,
             "modelEnv": self.model_env,
             "modelArgs": self.model_args,
             "explainerServerless": self.explainer_serverless,
             "explainerInstanceType": self.explainer_instance_type,
-            "explainerCredentialsId": self.explainer_credentials_id,
+            "explainerBlobCredentialsId": self.explainer_blob_credentials_id,
+            "explainerDockerCredentialsId": self.explainer_docker_credentials_id,
             "explainerMemRequest": self.explainer_mem_request,
             "explainerMemLimit": self.explainer_mem_limit,
             "explainerCpuRequest": self.explainer_cpu_request,
             "explainerCpuLimit": self.explainer_cpu_limit,
             "explainerGpuRequest": self.explainer_gpu_request,
             "explainerEnv": self.explainer_env,
             "explainerArgs": self.explainer_args,
             "transformerServerless": self.transformer_serverless,
-            "transformerCredentialsId": self.transformer_credentials_id,
+            "transformerBlobCredentialsId": None,
+            "transformerDockerCredentialsId": self.transformer_docker_credentials_id,
             "transformerInstanceType": self.transformer_instance_type,
             "transformerMemRequest": self.transformer_mem_request,
             "transformerMemLimit": self.transformer_mem_limit,
             "transformerCpuRequest": self.transformer_cpu_request,
             "transformerCpuLimit": self.transformer_cpu_limit,
             "transformerGpuRequest": self.transformer_gpu_request,
             "transformerEnv": self.transformer_env,
```

### Comparing `deeploy-1.37.1/deeploy/models/create_deployment_base.py` & `deeploy-1.37.3/deeploy/models/create_deployment_base.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_evaluation.py` & `deeploy-1.37.3/deeploy/models/create_evaluation.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_explainer_reference.py` & `deeploy-1.37.3/deeploy/models/create_explainer_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_metadata.py` & `deeploy-1.37.3/deeploy/models/create_metadata.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_model_reference.py` & `deeploy-1.37.3/deeploy/models/create_model_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_sagemaker_deployment.py` & `deeploy-1.37.3/deeploy/models/create_sagemaker_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/create_transformer_reference.py` & `deeploy-1.37.3/deeploy/models/create_transformer_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/deployment.py` & `deeploy-1.37.3/deeploy/models/deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/get_prediction_logs_options.py` & `deeploy-1.37.3/deeploy/models/get_prediction_logs_options.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/prediction_log.py` & `deeploy-1.37.3/deeploy/models/prediction_log.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/reference_json.py` & `deeploy-1.37.3/deeploy/models/reference_json.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/update_azure_ml_deployment.py` & `deeploy-1.37.3/deeploy/models/update_azure_ml_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/update_deployment.py` & `deeploy-1.37.3/deeploy/models/update_deployment.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 
 class UpdateDeployment(UpdateDeploymentBase):
     """Class that contains the options for updating a Deployment"""
 
     model_serverless: Optional[bool] = None
     """bool, optional: whether to deploy the model in a serverless fashion. Defaults to False"""
-    model_credentials_id: Optional[str] = None
-    """str, optional: uuid of credentials generated in Deeploy to access private Blob storage or Docker repo"""
+    model_blob_credentials_id: Optional[str] = None
+    """str, optional: uuid of credentials generated in Deeploy to access private Blob storage"""
+    model_docker_credentials_id: Optional[str] = None
+    """str, optional: uuid of credentials generated in Deeploy to access private Docker repo"""
     model_instance_type: Optional[str] = None
     """str, optional: the preferred instance type for the model"""
     model_mem_request: Optional[int] = None
     """int, optional: RAM request of model pod, in Megabytes."""
     model_mem_limit: Optional[int] = None
     """int, optional: RAM limit of model pod, in Megabytes."""
     model_cpu_request: Optional[float] = None
@@ -24,16 +26,18 @@
     """float, optional: GPU request of model pod, in number of GPUs."""
     model_env: Optional[dict] = None
     """dict, optional: env variables to pass to model container key is env var name, value is env var value"""
     model_args: Optional[dict] = None
     """dict, optional: arguments to pass to model container key is argument name, value is argument value"""
     explainer_serverless: Optional[bool] = None
     """bool, optional: whether to deploy the explainer in a serverless fashion. Defaults to False"""
-    explainer_credentials_id: Optional[str] = None
-    """str, optional: Credential id of credential generated in Deeploy to access private Blob storage or Docker repo"""
+    explainer_blob_credentials_id: Optional[str] = None
+    """str, optional: Credential id of credential generated in Deeploy to access private Blob storage"""
+    explainer_docker_credentials_id: Optional[str] = None
+    """str, optional: Credential id of credential generated in Deeploy to access private Docker repo"""
     explainer_instance_type: Optional[str] = None
     """str, optional: The preferred instance type for the explainer pod."""
     explainer_mem_request: Optional[int] = None
     """int, optional: RAM request of explainer pod, in Megabytes."""
     explainer_mem_limit: Optional[int] = None
     """int, optional: RAM limit of explainer pod, in Megabytes."""
     explainer_cpu_request: Optional[float] = None
@@ -44,16 +48,16 @@
     """float, optional: GPU request of explainer pod, in number of GPUs."""
     explainer_env: Optional[dict] = None
     """dict, optional: env variables to pass to explainer container key is env var name, value is env var value"""
     explainer_args: Optional[dict] = None
     """dict, optional: arguments to pass to explainer container key is argument name, value is argument value"""
     transformer_serverless: Optional[bool] = None
     """bool, optional: whether to deploy the transformer in a serverless fashion. Defaults to False"""
-    transformer_credentials_id: Optional[str] = None
-    """str, optional: Credential id of credential generated in Deeploy to access private Blob storage or Docker repo"""
+    transformer_docker_credentials_id: Optional[str] = None
+    """str, optional: Credential id of credential generated in Deeploy to access private Docker repo"""
     transformer_instance_type: Optional[str] = None
     """str, optional: The preferred instance type for the transformer pod."""
     transformer_mem_request: Optional[int] = None
     """int, optional: RAM request of transformer pod, in Megabytes."""
     transformer_mem_limit: Optional[int] = None
     """int, optional: RAM limit of transformer pod, in Megabytes."""
     transformer_cpu_request: Optional[float] = None
@@ -67,35 +71,38 @@
     transformer_args: Optional[dict] = None
     """dict, optional: arguments to pass to transformer container key is argument name, value is argument value"""
 
     def to_request_body(self) -> Dict:
         request_body = {
             **super().to_request_body(),
             "modelServerless": self.model_serverless,
-            "modelCredentialsId": self.model_credentials_id,
+            "modelBlobCredentialsId": self.model_blob_credentials_id,
+            "modelDockerCredentialsId": self.model_docker_credentials_id,
             "modelInstanceType": self.model_instance_type,
             "modelMemRequest": self.model_mem_request,
             "modelMemLimit": self.model_mem_limit,
             "modelCpuRequest": self.model_cpu_request,
             "modelCpuLimit": self.model_cpu_limit,
             "modelGpuRequest": self.model_gpu_request,
             "modelEnv": self.model_env,
             "modelArgs": self.model_args,
             "explainerServerless": self.explainer_serverless,
             "explainerInstanceType": self.explainer_instance_type,
-            "explainerCredentialsId": self.explainer_credentials_id,
+            "explainerBlobCredentialsId": self.explainer_blob_credentials_id,
+            "explainerDockerCredentialsId": self.explainer_docker_credentials_id,
             "explainerMemRequest": self.explainer_mem_request,
             "explainerMemLimit": self.explainer_mem_limit,
             "explainerCpuRequest": self.explainer_cpu_request,
             "explainerCpuLimit": self.explainer_cpu_limit,
             "explainerGpuRequest": self.explainer_gpu_request,
             "explainerEnv": self.explainer_env,
             "explainerArgs": self.explainer_args,
             "transformerServerless": self.transformer_serverless,
-            "transformerCredentialsId": self.transformer_credentials_id,
+            "transformerBlobCredentialsId": None,
+            "transformerDockerCredentialsId": self.transformer_docker_credentials_id,
             "transformerInstanceType": self.transformer_instance_type,
             "transformerMemRequest": self.transformer_mem_request,
             "transformerMemLimit": self.transformer_mem_limit,
             "transformerCpuRequest": self.transformer_cpu_request,
             "transformerCpuLimit": self.transformer_cpu_limit,
             "transformerGpuRequest": self.transformer_gpu_request,
             "transformerEnv": self.transformer_env,
```

### Comparing `deeploy-1.37.1/deeploy/models/update_deployment_base.py` & `deeploy-1.37.3/deeploy/models/update_deployment_base.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/update_deployment_description.py` & `deeploy-1.37.3/deeploy/models/update_deployment_description.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/models/update_sagemaker_deployment.py` & `deeploy-1.37.3/deeploy/models/update_sagemaker_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/deeploy_service.py` & `deeploy-1.37.3/deeploy/services/deeploy_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/explainer_wrapper.py` & `deeploy-1.37.3/deeploy/services/explainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/explainers/alibi.py` & `deeploy-1.37.3/deeploy/services/explainers/alibi.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/explainers/omni_tabular.py` & `deeploy-1.37.3/deeploy/services/explainers/omni_tabular.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/explainers/shap.py` & `deeploy-1.37.3/deeploy/services/explainers/shap.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/file_service.py` & `deeploy-1.37.3/deeploy/services/file_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/git_service.py` & `deeploy-1.37.3/deeploy/services/git_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/model_wrapper.py` & `deeploy-1.37.3/deeploy/services/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/models/pytorch.py` & `deeploy-1.37.3/deeploy/services/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/models/sklearn.py` & `deeploy-1.37.3/deeploy/services/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/models/tensorflow.py` & `deeploy-1.37.3/deeploy/services/models/tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy/services/models/xgboost.py` & `deeploy-1.37.3/deeploy/services/models/xgboost.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/deeploy.egg-info/PKG-INFO` & `deeploy-1.37.3/deeploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeploy
-Version: 1.37.1
+Version: 1.37.3
 Summary: The official Deeploy client for Python
 Home-page: https://gitlab.com/deeploy-ml/deeploy-python-client
 Author: Tim Kleinloog
 Author-email: opensource@deeploy.ml
 License: UNKNOWN
 Project-URL: Documentation, https://deeploy-ml.gitlab.io/deeploy-python-client/
 Project-URL: Deeploy website, https://deeploy.ml
```

### Comparing `deeploy-1.37.1/deeploy.egg-info/SOURCES.txt` & `deeploy-1.37.3/deeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.1/setup.py` & `deeploy-1.37.3/setup.py`

 * *Files identical despite different names*


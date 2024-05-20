# Comparing `tmp/sarus_data_spec_public-4.0.1.tar.gz` & `tmp/sarus_data_spec_public-4.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-4.0.1.tar", last modified: Fri May 17 15:57:11 2024, max compression
+gzip compressed data, was "sarus_data_spec_public-4.0.2.dev0.tar", last modified: Mon May 20 12:26:15 2024, max compression
```

## Comparing `sarus_data_spec_public-4.0.1.tar` & `sarus_data_spec_public-4.0.2.dev0.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.683242 sarus_data_spec_public-4.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      656 2024-05-17 15:57:11.683242 sarus_data_spec_public-4.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.641242 sarus_data_spec_public-4.0.1/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      942 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.642242 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8510 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     7389 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     4266 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.643242 sarus_data_spec_public-4.0.1/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    21819 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.645242 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22994 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
--rw-rw-rw-   0 root         (0) root         (0)    11623 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.647242 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17255 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     5717 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/recursive_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    28910 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5355 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.648242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7629 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32667 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6724 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/cache_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.649242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.649242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.650242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.650242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7120 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.651242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.654242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23600 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)    10321 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)    21505 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/optbinning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.655242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
--rw-rw-rw-   0 root         (0) root         (0)    31872 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
--rw-rw-rw-   0 root         (0) root         (0)    78764 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    37561 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)    34976 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.657242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/
--rw-rw-rw-   0 root         (0) root         (0)     4162 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26932 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)    13453 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
--rw-rw-rw-   0 root         (0) root         (0)    14139 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     6514 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.660242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20941 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38069 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12690 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8598 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    25448 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    13273 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.664242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17193 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
--rw-rw-rw-   0 root         (0) root         (0)    13308 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11420 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/push_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     8639 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.664242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sampling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)     9522 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11403 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    13558 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
--rw-rw-rw-   0 root         (0) root         (0)    27871 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.665242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.666242 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8985 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/bigdata.py
--rw-rw-rw-   0 root         (0) root         (0)     5703 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/queries.py
--rw-rw-rw-   0 root         (0) root         (0)    10574 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.680242 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     1507 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     1712 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2160 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     1964 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)     3941 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9653 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)     2557 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4178 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     1417 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     1739 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2169 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     1777 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     1449 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)     2416 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4839 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     1634 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     1545 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2606 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)     3904 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9843 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      694 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)     2611 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4578 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2154 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    11222 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32747 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)     3258 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6181 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7135 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)    17096 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    49955 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)     9784 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    30590 2024-05-17 15:57:00.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    13753 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4757 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17261 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.681242 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14527 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5606 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    40753 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   123255 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    40943 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 15:57:11.683242 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      656 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9149 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-17 15:57:11.000000 sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     6984 2024-05-17 15:57:11.685242 sarus_data_spec_public-4.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1186 2024-05-17 15:56:17.000000 sarus_data_spec_public-4.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.184986 sarus_data_spec_public-4.0.2.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-20 12:26:15.184986 sarus_data_spec_public-4.0.2.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.141986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      947 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.143986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8510 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     7389 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     4364 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.144986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    21819 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.146986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22994 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11623 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.148986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17255 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/recursive_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    28910 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5355 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9582 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.149986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7850 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32667 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6724 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/cache_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.149986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.150986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.151986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.151986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7120 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.151986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.155986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24946 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10321 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)    21505 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/optbinning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.156986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    31872 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)    78764 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    37561 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)    34976 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.158986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26932 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13453 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14139 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     6514 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.160986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20941 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38069 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25448 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    13273 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.164986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17193 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    13308 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/push_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8639 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.165986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)     9522 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11403 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    13558 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    27871 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.166986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.166986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8985 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/bigdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5703 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10574 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.181986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)     3941 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9653 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)     3904 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9843 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      694 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32747 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)     3258 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7135 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)    17096 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    49955 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)     9784 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30590 2024-05-20 12:26:04.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    13753 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4757 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17261 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.182986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14527 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    40753 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   123255 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    40943 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 12:26:15.184986 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9149 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-20 12:26:15.000000 sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6984 2024-05-20 12:26:15.185986 sarus_data_spec_public-4.0.2.dev0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2024-05-20 12:25:41.000000 sarus_data_spec_public-4.0.2.dev0/setup.py
```

### Comparing `sarus_data_spec_public-4.0.1/PKG-INFO` & `sarus_data_spec_public-4.0.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.1
+Version: 4.0.2.dev0
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/__init__.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "VariantConstraint",
 ]
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = "sarus_data_spec"
-VERSION: Final[str] = "4.0.1"
+VERSION: Final[str] = "4.0.2.dev0"
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == "sarus_data_spec.context.worker":
```

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/conversion.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/attribute.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/bounds.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/constants.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,7 +164,11 @@
 # Model checkpoints
 TRAIN_STATE = "state"
 MODEL_NAME = "model_name"
 PROMPT = "prompt"
 
 # relationship spec
 SHARED_ID_SPACES = "shared-id-spaces"
+
+
+# sarus default output (for empty mock/synthetic)
+SARUS_DEFAULT_OUTPUT = "sarus_default_output"
```

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/context/public.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataset.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_rewriter/utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_rewriter/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/recursive_validator.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/recursive_validator.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/signature.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/factory.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/json_serialisation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import base64
 from datetime import date, datetime, time, timedelta, timezone
 from typing import Any
 import json
 import sys
 
 from dateutil.parser import parse
 import numpy as np
 import pandas as pd
+import pyarrow as pa
+import pyarrow.ipc as ipc
 
 
 class SarusJSONEncoder(json.JSONEncoder):
     def default(self, obj: Any) -> Any:
         if isinstance(obj, np.ndarray):
             return {"_type": "numpy.ndarray", "data": obj.tolist()}
         elif isinstance(obj, pd.DataFrame):
@@ -99,14 +102,26 @@
                 "_type": "range",
                 "data": {
                     '"start"': obj.start,
                     '"stop"': obj.stop,
                     '"step"': obj.step,
                 },
             }
+        elif isinstance(obj, pa.Table):
+            sink = pa.BufferOutputStream()
+            writer = ipc.new_stream(sink, obj.schema)
+            writer.write_table(obj)
+            writer.close()
+            serialized_data = (
+                sink.getvalue()
+            )  # This is the serialized data in a byte array format
+            base64_encoded_data = base64.b64encode(serialized_data).decode(
+                "utf-8"
+            )
+            return {"_type": "pa.Table", "data": base64_encoded_data}
         return super().default(obj)
 
     def encode_obj(self, obj: Any) -> Any:
         if isinstance(obj, tuple):
             return {
                 "_type": "tuple",
                 "data": [self.encode_obj(v) for v in obj],
@@ -194,14 +209,20 @@
                         raise ValueError("Invalid module name")
                 elif obj["_type"] == "dtype":
                     return pd.api.types.pandas_dtype(data)
                 elif obj["_type"] == "slice":
                     return slice(*data)
                 elif obj["_type"] == "range":
                     return range(data["start"], data["stop"], data["step"])
+                elif obj["_type"] == "pa.Table":
+                    binary_data = base64.b64decode(obj["data"])
+                    buffer = pa.py_buffer(binary_data)
+                    reader = ipc.open_stream(buffer)
+                    deserialized_table = reader.read_all()
+                    return deserialized_table
             return {self.decode(k): self.decode_obj(v) for k, v in obj.items()}
         elif isinstance(obj, list):
             return [self.decode_obj(v) for v in obj]
         return obj
 
     @classmethod
     def decode_bytes(cls, b: bytes, *args: Any, **kwargs: Any) -> Any:
```

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/async_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,23 @@
 
 async def async_iter(data_list: t.Collection[T]) -> t.AsyncIterator[T]:
     """Convert a collection into an AsyncIterator."""
     for data in data_list:
         yield data
 
 
+async def is_async_iterator_empty(
+    ait: t.AsyncIterator[T],
+) -> t.Tuple[bool, t.AsyncIterator[T]]:
+    items = []
+    async for item in ait:
+        items.append(item)
+    return len(items) == 0, async_iter(items)
+
+
 async def decoupled_async_iter(
     source: t.AsyncIterator[T], buffer_size: int = 100
 ) -> t.AsyncIterator[T]:
     """Create a consumer/producer pattern using an asyncio.Queue."""
     queue: asyncio.Queue = asyncio.Queue(maxsize=buffer_size)
 
     async def producer() -> None:
```

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/cache_utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/cache_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,19 @@
     compute_admin_data,
     create_admin_columns,
     merge_data_and_admin,
 )
 from sarus_data_spec.arrow.array import fit_array_to_schema_type_async_gen
 from sarus_data_spec.arrow.conversion import to_pyarrow_table
 from sarus_data_spec.arrow.schema import type_from_arrow_schema
-from sarus_data_spec.constants import MAX_MAX_MULT, MULTIPLICITY
+from sarus_data_spec.constants import (
+    MAX_MAX_MULT,
+    MULTIPLICITY,
+    SARUS_DEFAULT_OUTPUT,
+)
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusSignature,
     SarusSignatureValue,
 )
 from sarus_data_spec.dataspec_validator.typing import PUPKind
@@ -376,14 +380,40 @@
         transform = self.scalar.transform()
         ds_args, ds_kwargs = self.scalar.parents()
         return await async_compute_external_value(
             transform, *ds_args, **ds_kwargs
         )
 
 
+def has_sarus_default_output(external_transform: st.Transform) -> bool:
+    _, py_kwargs, _, _ = static_arguments(external_transform)
+    return SARUS_DEFAULT_OUTPUT in py_kwargs
+
+
+def sarus_default_output(external_transform: st.Transform) -> pa.Table:
+    _, py_kwargs, _, _ = static_arguments(external_transform)
+    if SARUS_DEFAULT_OUTPUT in py_kwargs:
+        default_output = py_kwargs[SARUS_DEFAULT_OUTPUT]
+        if isinstance(default_output, pa.Table):
+            return default_output
+        elif isinstance(default_output, pd.DataFrame):
+            default_table = pa.Table.from_pandas(
+                default_output, preserve_index=False
+            )
+            return default_table
+        else:
+            raise NotImplementedError(
+                f"Type {default_output} for the default output is not supported."
+            )
+    else:
+        raise ValueError(
+            f"No sarus default output for this transform: {external_transform.uuid()}"
+        )
+
+
 async def async_compute_external_value(
     transform: st.Transform,
     *ds_args: t.Union[st.DataSpec, st.Transform],
     **ds_kwargs: t.Union[st.DataSpec, st.Transform],
 ) -> t.Any:
     """Compute the value of an external transform applied on Dataspecs.
 
@@ -622,8 +652,17 @@
         table = merge_data_and_admin(data_table, output_admin_data)
 
     else:
         result = await implementation.compute(bound_signature)
         data_table = to_pyarrow_table(result)
         table = create_admin_columns(data_table)
 
-    return async_iter(table.to_batches(max_chunksize=batch_size))
+    if table.num_rows > 0:
+        ait = async_iter(table.to_batches(max_chunksize=batch_size))
+    # use default value if it exists
+    elif has_sarus_default_output(dataset.transform()):
+        default_table = sarus_default_output(dataset.transform())
+        ait = async_iter(default_table.to_batches(max_chunksize=batch_size))
+    else:
+        ait = async_iter([])
+
+    return ait
```

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/optbinning.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/optbinning.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/scipy.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/scipy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/explainer.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/explainer.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/maskers.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/maskers.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/plots.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/plots.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/shap/utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/error_estimation.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/error_estimation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/push_sql.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/push_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/to_small_data.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/to_small_data.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/bigdata.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/bigdata.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/ops/sql_utils/queries.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/ops/sql_utils/queries.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/marginals.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/path.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/predicate.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/scalar.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/schema.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/size.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/statistics.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/status.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/transform.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/type.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/typing.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/PKG-INFO` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.1
+Version: 4.0.2.dev0
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sarus_data_spec_public-4.0.1/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-4.0.2.dev0/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/setup.cfg` & `sarus_data_spec_public-4.0.2.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.1/setup.py` & `sarus_data_spec_public-4.0.2.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == "__main__":
-    setup(version="4.0.1")
+    setup(version="4.0.2.dev0")
```


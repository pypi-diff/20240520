# Comparing `tmp/bigflow-1.9.0.tar.gz` & `tmp/bigflow-1.9.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigflow-1.9.0.tar", last modified: Mon May 20 09:55:47 2024, max compression
+gzip compressed data, was "bigflow-1.9.0.dev1.tar", last modified: Thu May 16 15:23:28 2024, max compression
```

## Comparing `bigflow-1.9.0.tar` & `bigflow-1.9.0.dev1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.740845 bigflow-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-05-20 09:54:57.000000 bigflow-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 09:54:57.000000 bigflow-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-20 09:54:57.000000 bigflow-1.9.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-20 09:55:47.740845 bigflow-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-20 09:54:57.000000 bigflow-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.720845 bigflow-1.9.0/bigflow/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.720845 bigflow-1.9.0/bigflow/bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/bigquery/dataset_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/bigquery/dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/bigquery/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/bigquery/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/bigquery/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.720845 bigflow-1.9.0/bigflow/build/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.720845 bigflow-1.9.0/bigflow/build/dataflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/operate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/reflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/build/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    35173 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/dagbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/dataflow/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/dataflow/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/dataflow/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/dataflow/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/dataflow/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/konfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/infra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/templates/migrate-11/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/templates/new-project/
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/.gitignore.j2
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/deployment_config.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/templates/new-project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/templates/new-project/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/test/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/templates/new-project/test/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.724845 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.728845 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.728845 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/scaffold/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.728845 bigflow-1.9.0/bigflow/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/testing/isolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13832 2024-05-20 09:54:57.000000 bigflow-1.9.0/bigflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.736845 bigflow-1.9.0/bigflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-20 09:55:47.000000 bigflow-1.9.0/bigflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-20 09:55:47.000000 bigflow-1.9.0/bigflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:55:47.000000 bigflow-1.9.0/bigflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 09:55:47.000000 bigflow-1.9.0/bigflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 09:55:47.000000 bigflow-1.9.0/bigflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-20 09:54:57.000000 bigflow-1.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.728845 bigflow-1.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 09:54:57.000000 bigflow-1.9.0/scripts/bf
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 09:54:57.000000 bigflow-1.9.0/scripts/bigflow
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:55:47.740845 bigflow-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-20 09:54:57.000000 bigflow-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.732845 bigflow-1.9.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.732845 bigflow-1.9.0/test/buildd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/buildd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.732845 bigflow-1.9.0/test/buildd/dataflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/buildd/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/buildd/test_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/buildd/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/buildd/test_operate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/buildd/test_pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/buildd/test_reflect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/buildd/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.732845 bigflow-1.9.0/test/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.732845 bigflow-1.9.0/test/cli/cli_logs_duplicated_workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/cli_logs_duplicated_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/cli_logs_duplicated_workflows/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.732845 bigflow-1.9.0/test/cli/cli_logs_log_name_workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/cli_logs_log_name_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/cli_logs_log_name_workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.732845 bigflow-1.9.0/test/cli/cli_logs_regular_workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/cli_logs_regular_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/cli_logs_regular_workflows/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)    42553 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.732845 bigflow-1.9.0/test/cli/test_module/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/test_module/Unused1.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/test_module/Unused2.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/test_module/Unused3.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/cli/test_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.736845 bigflow-1.9.0/test/dagbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/dagbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/dagbuilder/test_dagbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14048 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23905 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_konfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.736845 bigflow-1.9.0/test/test_user_commons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_user_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_user_commons/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_user_commons/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:55:47.736845 bigflow-1.9.0/test/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/testing/nonpure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-20 09:54:57.000000 bigflow-1.9.0/test/testing/test_isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.384075 bigflow-1.9.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-16 15:23:28.384075 bigflow-1.9.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.360075 bigflow-1.9.0.dev1/bigflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.360075 bigflow-1.9.0.dev1/bigflow/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/dataset_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.360075 bigflow-1.9.0.dev1/bigflow/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.360075 bigflow-1.9.0.dev1/bigflow/build/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/operate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/reflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35173 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dagbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/konfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/migrate-11/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/.gitignore.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/deployment_config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/bigflow/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/testing/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13832 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/bigflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/scripts/bf
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/scripts/bigflow
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:23:28.384075 bigflow-1.9.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/buildd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/buildd/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_operate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_reflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/cli/cli_logs_duplicated_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_duplicated_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_duplicated_workflows/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/cli/cli_logs_log_name_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_log_name_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_log_name_workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/cli/cli_logs_regular_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_regular_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_regular_workflows/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42553 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/cli/test_module/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_module/Unused1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_module/Unused2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_module/Unused3.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/dagbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/dagbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/dagbuilder/test_dagbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14048 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23905 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_konfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/test_user_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_user_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_user_commons/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_user_commons/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/testing/nonpure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/testing/test_isolate.py
```

### Comparing `bigflow-1.9.0/LICENSE` & `bigflow-1.9.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/NOTICE` & `bigflow-1.9.0.dev1/NOTICE`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/PKG-INFO` & `bigflow-1.9.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigflow
-Version: 1.9.0
+Version: 1.9.0.dev1
 Summary: BigQuery client wrapper with clean API
 Home-page: https://github.com/allegro/bigflow
 Author: Pogranicze
 Author-email: pogranicze-team@allegro.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `bigflow-1.9.0/README.md` & `bigflow-1.9.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/__init__.py` & `bigflow-1.9.0.dev1/bigflow/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/bigquery/__init__.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/bigquery/dataset_configuration.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/dataset_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/bigquery/dataset_manager.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/bigquery/interactive.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/bigquery/interface.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/interface.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/bigquery/job.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/build/dev.py` & `bigflow-1.9.0.dev1/bigflow/build/dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/build/dist.py` & `bigflow-1.9.0.dev1/bigflow/build/dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/build/legacy.py` & `bigflow-1.9.0.dev1/bigflow/build/legacy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/build/operate.py` & `bigflow-1.9.0.dev1/bigflow/build/operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/build/pip.py` & `bigflow-1.9.0.dev1/bigflow/build/pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/build/reflect.py` & `bigflow-1.9.0.dev1/bigflow/build/reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/build/spec.py` & `bigflow-1.9.0.dev1/bigflow/build/spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/cli.py` & `bigflow-1.9.0.dev1/bigflow/cli.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/commons.py` & `bigflow-1.9.0.dev1/bigflow/commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/configuration.py` & `bigflow-1.9.0.dev1/bigflow/configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/dagbuilder.py` & `bigflow-1.9.0.dev1/bigflow/dagbuilder.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/dataflow/io.py` & `bigflow-1.9.0.dev1/bigflow/dataflow/io.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/dataflow/job.py` & `bigflow-1.9.0.dev1/bigflow/dataflow/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/dataflow/ml.py` & `bigflow-1.9.0.dev1/bigflow/dataflow/ml.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/dataflow/options.py` & `bigflow-1.9.0.dev1/bigflow/dataflow/options.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/deploy.py` & `bigflow-1.9.0.dev1/bigflow/deploy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/konfig.py` & `bigflow-1.9.0.dev1/bigflow/konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/migrate.py` & `bigflow-1.9.0.dev1/bigflow/migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/resources.py` & `bigflow-1.9.0.dev1/bigflow/resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/infra.py` & `bigflow-1.9.0.dev1/bigflow/scaffold/infra.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/scaffold.py` & `bigflow-1.9.0.dev1/bigflow/scaffold/scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/README.txt` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/README.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/.gitignore.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/Dockerfile` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/README.md` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/README.md`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/deployment_config.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/deployment_config.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/scaffold/templating.py` & `bigflow-1.9.0.dev1/bigflow/scaffold/templating.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/testing/isolate.py` & `bigflow-1.9.0.dev1/bigflow/testing/isolate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/version.py` & `bigflow-1.9.0.dev1/bigflow/version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow/workflow.py` & `bigflow-1.9.0.dev1/bigflow/workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow.egg-info/PKG-INFO` & `bigflow-1.9.0.dev1/bigflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigflow
-Version: 1.9.0
+Version: 1.9.0.dev1
 Summary: BigQuery client wrapper with clean API
 Home-page: https://github.com/allegro/bigflow
 Author: Pogranicze
 Author-email: pogranicze-team@allegro.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `bigflow-1.9.0/bigflow.egg-info/SOURCES.txt` & `bigflow-1.9.0.dev1/bigflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/bigflow.egg-info/requires.txt` & `bigflow-1.9.0.dev1/bigflow.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/setup.py` & `bigflow-1.9.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/buildd/test_dev.py` & `bigflow-1.9.0.dev1/test/buildd/test_dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/buildd/test_dist.py` & `bigflow-1.9.0.dev1/test/buildd/test_dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/buildd/test_operate.py` & `bigflow-1.9.0.dev1/test/buildd/test_operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/buildd/test_pip.py` & `bigflow-1.9.0.dev1/test/buildd/test_pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/buildd/test_reflect.py` & `bigflow-1.9.0.dev1/test/buildd/test_reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/buildd/test_spec.py` & `bigflow-1.9.0.dev1/test/buildd/test_spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/cli/test_cli.py` & `bigflow-1.9.0.dev1/test/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/cli/test_module/Unused1.py` & `bigflow-1.9.0.dev1/test/cli/test_module/Unused1.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/dagbuilder/test_dagbuilder.py` & `bigflow-1.9.0.dev1/test/dagbuilder/test_dagbuilder.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_commons.py` & `bigflow-1.9.0.dev1/test/test_commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_configuration.py` & `bigflow-1.9.0.dev1/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_dataflow.py` & `bigflow-1.9.0.dev1/test/test_dataflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_deploy.py` & `bigflow-1.9.0.dev1/test/test_deploy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_interactive.py` & `bigflow-1.9.0.dev1/test/test_interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_job.py` & `bigflow-1.9.0.dev1/test/test_job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_konfig.py` & `bigflow-1.9.0.dev1/test/test_konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_migrate.py` & `bigflow-1.9.0.dev1/test/test_migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_resources.py` & `bigflow-1.9.0.dev1/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_scaffold.py` & `bigflow-1.9.0.dev1/test/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_user_commons/test_labels.py` & `bigflow-1.9.0.dev1/test/test_user_commons/test_labels.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_user_commons/test_sensor.py` & `bigflow-1.9.0.dev1/test/test_user_commons/test_sensor.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_version.py` & `bigflow-1.9.0.dev1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/test_workflow.py` & `bigflow-1.9.0.dev1/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.9.0/test/testing/test_isolate.py` & `bigflow-1.9.0.dev1/test/testing/test_isolate.py`

 * *Files identical despite different names*


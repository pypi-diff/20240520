# Comparing `tmp/dcicutils-8.8.4.1b9.tar.gz` & `tmp/dcicutils-8.9.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.4.1b9.tar", max compression
+gzip compressed data, was "dcicutils-8.9.0.0b0.tar", max compression
```

## Comparing `dcicutils-8.8.4.1b9.tar` & `dcicutils-8.9.0.0b0.tar`

### file list

```diff
@@ -1,79 +1,78 @@
--rw-r--r--   0        0        0     1102 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/README.rst
--rw-r--r--   0        0        0        0 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     3295 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7626 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/data_utils.py
--rw-r--r--   0        0        0    13499 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    73123 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     4896 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0      807 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/http_utils.py
--rw-r--r--   0        0        0    11502 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-25 13:01:40.086676 dcicutils-8.8.4.1b9/dcicutils/log_utils.py
--rw-r--r--   0        0        0   105530 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30779 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    19468 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    61238 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/task_utils.py
--rw-r--r--   0        0        0     2340 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     3265 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4733 2024-04-25 13:01:40.090676 dcicutils-8.8.4.1b9/pyproject.toml
--rw-r--r--   0        0        0     3396 1970-01-01 00:00:00.000000 dcicutils-8.8.4.1b9/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/README.rst
+-rw-r--r--   0        0        0        0 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3295 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7626 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    13499 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-05-13 15:45:55.570363 dcicutils-8.9.0.0b0/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   104610 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30779 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    19468 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10605 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-05-13 15:45:55.574363 dcicutils-8.9.0.0b0/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    61238 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4689 2024-05-13 15:45:55.578363 dcicutils-8.9.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.9.0.0b0/PKG-INFO
```

### Comparing `dcicutils-8.8.4.1b9/LICENSE.txt` & `dcicutils-8.9.0.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/README.rst` & `dcicutils-8.9.0.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/base.py` & `dcicutils-8.9.0.0b0/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/beanstalk_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/bundle_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/captured_output.py` & `dcicutils-8.9.0.0b0/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/cloudformation_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/codebuild_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/command_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/common.py` & `dcicutils-8.9.0.0b0/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/contribution_scripts.py` & `dcicutils-8.9.0.0b0/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/contribution_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/creds_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/data_readers.py` & `dcicutils-8.9.0.0b0/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/data_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/datetime_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/deployment_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/diff_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/docker_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/ecr_scripts.py` & `dcicutils-8.9.0.0b0/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/ecr_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/ecs_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/env_base.py` & `dcicutils-8.9.0.0b0/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/env_manager.py` & `dcicutils-8.9.0.0b0/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/env_scripts.py` & `dcicutils-8.9.0.0b0/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/env_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/env_utils_legacy.py` & `dcicutils-8.9.0.0b0/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/es_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/exceptions.py` & `dcicutils-8.9.0.0b0/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/ff_mocks.py` & `dcicutils-8.9.0.0b0/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/ff_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/ff_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -891,20 +891,17 @@
 
 def _get_es_metadata(uuids, es_client, filters, sources, chunk_size, auth):
     """
     Internal function needed because there are multiple levels of iteration
     used to create the generator.
     Should NOT be used directly
     """
-    def get_es_host_local() -> Optional[str]:
-        return os.environ.get("ES_HOST_LOCAL", None)
     health = get_health_page(key=auth)
     if es_client is None:
-        if not (es_url := get_es_host_local()):
-            es_url = health['elasticsearch']
+        es_url = health['elasticsearch']
         es_client = es_utils.create_es_client(es_url, use_aws_auth=True)
     namespace_star = health.get('namespace', '') + '*'
     # match all given uuids to _id fields
     # sending in too many uuids in the terms query can crash es; break them up
     # into groups of max size 100
     for i in range(0, len(uuids), chunk_size):
         query_uuids = uuids[i:i + chunk_size]
```

### Comparing `dcicutils-8.8.4.1b9/dcicutils/function_cache_decorator.py` & `dcicutils-8.9.0.0b0/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/glacier_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/jh_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/kibana/dashboards.json` & `dcicutils-8.9.0.0b0/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/kibana/readme.md` & `dcicutils-8.9.0.0b0/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/lang_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.9.0.0b0/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/license_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/log_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/misc_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/misc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 This file contains functions that might be generally useful.
 """
 
 from collections import namedtuple
-import appdirs
 import contextlib
 import datetime
 import functools
 import hashlib
 import inspect
 import io
 import json
 import logging
 import math
 import os
-import platform
 import pytz
 import re
 import rfc3986.validators
 import rfc3986.exceptions
 import time
 import uuid
 import warnings
@@ -1520,15 +1518,15 @@
         i -= 1
     return list_or_tuple[:i + 1]
 
 
 def create_dict(**kwargs) -> dict:
     result = {}
     for name in kwargs:
-        if not (kwargs[name] is None):
+        if kwargs[name]:
             result[name] = kwargs[name]
     return result
 
 
 def create_readonly_object(**kwargs):
     """
     Returns a new/unique object instance with readonly properties equal to the give kwargs.
@@ -2668,33 +2666,7 @@
                 if self.padded and len(line) < n_headers:
                     line = pad_to(n_headers, line, padding=self.padding)
                 yield dict(zip(self.headers, line))
             elif isinstance(line, dict):
                 yield line
             else:
                 raise Exception(f"If the first line is not a list, all lines must be dictionaries: {line!r}")
-
-
-def get_app_specific_directory() -> str:
-    """
-    Returns the standard system application specific directory:
-    - On MacOS this directory: is: ~/Library/Application Support
-    - On Linux this directory is: ~/.local/share
-    - On Windows this directory is: %USERPROFILE%\AppData\Local  # noqa
-    N.B. This is has been tested on MacOS and Linux but not on Windows.
-    """
-    return appdirs.user_data_dir()
-
-
-def get_os_name() -> str:
-    if os_name := platform.system():
-        if os_name == "Darwin": return "osx"  # noqa
-        elif os_name == "Linux": return "linux"  # noqa
-        elif os_name == "Windows": return "windows"  # noqa
-    return ""
-
-
-def get_cpu_architecture_name() -> str:
-    if os_architecture_name := platform.machine():
-        if os_architecture_name == "x86_64": return "amd64"  # noqa
-        return os_architecture_name
-    return ""
```

### Comparing `dcicutils-8.8.4.1b9/dcicutils/obfuscation_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/opensearch_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/portal_object_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/portal_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/progress_bar.py` & `dcicutils-8.9.0.0b0/dcicutils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/project_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/qa_checkers.py` & `dcicutils-8.9.0.0b0/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/qa_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/redis_tools.py` & `dcicutils-8.9.0.0b0/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/redis_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/s3_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/schema_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/schema_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     REF = "$ref"
     REQUIRED = "required"
     STRING = "string"
     TYPE = "type"
 
 
 class EncodedSchemaConstants:
+    DESCRIPTION = "description"
     IDENTIFYING_PROPERTIES = "identifyingProperties"
     LINK_TO = "linkTo"
     MERGE_REF = "$merge"
     MIXIN_PROPERTIES = "mixinProperties"
     UNIQUE_KEY = "uniqueKey"
 
 
@@ -183,14 +184,29 @@
     return [
         get_format(one_of_schema)
         for one_of_schema in get_one_of(schema)
         if get_format(one_of_schema)
     ]
 
 
+def is_link(property_schema: Dict[str, Any]) -> bool:
+    """Is property schema a link?"""
+    return property_schema.get(SchemaConstants.LINK_TO, False)
+
+
+def get_enum(property_schema: Dict[str, Any]) -> List[str]:
+    """Return the enum of a property schema."""
+    return property_schema.get(SchemaConstants.ENUM, [])
+
+
+def get_description(schema: Dict[str, Any]) -> str:
+    """Return the description of a schema."""
+    return schema.get(SchemaConstants.DESCRIPTION, "")
+
+
 class Schema:
 
     def __init__(self, schema: dict, type: Optional[str] = None) -> None:
         self._data = schema if isinstance(schema, dict) else (schema.data if isinstance(schema, Schema) else {})
         self._type = ((type if isinstance(type, str) else "") or
                       Schema.type_name(self._data.get("title", "")) or
                       Schema.type_name(self._data.get("$id", "")))
```

### Comparing `dcicutils-8.8.4.1b9/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.9.0.0b0/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.9.0.0b0/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.9.0.0b0/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/secrets_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/sheet_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/snapshot_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/structured_data.py` & `dcicutils-8.9.0.0b0/dcicutils/structured_data.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/submitr/progress_constants.py` & `dcicutils-8.9.0.0b0/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.9.0.0b0/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/task_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/tmpfile_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/zip_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,47 @@
 from contextlib import contextmanager
+from dcicutils.tmpfile_utils import temporary_directory, temporary_file
+import gzip
 import os
-import shutil
-import tempfile
-from typing import List, Optional, Union
+import tarfile
+from typing import List, Optional
+import zipfile
 
 
 @contextmanager
-def temporary_directory() -> str:
-    try:
-        with tempfile.TemporaryDirectory() as tmp_directory_name:
-            yield tmp_directory_name
-    finally:
-        remove_temporary_directory(tmp_directory_name)
+def unpack_zip_file_to_temporary_directory(file: str) -> str:
+    with temporary_directory() as tmp_directory_name:
+        with zipfile.ZipFile(file, "r") as zipf:
+            zipf.extractall(tmp_directory_name)
+        yield tmp_directory_name
 
 
 @contextmanager
-def temporary_file(name: Optional[str] = None, suffix: Optional[str] = None,
-                   content: Optional[Union[str, bytes, List[str]]] = None) -> str:
+def unpack_tar_file_to_temporary_directory(file: str) -> str:
     with temporary_directory() as tmp_directory_name:
-        tmp_file_name = os.path.join(tmp_directory_name, name or tempfile.mktemp(dir="")) + (suffix or "")
-        with open(tmp_file_name, "wb" if isinstance(content, bytes) else "w") as tmp_file:
-            if content is not None:
-                tmp_file.write("\n".join(content) if isinstance(content, list) else content)
-        yield tmp_file_name
-
-
-def remove_temporary_directory(tmp_directory_name: str) -> None:
-    """
-    Removes the given directory, recursively; but ONLY if it is (somewhere) within the system temporary directory.
-    """
-    def is_temporary_directory(path: str) -> bool:
-        try:
-            tmpdir = tempfile.gettempdir()
-            return os.path.commonpath([path, tmpdir]) == tmpdir and os.path.exists(path) and os.path.isdir(path)
-        except Exception:
-            return False
-    if is_temporary_directory(tmp_directory_name):  # Guard against errant deletion.
-        shutil.rmtree(tmp_directory_name)
-
-
-def create_temporary_file_name(prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
-    """
-    Generates and returns the full path to file within the system temporary directory.
-    """
-    with tempfile.NamedTemporaryFile(prefix=prefix, suffix=suffix, delete=False) as tmp_file:
-        tmp_file_name = tmp_file.name
-    return tmp_file_name
-
-
-def remove_temporary_file(tmp_file_name: str) -> bool:
-    """
-    Removes the given file; but ONLY if it is (somewhere) within the system temporary directory.
-    """
-    try:
-        tmpdir = tempfile.gettempdir()
-        if (os.path.commonpath([tmpdir, tmp_file_name]) == tmpdir) and os.path.isfile(tmp_file_name):
-            os.remove(tmp_file_name)
-            return True
-        return False
-    except Exception:
-        return False
+        with tarfile.open(file, "r") as tarf:
+            tarf.extractall(tmp_directory_name)
+        yield tmp_directory_name
+
+
+def unpack_files(file: str, suffixes: Optional[List[str]] = None) -> Optional[str]:
+    unpack_file_to_tmp_directory = {
+        ".tar": unpack_tar_file_to_temporary_directory,
+        ".zip": unpack_zip_file_to_temporary_directory
+    }.get(file[dot:]) if (dot := file.rfind(".")) > 0 else None
+    if unpack_file_to_tmp_directory is not None:
+        with unpack_file_to_tmp_directory(file) as tmp_directory_name:
+            for directory, _, files in os.walk(tmp_directory_name):  # Ignore "." prefixed files.
+                for file in [file for file in files if not file.startswith(".")]:
+                    if not suffixes or any(file.endswith(suffix) for suffix in suffixes):
+                        yield os.path.join(directory, file)
+
+
+@contextmanager
+def unpack_gz_file_to_temporary_file(file: str, suffix: Optional[str] = None) -> str:
+    if (gz := file.endswith(".gz")) or file.endswith(".tgz"):  # The .tgz suffix is simply short for .tar.gz.
+        with temporary_file(name=os.path.basename(file[:-3] if gz else file[:-4] + ".tar")) as tmp_file_name:
+            with open(tmp_file_name, "wb") as outputf:
+                with gzip.open(file, "rb") as inputf:
+                    outputf.write(inputf.read())
+                    outputf.close()
+                    yield tmp_file_name
```

### Comparing `dcicutils-8.8.4.1b9/dcicutils/trace_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/validation_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/dcicutils/variant_utils.py` & `dcicutils-8.9.0.0b0/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b9/pyproject.toml` & `dcicutils-8.9.0.0b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.4.1b9"  # TODO: To become 8.8.5
+version = "8.9.0.0b0"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
@@ -33,21 +33,20 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.13"
-boto3 = "^1.34.90"
-botocore = "^1.34.90"
+python = ">=3.8,<3.12"
+boto3 = "^1.28.57"
+botocore = "^1.31.57"
 # The DCIC portals (cgap-portal and fourfront) are very particular about which ElasticSearch version.
 # This value is intentionally pinned and must not be changed casually.
 elasticsearch = "7.13.4"
-appdirs = "^1.4.4"
 aws-requests-auth = ">=0.4.2,<1"
 chardet = "^5.2.0"
 docker = "^4.4.4"
 gitpython = "^3.1.2"
 jsonc-parser = "^1.1.5"
 jsonschema = "^4.19.0"
 openpyxl = "^3.1.2"
@@ -66,16 +65,16 @@
 tqdm = "^4.66.2"
 typing-extensions = ">=3.8"  # Fourfront uses 3.8
 urllib3 = "^1.26.6"
 webtest = "^2.0.34"
 
 
 [tool.poetry.dev-dependencies]
-boto3-stubs = "^1.34.90"
-botocore-stubs = "^1.34.90"
+boto3-stubs = "^1.28.57"
+botocore-stubs = "^1.31.57"
 coverage = ">=7.2.3"
 # Loaded manually in GA workflow for coverage because a dependency on 2to3
 # in its docopts dependency makes a problem for laoding it here in poetry. -kmp 7-Apr-2023
 # coveralls = ">=3.3.1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
 pip-licenses = "^4.3.3"
```

### Comparing `dcicutils-8.8.4.1b9/PKG-INFO` & `dcicutils-8.9.0.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.4.1b9
+Version: 8.9.0.0b0
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
-Requires-Python: >=3.8,<3.13
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,18 +20,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
-Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: aws-requests-auth (>=0.4.2,<1)
-Requires-Dist: boto3 (>=1.34.90,<2.0.0)
-Requires-Dist: botocore (>=1.34.90,<2.0.0)
+Requires-Dist: boto3 (>=1.28.57,<2.0.0)
+Requires-Dist: botocore (>=1.31.57,<2.0.0)
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: docker (>=4.4.4,<5.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: jsonc-parser (>=1.1.5,<2.0.0)
 Requires-Dist: jsonschema (>=4.19.0,<5.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
```


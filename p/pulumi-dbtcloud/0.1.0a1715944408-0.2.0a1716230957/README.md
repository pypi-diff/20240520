# Comparing `tmp/pulumi_dbtcloud-0.1.0a1715944408.tar.gz` & `tmp/pulumi_dbtcloud-0.2.0a1716230957.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_dbtcloud-0.1.0a1715944408.tar", last modified: Fri May 17 11:15:58 2024, max compression
+gzip compressed data, was "pulumi_dbtcloud-0.2.0a1716230957.tar", last modified: Mon May 20 18:51:56 2024, max compression
```

## Comparing `pulumi_dbtcloud-0.1.0a1715944408.tar` & `pulumi_dbtcloud-0.2.0a1716230957.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:15:58.001407 pulumi_dbtcloud-0.1.0a1715944408/
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-17 11:15:58.001407 pulumi_dbtcloud-0.1.0a1715944408/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:15:58.001407 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    58952 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/big_query_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:15:58.001407 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    44015 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/environment_variable_job_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/fabric_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/fabric_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_azure_dev_ops_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_azure_dev_ops_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_big_query_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    15719 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    68381 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/license_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    29421 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22244 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/project_artefacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/project_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/project_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38478 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:15:58.001407 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-17 11:15:57.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-17 11:15:57.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:15:57.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 11:15:57.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 11:15:57.000000 pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-17 11:15:51.000000 pulumi_dbtcloud-0.1.0a1715944408/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:15:58.001407 pulumi_dbtcloud-0.1.0a1715944408/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:56.346298 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58952 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/big_query_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44015 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment_variable_job_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/fabric_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/fabric_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_azure_dev_ops_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_azure_dev_ops_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_big_query_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15719 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68381 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/license_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29421 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22244 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_artefacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38478 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/setup.cfg
```

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/PKG-INFO` & `pulumi_dbtcloud-0.2.0a1716230957/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dbtcloud
-Version: 0.1.0a1715944408
+Version: 0.2.0a1716230957
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-dbtcloud
 Keywords: pulumi,dbtcloud,dbt,cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -21,24 +21,14 @@
 This package is available for several languages/platforms:
 
 - JavaScript/TypeScript: [`@pulumi/dbtcloud`](https://www.npmjs.com/package/@pulumi/dbtcloud)
 - Python: [`pulumi-dbtcloud`](https://pypi.org/project/pulumi-dbtcloud/)
 - Go: [`github.com/pulumi/pulumi-dbtcloud/sdk/go/dbtcloud`](https://pkg.go.dev/github.com/pulumi/pulumi-dbtcloud/sdk/go/dbtcloud)
 - .NET: [`Pulumi.Dbtcloud`](https://www.nuget.org/packages/Pulumi.DbtCloud)
 
-## Provider Binary
-
-The dbt Cloud provider binary is a third party binary. It can be installed using the pulumi plugin command.
-
-```bash
-pulumi plugin install resource dbtcloud <version> --server github://api.github.com/pulumi/pulumi-dbtcloud
-```
-
-Replace `<version>` with your desired version.
-
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
 npm install @pulumi/dbtcloud
 ```
```

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/README.md` & `pulumi_dbtcloud-0.2.0a1716230957/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,14 @@
 This package is available for several languages/platforms:
 
 - JavaScript/TypeScript: [`@pulumi/dbtcloud`](https://www.npmjs.com/package/@pulumi/dbtcloud)
 - Python: [`pulumi-dbtcloud`](https://pypi.org/project/pulumi-dbtcloud/)
 - Go: [`github.com/pulumi/pulumi-dbtcloud/sdk/go/dbtcloud`](https://pkg.go.dev/github.com/pulumi/pulumi-dbtcloud/sdk/go/dbtcloud)
 - .NET: [`Pulumi.Dbtcloud`](https://www.nuget.org/packages/Pulumi.DbtCloud)
 
-## Provider Binary
-
-The dbt Cloud provider binary is a third party binary. It can be installed using the pulumi plugin command.
-
-```bash
-pulumi plugin install resource dbtcloud <version> --server github://api.github.com/pulumi/pulumi-dbtcloud
-```
-
-Replace `<version>` with your desired version.
-
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
 npm install @pulumi/dbtcloud
 ```
```

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/__init__.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/_inputs.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/_utilities.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/big_query_connection.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/big_query_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/big_query_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/big_query_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/config/__init__.pyi` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/config/vars.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/connection.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/databricks_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/databricks_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/environment.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/environment_variable.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/environment_variable_job_override.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment_variable_job_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/extended_attributes.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/extended_attributes.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/fabric_connection.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/fabric_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/fabric_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/fabric_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_azure_dev_ops_project.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_azure_dev_ops_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_azure_dev_ops_repository.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_azure_dev_ops_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_big_query_connection.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_big_query_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_big_query_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_big_query_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_connection.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_databricks_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_databricks_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_environment.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_environment_variable.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_extended_attributes.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_extended_attributes.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_group.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_group_users.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_group_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_job.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_notification.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_postgres_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_postgres_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_privatelink_endpoint.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_project.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_repository.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_service_token.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_service_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_snowflake_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_user.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_user_groups.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/get_webhook.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/group.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/job.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/license_map.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/license_map.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/notification.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/outputs.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/postgres_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/postgres_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/project.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/project_artefacts.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_artefacts.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/project_connection.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/project_repository.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/provider.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/repository.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/service_token.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/snowflake_credential.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/user_groups.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud/webhook.py` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud.egg-info/PKG-INFO` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dbtcloud
-Version: 0.1.0a1715944408
+Version: 0.2.0a1716230957
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-dbtcloud
 Keywords: pulumi,dbtcloud,dbt,cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -21,24 +21,14 @@
 This package is available for several languages/platforms:
 
 - JavaScript/TypeScript: [`@pulumi/dbtcloud`](https://www.npmjs.com/package/@pulumi/dbtcloud)
 - Python: [`pulumi-dbtcloud`](https://pypi.org/project/pulumi-dbtcloud/)
 - Go: [`github.com/pulumi/pulumi-dbtcloud/sdk/go/dbtcloud`](https://pkg.go.dev/github.com/pulumi/pulumi-dbtcloud/sdk/go/dbtcloud)
 - .NET: [`Pulumi.Dbtcloud`](https://www.nuget.org/packages/Pulumi.DbtCloud)
 
-## Provider Binary
-
-The dbt Cloud provider binary is a third party binary. It can be installed using the pulumi plugin command.
-
-```bash
-pulumi plugin install resource dbtcloud <version> --server github://api.github.com/pulumi/pulumi-dbtcloud
-```
-
-Replace `<version>` with your desired version.
-
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
 npm install @pulumi/dbtcloud
 ```
```

### Comparing `pulumi_dbtcloud-0.1.0a1715944408/pulumi_dbtcloud.egg-info/SOURCES.txt` & `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/dataherald-0.8.0.tar.gz` & `tmp/dataherald-0.9.0.tar.gz`

## Comparing `dataherald-0.8.0.tar` & `dataherald-0.9.0.tar`

### file list

```diff
@@ -1,103 +1,102 @@
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/__init__.py
--rw-r--r--   0        0        0    57866 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_base_client.py
--rw-r--r--   0        0        0    20719 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_client.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_compat.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_constants.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_exceptions.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_files.py
--rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_qs.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_resource.py
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_response.py
--rw-r--r--   0        0        0     7116 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_streaming.py
--rw-r--r--   0        0        0    10125 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_types.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/py.typed
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_utils/__init__.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_utils/_logs.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_utils/_streams.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_utils/_transform.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_utils/_typing.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/_utils/_utils.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/__init__.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/engine.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/finetunings.py
--rw-r--r--   0        0        0    18783 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/generations.py
--rw-r--r--   0        0        0    12577 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/golden_sqls.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/heartbeat.py
--rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/nl_generations.py
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/table_descriptions.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/database_connections/__init__.py
--rw-r--r--   0        0        0    14970 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/database_connections/database_connections.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/database_connections/drivers.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/instructions/__init__.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/instructions/first.py
--rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/instructions/instructions.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/prompts/prompts.py
--rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/prompts/sql_generations.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/sql_generations/__init__.py
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/sql_generations/nl_generations.py
--rw-r--r--   0        0        0    14638 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/resources/sql_generations/sql_generations.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/__init__.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/database_connection_create_params.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/database_connection_list_response.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/database_connection_update_params.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/db_connection_response.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/finetuning_create_params.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/finetuning_list_params.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/finetuning_list_response.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/finetuning_response.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/generation_list_item.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/generation_list_params.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/generation_list_response.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/generation_response.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/generation_sql_generation_params.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/generation_update_params.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/golden_sql_list_params.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/golden_sql_list_response.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/golden_sql_upload_params.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/golden_sql_upload_response.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/instruction_create_params.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/instruction_list_params.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/instruction_list_response.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/instruction_update_params.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/nl_generation_create_params.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/nl_generation_list_params.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/nl_generation_list_response.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/prompt_create_params.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/prompt_list_params.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/prompt_list_response.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/prompt_response.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/sql_generation_create_params.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/sql_generation_execute_params.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/sql_generation_execute_response.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/sql_generation_list_params.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/sql_generation_list_response.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/table_description_list_params.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/table_description_list_response.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/table_description_response.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/table_description_sync_schemas_params.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/table_description_update_params.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/database_connections/__init__.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/database_connections/driver_list_response.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/database_connections/driver_response.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/instructions/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/prompts/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/prompts/sql_generation_create_params.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/prompts/sql_generation_nl_generations_params.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/prompts/sql_generation_retrieve_params.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/shared/__init__.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/shared/golden_sql_response.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/shared/instruction_response.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/shared/nl_generation_response.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/shared/sql_generation_response.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/sql_generations/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/sql_generations/nl_generation_create_params.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dataherald-0.8.0/src/dataherald/types/sql_generations/nl_generation_retrieve_params.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 dataherald-0.8.0/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 dataherald-0.8.0/LICENSE
--rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 dataherald-0.8.0/README.md
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 dataherald-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 dataherald-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/__init__.py
+-rw-r--r--   0        0        0    57711 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_base_client.py
+-rw-r--r--   0        0        0    20719 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_client.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_compat.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_constants.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_exceptions.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_files.py
+-rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_qs.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_resource.py
+-rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_response.py
+-rw-r--r--   0        0        0     7116 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_streaming.py
+-rw-r--r--   0        0        0    10081 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_types.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/py.typed
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_utils/__init__.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_utils/_logs.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_utils/_streams.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_utils/_transform.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_utils/_typing.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/lib/.keep
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/__init__.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/engine.py
+-rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/finetunings.py
+-rw-r--r--   0        0        0    18758 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/generations.py
+-rw-r--r--   0        0        0    12513 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/golden_sqls.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/heartbeat.py
+-rw-r--r--   0        0        0    10784 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/nl_generations.py
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/table_descriptions.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/database_connections/__init__.py
+-rw-r--r--   0        0        0    14945 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/database_connections/database_connections.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/database_connections/drivers.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/instructions/__init__.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/instructions/first.py
+-rw-r--r--   0        0        0    13735 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/instructions/instructions.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/prompts/prompts.py
+-rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/prompts/sql_generations.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/sql_generations/__init__.py
+-rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/sql_generations/nl_generations.py
+-rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/resources/sql_generations/sql_generations.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/__init__.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/database_connection_create_params.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/database_connection_list_response.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/database_connection_update_params.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/db_connection_response.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/finetuning_create_params.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/finetuning_list_params.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/finetuning_list_response.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/finetuning_response.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/generation_list_item.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/generation_list_params.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/generation_list_response.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/generation_response.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/generation_sql_generation_params.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/generation_update_params.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/golden_sql_list_params.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/golden_sql_list_response.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/golden_sql_upload_params.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/golden_sql_upload_response.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/instruction_create_params.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/instruction_list_params.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/instruction_list_response.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/instruction_update_params.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/nl_generation_create_params.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/nl_generation_list_params.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/nl_generation_list_response.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/prompt_create_params.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/prompt_list_params.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/prompt_list_response.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/prompt_response.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/sql_generation_create_params.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/sql_generation_list_params.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/sql_generation_list_response.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/table_description_list_params.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/table_description_list_response.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/table_description_response.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/table_description_sync_schemas_params.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/table_description_update_params.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/database_connections/__init__.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/database_connections/driver_list_response.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/database_connections/driver_response.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/instructions/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/prompts/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/prompts/sql_generation_create_params.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/prompts/sql_generation_nl_generations_params.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/prompts/sql_generation_retrieve_params.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/shared/__init__.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/shared/golden_sql_response.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/shared/instruction_response.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/shared/nl_generation_response.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/shared/sql_generation_response.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/sql_generations/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/sql_generations/nl_generation_create_params.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dataherald-0.9.0/src/dataherald/types/sql_generations/nl_generation_retrieve_params.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 dataherald-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 dataherald-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 dataherald-0.9.0/README.md
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 dataherald-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 dataherald-0.9.0/PKG-INFO
```

### Comparing `dataherald-0.8.0/src/dataherald/__init__.py` & `dataherald-0.9.0/src/dataherald/__init__.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_base_client.py` & `dataherald-0.9.0/src/dataherald/_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,26 @@
 from ._qs import Querystring
 from ._files import to_httpx_files, async_to_httpx_files
 from ._types import (
     NOT_GIVEN,
     Body,
     Omit,
     Query,
-    ModelT,
     Headers,
     Timeout,
     NotGiven,
     ResponseT,
     Transport,
     AnyMapping,
     PostParser,
     ProxiesTypes,
     RequestFiles,
     HttpxSendArgs,
     AsyncTransport,
     RequestOptions,
-    UnknownResponse,
     ModelBuilderProtocol,
     BinaryResponseContent,
 )
 from ._utils import is_dict, is_given, is_mapping
 from ._compat import model_copy, model_dump
 from ._models import GenericModel, FinalRequestOptions, validate_type, construct_type
 from ._response import APIResponse
@@ -138,39 +136,39 @@
         url: URL | NotGiven = NOT_GIVEN,
         params: Query | NotGiven = NOT_GIVEN,
     ) -> None:
         self.url = url
         self.params = params
 
 
-class BasePage(GenericModel, Generic[ModelT]):
+class BasePage(GenericModel, Generic[_T]):
     """
     Defines the core interface for pagination.
 
     Type Args:
         ModelT: The pydantic model that represents an item in the response.
 
     Methods:
         has_next_page(): Check if there is another page available
         next_page_info(): Get the necessary information to make a request for the next page
     """
 
     _options: FinalRequestOptions = PrivateAttr()
-    _model: Type[ModelT] = PrivateAttr()
+    _model: Type[_T] = PrivateAttr()
 
     def has_next_page(self) -> bool:
         items = self._get_page_items()
         if not items:
             return False
         return self.next_page_info() is not None
 
     def next_page_info(self) -> Optional[PageInfo]:
         ...
 
-    def _get_page_items(self) -> Iterable[ModelT]:  # type: ignore[empty-body]
+    def _get_page_items(self) -> Iterable[_T]:  # type: ignore[empty-body]
         ...
 
     def _params_from_url(self, url: URL) -> httpx.QueryParams:
         # TODO: do we have to preprocess params here?
         return httpx.QueryParams(cast(Any, self._options.params)).merge(url.params)
 
     def _info_to_options(self, info: PageInfo) -> FinalRequestOptions:
@@ -187,36 +185,36 @@
             options.params = dict(url.params)
             options.url = str(url)
             return options
 
         raise ValueError("Unexpected PageInfo state")
 
 
-class BaseSyncPage(BasePage[ModelT], Generic[ModelT]):
+class BaseSyncPage(BasePage[_T], Generic[_T]):
     _client: SyncAPIClient = pydantic.PrivateAttr()
 
     def _set_private_attributes(
         self,
         client: SyncAPIClient,
-        model: Type[ModelT],
+        model: Type[_T],
         options: FinalRequestOptions,
     ) -> None:
         self._model = model
         self._client = client
         self._options = options
 
     # Pydantic uses a custom `__iter__` method to support casting BaseModels
     # to dictionaries. e.g. dict(model).
     # As we want to support `for item in page`, this is inherently incompatible
     # with the default pydantic behaviour. It is not possible to support both
     # use cases at once. Fortunately, this is not a big deal as all other pydantic
     # methods should continue to work as expected as there is an alternative method
     # to cast a model to a dictionary, model.dict(), which is used internally
     # by pydantic.
-    def __iter__(self) -> Iterator[ModelT]:  # type: ignore
+    def __iter__(self) -> Iterator[_T]:  # type: ignore
         for page in self.iter_pages():
             for item in page._get_page_items():
                 yield item
 
     def iter_pages(self: SyncPageT) -> Iterator[SyncPageT]:
         page = self
         while True:
@@ -233,21 +231,21 @@
                 "No next page expected; please check `.has_next_page()` before calling `.get_next_page()`."
             )
 
         options = self._info_to_options(info)
         return self._client._request_api_list(self._model, page=self.__class__, options=options)
 
 
-class AsyncPaginator(Generic[ModelT, AsyncPageT]):
+class AsyncPaginator(Generic[_T, AsyncPageT]):
     def __init__(
         self,
         client: AsyncAPIClient,
         options: FinalRequestOptions,
         page_cls: Type[AsyncPageT],
-        model: Type[ModelT],
+        model: Type[_T],
     ) -> None:
         self._model = model
         self._client = client
         self._options = options
         self._page_cls = page_cls
 
     def __await__(self) -> Generator[Any, None, AsyncPageT]:
@@ -262,38 +260,38 @@
             )
             return resp
 
         self._options.post_parser = _parser
 
         return await self._client.request(self._page_cls, self._options)
 
-    async def __aiter__(self) -> AsyncIterator[ModelT]:
+    async def __aiter__(self) -> AsyncIterator[_T]:
         # https://github.com/microsoft/pyright/issues/3464
         page = cast(
             AsyncPageT,
             await self,  # type: ignore
         )
         async for item in page:
             yield item
 
 
-class BaseAsyncPage(BasePage[ModelT], Generic[ModelT]):
+class BaseAsyncPage(BasePage[_T], Generic[_T]):
     _client: AsyncAPIClient = pydantic.PrivateAttr()
 
     def _set_private_attributes(
         self,
-        model: Type[ModelT],
+        model: Type[_T],
         client: AsyncAPIClient,
         options: FinalRequestOptions,
     ) -> None:
         self._model = model
         self._client = client
         self._options = options
 
-    async def __aiter__(self) -> AsyncIterator[ModelT]:
+    async def __aiter__(self) -> AsyncIterator[_T]:
         async for page in self.iter_pages():
             for item in page._get_page_items():
                 yield item
 
     async def iter_pages(self: AsyncPageT) -> AsyncIterator[AsyncPageT]:
         page = self
         while True:
@@ -524,15 +522,15 @@
         data: object,
         cast_to: type[ResponseT],
         response: httpx.Response,
     ) -> ResponseT:
         if data is None:
             return cast(ResponseT, None)
 
-        if cast_to is UnknownResponse:
+        if cast_to is object:
             return cast(ResponseT, data)
 
         try:
             if inspect.isclass(cast_to) and issubclass(cast_to, ModelBuilderProtocol):
                 return cast(ResponseT, cast_to.build(response=response, data=data))
 
             if self._strict_response_validation:
@@ -966,15 +964,15 @@
             remaining_retries=remaining,
             stream=stream,
             stream_cls=stream_cls,
         )
 
     def _request_api_list(
         self,
-        model: Type[ModelT],
+        model: Type[object],
         page: Type[SyncPageT],
         options: FinalRequestOptions,
     ) -> SyncPageT:
         def _parser(resp: SyncPageT) -> SyncPageT:
             resp._set_private_attributes(
                 client=self,
                 model=model,
@@ -1128,15 +1126,15 @@
         opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
         return self.request(cast_to, opts)
 
     def get_api_list(
         self,
         path: str,
         *,
-        model: Type[ModelT],
+        model: Type[object],
         page: Type[SyncPageT],
         body: Body | None = None,
         options: RequestOptions = {},
         method: str = "get",
     ) -> SyncPageT:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
@@ -1430,18 +1428,18 @@
             remaining_retries=remaining,
             stream=stream,
             stream_cls=stream_cls,
         )
 
     def _request_api_list(
         self,
-        model: Type[ModelT],
+        model: Type[_T],
         page: Type[AsyncPageT],
         options: FinalRequestOptions,
-    ) -> AsyncPaginator[ModelT, AsyncPageT]:
+    ) -> AsyncPaginator[_T, AsyncPageT]:
         return AsyncPaginator(client=self, options=options, page_cls=page, model=model)
 
     @overload
     async def get(
         self,
         path: str,
         *,
@@ -1580,21 +1578,20 @@
         opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
         return await self.request(cast_to, opts)
 
     def get_api_list(
         self,
         path: str,
         *,
-        # TODO: support paginating `str`
-        model: Type[ModelT],
+        model: Type[_T],
         page: Type[AsyncPageT],
         body: Body | None = None,
         options: RequestOptions = {},
         method: str = "get",
-    ) -> AsyncPaginator[ModelT, AsyncPageT]:
+    ) -> AsyncPaginator[_T, AsyncPageT]:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
 
 
 def make_request_options(
     *,
     query: Query | None = None,
```

### Comparing `dataherald-0.8.0/src/dataherald/_client.py` & `dataherald-0.9.0/src/dataherald/_client.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_compat.py` & `dataherald-0.9.0/src/dataherald/_compat.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_exceptions.py` & `dataherald-0.9.0/src/dataherald/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_files.py` & `dataherald-0.9.0/src/dataherald/_files.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_models.py` & `dataherald-0.9.0/src/dataherald/_models.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_qs.py` & `dataherald-0.9.0/src/dataherald/_qs.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_resource.py` & `dataherald-0.9.0/src/dataherald/_resource.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_response.py` & `dataherald-0.9.0/src/dataherald/_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime
 import functools
 from typing import TYPE_CHECKING, Any, Union, Generic, TypeVar, Callable, cast
 from typing_extensions import Awaitable, ParamSpec, override, get_origin
 
 import httpx
 
-from ._types import NoneType, UnknownResponse, BinaryResponseContent
+from ._types import NoneType, BinaryResponseContent
 from ._utils import is_given, extract_type_var_from_base
 from ._models import BaseModel, is_basemodel
 from ._constants import RAW_RESPONSE_HEADER
 from ._exceptions import APIResponseValidationError
 
 if TYPE_CHECKING:
     from ._models import FinalRequestOptions
@@ -158,15 +158,15 @@
         # which means we must return *exactly* what was input or transform it in a
         # way that retains the TypeVar state. As we cannot do that in this function
         # then we have to resort to using `cast`. At the time of writing, we know this
         # to be safe as we have handled all the types that could be bound to the
         # `ResponseT` TypeVar, however if that TypeVar is ever updated in the future, then
         # this function would become unsafe but a type checker would not report an error.
         if (
-            cast_to is not UnknownResponse
+            cast_to is not object
             and not origin is list
             and not origin is dict
             and not origin is Union
             and not issubclass(origin, BaseModel)
         ):
             raise RuntimeError(
                 f"Invalid state, expected {cast_to} to be a subclass type of {BaseModel}, {dict}, {list} or {Union}."
```

### Comparing `dataherald-0.8.0/src/dataherald/_streaming.py` & `dataherald-0.9.0/src/dataherald/_streaming.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_types.py` & `dataherald-0.9.0/src/dataherald/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,19 +254,14 @@
     max_retries: int
     timeout: float | Timeout | None
     params: Query
     extra_json: AnyMapping
     idempotency_key: str
 
 
-# Sentinel class used when the response type is an object with an unknown schema
-class UnknownResponse:
-    ...
-
-
 # Sentinel class used until PEP 0661 is accepted
 class NotGiven:
     """
     A sentinel singleton class used to distinguish omitted keyword arguments
     from those passed in with the value None (which may have different behavior).
 
     For example:
@@ -335,15 +330,25 @@
         ...
 
 
 HeadersLike = Union[Headers, HeadersLikeProtocol]
 
 ResponseT = TypeVar(
     "ResponseT",
-    bound="Union[str, None, BaseModel, List[Any], Dict[str, Any], Response, UnknownResponse, ModelBuilderProtocol, BinaryResponseContent]",
+    bound=Union[
+        object,
+        str,
+        None,
+        "BaseModel",
+        List[Any],
+        Dict[str, Any],
+        Response,
+        ModelBuilderProtocol,
+        BinaryResponseContent,
+    ],
 )
 
 StrBytesIntFloat = Union[str, bytes, int, float]
 
 # Note: copied from Pydantic
 # https://github.com/pydantic/pydantic/blob/32ea570bf96e84234d2992e1ddf40ab8a565925a/pydantic/main.py#L49
 IncEx: TypeAlias = "set[int] | set[str] | dict[int, Any] | dict[str, Any] | None"
```

### Comparing `dataherald-0.8.0/src/dataherald/_utils/__init__.py` & `dataherald-0.9.0/src/dataherald/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_utils/_logs.py` & `dataherald-0.9.0/src/dataherald/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_utils/_proxy.py` & `dataherald-0.9.0/src/dataherald/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_utils/_transform.py` & `dataherald-0.9.0/src/dataherald/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_utils/_typing.py` & `dataherald-0.9.0/src/dataherald/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/_utils/_utils.py` & `dataherald-0.9.0/src/dataherald/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/resources/__init__.py` & `dataherald-0.9.0/src/dataherald/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/resources/engine.py` & `dataherald-0.9.0/src/dataherald/resources/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
-from .._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-    UnknownResponse,
-)
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from .._base_client import (
     make_request_options,
 )
 
@@ -39,15 +32,15 @@
     ) -> object:
         """Engine Heartbeat"""
         return self._get(
             "/engine/heartbeat",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class AsyncEngine(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncEngineWithRawResponse:
         return AsyncEngineWithRawResponse(self)
@@ -64,15 +57,15 @@
     ) -> object:
         """Engine Heartbeat"""
         return await self._get(
             "/engine/heartbeat",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class EngineWithRawResponse:
     def __init__(self, engine: Engine) -> None:
         self.heartbeat = to_raw_response_wrapper(
             engine.heartbeat,
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/finetunings.py` & `dataherald-0.9.0/src/dataherald/resources/finetunings.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,15 @@
 
 from ..types import (
     FinetuningResponse,
     FinetuningListResponse,
     finetuning_list_params,
     finetuning_create_params,
 )
-from .._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-)
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from .._base_client import (
     make_request_options,
 )
@@ -34,16 +28,17 @@
     @cached_property
     def with_raw_response(self) -> FinetuningsWithRawResponse:
         return FinetuningsWithRawResponse(self)
 
     def create(
         self,
         *,
-        base_llm: finetuning_create_params.BaseLlm,
         db_connection_id: str,
+        alias: str | NotGiven = NOT_GIVEN,
+        base_llm: finetuning_create_params.BaseLlm | NotGiven = NOT_GIVEN,
         golden_records: List[str] | NotGiven = NOT_GIVEN,
         metadata: object | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -61,16 +56,17 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._post(
             "/api/finetunings",
             body=maybe_transform(
                 {
-                    "base_llm": base_llm,
                     "db_connection_id": db_connection_id,
+                    "alias": alias,
+                    "base_llm": base_llm,
                     "golden_records": golden_records,
                     "metadata": metadata,
                 },
                 finetuning_create_params.FinetuningCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -151,16 +147,17 @@
     @cached_property
     def with_raw_response(self) -> AsyncFinetuningsWithRawResponse:
         return AsyncFinetuningsWithRawResponse(self)
 
     async def create(
         self,
         *,
-        base_llm: finetuning_create_params.BaseLlm,
         db_connection_id: str,
+        alias: str | NotGiven = NOT_GIVEN,
+        base_llm: finetuning_create_params.BaseLlm | NotGiven = NOT_GIVEN,
         golden_records: List[str] | NotGiven = NOT_GIVEN,
         metadata: object | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -178,16 +175,17 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
             "/api/finetunings",
             body=maybe_transform(
                 {
-                    "base_llm": base_llm,
                     "db_connection_id": db_connection_id,
+                    "alias": alias,
+                    "base_llm": base_llm,
                     "golden_records": golden_records,
                     "metadata": metadata,
                 },
                 finetuning_create_params.FinetuningCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/generations.py` & `dataherald-0.9.0/src/dataherald/resources/generations.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,21 +9,15 @@
 from ..types import (
     GenerationResponse,
     GenerationListResponse,
     generation_list_params,
     generation_update_params,
     generation_sql_generation_params,
 )
-from .._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-)
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from .._base_client import (
     make_request_options,
 )
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/golden_sqls.py` & `dataherald-0.9.0/src/dataherald/resources/golden_sqls.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,15 @@
 
 from ..types import (
     GoldenSqlListResponse,
     GoldenSqlUploadResponse,
     golden_sql_list_params,
     golden_sql_upload_params,
 )
-from .._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-    UnknownResponse,
-)
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from .._base_client import (
     make_request_options,
 )
@@ -138,15 +131,15 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._delete(
             f"/api/golden-sqls/{id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
     def upload(
         self,
         *,
         body: List[golden_sql_upload_params.Body],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -284,15 +277,15 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._delete(
             f"/api/golden-sqls/{id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
     async def upload(
         self,
         *,
         body: List[golden_sql_upload_params.Body],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/heartbeat.py` & `dataherald-0.9.0/src/dataherald/resources/heartbeat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
-from .._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-    UnknownResponse,
-)
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from .._base_client import (
     make_request_options,
 )
 
@@ -39,15 +32,15 @@
     ) -> object:
         """Heartbeat"""
         return self._get(
             "/heartbeat",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class AsyncHeartbeat(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncHeartbeatWithRawResponse:
         return AsyncHeartbeatWithRawResponse(self)
@@ -64,15 +57,15 @@
     ) -> object:
         """Heartbeat"""
         return await self._get(
             "/heartbeat",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class HeartbeatWithRawResponse:
     def __init__(self, heartbeat: Heartbeat) -> None:
         self.retrieve = to_raw_response_wrapper(
             heartbeat.retrieve,
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/nl_generations.py` & `dataherald-0.9.0/src/dataherald/resources/nl_generations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
 from ..types import NlGenerationListResponse, nl_generation_list_params, nl_generation_create_params
-from .._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-)
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from .._base_client import (
     make_request_options,
 )
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/table_descriptions.py` & `dataherald-0.9.0/src/dataherald/resources/table_descriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,15 @@
 from ..types import (
     TableDescriptionResponse,
     TableDescriptionListResponse,
     table_description_list_params,
     table_description_update_params,
     table_description_sync_schemas_params,
 )
-from .._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-    UnknownResponse,
-)
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from .._base_client import (
     make_request_options,
 )
@@ -186,15 +179,15 @@
                     "table_names": table_names,
                 },
                 table_description_sync_schemas_params.TableDescriptionSyncSchemasParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class AsyncTableDescriptions(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncTableDescriptionsWithRawResponse:
         return AsyncTableDescriptionsWithRawResponse(self)
@@ -348,15 +341,15 @@
                     "table_names": table_names,
                 },
                 table_description_sync_schemas_params.TableDescriptionSyncSchemasParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class TableDescriptionsWithRawResponse:
     def __init__(self, table_descriptions: TableDescriptions) -> None:
         self.retrieve = to_raw_response_wrapper(
             table_descriptions.retrieve,
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/database_connections/__init__.py` & `dataherald-0.9.0/src/dataherald/resources/database_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/resources/database_connections/database_connections.py` & `dataherald-0.9.0/src/dataherald/resources/database_connections/database_connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,21 +9,15 @@
 from ...types import (
     DBConnectionResponse,
     DatabaseConnectionListResponse,
     database_connection_create_params,
     database_connection_update_params,
 )
 from .drivers import Drivers, AsyncDrivers, DriversWithRawResponse, AsyncDriversWithRawResponse
-from ..._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-)
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/database_connections/drivers.py` & `dataherald-0.9.0/src/dataherald/resources/database_connections/drivers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
-from ..._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-)
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
 from ...types.database_connections import DriverListResponse
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/instructions/first.py` & `dataherald-0.9.0/src/dataherald/resources/instructions/first.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
-from ..._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-)
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
 from ...types.shared import InstructionResponse
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/instructions/instructions.py` & `dataherald-0.9.0/src/dataherald/resources/instructions/instructions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,15 @@
 from .first import First, AsyncFirst, FirstWithRawResponse, AsyncFirstWithRawResponse
 from ...types import (
     InstructionListResponse,
     instruction_list_params,
     instruction_create_params,
     instruction_update_params,
 )
-from ..._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-    UnknownResponse,
-)
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
@@ -184,15 +177,15 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._delete(
             f"/api/instructions/{id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class AsyncInstructions(AsyncAPIResource):
     @cached_property
     def first(self) -> AsyncFirst:
         return AsyncFirst(self._client)
@@ -345,15 +338,15 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._delete(
             f"/api/instructions/{id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class InstructionsWithRawResponse:
     def __init__(self, instructions: Instructions) -> None:
         self.first = FirstWithRawResponse(instructions.first)
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/prompts/__init__.py` & `dataherald-0.9.0/src/dataherald/resources/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/resources/prompts/prompts.py` & `dataherald-0.9.0/src/dataherald/resources/prompts/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
 from ...types import PromptResponse, PromptListResponse, prompt_list_params, prompt_create_params
-from ..._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-)
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/prompts/sql_generations.py` & `dataherald-0.9.0/src/dataherald/resources/prompts/sql_generations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
-from ..._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-    UnknownResponse,
-)
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
@@ -118,15 +111,15 @@
                         "order": order,
                         "page": page,
                         "page_size": page_size,
                     },
                     sql_generation_retrieve_params.SqlGenerationRetrieveParams,
                 ),
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
     def nl_generations(
         self,
         id: str,
         *,
         sql_generation: sql_generation_nl_generations_params.SqlGeneration,
@@ -257,15 +250,15 @@
                         "order": order,
                         "page": page,
                         "page_size": page_size,
                     },
                     sql_generation_retrieve_params.SqlGenerationRetrieveParams,
                 ),
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
     async def nl_generations(
         self,
         id: str,
         *,
         sql_generation: sql_generation_nl_generations_params.SqlGeneration,
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/sql_generations/__init__.py` & `dataherald-0.9.0/src/dataherald/resources/sql_generations/__init__.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/resources/sql_generations/nl_generations.py` & `dataherald-0.9.0/src/dataherald/resources/sql_generations/nl_generations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
-from ..._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-    UnknownResponse,
-)
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
@@ -110,15 +103,15 @@
                         "order": order,
                         "page": page,
                         "page_size": page_size,
                     },
                     nl_generation_retrieve_params.NlGenerationRetrieveParams,
                 ),
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class AsyncNlGenerations(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncNlGenerationsWithRawResponse:
         return AsyncNlGenerationsWithRawResponse(self)
@@ -203,15 +196,15 @@
                         "order": order,
                         "page": page,
                         "page_size": page_size,
                     },
                     nl_generation_retrieve_params.NlGenerationRetrieveParams,
                 ),
             ),
-            cast_to=UnknownResponse,
+            cast_to=object,
         )
 
 
 class NlGenerationsWithRawResponse:
     def __init__(self, nl_generations: NlGenerations) -> None:
         self.create = to_raw_response_wrapper(
             nl_generations.create,
```

### Comparing `dataherald-0.8.0/src/dataherald/resources/sql_generations/sql_generations.py` & `dataherald-0.9.0/src/dataherald/resources/sql_generations/sql_generations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,15 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import httpx
 
-from ...types import (
-    SqlGenerationListResponse,
-    SqlGenerationExecuteResponse,
-    sql_generation_list_params,
-    sql_generation_create_params,
-    sql_generation_execute_params,
-)
-from ..._types import (
-    NOT_GIVEN,
-    Body,
-    Query,
-    Headers,
-    NotGiven,
-)
+from ...types import SqlGenerationListResponse, sql_generation_list_params, sql_generation_create_params
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import to_raw_response_wrapper, async_to_raw_response_wrapper
 from ..._base_client import (
     make_request_options,
 )
@@ -163,47 +151,14 @@
                     },
                     sql_generation_list_params.SqlGenerationListParams,
                 ),
             ),
             cast_to=SqlGenerationListResponse,
         )
 
-    def execute(
-        self,
-        id: str,
-        *,
-        max_rows: int,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SqlGenerationExecuteResponse:
-        """
-        Execute Sql Generation
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        return self._post(
-            f"/api/sql-generations/{id}/execute",
-            body=maybe_transform({"max_rows": max_rows}, sql_generation_execute_params.SqlGenerationExecuteParams),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=SqlGenerationExecuteResponse,
-        )
-
 
 class AsyncSqlGenerations(AsyncAPIResource):
     @cached_property
     def nl_generations(self) -> AsyncNlGenerations:
         return AsyncNlGenerations(self._client)
 
     @cached_property
@@ -328,64 +283,28 @@
                     },
                     sql_generation_list_params.SqlGenerationListParams,
                 ),
             ),
             cast_to=SqlGenerationListResponse,
         )
 
-    async def execute(
-        self,
-        id: str,
-        *,
-        max_rows: int,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> SqlGenerationExecuteResponse:
-        """
-        Execute Sql Generation
-
-        Args:
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          timeout: Override the client-level default timeout for this request, in seconds
-        """
-        return await self._post(
-            f"/api/sql-generations/{id}/execute",
-            body=maybe_transform({"max_rows": max_rows}, sql_generation_execute_params.SqlGenerationExecuteParams),
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
-            ),
-            cast_to=SqlGenerationExecuteResponse,
-        )
-
 
 class SqlGenerationsWithRawResponse:
     def __init__(self, sql_generations: SqlGenerations) -> None:
         self.nl_generations = NlGenerationsWithRawResponse(sql_generations.nl_generations)
 
         self.create = to_raw_response_wrapper(
             sql_generations.create,
         )
         self.retrieve = to_raw_response_wrapper(
             sql_generations.retrieve,
         )
         self.list = to_raw_response_wrapper(
             sql_generations.list,
         )
-        self.execute = to_raw_response_wrapper(
-            sql_generations.execute,
-        )
 
 
 class AsyncSqlGenerationsWithRawResponse:
     def __init__(self, sql_generations: AsyncSqlGenerations) -> None:
         self.nl_generations = AsyncNlGenerationsWithRawResponse(sql_generations.nl_generations)
 
         self.create = async_to_raw_response_wrapper(
@@ -393,10 +312,7 @@
         )
         self.retrieve = async_to_raw_response_wrapper(
             sql_generations.retrieve,
         )
         self.list = async_to_raw_response_wrapper(
             sql_generations.list,
         )
-        self.execute = async_to_raw_response_wrapper(
-            sql_generations.execute,
-        )
```

### Comparing `dataherald-0.8.0/src/dataherald/types/__init__.py` & `dataherald-0.9.0/src/dataherald/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,17 +33,15 @@
 from .golden_sql_upload_response import GoldenSqlUploadResponse as GoldenSqlUploadResponse
 from .sql_generation_list_params import SqlGenerationListParams as SqlGenerationListParams
 from .table_description_response import TableDescriptionResponse as TableDescriptionResponse
 from .nl_generation_create_params import NlGenerationCreateParams as NlGenerationCreateParams
 from .nl_generation_list_response import NlGenerationListResponse as NlGenerationListResponse
 from .sql_generation_create_params import SqlGenerationCreateParams as SqlGenerationCreateParams
 from .sql_generation_list_response import SqlGenerationListResponse as SqlGenerationListResponse
-from .sql_generation_execute_params import SqlGenerationExecuteParams as SqlGenerationExecuteParams
 from .table_description_list_params import TableDescriptionListParams as TableDescriptionListParams
-from .sql_generation_execute_response import SqlGenerationExecuteResponse as SqlGenerationExecuteResponse
 from .table_description_list_response import TableDescriptionListResponse as TableDescriptionListResponse
 from .table_description_update_params import TableDescriptionUpdateParams as TableDescriptionUpdateParams
 from .generation_sql_generation_params import GenerationSqlGenerationParams as GenerationSqlGenerationParams
 from .database_connection_create_params import DatabaseConnectionCreateParams as DatabaseConnectionCreateParams
 from .database_connection_list_response import DatabaseConnectionListResponse as DatabaseConnectionListResponse
 from .database_connection_update_params import DatabaseConnectionUpdateParams as DatabaseConnectionUpdateParams
 from .table_description_sync_schemas_params import (
```

### Comparing `dataherald-0.8.0/src/dataherald/types/database_connection_create_params.py` & `dataherald-0.9.0/src/dataherald/types/database_connection_create_params.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/database_connection_update_params.py` & `dataherald-0.9.0/src/dataherald/types/database_connection_update_params.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/db_connection_response.py` & `dataherald-0.9.0/src/dataherald/types/db_connection_response.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/finetuning_create_params.py` & `dataherald-0.9.0/src/dataherald/types/finetuning_create_params.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 from typing import Dict, List
 from typing_extensions import Required, TypedDict
 
 __all__ = ["FinetuningCreateParams", "BaseLlm"]
 
 
 class FinetuningCreateParams(TypedDict, total=False):
-    base_llm: Required[BaseLlm]
-
     db_connection_id: Required[str]
 
+    alias: str
+
+    base_llm: BaseLlm
+
     golden_records: List[str]
 
     metadata: object
 
 
 class BaseLlm(TypedDict, total=False):
     _model_name: str
```

### Comparing `dataherald-0.8.0/src/dataherald/types/finetuning_response.py` & `dataherald-0.9.0/src/dataherald/types/finetuning_response.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/generation_list_item.py` & `dataherald-0.9.0/src/dataherald/types/generation_list_item.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/generation_response.py` & `dataherald-0.9.0/src/dataherald/types/generation_response.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/nl_generation_create_params.py` & `dataherald-0.9.0/src/dataherald/types/nl_generation_create_params.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/prompt_response.py` & `dataherald-0.9.0/src/dataherald/types/prompt_response.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/table_description_response.py` & `dataherald-0.9.0/src/dataherald/types/table_description_response.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/table_description_update_params.py` & `dataherald-0.9.0/src/dataherald/types/table_description_update_params.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/shared/golden_sql_response.py` & `dataherald-0.9.0/src/dataherald/types/shared/golden_sql_response.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/shared/nl_generation_response.py` & `dataherald-0.9.0/src/dataherald/types/shared/nl_generation_response.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/src/dataherald/types/shared/sql_generation_response.py` & `dataherald-0.9.0/src/dataherald/types/shared/sql_generation_response.py`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/LICENSE` & `dataherald-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/README.md` & `dataherald-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dataherald-0.8.0/pyproject.toml` & `dataherald-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dataherald"
-version = "0.8.0"
+version = "0.9.0"
 description = "The official Python library for the Dataherald API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Dataherald", email = "support@dataherald.com" },
 ]
 dependencies = [
```

### Comparing `dataherald-0.8.0/PKG-INFO` & `dataherald-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataherald
-Version: 0.8.0
+Version: 0.9.0
 Summary: The official Python library for the Dataherald API
 Project-URL: Homepage, https://github.com/Dataherald/dataherald-python
 Project-URL: Repository, https://github.com/Dataherald/dataherald-python
 Author-email: Dataherald <support@dataherald.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```


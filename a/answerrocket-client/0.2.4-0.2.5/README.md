# Comparing `tmp/answerrocket_client-0.2.4.tar.gz` & `tmp/answerrocket_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "answerrocket_client-0.2.4.tar", last modified: Thu May 16 12:59:29 2024, max compression
+gzip compressed data, was "answerrocket_client-0.2.5.tar", last modified: Mon May 20 20:25:44 2024, max compression
```

## Comparing `answerrocket_client-0.2.4.tar` & `answerrocket_client-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:29.620803 answerrocket_client-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-16 12:59:29.620803 answerrocket_client-0.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:29.620803 answerrocket_client-0.2.4/answer_rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:29.620803 answerrocket_client-0.2.4/answer_rocket/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/graphql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    51195 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/graphql/sdk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/answer_rocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:29.620803 answerrocket_client-0.2.4/answerrocket_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-16 12:59:29.000000 answerrocket_client-0.2.4/answerrocket_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-16 12:59:29.000000 answerrocket_client-0.2.4/answerrocket_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:59:29.000000 answerrocket_client-0.2.4/answerrocket_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 12:59:29.000000 answerrocket_client-0.2.4/answerrocket_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 12:59:29.000000 answerrocket_client-0.2.4/answerrocket_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:59:29.620803 answerrocket_client-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:59:29.620803 answerrocket_client-0.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 12:59:25.000000 answerrocket_client-0.2.4/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.963934 answerrocket_client-0.2.5/answer_rocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.963934 answerrocket_client-0.2.5/answer_rocket/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/graphql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51671 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/graphql/sdk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/answerrocket_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/test/test_client.py
```

### Comparing `answerrocket_client-0.2.4/PKG-INFO` & `answerrocket_client-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.4/answer_rocket/auth.py` & `answerrocket_client-0.2.5/answer_rocket/auth.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/answer_rocket/chat.py` & `answerrocket_client-0.2.5/answer_rocket/chat.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/answer_rocket/client.py` & `answerrocket_client-0.2.5/answer_rocket/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/answer_rocket/config.py` & `answerrocket_client-0.2.5/answer_rocket/config.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/answer_rocket/data.py` & `answerrocket_client-0.2.5/answer_rocket/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
-from typing import Optional
+from typing import Optional, List
 from uuid import UUID
 
 import pandas as pd
 from sgqlc.operation import Fragment
-from sgqlc.types import Variable, Arg, non_null, String, Int
+from sgqlc.types import Variable, Arg, non_null, String, Int, list_of
 
 from answer_rocket.auth import AuthHelper
 from answer_rocket.graphql.client import GraphQlClient
 from answer_rocket.graphql.schema import UUID as GQL_UUID, MaxMetricAttribute, MaxDomainObject, \
     MaxDimensionEntity, MaxFactEntity, MaxNormalAttribute, \
-    MaxPrimaryAttribute, MaxReferenceAttribute, MaxCalculatedMetric, MaxDataset, MaxCalculatedAttribute
+    MaxPrimaryAttribute, MaxReferenceAttribute, MaxCalculatedMetric, MaxDataset, MaxCalculatedAttribute, \
+    MaxMutationResponse
 from answer_rocket.types import MaxResult, RESULT_EXCEPTION_CODE
 
 
 class ExecuteSqlQueryResult(MaxResult):
     df = None
 
 
@@ -479,7 +480,40 @@
         # fragment.domain_entity().id()
         # fragment.domain_entity().name()
 
     def _add_dimension_attribute_fields(self, fragment: Fragment):
         fragment.default_filter_value()
         fragment.is_required_in_query()
         fragment.dimension_value_mapping_list()
+
+    def reload_dataset(self, dataset_id: Optional[UUID] = None, database_id: Optional[UUID] = None, table_names: Optional[List[str]] = None) -> MaxMutationResponse:
+        try:
+            """
+            dataset_id: the UUID of the dataset
+            """
+            mutation_args = {
+                'datasetId': str(dataset_id) if dataset_id is not None else None,
+                'databaseId': str(database_id) if database_id is not None else None,
+                'tableNames': table_names
+            }
+
+            mutation_vars = {
+                'dataset_id': Arg(GQL_UUID),
+                'database_id': Arg(GQL_UUID),
+                'table_names': Arg(list_of(non_null(String))),
+            }
+
+            operation = self._gql_client.mutation(variables=mutation_vars)
+
+            operation.reload_dataset(
+                dataset_id=Variable('dataset_id'),
+                database_id=Variable('database_id'),
+                table_names=Variable('table_names'),
+            )
+
+            result = self._gql_client.submit(operation, mutation_args)
+
+            mutation_response = result.reload_dataset
+
+            return mutation_response
+        except Exception as e:
+            return None
```

### Comparing `answerrocket_client-0.2.4/answer_rocket/graphql/client.py` & `answerrocket_client-0.2.5/answer_rocket/graphql/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/answer_rocket/graphql/schema.py` & `answerrocket_client-0.2.5/answer_rocket/graphql/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
     first_name = sgqlc.types.Field(String, graphql_name='firstName')
     last_name = sgqlc.types.Field(String, graphql_name='lastName')
     email_address = sgqlc.types.Field(String, graphql_name='emailAddress')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('create_max_copilot_skill_chat_question', 'update_max_copilot_skill_chat_question', 'delete_max_copilot_skill_chat_question', 'create_max_copilot_question', 'update_max_copilot_question', 'delete_max_copilot_question', 'update_chat_answer_payload', 'ask_chat_question', 'evaluate_chat_question', 'queue_chat_question', 'cancel_chat_question', 'create_chat_thread')
+    __field_names__ = ('create_max_copilot_skill_chat_question', 'update_max_copilot_skill_chat_question', 'delete_max_copilot_skill_chat_question', 'create_max_copilot_question', 'update_max_copilot_question', 'delete_max_copilot_question', 'reload_dataset', 'update_chat_answer_payload', 'ask_chat_question', 'evaluate_chat_question', 'queue_chat_question', 'cancel_chat_question', 'create_chat_thread')
     create_max_copilot_skill_chat_question = sgqlc.types.Field(sgqlc.types.non_null(CreateMaxCopilotSkillChatQuestionResponse), graphql_name='createMaxCopilotSkillChatQuestion', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
         ('copilot_skill_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId', default=None)),
         ('question', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='question', default=None)),
         ('expected_completion_response', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='expectedCompletionResponse', default=None)),
 ))
     )
@@ -550,14 +550,20 @@
 ))
     )
     delete_max_copilot_question = sgqlc.types.Field(sgqlc.types.non_null(MaxMutationResponse), graphql_name='deleteMaxCopilotQuestion', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
         ('copilot_question_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotQuestionId', default=None)),
 ))
     )
+    reload_dataset = sgqlc.types.Field(sgqlc.types.non_null(MaxMutationResponse), graphql_name='reloadDataset', args=sgqlc.types.ArgDict((
+        ('dataset_id', sgqlc.types.Arg(UUID, graphql_name='datasetId', default=None)),
+        ('database_id', sgqlc.types.Arg(UUID, graphql_name='databaseId', default=None)),
+        ('table_names', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='tableNames', default=None)),
+))
+    )
     update_chat_answer_payload = sgqlc.types.Field(JSON, graphql_name='updateChatAnswerPayload', args=sgqlc.types.ArgDict((
         ('answer_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='answerId', default=None)),
         ('payload', sgqlc.types.Arg(sgqlc.types.non_null(JSON), graphql_name='payload', default=None)),
 ))
     )
     ask_chat_question = sgqlc.types.Field(MaxChatEntry, graphql_name='askChatQuestion', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
```

### Comparing `answerrocket_client-0.2.4/answer_rocket/graphql/sdk_operations.py` & `answerrocket_client-0.2.5/answer_rocket/graphql/sdk_operations.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/answer_rocket/output.py` & `answerrocket_client-0.2.5/answer_rocket/output.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/answer_rocket/skill.py` & `answerrocket_client-0.2.5/answer_rocket/skill.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/answerrocket_client.egg-info/PKG-INFO` & `answerrocket_client-0.2.5/answerrocket_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.4/answerrocket_client.egg-info/SOURCES.txt` & `answerrocket_client-0.2.5/answerrocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.4/readme.md` & `answerrocket_client-0.2.5/readme.md`

 * *Files identical despite different names*


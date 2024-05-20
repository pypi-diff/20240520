# Comparing `tmp/langchain_astradb-0.3.1.tar.gz` & `tmp/langchain_astradb-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_astradb-0.3.1.tar", max compression
+gzip compressed data, was "langchain_astradb-0.3.2.tar", max compression
```

## Comparing `langchain_astradb-0.3.1.tar` & `langchain_astradb-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/LICENSE
--rw-r--r--   0        0        0     2058 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/README.md
--rw-r--r--   0        0        0      624 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/__init__.py
--rw-r--r--   0        0        0    20613 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/cache.py
--rw-r--r--   0        0        0     5344 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/chat_message_histories.py
--rw-r--r--   0        0        0     4549 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/document_loaders.py
--rw-r--r--   0        0        0        0 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/py.typed
--rw-r--r--   0        0        0     8833 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/storage.py
--rw-r--r--   0        0        0    14319 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/utils/astradb.py
--rw-r--r--   0        0        0     3165 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/utils/mmr.py
--rw-r--r--   0        0        0    62160 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/vectorstores.py
--rw-r--r--   0        0        0     2888 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 langchain_astradb-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2058 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/README.md
+-rw-r--r--   0        0        0      624 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/__init__.py
+-rw-r--r--   0        0        0    21179 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/cache.py
+-rw-r--r--   0        0        0     5627 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/chat_message_histories.py
+-rw-r--r--   0        0        0     4837 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/document_loaders.py
+-rw-r--r--   0        0        0        0 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/py.typed
+-rw-r--r--   0        0        0     9399 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/storage.py
+-rw-r--r--   0        0        0    15826 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/utils/astradb.py
+-rw-r--r--   0        0        0     3165 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/utils/mmr.py
+-rw-r--r--   0        0        0    62443 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/vectorstores.py
+-rw-r--r--   0        0        0     2888 2024-05-20 19:31:29.279205 langchain_astradb-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 langchain_astradb-0.3.2/PKG-INFO
```

### Comparing `langchain_astradb-0.3.1/LICENSE` & `langchain_astradb-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.1/README.md` & `langchain_astradb-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.1/langchain_astradb/__init__.py` & `langchain_astradb-0.3.2/langchain_astradb/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.1/langchain_astradb/cache.py` & `langchain_astradb-0.3.2/langchain_astradb/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,23 +108,26 @@
         The lookup keys, combined in the _id of the documents, are:
             - prompt, a string
             - llm_string, a deterministic str representation of the model parameters.
               (needed to prevent same-prompt-different-model collisions)
 
         Args:
             collection_name: name of the Astra DB collection to create/use.
-            token: API token for Astra DB usage.
-            api_endpoint: full URL to the API endpoint,
-                such as `https://<DB-ID>-us-east1.apps.astra.datastax.com`.
+            token: API token for Astra DB usage. If not provided, the environment
+                variable ASTRA_DB_APPLICATION_TOKEN is inspected.
+            api_endpoint: full URL to the API endpoint, such as
+                `https://<DB-ID>-us-east1.apps.astra.datastax.com`. If not provided,
+                the environment variable ASTRA_DB_API_ENDPOINT is inspected.
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AsyncAstraDB' instance.
-            namespace: namespace (aka keyspace) where the
-                collection is created. Defaults to the database's "default namespace".
+            namespace: namespace (aka keyspace) where the collection is created.
+                If not provided, the environment variable ASTRA_DB_KEYSPACE is
+                inspected. Defaults to the database's "default namespace".
             setup_mode: mode used to create the Astra DB collection (SYNC, ASYNC or
                 OFF).
             pre_delete_collection: whether to delete the collection
                 before creating it. If False and the collection already exists,
                 the collection will be used as is.
         """
         self.astra_env = _AstraDBCollectionEnvironment(
@@ -303,23 +306,26 @@
 
         You can choose the preferred similarity (or use the API default).
         The default score threshold is tuned to the default metric.
         Tune it carefully yourself if switching to another distance metric.
 
         Args:
             collection_name: name of the Astra DB collection to create/use.
-            token: API token for Astra DB usage.
-            api_endpoint: full URL to the API endpoint,
-                such as `https://<DB-ID>-us-east1.apps.astra.datastax.com`.
+            token: API token for Astra DB usage. If not provided, the environment
+                variable ASTRA_DB_APPLICATION_TOKEN is inspected.
+            api_endpoint: full URL to the API endpoint, such as
+                `https://<DB-ID>-us-east1.apps.astra.datastax.com`. If not provided,
+                the environment variable ASTRA_DB_API_ENDPOINT is inspected.
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AsyncAstraDB' instance.
-            namespace: namespace (aka keyspace) where the
-                collection is created. Defaults to the database's "default namespace".
+            namespace: namespace (aka keyspace) where the collection is created.
+                If not provided, the environment variable ASTRA_DB_KEYSPACE is
+                inspected. Defaults to the database's "default namespace".
             setup_mode: mode used to create the Astra DB collection (SYNC, ASYNC or
                 OFF).
             pre_delete_collection: whether to delete the collection
                 before creating it. If False and the collection already exists,
                 the collection will be used as is.
             embedding: Embedding provider for semantic encoding and search.
             metric: the function to use for evaluating similarity of text embeddings.
```

### Comparing `langchain_astradb-0.3.1/langchain_astradb/chat_message_histories.py` & `langchain_astradb-0.3.2/langchain_astradb/chat_message_histories.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,23 +37,26 @@
     ) -> None:
         """Chat message history that stores history in Astra DB.
 
         Args:
             session_id: arbitrary key that is used to store the messages
                 of a single chat session.
             collection_name: name of the Astra DB collection to create/use.
-            token: API token for Astra DB usage.
-            api_endpoint: full URL to the API endpoint,
-                such as "https://<DB-ID>-us-east1.apps.astra.datastax.com".
+            token: API token for Astra DB usage. If not provided, the environment
+                variable ASTRA_DB_APPLICATION_TOKEN is inspected.
+            api_endpoint: full URL to the API endpoint, such as
+                `https://<DB-ID>-us-east1.apps.astra.datastax.com`. If not provided,
+                the environment variable ASTRA_DB_API_ENDPOINT is inspected.
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AsyncAstraDB' instance.
-            namespace: namespace (aka keyspace) where the
-                collection is created. Defaults to the database's "default namespace".
+            namespace: namespace (aka keyspace) where the collection is created.
+                If not provided, the environment variable ASTRA_DB_KEYSPACE is
+                inspected. Defaults to the database's "default namespace".
         """
         self.astra_env = _AstraDBCollectionEnvironment(
             collection_name=collection_name,
             token=token,
             api_endpoint=api_endpoint,
             astra_db_client=astra_db_client,
             async_astra_db_client=async_astra_db_client,
```

### Comparing `langchain_astradb-0.3.1/langchain_astradb/document_loaders.py` & `langchain_astradb-0.3.2/langchain_astradb/document_loaders.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,23 +43,26 @@
         page_content_mapper: Callable[[Dict], str] = json.dumps,
         metadata_mapper: Optional[Callable[[Dict], Dict[str, Any]]] = None,
     ) -> None:
         """Load DataStax Astra DB documents.
 
         Args:
             collection_name: name of the Astra DB collection to use.
-            token: API token for Astra DB usage.
-            api_endpoint: full URL to the API endpoint,
-                such as `https://<DB-ID>-us-east1.apps.astra.datastax.com`.
+            token: API token for Astra DB usage. If not provided, the environment
+                variable ASTRA_DB_APPLICATION_TOKEN is inspected.
+            api_endpoint: full URL to the API endpoint, such as
+                `https://<DB-ID>-us-east1.apps.astra.datastax.com`. If not provided,
+                the environment variable ASTRA_DB_API_ENDPOINT is inspected.
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AsyncAstraDB' instance.
-            namespace: namespace (aka keyspace) where the
-                collection is. Defaults to the database's "default namespace".
+            namespace: namespace (aka keyspace) where the collection resides.
+                If not provided, the environment variable ASTRA_DB_KEYSPACE is
+                inspected. Defaults to the database's "default namespace".
             filter_criteria: Criteria to filter documents.
             projection: Specifies the fields to return. If not provided, reads
                 fall back to the Data API default projection.
             find_options: Additional options for the query.
             nb_prefetched: Max number of documents to pre-fetch. Defaults to 1000.
             page_content_mapper: Function applied to collection documents to create
                 the `page_content` of the LangChain Document. Defaults to `json.dumps`.
```

### Comparing `langchain_astradb-0.3.1/langchain_astradb/storage.py` & `langchain_astradb-0.3.2/langchain_astradb/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,23 +134,26 @@
             {
               "_id": "<key>",
               "value": <value>
             }
 
         Args:
             collection_name: name of the Astra DB collection to create/use.
-            token: API token for Astra DB usage.
-            api_endpoint: full URL to the API endpoint,
-                such as `https://<DB-ID>-us-east1.apps.astra.datastax.com`.
+            token: API token for Astra DB usage. If not provided, the environment
+                variable ASTRA_DB_APPLICATION_TOKEN is inspected.
+            api_endpoint: full URL to the API endpoint, such as
+                `https://<DB-ID>-us-east1.apps.astra.datastax.com`. If not provided,
+                the environment variable ASTRA_DB_API_ENDPOINT is inspected.
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AsyncAstraDB' instance.
-            namespace: namespace (aka keyspace) where the
-                collection is created. Defaults to the database's "default namespace".
+            namespace: namespace (aka keyspace) where the collection is created.
+                If not provided, the environment variable ASTRA_DB_KEYSPACE is
+                inspected. Defaults to the database's "default namespace".
             setup_mode: mode used to create the Astra DB collection (SYNC, ASYNC or
                 OFF).
             pre_delete_collection: whether to delete the collection
                 before creating it. If False and the collection already exists,
                 the collection will be used as is.
         """
         super().__init__(
@@ -193,23 +196,26 @@
             {
               "_id": "<key>",
               "value": "<byte64 string value>"
             }
 
         Args:
             collection_name: name of the Astra DB collection to create/use.
-            token: API token for Astra DB usage.
-            api_endpoint: full URL to the API endpoint,
-                such as `https://<DB-ID>-us-east1.apps.astra.datastax.com`.
+            token: API token for Astra DB usage. If not provided, the environment
+                variable ASTRA_DB_APPLICATION_TOKEN is inspected.
+            api_endpoint: full URL to the API endpoint, such as
+                `https://<DB-ID>-us-east1.apps.astra.datastax.com`. If not provided,
+                the environment variable ASTRA_DB_API_ENDPOINT is inspected.
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AsyncAstraDB' instance.
-            namespace: namespace (aka keyspace) where the
-                collection is created. Defaults to the database's "default namespace".
+            namespace: namespace (aka keyspace) where the collection is created.
+                If not provided, the environment variable ASTRA_DB_KEYSPACE is
+                inspected. Defaults to the database's "default namespace".
             setup_mode: mode used to create the Astra DB collection (SYNC, ASYNC or
                 OFF).
             pre_delete_collection: whether to delete the collection
                 before creating it. If False and the collection already exists,
                 the collection will be used as is.
         """
         super().__init__(
```

### Comparing `langchain_astradb-0.3.1/langchain_astradb/utils/astradb.py` & `langchain_astradb-0.3.2/langchain_astradb/utils/astradb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
 import json
+import logging
+import os
 import warnings
 from asyncio import InvalidStateError, Task
 from enum import Enum
 from typing import Any, Awaitable, Dict, List, Optional, Union
 
 import langchain_core
 from astrapy.api import APIRequestError
 from astrapy.db import AstraDB, AstraDBCollection, AsyncAstraDB, AsyncAstraDBCollection
 from astrapy.info import CollectionVectorServiceOptions
 
+TOKEN_ENV_VAR = "ASTRA_DB_APPLICATION_TOKEN"
+API_ENDPOINT_ENV_VAR = "ASTRA_DB_API_ENDPOINT"
+NAMESPACE_ENV_VAR = "ASTRA_DB_KEYSPACE"
+
+logger = logging.getLogger()
+
 
 class SetupMode(Enum):
     SYNC = 1
     ASYNC = 2
     OFF = 3
 
 
@@ -25,54 +33,86 @@
         self,
         token: Optional[str] = None,
         api_endpoint: Optional[str] = None,
         astra_db_client: Optional[AstraDB] = None,
         async_astra_db_client: Optional[AsyncAstraDB] = None,
         namespace: Optional[str] = None,
     ) -> None:
-        self.token = token
-        self.api_endpoint = api_endpoint
-        astra_db = astra_db_client
-        async_astra_db = async_astra_db_client
-        self.namespace = namespace
+        self.token: Optional[str]
+        self.api_endpoint: Optional[str]
+        self.namespace: Optional[str]
 
-        # Conflicting-arg checks:
         if astra_db_client is not None or async_astra_db_client is not None:
             if token is not None or api_endpoint is not None:
                 raise ValueError(
                     "You cannot pass 'astra_db_client' or 'async_astra_db_client' to "
                     "AstraDBEnvironment if passing 'token' and 'api_endpoint'."
                 )
+            if astra_db_client is not None:
+                _astra_db = astra_db_client.copy()
+            else:
+                _astra_db = None
+            if async_astra_db_client is not None:
+                _async_astra_db = async_astra_db_client.copy()
+            else:
+                _async_astra_db = None
 
-        if token and api_endpoint:
-            astra_db = AstraDB(
-                token=token,
-                api_endpoint=api_endpoint,
-                namespace=self.namespace,
-            )
-            async_astra_db = AsyncAstraDB(
-                token=token,
-                api_endpoint=api_endpoint,
-                namespace=self.namespace,
-            )
-
-        if astra_db:
-            self.astra_db = astra_db.copy()
-            if async_astra_db:
-                self.async_astra_db = async_astra_db.copy()
-            else:
-                self.async_astra_db = self.astra_db.to_async()
-        elif async_astra_db:
-            self.async_astra_db = async_astra_db.copy()
-            self.astra_db = self.async_astra_db.to_sync()
+            self.token = token
+            self.api_endpoint = api_endpoint
+            self.namespace = namespace
         else:
-            raise ValueError(
-                "Must provide 'astra_db_client' or 'async_astra_db_client' or "
-                "'token' and 'api_endpoint'"
-            )
+            # secrets-based initialization
+            if token is None:
+                logger.info(
+                    "Attempting to fetch token from environment "
+                    f"variable '{TOKEN_ENV_VAR}'"
+                )
+                _token = os.environ.get(TOKEN_ENV_VAR)
+            else:
+                _token = token
+            if api_endpoint is None:
+                logger.info(
+                    "Attempting to fetch API endpoint from environment "
+                    f"variable '{API_ENDPOINT_ENV_VAR}'"
+                )
+                _api_endpoint = os.environ.get(API_ENDPOINT_ENV_VAR)
+            else:
+                _api_endpoint = api_endpoint
+            if namespace is None:
+                _namespace = os.environ.get(NAMESPACE_ENV_VAR)
+            else:
+                _namespace = namespace
+
+            self.token = _token
+            self.api_endpoint = _api_endpoint
+            self.namespace = _namespace
+            #
+            if _token and _api_endpoint:
+                _astra_db = AstraDB(
+                    token=_token,
+                    api_endpoint=_api_endpoint,
+                    namespace=_namespace,
+                )
+                _async_astra_db = None
+            else:
+                raise ValueError(
+                    "API endpoint and/or token for Astra DB not provided. "
+                    "Either pass them explicitly to the object constructor "
+                    f"or set the {API_ENDPOINT_ENV_VAR}, {TOKEN_ENV_VAR} "
+                    "environment variables."
+                )
+
+        # complete sync/async with the other if necessary
+        if _astra_db is None:
+            _astra_db = _async_astra_db.to_sync()  # type: ignore[union-attr]
+        if _async_astra_db is None:
+            _async_astra_db = _astra_db.to_async()
+
+        self.astra_db = _astra_db
+        self.async_astra_db = _async_astra_db
 
         self.astra_db.set_caller(
             caller_name="langchain",
             caller_version=getattr(langchain_core, "__version__", None),
         )
         self.async_astra_db.set_caller(
             caller_name="langchain",
```

### Comparing `langchain_astradb-0.3.1/langchain_astradb/utils/mmr.py` & `langchain_astradb-0.3.2/langchain_astradb/utils/mmr.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.1/langchain_astradb/vectorstores.py` & `langchain_astradb-0.3.2/langchain_astradb/vectorstores.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,23 +180,26 @@
 
         Args:
             embedding: the embeddings function or service to use.
                 This enables client-side embedding functions or calls to external
                 embedding providers. Only one of `embedding` or
                 `collection_vector_service_options` can be provided.
             collection_name: name of the Astra DB collection to create/use.
-            token: API token for Astra DB usage.
+            token: API token for Astra DB usage. If not provided, the environment
+                variable ASTRA_DB_APPLICATION_TOKEN is inspected.
             api_endpoint: full URL to the API endpoint, such as
-                `https://<DB-ID>-us-east1.apps.astra.datastax.com`.
+                `https://<DB-ID>-us-east1.apps.astra.datastax.com`. If not provided,
+                the environment variable ASTRA_DB_API_ENDPOINT is inspected.
             astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AstraDB' instance.
             async_astra_db_client: *alternative to token+api_endpoint*,
                 you can pass an already-created 'astrapy.db.AsyncAstraDB' instance.
             namespace: namespace (aka keyspace) where the collection is created.
-                Defaults to the database's "default namespace".
+                If not provided, the environment variable ASTRA_DB_KEYSPACE is
+                inspected. Defaults to the database's "default namespace".
             metric: similarity function to use out of those available in Astra DB.
                 If left out, it will use Astra DB API's defaults (i.e. "cosine" - but,
                 for performance reasons, "dot_product" is suggested if embeddings are
                 normalized to one).
             batch_size: Size of batches for bulk insertions.
             bulk_insert_batch_concurrency: Number of threads or coroutines to insert
                 batches concurrently.
```

### Comparing `langchain_astradb-0.3.1/pyproject.toml` & `langchain_astradb-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-astradb"
-version = "0.3.1"
+version = "0.3.2"
 description = "An integration package connecting Astra DB and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-datastax"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_astradb-0.3.1/PKG-INFO` & `langchain_astradb-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-astradb
-Version: 0.3.1
+Version: 0.3.2
 Summary: An integration package connecting Astra DB and LangChain
 Home-page: https://github.com/langchain-ai/langchain-datastax
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


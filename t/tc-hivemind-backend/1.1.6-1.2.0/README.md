# Comparing `tmp/tc_hivemind_backend-1.1.6.tar.gz` & `tmp/tc_hivemind_backend-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc_hivemind_backend-1.1.6.tar", last modified: Mon May  6 10:09:05 2024, max compression
+gzip compressed data, was "tc_hivemind_backend-1.2.0.tar", last modified: Mon May 20 07:19:06 2024, max compression
```

## Comparing `tc_hivemind_backend-1.1.6.tar` & `tc_hivemind_backend-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.199918 tc_hivemind_backend-1.1.6/tc_hivemind_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/pg_db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/utils/delete_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/utils/model_hyperparams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/tc_hivemind_backend/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/embeddings/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/pg_vector_access.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/integration/test_delete_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/integration/test_pg_vector_access.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/unit/test_convert_tuple_str.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/unit/test_load_db_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-06 10:08:54.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/unit/test_load_model_hyperparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:05.203918 tc_hivemind_backend-1.1.6/tc_hivemind_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-06 10:09:05.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-06 10:09:05.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:09:05.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-06 10:09:05.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 10:09:05.000000 tc_hivemind_backend-1.1.6/tc_hivemind_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.162875 tc_hivemind_backend-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-20 07:19:06.162875 tc_hivemind_backend-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 07:19:06.162875 tc_hivemind_backend-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.158875 tc_hivemind_backend-1.2.0/tc_hivemind_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.158875 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/pg_db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.158875 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/utils/delete_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/utils/model_hyperparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.162875 tc_hivemind_backend-1.2.0/tc_hivemind_backend/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/embeddings/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/pg_vector_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/qdrant_vector_access.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.162875 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.162875 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/integration/test_delete_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/integration/test_pg_vector_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/integration/test_qdrant_vector_access.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.162875 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/unit/test_convert_tuple_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/unit/test_load_db_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-20 07:18:59.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/unit/test_load_model_hyperparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:19:06.162875 tc_hivemind_backend-1.2.0/tc_hivemind_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-20 07:19:06.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-20 07:19:06.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:19:06.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-20 07:19:06.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 07:19:06.000000 tc_hivemind_backend-1.2.0/tc_hivemind_backend.egg-info/top_level.txt
```

### Comparing `tc_hivemind_backend-1.1.6/PKG-INFO` & `tc_hivemind_backend-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-hivemind-backend
-Version: 1.1.6
+Version: 1.2.0
 Summary: This repository is a shared library for together hivemind etl and bot codes.
 Author: Mohammad Amin Dadgar, TogetherCrew
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Requires-Dist: numpy>=1.24.1
 Requires-Dist: pytest>=7.2.0
 Requires-Dist: pytest-cov>=4.0.0
@@ -18,14 +18,16 @@
 Requires-Dist: llama-index-llms-openai==0.1.7
 Requires-Dist: llama-index-legacy
 Requires-Dist: sqlalchemy[asyncio]
 Requires-Dist: cohere<5.0.0,>=4.39
 Requires-Dist: pgvector
 Requires-Dist: asyncpg
 Requires-Dist: psycopg2-binary
+Requires-Dist: llama-index-vector-stores-qdrant==0.2.8
+Requires-Dist: qdrant-client==1.9.1
 
 # Hivemind-backend
 
 [![Maintainability](https://api.codeclimate.com/v1/badges/1f01c7faab6d09fa3a83/maintainability)](https://codeclimate.com/github/TogetherCrew/hivemind-backend/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/1f01c7faab6d09fa3a83/test_coverage)](https://codeclimate.com/github/TogetherCrew/hivemind-backend/test_coverage)
 
 This repository is designed to be a shared library for our hivemind etl sctips and bot codes.
```

### Comparing `tc_hivemind_backend-1.1.6/setup.py` & `tc_hivemind_backend-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-hivemind-backend",
-    version="1.1.6",
+    version="1.2.0",
     author="Mohammad Amin Dadgar, TogetherCrew",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="This repository is a shared library for together hivemind etl and bot codes.",
     long_description=open("README.md").read(),
     install_requires=requirements,
```

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/pg_db_utils.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/pg_db_utils.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/postgresql.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/utils/delete_data.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/utils/delete_data.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/db/utils/model_hyperparams.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/db/utils/model_hyperparams.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/embeddings/cohere.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/pg_vector_access.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/pg_vector_access.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/integration/test_delete_data.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/integration/test_delete_data.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/integration/test_pg_vector_access.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/integration/test_pg_vector_access.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/unit/test_convert_tuple_str.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/unit/test_convert_tuple_str.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/unit/test_load_db_credentials.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/unit/test_load_db_credentials.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import unittest
 
-from tc_hivemind_backend.db.credentials import load_postgres_credentials
+from tc_hivemind_backend.db.credentials import (
+    load_postgres_credentials,
+    load_qdrant_credentials,
+)
 
 
 class TestCredentialLoadings(unittest.TestCase):
     def test_postgres_envs_type(self):
         postgres_creds = load_postgres_credentials()
 
         self.assertIsInstance(postgres_creds, dict)
@@ -17,7 +20,14 @@
         self.assertNotEqual(postgres_creds["user"], None)
         self.assertNotEqual(postgres_creds["port"], None)
 
         self.assertIsInstance(postgres_creds["host"], str)
         self.assertIsInstance(postgres_creds["password"], str)
         self.assertIsInstance(postgres_creds["user"], str)
         self.assertIsInstance(postgres_creds["port"], str)
+
+    def test_load_qdrant_creds(self):
+        qdrant_creds = load_qdrant_credentials()
+
+        self.assertIsNotNone(qdrant_creds["host"])
+        self.assertIsNotNone(qdrant_creds["port"])
+        self.assertIsNotNone(qdrant_creds["api_key"])
```

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend/tests/unit/test_load_model_hyperparameters.py` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend/tests/unit/test_load_model_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend.egg-info/PKG-INFO` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-hivemind-backend
-Version: 1.1.6
+Version: 1.2.0
 Summary: This repository is a shared library for together hivemind etl and bot codes.
 Author: Mohammad Amin Dadgar, TogetherCrew
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Requires-Dist: numpy>=1.24.1
 Requires-Dist: pytest>=7.2.0
 Requires-Dist: pytest-cov>=4.0.0
@@ -18,14 +18,16 @@
 Requires-Dist: llama-index-llms-openai==0.1.7
 Requires-Dist: llama-index-legacy
 Requires-Dist: sqlalchemy[asyncio]
 Requires-Dist: cohere<5.0.0,>=4.39
 Requires-Dist: pgvector
 Requires-Dist: asyncpg
 Requires-Dist: psycopg2-binary
+Requires-Dist: llama-index-vector-stores-qdrant==0.2.8
+Requires-Dist: qdrant-client==1.9.1
 
 # Hivemind-backend
 
 [![Maintainability](https://api.codeclimate.com/v1/badges/1f01c7faab6d09fa3a83/maintainability)](https://codeclimate.com/github/TogetherCrew/hivemind-backend/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/1f01c7faab6d09fa3a83/test_coverage)](https://codeclimate.com/github/TogetherCrew/hivemind-backend/test_coverage)
 
 This repository is designed to be a shared library for our hivemind etl sctips and bot codes.
```

### Comparing `tc_hivemind_backend-1.1.6/tc_hivemind_backend.egg-info/SOURCES.txt` & `tc_hivemind_backend-1.2.0/tc_hivemind_backend.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 README.md
 setup.py
 tc_hivemind_backend/__init__.py
 tc_hivemind_backend/pg_vector_access.py
+tc_hivemind_backend/qdrant_vector_access.py
 tc_hivemind_backend.egg-info/PKG-INFO
 tc_hivemind_backend.egg-info/SOURCES.txt
 tc_hivemind_backend.egg-info/dependency_links.txt
 tc_hivemind_backend.egg-info/requires.txt
 tc_hivemind_backend.egg-info/top_level.txt
 tc_hivemind_backend/db/__init__.py
 tc_hivemind_backend/db/credentials.py
 tc_hivemind_backend/db/pg_db_utils.py
 tc_hivemind_backend/db/postgresql.py
+tc_hivemind_backend/db/qdrant.py
 tc_hivemind_backend/db/utils/__init__.py
 tc_hivemind_backend/db/utils/delete_data.py
 tc_hivemind_backend/db/utils/model_hyperparams.py
 tc_hivemind_backend/embeddings/__init__.py
 tc_hivemind_backend/embeddings/cohere.py
 tc_hivemind_backend/tests/__init__.py
 tc_hivemind_backend/tests/integration/__init__.py
 tc_hivemind_backend/tests/integration/test_delete_data.py
 tc_hivemind_backend/tests/integration/test_pg_vector_access.py
+tc_hivemind_backend/tests/integration/test_qdrant_vector_access.py
 tc_hivemind_backend/tests/unit/__init__.py
 tc_hivemind_backend/tests/unit/test_convert_tuple_str.py
 tc_hivemind_backend/tests/unit/test_load_db_credentials.py
 tc_hivemind_backend/tests/unit/test_load_model_hyperparameters.py
```


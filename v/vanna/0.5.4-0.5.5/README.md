# Comparing `tmp/vanna-0.5.4.tar.gz` & `tmp/vanna-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vanna-0.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vanna-0.5.4.tar` & `vanna-0.5.5.tar`

### file list

```diff
@@ -1,42 +1,48 @@
--rw-r--r--   0        0        0     8010 2024-05-07 14:14:04.015724 vanna-0.5.4/README.md
--rw-r--r--   0        0        0     1662 2024-05-07 14:14:04.031724 vanna-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     8725 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/ZhipuAI/ZhipuAI_Chat.py
--rw-r--r--   0        0        0     2849 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
--rw-r--r--   0        0        0      116 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/ZhipuAI/__init__.py
--rw-r--r--   0        0        0     9248 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/__init__.py
--rw-r--r--   0        0        0       43 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/anthropic/__init__.py
--rw-r--r--   0        0        0     2615 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/anthropic/anthropic_chat.py
--rw-r--r--   0        0        0       28 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/base/__init__.py
--rw-r--r--   0        0        0    70850 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/base/base.py
--rw-r--r--   0        0        0       50 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/chromadb/__init__.py
--rw-r--r--   0        0        0     8792 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/chromadb/chromadb_vector.py
--rw-r--r--   0        0        0      685 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/exceptions/__init__.py
--rw-r--r--   0        0        0    25192 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/flask/__init__.py
--rw-r--r--   0        0        0   187711 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/flask/assets.py
--rw-r--r--   0        0        0     1246 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/flask/auth.py
--rw-r--r--   0        0        0       41 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/google/__init__.py
--rw-r--r--   0        0        0     1584 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/google/gemini_chat.py
--rw-r--r--   0        0        0       19 2024-05-07 14:14:04.031724 vanna-0.5.4/src/vanna/hf/__init__.py
--rw-r--r--   0        0        0     2703 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/hf/hf.py
--rw-r--r--   0        0        0      313 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/local.py
--rw-r--r--   0        0        0       37 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/marqo/__init__.py
--rw-r--r--   0        0        0     5242 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/marqo/marqo.py
--rw-r--r--   0        0        0       29 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/mistral/__init__.py
--rw-r--r--   0        0        0     1508 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/mistral/mistral.py
--rw-r--r--   0        0        0       27 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/ollama/__init__.py
--rw-r--r--   0        0        0     3794 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/ollama/ollama.py
--rw-r--r--   0        0        0       86 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/openai/__init__.py
--rw-r--r--   0        0        0     4764 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/openai/openai_chat.py
--rw-r--r--   0        0        0     1260 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/openai/openai_embeddings.py
--rw-r--r--   0        0        0       54 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/opensearch/__init__.py
--rw-r--r--   0        0        0    11980 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/opensearch/opensearch_vector.py
--rw-r--r--   0        0        0       73 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/qdrant/__init__.py
--rw-r--r--   0        0        0    12613 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/qdrant/qdrant.py
--rw-r--r--   0        0        0     1856 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/remote.py
--rw-r--r--   0        0        0     4957 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/types/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/utils.py
--rw-r--r--   0        0        0       48 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/vannadb/__init__.py
--rw-r--r--   0        0        0     6168 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/vannadb/vannadb_vector.py
--rw-r--r--   0        0        0       23 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/vllm/__init__.py
--rw-r--r--   0        0        0     2427 2024-05-07 14:14:04.035724 vanna-0.5.4/src/vanna/vllm/vllm.py
--rw-r--r--   0        0        0    11332 1970-01-01 00:00:00.000000 vanna-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     8010 2024-05-20 14:43:14.951615 vanna-0.5.5/README.md
+-rw-r--r--   0        0        0     1725 2024-05-20 14:43:14.967615 vanna-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     8725 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/ZhipuAI/ZhipuAI_Chat.py
+-rw-r--r--   0        0        0     2849 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
+-rw-r--r--   0        0        0      116 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/ZhipuAI/__init__.py
+-rw-r--r--   0        0        0     9248 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/anthropic/__init__.py
+-rw-r--r--   0        0        0     2615 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/anthropic/anthropic_chat.py
+-rw-r--r--   0        0        0       28 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/base/__init__.py
+-rw-r--r--   0        0        0    70853 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/base/base.py
+-rw-r--r--   0        0        0       50 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/chromadb/__init__.py
+-rw-r--r--   0        0        0     8792 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/chromadb/chromadb_vector.py
+-rw-r--r--   0        0        0      685 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/exceptions/__init__.py
+-rw-r--r--   0        0        0    25192 2024-05-20 14:43:14.967615 vanna-0.5.5/src/vanna/flask/__init__.py
+-rw-r--r--   0        0        0   187711 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/flask/assets.py
+-rw-r--r--   0        0        0     1246 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/flask/auth.py
+-rw-r--r--   0        0        0       41 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/google/__init__.py
+-rw-r--r--   0        0        0     1584 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/google/gemini_chat.py
+-rw-r--r--   0        0        0       19 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/hf/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/hf/hf.py
+-rw-r--r--   0        0        0      313 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/local.py
+-rw-r--r--   0        0        0       37 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/marqo/__init__.py
+-rw-r--r--   0        0        0     5242 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/marqo/marqo.py
+-rw-r--r--   0        0        0       29 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/mistral/__init__.py
+-rw-r--r--   0        0        0     1508 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/mistral/mistral.py
+-rw-r--r--   0        0        0       97 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/mock/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/mock/embedding.py
+-rw-r--r--   0        0        0      518 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/mock/llm.py
+-rw-r--r--   0        0        0     2681 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/mock/vectordb.py
+-rw-r--r--   0        0        0       27 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/ollama/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/ollama/ollama.py
+-rw-r--r--   0        0        0       86 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/openai/__init__.py
+-rw-r--r--   0        0        0     4764 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/openai/openai_chat.py
+-rw-r--r--   0        0        0     1260 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/openai/openai_embeddings.py
+-rw-r--r--   0        0        0       54 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/opensearch/__init__.py
+-rw-r--r--   0        0        0    12226 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/opensearch/opensearch_vector.py
+-rw-r--r--   0        0        0       90 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/pinecone/__init__.py
+-rw-r--r--   0        0        0    11448 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/pinecone/pinecone_vector.py
+-rw-r--r--   0        0        0       73 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/qdrant/__init__.py
+-rw-r--r--   0        0        0    12613 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/qdrant/qdrant.py
+-rw-r--r--   0        0        0     1856 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/remote.py
+-rw-r--r--   0        0        0     4957 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/types/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/utils.py
+-rw-r--r--   0        0        0       48 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/vannadb/__init__.py
+-rw-r--r--   0        0        0     6168 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/vannadb/vannadb_vector.py
+-rw-r--r--   0        0        0       23 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/vllm/__init__.py
+-rw-r--r--   0        0        0     2427 2024-05-20 14:43:14.971615 vanna-0.5.5/src/vanna/vllm/vllm.py
+-rw-r--r--   0        0        0    11505 1970-01-01 00:00:00.000000 vanna-0.5.5/PKG-INFO
```

### Comparing `vanna-0.5.4/README.md` & `vanna-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/pyproject.toml` & `vanna-0.5.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vanna"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -29,21 +29,22 @@
 postgres = ["psycopg2-binary", "db-dtypes"]
 mysql = ["PyMySQL"]
 clickhouse = ["clickhouse_driver"]
 bigquery = ["google-cloud-bigquery"]
 snowflake = ["snowflake-connector-python"]
 duckdb = ["duckdb"]
 google = ["google-generativeai", "google-cloud-aiplatform"]
-all = ["psycopg2-binary", "db-dtypes", "PyMySQL", "google-cloud-bigquery", "snowflake-connector-python", "duckdb", "openai", "mistralai", "chromadb", "anthropic", "zhipuai", "marqo", "google-generativeai", "google-cloud-aiplatform", "qdrant-client", "fastembed", "ollama", "httpx", "opensearch-py", "opensearch-dsl", "transformers"]
+all = ["psycopg2-binary", "db-dtypes", "PyMySQL", "google-cloud-bigquery", "snowflake-connector-python", "duckdb", "openai", "mistralai", "chromadb", "anthropic", "zhipuai", "marqo", "google-generativeai", "google-cloud-aiplatform", "qdrant-client", "fastembed", "ollama", "httpx", "opensearch-py", "opensearch-dsl", "transformers", "pinecone-client"]
 test = ["tox"]
 chromadb = ["chromadb"]
 openai = ["openai"]
 mistralai = ["mistralai"]
 anthropic = ["anthropic"]
 gemini = ["google-generativeai"]
 marqo = ["marqo"]
 zhipuai = ["zhipuai"]
 ollama = ["ollama", "httpx"]
 qdrant = ["qdrant-client", "fastembed"]
 vllm = ["vllm"]
+pinecone = ["pinecone-client", "fastembed"]
 opensearch = ["opensearch-py", "opensearch-dsl"]
 hf = ["transformers"]
```

### Comparing `vanna-0.5.4/src/vanna/ZhipuAI/ZhipuAI_Chat.py` & `vanna-0.5.5/src/vanna/ZhipuAI/ZhipuAI_Chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/ZhipuAI/ZhipuAI_embeddings.py` & `vanna-0.5.5/src/vanna/ZhipuAI/ZhipuAI_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/__init__.py` & `vanna-0.5.5/src/vanna/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/anthropic/anthropic_chat.py` & `vanna-0.5.5/src/vanna/anthropic/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/base/base.py` & `vanna-0.5.5/src/vanna/base/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,15 @@
             doc_list (list): A list of documentation.
 
         Returns:
             any: The prompt for the LLM to generate SQL.
         """
 
         if initial_prompt is None:
-            initial_prompt = f"You are a {self.dialect} expert. "
+            initial_prompt = f"You are a {self.dialect} expert. " + \
             "Please help to generate a SQL query to answer the question. Your response should ONLY be based on the given context and follow the response guidelines and format instructions. "
 
         initial_prompt = self.add_ddl_to_prompt(
             initial_prompt, ddl_list, max_tokens=14000
         )
 
         if self.static_documentation != "":
@@ -1697,15 +1697,15 @@
 
         except Exception as e:
             print("Couldn't run sql: ", e)
             if print_results:
                 return None
             else:
                 return sql, None, None
-        return sql, df, None
+        return sql, df, fig
 
     def train(
         self,
         question: str = None,
         sql: str = None,
         ddl: str = None,
         documentation: str = None,
```

### Comparing `vanna-0.5.4/src/vanna/chromadb/chromadb_vector.py` & `vanna-0.5.5/src/vanna/chromadb/chromadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/exceptions/__init__.py` & `vanna-0.5.5/src/vanna/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/flask/__init__.py` & `vanna-0.5.5/src/vanna/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/flask/assets.py` & `vanna-0.5.5/src/vanna/flask/assets.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/flask/auth.py` & `vanna-0.5.5/src/vanna/flask/auth.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/google/gemini_chat.py` & `vanna-0.5.5/src/vanna/google/gemini_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/hf/hf.py` & `vanna-0.5.5/src/vanna/hf/hf.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/marqo/marqo.py` & `vanna-0.5.5/src/vanna/marqo/marqo.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/mistral/mistral.py` & `vanna-0.5.5/src/vanna/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/ollama/ollama.py` & `vanna-0.5.5/src/vanna/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/openai/openai_chat.py` & `vanna-0.5.5/src/vanna/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/openai/openai_embeddings.py` & `vanna-0.5.5/src/vanna/openai/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/opensearch/opensearch_vector.py` & `vanna-0.5.5/src/vanna/opensearch/opensearch_vector.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,35 +151,40 @@
       timeout = 60
 
     if config is not None and "es_max_retries" in config:
       max_retries = config["es_max_retries"]
     else:
       max_retries = 10
 
+    if config is not None and "es_http_compress" in config:
+      es_http_compress = config["es_http_compress"]
+    else:
+      es_http_compress = False
+
     print("OpenSearch_VectorStore initialized with es_urls: ", es_urls,
           " host: ", host, " port: ", port, " ssl: ", ssl, " verify_certs: ",
           verify_certs, " timeout: ", timeout, " max_retries: ", max_retries)
     if es_urls is not None:
       # Initialize the OpenSearch client by passing a list of URLs
       self.client = OpenSearch(
         hosts=[es_urls],
-        http_compress=True,
+        http_compress=es_http_compress,
         use_ssl=ssl,
         verify_certs=verify_certs,
         timeout=timeout,
         max_retries=max_retries,
         retry_on_timeout=True,
         http_auth=auth,
         headers=headers
       )
     else:
       # Initialize the OpenSearch client by passing a host and port
       self.client = OpenSearch(
         hosts=[{'host': host, 'port': port}],
-        http_compress=True,
+        http_compress=es_http_compress,
         use_ssl=ssl,
         verify_certs=verify_certs,
         timeout=timeout,
         max_retries=max_retries,
         retry_on_timeout=True,
         http_auth=auth,
         headers=headers
@@ -263,39 +268,42 @@
     query = {
       "query": {
         "match": {
           "ddl": question
         }
       }
     }
+    print(query)
     response = self.client.search(index=self.ddl_index, body=query,
                                   **kwargs)
     return [hit['_source']['ddl'] for hit in response['hits']['hits']]
 
   def get_related_documentation(self, question: str, **kwargs) -> List[str]:
     query = {
       "query": {
         "match": {
           "doc": question
         }
       }
     }
+    print(query)
     response = self.client.search(index=self.document_index,
                                   body=query,
                                   **kwargs)
     return [hit['_source']['doc'] for hit in response['hits']['hits']]
 
   def get_similar_question_sql(self, question: str, **kwargs) -> List[str]:
     query = {
       "query": {
         "match": {
           "question": question
         }
       }
     }
+    print(query)
     response = self.client.search(index=self.question_sql_index,
                                   body=query,
                                   **kwargs)
     return [(hit['_source']['question'], hit['_source']['sql']) for hit in
             response['hits']['hits']]
 
   def get_training_data(self, **kwargs) -> pd.DataFrame:
@@ -303,14 +311,15 @@
     # WARNING: Do not use this approach in production for large indices!
     data = []
     response = self.client.search(
       index=self.document_index,
       body={"query": {"match_all": {}}},
       size=1000
     )
+    print(query)
     # records = [hit['_source'] for hit in response['hits']['hits']]
     for hit in response['hits']['hits']:
       data.append(
         {
           "id": hit["_id"],
           "training_data_type": "documentation",
           "question": "",
```

### Comparing `vanna-0.5.4/src/vanna/qdrant/qdrant.py` & `vanna-0.5.5/src/vanna/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/remote.py` & `vanna-0.5.5/src/vanna/remote.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/types/__init__.py` & `vanna-0.5.5/src/vanna/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/utils.py` & `vanna-0.5.5/src/vanna/utils.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/vannadb/vannadb_vector.py` & `vanna-0.5.5/src/vanna/vannadb/vannadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/src/vanna/vllm/vllm.py` & `vanna-0.5.5/src/vanna/vllm/vllm.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.4/PKG-INFO` & `vanna-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.5.4
+Version: 0.5.5
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,14 +34,15 @@
 Requires-Dist: qdrant-client ; extra == "all"
 Requires-Dist: fastembed ; extra == "all"
 Requires-Dist: ollama ; extra == "all"
 Requires-Dist: httpx ; extra == "all"
 Requires-Dist: opensearch-py ; extra == "all"
 Requires-Dist: opensearch-dsl ; extra == "all"
 Requires-Dist: transformers ; extra == "all"
+Requires-Dist: pinecone-client ; extra == "all"
 Requires-Dist: anthropic ; extra == "anthropic"
 Requires-Dist: google-cloud-bigquery ; extra == "bigquery"
 Requires-Dist: chromadb ; extra == "chromadb"
 Requires-Dist: clickhouse_driver ; extra == "clickhouse"
 Requires-Dist: duckdb ; extra == "duckdb"
 Requires-Dist: google-generativeai ; extra == "gemini"
 Requires-Dist: google-generativeai ; extra == "google"
@@ -51,14 +52,16 @@
 Requires-Dist: mistralai ; extra == "mistralai"
 Requires-Dist: PyMySQL ; extra == "mysql"
 Requires-Dist: ollama ; extra == "ollama"
 Requires-Dist: httpx ; extra == "ollama"
 Requires-Dist: openai ; extra == "openai"
 Requires-Dist: opensearch-py ; extra == "opensearch"
 Requires-Dist: opensearch-dsl ; extra == "opensearch"
+Requires-Dist: pinecone-client ; extra == "pinecone"
+Requires-Dist: fastembed ; extra == "pinecone"
 Requires-Dist: psycopg2-binary ; extra == "postgres"
 Requires-Dist: db-dtypes ; extra == "postgres"
 Requires-Dist: qdrant-client ; extra == "qdrant"
 Requires-Dist: fastembed ; extra == "qdrant"
 Requires-Dist: snowflake-connector-python ; extra == "snowflake"
 Requires-Dist: tox ; extra == "test"
 Requires-Dist: vllm ; extra == "vllm"
@@ -76,14 +79,15 @@
 Provides-Extra: hf
 Provides-Extra: marqo
 Provides-Extra: mistralai
 Provides-Extra: mysql
 Provides-Extra: ollama
 Provides-Extra: openai
 Provides-Extra: opensearch
+Provides-Extra: pinecone
 Provides-Extra: postgres
 Provides-Extra: qdrant
 Provides-Extra: snowflake
 Provides-Extra: test
 Provides-Extra: vllm
 Provides-Extra: zhipuai
```


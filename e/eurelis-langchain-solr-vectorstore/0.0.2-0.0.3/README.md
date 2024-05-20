# Comparing `tmp/eurelis_langchain_solr_vectorstore-0.0.2.tar.gz` & `tmp/eurelis_langchain_solr_vectorstore-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurelis_langchain_solr_vectorstore-0.0.2.tar", last modified: Sun May  5 08:59:19 2024, max compression
+gzip compressed data, was "eurelis_langchain_solr_vectorstore-0.0.3.tar", last modified: Mon May 20 17:56:27 2024, max compression
```

## Comparing `eurelis_langchain_solr_vectorstore-0.0.2.tar` & `eurelis_langchain_solr_vectorstore-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-05 08:59:19.977434 eurelis_langchain_solr_vectorstore-0.0.2/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     1064 2023-10-29 17:22:12.000000 eurelis_langchain_solr_vectorstore-0.0.2/LICENSE
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3403 2024-05-05 08:59:19.976963 eurelis_langchain_solr_vectorstore-0.0.2/PKG-INFO
--rw-r--r--   0 vincentlambert   (501) staff       (20)     2752 2024-05-05 08:53:51.000000 eurelis_langchain_solr_vectorstore-0.0.2/README.md
--rw-r--r--   0 vincentlambert   (501) staff       (20)      791 2024-05-05 08:53:51.000000 eurelis_langchain_solr_vectorstore-0.0.2/pyproject.toml
--rw-r--r--   0 vincentlambert   (501) staff       (20)       38 2024-05-05 08:59:19.977611 eurelis_langchain_solr_vectorstore-0.0.2/setup.cfg
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-05 08:59:19.967993 eurelis_langchain_solr_vectorstore-0.0.2/src/
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-05 08:59:19.973131 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/
--rw-r--r--   0 vincentlambert   (501) staff       (20)    16382 2024-05-05 08:53:51.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/__init__.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     9877 2024-05-05 08:53:51.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/solr_core.py
--rw-r--r--   0 vincentlambert   (501) staff       (20)     5079 2023-10-29 17:22:12.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/types.py
-drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-05 08:59:19.976499 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/
--rw-r--r--   0 vincentlambert   (501) staff       (20)     3403 2024-05-05 08:59:19.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/PKG-INFO
--rw-r--r--   0 vincentlambert   (501) staff       (20)      431 2024-05-05 08:59:19.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/SOURCES.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)        1 2024-05-05 08:59:19.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/dependency_links.txt
--rw-r--r--   0 vincentlambert   (501) staff       (20)       35 2024-05-05 08:59:19.000000 eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/top_level.txt
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-20 17:56:27.500733 eurelis_langchain_solr_vectorstore-0.0.3/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     1064 2023-10-29 17:22:12.000000 eurelis_langchain_solr_vectorstore-0.0.3/LICENSE
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3490 2024-05-20 17:56:27.499764 eurelis_langchain_solr_vectorstore-0.0.3/PKG-INFO
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     2839 2024-05-20 17:54:10.000000 eurelis_langchain_solr_vectorstore-0.0.3/README.md
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      791 2024-05-20 17:54:10.000000 eurelis_langchain_solr_vectorstore-0.0.3/pyproject.toml
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       38 2024-05-20 17:56:27.500933 eurelis_langchain_solr_vectorstore-0.0.3/setup.cfg
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-20 17:56:27.484741 eurelis_langchain_solr_vectorstore-0.0.3/src/
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-20 17:56:27.491750 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)    16480 2024-05-20 17:54:10.000000 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore/__init__.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)    10083 2024-05-20 17:54:10.000000 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore/solr_core.py
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     5079 2023-10-29 17:22:12.000000 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore/types.py
+drwxr-xr-x   0 vincentlambert   (501) staff       (20)        0 2024-05-20 17:56:27.498696 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore.egg-info/
+-rw-r--r--   0 vincentlambert   (501) staff       (20)     3490 2024-05-20 17:56:27.000000 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore.egg-info/PKG-INFO
+-rw-r--r--   0 vincentlambert   (501) staff       (20)      431 2024-05-20 17:56:27.000000 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore.egg-info/SOURCES.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)        1 2024-05-20 17:56:27.000000 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore.egg-info/dependency_links.txt
+-rw-r--r--   0 vincentlambert   (501) staff       (20)       35 2024-05-20 17:56:27.000000 eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore.egg-info/top_level.txt
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.2/LICENSE` & `eurelis_langchain_solr_vectorstore-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eurelis_langchain_solr_vectorstore-0.0.2/PKG-INFO` & `eurelis_langchain_solr_vectorstore-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurelis_langchain_solr_vectorstore
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library that provide a Solr based vector store for Langchain
 Author-email: Jérôme DIAZ <j.diaz@eurelis.com>, Vincent LAMBERT <v.lambert@eurelis.com>
 Project-URL: Homepage, https://github.com/Eurelis/Eurelis-Langchain-SolR-VectorStore
 Project-URL: Bug Tracker, https://github.com/Eurelis/Eurelis-Langchain-SolR-VectorStore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,16 @@
 ```python
 vector_store = Solr(embeddings, core_kwargs={
     'page_content_field': 'text_t',  # field containing the text content
     'vector_field': 'vector',        # field containing the embeddings of the text content
     'core_name': 'langchain',        # core name
     'url_base': 'http://localhost:8983/solr', # base url to access solr
     'query_handler': 'select', # handler to use to query solr
-    'update_handler': 'update' # update handler for solr
+    'update_handler': 'update', # update handler for solr
+    'metadata_fields': [] # additional solr fields to consider as metadata, ie ['id']
 })  # with custom default core configuration
 ```
 
 In the code above you have both the allowed core arguments and the default value.
 
 ### Metadata
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.2/README.md` & `eurelis_langchain_solr_vectorstore-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 ```python
 vector_store = Solr(embeddings, core_kwargs={
     'page_content_field': 'text_t',  # field containing the text content
     'vector_field': 'vector',        # field containing the embeddings of the text content
     'core_name': 'langchain',        # core name
     'url_base': 'http://localhost:8983/solr', # base url to access solr
     'query_handler': 'select', # handler to use to query solr
-    'update_handler': 'update' # update handler for solr
+    'update_handler': 'update', # update handler for solr
+    'metadata_fields': [] # additional solr fields to consider as metadata, ie ['id']
 })  # with custom default core configuration
 ```
 
 In the code above you have both the allowed core arguments and the default value.
 
 ### Metadata
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.2/pyproject.toml` & `eurelis_langchain_solr_vectorstore-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eurelis_langchain_solr_vectorstore"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jérôme DIAZ", email="j.diaz@eurelis.com" },
   { name="Vincent LAMBERT", email="v.lambert@eurelis.com" }
 ]
 description = "Library that provide a Solr based vector store for Langchain"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/__init__.py` & `eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             core_kwargs={
                 'page_content_field': 'text_t', # name of the solr to store the page content in
                 'vector_field: 'vector', # name of the solr field to store the vector in
                 'core_name': 'langchain', # name of the solr core
                 'url_base': 'http://localhost:8983/solr' # base url to access solr
                 'query_handler': 'select' # select handler to query solr
                 'update_handler': 'update' # update handler to query solr
+                'metadata_fields': [] # additional solr fields to consider as metadata, ie ['id']
             }
         )
     Args:
         embedding_function: Embeddings instance,
         core_kwargs: arguments to construct the solr core handler
     """
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/solr_core.py` & `eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore/solr_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     def __init__(self, **kwargs):
         self._page_content_field = kwargs.get("page_content_field", "text_t")
         self._vector_field = kwargs.get("vector_field", "vector")
         self._core_name = kwargs.get("core_name", "langchain")
         self._url_base = kwargs.get("url_base", "http://localhost:8983/solr")
         self._query_handler = kwargs.get("query_handler", "select")
         self._update_handler = kwargs.get("update_handler", "update")
+        self._metadata_fields = set(kwargs.get("metadata_fields", []))
 
     def get_handler_url(self, handler: str):
         return f"{self._url_base}/{self._core_name}/{handler}"
 
     @staticmethod
     def metadata_to_solr_fields(
         metadata: Mapping[str, str | int | float | bool]
@@ -142,14 +143,18 @@
 
         for doc in data_json["response"]["docs"]:
             page_content = doc.get(self._page_content_field)
             results_documents.append(page_content)
 
             metadata = {}
             for solr_field, value in doc.items():
+                if solr_field in self._metadata_fields:
+                    metadata[solr_field] = value
+                    continue
+
                 metadata_key = SolrCore.metadata_key_for_field_name(solr_field)
                 if not metadata_key or not isinstance(value, (str, int, float, bool)):
                     continue
                 metadata[metadata_key] = value
 
             results_metadatas.append(metadata)
             results_distances.append(doc.get("score", 0))
```

### Comparing `eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore/types.py` & `eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore/types.py`

 * *Files identical despite different names*

### Comparing `eurelis_langchain_solr_vectorstore-0.0.2/src/eurelis_langchain_solr_vectorstore.egg-info/PKG-INFO` & `eurelis_langchain_solr_vectorstore-0.0.3/src/eurelis_langchain_solr_vectorstore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurelis_langchain_solr_vectorstore
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library that provide a Solr based vector store for Langchain
 Author-email: Jérôme DIAZ <j.diaz@eurelis.com>, Vincent LAMBERT <v.lambert@eurelis.com>
 Project-URL: Homepage, https://github.com/Eurelis/Eurelis-Langchain-SolR-VectorStore
 Project-URL: Bug Tracker, https://github.com/Eurelis/Eurelis-Langchain-SolR-VectorStore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,16 @@
 ```python
 vector_store = Solr(embeddings, core_kwargs={
     'page_content_field': 'text_t',  # field containing the text content
     'vector_field': 'vector',        # field containing the embeddings of the text content
     'core_name': 'langchain',        # core name
     'url_base': 'http://localhost:8983/solr', # base url to access solr
     'query_handler': 'select', # handler to use to query solr
-    'update_handler': 'update' # update handler for solr
+    'update_handler': 'update', # update handler for solr
+    'metadata_fields': [] # additional solr fields to consider as metadata, ie ['id']
 })  # with custom default core configuration
 ```
 
 In the code above you have both the allowed core arguments and the default value.
 
 ### Metadata
```


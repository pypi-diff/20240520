# Comparing `tmp/memvectordb_python-0.0.2.tar.gz` & `tmp/memvectordb_python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memvectordb_python-0.0.2.tar", max compression
+gzip compressed data, was "memvectordb_python-0.0.3.tar", max compression
```

## Comparing `memvectordb_python-0.0.2.tar` & `memvectordb_python-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2164 2024-05-17 13:49:55.624854 memvectordb_python-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-17 13:49:55.624854 memvectordb_python-0.0.2/memvectordb/__init__.py
--rw-r--r--   0        0        0     7325 2024-05-17 13:49:55.624854 memvectordb_python-0.0.2/memvectordb/collection.py
--rw-r--r--   0        0        0      445 2024-05-17 13:49:55.624854 memvectordb_python-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3198 1970-01-01 00:00:00.000000 memvectordb_python-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2042 2024-05-20 07:46:07.387898 memvectordb_python-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:46:07.387898 memvectordb_python-0.0.3/memvectordb/__init__.py
+-rw-r--r--   0        0        0     8103 2024-05-20 07:46:07.387898 memvectordb_python-0.0.3/memvectordb/collection.py
+-rw-r--r--   0        0        0      445 2024-05-20 07:46:07.387898 memvectordb_python-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 memvectordb_python-0.0.3/PKG-INFO
```

### Comparing `memvectordb_python-0.0.2/README.md` & `memvectordb_python-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -79,26 +79,23 @@
         "metadata": {
             "key1": "value3",
             "key2": "value4"
         }
     }
 ]
 
-for embedding in embeddings:
-    client.batch_insert_embeddings(
+client.batch_insert_embeddings(
         collection_name=collection_name, 
-        vector_id=embedding["id"], 
-        vector=embedding["vector"], 
-        metadata=embedding["metadata"]
+        embeddings = embeddings
     )
 ```
 ## To Query Vectors.
 
 ```python
 k = "number-of-items-to query"
 collection_name = "collection_name"
 query_vector = "query_vector"
 
 # example of query_vector: [0.32654, 0.24423, 0.7655] 
 # ensure the dimensions match the collection's dimensions
-client.get_similarity(collection_name, k, query_vector)
+client.query(collection_name, k, query_vector)
 ```
```

### Comparing `memvectordb_python-0.0.2/memvectordb/collection.py` & `memvectordb_python-0.0.3/memvectordb/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,41 +133,57 @@
             return response_data
         else:
             raise Exception(f"Failed to insert embedding: {response.status_code}")
         
     def batch_insert_embeddings(
         self, 
         collection_name: str, 
-        vector_id: int,
-        vector: List[float],
-        metadata: Optional[List[Dict]] = None
+        embeddings: List[Dict[str, Any]]
     ) -> str:
         """
-        This method inserts a batch of embeddings into a specified collection.
+        Insert a batch of embeddings into a specified collection.
 
         Args:
             collection_name (str): The name of the collection to insert the embeddings into.
-            vector_id (int): The unique identifier for the vector.
-            vector (List[float]): The vector to be inserted.
-            metadata (Optional[List[Dict]]): Additional metadata associated with the vector.
+            embeddings (List[Dict[str, Any]]): List of dictionaries representing embeddings. 
+                Each dictionary should contain keys 'id' (int), 'vector' (List[float]), 
+                and optional 'metadata' (List[Dict[str, Any]]).
+        example: 
+                {
+                    "collection_name" : "test_collection_name",
+                    "embeddings" :
+                            [
+                            {
+                                "id": "1",
+                                "vector": [0.14, 0.316, 0.433],
+                                "metadata": {
+                                    "key1": "value1",
+                                    "key2": "value2"
+                                }
+                            },
+                            {
+                                "id": "2",
+                                "vector": [0.27, 0.531, 0.621],
+                                "metadata": {
+                                    "key1": "value3",
+                                    "key2": "value4"
+                                }
+                            }
+                        ]
+                }
 
         Returns:
-            str: Status of the insertion operation.
+            str: Status message indicating the success of the insertion operation.
         """
-        embeddings = {
-            "id": str(vector_id),
-            "vector": vector,
-            "metadata": metadata
-        }
         payload = {
             "collection_name": collection_name,
-            "embeddings": [embeddings]
+            "embeddings": embeddings
         }
         headers = {"Content-Type": "application/json"}
-        url = f"{self.base_url}/update_collection"
+        url = f"{self.base_url}/batch_insert_embeddings"
         response = requests.post(url, json=payload, headers=headers)
         response_data = response.json()
         if response.status_code == 200:
             return response_data
         else:
             raise Exception(f"Failed to insert embedding: {response_data}")
```

### Comparing `memvectordb_python-0.0.2/PKG-INFO` & `memvectordb_python-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memvectordb-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: memvectordb python client.
 Home-page: https://github.com/KevKibe/memvectordb-python-client
 License: MIT
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
@@ -104,27 +104,24 @@
         "metadata": {
             "key1": "value3",
             "key2": "value4"
         }
     }
 ]
 
-for embedding in embeddings:
-    client.batch_insert_embeddings(
+client.batch_insert_embeddings(
         collection_name=collection_name, 
-        vector_id=embedding["id"], 
-        vector=embedding["vector"], 
-        metadata=embedding["metadata"]
+        embeddings = embeddings
     )
 ```
 ## To Query Vectors.
 
 ```python
 k = "number-of-items-to query"
 collection_name = "collection_name"
 query_vector = "query_vector"
 
 # example of query_vector: [0.32654, 0.24423, 0.7655] 
 # ensure the dimensions match the collection's dimensions
-client.get_similarity(collection_name, k, query_vector)
+client.query(collection_name, k, query_vector)
 ```
```


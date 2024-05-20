# Comparing `tmp/docmesh_core-0.0.5.tar.gz` & `tmp/docmesh_core-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_core-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_core-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_core-0.0.5.tar` & `docmesh_core-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.5/README.md
--rw-r--r--   0        0        0       22 2024-05-17 06:23:16.598358 docmesh_core-0.0.5/docmesh_core/__init__.py
--rw-r--r--   0        0        0     1244 2024-05-15 11:01:49.702507 docmesh_core-0.0.5/docmesh_core/db/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.5/docmesh_core/db/auth.py
--rw-r--r--   0        0        0    10901 2024-05-16 11:05:05.685045 docmesh_core-0.0.5/docmesh_core/db/neo.py
--rw-r--r--   0        0        0      417 2024-05-15 10:24:49.939048 docmesh_core-0.0.5/docmesh_core/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.5/docmesh_core/utils/graph_utils.py
--rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.5/docmesh_core/utils/semantic_scholar.py
--rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.6/README.md
+-rw-r--r--   0        0        0       22 2024-05-20 07:43:11.239920 docmesh_core-0.0.6/docmesh_core/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-20 07:41:31.413472 docmesh_core-0.0.6/docmesh_core/db/__init__.py
+-rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.6/docmesh_core/db/auth.py
+-rw-r--r--   0        0        0    11864 2024-05-20 05:24:06.535535 docmesh_core-0.0.6/docmesh_core/db/neo.py
+-rw-r--r--   0        0        0      417 2024-05-15 10:24:49.939048 docmesh_core-0.0.6/docmesh_core/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.6/docmesh_core/utils/graph_utils.py
+-rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.6/docmesh_core/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.6/PKG-INFO
```

### Comparing `docmesh_core-0.0.5/docmesh_core/db/__init__.py` & `docmesh_core-0.0.6/docmesh_core/db/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     list_latest_papers,
     list_unread_similar_papers,
     list_unread_semantic_papers,
     list_unread_follows_papers,
     list_unread_influential_papers,
     list_unembedded_papers,
     get_latest_citegraph,
+    get_collection,
+    add_collection,
+    add_paper_to_collection,
 )
 from .auth import (
     add_auth_for_entity,
     get_auth_from_entity,
     get_entity_from_auth,
 )
 
@@ -45,11 +48,14 @@
     "list_latest_papers",
     "list_unread_similar_papers",
     "list_unread_semantic_papers",
     "list_unread_follows_papers",
     "list_unread_influential_papers",
     "list_unembedded_papers",
     "get_latest_citegraph",
+    "get_collection",
+    "add_collection",
+    "add_paper_to_collection",
     "add_auth_for_entity",
     "get_auth_from_entity",
     "get_entity_from_auth",
 ]
```

### Comparing `docmesh_core-0.0.5/docmesh_core/db/auth.py` & `docmesh_core-0.0.6/docmesh_core/db/auth.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.5/docmesh_core/db/neo.py` & `docmesh_core-0.0.6/docmesh_core/db/neo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import pandas as pd
 
 from typing import Any
 from pandas.core.frame import DataFrame
 
 from neomodel import db
 from neomodel import (
@@ -78,14 +77,27 @@
             "reference_count": self.reference_count,
             "citation_count": self.citation_count,
             "pdf": self.pdf,
         }
         return data
 
 
+class Collection(StructuredNode):
+    name = StringProperty(unique_index=True)
+
+    papers = RelationshipTo("Paper", "contain")
+
+
+class Venue(StructuredNode):
+    name = StringProperty(unique_index=True)
+
+    collections = RelationshipTo("Collection", "publish")
+
+
+
 def _nodelist_to_dataframe(nodes: list[StructuredNode]) -> DataFrame:
     df = pd.DataFrame.from_dict([node.serialize for node in nodes])
     return df
 
 
 def get_entity(entity_name: str) -> Entity:
     entity = Entity.nodes.get(name=entity_name)
@@ -383,7 +395,28 @@
                 "entity_name": entity_name,
                 "n": n,
             },
         )
     )
 
     return df
+
+
+def get_collection(collection_name: str) -> Collection:
+    collection = Collection.nodes.get(name=collection_name)
+    return collection
+
+
+@db.transaction
+def add_collection(collection_name: str) -> Collection:
+    collection: Collection = Collection.create_or_update({"name": collection_name})
+    return collection
+
+
+@db.transaction
+def add_paper_to_collection(paper_id: str, collection_name: str) -> None:
+    paper: Paper = get_paper_from_id(paper_id)
+    collection: Collection = get_collection(collection_name)
+    # XXX: neomodel says that they can ensure relationship uniqueness
+    # however, it doesn't
+    if not collection.papers.is_connected(paper):
+        collection.papers.connect(paper)
```

### Comparing `docmesh_core-0.0.5/docmesh_core/utils/semantic_scholar.py` & `docmesh_core-0.0.6/docmesh_core/utils/semantic_scholar.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.5/pyproject.toml` & `docmesh_core-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.5/PKG-INFO` & `docmesh_core-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh_core
-Version: 0.0.5
+Version: 0.0.6
 Summary: Core components for docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


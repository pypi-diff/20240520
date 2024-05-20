# Comparing `tmp/pycgs-1.0.0.tar.gz` & `tmp/pycgs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycgs-1.0.0.tar", max compression
+gzip compressed data, was "pycgs-1.0.1.tar", max compression
```

## Comparing `pycgs-1.0.0.tar` & `pycgs-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-12-20 13:38:05.351111 pycgs-1.0.0/LICENSE
--rw-r--r--   0        0        0     1281 2023-12-28 06:37:07.966381 pycgs-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-12-28 06:21:20.171976 pycgs-1.0.0/pycgs/__init__.py
--rw-r--r--   0        0        0     2800 2023-12-28 06:36:48.919673 pycgs-1.0.0/pycgs/cgs.py
--rw-r--r--   0        0        0      158 2023-12-28 06:21:18.689937 pycgs-1.0.0/pycgs/type.py
--rw-r--r--   0        0        0      631 2023-12-28 10:39:59.103439 pycgs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 pycgs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-20 13:38:05.351111 pycgs-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1831 2024-05-20 13:14:47.762406 pycgs-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-12-28 06:21:20.171976 pycgs-1.0.1/pycgs/__init__.py
+-rw-r--r--   0        0        0     3062 2024-05-20 13:00:11.369246 pycgs-1.0.1/pycgs/cgs.py
+-rw-r--r--   0        0        0      158 2023-12-28 06:21:18.689937 pycgs-1.0.1/pycgs/type.py
+-rw-r--r--   0        0        0      630 2024-05-20 12:41:52.701775 pycgs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 pycgs-1.0.1/PKG-INFO
```

### Comparing `pycgs-1.0.0/LICENSE` & `pycgs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycgs-1.0.0/pycgs/cgs.py` & `pycgs-1.0.1/pycgs/cgs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 This module contains the algorithms for Coreference-based Graph Search (CGS).
 """
 
-
 import networkx as nx
 
 from pycgs.type import Edge, EdgeWithWeight
 
 
 __all__ = ["foundational_cgs", "weighted_cgs"]
 
@@ -15,16 +14,19 @@
     """
     Foundational CGS algorithm.
     """
     # Create a Directed Acyclic Graph
     cptg = nx.DiGraph()  # CPTG: Coreference-based Primary Term Graph
 
     # Add edges to the graph based on the coreference relationships
-    for src, tgt in relationships:
-        cptg.add_edge(src, tgt)
+    cptg.add_edges_from(set(relationships))  # Use set to remove duplicates
+
+    # Check if the graph is a Directed Acyclic Graph
+    if not nx.is_directed_acyclic_graph(cptg):
+        raise ValueError("The graph is  not a Directed Acyclic Graph.")
 
     # Initialize the dictionary to store the ultimate Primary Terms
     primary_term_dict = {}
 
     # Iterate through each node in the graph
     for node in cptg.nodes():
         # Check if the node is a Primary Term (out-degree == 0)
@@ -32,15 +34,17 @@
             # The node is a Primary Term, map it to itself
             primary_term_dict[node] = node
         else:
             # The node is not a Primary Term, find its ultimate Primary Term
             current = node
             while cptg.out_degree(current) != 0:
                 # Follow the directed edges to find the Primary Term
-                current = next(cptg.successors(current))
+                current = sorted(cptg.successors(current))[
+                    0
+                ]  # Sort to get a deterministic result
             primary_term_dict[node] = current
 
     return primary_term_dict
 
 
 def weighted_cgs(relationships: list[EdgeWithWeight]) -> dict[str, str]:
     """
```

### Comparing `pycgs-1.0.0/pyproject.toml` & `pycgs-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pycgs"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python implementation of the Coreference-based Graph Search (CGS) algorithm."
 authors = ["YANG Zijie <yangzijie@westlake.edu.cn>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 networkx = "^3.1.0"
 
-[tool.poetry.group.test.dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # If you want to publish the package, please:
```

### Comparing `pycgs-1.0.0/PKG-INFO` & `pycgs-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,11 @@
-Metadata-Version: 2.1
-Name: pycgs
-Version: 1.0.0
-Summary: Python implementation of the Coreference-based Graph Search (CGS) algorithm.
-License: Apache-2.0
-Author: YANG Zijie
-Author-email: yangzijie@westlake.edu.cn
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: networkx (>=3.1.0,<4.0.0)
-Description-Content-Type: text/markdown
-
 # Coreference-based Graph Search (CGS)
 
+[![PyPI version](https://img.shields.io/pypi/v/pycgs.svg)](https://pypi.org/project/pycgs/)
+
 This is the Python implementation of the CGS algorithm.
 
 ## Documentation
 
 The documentation for `pycgs` is available on the documentation website of the ShennongAlpha ([ShennongDoc](https://shennongalpha.westlake.edu.cn/doc/)):
 
 - [English](https://shennongalpha.westlake.edu.cn/doc/en/pycgs/)
@@ -51,7 +38,19 @@
 primary_terms = cgs.weighted_cgs(weighted_relationships)
 
 print(primary_terms)
 # Output:
 # {'A': 'C', 'B': 'C', 'C': 'C', 'D': 'C', 'E': 'E'}
 ```
 
+## Cite this work
+
+```bibtex
+@misc{yang2024shennongalpha,
+      title={ShennongAlpha: an AI-driven sharing and collaboration platform for intelligent curation, acquisition, and translation of natural medicinal material knowledge}, 
+      author={Zijie Yang and Yongjing Yin and Chaojun Kong and Tiange Chi and Wufan Tao and Yue Zhang and Tian Xu},
+      year={2024},
+      eprint={2401.00020},
+      archivePrefix={arXiv},
+      primaryClass={cs.AI}
+}
+```
```


# Comparing `tmp/pandasaurus_cxg-0.1.8.tar.gz` & `tmp/pandasaurus_cxg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasaurus_cxg-0.1.8.tar", max compression
+gzip compressed data, was "pandasaurus_cxg-0.1.9.tar", max compression
```

## Comparing `pandasaurus_cxg-0.1.8.tar` & `pandasaurus_cxg-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-06-02 09:38:11.366287 pandasaurus_cxg-0.1.8/LICENSE
--rw-r--r--   0        0        0     3422 2023-11-03 12:50:53.135452 pandasaurus_cxg-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-06-13 12:28:04.929113 pandasaurus_cxg-0.1.8/pandasaurus_cxg/__init__.py
--rw-r--r--   0        0        0    11275 2023-11-03 12:49:19.764021 pandasaurus_cxg-0.1.8/pandasaurus_cxg/anndata_analyzer.py
--rw-r--r--   0        0        0    12866 2023-09-29 14:40:53.716559 pandasaurus_cxg-0.1.8/pandasaurus_cxg/anndata_enricher.py
--rw-r--r--   0        0        0     6595 2023-09-29 14:40:53.716772 pandasaurus_cxg-0.1.8/pandasaurus_cxg/enrichment_analysis.py
--rw-r--r--   0        0        0        0 2023-09-06 08:20:39.164748 pandasaurus_cxg-0.1.8/pandasaurus_cxg/graph_generator/__init__.py
--rw-r--r--   0        0        0    18553 2024-02-05 15:01:04.333046 pandasaurus_cxg-0.1.8/pandasaurus_cxg/graph_generator/graph_generator.py
--rw-r--r--   0        0        0     4176 2023-09-29 14:40:53.717249 pandasaurus_cxg-0.1.8/pandasaurus_cxg/graph_generator/graph_generator_utils.py
--rw-r--r--   0        0        0      286 2023-09-29 12:12:24.021281 pandasaurus_cxg-0.1.8/pandasaurus_cxg/graph_generator/graph_predicates.py
--rw-r--r--   0        0        0        0 2023-06-23 11:33:16.769497 pandasaurus_cxg-0.1.8/pandasaurus_cxg/schema/__init__.py
--rw-r--r--   0        0        0      549 2023-08-24 14:26:41.001994 pandasaurus_cxg-0.1.8/pandasaurus_cxg/schema/cell_x_gene_schema.py
--rw-r--r--   0        0        0        0 2023-06-15 12:22:49.490756 pandasaurus_cxg-0.1.8/pandasaurus_cxg/utils/__init__.py
--rw-r--r--   0        0        0      971 2023-08-29 08:43:15.400647 pandasaurus_cxg-0.1.8/pandasaurus_cxg/utils/anndata_loader.py
--rw-r--r--   0        0        0     2110 2023-11-03 12:49:19.764682 pandasaurus_cxg-0.1.8/pandasaurus_cxg/utils/exceptions.py
--rw-r--r--   0        0        0      926 2023-08-08 15:17:54.941714 pandasaurus_cxg-0.1.8/pandasaurus_cxg/utils/logging_config.py
--rw-r--r--   0        0        0     1079 2024-02-05 16:33:49.910426 pandasaurus_cxg-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4461 1970-01-01 00:00:00.000000 pandasaurus_cxg-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-20 15:15:26.874527 pandasaurus_cxg-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3422 2024-02-20 15:15:26.874629 pandasaurus_cxg-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-20 15:15:26.876197 pandasaurus_cxg-0.1.9/pandasaurus_cxg/__init__.py
+-rw-r--r--   0        0        0    11275 2024-02-20 15:15:26.876317 pandasaurus_cxg-0.1.9/pandasaurus_cxg/anndata_analyzer.py
+-rw-r--r--   0        0        0    12866 2024-02-20 15:15:26.876426 pandasaurus_cxg-0.1.9/pandasaurus_cxg/anndata_enricher.py
+-rw-r--r--   0        0        0     6595 2024-02-20 15:15:26.876519 pandasaurus_cxg-0.1.9/pandasaurus_cxg/enrichment_analysis.py
+-rw-r--r--   0        0        0        0 2024-02-20 15:15:26.876592 pandasaurus_cxg-0.1.9/pandasaurus_cxg/graph_generator/__init__.py
+-rw-r--r--   0        0        0    18553 2024-02-20 15:15:26.876713 pandasaurus_cxg-0.1.9/pandasaurus_cxg/graph_generator/graph_generator.py
+-rw-r--r--   0        0        0     4176 2024-02-20 15:15:26.876814 pandasaurus_cxg-0.1.9/pandasaurus_cxg/graph_generator/graph_generator_utils.py
+-rw-r--r--   0        0        0      286 2024-02-20 15:15:26.876890 pandasaurus_cxg-0.1.9/pandasaurus_cxg/graph_generator/graph_predicates.py
+-rw-r--r--   0        0        0        0 2024-02-20 15:15:26.876972 pandasaurus_cxg-0.1.9/pandasaurus_cxg/schema/__init__.py
+-rw-r--r--   0        0        0      549 2024-02-20 15:15:26.877071 pandasaurus_cxg-0.1.9/pandasaurus_cxg/schema/cell_x_gene_schema.py
+-rw-r--r--   0        0        0        0 2024-02-20 15:15:26.877155 pandasaurus_cxg-0.1.9/pandasaurus_cxg/utils/__init__.py
+-rw-r--r--   0        0        0      971 2024-02-20 15:15:26.877263 pandasaurus_cxg-0.1.9/pandasaurus_cxg/utils/anndata_loader.py
+-rw-r--r--   0        0        0     2110 2024-02-20 15:15:26.877344 pandasaurus_cxg-0.1.9/pandasaurus_cxg/utils/exceptions.py
+-rw-r--r--   0        0        0      926 2024-02-20 15:15:26.877431 pandasaurus_cxg-0.1.9/pandasaurus_cxg/utils/logging_config.py
+-rw-r--r--   0        0        0     1079 2024-03-06 14:31:17.296666 pandasaurus_cxg-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 pandasaurus_cxg-0.1.9/PKG-INFO
```

### Comparing `pandasaurus_cxg-0.1.8/LICENSE` & `pandasaurus_cxg-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/README.md` & `pandasaurus_cxg-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/anndata_analyzer.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/anndata_analyzer.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/anndata_enricher.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/anndata_enricher.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/enrichment_analysis.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/enrichment_analysis.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/graph_generator/graph_generator.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/graph_generator/graph_generator.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/graph_generator/graph_generator_utils.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/graph_generator/graph_generator_utils.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/schema/cell_x_gene_schema.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/schema/cell_x_gene_schema.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/utils/anndata_loader.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/utils/anndata_loader.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/utils/exceptions.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pandasaurus_cxg/utils/logging_config.py` & `pandasaurus_cxg-0.1.9/pandasaurus_cxg/utils/logging_config.py`

 * *Files identical despite different names*

### Comparing `pandasaurus_cxg-0.1.8/pyproject.toml` & `pandasaurus_cxg-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pandasaurus-cxg"
-version = "0.1.8"
+version = "0.1.9"
 description = "Ontology enrichment tool for CxG standard AnnData files."
 authors = ["Ugur Bayindir <ugur@ebi.ac.uk>"]
 license = "http://www.apache.org/licenses/LICENSE-2.0"
 readme = "README.md"
 packages = [{include = "pandasaurus_cxg"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.0.2"
 anndata = "^0.9.1"
 rdflib = "^6.3.2"
-oaklib = "0.5.13"
+oaklib = "0.5.25"
 matplotlib = "^3.7.2"
-pandasaurus = "^0.3.6"
+pandasaurus = "^0.3.8"
 pygraphviz = "^1.11"
 sphinx = { version = "^7.2.6", optional = true }
 sphinx-rtd-theme = { version = "^1.3.0", optional = true }
 sphinx-copybutton = { version = "^0.5.2", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
```

### Comparing `pandasaurus_cxg-0.1.8/PKG-INFO` & `pandasaurus_cxg-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pandasaurus-cxg
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ontology enrichment tool for CxG standard AnnData files.
 License: http://www.apache.org/licenses/LICENSE-2.0
 Author: Ugur Bayindir
 Author-email: ugur@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Requires-Dist: anndata (>=0.9.1,<0.10.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
-Requires-Dist: oaklib (==0.5.13)
+Requires-Dist: oaklib (==0.5.25)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: pandasaurus (>=0.3.6,<0.4.0)
+Requires-Dist: pandasaurus (>=0.3.8,<0.4.0)
 Requires-Dist: pygraphviz (>=1.11,<2.0)
 Requires-Dist: rdflib (>=6.3.2,<7.0.0)
 Requires-Dist: sphinx (>=7.2.6,<8.0.0) ; extra == "docs"
 Requires-Dist: sphinx-copybutton (>=0.5.2,<0.6.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.3.0,<2.0.0) ; extra == "docs"
 Description-Content-Type: text/markdown
```


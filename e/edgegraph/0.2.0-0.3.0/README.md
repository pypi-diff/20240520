# Comparing `tmp/edgegraph-0.2.0.tar.gz` & `tmp/edgegraph-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegraph-0.2.0.tar", last modified: Mon Apr 22 02:31:57 2024, max compression
+gzip compressed data, was "edgegraph-0.3.0.tar", last modified: Mon May 20 01:59:04 2024, max compression
```

## Comparing `edgegraph-0.2.0.tar` & `edgegraph-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.891065 edgegraph-0.2.0/
--rw-r--r--   0 misha     (1000) misha     (1000)     7653 2024-02-03 17:29:08.000000 edgegraph-0.2.0/LICENSE.txt
--rw-r--r--   0 misha     (1000) misha     (1000)    11342 2024-04-22 02:31:57.891065 edgegraph-0.2.0/PKG-INFO
--rw-r--r--   0 misha     (1000) misha     (1000)     1974 2024-04-22 02:31:28.000000 edgegraph-0.2.0/README.md
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/
--rw-r--r--   0 misha     (1000) misha     (1000)       80 2023-11-23 23:59:00.000000 edgegraph-0.2.0/edgegraph/__init__.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/builder/
--rw-r--r--   0 misha     (1000) misha     (1000)       98 2024-01-13 17:42:47.000000 edgegraph-0.2.0/edgegraph/builder/__init__.py
--rw-r--r--   0 misha     (1000) misha     (1000)     2511 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/builder/adjlist.py
--rw-r--r--   0 misha     (1000) misha     (1000)     4667 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/builder/adjmatrix.py
--rw-r--r--   0 misha     (1000) misha     (1000)     2890 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/builder/explicit.py
--rw-r--r--   0 misha     (1000) misha     (1000)     1698 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/builder/randgraph.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/output/
--rw-r--r--   0 misha     (1000) misha     (1000)      119 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/output/__init__.py
--rw-r--r--   0 misha     (1000) misha     (1000)     3006 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/output/plaintext.py
--rw-r--r--   0 misha     (1000) misha     (1000)    13381 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/output/plantuml.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/structure/
--rw-r--r--   0 misha     (1000) misha     (1000)      321 2024-01-06 22:51:15.000000 edgegraph-0.2.0/edgegraph/structure/__init__.py
--rw-r--r--   0 misha     (1000) misha     (1000)     7022 2024-01-21 18:34:41.000000 edgegraph-0.2.0/edgegraph/structure/base.py
--rw-r--r--   0 misha     (1000) misha     (1000)     2458 2024-01-07 18:11:08.000000 edgegraph-0.2.0/edgegraph/structure/directededge.py
--rw-r--r--   0 misha     (1000) misha     (1000)     4010 2024-01-04 22:18:37.000000 edgegraph-0.2.0/edgegraph/structure/link.py
--rw-r--r--   0 misha     (1000) misha     (1000)     4082 2024-01-06 23:41:34.000000 edgegraph-0.2.0/edgegraph/structure/twoendedlink.py
--rw-r--r--   0 misha     (1000) misha     (1000)      955 2024-01-07 18:11:08.000000 edgegraph-0.2.0/edgegraph/structure/undirectededge.py
--rw-r--r--   0 misha     (1000) misha     (1000)     8462 2024-01-13 22:25:13.000000 edgegraph-0.2.0/edgegraph/structure/universe.py
--rw-r--r--   0 misha     (1000) misha     (1000)     3974 2024-01-04 22:18:37.000000 edgegraph-0.2.0/edgegraph/structure/vertex.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/traversal/
--rw-r--r--   0 misha     (1000) misha     (1000)       86 2024-01-15 02:49:14.000000 edgegraph-0.2.0/edgegraph/traversal/__init__.py
--rw-r--r--   0 misha     (1000) misha     (1000)     3207 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/traversal/breadthfirst.py
--rw-r--r--   0 misha     (1000) misha     (1000)     9283 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/traversal/depthfirst.py
--rw-r--r--   0 misha     (1000) misha     (1000)     3993 2024-02-08 03:50:53.000000 edgegraph-0.2.0/edgegraph/traversal/helpers.py
--rw-r--r--   0 misha     (1000) misha     (1000)      470 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/version.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph.egg-info/
--rw-r--r--   0 misha     (1000) misha     (1000)    11342 2024-04-22 02:31:57.000000 edgegraph-0.2.0/edgegraph.egg-info/PKG-INFO
--rw-r--r--   0 misha     (1000) misha     (1000)      865 2024-04-22 02:31:57.000000 edgegraph-0.2.0/edgegraph.egg-info/SOURCES.txt
--rw-r--r--   0 misha     (1000) misha     (1000)        1 2024-04-22 02:31:57.000000 edgegraph-0.2.0/edgegraph.egg-info/dependency_links.txt
--rw-r--r--   0 misha     (1000) misha     (1000)       10 2024-04-22 02:31:57.000000 edgegraph-0.2.0/edgegraph.egg-info/top_level.txt
--rw-r--r--   0 misha     (1000) misha     (1000)     1471 2024-02-03 17:53:21.000000 edgegraph-0.2.0/pyproject.toml
--rw-r--r--   0 misha     (1000) misha     (1000)       38 2024-04-22 02:31:57.891065 edgegraph-0.2.0/setup.cfg
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/tests/
--rw-r--r--   0 misha     (1000) misha     (1000)     1030 2024-02-03 17:45:46.000000 edgegraph-0.2.0/tests/test_version.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-05-20 01:59:04.851089 edgegraph-0.3.0/
+-rw-r--r--   0 misha     (1000) misha     (1000)     7653 2024-02-03 17:29:08.000000 edgegraph-0.3.0/LICENSE.txt
+-rw-r--r--   0 misha     (1000) misha     (1000)    11663 2024-05-20 01:59:04.851089 edgegraph-0.3.0/PKG-INFO
+-rw-r--r--   0 misha     (1000) misha     (1000)     2078 2024-05-20 01:58:26.000000 edgegraph-0.3.0/README.md
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-05-20 01:59:04.847089 edgegraph-0.3.0/edgegraph/
+-rw-r--r--   0 misha     (1000) misha     (1000)       80 2023-11-23 23:59:00.000000 edgegraph-0.3.0/edgegraph/__init__.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-05-20 01:59:04.847089 edgegraph-0.3.0/edgegraph/builder/
+-rw-r--r--   0 misha     (1000) misha     (1000)       98 2024-01-13 17:42:47.000000 edgegraph-0.3.0/edgegraph/builder/__init__.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     2511 2024-04-22 02:31:28.000000 edgegraph-0.3.0/edgegraph/builder/adjlist.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     4667 2024-04-22 02:31:28.000000 edgegraph-0.3.0/edgegraph/builder/adjmatrix.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3856 2024-05-20 01:58:26.000000 edgegraph-0.3.0/edgegraph/builder/explicit.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     1698 2024-04-22 02:31:28.000000 edgegraph-0.3.0/edgegraph/builder/randgraph.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-05-20 01:59:04.847089 edgegraph-0.3.0/edgegraph/output/
+-rw-r--r--   0 misha     (1000) misha     (1000)      119 2024-04-22 02:31:28.000000 edgegraph-0.3.0/edgegraph/output/__init__.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3006 2024-04-26 18:33:08.000000 edgegraph-0.3.0/edgegraph/output/plaintext.py
+-rw-r--r--   0 misha     (1000) misha     (1000)    13381 2024-04-26 18:33:08.000000 edgegraph-0.3.0/edgegraph/output/plantuml.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     7247 2024-05-20 01:58:26.000000 edgegraph-0.3.0/edgegraph/output/pyvis.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-05-20 01:59:04.847089 edgegraph-0.3.0/edgegraph/structure/
+-rw-r--r--   0 misha     (1000) misha     (1000)      321 2024-01-06 22:51:15.000000 edgegraph-0.3.0/edgegraph/structure/__init__.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     7022 2024-01-21 18:34:41.000000 edgegraph-0.3.0/edgegraph/structure/base.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     2458 2024-01-07 18:11:08.000000 edgegraph-0.3.0/edgegraph/structure/directededge.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     4010 2024-01-04 22:18:37.000000 edgegraph-0.3.0/edgegraph/structure/link.py
+-rw-r--r--   0 misha     (1000) misha     (1000)    15577 2024-05-20 01:58:26.000000 edgegraph-0.3.0/edgegraph/structure/singleton.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     4082 2024-01-06 23:41:34.000000 edgegraph-0.3.0/edgegraph/structure/twoendedlink.py
+-rw-r--r--   0 misha     (1000) misha     (1000)      955 2024-01-07 18:11:08.000000 edgegraph-0.3.0/edgegraph/structure/undirectededge.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     8462 2024-01-13 22:25:13.000000 edgegraph-0.3.0/edgegraph/structure/universe.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3974 2024-01-04 22:18:37.000000 edgegraph-0.3.0/edgegraph/structure/vertex.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-05-20 01:59:04.847089 edgegraph-0.3.0/edgegraph/traversal/
+-rw-r--r--   0 misha     (1000) misha     (1000)       86 2024-01-15 02:49:14.000000 edgegraph-0.3.0/edgegraph/traversal/__init__.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3207 2024-04-22 02:31:28.000000 edgegraph-0.3.0/edgegraph/traversal/breadthfirst.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     9283 2024-04-26 18:33:08.000000 edgegraph-0.3.0/edgegraph/traversal/depthfirst.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3993 2024-02-08 03:50:53.000000 edgegraph-0.3.0/edgegraph/traversal/helpers.py
+-rw-r--r--   0 misha     (1000) misha     (1000)      470 2024-05-20 01:58:26.000000 edgegraph-0.3.0/edgegraph/version.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-05-20 01:59:04.851089 edgegraph-0.3.0/edgegraph.egg-info/
+-rw-r--r--   0 misha     (1000) misha     (1000)    11663 2024-05-20 01:59:04.000000 edgegraph-0.3.0/edgegraph.egg-info/PKG-INFO
+-rw-r--r--   0 misha     (1000) misha     (1000)      924 2024-05-20 01:59:04.000000 edgegraph-0.3.0/edgegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 misha     (1000) misha     (1000)        1 2024-05-20 01:59:04.000000 edgegraph-0.3.0/edgegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 misha     (1000) misha     (1000)       10 2024-05-20 01:59:04.000000 edgegraph-0.3.0/edgegraph.egg-info/top_level.txt
+-rw-r--r--   0 misha     (1000) misha     (1000)     2127 2024-05-20 01:58:26.000000 edgegraph-0.3.0/pyproject.toml
+-rw-r--r--   0 misha     (1000) misha     (1000)       38 2024-05-20 01:59:04.851089 edgegraph-0.3.0/setup.cfg
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-05-20 01:59:04.847089 edgegraph-0.3.0/tests/
+-rw-r--r--   0 misha     (1000) misha     (1000)     1025 2024-05-20 01:58:26.000000 edgegraph-0.3.0/tests/test_version.py
```

### Comparing `edgegraph-0.2.0/LICENSE.txt` & `edgegraph-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/PKG-INFO` & `edgegraph-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegraph
-Version: 0.2.0
+Version: 0.3.0
 Summary: Object oriented edge-vertex graph library.
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -165,18 +165,22 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
         
-Project-URL: Homepage, https://github.com/mishaturnbull/edgegraph
+Project-URL: Homepage, https://edgegraph.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/mishaturnbull/edgegraph
-Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.8
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # EdgeGraph
 
 EdgeGraph is an object-oriented approach to network graphs.  It provides
 classes to inherit from in other applications / modules, and provides
@@ -208,19 +212,21 @@
 * [x] Breadth-first search and traversal
 * [x] Depth-first search and traversal
 * [ ] Topological sorting
 * [ ] Strongly connected component detection
 * [ ] Universe island detection
 * [ ] Shortest path detection
 * [x] Graph drawing generation via PlantUML
+* [x] Graph export to PyVis, ready for interactive display
 * [ ] Formal automata modelling (DFA, NFA, etc)
 * [ ] Operation flow graph modelling (nodes as operations instead of states)
 * [ ] "Functional graphs" -- attach executable code to nodes and run a graph as
       a program
 * [ ] Object serialization, save-to- and load-from-file
+* [x] Singleton and semi-singleton utilities
 
 These features, as with the API, may be changed or dropped at any time without
 warning.  I do have a day job, after all :)
 
 Sphinx documentation and full Pytest-driven unit testing coverage is expected
 to match the progress of the code.
```

### Comparing `edgegraph-0.2.0/README.md` & `edgegraph-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 * [x] Breadth-first search and traversal
 * [x] Depth-first search and traversal
 * [ ] Topological sorting
 * [ ] Strongly connected component detection
 * [ ] Universe island detection
 * [ ] Shortest path detection
 * [x] Graph drawing generation via PlantUML
+* [x] Graph export to PyVis, ready for interactive display
 * [ ] Formal automata modelling (DFA, NFA, etc)
 * [ ] Operation flow graph modelling (nodes as operations instead of states)
 * [ ] "Functional graphs" -- attach executable code to nodes and run a graph as
       a program
 * [ ] Object serialization, save-to- and load-from-file
+* [x] Singleton and semi-singleton utilities
 
 These features, as with the API, may be changed or dropped at any time without
 warning.  I do have a day job, after all :)
 
 Sphinx documentation and full Pytest-driven unit testing coverage is expected
 to match the progress of the code.
```

### Comparing `edgegraph-0.2.0/edgegraph/builder/adjlist.py` & `edgegraph-0.3.0/edgegraph/builder/adjlist.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/builder/adjmatrix.py` & `edgegraph-0.3.0/edgegraph/builder/adjmatrix.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/builder/randgraph.py` & `edgegraph-0.3.0/edgegraph/builder/randgraph.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/output/plaintext.py` & `edgegraph-0.3.0/edgegraph/output/plaintext.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/output/plantuml.py` & `edgegraph-0.3.0/edgegraph/output/plantuml.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/structure/base.py` & `edgegraph-0.3.0/edgegraph/structure/base.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/structure/directededge.py` & `edgegraph-0.3.0/edgegraph/structure/directededge.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/structure/link.py` & `edgegraph-0.3.0/edgegraph/structure/link.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/structure/twoendedlink.py` & `edgegraph-0.3.0/edgegraph/structure/twoendedlink.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/structure/undirectededge.py` & `edgegraph-0.3.0/edgegraph/structure/undirectededge.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/structure/universe.py` & `edgegraph-0.3.0/edgegraph/structure/universe.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/structure/vertex.py` & `edgegraph-0.3.0/edgegraph/structure/vertex.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/traversal/breadthfirst.py` & `edgegraph-0.3.0/edgegraph/traversal/breadthfirst.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/traversal/depthfirst.py` & `edgegraph-0.3.0/edgegraph/traversal/depthfirst.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph/traversal/helpers.py` & `edgegraph-0.3.0/edgegraph/traversal/helpers.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.2.0/edgegraph.egg-info/PKG-INFO` & `edgegraph-0.3.0/edgegraph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegraph
-Version: 0.2.0
+Version: 0.3.0
 Summary: Object oriented edge-vertex graph library.
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -165,18 +165,22 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
         
-Project-URL: Homepage, https://github.com/mishaturnbull/edgegraph
+Project-URL: Homepage, https://edgegraph.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/mishaturnbull/edgegraph
-Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.8
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # EdgeGraph
 
 EdgeGraph is an object-oriented approach to network graphs.  It provides
 classes to inherit from in other applications / modules, and provides
@@ -208,19 +212,21 @@
 * [x] Breadth-first search and traversal
 * [x] Depth-first search and traversal
 * [ ] Topological sorting
 * [ ] Strongly connected component detection
 * [ ] Universe island detection
 * [ ] Shortest path detection
 * [x] Graph drawing generation via PlantUML
+* [x] Graph export to PyVis, ready for interactive display
 * [ ] Formal automata modelling (DFA, NFA, etc)
 * [ ] Operation flow graph modelling (nodes as operations instead of states)
 * [ ] "Functional graphs" -- attach executable code to nodes and run a graph as
       a program
 * [ ] Object serialization, save-to- and load-from-file
+* [x] Singleton and semi-singleton utilities
 
 These features, as with the API, may be changed or dropped at any time without
 warning.  I do have a day job, after all :)
 
 Sphinx documentation and full Pytest-driven unit testing coverage is expected
 to match the progress of the code.
```

### Comparing `edgegraph-0.2.0/edgegraph.egg-info/SOURCES.txt` & `edgegraph-0.3.0/edgegraph.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 edgegraph/builder/adjlist.py
 edgegraph/builder/adjmatrix.py
 edgegraph/builder/explicit.py
 edgegraph/builder/randgraph.py
 edgegraph/output/__init__.py
 edgegraph/output/plaintext.py
 edgegraph/output/plantuml.py
+edgegraph/output/pyvis.py
 edgegraph/structure/__init__.py
 edgegraph/structure/base.py
 edgegraph/structure/directededge.py
 edgegraph/structure/link.py
+edgegraph/structure/singleton.py
 edgegraph/structure/twoendedlink.py
 edgegraph/structure/undirectededge.py
 edgegraph/structure/universe.py
 edgegraph/structure/vertex.py
 edgegraph/traversal/__init__.py
 edgegraph/traversal/breadthfirst.py
 edgegraph/traversal/depthfirst.py
```

### Comparing `edgegraph-0.2.0/pyproject.toml` & `edgegraph-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["version"]
 name = "edgegraph"
-requires-python = ">= 3.8"
+requires-python = ">= 3.7"
 dependencies = []
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 description = "Object oriented edge-vertex graph library."
 classifiers = [
-	"Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3 :: Only",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [project.urls]
-Homepage = "https://github.com/mishaturnbull/edgegraph"
+Homepage = "https://edgegraph.readthedocs.io/en/latest/"
 Repository = "https://github.com/mishaturnbull/edgegraph"
 
 [tool.setuptools.dynamic]
 version = {attr = "edgegraph.version.__version__"}
 
 # Pylint settings
 [tool.pylint.main]
@@ -39,9 +43,23 @@
             # see https://github.com/pylint-dev/pylint/issues/8215
             # using ``from __future__ import annotations`` does not silence
             # pylint's undefined variable error -- because that is used all
             # over the place, everything goes to shite if this error isn't
             # silenced.  instead, i'll assume (hopefully) that such errors are
             # caught by unit testing.
             "undefined-variable",
+
+            # performance gain from lazy logging formatting is negligible by
+            # timing tests
+            "logging-fstring-interpolation",
            ]
 
+[tool.pytest.ini_options]
+markers = [
+    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+]
+addopts = "-ra --durations=5"
+log_cli = false
+log_cli_level = "DEBUG"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+log_cli_date_format = "%Y-%m-%d %H:%M:%S"
+
```

### Comparing `edgegraph-0.2.0/tests/test_version.py` & `edgegraph-0.3.0/tests/test_version.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 """
-Unit tests for Universe object.
+Ensure the versioning constants are valid.
 """
 
-import pytest
 import re
 from edgegraph import version
 
 def test_version():
     """
     Test version attributes are accessible.
 
@@ -26,15 +25,15 @@
     # 5 is the minimum possible length, of "0.0.0"
     assert len(version.__version__) >= 5
 
 def test_python_version_compliance():
     """
     Test version attribute is complaint with PyPA standard.
 
-    See 
+    See
     https://packaging.python.org/en/latest/specifications/version-specifiers/#version-specifiers
     """
 
-    PTRN = (r'^([1-9][0-9]*!)?(0|[1-9][0-9]*)(\.(0|[1-9][0-9]*))*((a|b|rc)"'
+    ptrn= (r'^([1-9][0-9]*!)?(0|[1-9][0-9]*)(\.(0|[1-9][0-9]*))*((a|b|rc)"'
            r'(0|[1-9][0-9]*))?(\.post(0|[1-9][0-9]*))?(\.dev(0|[1-9][0-9]*))?$')
-    assert re.match(PTRN, version.__version__)
+    assert re.match(ptrn, version.__version__)
```


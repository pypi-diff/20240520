# Comparing `tmp/opentldr-0.5.1.tar.gz` & `tmp/opentldr-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentldr-0.5.1.tar", last modified: Thu May  9 21:17:29 2024, max compression
+gzip compressed data, was "opentldr-0.5.2.tar", last modified: Mon May 20 01:47:41 2024, max compression
```

## Comparing `opentldr-0.5.1.tar` & `opentldr-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:17:29.050219 opentldr-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 21:17:23.000000 opentldr-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 21:17:23.000000 opentldr-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-09 21:17:29.050219 opentldr-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-09 21:17:23.000000 opentldr-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-09 21:17:23.000000 opentldr-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:17:29.050219 opentldr-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:17:29.042219 opentldr-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:17:29.046219 opentldr-0.5.1/src/opentldr/
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/AbstractDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/DataRepoJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    28658 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/FileSystemDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    34572 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/KnowledgeGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/S3DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-09 21:17:23.000000 opentldr-0.5.1/src/opentldr/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:17:29.050219 opentldr-0.5.1/src/opentldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-09 21:17:29.000000 opentldr-0.5.1/src/opentldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 21:17:29.000000 opentldr-0.5.1/src/opentldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:17:29.000000 opentldr-0.5.1/src/opentldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-09 21:17:29.000000 opentldr-0.5.1/src/opentldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 21:17:29.000000 opentldr-0.5.1/src/opentldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:17:29.050219 opentldr-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 21:17:23.000000 opentldr-0.5.1/tests/test_contentrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 21:17:23.000000 opentldr-0.5.1/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-09 21:17:23.000000 opentldr-0.5.1/tests/test_knowledgegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-09 21:17:23.000000 opentldr-0.5.1/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.262182 opentldr-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 01:47:36.000000 opentldr-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:36.000000 opentldr-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-20 01:47:41.262182 opentldr-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-20 01:47:36.000000 opentldr-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-20 01:47:36.000000 opentldr-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:47:41.262182 opentldr-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.254182 opentldr-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.258182 opentldr-0.5.2/src/opentldr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/AbstractDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/DataRepoJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28658 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/FileSystemDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34618 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/KnowledgeGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/S3DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.262182 opentldr-0.5.2/src/opentldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.262182 opentldr-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 01:47:36.000000 opentldr-0.5.2/tests/test_contentrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 01:47:36.000000 opentldr-0.5.2/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-20 01:47:36.000000 opentldr-0.5.2/tests/test_knowledgegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-20 01:47:36.000000 opentldr-0.5.2/tests/test_workflow.py
```

### Comparing `opentldr-0.5.1/LICENSE` & `opentldr-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/PKG-INFO` & `opentldr-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.1
+Version: 0.5.2
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,19 @@
 
 # OpenTLDR-Core
 An Open Framework for Generating an Tailored Daily Report
 This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
+The latest OpenTLDR-Core library is availible as a Pip Package:
+<pre>
+python3 -m pip install opentldr
+</pre>
+
 ## Introduction to OpenTLDR
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you can find in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
 - A **KnowledgeGraph** module that has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
```

### Comparing `opentldr-0.5.1/README.md` & `opentldr-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # OpenTLDR-Core
 An Open Framework for Generating an Tailored Daily Report
 This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
+The latest OpenTLDR-Core library is availible as a Pip Package:
+<pre>
+python3 -m pip install opentldr
+</pre>
+
 ## Introduction to OpenTLDR
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you can find in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
 - A **KnowledgeGraph** module that has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
```

### Comparing `opentldr-0.5.1/pyproject.toml` & `opentldr-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "opentldr"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Chris Argenta", email="cargenta@rockfishresearch.com" },
 ]
 description = "An open framework for creation of a Tailored Daily Report."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `opentldr-0.5.1/src/opentldr/AbstractDataRepo.py` & `opentldr-0.5.2/src/opentldr/AbstractDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/src/opentldr/DataRepo.py` & `opentldr-0.5.2/src/opentldr/DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/src/opentldr/DataRepoJson.py` & `opentldr-0.5.2/src/opentldr/DataRepoJson.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/src/opentldr/Domain.py` & `opentldr-0.5.2/src/opentldr/Domain.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/src/opentldr/FileSystemDataRepo.py` & `opentldr-0.5.2/src/opentldr/FileSystemDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/src/opentldr/KnowledgeGraph.py` & `opentldr-0.5.2/src/opentldr/KnowledgeGraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from neo4j import GraphDatabase
 import neomodel as nm
 
 from opentldr.Domain import *
 from .log import log
 
 load_dotenv()
+load_dotenv("{d}/.env".format(d=os.getcwd()))
 
 def _getenv(variable:str , default:str):
         '''
         _getenv(variable, default) attempts to resolve the value of the environment variable specified.
         If it cannot find the variable in the OS or .env (from dotenv package) it will fail over to the
         provided default value while giving a warning to the logging system.
         '''
```

### Comparing `opentldr-0.5.1/src/opentldr/S3DataRepo.py` & `opentldr-0.5.2/src/opentldr/S3DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/src/opentldr/Workflow.py` & `opentldr-0.5.2/src/opentldr/Workflow.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/src/opentldr.egg-info/PKG-INFO` & `opentldr-0.5.2/src/opentldr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.1
+Version: 0.5.2
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,19 @@
 
 # OpenTLDR-Core
 An Open Framework for Generating an Tailored Daily Report
 This repository contains the OpenTLDR package. You can 'pip install opentldr' to get the contents of this repository as a python package in your virtaul env.
 
 ![overview image](resources/opentldr.png)
 
+The latest OpenTLDR-Core library is availible as a Pip Package:
+<pre>
+python3 -m pip install opentldr
+</pre>
+
 ## Introduction to OpenTLDR
 
 OpenTLDR is an open source framework written in Python to implement the process of creating a Tailored Daily Report from a series of news-like articles. This repository contains the Core classes used as a library by OpenTLDR implementations, like the example notebooks you can find in the OpenTLDR-Example repo on GitHub.
 
 OpenTLDR is composed of Python modules:
 - A **KnowledgeGraph** module that has been implemented as a layer on top of the Neo4j Graph Database
 - A module with a set of **Domain** classes that implement the nodes and edges in a TLDR-focused knowledge graph
```

### Comparing `opentldr-0.5.1/src/opentldr.egg-info/SOURCES.txt` & `opentldr-0.5.2/src/opentldr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/tests/test_knowledgegraph.py` & `opentldr-0.5.2/tests/test_knowledgegraph.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.1/tests/test_workflow.py` & `opentldr-0.5.2/tests/test_workflow.py`

 * *Files identical despite different names*


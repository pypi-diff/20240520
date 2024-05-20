# Comparing `tmp/graphretrieval-0.1.3.tar.gz` & `tmp/graphretrieval-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphretrieval-0.1.3.tar", last modified: Sun May 19 12:48:53 2024, max compression
+gzip compressed data, was "graphretrieval-0.1.4.tar", last modified: Mon May 20 09:14:33 2024, max compression
```

## Comparing `graphretrieval-0.1.3.tar` & `graphretrieval-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/GraphRetrieval/
--rw-r--r--   0 runner    (1001) docker     (127)    25088 2024-05-19 12:48:45.000000 graphretrieval-0.1.3/GraphRetrieval/GraphRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-19 12:48:45.000000 graphretrieval-0.1.3/GraphRetrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/GraphRetrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-19 12:48:45.000000 graphretrieval-0.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-19 12:48:45.000000 graphretrieval-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:14:33.855372 graphretrieval-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:14:33.851372 graphretrieval-0.1.4/GraphRetrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)    25088 2024-05-20 09:14:29.000000 graphretrieval-0.1.4/GraphRetrieval/GraphRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-20 09:14:29.000000 graphretrieval-0.1.4/GraphRetrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:14:33.855372 graphretrieval-0.1.4/GraphRetrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-20 09:14:33.000000 graphretrieval-0.1.4/GraphRetrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 09:14:33.000000 graphretrieval-0.1.4/GraphRetrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:14:33.000000 graphretrieval-0.1.4/GraphRetrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-20 09:14:33.000000 graphretrieval-0.1.4/GraphRetrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 09:14:33.000000 graphretrieval-0.1.4/GraphRetrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-20 09:14:33.855372 graphretrieval-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-20 09:14:29.000000 graphretrieval-0.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:14:33.855372 graphretrieval-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-20 09:14:29.000000 graphretrieval-0.1.4/setup.py
```

### Comparing `graphretrieval-0.1.3/GraphRetrieval/GraphRetrieval.py` & `graphretrieval-0.1.4/GraphRetrieval/GraphRetrieval.py`

 * *Files identical despite different names*

### Comparing `graphretrieval-0.1.3/GraphRetrieval.egg-info/PKG-INFO` & `graphretrieval-0.1.4/GraphRetrieval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.3
+Version: 0.1.4
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
 Requires-Dist: langchain
 Requires-Dist: sentence_transformers
 Requires-Dist: langchain-community
 Requires-Dist: langchain-openai
 Requires-Dist: langchain-experimental
 Requires-Dist: neo4j
-Requires-Dist: wikipedia
 Requires-Dist: tiktoken
 Requires-Dist: pypdf2
 
 
 # GraphRetrieval
 
 GraphRetrieval is a Python library designed for advanced text retrieval and knowledge graph querying. It supports various models and techniques to enable efficient and accurate information retrieval from large text corpora and knowledge bases.
```

### Comparing `graphretrieval-0.1.3/PKG-INFO` & `graphretrieval-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.3
+Version: 0.1.4
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
 Requires-Dist: langchain
 Requires-Dist: sentence_transformers
 Requires-Dist: langchain-community
 Requires-Dist: langchain-openai
 Requires-Dist: langchain-experimental
 Requires-Dist: neo4j
-Requires-Dist: wikipedia
 Requires-Dist: tiktoken
 Requires-Dist: pypdf2
 
 
 # GraphRetrieval
 
 GraphRetrieval is a Python library designed for advanced text retrieval and knowledge graph querying. It supports various models and techniques to enable efficient and accurate information retrieval from large text corpora and knowledge bases.
```

### Comparing `graphretrieval-0.1.3/README.rst` & `graphretrieval-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `graphretrieval-0.1.3/setup.py` & `graphretrieval-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 This `README.md` provides an overview of the GraphRetrieval library, installation instructions, and example usage scenarios, with the specified changes to the file path and environment variables sections.
 """
 
 setup(
     name='GraphRetrieval',
-    version='0.1.3',
+    version='0.1.4',
     description='Graph retrieval',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='JVNK',
     author_email='jaya11vibhav@gmail.com',
     url='https://github.com/jayavibhavnk/GraphRetrieval',
     packages=find_packages(),
@@ -163,15 +163,14 @@
       'langchain_openai',
       'langchain',
       'sentence_transformers',
       'langchain-community', 
       'langchain-openai',
       'langchain-experimental',
       'neo4j',
-      'wikipedia',
       'tiktoken',
       'pypdf2'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha'
     ],
 )
```


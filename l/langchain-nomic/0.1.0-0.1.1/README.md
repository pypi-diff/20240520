# Comparing `tmp/langchain_nomic-0.1.0.tar.gz` & `tmp/langchain_nomic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_nomic-0.1.0.tar", max compression
+gzip compressed data, was "langchain_nomic-0.1.1.tar", max compression
```

## Comparing `langchain_nomic-0.1.0.tar` & `langchain_nomic-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-05-15 21:30:33.057146 langchain_nomic-0.1.0/LICENSE
--rw-r--r--   0        0        0      476 2024-05-15 21:30:33.057146 langchain_nomic-0.1.0/README.md
--rw-r--r--   0        0        0       93 2024-05-15 21:30:33.057146 langchain_nomic-0.1.0/langchain_nomic/__init__.py
--rw-r--r--   0        0        0     2045 2024-05-15 21:30:33.057146 langchain_nomic-0.1.0/langchain_nomic/embeddings.py
--rw-r--r--   0        0        0        0 2024-05-15 21:30:33.057146 langchain_nomic-0.1.0/langchain_nomic/py.typed
--rw-r--r--   0        0        0     2503 2024-05-15 21:30:33.057146 langchain_nomic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 langchain_nomic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-20 21:17:37.497093 langchain_nomic-0.1.1/LICENSE
+-rw-r--r--   0        0        0      476 2024-05-20 21:17:37.497093 langchain_nomic-0.1.1/README.md
+-rw-r--r--   0        0        0       93 2024-05-20 21:17:37.497093 langchain_nomic-0.1.1/langchain_nomic/__init__.py
+-rw-r--r--   0        0        0     3495 2024-05-20 21:17:37.497093 langchain_nomic-0.1.1/langchain_nomic/embeddings.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:17:37.497093 langchain_nomic-0.1.1/langchain_nomic/py.typed
+-rw-r--r--   0        0        0     2503 2024-05-20 21:17:37.497093 langchain_nomic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 langchain_nomic-0.1.1/PKG-INFO
```

### Comparing `langchain_nomic-0.1.0/LICENSE` & `langchain_nomic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_nomic-0.1.0/pyproject.toml` & `langchain_nomic-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-nomic"
-version = "0.1.0"
+version = "0.1.1"
 description = "An integration package connecting Nomic and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/nomic"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = ">=0.1.46,<0.3"
-nomic = "^3.0.12"
+nomic = "^3.0.29"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
```

### Comparing `langchain_nomic-0.1.0/PKG-INFO` & `langchain_nomic-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-nomic
-Version: 0.1.0
+Version: 0.1.1
 Summary: An integration package connecting Nomic and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain-core (>=0.1.46,<0.3)
-Requires-Dist: nomic (>=3.0.12,<4.0.0)
+Requires-Dist: nomic (>=3.0.29,<4.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/nomic
 Description-Content-Type: text/markdown
 
 # langchain-nomic
 
 This package contains the LangChain integration with Nomic
```


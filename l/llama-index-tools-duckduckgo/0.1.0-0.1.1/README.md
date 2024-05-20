# Comparing `tmp/llama_index_tools_duckduckgo-0.1.0.tar.gz` & `tmp/llama_index_tools_duckduckgo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_tools_duckduckgo-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_tools_duckduckgo-0.1.1.tar", max compression
```

## Comparing `llama_index_tools_duckduckgo-0.1.0.tar` & `llama_index_tools_duckduckgo-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1043 2024-02-28 18:53:20.640827 llama_index_tools_duckduckgo-0.1.0/README.md
--rw-r--r--   0        0        0      111 2024-02-28 18:53:20.640827 llama_index_tools_duckduckgo-0.1.0/llama_index/tools/duckduckgo/__init__.py
--rw-r--r--   0        0        0     1608 2024-02-28 18:53:20.640827 llama_index_tools_duckduckgo-0.1.0/llama_index/tools/duckduckgo/base.py
--rw-r--r--   0        0        0     1533 2024-02-28 18:53:20.650827 llama_index_tools_duckduckgo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 llama_index_tools_duckduckgo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2024-05-20 02:45:35.136341 llama_index_tools_duckduckgo-0.1.1/README.md
+-rw-r--r--   0        0        0      111 2024-05-20 02:45:35.136341 llama_index_tools_duckduckgo-0.1.1/llama_index/tools/duckduckgo/__init__.py
+-rw-r--r--   0        0        0     1730 2024-05-20 02:45:35.136341 llama_index_tools_duckduckgo-0.1.1/llama_index/tools/duckduckgo/base.py
+-rw-r--r--   0        0        0     1533 2024-05-20 02:45:35.136341 llama_index_tools_duckduckgo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 llama_index_tools_duckduckgo-0.1.1/PKG-INFO
```

### Comparing `llama_index_tools_duckduckgo-0.1.0/README.md` & `llama_index_tools_duckduckgo-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This tool has a more extensive example usage documented in a Jupyter notebook [here](./examples/duckduckgo_search.ipynb)
 
 Here's an example usage of the DuckDuckGoSearchToolSpec.
 
 ```python
 from llama_index.tools.duckduckgo import DuckDuckGoSearchToolSpec
-from llama_index.agent import OpenAIAgent
+from llama_index.agent.openai import OpenAIAgent
 
 tool_spec = DuckDuckGoSearchToolSpec()
 
 agent = OpenAIAgent.from_tools(DuckDuckGoSearchToolSpec.to_tool_list())
 
 agent.chat("What's going on with the superconductor lk-99")
 agent.chat("what are the latest developments in machine learning")
```

### Comparing `llama_index_tools_duckduckgo-0.1.0/llama_index/tools/duckduckgo/base.py` & `llama_index_tools_duckduckgo-0.1.1/llama_index/tools/duckduckgo/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,21 +24,30 @@
         """
         from duckduckgo_search import DDGS
 
         with DDGS() as ddg:
             return list(ddg.answers(query))
 
     def duckduckgo_full_search(
-        self, query: str, region: Optional[str] = None, max_results: Optional[int] = 10
+        self,
+        query: str,
+        region: Optional[str] = "wt-wt",
+        max_results: Optional[int] = 10,
     ) -> List[Dict]:
         """
         Make a query to DuckDuckGo search to receive a full search results.
 
         Args:
             query (str): The query to be passed to DuckDuckGo.
             region (Optional[str]): The region to be used for the search in [country-language] convention, ex us-en, uk-en, ru-ru, etc...
             max_results (Optional[int]): The maximum number of results to be returned.
         """
         from duckduckgo_search import DDGS
 
+        params = {
+            "keywords": query,
+            "region": region,
+            "max_results": max_results,
+        }
+
         with DDGS() as ddg:
-            return list(ddg.text(query, region=region, max_results=max_results))
+            return list(ddg.text(**params))
```

### Comparing `llama_index_tools_duckduckgo-0.1.0/pyproject.toml` & `llama_index_tools_duckduckgo-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 description = "llama-index tools integrating DuckDuckGo search"
 exclude = ["**/BUILD"]
 keywords = ["research"]
 license = "MIT"
 maintainers = ["leehuwuj"]
 name = "llama-index-tools-duckduckgo"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
+python = ">=3.8.1,<4.0"
 llama-index = "^0.10.1"
-duckduckgo-search = "4.5.0"
+duckduckgo-search = "^6.1.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_tools_duckduckgo-0.1.0/PKG-INFO` & `llama_index_tools_duckduckgo-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: llama-index-tools-duckduckgo
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index tools integrating DuckDuckGo search
 License: MIT
 Keywords: research
 Author: Your Name
 Author-email: you@example.com
 Maintainer: leehuwuj
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: duckduckgo-search (==4.5.0)
+Requires-Dist: duckduckgo-search (>=6.1.0,<7.0.0)
 Requires-Dist: llama-index (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # DuckDuckGo Search Tool
 
 This tool enables agents to search and retrieve results from the DuckDuckGo search engine. It utilizes the duckduckgo_search package, which either fetches instant query answers from DuckDuckGo or conducts a full search and parses the results.
 
@@ -25,15 +25,15 @@
 
 This tool has a more extensive example usage documented in a Jupyter notebook [here](./examples/duckduckgo_search.ipynb)
 
 Here's an example usage of the DuckDuckGoSearchToolSpec.
 
 ```python
 from llama_index.tools.duckduckgo import DuckDuckGoSearchToolSpec
-from llama_index.agent import OpenAIAgent
+from llama_index.agent.openai import OpenAIAgent
 
 tool_spec = DuckDuckGoSearchToolSpec()
 
 agent = OpenAIAgent.from_tools(DuckDuckGoSearchToolSpec.to_tool_list())
 
 agent.chat("What's going on with the superconductor lk-99")
 agent.chat("what are the latest developments in machine learning")
```


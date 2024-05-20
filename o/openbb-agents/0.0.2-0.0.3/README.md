# Comparing `tmp/openbb_agents-0.0.2.tar.gz` & `tmp/openbb_agents-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_agents-0.0.2.tar", max compression
+gzip compressed data, was "openbb_agents-0.0.3.tar", max compression
```

## Comparing `openbb_agents-0.0.2.tar` & `openbb_agents-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4157 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/README.md
--rw-r--r--   0        0        0     1210 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/openbb_agents/__init__.py
--rw-r--r--   0        0        0    10409 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/openbb_agents/agent.py
--rw-r--r--   0        0        0     8626 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/openbb_agents/chains.py
--rw-r--r--   0        0        0      753 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/openbb_agents/models.py
--rw-r--r--   0        0        0     6496 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/openbb_agents/prompts.py
--rw-r--r--   0        0        0     1595 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/openbb_agents/testing.py
--rw-r--r--   0        0        0     4160 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/openbb_agents/tools.py
--rw-r--r--   0        0        0      506 2024-05-17 09:45:57.199595 openbb_agents-0.0.2/openbb_agents/utils.py
--rw-r--r--   0        0        0      998 2024-05-17 09:45:57.203595 openbb_agents-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5082 1970-01-01 00:00:00.000000 openbb_agents-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4153 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/README.md
+-rw-r--r--   0        0        0     1210 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/__init__.py
+-rw-r--r--   0        0        0    10409 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/agent.py
+-rw-r--r--   0        0        0     8626 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/chains.py
+-rw-r--r--   0        0        0      753 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/models.py
+-rw-r--r--   0        0        0     6496 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/prompts.py
+-rw-r--r--   0        0        0     1595 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/testing.py
+-rw-r--r--   0        0        0     4160 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/tools.py
+-rw-r--r--   0        0        0      506 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/openbb_agents/utils.py
+-rw-r--r--   0        0        0      999 2024-05-20 11:03:56.175819 openbb_agents-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5035 1970-01-01 00:00:00.000000 openbb_agents-0.0.3/PKG-INFO
```

### Comparing `openbb_agents-0.0.2/README.md` & `openbb_agents-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This is a project that leverages LLMs and [OpenBB Platform](https://github.com/OpenBB-finance/OpenBBTerminal/tree/develop/openbb_platform) to create financial
 analyst agents that can autonomously perform financial research, and answer
 questions using up-to-date data. This is possible as a result of agents
 utilizing function calling to interact with the OpenBB Platform.
 
 
 ## Installation
-Currently, we only support Python 3.11. We will be adding support for more version of Python relatively soon.
+Currently, we support Python 3.10+. We will be adding support for more version of Python relatively soon.
 
 `openbb-agents` is available as a PyPI package:
 
 ``` sh
 pip install openbb-agents --upgrade
 ```
```

### Comparing `openbb_agents-0.0.2/openbb_agents/__init__.py` & `openbb_agents-0.0.3/openbb_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.2/openbb_agents/agent.py` & `openbb_agents-0.0.3/openbb_agents/agent.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.2/openbb_agents/chains.py` & `openbb_agents-0.0.3/openbb_agents/chains.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.2/openbb_agents/models.py` & `openbb_agents-0.0.3/openbb_agents/models.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.2/openbb_agents/prompts.py` & `openbb_agents-0.0.3/openbb_agents/prompts.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.2/openbb_agents/testing.py` & `openbb_agents-0.0.3/openbb_agents/testing.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.2/openbb_agents/tools.py` & `openbb_agents-0.0.3/openbb_agents/tools.py`

 * *Files identical despite different names*

### Comparing `openbb_agents-0.0.2/pyproject.toml` & `openbb_agents-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "openbb-agents"
-version = "0.0.2"
+version = "0.0.3"
 description = "LLMs X OpenBB Platform"
 authors = ["Michael Struwig <michael.struwig@openbb.finance>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11,<3.12"
+python = ">=3.10,<3.12"
 jupyterlab = "^4.0.9"
 sentence-transformers = "^2.2.2"
 tiktoken = "^0.5.1"
 faiss-cpu = "^1.7.4"
 magentic = {extras = ["anthropic", "litellm"], version = "^0.24.0"}
 pydantic = "2.7.1"
 openbb = "4.1.7"
 langchain = "^0.1.17"
 langchain-community = "^0.0.37"
 langchain-openai = "^0.1.6"
 openbb-yfinance = "^1.1.5"
-pytest-asyncio = "^0.23.6"
-pytest-xdist = "^3.6.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.5.0"
 pytest = "^7.4.3"
+pytest-asyncio = "^0.23.6"
+pytest-xdist = "^3.6.1"
 ruff = ">=0.1.6"
 
 [tool.ruff.lint]
 select = [
     "E", # pycodestyle
     "F", # pyflakes
     "B", # flake8-bugbear
```

### Comparing `openbb_agents-0.0.2/PKG-INFO` & `openbb_agents-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: openbb-agents
-Version: 0.0.2
+Version: 0.0.3
 Summary: LLMs X OpenBB Platform
 Author: Michael Struwig
 Author-email: michael.struwig@openbb.finance
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: jupyterlab (>=4.0.9,<5.0.0)
 Requires-Dist: langchain (>=0.1.17,<0.2.0)
 Requires-Dist: langchain-community (>=0.0.37,<0.0.38)
 Requires-Dist: langchain-openai (>=0.1.6,<0.2.0)
 Requires-Dist: magentic[anthropic,litellm] (>=0.24.0,<0.25.0)
 Requires-Dist: openbb (==4.1.7)
 Requires-Dist: openbb-yfinance (>=1.1.5,<2.0.0)
 Requires-Dist: pydantic (==2.7.1)
-Requires-Dist: pytest-asyncio (>=0.23.6,<0.24.0)
-Requires-Dist: pytest-xdist (>=3.6.1,<4.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.5.1,<0.6.0)
 Description-Content-Type: text/markdown
 
 # OpenBB LLM Agents
 Work-in-progress.
 
 This is a project that leverages LLMs and [OpenBB Platform](https://github.com/OpenBB-finance/OpenBBTerminal/tree/develop/openbb_platform) to create financial
 analyst agents that can autonomously perform financial research, and answer
 questions using up-to-date data. This is possible as a result of agents
 utilizing function calling to interact with the OpenBB Platform.
 
 
 ## Installation
-Currently, we only support Python 3.11. We will be adding support for more version of Python relatively soon.
+Currently, we support Python 3.10+. We will be adding support for more version of Python relatively soon.
 
 `openbb-agents` is available as a PyPI package:
 
 ``` sh
 pip install openbb-agents --upgrade
 ```
```


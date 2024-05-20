# Comparing `tmp/bioimageio-chatbot-0.1.98.tar.gz` & `tmp/bioimageio_chatbot-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio-chatbot-0.1.98.tar", last modified: Sat Apr 13 08:11:32 2024, max compression
+gzip compressed data, was "bioimageio_chatbot-0.1.99.tar", last modified: Mon May 20 20:29:08 2024, max compression
```

## Comparing `bioimageio-chatbot-0.1.98.tar` & `bioimageio_chatbot-0.1.99.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:11:32.027685 bioimageio-chatbot-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-04-13 08:11:32.027685 bioimageio-chatbot-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:11:32.023685 bioimageio-chatbot-0.1.98/bioimageio_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20615 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:11:32.027685 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/bia_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/biii_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/docs_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/hpa_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/vision_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:11:32.027685 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/web_search_extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/gpts_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/jsonschema_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:11:32.027685 bioimageio-chatbot-0.1.98/bioimageio_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-04-13 08:11:32.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-13 08:11:32.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 08:11:32.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 08:11:32.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 08:11:32.000000 bioimageio-chatbot-0.1.98/bioimageio_chatbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 08:11:32.027685 bioimageio-chatbot-0.1.98/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:11:32.027685 bioimageio-chatbot-0.1.98/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/tests/test_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/tests/test_chatbot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/tests/test_eval_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 08:11:21.000000 bioimageio-chatbot-0.1.98/tests/test_knowledge_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:29:08.300285 bioimageio_chatbot-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-05-20 20:29:08.300285 bioimageio_chatbot-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:29:08.296285 bioimageio_chatbot-0.1.99/bioimageio_chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20615 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:29:08.300285 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/bia_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/biii_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/docs_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/hpa_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/vision_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:29:08.300285 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/web_search_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/gpts_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/jsonschema_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:29:08.300285 bioimageio_chatbot-0.1.99/bioimageio_chatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-05-20 20:29:08.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-20 20:29:08.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:29:08.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-20 20:29:08.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 20:29:08.000000 bioimageio_chatbot-0.1.99/bioimageio_chatbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:29:08.300285 bioimageio_chatbot-0.1.99/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:29:08.300285 bioimageio_chatbot-0.1.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/tests/test_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/tests/test_chatbot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/tests/test_eval_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-20 20:28:54.000000 bioimageio_chatbot-0.1.99/tests/test_knowledge_base.py
```

### Comparing `bioimageio-chatbot-0.1.98/LICENSE` & `bioimageio_chatbot-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/PKG-INFO` & `bioimageio_chatbot-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.98
+Version: 0.1.99
 Summary: Your Personal Assistant in Computational BioImaging.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: schema-agents>=0.1.49
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.98 Summary: Your
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.99 Summary: Your
 Personal Assistant in Computational BioImaging. Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.49 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
```

### Comparing `bioimageio-chatbot-0.1.98/README.md` & `bioimageio_chatbot-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/__main__.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/__main__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/__init__.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import asyncio
 import re
 import pkgutil
+import importlib.util
 from pydantic import BaseModel
 from bioimageio_chatbot.utils import ChatbotExtension
 from bioimageio_chatbot.jsonschema_pydantic import json_schema_to_pydantic_model
 from schema_agents import schema_tool
 
 def get_builtin_extensions():
     extensions = []
     for module in pkgutil.walk_packages(__path__, __name__ + '.'):
         if module.name.endswith('_extension'):
-            ext_module = module.module_finder.find_module(module.name).load_module(module.name)
+            if hasattr(module.module_finder, 'find_module'):
+                ext_module = module.module_finder.find_module(module.name).load_module(module.name)
+            else:
+                # for newer python versions, find_spec is used instead of find_module
+                module_spec = importlib.util.find_spec(module.name)
+                ext_module = importlib.util.module_from_spec(module_spec)
+                module_spec.loader.exec_module(ext_module)
             exts = ext_module.get_extension() or []
             if isinstance(exts, ChatbotExtension):
                 exts = [exts]
             for ext in exts:
                 if not isinstance(ext, ChatbotExtension):
                     print(f"Failed to load chatbot extension: {module.name}.")
                     continue
```

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/bia_extension.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/bia_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/biii_extension.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/biii_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/docs_extension.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/docs_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/hpa_extension.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/hpa_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/vision_extension.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/vision_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/evaluation.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/evaluation.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/gpts_action.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/gpts_action.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/jsonschema_pydantic.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/jsonschema_pydantic.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/knowledge_base.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/quota.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/quota.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot/utils.py` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot.egg-info/PKG-INFO` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.98
+Version: 0.1.99
 Summary: Your Personal Assistant in Computational BioImaging.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: schema-agents>=0.1.49
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.98 Summary: Your
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.99 Summary: Your
 Personal Assistant in Computational BioImaging. Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.49 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
```

### Comparing `bioimageio-chatbot-0.1.98/bioimageio_chatbot.egg-info/SOURCES.txt` & `bioimageio_chatbot-0.1.99/bioimageio_chatbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/pyproject.toml` & `bioimageio_chatbot-0.1.99/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "bioimageio-chatbot"
-version = "0.1.98"
+version = "0.1.99"
 readme = "README.md"
 description = "Your Personal Assistant in Computational BioImaging."
 dependencies = [
   "schema-agents>=0.1.49",
   "imjoy-rpc>=0.5.48.post2",
   "requests",
   "pypdf",
```

### Comparing `bioimageio-chatbot-0.1.98/tests/test_chatbot.py` & `bioimageio_chatbot-0.1.99/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/tests/test_chatbot_answer.py` & `bioimageio_chatbot-0.1.99/tests/test_chatbot_answer.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.98/tests/test_eval_agent.py` & `bioimageio_chatbot-0.1.99/tests/test_eval_agent.py`

 * *Files identical despite different names*


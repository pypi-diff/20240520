# Comparing `tmp/modelmerge-0.4.9.tar.gz` & `tmp/modelmerge-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.4.9.tar", last modified: Sun May 19 07:22:59 2024, max compression
+gzip compressed data, was "modelmerge-0.5.0.tar", last modified: Sun May 19 19:30:20 2024, max compression
```

## Comparing `modelmerge-0.4.9.tar` & `modelmerge-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.820585 modelmerge-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-19 07:22:51.000000 modelmerge-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 07:22:59.820585 modelmerge-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-19 07:22:51.000000 modelmerge-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:22:59.820585 modelmerge-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 07:22:51.000000 modelmerge-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.808585 modelmerge-0.4.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.812585 modelmerge-0.4.9/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.812585 modelmerge-0.4.9/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30492 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.812585 modelmerge-0.4.9/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.812585 modelmerge-0.4.9/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.816585 modelmerge-0.4.9/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.820585 modelmerge-0.4.9/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.820585 modelmerge-0.4.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.522075 modelmerge-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-19 19:30:12.000000 modelmerge-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 19:30:20.522075 modelmerge-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-19 19:30:12.000000 modelmerge-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:30:20.522075 modelmerge-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 19:30:12.000000 modelmerge-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.514074 modelmerge-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.514074 modelmerge-0.5.0/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.514074 modelmerge-0.5.0/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30490 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20892 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.518074 modelmerge-0.5.0/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.518074 modelmerge-0.5.0/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/tools/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/tools/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.518074 modelmerge-0.5.0/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-19 19:30:12.000000 modelmerge-0.5.0/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.522075 modelmerge-0.5.0/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 19:30:20.000000 modelmerge-0.5.0/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-19 19:30:20.000000 modelmerge-0.5.0/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:30:20.000000 modelmerge-0.5.0/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-19 19:30:20.000000 modelmerge-0.5.0/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 19:30:20.000000 modelmerge-0.5.0/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:30:20.522075 modelmerge-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_get_token_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-19 19:30:12.000000 modelmerge-0.5.0/test/test_whisper.py
```

### Comparing `modelmerge-0.4.9/LICENSE` & `modelmerge-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/PKG-INFO` & `modelmerge-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.9
+Version: 0.5.0
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.9/README.md` & `modelmerge-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.5.0/src/ModelMerge/models/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import httpx
 import requests
 import tiktoken
 
 # import config
 from ..utils.scripts import check_json, cut_message
 from ..utils.prompt import search_key_word_prompt
-from ..tools.function_call import function_call_list
+from ..tools.chatgpt import function_call_list
 from ..plugins import *
 
 def get_filtered_keys_from_object(obj: object, *keys: str) -> Set[str]:
     """
     Get filtered list of object variable names.
     :param keys: List of keys to include. If the first key is "not", the remaining keys will be removed from the class keys.
     :return: List of class keys.
@@ -380,15 +380,15 @@
             if line == "[DONE]":
                 break
             resp: dict = json.loads(line)
             # print("resp", resp)
             usage = resp.get("usage")
             if usage:
                 total_tokens = usage.get("total_tokens") or 0
-                print("total_tokens", total_tokens)
+                print("\n\rtotal_tokens", total_tokens)
             choices = resp.get("choices")
             if not choices:
                 continue
             delta = choices[0].get("delta")
             if not delta:
                 continue
             if "role" in delta and response_role == None:
```

### Comparing `modelmerge-0.4.9/src/ModelMerge/models/claude.py` & `modelmerge-0.5.0/src/ModelMerge/models/groq.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,201 +1,49 @@
-from ..tools.function_call import claude_tools_list
 import os
 import json
-import tiktoken
 import requests
+import tiktoken
 
 from .config import BaseLLM
 
-class claudeConversation(dict):
-    def Conversation(self, index):
-        conversation_list = super().__getitem__(index)
-        return "\n\n" + "\n\n".join([f"{item['role']}:{item['content']}" for item in conversation_list]) + "\n\nAssistant:"
-
-class claude(BaseLLM):
+class groq(BaseLLM):
     def __init__(
         self,
         api_key: str,
-        engine: str = os.environ.get("GPT_ENGINE") or "claude-2.1",
-        api_url: str = "https://api.anthropic.com/v1/complete",
+        engine: str = os.environ.get("GPT_ENGINE") or "llama3-70b-8192",
+        api_url: str = "https://api.groq.com/openai/v1/chat/completions",
         system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
         temperature: float = 0.5,
-        top_p: float = 0.7,
+        top_p: float = 1,
         timeout: float = 20,
     ):
         super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p)
         self.api_url = api_url
-        self.conversation = claudeConversation()
 
     def add_to_conversation(
         self,
         message: str,
         role: str,
         convo_id: str = "default",
         pass_history: bool = True,
         total_tokens: int = 0,
     ) -> None:
         """
         Add a message to the conversation
         """
-
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.conversation[convo_id].append({"role": role, "content": message})
         if total_tokens:
             self.tokens_usage[convo_id] += total_tokens
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
         """
         Reset the conversation
         """
-        self.conversation[convo_id] = claudeConversation()
-
-    def __truncate_conversation(self, convo_id: str = "default") -> None:
-        """
-        Truncate the conversation
-        """
-        while True:
-            if (
-                self.get_token_count(convo_id) > self.truncate_limit
-                and len(self.conversation[convo_id]) > 1
-            ):
-                # Don't remove the first message
-                self.conversation[convo_id].pop(1)
-            else:
-                break
-
-    def get_token_count(self, convo_id: str = "default") -> int:
-        """
-        Get token count
-        """
-        tiktoken.model.MODEL_TO_ENCODING["claude-2.1"] = "cl100k_base"
-        encoding = tiktoken.encoding_for_model(self.engine)
-
-        num_tokens = 0
-        for message in self.conversation[convo_id]:
-            # every message follows <im_start>{role/name}\n{content}<im_end>\n
-            num_tokens += 5
-            for key, value in message.items():
-                if value:
-                    num_tokens += len(encoding.encode(value))
-                if key == "name":  # if there's a name, the role is omitted
-                    num_tokens += 5  # role is always required and always 1 token
-        num_tokens += 5  # every reply is primed with <im_start>assistant
-        return num_tokens
-
-    def ask_stream(
-        self,
-        prompt: str,
-        role: str = "Human",
-        convo_id: str = "default",
-        model: str = None,
-        pass_history: bool = True,
-        model_max_tokens: int = 4096,
-        **kwargs,
-    ):
-        pass_history = True
-        if convo_id not in self.conversation or pass_history == False:
-            self.reset(convo_id=convo_id)
-        self.add_to_conversation(prompt, role, convo_id=convo_id)
-        # self.__truncate_conversation(convo_id=convo_id)
-        # print(self.conversation[convo_id])
-
-        url = self.api_url
-        headers = {
-            "accept": "application/json",
-            "anthropic-version": "2023-06-01",
-            "content-type": "application/json",
-            "x-api-key": f"{kwargs.get('api_key', self.api_key)}",
-        }
-
-        json_post = {
-            "model": model or self.engine,
-            "prompt": self.conversation.Conversation(convo_id) if pass_history else f"\n\nHuman:{prompt}\n\nAssistant:",
-            "stream": True,
-            "temperature": kwargs.get("temperature", self.temperature),
-            "top_p": kwargs.get("top_p", self.top_p),
-            "max_tokens_to_sample": model_max_tokens,
-        }
-
-        try:
-            response = self.session.post(
-                url,
-                headers=headers,
-                json=json_post,
-                timeout=kwargs.get("timeout", self.timeout),
-                stream=True,
-            )
-        except ConnectionError:
-            print("连接错误，请检查服务器状态或网络连接。")
-            return
-        except requests.exceptions.ReadTimeout:
-            print("请求超时，请检查网络连接或增加超时时间。{e}")
-            return
-        except Exception as e:
-            print(f"发生了未预料的错误: {e}")
-            return
-
-        if response.status_code != 200:
-            print(response.text)
-            raise BaseException(f"{response.status_code} {response.reason} {response.text}")
-        response_role: str = "Assistant"
-        full_response: str = ""
-        for line in response.iter_lines():
-            if not line or line.decode("utf-8") == "event: completion" or line.decode("utf-8") == "event: ping" or line.decode("utf-8") == "data: {}":
-                continue
-            line = line.decode("utf-8")[6:]
-            # print(line)
-            resp: dict = json.loads(line)
-            content = resp.get("completion")
-            if content:
-                full_response += content
-                yield content
-        self.add_to_conversation(full_response, response_role, convo_id=convo_id)
-
-class claude3(BaseLLM):
-    def __init__(
-        self,
-        api_key: str,
-        engine: str = os.environ.get("GPT_ENGINE") or "claude-3-opus-20240229",
-        api_url: str = "https://api.anthropic.com/v1/messages",
-        system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
-        temperature: float = 0.5,
-        timeout: float = 20,
-        top_p: float = 0.7,
-    ):
-        super().__init__(api_key, engine, api_url, system_prompt, timeout=timeout, temperature=temperature, top_p=top_p)
-        self.api_url = api_url
-        self.conversation: dict[str, list[dict]] = {
-            "default": [],
-        }
-
-    def add_to_conversation(
-        self,
-        message: str,
-        role: str,
-        convo_id: str = "default",
-        pass_history: bool = True,
-    ) -> None:
-        """
-        Add a message to the conversation
-        """
-
-        if convo_id not in self.conversation or pass_history == False:
-            self.reset(convo_id=convo_id)
-        self.conversation[convo_id].append({"role": role, "content": message})
-        index = len(self.conversation[convo_id]) - 2
-        if index >= 0 and self.conversation[convo_id][index]["role"] == self.conversation[convo_id][index + 1]["role"]:
-            self.conversation[convo_id][index]["content"] += self.conversation[convo_id][index + 1]["content"]
-            self.conversation[convo_id].pop(index + 1)
-
-    def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
-        """
-        Reset the conversation
-        """
         self.conversation[convo_id] = list()
 
     def __truncate_conversation(self, convo_id: str = "default") -> None:
         """
         Truncate the conversation
         """
         while True:
@@ -208,16 +56,16 @@
             else:
                 break
 
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
-        tiktoken.model.MODEL_TO_ENCODING["claude-2.1"] = "cl100k_base"
-        encoding = tiktoken.encoding_for_model(self.engine)
+        # tiktoken.model.MODEL_TO_ENCODING["mixtral-8x7b-32768"] = "cl100k_base"
+        encoding = tiktoken.get_encoding("cl100k_base")
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             num_tokens += 5
             for key, value in message.items():
                 if value:
@@ -230,47 +78,44 @@
     def ask_stream(
         self,
         prompt: str,
         role: str = "user",
         convo_id: str = "default",
         model: str = None,
         pass_history: bool = True,
-        model_max_tokens: int = 4096,
+        model_max_tokens: int = 1024,
         **kwargs,
     ):
         pass_history = True
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.add_to_conversation(prompt, role, convo_id=convo_id)
         # self.__truncate_conversation(convo_id=convo_id)
         # print(self.conversation[convo_id])
 
         url = self.api_url
         headers = {
-            "x-api-key": f"{kwargs.get('api_key', self.api_key)}",
-            "anthropic-version": "2023-06-01",
-            "content-type": "application/json",
-            # "anthropic-beta": "tools-2024-04-04"
+            "Authorization": f"Bearer {kwargs.get('GROQ_API_KEY', self.api_key)}",
+            "Content-Type": "application/json",
         }
 
         json_post = {
-            "model": model or self.engine,
             "messages": self.conversation[convo_id] if pass_history else [{
                 "role": "user",
                 "content": prompt
             }],
+            "model": model or self.engine,
             "temperature": kwargs.get("temperature", self.temperature),
-            "top_p": kwargs.get("top_p", self.top_p),
             "max_tokens": model_max_tokens,
+            "top_p": kwargs.get("top_p", self.top_p),
+            "stop": None,
             "stream": True,
         }
-        if self.system_prompt:
-            json_post["system"] = self.system_prompt
-
-        print(json.dumps(json_post, indent=4, ensure_ascii=False))
+        # print("json_post", json_post)
+        # print(os.environ.get("GPT_ENGINE"), model, self.engine)
 
         try:
             response = self.session.post(
                 url,
                 headers=headers,
                 json=json_post,
                 timeout=kwargs.get("timeout", self.timeout),
@@ -288,25 +133,35 @@
 
         if response.status_code != 200:
             print(response.text)
             raise BaseException(f"{response.status_code} {response.reason} {response.text}")
         response_role: str = "assistant"
         full_response: str = ""
         for line in response.iter_lines():
-            if not line or line.decode("utf-8")[:6] == "event:" or line.decode("utf-8") == "data: {}":
+            if not line:
                 continue
+            # Remove "data: "
             # print(line.decode("utf-8"))
-            # if "tool_use" in line.decode("utf-8"):
-            #     tool_input = json.loads(line.decode("utf-8")["content"][1]["input"])
-            # else:
-            #     line = line.decode("utf-8")[6:]
-            line = line.decode("utf-8")[6:]
-            # print(line)
+            if line.decode("utf-8")[:6] == "data: ":
+                line = line.decode("utf-8")[6:]
+            else:
+                print(line.decode("utf-8"))
+                full_response = json.loads(line.decode("utf-8"))["choices"][0]["message"]["content"]
+                yield full_response
+                break
+            if line == "[DONE]":
+                break
             resp: dict = json.loads(line)
-            delta = resp.get("delta")
+            # print("resp", resp)
+            choices = resp.get("choices")
+            if not choices:
+                continue
+            delta = choices[0].get("delta")
             if not delta:
                 continue
-            if "text" in delta:
-                content = delta["text"]
+            if "role" in delta:
+                response_role = delta["role"]
+            if "content" in delta and delta["content"]:
+                content = delta["content"]
                 full_response += content
                 yield content
         self.add_to_conversation(full_response, response_role, convo_id=convo_id)
```

### Comparing `modelmerge-0.4.9/src/ModelMerge/models/config.py` & `modelmerge-0.5.0/src/ModelMerge/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import json
 import httpx
 import requests
 from pathlib import Path
+from collections import defaultdict
+
 
 from ..utils import prompt
 
 PLUGINS = {
     "SEARCH": (os.environ.get('SEARCH', "True") == "False") == False,
     "URL": True,
     "CODE": True,
@@ -38,29 +40,29 @@
         self.image_url: str = urlunparse(parsed_url[:2] + (before_v1 + "/v1/images/generations",) + ("",) * 3)
 
 class BaseLLM:
     def __init__(
         self,
         api_key: str,
         engine: str = os.environ.get("GPT_ENGINE") or "gpt-3.5-turbo",
-        api_url: str = (os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions"),
+        api_url: str = (os.environ.get("API_URL", None) or "https://api.openai.com/v1/chat/completions"),
         system_prompt: str = prompt.chatgpt_system_prompt,
         proxy: str = None,
         timeout: float = 600,
         max_tokens: int = None,
         temperature: float = 0.5,
         top_p: float = 1.0,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         reply_count: int = 1,
         truncate_limit: int = None,
     ) -> None:
         self.api_key: str = api_key
         self.engine: str = engine
-        self.api_url: str = BaseAPI(api_url)
+        self.api_url: str = BaseAPI(api_url or "https://api.openai.com/v1/chat/completions")
         self.system_prompt: str = system_prompt
         self.max_tokens: int = max_tokens
         self.truncate_limit: int = truncate_limit
         self.temperature: float = temperature
         self.top_p: float = top_p
         self.presence_penalty: float = presence_penalty
         self.frequency_penalty: float = frequency_penalty
@@ -94,17 +96,15 @@
             "default": [
                 {
                     "role": "system",
                     "content": system_prompt,
                 },
             ],
         }
-        self.tokens_usage = {
-            "default": 0,
-        }
+        self.tokens_usage = defaultdict(int)
         self.function_calls_counter = {}
         self.function_call_max_loop = 10
 
     def add_to_conversation(
         self,
         message: list,
         role: str,
@@ -144,15 +144,14 @@
         Get token count
         """
         pass
 
     def get_message_token(self, url, json_post):
         pass
 
-
     def get_post_body(
         self,
         prompt: str,
         role: str = "user",
         convo_id: str = "default",
         model: str = None,
         pass_history: bool = True,
```

### Comparing `modelmerge-0.4.9/src/ModelMerge/models/genimi.py` & `modelmerge-0.5.0/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/src/ModelMerge/plugins/image.py` & `modelmerge-0.5.0/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.5.0/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.5.0/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/src/ModelMerge/utils/prompt.py` & `modelmerge-0.5.0/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/src/ModelMerge/utils/scripts.py` & `modelmerge-0.5.0/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.5.0/src/modelmerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.9
+Version: 0.5.0
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.9/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.5.0/src/modelmerge.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 src/ModelMerge/plugins/image.py
 src/ModelMerge/plugins/run_python.py
 src/ModelMerge/plugins/tarvel.py
 src/ModelMerge/plugins/today.py
 src/ModelMerge/plugins/version.py
 src/ModelMerge/plugins/websearch.py
 src/ModelMerge/tools/__init__.py
-src/ModelMerge/tools/function_call.py
+src/ModelMerge/tools/chatgpt.py
+src/ModelMerge/tools/claude.py
 src/ModelMerge/utils/__init__.py
 src/ModelMerge/utils/prompt.py
 src/ModelMerge/utils/scripts.py
 src/modelmerge.egg-info/PKG-INFO
 src/modelmerge.egg-info/SOURCES.txt
 src/modelmerge.egg-info/dependency_links.txt
 src/modelmerge.egg-info/requires.txt
 src/modelmerge.egg-info/top_level.txt
 test/test.py
 test/test_API.py
 test/test_Web_crawler.py
 test/test_claude_zh_char.py
 test/test_ddg_search.py
 test/test_download_pdf.py
+test/test_get_token_dict.py
 test/test_google_search.py
 test/test_jieba.py
 test/test_json.py
 test/test_langchain_search_old.py
 test/test_logging.py
 test/test_ollama.py
 test/test_py_run.py
```

### Comparing `modelmerge-0.4.9/test/test_Web_crawler.py` & `modelmerge-0.5.0/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_claude_zh_char.py` & `modelmerge-0.5.0/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_ddg_search.py` & `modelmerge-0.5.0/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_download_pdf.py` & `modelmerge-0.5.0/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_google_search.py` & `modelmerge-0.5.0/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_jieba.py` & `modelmerge-0.5.0/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_json.py` & `modelmerge-0.5.0/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_langchain_search_old.py` & `modelmerge-0.5.0/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_logging.py` & `modelmerge-0.5.0/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_ollama.py` & `modelmerge-0.5.0/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_py_run.py` & `modelmerge-0.5.0/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_tikitoken.py` & `modelmerge-0.5.0/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_token.py` & `modelmerge-0.5.0/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.9/test/test_url.py` & `modelmerge-0.5.0/test/test_url.py`

 * *Files identical despite different names*


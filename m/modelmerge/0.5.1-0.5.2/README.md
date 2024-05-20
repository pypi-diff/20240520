# Comparing `tmp/modelmerge-0.5.1.tar.gz` & `tmp/modelmerge-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.5.1.tar", last modified: Mon May 20 04:14:41 2024, max compression
+gzip compressed data, was "modelmerge-0.5.2.tar", last modified: Mon May 20 05:14:34 2024, max compression
```

## Comparing `modelmerge-0.5.1.tar` & `modelmerge-0.5.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.395236 modelmerge-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-20 04:14:31.000000 modelmerge-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-20 04:14:41.395236 modelmerge-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-20 04:14:31.000000 modelmerge-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 04:14:41.395236 modelmerge-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-20 04:14:31.000000 modelmerge-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.387236 modelmerge-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.387236 modelmerge-0.5.1/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.391236 modelmerge-0.5.1/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30646 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20892 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.391236 modelmerge-0.5.1/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.391236 modelmerge-0.5.1/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/tools/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/tools/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.391236 modelmerge-0.5.1/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-20 04:14:31.000000 modelmerge-0.5.1/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.395236 modelmerge-0.5.1/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-20 04:14:41.000000 modelmerge-0.5.1/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-20 04:14:41.000000 modelmerge-0.5.1/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 04:14:41.000000 modelmerge-0.5.1/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 04:14:41.000000 modelmerge-0.5.1/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 04:14:41.000000 modelmerge-0.5.1/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:14:41.395236 modelmerge-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_get_token_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-20 04:14:31.000000 modelmerge-0.5.1/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.625359 modelmerge-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-20 05:14:26.000000 modelmerge-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-20 05:14:34.625359 modelmerge-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-20 05:14:26.000000 modelmerge-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:14:34.625359 modelmerge-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-20 05:14:26.000000 modelmerge-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.617359 modelmerge-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.617359 modelmerge-0.5.2/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.617359 modelmerge-0.5.2/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31053 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20892 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.621359 modelmerge-0.5.2/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.621359 modelmerge-0.5.2/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/tools/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/tools/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.621359 modelmerge-0.5.2/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-20 05:14:26.000000 modelmerge-0.5.2/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.625359 modelmerge-0.5.2/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-20 05:14:34.000000 modelmerge-0.5.2/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-20 05:14:34.000000 modelmerge-0.5.2/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:14:34.000000 modelmerge-0.5.2/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 05:14:34.000000 modelmerge-0.5.2/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 05:14:34.000000 modelmerge-0.5.2/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:14:34.625359 modelmerge-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_get_token_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-20 05:14:26.000000 modelmerge-0.5.2/test/test_whisper.py
```

### Comparing `modelmerge-0.5.1/LICENSE` & `modelmerge-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/PKG-INFO` & `modelmerge-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.1
+Version: 0.5.2
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.1/README.md` & `modelmerge-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.5.2/src/ModelMerge/models/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,14 +350,21 @@
                 return
             except Exception as e:
                 print(f"发生了未预料的错误: {e}")
                 return
             # print("response.text", response.text)
             if response.status_code == 400:
                 print("response.text", response.text)
+                if "invalid_request_error" in response.text:
+                    for index, mess in enumerate(json_post["messages"]):
+                        if type(mess["content"]) == list:
+                            json_post["messages"][index] = {
+                                "role": mess["role"],
+                                "content": mess["content"][0]["text"]
+                            }
                 if "function_call" in json_post:
                     del json_post["function_call"]
                 if "functions" in json_post:
                     del json_post["functions"]
                 continue
             if response.status_code == 200:
                 break
```

### Comparing `modelmerge-0.5.1/src/ModelMerge/models/claude.py` & `modelmerge-0.5.2/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/models/config.py` & `modelmerge-0.5.2/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/models/genimi.py` & `modelmerge-0.5.2/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/models/groq.py` & `modelmerge-0.5.2/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/plugins/image.py` & `modelmerge-0.5.2/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.5.2/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.5.2/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/tools/chatgpt.py` & `modelmerge-0.5.2/src/ModelMerge/tools/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/tools/claude.py` & `modelmerge-0.5.2/src/ModelMerge/tools/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/utils/prompt.py` & `modelmerge-0.5.2/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/ModelMerge/utils/scripts.py` & `modelmerge-0.5.2/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.5.2/src/modelmerge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.5.1
+Version: 0.5.2
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.5.1/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.5.2/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_Web_crawler.py` & `modelmerge-0.5.2/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_claude_zh_char.py` & `modelmerge-0.5.2/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_ddg_search.py` & `modelmerge-0.5.2/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_download_pdf.py` & `modelmerge-0.5.2/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_get_token_dict.py` & `modelmerge-0.5.2/test/test_get_token_dict.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_google_search.py` & `modelmerge-0.5.2/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_jieba.py` & `modelmerge-0.5.2/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_json.py` & `modelmerge-0.5.2/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_langchain_search_old.py` & `modelmerge-0.5.2/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_logging.py` & `modelmerge-0.5.2/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_ollama.py` & `modelmerge-0.5.2/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_py_run.py` & `modelmerge-0.5.2/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_tikitoken.py` & `modelmerge-0.5.2/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_token.py` & `modelmerge-0.5.2/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.5.1/test/test_url.py` & `modelmerge-0.5.2/test/test_url.py`

 * *Files identical despite different names*


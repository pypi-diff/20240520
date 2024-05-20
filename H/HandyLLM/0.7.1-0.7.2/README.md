# Comparing `tmp/handyllm-0.7.1.tar.gz` & `tmp/handyllm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handyllm-0.7.1.tar", last modified: Tue May  7 12:11:44 2024, max compression
+gzip compressed data, was "handyllm-0.7.2.tar", last modified: Mon May 20 09:17:42 2024, max compression
```

## Comparing `handyllm-0.7.1.tar` & `handyllm-0.7.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:11:44.402380 handyllm-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 12:11:44.402380 handyllm-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-07 12:11:39.000000 handyllm-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 12:11:39.000000 handyllm-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 12:11:44.402380 handyllm-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:11:44.398380 handyllm-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:11:44.402380 handyllm-0.7.1/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 12:11:44.000000 handyllm-0.7.1/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-07 12:11:44.000000 handyllm-0.7.1/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:11:44.000000 handyllm-0.7.1/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 12:11:44.000000 handyllm-0.7.1/src/HandyLLM.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 12:11:44.000000 handyllm-0.7.1/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 12:11:44.000000 handyllm-0.7.1/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:11:44.402380 handyllm-0.7.1/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/_str_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:11:44.402380 handyllm-0.7.1/src/handyllm/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/deprecated/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/deprecated/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    32619 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/hprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-07 12:11:39.000000 handyllm-0.7.1/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:11:44.402380 handyllm-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-07 12:11:39.000000 handyllm-0.7.1/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-07 12:11:39.000000 handyllm-0.7.1/tests/test_client_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-07 12:11:39.000000 handyllm-0.7.1/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-07 12:11:39.000000 handyllm-0.7.1/tests/test_hprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 12:11:39.000000 handyllm-0.7.1/tests/test_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 09:17:32.000000 handyllm-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-20 09:17:42.248525 handyllm-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-20 09:17:32.000000 handyllm-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 09:17:32.000000 handyllm-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:17:42.248525 handyllm-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.244525 handyllm-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/_str_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/src/handyllm/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/deprecated/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/deprecated/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32490 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_client_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_prompt.py
```

### Comparing `handyllm-0.7.1/PKG-INFO` & `handyllm-0.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.7.1
+Version: 0.7.2
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: httpx
 Requires-Dist: python-frontmatter
 Requires-Dist: mergedeep
 Requires-Dist: python-dotenv
 Requires-Dist: PyYAML
 
@@ -34,17 +35,18 @@
 📃 **Handy Prompt**: self-containing prompt in a human-friendly mark-up format `.hprompt`. 
 
 - **Easy write**: mark-up format, placeholder variables, request arguments, output logs... And most importantly VSCode syntax highlight!
 - **Easy run**: both CLI and APIs available for parsing and running; run it with the CLI tool *WITHOUT* any code! 
 - **Easy chain**: You can chain `hprompt` files to construct dynamic logic.
 
 <p float="left" align="center">
-  <img src="https://raw.githubusercontent.com/atomiechen/vscode-handyllm/main/demo/example.jpg" width="60%" />
+  <img src="https://raw.githubusercontent.com/atomiechen/vscode-handyllm/main/demo/example.png" width="70%" />
 </p>
 
+
 **Other features:**
 
 ☯️ Unified API design with both sync and async support
 
 🍡 OpenAI and Azure APIs all in one
 
 ☕️ Easy life with API endpoint management
@@ -67,7 +69,13 @@
 
 
 
 ## Documentation
 
 Please check out our [wiki](https://github.com/atomiechen/HandyLLM/wiki) for comprehensive guides ^_^
 
+
+
+## License
+
+[HandyLLM](https://github.com/atomiechen/HandyLLM) © 2024 by [Atomie CHEN](https://github.com/atomiechen) is licensed under the MIT License - see the [LICENSE](https://github.com/atomiechen/HandyLLM/blob/main/LICENSE) file for details.
+
```

### Comparing `handyllm-0.7.1/README.md` & `handyllm-0.7.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 📃 **Handy Prompt**: self-containing prompt in a human-friendly mark-up format `.hprompt`. 
 
 - **Easy write**: mark-up format, placeholder variables, request arguments, output logs... And most importantly VSCode syntax highlight!
 - **Easy run**: both CLI and APIs available for parsing and running; run it with the CLI tool *WITHOUT* any code! 
 - **Easy chain**: You can chain `hprompt` files to construct dynamic logic.
 
 <p float="left" align="center">
-  <img src="https://raw.githubusercontent.com/atomiechen/vscode-handyllm/main/demo/example.jpg" width="60%" />
+  <img src="https://raw.githubusercontent.com/atomiechen/vscode-handyllm/main/demo/example.png" width="70%" />
 </p>
 
+
 **Other features:**
 
 ☯️ Unified API design with both sync and async support
 
 🍡 OpenAI and Azure APIs all in one
 
 ☕️ Easy life with API endpoint management
@@ -48,7 +49,13 @@
 
 
 
 ## Documentation
 
 Please check out our [wiki](https://github.com/atomiechen/HandyLLM/wiki) for comprehensive guides ^_^
 
+
+
+## License
+
+[HandyLLM](https://github.com/atomiechen/HandyLLM) © 2024 by [Atomie CHEN](https://github.com/atomiechen) is licensed under the MIT License - see the [LICENSE](https://github.com/atomiechen/HandyLLM/blob/main/LICENSE) file for details.
+
```

### Comparing `handyllm-0.7.1/pyproject.toml` & `handyllm-0.7.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `handyllm-0.7.1/src/HandyLLM.egg-info/PKG-INFO` & `handyllm-0.7.2/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.7.1
+Version: 0.7.2
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: httpx
 Requires-Dist: python-frontmatter
 Requires-Dist: mergedeep
 Requires-Dist: python-dotenv
 Requires-Dist: PyYAML
 
@@ -34,17 +35,18 @@
 📃 **Handy Prompt**: self-containing prompt in a human-friendly mark-up format `.hprompt`. 
 
 - **Easy write**: mark-up format, placeholder variables, request arguments, output logs... And most importantly VSCode syntax highlight!
 - **Easy run**: both CLI and APIs available for parsing and running; run it with the CLI tool *WITHOUT* any code! 
 - **Easy chain**: You can chain `hprompt` files to construct dynamic logic.
 
 <p float="left" align="center">
-  <img src="https://raw.githubusercontent.com/atomiechen/vscode-handyllm/main/demo/example.jpg" width="60%" />
+  <img src="https://raw.githubusercontent.com/atomiechen/vscode-handyllm/main/demo/example.png" width="70%" />
 </p>
 
+
 **Other features:**
 
 ☯️ Unified API design with both sync and async support
 
 🍡 OpenAI and Azure APIs all in one
 
 ☕️ Easy life with API endpoint management
@@ -67,7 +69,13 @@
 
 
 
 ## Documentation
 
 Please check out our [wiki](https://github.com/atomiechen/HandyLLM/wiki) for comprehensive guides ^_^
 
+
+
+## License
+
+[HandyLLM](https://github.com/atomiechen/HandyLLM) © 2024 by [Atomie CHEN](https://github.com/atomiechen) is licensed under the MIT License - see the [LICENSE](https://github.com/atomiechen/HandyLLM/blob/main/LICENSE) file for details.
+
```

### Comparing `handyllm-0.7.1/src/HandyLLM.egg-info/SOURCES.txt` & `handyllm-0.7.2/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 src/HandyLLM.egg-info/PKG-INFO
 src/HandyLLM.egg-info/SOURCES.txt
 src/HandyLLM.egg-info/dependency_links.txt
 src/HandyLLM.egg-info/entry_points.txt
 src/HandyLLM.egg-info/requires.txt
```

### Comparing `handyllm-0.7.1/src/handyllm/_str_enum.py` & `handyllm-0.7.2/src/handyllm/_str_enum.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/src/handyllm/_utils.py` & `handyllm-0.7.2/src/handyllm/_utils.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/src/handyllm/cli.py` & `handyllm-0.7.2/src/handyllm/cli.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/src/handyllm/deprecated/api_request.py` & `handyllm-0.7.2/src/handyllm/deprecated/api_request.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/src/handyllm/deprecated/openai_api.py` & `handyllm-0.7.2/src/handyllm/deprecated/openai_api.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/src/handyllm/endpoint_manager.py` & `handyllm-0.7.2/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/src/handyllm/hprompt.py` & `handyllm-0.7.2/src/handyllm/hprompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 import frontmatter
 from mergedeep import merge, Strategy
 from dotenv import load_dotenv
 
 from .prompt_converter import PromptConverter
 from .openai_client import ClientMode, OpenAIClient
 from .utils import (
-    astream_chat_with_role, astream_completions, 
-    stream_chat_with_role, stream_completions, 
+    astream_chat_all, astream_completions, 
+    stream_chat_all, stream_completions, 
 )
 from ._str_enum import AutoStrEnum
 
 
 PromptType = TypeVar('PromptType', bound='HandyPrompt')
 PathType = Union[str, os.PathLike[str]]
 
@@ -278,23 +278,26 @@
     
     TEMPLATE_OUTPUT_FILENAME = "result.%Y%m%d-%H%M%S.hprompt"
     TEMPLATE_OUTPUT_EVAL_FILENAME = "evaled.%Y%m%d-%H%M%S.hprompt"
     
     def __init__(
         self, data: Union[str, list], request: Optional[dict] = None, 
         meta: Optional[Union[dict, RunConfig]] = None, 
-        base_path: Optional[PathType] = None):
+        base_path: Optional[PathType] = None,
+        response: Optional[dict] = None,
+        ):
         self.data = data
         self.request = request or {}
         # parse meta to run_config
         if isinstance(meta, RunConfig):
             self.run_config = meta
         else:
             self.run_config = RunConfig.from_dict(meta or {}, base_path=base_path)
         self.base_path = base_path
+        self.response = response
     
     def __str__(self) -> str:
         return str(self.data)
     
     def __repr__(self) -> str:
         return "{}({}, {}, {})".format(
             self.__class__.__name__,
@@ -550,16 +553,20 @@
                 strategy=Strategy.REPLACE
             )
         return var_map
 
 
 class ChatPrompt(HandyPrompt):
         
-    def __init__(self, chat: list, request: dict, meta: Union[dict, RunConfig], base_path: Optional[PathType] = None):
-        super().__init__(chat, request, meta, base_path)
+    def __init__(
+        self, chat: list, request: dict, meta: Union[dict, RunConfig], 
+        base_path: Optional[PathType] = None,
+        response: Optional[dict] = None,
+        ):
+        super().__init__(chat, request, meta, base_path, response)
     
     @property
     def chat(self) -> list:
         return self.data
     
     @chat.setter
     def chat(self, value: list):
@@ -578,28 +585,14 @@
         var_map = self._parse_var_map(run_config)
         if var_map:
             return converter.chat_replace_variables(
                 self.chat, var_map, inplace=False)
         else:
             return self.chat
     
-    def _stream_chat_proc(self, response, fd: Optional[io.IOBase] = None) -> tuple[str, str]:
-        # stream response to fd
-        role = ""
-        content = ""
-        for r, text in stream_chat_with_role(response):
-            if r != role:
-                role = r
-                if fd:
-                    fd.write(f"${role}$\n")
-            elif fd:
-                fd.write(text)
-            content += text
-        return role, content
-    
     def _run_with_client(
         self, client: OpenAIClient, 
         run_config: RunConfig,
         new_request: dict,
         stream: bool,
         ) -> ChatPrompt:
         response = client.chat(
@@ -610,44 +603,32 @@
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     # dump frontmatter
                     fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
-                    role, content = self._stream_chat_proc(response, fout)
+                    role, content, tool_calls = converter.stream_chat2raw(stream_chat_all(response), fout)
             elif run_config.output_fd:
                 # dump frontmatter, no base_path
                 run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
                 # stream response to a file descriptor
-                role, content = self._stream_chat_proc(response, run_config.output_fd)
+                role, content, tool_calls = converter.stream_chat2raw(stream_chat_all(response), run_config.output_fd)
             else:
-                role, content = self._stream_chat_proc(response)
+                role, content, tool_calls = converter.stream_chat2raw(stream_chat_all(response))
         else:
             role = response['choices'][0]['message']['role']
-            content = response['choices'][0]['message']['content']
+            content = response['choices'][0]['message'].get('content')
+            tool_calls = response['choices'][0]['message'].get('tool_calls')
         return ChatPrompt(
-            [{"role": role, "content": content}],
-            new_request, run_config, base_path
+            [{"role": role, "content": content, "tool_calls": tool_calls}],
+            new_request, run_config, base_path,
+            response=response
         )
     
-    async def _astream_chat_proc(self, response, fd: Optional[io.IOBase] = None) -> tuple[str, str]:
-        # stream response to fd
-        role = ""
-        content = ""
-        async for r, text in astream_chat_with_role(response):
-            if r != role:
-                role = r
-                if fd:
-                    fd.write(f"${role}$\n")
-            elif fd:
-                fd.write(text)
-            content += text
-        return role, content
-    
     async def _arun_with_client(
         self, client: OpenAIClient, 
         run_config: RunConfig,
         new_request: dict,
         stream: bool,
         ) -> ChatPrompt:
         response = await client.chat(
@@ -657,27 +638,29 @@
         new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
-                    role, content = await self._astream_chat_proc(response, fout)
+                    role, content, tool_calls = await converter.astream_chat2raw(astream_chat_all(response), fout)
             elif run_config.output_fd:
                 # stream response to a file descriptor
                 run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
-                role, content = await self._astream_chat_proc(response, run_config.output_fd)
+                role, content, tool_calls = await converter.astream_chat2raw(astream_chat_all(response), run_config.output_fd)
             else:
-                role, content = await self._astream_chat_proc(response)
+                role, content, tool_calls = await converter.astream_chat2raw(astream_chat_all(response))
         else:
             role = response['choices'][0]['message']['role']
-            content = response['choices'][0]['message']['content']
+            content = response['choices'][0]['message'].get('content')
+            tool_calls = response['choices'][0]['message'].get('tool_calls')
         return ChatPrompt(
-            [{"role": role, "content": content}],
-            new_request, run_config, base_path
+            [{"role": role, "content": content, "tool_calls": tool_calls}],
+            new_request, run_config, base_path,
+            response=response
         )
 
     def __add__(self, other: Union[str, list, ChatPrompt]):
         # support concatenation with string, list or another ChatPrompt
         if isinstance(other, str):
             return ChatPrompt(
                 self.chat + [{"role": "user", "content": other}],
@@ -715,16 +698,20 @@
         else:
             raise TypeError(f"unsupported operand type(s) for +: 'ChatPrompt' and '{type(other)}'")
         return self
 
 
 class CompletionsPrompt(HandyPrompt):
     
-    def __init__(self, prompt: str, request: dict, meta: Union[dict, RunConfig], base_path: PathType = None):
-        super().__init__(prompt, request, meta, base_path)
+    def __init__(
+        self, prompt: str, request: dict, meta: Union[dict, RunConfig], 
+        base_path: PathType = None,
+        response: Optional[dict] = None,
+        ):
+        super().__init__(prompt, request, meta, base_path, response)
     
     @property
     def prompt(self) -> str:
         return self.data
     
     @prompt.setter
     def prompt(self, value: str):
@@ -771,15 +758,17 @@
                 # stream response to a file descriptor
                 run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
                 content = self._stream_completions_proc(response, run_config.output_fd)
             else:
                 content = self._stream_completions_proc(response)
         else:
             content = response['choices'][0]['text']
-        return CompletionsPrompt(content, new_request, run_config, base_path)
+        return CompletionsPrompt(
+            content, new_request, run_config, base_path, response=response
+            )
 
     async def _astream_completions_proc(self, response, fd: Optional[io.IOBase] = None) -> str:
         # stream response to fd
         content = ""
         async for text in astream_completions(response):
             if fd:
                 fd.write(text)
@@ -808,15 +797,17 @@
                 # stream response to a file descriptor
                 run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
                 content = await self._astream_completions_proc(response, run_config.output_fd)
             else:
                 content = await self._astream_completions_proc(response)
         else:
             content = response['choices'][0]['text']
-        return CompletionsPrompt(content, new_request, run_config, base_path)
+        return CompletionsPrompt(
+            content, new_request, run_config, base_path, response=response
+            )
     
     def __add__(self, other: Union[str, CompletionsPrompt]):
         # support concatenation with string or another CompletionsPrompt
         if isinstance(other, str):
             return CompletionsPrompt(
                 self.prompt + other,
                 copy.deepcopy(self.request),
```

### Comparing `handyllm-0.7.1/src/handyllm/openai_api.py` & `handyllm-0.7.2/src/handyllm/openai_api.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/src/handyllm/openai_client.py` & `handyllm-0.7.2/src/handyllm/openai_client.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/src/handyllm/requestor.py` & `handyllm-0.7.2/src/handyllm/requestor.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/tests/test_azure.py` & `handyllm-0.7.2/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/tests/test_client_async_sync.py` & `handyllm-0.7.2/tests/test_client_async_sync.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/tests/test_endpoint.py` & `handyllm-0.7.2/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/tests/test_hprompt.py` & `handyllm-0.7.2/tests/test_hprompt.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.1/tests/test_prompt.py` & `handyllm-0.7.2/tests/test_prompt.py`

 * *Files identical despite different names*


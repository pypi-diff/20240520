# Comparing `tmp/easytl-0.3.3.tar.gz` & `tmp/easytl-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.3.3.tar", last modified: Tue May 14 00:05:39 2024, max compression
+gzip compressed data, was "easytl-0.4.0a0.tar", last modified: Mon May 20 01:57:41 2024, max compression
```

## Comparing `easytl-0.3.3.tar` & `easytl-0.4.0a0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.431685 easytl-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.423685 easytl-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.427685 easytl-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-14 00:04:12.000000 easytl-0.3.3/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-14 00:04:12.000000 easytl-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-14 00:04:12.000000 easytl-0.3.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-14 00:05:39.431685 easytl-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-14 00:04:12.000000 easytl-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-14 00:04:12.000000 easytl-0.3.3/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 00:04:12.000000 easytl-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 00:05:39.431685 easytl-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.423685 easytl-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.427685 easytl-0.3.3/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16049 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/anthropic_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    71506 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/googletl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    27077 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-14 00:04:12.000000 easytl-0.3.3/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.431685 easytl-0.3.3/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 00:05:39.000000 easytl-0.3.3/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:05:39.427685 easytl-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-14 00:04:12.000000 easytl-0.3.3/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-14 00:04:12.000000 easytl-0.3.3/tests/passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:57:41.422955 easytl-0.4.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:57:41.418955 easytl-0.4.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:57:41.418955 easytl-0.4.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-20 01:55:52.000000 easytl-0.4.0a0/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-20 01:55:52.000000 easytl-0.4.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-20 01:55:52.000000 easytl-0.4.0a0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-20 01:57:41.422955 easytl-0.4.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-20 01:55:52.000000 easytl-0.4.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-20 01:55:52.000000 easytl-0.4.0a0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-20 01:55:52.000000 easytl-0.4.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:57:41.422955 easytl-0.4.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:57:41.418955 easytl-0.4.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:57:41.422955 easytl-0.4.0a0/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/anthropic_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94108 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/googletl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37317 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 01:55:52.000000 easytl-0.4.0a0/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:57:41.422955 easytl-0.4.0a0/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-05-20 01:57:41.000000 easytl-0.4.0a0/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-20 01:57:41.000000 easytl-0.4.0a0/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:57:41.000000 easytl-0.4.0a0/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-20 01:57:41.000000 easytl-0.4.0a0/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 01:57:41.000000 easytl-0.4.0a0/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:57:41.422955 easytl-0.4.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-20 01:55:52.000000 easytl-0.4.0a0/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-20 01:55:52.000000 easytl-0.4.0a0/tests/passing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-20 01:55:52.000000 easytl-0.4.0a0/tests/simple_test.py
```

### Comparing `easytl-0.3.3/.github/workflows/workflow.yml` & `easytl-0.4.0a0/.github/workflows/workflow.yml`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
           python -m pip install build
 
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
+          ANTHROPIC_API_KEY: ${{ secrets.ANTHROPIC_API_KEY }}
           GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Build the package
         run: |
@@ -63,14 +64,15 @@
           python -m pip install build
 
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
+          ANTHROPIC_API_KEY: ${{ secrets.ANTHROPIC_API_KEY }}
           GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Build the package
         run: |
@@ -99,14 +101,15 @@
           python -m pip install build
 
       - name: Set Environment Variables and Run Tests
         env:
           DEEPL_API_KEY: ${{ secrets.DEEPL_API_KEY }}
           GEMINI_API_KEY: ${{ secrets.GEMINI_API_KEY }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
+          ANTHROPIC_API_KEY: ${{ secrets.ANTHROPIC_API_KEY }}
           GOOGLE_TRANSLATE_SERVICE_KEY_VALUE: ${{ secrets.GOOGLE_TRANSLATE_SERVICE_KEY_VALUE }}
           LOGGING_DIRECTORY: /tmp/
         run: |
           python tests/passing.py
 
       - name: Install twine
         run: |
```

### Comparing `easytl-0.3.3/.gitignore` & `easytl-0.4.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `easytl-0.3.3/LICENSE.md` & `easytl-0.4.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.3/PKG-INFO` & `easytl-0.4.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.3.3
+Version: 0.4.0a0
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.3
+Requires-Dist: google-generativeai==0.5.4
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.29.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: google-cloud-translate==3.15.3
+Requires-Dist: anthropic==0.26.0
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
 - [Features](#features)
```

### Comparing `easytl-0.3.3/README.md` & `easytl-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.3/SECURITY.md` & `easytl-0.4.0a0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.3/pyproject.toml` & `easytl-0.4.0a0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,25 @@
     "tomli"
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [
-    "google-generativeai==0.5.3",
+    "google-generativeai==0.5.4",
     "deepl==1.16.1",
     "openai==1.29.0",
     "backoff==2.2.1",
     "tiktoken==0.6.0",
-    "google-cloud-translate==3.15.3"
+    "google-cloud-translate==3.15.3",
+    "anthropic==0.26.0"
 ]
 
 name = "easytl"
-version = "v0.3.3"
+version = "v0.4.0-alpha"
 authors = [
   { name="Bikatr7", email="Bikatr7@proton.me" },
 ]
 description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `easytl-0.3.3/src/easytl/anthropic_service.py` & `easytl-0.4.0a0/src/easytl/anthropic_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 
 ## built-in libraries
 import typing
 import asyncio
 
 ## third-party imports
 from anthropic import Anthropic, AsyncAnthropic
-from anthropic.types import Message
 
 ## custom modules
 from .exceptions import EasyTLException
-from .classes import ModelTranslationMessage, NotGiven, NOT_GIVEN
+from .classes import ModelTranslationMessage, NotGiven, NOT_GIVEN, AnthropicMessage, AnthropicToolsBetaMessage
 from .util import VALID_JSON_ANTHROPIC_MODELS, _is_iterable_of_strings, _convert_iterable_to_str, _estimate_cost
 from .decorators import _sync_logging_decorator, _async_logging_decorator
 
 class AnthropicService:
 
     _default_model:str = "claude-3-haiku-20240307"
     _default_translation_instructions:str = "Please translate the following text into English."
 
-    _system:str = _default_translation_instructions
+    _system:str | None   = _default_translation_instructions 
 
     _model:str = _default_model
     _temperature:float | NotGiven = NOT_GIVEN
     _top_p:float | NotGiven = NOT_GIVEN
     _top_k:int | NotGiven = NOT_GIVEN
     _stream:typing.Literal[False] | NotGiven = False
     _stop_sequences:typing.List[str] | NotGiven = NOT_GIVEN
@@ -40,14 +39,34 @@
     _rate_limit_delay:float | None = None
 
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
     _log_directory:str | None = None
 
     _json_mode:bool = False
+    _response_schema:typing.Mapping[str, typing.Any] | None = None
+    
+    _json_tool = {
+        "name": "format_to_json",
+        "description": "Formats text into json. This is required.",
+        "input_schema": {
+            "type": "object",
+            "properties": {
+                "input": {
+                    "type": "string",
+                    "description": "The text you were given to translate"
+                },
+                "output": {
+                    "type": "string",
+                    "description": "The translated text"
+                }
+            },
+            "required": ["input", "output"]
+        }
+    }
 
 ##-------------------start-of-set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _set_api_key(api_key:str) -> None:
 
         """
@@ -62,48 +81,54 @@
         AnthropicService._async_client.api_key = api_key
         AnthropicService._sync_client.api_key = api_key
 
 ##-------------------start-of-set_attributes()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def _set_attributes(model:str = _default_model,
+                        system:str | None = _default_translation_instructions,
                         temperature:float | NotGiven = NOT_GIVEN,
                         top_p:float | NotGiven = NOT_GIVEN,
                         top_k:int | NotGiven = NOT_GIVEN,
                         stream:typing.Literal[False] | NotGiven = False,
                         stop_sequences:typing.List[str] | NotGiven = NOT_GIVEN,
                         max_tokens:int | NotGiven = NOT_GIVEN,
                         decorator:typing.Union[typing.Callable, None]=None,
                         logging_directory:str | None=None,
                         semaphore:int | None=None,
                         rate_limit_delay:float | None=None,
-                        json_mode:bool=False
+                        json_mode:bool=False,
+                        response_schema:typing.Mapping[str, typing.Any] | None = None
                         ) -> None:
     
             """
     
             Sets the attributes for the Anthropic Service.
     
             """
     
             AnthropicService._model = model
+            AnthropicService._system = system
             AnthropicService._temperature = temperature
             AnthropicService._top_p = top_p
             AnthropicService._top_k = top_k
             AnthropicService._stream = stream
             AnthropicService._stop_sequences = stop_sequences
             AnthropicService._max_tokens = max_tokens
 
             AnthropicService._decorator_to_use = decorator
 
             AnthropicService._log_directory = logging_directory
 
             AnthropicService._rate_limit_delay = rate_limit_delay
 
             AnthropicService._json_mode = json_mode
+            AnthropicService._response_schema = response_schema
+
+            AnthropicService._json_tool['input_schema'] = AnthropicService._response_schema
 
             ## if a decorator is used, we want to disable retries, otherwise set it to the default value which is 2
             if(AnthropicService._decorator_to_use is not None):
                 AnthropicService._sync_client.max_retries = 0
                 AnthropicService._async_client.max_retries = 0
             else:
                 AnthropicService._sync_client.max_retries = 2
@@ -160,26 +185,26 @@
     
 ##-------------------start-of-_translate_text()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     @_sync_logging_decorator
     def _translate_text(translation_instructions: typing.Optional[str],
                                 translation_prompt: ModelTranslationMessage
-                                ) -> Message:
+                                ) -> AnthropicMessage | AnthropicToolsBetaMessage:
         
         """
         
         Synchronously translates the text using the Anthropic API.
 
         Parameters:
         translation_instructions (str) : The instructions to use for the translation.
         translation_prompt (ModelTranslationMessage) : The text to translate.
 
         Returns:
-        response (Message) : The response from the API.
+        response (AnthropicMessage) : The response from the API.
 
         """
         
         if(translation_instructions is None):
             translation_instructions = AnthropicService._default_translation_instructions
 
         if(AnthropicService._decorator_to_use is None):
@@ -190,26 +215,26 @@
     
 ##-------------------start-of-_translate_text()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     @_async_logging_decorator
     async def _translate_text_async(translation_instructions: typing.Optional[str],
                                 translation_prompt: ModelTranslationMessage
-                                ) -> Message:
+                                ) -> AnthropicMessage | AnthropicToolsBetaMessage:
         
         """
 
         Asynchronously translates the text using the Anthropic API.
 
         Parameters:
         translation_instructions (str) : The instructions to use for the translation.
         translation_prompt (ModelTranslationMessage) : The text to translate.
 
         Returns:
-        response (Message) : The response from the API.
+        response (AnthropicMessage) : The response from the API.
 
         """
         
         if(translation_instructions is None):
             translation_instructions = AnthropicService._default_translation_instructions
 
         if(AnthropicService._decorator_to_use is None):
@@ -217,85 +242,97 @@
         
         decorated_function = AnthropicService._decorator_to_use(AnthropicService.__translate_text_async)
         return await decorated_function(translation_instructions, translation_prompt)
 
 ##-------------------start-of-_translate_message()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def __translate_text(instructions:str, prompt:ModelTranslationMessage) -> Message:
+    def __translate_text(instructions:str, prompt:ModelTranslationMessage) -> AnthropicMessage | AnthropicToolsBetaMessage:
 
         """
 
         Synchronously translates the text using the Anthropic API.
 
         Parameters:
         instructions (str) : The instructions to use for the translation.
         prompt (ModelTranslationMessage) : The text to translate.
 
         Returns:
-        response (Message) : The response from the API.
+        response (AnthropicMessage) : The response from the API.
 
         """
-
+        
+        attributes = ["temperature", "top_p", "top_k", "stream", "stop_sequences", "max_tokens"]
         message_args = {
             "model": AnthropicService._model,
             "system": instructions,
             "messages": [prompt.to_dict()],  # type: ignore
-            "temperature": AnthropicService._temperature,
-            "top_p": AnthropicService._top_p,
-            "top_k": AnthropicService._top_k,
-            "stream": AnthropicService._stream,
-            "stop_sequences": AnthropicService._stop_sequences,
         }
-
-        if(AnthropicService._max_tokens != NOT_GIVEN):
-            message_args["max_tokens"] = AnthropicService._max_tokens
-
-        response = AnthropicService._sync_client.messages.create(**message_args)
+        
+        for attr in attributes:
+            value = getattr(AnthropicService, f"_{attr}")
+            if(value != NOT_GIVEN):
+                message_args[attr] = value
+        
+        # Special case for max_tokens
+        if("max_tokens" not in message_args):
+            message_args["max_tokens"] = 4096
+        
+        if(AnthropicService._json_mode and AnthropicService._model in VALID_JSON_ANTHROPIC_MODELS):
+            message_args["tools"] = [AnthropicService._json_tool]
+            message_args["tool_choice"] = {"type": "tool", "name": "format_to_json"}
+        
+        response = AnthropicService._sync_client.beta.tools.messages.create(**message_args)
 
         return response
     
 ##-------------------start-of- __translate_text_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    async def __translate_text_async(instruction:str, prompt:ModelTranslationMessage) -> Message:
+    async def __translate_text_async(instructions:str, prompt:ModelTranslationMessage) -> AnthropicMessage | AnthropicToolsBetaMessage:
 
         """
 
         Asynchronously translates the text using the Anthropic API.
 
         Parameters:
         instruction (str) : The instructions to use for the translation.
         prompt (ModelTranslationMessage) : The text to translate.
 
         Returns:
-        response (Message) : The response from the API.
+        response (AnthropicMessage) : The response from the API.
 
         """
 
         async with AnthropicService._semaphore:
 
             if(AnthropicService._rate_limit_delay is not None):
                 await asyncio.sleep(AnthropicService._rate_limit_delay)
 
+            attributes = ["temperature", "top_p", "top_k", "stream", "stop_sequences", "max_tokens"]
             message_args = {
                 "model": AnthropicService._model,
-                "system": instruction,
+                "system": instructions,
                 "messages": [prompt.to_dict()],  # type: ignore
-                "temperature": AnthropicService._temperature,
-                "top_p": AnthropicService._top_p,
-                "top_k": AnthropicService._top_k,
-                "stream": AnthropicService._stream,
-                "stop_sequences": AnthropicService._stop_sequences,
             }
+            
+            for attr in attributes:
+                value = getattr(AnthropicService, f"_{attr}")
+                if(value != NOT_GIVEN):
+                    message_args[attr] = value
+            
+            # Special case for max_tokens
+            if("max_tokens" not in message_args):
+                message_args["max_tokens"] = 4096
+            
+            if(AnthropicService._json_mode and AnthropicService._model in VALID_JSON_ANTHROPIC_MODELS):
+                message_args["tools"] = [AnthropicService._json_tool]
+                message_args["tool_choice"] = {"type": "tool", "name": "format_to_json"}
 
-            if(AnthropicService._max_tokens != NOT_GIVEN):
-                message_args["max_tokens"] = AnthropicService._max_tokens
-
-            response = await AnthropicService._async_client.messages.create(**message_args)
+            response = await AnthropicService._async_client.beta.tools.messages.create(**message_args)
 
             return response
     
 ##-------------------start-of-test_api_key_validity()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     def _test_api_key_validity() -> typing.Tuple[bool, typing.Union[Exception, None]]:
```

### Comparing `easytl-0.3.3/src/easytl/classes.py` & `easytl-0.4.0a0/src/easytl/classes.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 ## openai api data used by openai_service to type check
 from openai.types.chat.chat_completion import ChatCompletion
 
 ## gemini api data used by gemini_service to type check
 from google.generativeai import GenerationConfig
 from google.generativeai.types import GenerateContentResponse, AsyncGenerateContentResponse
 
+## anthropic api data used by anthropic_service to type check
+from anthropic.types import Message as AnthropicMessage, TextBlock as AnthropicTextBlock
+from anthropic.types.beta.tools import ToolsBetaMessage as AnthropicToolsBetaMessage
+from anthropic.types.beta.tools import ToolUseBlock as AnthropicToolUseBlock
+
 ##-------------------start-of-Message--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 class Message:
 
     """
 
     Message is a class that is used to send translation batches to the OpenAI API.
```

### Comparing `easytl-0.3.3/src/easytl/decorators.py` & `easytl-0.4.0a0/src/easytl/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,32 +4,36 @@
 
 ## built-in libraries
 from functools import wraps
 
 import datetime
 import os
 
+## custom modules
+from .classes import AnthropicTextBlock, AnthropicToolUseBlock
+
 ##-------------------start-of-get_nested_attribute()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _get_nested_attribute(obj, attrs):
-    for attr in attrs:
+    for attr, type_hint in attrs:
         try:
             if(isinstance(obj, list) and attr.isdigit()):
                 obj = obj[int(attr)]
             else:
                 try:
-                    obj = getattr(obj, attr)
+                    if(type_hint is None or isinstance(obj, type_hint)):
+                        obj = getattr(obj, attr)
                 except AttributeError:
                     ## Try dictionary access
                     obj = obj[attr]
 
         except (AttributeError, IndexError, KeyError):
             raise ValueError(f"Attribute {attr} in object {obj} not found.")
         
-    return obj
+    return str(obj)
 
 ##-------------------start-of-logging_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _async_logging_decorator(func):
 
     @wraps(func)
     async def wrapper(*args, **kwargs):
@@ -52,17 +56,24 @@
 
         filename = f"easytl-log.txt"
         filepath = os.path.join(directory, filename)
         
         result = await func(*args, **kwargs)
 
         ## Get the attribute to log
-        attr_to_log = log_attributes.get(cls_name, None)
-        if(attr_to_log and not isinstance(result, str)):
-            log_data = _get_nested_attribute(result, attr_to_log)
+        attr_to_logs = log_attributes.get(cls_name, None)
+        if(attr_to_logs):
+            log_data = []
+            for attr_to_log in attr_to_logs:
+                if(not isinstance(attr_to_log, list) and cls_name != 'OpenAIService'):
+                    ## coerce to list
+                    attr_to_log = [attr_to_log]
+                if(not isinstance(result, str)):
+                    log_data.append(_get_nested_attribute(result, attr_to_log))
+            log_data = '\n'.join(log_data)
         
         ## did you know multi-line f-strings take leading spaces into account?
         log_data = f"""
 {'=' * 40}
 Function Call Details:
 {'-' * 40}
 Class Name: {cls_name}
@@ -108,17 +119,24 @@
 
         filename = f"easytl-log.txt"
         filepath = os.path.join(directory, filename)
         
         result = func(*args, **kwargs)
 
         ## Get the attribute to log
-        attr_to_log = log_attributes.get(cls_name, None)
-        if(attr_to_log and not isinstance(result, str)):
-            log_data = _get_nested_attribute(result, attr_to_log)
+        attr_to_logs = log_attributes.get(cls_name, None)
+        if(attr_to_logs):
+            log_data = []
+            for attr_to_log in attr_to_logs:
+                if(not isinstance(attr_to_log, list) and cls_name != 'OpenAIService'):
+                    ## coerce to list
+                    attr_to_log = [attr_to_log]
+                if(not isinstance(result, str)):
+                    log_data.append(_get_nested_attribute(result, attr_to_log))
+            log_data = '\n'.join(log_data)
         
         ## did you know multi-line f-strings take leading spaces into account?
         log_data = f"""
 {'=' * 40}
 Function Call Details:
 {'-' * 40}
 Class Name: {cls_name}
@@ -139,12 +157,19 @@
         
         return result
     
     return wrapper
 
 ## Since we're dealing with objects here...
 log_attributes = {
-    'GeminiService': ['text'],
-    'DeepLService': ['text'],
-    'OpenAIService': ['choices', '0', 'message', 'content'],
-    'GoogleTLService': ['translatedText']
-}
+    'GeminiService': [('text', None)],
+    'DeepLService': [
+('text', None)],
+    'OpenAIService': [[('choices', None), ('0', None), ('message', None), ('content', None)],
+                      [('choices', None), ('0', None), ('message', None), ('content', None)],
+                      ],
+    'GoogleTLService': [('translatedText', None)],
+    'AnthropicService': [
+        [('content', None), ('0', None), ('text', AnthropicTextBlock)],
+        [('content', None), ('0', None), ('input', AnthropicToolUseBlock)]
+    ]
+}
```

### Comparing `easytl-0.3.3/src/easytl/deepl_service.py` & `easytl-0.4.0a0/src/easytl/deepl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.3/src/easytl/easytl.py` & `easytl-0.4.0a0/src/easytl/easytl.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 ## built-in libraries
 import typing
 import asyncio
 
 import warnings
 
 ## third-party libraries
-from .classes import Language, SplitSentences, Formality, GlossaryInfo
+from .classes import Language, SplitSentences, Formality, GlossaryInfo, NOT_GIVEN, NotGiven
 
 ## custom modules
 from .deepl_service import DeepLService
 from .gemini_service import GeminiService
 from .openai_service import OpenAIService
 from .googletl_service import GoogleTLService
+from .anthropic_service import AnthropicService
 
-from. classes import ModelTranslationMessage, SystemTranslationMessage, TextResult, GenerateContentResponse, AsyncGenerateContentResponse, ChatCompletion
-from .exceptions import DeepLException, GoogleAPIError, OpenAIError, InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException
+from. classes import ModelTranslationMessage, SystemTranslationMessage, TextResult, GenerateContentResponse, AsyncGenerateContentResponse, ChatCompletion, AnthropicMessage, AnthropicToolsBetaMessage, AnthropicTextBlock, AnthropicToolUseBlock
+from .exceptions import DeepLException, GoogleAPIError, OpenAIError, InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException, AnthropicError
 
-from .util import _validate_easytl_translation_settings, _is_iterable_of_strings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences
+from .util import _validate_easytl_translation_settings, _is_iterable_of_strings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences, _validate_response_schema,  _return_curated_anthropic_settings
 
 class EasyTL:
 
     """
     
     EasyTL global client, used to interact with Translation APIs.
 
@@ -60,45 +61,46 @@
         """
 
         warnings.warn("set_api_key is deprecated and will be removed in a future version. Use set_credentials instead.", DeprecationWarning, stacklevel=2)
 
         service_map = {
             "deepl": DeepLService,
             "gemini": GeminiService,
-            "openai": OpenAIService
+            "openai": OpenAIService,
         }
 
         assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini' and 'openai'.")
 
         service_map[api_type]._set_api_key(api_key)
 
 ##-------------------start-of-set_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def set_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate"], credentials:str) -> None:
+    def set_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic"], credentials:str) -> None:
 
         """
 
         Sets the credentials for the specified API type.
 
         Parameters:
-        api_type (literal["deepl", "gemini", "openai", "google translate"]) : The API type to set the credentials for.
-        credentials (string) : The credentials to set. This is an api key for deepl, gemini and openai. For google translate, this is a path to your json that has your service account key.
+        api_type (literal["deepl", "gemini", "openai", "google translate", "anthropic"]) : The API type to set the credentials for.
+        credentials (string) : The credentials to set. This is an api key for deepl, gemini, anthropic, and openai. For google translate, this is a path to your json that has your service account key.
 
         """
 
         service_map = {
             "deepl": DeepLService._set_api_key,
             "gemini": GeminiService._set_api_key,
             "openai": OpenAIService._set_api_key,
-            "google translate": GoogleTLService._set_credentials
+            "google translate": GoogleTLService._set_credentials,
+            "anthropic": AnthropicService._set_api_key
 
         }
 
-        assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai' and 'google translate'.")
+        assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai', 'google translate', and 'anthropic'.")
 
         service_map[api_type](credentials)
 
 ##-------------------start-of-test_api_key_validity()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
             
     @staticmethod
     def test_api_key_validity(api_type:typing.Literal["deepl", "gemini", "openai"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
@@ -137,37 +139,38 @@
             return False, _e
 
         return True, None
     
 ##-------------------start-of-test_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def test_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
+    def test_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
 
         """
 
         Tests the validity of the credentials for the specified API type.
 
         Parameters:
-        api_type (literal["deepl", "gemini", "openai", "google translate"]) : The API type to test the credentials for.
+        api_type (literal["deepl", "gemini", "openai", "google translate", "anthropic"]) : The API type to test the credentials for.
 
         Returns:
         (bool) : Whether the credentials are valid.
         (Exception) : The exception that was raised, if any. None otherwise.
 
         """
 
         api_services = {
             "deepl": {"service": DeepLService, "exception": DeepLException, "test_func": DeepLService._test_api_key_validity},
             "gemini": {"service": GeminiService, "exception": GoogleAPIError, "test_func": GeminiService._test_api_key_validity},
             "openai": {"service": OpenAIService, "exception": OpenAIError, "test_func": OpenAIService._test_api_key_validity},
-            "google translate": {"service": GoogleTLService, "exception": GoogleAPIError, "test_func": GoogleTLService._test_credentials}
+            "google translate": {"service": GoogleTLService, "exception": GoogleAPIError, "test_func": GoogleTLService._test_credentials},
+            "anthropic": {"service": AnthropicService, "exception": AnthropicError, "test_func": AnthropicService._test_api_key_validity}
         }
 
-        assert api_type in api_services, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai' and 'google translate'.")
+        assert api_type in api_services, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai', 'google translate', and 'anthropic'.")
 
         _is_valid, _e = api_services[api_type]["test_func"]()
 
         if(not _is_valid):
             ## Done to make sure the exception is due to the specified API type and not the fault of EasyTL
             assert isinstance(_e, api_services[api_type]["exception"]), _e
             return False, _e
@@ -581,14 +584,15 @@
 
     @staticmethod
     def gemini_translate(text:typing.Union[str, typing.Iterable[str]],
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
                         logging_directory:str | None = None,
                         response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                        response_schema:str | typing.Mapping[str, typing.Any] | None = None,
                         translation_delay:float | None = None,
                         translation_instructions:str | None = None,
                         model:str="gemini-pro",
                         temperature:float=0.5,
                         top_p:float=0.9,
                         top_k:int=40,
                         stop_sequences:typing.List[str] | None=None,
@@ -608,14 +612,15 @@
         
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a GenerateContentResponse object, 'json' returns a json-parseable string.
+        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         model (string) : The model to use. 
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
         stop_sequences (list or None) : The sequences to stop at.
@@ -630,14 +635,16 @@
 
         _settings = _return_curated_gemini_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
         _validate_stop_sequences(stop_sequences)
 
+        response_schema = _validate_response_schema(response_schema)
+
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("gemini")
 
         json_mode = True if response_type == "json" else False
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
@@ -649,15 +656,16 @@
                                           stream=False,
                                           stop_sequences=stop_sequences,
                                           max_output_tokens=max_output_tokens,
                                           decorator=decorator,
                                           logging_directory=logging_directory,
                                           semaphore=None,
                                           rate_limit_delay=translation_delay,
-                                          json_mode=json_mode)
+                                          json_mode=json_mode,
+                                          response_schema=response_schema)
             
             ## Done afterwards, cause default translation instructions can change based on set_attributes()       
             GeminiService._system_message = translation_instructions or GeminiService._default_translation_instructions
         
         if(isinstance(text, str)):
             _result = GeminiService._translate_text(text)
             
@@ -682,14 +690,15 @@
     
     @staticmethod
     async def gemini_translate_async(text:typing.Union[str, typing.Iterable[str]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
                                     logging_directory:str | None = None,
                                     response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                                    response_schema:str | typing.Mapping[str, typing.Any] | None = None,
                                     semaphore:int | None = None,
                                     translation_delay:float | None = None,
                                     translation_instructions:str | None = None,
                                     model:str="gemini-pro",
                                     temperature:float=0.5,
                                     top_p:float=0.9,
                                     top_k:int=40,
@@ -713,14 +722,15 @@
         
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a AsyncGenerateContentResponse object, 'json' returns a json-parseable string.
+        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
         semaphore (int) : The number of concurrent requests to make. Default is 15 for 1.0 and 2 for 1.5 gemini models. For Gemini, it is recommend to use translation_delay along with the semaphore to prevent rate limiting.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         model (string) : The model to use.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
@@ -736,14 +746,16 @@
 
         _settings = _return_curated_gemini_settings(locals())
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
         _validate_stop_sequences(stop_sequences)
 
+        response_schema = _validate_response_schema(response_schema)
+
         ## Should be done after validating the settings to reduce cost to the user
         EasyTL.test_credentials("gemini")
 
         json_mode = True if response_type == "json" else False
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
@@ -755,15 +767,16 @@
                                           stream=False,
                                           stop_sequences=stop_sequences,
                                           max_output_tokens=max_output_tokens,
                                           decorator=decorator,
                                           logging_directory=logging_directory,
                                           semaphore=semaphore,
                                           rate_limit_delay=translation_delay,
-                                          json_mode=json_mode)
+                                          json_mode=json_mode,
+                                          response_schema=response_schema)
             
             ## Done afterwards, cause default translation instructions can change based on set_attributes()
             GeminiService._system_message = translation_instructions or GeminiService._default_translation_instructions
             
         if(isinstance(text, str)):
             _result = await GeminiService._translate_text_async(text)
 
@@ -991,76 +1004,330 @@
 
         translation = _results if response_type == "raw" else [result.choices[0].message.content for result in _results if result.choices[0].message.content is not None]
 
         result = translation if isinstance(text, typing.Iterable) and not isinstance(text, str) else translation[0]
 
         return result
     
+##-------------------start-of-anthropic_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    def anthropic_translate(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
+                            override_previous_settings:bool = True,
+                            decorator:typing.Callable | None = None,
+                            logging_directory:str | None = None,
+                            response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                            response_schema:str | typing.Mapping[str, typing.Any] | None = None,
+                            translation_delay:float | None = None,
+                            translation_instructions:str | None = None,
+                            model:str="claude-3-haiku-20240307",
+                            temperature:float | NotGiven = NOT_GIVEN,
+                            top_p:float | NotGiven = NOT_GIVEN,
+                            top_k:int | NotGiven = NOT_GIVEN,
+                            stop_sequences:typing.List[str] | NotGiven = NOT_GIVEN,
+                            max_output_tokens:int | NotGiven = NOT_GIVEN) -> typing.Union[typing.List[str], str, 
+                                                                                          AnthropicMessage, typing.List[AnthropicMessage],
+                                                                                          AnthropicToolsBetaMessage, typing.List[AnthropicToolsBetaMessage]]:
+        
+        """
+
+        Translates the given text using Anthropic.
+
+        This function assumes that the API key has already been set.
+
+        Translation instructions default to translating the text to English. To change this, specify the instructions.
+
+        This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
+
+        Due to how Anthropic's API works, NOT_GIVEN is treated differently than None. If a parameter is set to NOT_GIVEN, it is not passed to the API. 
+
+        Anthropic's JSON response is quite unsophisticated and also in Beta, it costs a lot of extra tokens to return a json response. It's also inconsistent. Be careful when using it.
+
+        Parameters:
+        text (string or iterable) : The text to translate.
+        override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an Anthropic translation function.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, Anthropic will retry the request twice if it fails.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, an AnthropicMessage object, 'json' returns a json-parseable string. Anthropic's API is unsophisticated in this regard, it costs a lot of extra tokens to return a json response.
+        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json. 
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
+        model (string) : The model to use.
+        temperature (float or NotGiven) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
+        top_p (float or NotGiven) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
+        top_k (int or NotGiven) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
+        stop_sequences (list or NotGiven) : The sequences to stop at.
+        max_output_tokens (int or NotGiven) : The maximum number of tokens to output.
+
+        Returns:
+        result (string or list - string or AnthropicMessage or list - AnthropicMessage or AnthropicToolsBetaMessage or list - AnthropicToolsBetaMessage) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of AnthropicMessage objects if the response type is 'raw' and input was an iterable, an AnthropicMessage object otherwise. A list of AnthropicToolsBetaMessage objects if the response type is 'raw' and input was an iterable, an AnthropicToolsBetaMessage object otherwise.
+
+        """
+
+        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
+
+        _settings = _return_curated_anthropic_settings(locals())
+
+        _validate_easytl_translation_settings(_settings, "anthropic")
+
+        _validate_stop_sequences(stop_sequences)
+
+        response_schema = _validate_response_schema(response_schema)
+
+        ## Should be done after validating the settings to reduce cost to the user
+        EasyTL.test_credentials("anthropic")
+
+        json_mode = True if response_type == "json" else False
+
+        if(override_previous_settings == True):
+            AnthropicService._set_attributes(model=model,
+                                            system=translation_instructions,
+                                            temperature=temperature,
+                                            top_p=top_p,
+                                            top_k=top_k,
+                                            stop_sequences=stop_sequences,
+                                            stream=False,
+                                            max_tokens=max_output_tokens,
+                                            decorator=decorator,
+                                            logging_directory=logging_directory,
+                                            semaphore=None,
+                                            rate_limit_delay=translation_delay,
+                                            json_mode=json_mode,
+                                            response_schema=response_schema)
+            
+            ## Done afterwards, cause default translation instructions can change based on set_attributes()
+            AnthropicService._system = translation_instructions or AnthropicService._default_translation_instructions
+
+        assert isinstance(text, str) or _is_iterable_of_strings(text) or isinstance(text, ModelTranslationMessage) or _is_iterable_of_strings(text), InvalidTextInputException("text must be a string, an iterable of strings, a ModelTranslationMessage or an iterable of ModelTranslationMessages.")
+
+        _translation_batches = AnthropicService._build_translation_batches(text)
+
+        _translations = []
+
+        for _text in _translation_batches:
+
+            _result = AnthropicService._translate_text(AnthropicService._system, _text)
+
+            assert not isinstance(_result, list) and hasattr(_result, "content"), EasyTLException("Malformed response received. Please try again.")
+
+            if(response_type == "raw"):
+                translation = _result
+
+            ## response structure is different for beta
+            elif(isinstance(_result, AnthropicToolsBetaMessage)):
+                content = _result.content
+
+                if(isinstance(content[0], AnthropicTextBlock)):
+                    translation = content[0].text
+
+                elif(isinstance(content[0], AnthropicToolUseBlock)):
+                    translation = content[0].input
+
+            elif(isinstance(_result, AnthropicMessage)):
+                translation = _result.content[0].text
+                            
+            _translations.append(translation)
+
+        ## If originally a single text was provided, return a single translation instead of a list
+        result = _translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else _translations[0]
+
+        return result
+    
+##-------------------start-of-anthropic_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    async def anthropic_translate_async(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
+                                        override_previous_settings:bool = True,
+                                        decorator:typing.Callable | None = None,
+                                        logging_directory:str | None = None,
+                                        response_type:typing.Literal["text", "raw", "json"] | None = "text",
+                                        response_schema:str | typing.Mapping[str, typing.Any] | None = None,
+                                        semaphore:int | None = None,
+                                        translation_delay:float | None = None,
+                                        translation_instructions:str | None = None,
+                                        model:str="claude-3-haiku-20240307",
+                                        temperature:float | NotGiven = NOT_GIVEN,
+                                        top_p:float | NotGiven = NOT_GIVEN,
+                                        top_k:int | NotGiven = NOT_GIVEN,
+                                        stop_sequences:typing.List[str] | NotGiven = NOT_GIVEN,
+                                        max_output_tokens:int | NotGiven = NOT_GIVEN) -> typing.Union[typing.List[str], str, 
+                                                                                                    AnthropicMessage, typing.List[AnthropicMessage],
+                                                                                                    AnthropicToolsBetaMessage, typing.List[AnthropicToolsBetaMessage]]:
+        
+        """
+
+        Asynchronous version of anthropic_translate().
+
+        Will generally be faster for iterables. Order is preserved.
+
+        This function assumes that the API key has already been set.
+
+        Translation instructions default to translating the text to English. To change this, specify the instructions.
+
+        This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
+
+        Due to how Anthropic's API works, NOT_GIVEN is treated differently than None. If a parameter is set to NOT_GIVEN, it is not passed to the API.
+
+        Anthropic's JSON response is quite unsophisticated and also in Beta, it costs a lot of extra tokens to return a json response. It's also inconsistent. Be careful when using it.
+
+        Parameters:
+        text (string | ModelTranslationMessage or iterable) : The text to translate.
+        override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an Anthropic translation function.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, Anthropic will retry the request twice if it fails.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, an AnthropicMessage object, 'json' returns a json-parseable string. Anthropic's API is unsophisticated in this regard, it costs a lot of extra tokens to return a json response.
+        response_schema (string or mapping or None) : The schema to use for the response. If None, no schema is used. This is only used if the response type is 'json'. EasyTL only validates the schema to the extend that it is None or a valid json. It does not validate the contents of the json.
+        semaphore (int) : The number of concurrent requests to make. Default is 5.
+        translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
+        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
+        model (string) : The model to use.
+        temperature (float or NotGiven) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
+        top_p (float or NotGiven) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
+        top_k (int or NotGiven) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
+        stop_sequences (list or NotGiven) : The sequences to stop at.
+        max_output_tokens (int or NotGiven) : The maximum number of tokens to output.
+
+        Returns:
+        result (string or list - string or AnthropicMessage or list - AnthropicMessage or AnthropicToolsBetaMessage or list - AnthropicToolsBetaMessage) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of AnthropicMessage objects if the response type is 'raw' and input was an iterable, an AnthropicMessage object otherwise. A list of AnthropicToolsBetaMessage objects if the response type is 'raw' and input was an iterable, an AnthropicToolsBetaMessage object otherwise.
+
+        """
+
+        assert response_type in ["text", "raw", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
+
+        _settings = _return_curated_anthropic_settings(locals())
+
+        _validate_easytl_translation_settings(_settings, "anthropic")
+
+        _validate_stop_sequences(stop_sequences)
+
+        response_schema = _validate_response_schema(response_schema)
+
+        ## Should be done after validating the settings to reduce cost to the user
+        EasyTL.test_credentials("anthropic")
+
+        json_mode = True if response_type == "json" else False
+
+        if(override_previous_settings == True):
+            AnthropicService._set_attributes(model=model,
+                                            system=translation_instructions,
+                                            temperature=temperature,
+                                            top_p=top_p,
+                                            top_k=top_k,
+                                            stop_sequences=stop_sequences,
+                                            stream=False,
+                                            max_tokens=max_output_tokens,
+                                            decorator=decorator,
+                                            logging_directory=logging_directory,
+                                            semaphore=semaphore,
+                                            rate_limit_delay=translation_delay,
+                                            json_mode=json_mode,
+                                            response_schema=response_schema)
+            
+            ## Done afterwards, cause default translation instructions can change based on set_attributes()
+            AnthropicService._system = translation_instructions or AnthropicService._default_translation_instructions
+        
+        assert isinstance(text, str) or _is_iterable_of_strings(text) or isinstance(text, ModelTranslationMessage) or _is_iterable_of_strings(text), InvalidTextInputException("text must be a string, an iterable of strings, a ModelTranslationMessage or an iterable of ModelTranslationMessages.")
+
+        _translation_batches = AnthropicService._build_translation_batches(text)
+
+        _translations_tasks = []
+
+        for _text in _translation_batches:
+            _task = AnthropicService._translate_text_async(AnthropicService._system, _text)
+            _translations_tasks.append(_task)
+
+        _results = await asyncio.gather(*_translations_tasks)
+
+        _results:typing.List[AnthropicMessage | AnthropicToolsBetaMessage] = _results
+
+        assert all([hasattr(_r, "content") for _r in _results]), EasyTLException("Malformed response received. Please try again.")
+
+        if(response_type == "raw"):
+            translations = _results
+
+        ## response structure is different for beta
+        elif(isinstance(_results[0], AnthropicToolsBetaMessage)):
+            translations = [result.content[0].input if isinstance(result.content[0], AnthropicToolUseBlock) else result.content[0].text for result in _results]
+        
+        elif(isinstance(_results[0], AnthropicMessage)):
+            translations = [result.content[0].text for result in _results if isinstance(result.content[0], AnthropicTextBlock)]
+                
+        result = translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else translations[0]
+
+        return result # type: ignore
+        
 ##-------------------start-of-translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def translate(text:str | typing.Iterable[str],
-                  service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate"]] = "deepl",
+                  service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic"]] = "deepl",
                   **kwargs) -> typing.Union[typing.List[str], str, 
                                             typing.List[TextResult], TextResult, 
                                             typing.List[ChatCompletion], ChatCompletion,
                                             typing.List[GenerateContentResponse], GenerateContentResponse, 
-                                            typing.List[typing.Any], typing.Any]:
+                                            typing.List[typing.Any], typing.Any,
+                                            typing.List[AnthropicMessage], AnthropicMessage]:
         
         """
 
         Translates the given text to the target language using the specified service.
 
         Please see the documentation for the specific translation function for the service you want to use.
 
         DeepL: deepl_translate() 
         OpenAI: openai_translate() 
         Gemini: gemini_translate() 
         Google Translate: googletl_translate() 
+        Anthropic: anthropic_translate()
 
         All functions can return a list of strings or a string, depending on the input. The response type can be specified to return the raw response instead:
         DeepL: TextResult
         OpenAI: ChatCompletion
         Gemini: GenerateContentResponse
         Google Translate: any
+        Anthropic: AnthropicMessage or AnthropicToolsBetaMessage
 
         Parameters:
         service (string) : The service to use for translation.
         text (string) : The text to translate.
         **kwargs : The keyword arguments to pass to the translation function.
 
         Returns:
-        result (string or list - string or TextResult or list - TextResult or ChatCompletion or list - ChatCompletion or GenerateContentResponse or list - GenerateContentResponse or any or list - any) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise. A list of GenerateContentResponse objects if the response type is 'raw' and input was an iterable, a GenerateContentResponse object otherwise. A list of any objects if the response type is 'raw' and input was an iterable, an any object otherwise.
+        result (string or list - string or TextResult or list - TextResult or GenerateContentResponse or list - GenerateContentResponse or ChatCompletion or list - ChatCompletion or any or list - any or AnthropicMessage or list - AnthropicMessage or AnthropicToolsBetaMessage or list - AnthropicToolsBetaMessage) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise. A list of GenerateContentResponse objects if the response type is 'raw' and input was an iterable, a GenerateContentResponse object otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise. A list of any objects if the response type is 'raw' and input was an iterable, an any object otherwise. A list of AnthropicMessage objects if the response type is 'raw' and input was an iterable, an AnthropicMessage object otherwise. A list of AnthropicToolsBetaMessage objects if the response type is 'raw' and input was an iterable, an AnthropicToolsBetaMessage object otherwise.
 
         """
 
-        assert service in ["deepl", "openai", "gemini", "google translate"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini' or 'google translate'.")
+        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate' or 'anthropic'.")
 
         if(service == "deepl"):
             return EasyTL.deepl_translate(text, **kwargs)
 
         elif(service == "openai"):
             return EasyTL.openai_translate(text, **kwargs)
 
         elif(service == "gemini"):
            return EasyTL.gemini_translate(text, **kwargs)
         
         elif(service == "google translate"):
             return EasyTL.googletl_translate(text, **kwargs)
         
+        elif(service == "anthropic"):
+            return EasyTL.anthropic_translate(text, **kwargs)
+        
 ##-------------------start-of-translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     async def translate_async(text:str | typing.Iterable[str],
-                              service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate"]] = "deepl",
+                              service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic"]] = "deepl",
                               **kwargs) -> typing.Union[typing.List[str], str, 
                                                         typing.List[TextResult], TextResult,  
                                                         typing.List[ChatCompletion], ChatCompletion,
                                                         typing.List[AsyncGenerateContentResponse], AsyncGenerateContentResponse,
-                                                        typing.List[typing.Any], typing.Any]:
+                                                        typing.List[typing.Any], typing.Any,
+                                                        typing.List[AnthropicMessage], AnthropicMessage]:
 
         
         """
 
         Asynchronous version of translate().
         
         Translates the given text to the target language using the specified service.
@@ -1069,50 +1336,55 @@
 
         Please see the documentation for the specific translation function for the service you want to use.
 
         DeepL: deepl_translate_async()
         OpenAI: openai_translate_async() 
         Gemini: gemini_translate_async() 
         Google Translate: googletl_translate_async()
+        Anthropic: anthropic_translate_async()
 
         All functions can return a list of strings or a string, depending on the input. The response type can be specified to return the raw response instead:
         DeepL: TextResult
         OpenAI: ChatCompletion
         Gemini: AsyncGenerateContentResponse
         Google Translate: any
+        Anthropic: AnthropicMessage or AnthropicToolsBetaMessage
 
         Parameters:
         service (string) : The service to use for translation.
         text (string) : The text to translate.
         **kwargs : The keyword arguments to pass to the translation function.
 
         Returns:
-        result (string or list - string or TextResult or list - TextResult or AsyncGenerateContentResponse or list - AsyncGenerateContentResponse or ChatCompletion or list - ChatCompletion or any or list - any) : The translation result according to the service used.
+        result (string or list - string or TextResult or list - TextResult or AsyncGenerateContentResponse or list - AsyncGenerateContentResponse or ChatCompletion or list - ChatCompletion or any or list - any or AnthropicMessage or list - AnthropicMessage or AnthropicToolsBetaMessage or list - AnthropicToolsBetaMessage) : The translation result. A list of strings if the input was an iterable, a string otherwise. A list of TextResult objects if the response type is 'raw' and input was an iterable, a TextResult object otherwise. A list of AsyncGenerateContentResponse objects if the response type is 'raw' and input was an iterable, an AsyncGenerateContentResponse object otherwise. A list of ChatCompletion objects if the response type is 'raw' and input was an iterable, a ChatCompletion object otherwise. A list of any objects if the response type is 'raw' and input was an iterable, an any object otherwise. A list of AnthropicMessage objects if the response type is 'raw' and input was an iterable, an AnthropicMessage object otherwise. A list of AnthropicToolsBetaMessage objects if the response type is 'raw' and input was an iterable, an AnthropicToolsBetaMessage object otherwise.
 
         """
 
-        assert service in ["deepl", "openai", "gemini", "google translate"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini' or 'google translate'.")
+        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate' or 'anthropic'.")
 
         if(service == "deepl"):
             return await EasyTL.deepl_translate_async(text, **kwargs)
 
         elif(service == "openai"):
             return await EasyTL.openai_translate_async(text, **kwargs)
 
         elif(service == "gemini"):
             return await EasyTL.gemini_translate_async(text, **kwargs)
         
         elif(service == "google translate"):
             return await EasyTL.googletl_translate_async(text, **kwargs)
+        
+        elif(service == "anthropic"):
+            return await EasyTL.anthropic_translate_async(text, **kwargs)
 
 ##-------------------start-of-calculate_cost()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def calculate_cost(text:str | typing.Iterable[str],
-                       service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate"]] = "deepl",
+                       service:typing.Optional[typing.Literal["deepl", "openai", "gemini", "google translate", "anthropic"]] = "deepl",
                        model:typing.Optional[str] = None,
                        translation_instructions:typing.Optional[str] = None
                        ) -> typing.Tuple[int, float, str]:
         
         """
 
         Calculates the cost of translating the given text using the specified service.
@@ -1120,33 +1392,38 @@
         For LLMs, the cost is based on the default model unless specified.
 
         Model and Translation Instructions are ignored for DeepL and Google Translate.
 
         For deepl, number of tokens is the number of characters, the returned model is always "deepl".
         The same applies for google translate, but the model is "google translate".
 
+        Note that Anthropic's cost estimate is pretty sketchy and can be inaccurate. Refer to the actual response object for the cost or the API panel. This is because their tokenizer is not public and we're forced to estimate.
+
         Parameters:
         text (string or iterable) : The text to translate.
         service (string) : The service to use for translation.
         model (string or None) : The model to use for translation. If None, the default model is used.
         translation_instructions (string or None) : The translation instructions to use.
 
         Returns:
         num_tokens (int) : The number of tokens/characters in the text.
         cost (float) : The cost of translating the text.
         model (string) : The model used for translation.
 
         """
 
-        assert service in ["deepl", "openai", "gemini", "google translate"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini' or 'google translate'.")
+        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate' or 'anthropic'.")
 
         if(service == "deepl"):
             return DeepLService._calculate_cost(text)
         
         elif(service == "openai"):
             return OpenAIService._calculate_cost(text, translation_instructions, model)
 
         elif(service == "gemini"):
             return GeminiService._calculate_cost(text, translation_instructions, model)
         
         elif(service == "google translate"):
-            return GoogleTLService._calculate_cost(text)
+            return GoogleTLService._calculate_cost(text)
+        
+        elif(service == "anthropic"):
+            return AnthropicService._calculate_cost(text, translation_instructions, model)
```

### Comparing `easytl-0.3.3/src/easytl/gemini_service.py` & `easytl-0.4.0a0/src/easytl/gemini_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 ## built-in libraries
 import typing
 import asyncio
 
 import google.generativeai as genai
 
 ## custom modules
-from .util import _estimate_cost, _convert_iterable_to_str, _is_iterable_of_strings
+from .util import _estimate_cost, _convert_iterable_to_str, _is_iterable_of_strings, VALID_JSON_GEMINI_MODELS
+from .util import VALID_JSON_GEMINI_MODELS as VALID_SYSTEM_MESSAGE_MODELS
 from .decorators import _async_logging_decorator, _sync_logging_decorator
 
 from .classes import GenerationConfig, GenerateContentResponse, AsyncGenerateContentResponse
 from .exceptions import EasyTLException, InvalidTextInputException
 
 class GeminiService:
 
@@ -64,14 +65,15 @@
         {
             "category": "HARM_CATEGORY_DANGEROUS_CONTENT",
             "threshold": "BLOCK_NONE",
         },
     ]
 
     _json_mode:bool = False
+    _response_schema:typing.Mapping[str, typing.Any] | None = None
 
 ##-------------------start-of-_set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _set_api_key(api_key:str) -> None:
 
         """
@@ -97,15 +99,16 @@
                         stream:bool=False,
                         stop_sequences:typing.List[str] | None=None,
                         max_output_tokens:int | None=None,
                         decorator:typing.Union[typing.Callable, None]=None,
                         logging_directory:str | None=None,
                         semaphore:int | None=None,
                         rate_limit_delay:float | None=None,
-                        json_mode:bool=False
+                        json_mode:bool=False,
+                        response_schema:typing.Mapping[str, typing.Any] | None = None
                         ) -> None:
         
         """
 
         Sets the attributes for the Gemini service.
 
         """
@@ -123,24 +126,37 @@
         GeminiService._decorator_to_use = decorator
 
         GeminiService._log_directory = logging_directory
 
         GeminiService._rate_limit_delay = rate_limit_delay
 
         GeminiService._json_mode = json_mode
+        GeminiService._response_schema = response_schema
 
         # if a semaphore is not provided, set it to the default value based on the model
-        semaphore_values = {"gemini-1.5-pro-latest": 2}
+        ## rate limits for 1.5 models are 2 requests per second
+        ## rate limits for 1.0B models are 15 requests per second
+        semaphore_values = {"gemini-1.5-pro": 2,
+                            "gemini-1.5-flash": 2,
+                            "gemini-1.5-pro-latest": 2,
+                            "gemini-1.5-flash-latest": 2,
+                            }
+        
         GeminiService._semaphore_value = semaphore or semaphore_values.get(GeminiService._model, 15)
+        GeminiService._semaphore = asyncio.Semaphore(GeminiService._semaphore_value)
+
+        if(GeminiService._json_mode and GeminiService._model in VALID_JSON_GEMINI_MODELS and response_schema is not None):
+            GeminiService._default_translation_instructions = "Please translate the following text into English. Make sure to return the translated text in JSON format. The JSON should be in the format specified in the response schema."
 
-        if(GeminiService._json_mode and GeminiService._model == "gemini-1.5-pro-latest"):
-            GeminiService._default_translation_instructions = "Please translate the following text into English. Make sure to return the translated text in JSON format. The JSON should be in the following format: {\"text\": \"translated text\"}"
+        elif(GeminiService._json_mode and GeminiService._model in VALID_JSON_GEMINI_MODELS):
+            GeminiService._default_translation_instructions = "Please translate the following text into English. Make sure to return the translated text in JSON format."
 
         elif(GeminiService._json_mode):
-            raise EasyTLException("JSON mode for Gemini is only supported for the gemini-1.5-pro-latest model.")
+            allowed_models_string = ", ".join(VALID_JSON_GEMINI_MODELS)
+            raise EasyTLException(f"JSON mode for Gemini is only supported for the following models: {allowed_models_string}")
         
         else:
             GeminiService._default_translation_instructions = "Please translate the following text into English."
         
 ##-------------------start-of-_redefine_client()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
@@ -153,27 +169,28 @@
         """
 
         response_mime_type = "application/json" if GeminiService._json_mode else "text/plain"
         
         gen_model_params = {
             "model_name": GeminiService._model,
             "safety_settings": GeminiService._safety_settings,
-            "system_instruction": GeminiService._system_message if GeminiService._model == "gemini-1.5-pro-latest" else None
+            "system_instruction": GeminiService._system_message if GeminiService._model in VALID_SYSTEM_MESSAGE_MODELS else None
         }
         
         GeminiService._client = genai.GenerativeModel(**gen_model_params)
         
         generation_config_params = {
             "candidate_count": GeminiService._candidate_count,
             "stop_sequences": GeminiService._stop_sequences,
             "max_output_tokens": GeminiService._max_output_tokens,
             "temperature": GeminiService._temperature,
             "top_p": GeminiService._top_p,
             "top_k": GeminiService._top_k,
-            "response_mime_type": response_mime_type
+            "response_mime_type": response_mime_type,
+            "response_schema": GeminiService._response_schema if GeminiService._response_schema and GeminiService._json_mode else None
         }
         
         GeminiService._generation_config = GenerationConfig(**generation_config_params)
         
         GeminiService._semaphore = asyncio.Semaphore(GeminiService._semaphore_value)
 
 ##-------------------start-of-_redefine_client_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
@@ -264,15 +281,15 @@
         text_to_translate (string) : The text to translate.
 
         Returns:
         _response (GenerateContentResponse) : The translation.
 
         """
 
-        text_request = f"{text_to_translate}" if GeminiService._model == "gemini--1.5-pro-latest" else f"{GeminiService._system_message}\n{text_to_translate}"
+        text_request = f"{text_to_translate}" if GeminiService._model in VALID_SYSTEM_MESSAGE_MODELS else f"{GeminiService._system_message}\n{text_to_translate}"
 
         _response = GeminiService._client.generate_content(
             contents=text_request,
             generation_config=GeminiService._generation_config,
             safety_settings=GeminiService._safety_settings,
             stream=GeminiService._stream
         )
@@ -297,15 +314,15 @@
         """
 
         async with GeminiService._semaphore:
 
             if(GeminiService._rate_limit_delay is not None):
                 await asyncio.sleep(GeminiService._rate_limit_delay)
 
-            text_request = f"{text_to_translate}" if GeminiService._model == "gemini--1.5-pro-latest" else f"{GeminiService._system_message}\n{text_to_translate}"
+            text_request = f"{text_to_translate}" if GeminiService._model in VALID_SYSTEM_MESSAGE_MODELS else f"{GeminiService._system_message}\n{text_to_translate}"
 
             _response = await GeminiService._client.generate_content_async(
                 contents=text_request,
                 generation_config=GeminiService._generation_config,
                 safety_settings=GeminiService._safety_settings,
                 stream=GeminiService._stream
             )
```

### Comparing `easytl-0.3.3/src/easytl/googletl_service.py` & `easytl-0.4.0a0/src/easytl/googletl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.3/src/easytl/openai_service.py` & `easytl-0.4.0a0/src/easytl/openai_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.3/src/easytl/util.py` & `easytl-0.4.0a0/src/easytl/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,80 @@
 ## Copyright Bikatr7 (https://github.com/Bikatr7)
 ## Use of this source code is governed by a GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
+import json
+import logging
 
 ## third-party libraries
 import tiktoken
+import backoff
 
 ## custom modules
 import google.generativeai as genai
-from .exceptions import InvalidEasyTLSettingsException
+
+from .exceptions import InvalidEasyTLSettingsException, GoogleAPIError
+from .classes import NotGiven, NOT_GIVEN
+
+##-------------------start-of-_return_curated_anthropic_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def _return_curated_anthropic_settings(local_settings:dict[str, typing.Any]) -> dict:
+
+    """
+
+    Returns the curated Anthropic settings.
+
+    What this does is it takes local_settings from the calling function, and then returns a dictionary with the settings that are relevant to Anthropic that were converted to the correct type.
+
+    """
+
+    _settings = {
+    "anthropic_model": "",
+    "anthropic_temperature": "",
+    "anthropic_top_p": "",
+    "anthropic_top_k": "",
+    "anthropic_stop_sequences": "",
+    "anthropic_max_output_tokens": "",
+    }
+
+    _non_anthropic_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type", "semaphore", "translation_delay"]
+    _custom_validation_params = ["anthropic_stop_sequences", "anthropic_response_schema"]
+
+    for _key in _settings.keys():
+        param_name = _key.replace("anthropic_", "")
+        if(param_name in local_settings and _key not in _non_anthropic_params and _key not in _custom_validation_params):
+            _settings[_key] = _convert_to_correct_type(_key, local_settings[param_name])
+
+    return _settings
 
 ##-------------------start-of-_return_curated_gemini_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _return_curated_gemini_settings(local_settings:dict[str, typing.Any]) -> dict:
 
+    """
+    
+    Returns the curated Gemini settings.
+
+    What this does is it takes local_settings from the calling function, and then returns a dictionary with the settings that are relevant to Gemini that were converted to the correct type.
+    
+    """
+
     _settings = {
     "gemini_model": "",
     "gemini_temperature": "",
     "gemini_top_p": "",
     "gemini_top_k": "",
     "gemini_stop_sequences": "",
     "gemini_max_output_tokens": ""
     }
 
     _non_gemini_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type", "semaphore", "translation_delay"]
-    _custom_validation_params = ["gemini_stop_sequences"]
+    _custom_validation_params = ["gemini_stop_sequences", "gemini_response_schema"]
 
     for _key in _settings.keys():
         param_name = _key.replace("gemini_", "")
         if(param_name in local_settings and _key not in _non_gemini_params and _key not in _custom_validation_params):
             _settings[_key] = _convert_to_correct_type(_key, local_settings[param_name])
 
     return _settings
@@ -39,43 +83,67 @@
 
 def _return_curated_openai_settings(local_settings:dict[str, typing.Any]) -> dict:
         
         """
         
         Returns the curated OpenAI settings.
 
-        What this does is it takes local_settings from the calling function, and then returns a dictionary with the settings that are relevant to OpenA that were converted to the correct type.
+        What this does is it takes local_settings from the calling function, and then returns a dictionary with the settings that are relevant to OpenAI that were converted to the correct type.
 
         """
 
         _settings = {
         "openai_model": "",
         "openai_temperature": "",
         "openai_top_p": "",
         "openai_stop": "",
         "openai_max_tokens": "",
         "openai_presence_penalty": "",
         "openai_frequency_penalty": ""
         }
 
-        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type", "semaphore", "translation_delay"]
+        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type", "response_schema", "semaphore", "translation_delay"]
         _custom_validation_params = ["openai_stop"]
 
         for _key in _settings.keys():
             param_name = _key.replace("openai_", "")
             if(param_name in local_settings and _key not in _non_openai_params and _key not in _custom_validation_params):
                 _settings[_key] = _convert_to_correct_type(_key, local_settings[param_name])
 
         return _settings
 
 ##-------------------start-of-_return_curated_gemini_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def _validate_stop_sequences(stop_sequences:typing.List[str] | None) -> None:
+def _validate_stop_sequences(stop_sequences:typing.List[str] | None | NotGiven) -> None:
+
+    assert stop_sequences in [None, NOT_GIVEN] or isinstance(stop_sequences, str) or (hasattr(stop_sequences, '__iter__') and all(isinstance(i, str) for i in stop_sequences)), InvalidEasyTLSettingsException("Invalid stop sequences. Must be a string or a list of strings.") # type: ignore
+
+##-------------------start-of-_validate_response_schema()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def _validate_response_schema(response_schema:str | typing.Mapping[str, typing.Any] | None = None) -> typing.Mapping[str, typing.Any] | None:
+
+    if(response_schema is None):
+        return None
+
+    if(isinstance(response_schema, str)):
+        try:
+            return json.loads(response_schema)
+        except json.JSONDecodeError:
+            raise InvalidEasyTLSettingsException("Invalid response_schema. Must be a valid JSON string or None.")
+
+    if(isinstance(response_schema, dict)):
+
+        try:
+            json.dumps(response_schema)
+            return response_schema
+        
+        except (TypeError, OverflowError):
+            raise InvalidEasyTLSettingsException("Invalid response_schema. Must be a valid JSON object or None.")
 
-    assert stop_sequences is None or isinstance(stop_sequences, str) or (hasattr(stop_sequences, '__iter__') and all(isinstance(i, str) for i in stop_sequences)), InvalidEasyTLSettingsException("Invalid stop sequences. Must be a string or a list of strings.")
+    raise InvalidEasyTLSettingsException("Invalid response_schema. Must be a valid JSON, a valid JSON string, or None.")
 
 ##-------------------start-of-_string_to_bool()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _string_to_bool(string:str) -> bool:
 
     return string.lower() in ['true', '1', 'yes', 'y', 't']
 
@@ -95,17 +163,18 @@
         _iterator = iter(value)
         
     except TypeError:
         return False
     
     return all(isinstance(_item, str) for _item in _iterator)
 
-##-------------------start-of-_count_tokens()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+##-------------------start-of-_gemini_count_tokens()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def _count_tokens(text:str) -> int:
+@backoff.on_exception(backoff.expo, exception=(GoogleAPIError), logger=logging.getLogger(), max_tries=50, raise_on_giveup=True)
+def _gemini_count_tokens(text:str, model:str="gemini-pro") -> int:
 
     """
 
     Counts the number of tokens in the given text.
 
     Parameters:
     text (string) : The text to count tokens in.
@@ -115,15 +184,15 @@
 
     """
 
     return genai.GenerativeModel("gemini-pro").count_tokens(text).total_tokens
 
 ##-------------------start-of-_validate_easytl_translation_settings()--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def _validate_easytl_translation_settings(settings:dict, type:typing.Literal["gemini","openai"]) -> None:
+def _validate_easytl_translation_settings(settings:dict, type:typing.Literal["gemini","openai", "anthropic"]) -> None:
 
     """
 
     Validates the Kijiku Rules.json file.
 
     Parameters:
     settings (dict) : The settings to validate.
@@ -158,29 +227,42 @@
         "gemini_top_k",
     ##    "gemini_candidate_count",
     ##    "gemini_stream",
   ##      "gemini_stop_sequences",
         "gemini_max_output_tokens"
     ]
 
-    _validation_rules = {
+    _anthropic_keys = [
+        "anthropic_model",
+        "anthropic_temperature",
+        "anthropic_top_p",
+        "anthropic_top_k",
+    ##    "anthropic_stream",
+    ##    "anthropic_stop_sequences",
+        "anthropic_max_output_tokens"
+    ]
 
-        "openai_model": lambda x: isinstance(x, str) and x in ALLOWED_OPENAI_MODELS,
-        "openai_temperature": lambda x: isinstance(x, float) and 0 <= x <= 2,
-        "openai_top_p": lambda x: isinstance(x, float) and 0 <= x <= 1,
-        "openai_max_tokens": lambda x: x is None or isinstance(x, int) and x > 0,
-        "openai_presence_penalty": lambda x: isinstance(x, float) and -2 <= x <= 2,
-        "openai_frequency_penalty": lambda x: isinstance(x, float) and -2 <= x <= 2,
-        "gemini_model": lambda x: isinstance(x, str) and x in ALLOWED_GEMINI_MODELS,
-        "gemini_prompt": lambda x: x not in ["", "None", None],
-        "gemini_temperature": lambda x: isinstance(x, float) and 0 <= x <= 2,
-        "gemini_top_p": lambda x: x is None or (isinstance(x, float) and 0 <= x <= 2),
-        "gemini_top_k": lambda x: x is None or (isinstance(x, int) and x >= 0),
-        "gemini_max_output_tokens": lambda x: x is None or isinstance(x, int),
-##        "gemini_stop_sequences": lambda x: x is None or all(isinstance(i, str) for i in x)
+    _validation_rules = {
+        "openai_model": lambda x: isinstance(x, str) and x in ALLOWED_OPENAI_MODELS or x is None or x is NOT_GIVEN,
+        "openai_temperature": lambda x: isinstance(x, (int, float)) and 0 <= x <= 2 or x is None or x is NOT_GIVEN,
+        "openai_top_p": lambda x: isinstance(x, (int, float)) and 0 <= x <= 1 or x is None or x is NOT_GIVEN,
+        "openai_max_tokens": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, int) and x > 0),
+        "openai_presence_penalty": lambda x: isinstance(x, (int, float)) and -2 <= x <= 2 or x is None or x is NOT_GIVEN,
+        "openai_frequency_penalty": lambda x: isinstance(x, (int, float)) and -2 <= x <= 2 or x is None or x is NOT_GIVEN,
+        "gemini_model": lambda x: isinstance(x, str) and x in ALLOWED_GEMINI_MODELS or x is None or x is NOT_GIVEN,
+        "gemini_prompt": lambda x: x not in ["", "None", None, NOT_GIVEN],
+        "gemini_temperature": lambda x: isinstance(x, (int, float)) and 0 <= x <= 2 or x is None or x is NOT_GIVEN,
+        "gemini_top_p": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, (int, float)) and 0 <= x <= 2),
+        "gemini_top_k": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, int) and x >= 0),
+        "gemini_max_output_tokens": lambda x: x is None or x is NOT_GIVEN or isinstance(x, int),
+        "anthropic_model": lambda x: isinstance(x, str) and x in ALLOWED_ANTHROPIC_MODELS or x is None or x is NOT_GIVEN,
+        "anthropic_temperature": lambda x: isinstance(x, (int, float)) and 0 <= x <= 1 or x is None or x is NOT_GIVEN,
+        "anthropic_top_p": lambda x: isinstance(x, (int, float)) and 0 <= x <= 1 or x is None or x is NOT_GIVEN,
+        "anthropic_top_k": lambda x: isinstance(x, int) and x > 0 or x is None or x is NOT_GIVEN,
+        "anthropic_max_output_tokens": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, int) and x > 0)
     }
     
     try:
 
         ## assign to variables to reduce repetitive access    
         if(type == "openai"):
 
@@ -205,14 +287,24 @@
             ## _validate each _key using the validation rules
             for _key, _validate in _validation_rules.items():
                 if (_key in settings and not _validate(settings[_key])):
                     raise ValueError(f"Invalid _value for {_key}")
                 
         ##    settings["gemini_stream"] = False
       ##      settings["gemini_candidate_count"] = 1
+
+        elif(type == "anthropic"):
+
+            ## ensure all keys are present
+            assert all(_key in settings for _key in _anthropic_keys)
+
+            ## _validate each _key using the validation rules
+            for _key, _validate in _validation_rules.items():
+                if (_key in settings and not _validate(settings[_key])):
+                    raise ValueError(f"Invalid _value for {_key}")
         
     except Exception as e:
         raise InvalidEasyTLSettingsException(f"Invalid settings, Due to: {str(e)}")
 
 ##-------------------start-of-_convert_to_correct_type()-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _convert_to_correct_type(setting_name:str, initial_value:str) -> typing.Any:
@@ -229,34 +321,41 @@
     (typing.Any) : The converted value.
 
     """
 
     _value = initial_value
     
     _type_expectations = {
-        "openai_model": {"_type": str, "constraints": lambda x: x in ALLOWED_OPENAI_MODELS},
-       ## "openai_system_message": {"_type": str, "constraints": lambda x: x not in ["", "None", None]},
-        "openai_temperature": {"_type": float, "constraints": lambda x: 0 <= x <= 2},
-        "openai_top_p": {"_type": float, "constraints": lambda x: 0 <= x <= 2},
-       ## "openai_n": {"_type": int, "constraints": lambda x: x == 1},
-    ##    "openai_stream": {"_type": bool, "constraints": lambda x: x is False},
-      ##  "openai_stop": {"_type": None, "constraints": lambda x: x is None},
-    ##    "openai_logit_bias": {"_type": None, "constraints": lambda x: x is None},
-        "openai_max_tokens": {"_type": int, "constraints": lambda x: x is None or isinstance(x, int)},
-        "openai_presence_penalty": {"_type": float, "constraints": lambda x: -2 <= x <= 2},
-        "openai_frequency_penalty": {"_type": float, "constraints": lambda x: -2 <= x <= 2},
-        "gemini_model": {"_type": str, "constraints": lambda x: x in ALLOWED_GEMINI_MODELS},
-       ## "gemini_prompt": {"_type": str, "constraints": lambda x: x not in ["", "None", None]},
-        "gemini_temperature": {"_type": float, "constraints": lambda x: 0 <= x <= 2},
-        "gemini_top_p": {"_type": float, "constraints": lambda x: x is None or (isinstance(x, float) and 0 <= x <= 2)},
-        "gemini_top_k": {"_type": int, "constraints": lambda x: x is None or x >= 0},
-  ##      "gemini_candidate_count": {"_type": int, "constraints": lambda x: x == 1},
-      ##  "gemini_stream": {"_type": bool, "constraints": lambda x: x is False},
-   ## "gemini_stop_sequences": {"_type": list, "constraints": lambda x: x is None or all(isinstance(i, str) for i in x)},
-        "gemini_max_output_tokens": {"_type": int, "constraints": lambda x: x is None or isinstance(x, int)},
+        "openai_model": {"_type": str, "constraints": lambda x: x in ALLOWED_OPENAI_MODELS or x is None or x is NOT_GIVEN},
+        ## "openai_system_message": {"_type": str, "constraints": lambda x: x not in ["", "None", None, NOT_GIVEN]},
+        "openai_temperature": {"_type": float, "constraints": lambda x: isinstance(x, (int, float)) and 0 <= x <= 2 or x is None or x is NOT_GIVEN},
+        "openai_top_p": {"_type": float, "constraints": lambda x: isinstance(x, (int, float)) and 0 <= x <= 2 or x is None or x is NOT_GIVEN},
+        ## "openai_n": {"_type": int, "constraints": lambda x: x == 1},
+        ## "openai_stream": {"_type": bool, "constraints": lambda x: x is False},
+        ## "openai_stop": {"_type": None, "constraints": lambda x: x is None or x is NOT_GIVEN},
+        ## "openai_logit_bias": {"_type": None, "constraints": lambda x: x is None or x is NOT_GIVEN},
+        "openai_max_tokens": {"_type": int, "constraints": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, int) and x > 0)},
+        "openai_presence_penalty": {"_type": float, "constraints": lambda x: isinstance(x, (int, float)) and -2 <= x <= 2 or x is None or x is NOT_GIVEN},
+        "openai_frequency_penalty": {"_type": float, "constraints": lambda x: isinstance(x, (int, float)) and -2 <= x <= 2 or x is None or x is NOT_GIVEN},
+        "gemini_model": {"_type": str, "constraints": lambda x: x in ALLOWED_GEMINI_MODELS or x is None or x is NOT_GIVEN},
+        ## "gemini_prompt": {"_type": str, "constraints": lambda x: x not in ["", "None", None, NOT_GIVEN]},
+        "gemini_temperature": {"_type": float, "constraints": lambda x: isinstance(x, (int, float)) and 0 <= x <= 2 or x is None or x is NOT_GIVEN},
+        "gemini_top_p": {"_type": float, "constraints": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, float) and 0 <= x <= 2)},
+        "gemini_top_k": {"_type": int, "constraints": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, int) and x >= 0)},
+        ## "gemini_candidate_count": {"_type": int, "constraints": lambda x: x == 1},
+        ## "gemini_stream": {"_type": bool, "constraints": lambda x: x is False},
+        ## "gemini_stop_sequences": {"_type": list, "constraints": lambda x: x is None or x is NOT_GIVEN or all(isinstance(i, str) for i in x)},
+        "gemini_max_output_tokens": {"_type": int, "constraints": lambda x: x is None or x is NOT_GIVEN or isinstance(x, int)},
+        "anthropic_model": {"_type": str, "constraints": lambda x: x in ALLOWED_ANTHROPIC_MODELS or x is None or x is NOT_GIVEN},
+        "anthropic_temperature": {"_type": float, "constraints": lambda x: isinstance(x, (int, float)) and 0 <= x <= 1 or x is None or x is NOT_GIVEN},
+        "anthropic_top_p": {"_type": float, "constraints": lambda x: isinstance(x, (int, float)) and 0 <= x <= 1 or x is None or x is NOT_GIVEN},
+        "anthropic_top_k": {"_type": int, "constraints": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, int) and x > 0)},
+        ## "anthropic_stream": {"_type": bool, "constraints": lambda x: x is False},
+        ## "anthropic_stop_sequences": {"_type": list, "constraints": lambda x: x is None or x is NOT_GIVEN or all(isinstance(i, str) for i in x)},
+        "anthropic_max_output_tokens": {"_type": int, "constraints": lambda x: x is None or x is NOT_GIVEN or (isinstance(x, int) and x > 0)}
     }
 
     if(setting_name not in _type_expectations):
         raise ValueError("Invalid setting name")
 
     _setting_info = _type_expectations[setting_name]
 
@@ -265,18 +364,24 @@
 
     elif(isinstance(initial_value, str) and initial_value.lower() in ["none","null"]):
         _value = None
 
     if(_setting_info["_type"] is None):
         _converted_value = None
 
+    elif(_setting_info["_type"] == NOT_GIVEN or NotGiven):
+        _converted_value = NOT_GIVEN
+
     elif(_setting_info["_type"] == int) or (_setting_info["_type"] == float):
 
         if(_value is None or _value == ''):
             _converted_value = None
+
+        elif(_value == "NOT_GIVEN" or _value == NotGiven or _value == NOT_GIVEN):
+            _converted_value = NOT_GIVEN
             
         elif(_setting_info["_type"] == int):
             _converted_value = int(_value)
 
         else:
             _converted_value = float(_value)
 
@@ -305,15 +410,15 @@
     Returns:
     _num_tokens (int) : the number of tokens used.
     _min_cost (float) : the minimum cost of translation.
     model (string) : the model used to translate the text.
 
     """
 
-    assert model in ALLOWED_OPENAI_MODELS or model in ALLOWED_GEMINI_MODELS, f"""EasyTL does not support : {model}"""
+    assert model in ALLOWED_OPENAI_MODELS + ALLOWED_GEMINI_MODELS + ALLOWED_ANTHROPIC_MODELS, f"""EasyTL does not support : {model}"""
 
     ## default models are first, then the rest are sorted by price case
     if(price_case is None):
 
         if(model == "gpt-3.5-turbo"):
             print("Warning: gpt-3.5-turbo may change over time. Estimating cost assuming gpt-3.5-turbo-0125 as it is the most recent version of gpt-3.5-turbo.")
             return _estimate_cost(text, model="gpt-3.5-turbo-0125")
@@ -417,60 +522,96 @@
             print(f"Warning: gemini-1.0-pro-latest may change over time. Estimating cost assuming gemini-1.0-pro-001 as it is the most recent version of gemini-1.0-pro.")
             return _estimate_cost(text, model="gemini-1.0-pro-001", price_case=8)
         
         elif(model == "gemini-1.0-pro-vision-latest"):
             print("Warning: gemini-1.0-pro-vision-latest may change over time. Estimating cost assuming gemini-1.0-pro-vision-001 as it is the most recent version of gemini-1.0-pro-vision.")
             return _estimate_cost(text, model="gemini-1.0-pro-vision-001", price_case=8)
         
+        elif(model == "gemini-1.5-pro"):
+            return _estimate_cost(text, model=model, price_case=9)
+        
+        elif(model == "gemini-1.5-flash"):
+            return _estimate_cost(text, model=model, price_case=9)
+
         elif(model == "gemini-1.5-pro-latest"):
-            return _estimate_cost(text, model=model, price_case=8)
+            print("Warning: gemini-1.5-pro-latest may change over time. Estimating cost assuming gemini-1.5-pro as it is the most recent version of gemini-1.5-pro.")
+            return _estimate_cost(text, model="gemini-1.5-pro", price_case=9)
+        
+        elif(model == "gemini-1.5-flash-latest"):
+            print("Warning: gemini-1.5-flash-latest may change over time. Estimating cost assuming gemini-1.5-flash as it is the most recent version of gemini-1.5-flash.")
+            return _estimate_cost(text, model="gemini-1.5-flash", price_case=9)
         
   ##      elif(model == "gemini-1.0-ultra-latest"):
       ##      return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gemini-1.0-pro-001"):
             return _estimate_cost(text, model=model, price_case=8)
         
         elif(model == "gemini-1.0-pro-vision-001"):
             return _estimate_cost(text, model=model, price_case=8)
         
+        elif(model == "claude-3-opus-20240229"):
+            return _estimate_cost(text, model=model, price_case=13)
+        
+        elif(model == "claude-3-sonnet-20240229"):
+            return _estimate_cost(text, model=model, price_case=12)
+        
+        elif(model == "claude-3-haiku-20240307"):
+            return _estimate_cost(text, model=model, price_case=11)
+        
     else:
 
         _cost_details = MODEL_COSTS.get(model)
 
         if(not _cost_details):
             raise ValueError(f"Cost details not found for model: {model}.")
 
         ## break down the text into a string than into tokens
         text = ''.join(text)
 
-        _LLM_TYPE = "openai" if model in ALLOWED_OPENAI_MODELS else "gemini"
-
+        model_types = {
+            "openai": ALLOWED_OPENAI_MODELS,
+            "gemini": ALLOWED_GEMINI_MODELS,
+            "anthropic": ALLOWED_ANTHROPIC_MODELS
+        }
+        
+        _LLM_TYPE = next((model_type for model_type, allowed_models in model_types.items() if model in allowed_models))
 
         if(_LLM_TYPE == "openai"):
             _encoding = tiktoken.encoding_for_model(model)
             _num_tokens = len(_encoding.encode(text))
 
+        elif(_LLM_TYPE == "gemini"):
+            ## no local option, and it seems to rate limit too lol, so we'll try 5 times before giving up and doing it openai style
+            try:
+                _num_tokens = _gemini_count_tokens(text, model=model)
+            except:
+                _encoding = tiktoken.encoding_for_model("gpt-4-turbo-0125")
+                _num_tokens = len(_encoding.encode(text))
+
         else:
-            _num_tokens = _count_tokens(text)
+            ## literally no way exists to get the number of tokens for anthropic, so we'll just use the gpt-4-turbo-0125 model as a stand-in
+            _encoding = tiktoken.encoding_for_model("gpt-4-turbo-0125")
+            _num_tokens = len(_encoding.encode(text))
+            pass
 
         _input_cost = _cost_details["_input_cost"]
         _output_cost = _cost_details["_output_cost"]
 
         _min_cost_for_input = (_num_tokens / 1000) * _input_cost
         _min_cost_for_output = (_num_tokens / 1000) * _output_cost
         _min_cost = _min_cost_for_input + _min_cost_for_output
 
         return _num_tokens, _min_cost, model
     
-    ## _type checker doesn't like the chance of None being returned, so we raise an exception here if it gets to this point, which it shouldn't
+    ## type checker doesn't like the chance of None being returned, so we raise an exception here if it gets to this point, which it shouldn't
     raise Exception("An unknown error occurred while calculating the minimum cost of translation.")
 
 ##-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-18
+## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-05-19
 ## https://platform.openai.com/docs/models/overview
 ALLOWED_OPENAI_MODELS  = [
     "gpt-3.5-turbo",
     "gpt-3.5-turbo-0301",
     "gpt-3.5-turbo-0125",
     "gpt-3.5-turbo-0613",
     "gpt-3.5-turbo-1106",
@@ -491,54 +632,64 @@
     "gpt-4-1106-vision-preview",
     "gpt-4o",
     "gpt-4o-2024-05-13"
 ]
 
 VALID_JSON_OPENAI_MODELS = [
     "gpt-3.5-turbo-0125",
+    "gpt-3.5-turbo",
     "gpt-4-turbo",
     "gpt-4-turbo-preview",
     "gpt-4-turbo-2024-04-09",
     "gpt-4-0125-preview",
     "gpt-4-1106-preview",
     "gpt-4-vision-preview",
     "gpt-4-1106-vision-preview",
     "gpt-4o-2024-05-13",
     "gpt-4o"    
 ]
 
-## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-18
 ## https://ai.google.dev/models/gemini
 ALLOWED_GEMINI_MODELS = [
     "gemini-1.0-pro-001",
     "gemini-1.0-pro",
     "gemini-1.0-pro-latest",
     "gemini-1.0-pro-vision-001",
     "gemini-1.0-pro-vision",
     "gemini-1.0-pro-vision-latest",
     "gemini-1.5-pro-latest",
+    "gemini-1.5-pro",
+    "gemini-1.5-flash-latest",
+    "gemini-1.5-flash",
   ##  "gemini-1.0-ultra-latest",
     "gemini-pro",
     "gemini-pro-vision",
   ##  "gemini-ultra"
 ]
 
+VALID_JSON_GEMINI_MODELS = [
+    "gemini-1.5-pro-latest",
+    "gemini-1.5-pro",
+    "gemini-1.5-flash-latest",
+    "gemini-1.5-flash",
+]
+
+## https://docs.anthropic.com/en/docs/models-overview
 ALLOWED_ANTHROPIC_MODELS = [
     "claude-3-opus-20240229",
     "claude-3-sonnet-20240229",
     "claude-3-haiku-20240307"
 ]
 
 VALID_JSON_ANTHROPIC_MODELS = [
     "claude-3-opus-20240229",
     "claude-3-sonnet-20240229",
     "claude-3-haiku-20240307"
 ]
 
-## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-05-13
 MODEL_COSTS = {
     # Grouping GPT-3.5 models together
     "gpt-3.5-turbo-0125": {"price_case": 7, "_input_cost": 0.0005, "_output_cost": 0.0015},
     "gpt-3.5-turbo-0301": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-0613": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-1106": {"price_case": 2, "_input_cost": 0.0010, "_output_cost": 0.0020},
     "gpt-3.5-turbo-16k-0613": {"price_case": 3, "_input_cost": 0.0030, "_output_cost": 0.0040},
@@ -564,14 +715,45 @@
     "gemini-1.0-pro-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.0-pro-vision-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.5-pro-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
  ##   "gemini-1.0-ultra-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-pro": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-pro-vision": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
  ##   "gemini-ultra": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0}
+    "gemini-1.5-pro": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-1.5-flash-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
+    "gemini-1.5-flash": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
 
     ## grouping anthropic models together
     "claude-3-haiku-20240307": {"price_case": 11, "_input_cost": 0.00025, "_output_cost": 0.00125},
     "claude-3-sonnet-20240229": {"price_case": 12, "_input_cost": 0.003, "_output_cost": 0.015},
     "claude-3-opus-20240229": {"price_case": 13, "_input_cost": 0.015, "_output_cost": 0.075}
 
+}
+
+MODEL_MAX_TOKENS = {
+
+    ## openai models
+    "gpt-4o-2024-05-13": {"max_input_tokens": 128000, "max_output_tokens": 4096},
+    "gpt-4-turbo-2024-04-09": {"max_input_tokens": 128000, "max_output_tokens": 4096},
+    "gpt-4-0125-preview": {"max_input_tokens": 128000, "max_output_tokens": 4096},
+    "gpt-4-1106-preview": {"max_input_tokens": 128000, "max_output_tokens": 4096},
+    "gpt-4-1106-vision-preview": {"max_input_tokens": 128000, "max_output_tokens": 4096},
+    "gpt-4-0613": {"max_input_tokens": 8192, "max_output_tokens": 4096},
+    "gpt-4-32k-0613": {"max_input_tokens": 32768, "max_output_tokens": 4096},
+    "gpt-3.5-turbo-0125": {"max_input_tokens": 16385, "max_output_tokens": 4096},
+    "gpt-3.5-turbo-1106": {"max_input_tokens": 16385, "max_output_tokens": 4096},
+    "gpt-3.5-turbo-0613": {"max_input_tokens": 4096, "max_output_tokens": 4096},
+    "gpt-3.5-turbo-16k-0613": {"max_input_tokens": 16385, "max_output_tokens": 4096},
+
+    ## gemini models
+    "gemini-1.5-pro": {"max_input_tokens": 1048576, "max_output_tokens": 8192},
+    "gemini-1.5-flash": {"max_input_tokens": 1048576, "max_output_tokens": 8192},
+    "gemini-1.0-pro-001": {"max_input_tokens": 12288, "max_output_tokens": 4096},
+    "gemini-1.0-pro-vision-001": {"max_input_tokens": 12288, "max_output_tokens": 4096},
+
+    ## anthropic models
+    "claude-3-opus-20240229": {"max_input_tokens": 200000, "max_output_tokens": 4096},
+    "claude-3-sonnet-20240229": {"max_input_tokens": 200000, "max_output_tokens": 4096},
+    "claude-3-haiku-20240307": {"max_input_tokens": 200000, "max_output_tokens": 4096}
+
 }
```

### Comparing `easytl-0.3.3/src/easytl.egg-info/PKG-INFO` & `easytl-0.4.0a0/src/easytl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.3.3
+Version: 0.4.0a0
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.3
+Requires-Dist: google-generativeai==0.5.4
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.29.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: google-cloud-translate==3.15.3
+Requires-Dist: anthropic==0.26.0
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
 - [Quick Start](#quick-start)
 - [Installation](#installation)
 - [Features](#features)
```

### Comparing `easytl-0.3.3/src/easytl.egg-info/SOURCES.txt` & `easytl-0.4.0a0/src/easytl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 src/easytl/version.py
 src/easytl.egg-info/PKG-INFO
 src/easytl.egg-info/SOURCES.txt
 src/easytl.egg-info/dependency_links.txt
 src/easytl.egg-info/requires.txt
 src/easytl.egg-info/top_level.txt
 tests/issue_template.py
-tests/passing.py
+tests/passing.py
+tests/simple_test.py
```

### Comparing `easytl-0.3.3/tests/passing.py` & `easytl-0.4.0a0/tests/passing.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import os
 import time
 import logging
 
 import backoff
 
-from easytl.exceptions import DeepLException, GoogleAPIError, OpenAIError
+from easytl.exceptions import DeepLException, GoogleAPIError, OpenAIError, AnthropicAPIError
 
 ##-------------------start-of-read_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def read_api_key(filename):
     try:
         with open(filename, 'r') as file:
             return file.read().strip()
@@ -22,14 +22,15 @@
 def setup_preconditions():
 
     gemini_time_delay = 30
 
     deepl_api_key = os.environ.get('DEEPL_API_KEY')
     gemini_api_key = os.environ.get('GEMINI_API_KEY')
     openai_api_key = os.environ.get('OPENAI_API_KEY')
+    anthropic_api_key = os.environ.get('ANTHROPIC_API_KEY')
     json_value = os.environ.get('GOOGLE_TRANSLATE_SERVICE_KEY_VALUE')
 
     if(json_value is not None):
 
         with open("json_value.txt", "w") as file:
             file.write(json_value)
 
@@ -39,40 +40,59 @@
 
     if(deepl_api_key is None):
         deepl_api_key = read_api_key("tests/deepl.txt")
     if(gemini_api_key is None):
         gemini_api_key = read_api_key("tests/gemini.txt")
     if(openai_api_key is None):
         openai_api_key = read_api_key("tests/openai.txt")
+    if(anthropic_api_key is None):
+        anthropic_api_key = read_api_key("tests/anthropic.txt")
 
     if(json_value is None):
         google_tl_key_path = "tests/google_translate_key.json"
         
         logging_directory = "tests/"
         gemini_time_delay = 5
 
     assert deepl_api_key is not None, "DEEPL_API_KEY environment variable must be set"
     assert gemini_api_key is not None, "GEMINI_API_KEY environment variable must be set"
     assert openai_api_key is not None, "OPENAI_API_KEY environment variable must be set"
+    assert anthropic_api_key is not None, "ANTHROPIC_API_KEY environment variable must be set"
     assert google_tl_key_path is not None, "GOOGLE_TRANSLATE_SERVICE_KEY_VALUE environment variable must be set"
 
     EasyTL.set_credentials("deepl", deepl_api_key)
     EasyTL.set_credentials("gemini", gemini_api_key)
     EasyTL.set_credentials("openai", openai_api_key)
+    EasyTL.set_credentials("anthropic", anthropic_api_key)
     EasyTL.set_credentials("google translate", google_tl_key_path)
 
-    return gemini_time_delay, logging_directory
+    schema = {
+        "type": "object",
+        "properties": {
+            "input": {
+                "type": "string",
+                "description": "The text you were given to translate"
+            },
+            "output": {
+                "type": "string",
+                "description": "The translated text"
+            }
+        },
+        "required": ["input", "output"]
+    }
+
+    return gemini_time_delay, logging_directory, schema
 
 ##-------------------start-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def main():
 
-    gemini_time_delay, logging_directory = setup_preconditions()
+    gemini_time_delay, logging_directory, schema = setup_preconditions()
 
-    decorator = backoff.on_exception(backoff.expo, exception=(DeepLException, GoogleAPIError, OpenAIError), logger=logging.getLogger())
+    decorator = backoff.on_exception(backoff.expo, exception=(DeepLException, GoogleAPIError, OpenAIError, AnthropicAPIError), logger=logging.getLogger())
 
     print("------------------------------------------------Deepl------------------------------------------------")
 
     print("------------------------------------------------Text response------------------------------------------------")
 
     print(EasyTL.deepl_translate(text="Hello, world!", target_lang="DE", logging_directory=logging_directory, decorator=decorator))
     print(await EasyTL.deepl_translate_async(text="Hello, world!", target_lang="DE", logging_directory=logging_directory,decorator=decorator))
@@ -148,15 +168,15 @@
         print(result.text) # type: ignore
 
     for result in async_results: # type: ignore
         print(result.text)
 
     print("-----------------------------------------------JSON response-----------------------------------------------")
 
-    print(EasyTL.gemini_translate("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Translate this to German. Format the response as JSON.", response_type="json", logging_directory=logging_directory,decorator=decorator))
+    print(EasyTL.gemini_translate("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Translate this to German. Format the response as JSON parseable string must have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory,decorator=decorator, response_schema=schema))
     
     time.sleep(gemini_time_delay)
     
     print(await EasyTL.gemini_translate_async("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Format the response as JSON parseable string. It should have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory,decorator=decorator))
 
     print("------------------------------------------------Cost calculation------------------------------------------------")
 
@@ -194,14 +214,48 @@
 
     print("------------------------------------------------Cost calculation------------------------------------------------")
 
     tokens, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="openai", model="gpt-3.5-turbo", translation_instructions="Translate this to German.")
 
     print(f"Tokens: {tokens}, Cost: {cost}, Model: {model}")
 
+    print("------------------------------------------------Anthropic------------------------------------------------")
+
+    print("-----------------------------------------------Text response-----------------------------------------------")
+
+    print(EasyTL.anthropic_translate("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
+    print(await EasyTL.anthropic_translate_async("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
+
+    print(EasyTL.anthropic_translate("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator).content[0].text) # type: ignore
+    result = await EasyTL.anthropic_translate_async("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
+
+    print(result.content[0].text) # type: ignore
+
+    print("-----------------------------------------------Raw response-----------------------------------------------")
+
+    results = EasyTL.anthropic_translate(text=["Hello, world!", "Goodbye, world!"], model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
+    async_results = await EasyTL.anthropic_translate_async(text=["Hello, world!", "Goodbye, world!"], model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
+
+    for result in results: # type: ignore
+        print(result.content[0].text) # type: ignore
+
+    for result in async_results: # type: ignore
+        print(result.content[0].text) # type: ignore
+
+    print("-----------------------------------------------JSON response-----------------------------------------------")
+
+    print(EasyTL.anthropic_translate("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German. Format the response as JSON parseable string.", response_type="json", logging_directory=logging_directory,decorator=decorator, response_schema=schema))
+    print(await EasyTL.anthropic_translate_async("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German. Format the response as JSON parseable string.", response_type="json", logging_directory=logging_directory,decorator=decorator, response_schema=schema))
+
+    print("------------------------------------------------Cost calculation------------------------------------------------")
+
+    tokens, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="anthropic", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.")
+
+    print(f"Tokens: {tokens}, Cost: {cost}, Model: {model}")
+
 ##-------------------end-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 
 
 if(__name__ == "__main__"):
     ## setup logging
     logging.basicConfig(level=logging.DEBUG,
```


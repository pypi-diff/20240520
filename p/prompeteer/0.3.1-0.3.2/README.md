# Comparing `tmp/prompeteer-0.3.1.tar.gz` & `tmp/prompeteer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.3.1.tar", last modified: Wed May 15 15:31:05 2024, max compression
+gzip compressed data, was "prompeteer-0.3.2.tar", last modified: Sun May 19 13:47:11 2024, max compression
```

## Comparing `prompeteer-0.3.1.tar` & `prompeteer-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:31:05.938074 prompeteer-0.3.1/
--rw-r--r--   0 yoaz       (502) staff       (20)       42 2024-05-15 15:30:47.000000 prompeteer-0.3.1/MANIFEST.in
--rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-15 15:31:05.937563 prompeteer-0.3.1/PKG-INFO
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:31:05.929825 prompeteer-0.3.1/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3832 2024-05-15 14:32:25.000000 prompeteer-0.3.1/prompeteer/prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:31:05.932713 prompeteer-0.3.1/prompeteer/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1026 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/prompt/prompt.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2628 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/prompt/prompt_config.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:31:05.933772 prompeteer-0.3.1/prompeteer/providers/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/providers/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:31:05.934805 prompeteer-0.3.1/prompeteer/providers/aws_bedrock/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/providers/aws_bedrock/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1955 2024-05-15 15:18:52.000000 prompeteer-0.3.1/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1517 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/providers/aws_bedrock/aws_llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:31:05.935753 prompeteer-0.3.1/prompeteer/providers/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/providers/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1734 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/providers/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3077 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/providers/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1443 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/providers/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)      213 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/providers/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:31:05.936505 prompeteer-0.3.1/prompeteer/utils/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/utils/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3041 2024-05-15 12:42:33.000000 prompeteer-0.3.1/prompeteer/utils/utils.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-15 15:31:05.937063 prompeteer-0.3.1/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-15 15:31:05.000000 prompeteer-0.3.1/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      816 2024-05-15 15:31:05.000000 prompeteer-0.3.1/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-15 15:31:05.000000 prompeteer-0.3.1/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       52 2024-05-15 15:31:05.000000 prompeteer-0.3.1/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-15 15:31:05.000000 prompeteer-0.3.1/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)     3414 2024-05-15 13:59:10.000000 prompeteer-0.3.1/public_README.md
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-15 15:31:05.938144 prompeteer-0.3.1/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      877 2024-05-15 15:31:05.000000 prompeteer-0.3.1/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.395364 prompeteer-0.3.2/
+-rw-r--r--   0 yoaz       (502) staff       (20)       42 2024-05-15 15:30:47.000000 prompeteer-0.3.2/MANIFEST.in
+-rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-19 13:47:11.394972 prompeteer-0.3.2/PKG-INFO
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.385072 prompeteer-0.3.2/prompeteer/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     4142 2024-05-19 11:15:13.000000 prompeteer-0.3.2/prompeteer/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.387885 prompeteer-0.3.2/prompeteer/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      673 2024-05-19 12:43:18.000000 prompeteer-0.3.2/prompeteer/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3171 2024-05-19 13:02:38.000000 prompeteer-0.3.2/prompeteer/prompt/prompt_config.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.388914 prompeteer-0.3.2/prompeteer/providers/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/providers/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.390392 prompeteer-0.3.2/prompeteer/providers/aws_bedrock/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/providers/aws_bedrock/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2085 2024-05-19 13:43:20.000000 prompeteer-0.3.2/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1866 2024-05-19 12:41:47.000000 prompeteer-0.3.2/prompeteer/providers/aws_bedrock/aws_llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.391343 prompeteer-0.3.2/prompeteer/providers/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/providers/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2070 2024-05-19 12:41:18.000000 prompeteer-0.3.2/prompeteer/providers/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3074 2024-05-19 13:17:36.000000 prompeteer-0.3.2/prompeteer/providers/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1445 2024-05-19 11:15:13.000000 prompeteer-0.3.2/prompeteer/providers/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3790 2024-05-19 13:43:20.000000 prompeteer-0.3.2/prompeteer/providers/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.392095 prompeteer-0.3.2/prompeteer/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.2/prompeteer/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1012 2024-05-19 12:43:51.000000 prompeteer-0.3.2/prompeteer/utils/utils.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-19 13:47:11.394412 prompeteer-0.3.2/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      816 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       52 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-19 13:47:11.000000 prompeteer-0.3.2/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)     3414 2024-05-15 13:59:10.000000 prompeteer-0.3.2/public_README.md
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-19 13:47:11.395418 prompeteer-0.3.2/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      877 2024-05-19 13:47:11.000000 prompeteer-0.3.2/setup.py
```

### Comparing `prompeteer-0.3.1/PKG-INFO` & `prompeteer-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.3.1
+Version: 0.3.2
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.3.1/prompeteer/prompeteer.py` & `prompeteer-0.3.2/prompeteer/prompeteer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,89 @@
-# Author: Yoaz Menda
 import csv
 import logging
 import os
 from datetime import datetime
-from typing import List, Literal, Tuple
+from typing import List, Literal, Optional
 
-from prompeteer.providers.llm_request import ILLMRequest
-from prompeteer.providers.llm_client import ILLMClient, get_llm_client
 from prompeteer.prompt.prompt import Variable
-from prompeteer.prompt.prompt_config import load_prompt_config, PromptConfig
+from prompeteer.prompt.prompt_config import PromptConfig
+from prompeteer.providers.llm_client import LLMClient
+from prompeteer.providers.llm_request import LLMRequest
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 clients = {}
 
 
+class Result:
+    def __init__(self, response_text: str, request_text: Optional[str] = None):
+        self.response_text = response_text
+        self.request_text = request_text
+
+
 def run_prompt(prompt_config_file_path: str,
                input_csv: str,
                output_csv: str = None,
                destination: Literal['file', 'console'] = 'console',
                row_numbers_to_process: List[int] = None,
                include_prompt: bool = False):
-    results = _run_prompts(input_csv, prompt_config_file_path, row_numbers_to_process)
+    results = _run_prompts(input_csv, prompt_config_file_path, row_numbers_to_process, include_prompt)
     if destination == 'console':
-        handle_console(include_prompt, results)
+        handle_output_to_console(results)
     elif destination == 'file':
-        handle_file(results, include_prompt, input_csv, output_csv)
+        handle_output_to_file(results, input_csv, output_csv)
 
 
-def _run_prompts(input_csv: str, prompt_config_file_path: str, row_numbers_to_process: List[int]) -> List[
-    Tuple[str, str]]:
-    results: List[Tuple[str, str]] = []
-    prompt_config: PromptConfig = load_prompt_config(prompt_config_file_path)
+def _run_prompts(input_csv: str, prompt_config_file_path: str, row_numbers_to_process: List[int],
+                 include_prompt: bool) -> List[Result]:
+    results: List[Result] = []
+    prompt_config: PromptConfig = PromptConfig.from_file(prompt_config_file_path)
     # Open the input CSV file and process each row
     with open(input_csv, mode='r', newline='', encoding='utf-8') as file:
         reader = csv.DictReader(file, delimiter='|', quotechar='"')
         for csv_row_number, variables_row in enumerate(reader):
             if row_numbers_to_process is None or csv_row_number in row_numbers_to_process:
                 try:
-                    variables_to_inject: List[Variable] = [Variable(name, value) for name, value in variables_row.items()]
-                    llm_request: ILLMRequest = prompt_config.to_llm_request(variables_to_inject)
-                    client: ILLMClient = get_llm_client(prompt_config.llm_provider)
-                    response: str = client.call(llm_request)
-                    results.append((llm_request.get_prompt_text(), response))
+                    csv_row_variables: List[Variable] = [Variable(name, value) for name, value in
+                                                         variables_row.items()]
+                    llm_request: LLMRequest = prompt_config.to_llm_request(variables_to_inject=csv_row_variables)
+                    llm_client = LLMClient.get_client_by_provider(prompt_config.llm_provider)
+                    llm_response_text: str = llm_client.call(llm_request)
+                    prompt_text = llm_request.to_text() if include_prompt else None
+                    results.append(Result(response_text=llm_response_text, request_text=prompt_text))
                 except Exception as e:
                     logger.error(f"Error processing row {csv_row_number}: {e}")
                     continue  # Continue with the next row, logging the error for this one
     return results
 
 
-def handle_file(results: List[Tuple[str, str]], include_prompt: bool, input_csv: str, output_csv: str = None):
+def handle_output_to_file(results: List[Result], input_csv: str, output_csv: str = None):
     if output_csv is None:
         # if not provided, create the output csv file in the same location where the input_csv is located
         output_csv = create_output_file_name(os.path.dirname(input_csv), "result")
     with open(output_csv, 'w', newline='') as out_file:
-        fieldnames = ['request', 'response'] if include_prompt else ['response']
-        writer = csv.DictWriter(out_file, fieldnames=fieldnames, delimiter=",", quoting=csv.QUOTE_ALL,
-                                escapechar='\\')
+        fieldnames = ['response']
+        if any(result.request_text for result in results):
+            fieldnames.insert(0, 'request')
+        writer = csv.DictWriter(out_file, fieldnames=fieldnames, delimiter=",", quoting=csv.QUOTE_ALL, escapechar='\\')
         writer.writeheader()
         for result in results:
-            if include_prompt:
-                out_row = {
-                    'request': result[0].encode('utf_8').decode('unicode_escape'),
-                    'response': result[1]
-                }
-            else:
-                out_row = {
-                    'response': result[1]
-                }
+            # mandatory output fields
+            out_row = {'response': result.response_text}
+
+            # optional output fields
+            if result.request_text:
+                out_row['request'] = result.request_text.encode('utf_8').decode('unicode_escape')
             writer.writerow(out_row)
 
 
-def handle_console(include_prompt: bool, results: List[Tuple[str, str]]):
-    for request, response in results:
-        if include_prompt:
-            print("Request:", request)
-        print("Response:", response)
+def handle_output_to_console(results: List[Result]):
+    for result in results:
+        if result.request_text:
+            print("Request:", result.request_text)
+        print("Response:", result.response_text)
         print("--------------------------------------------------------------------------------------------")
 
 
 def create_output_file_name(directory, output_prefix) -> str:
     return os.path.join(directory, f"{output_prefix}_{datetime.now().strftime('%Y%m%d%H%M%S')}.csv")
```

### Comparing `prompeteer-0.3.1/prompeteer/prompt/prompt_config.py` & `prompeteer-0.3.2/prompeteer/prompt/prompt_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 import logging
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Optional
 
 import yaml
 
+from prompeteer.prompt.prompt import LLMProvider, DeclaredVariable, Variable
 from prompeteer.providers.aws_bedrock.aws_llm_request import AWSLLMRequest
 from prompeteer.providers.azure_openai.azure_llm_request import AzureLLMRequest
-from prompeteer.providers.llm_request import ILLMRequest
-from prompeteer.prompt.prompt import LLMProvider, DeclaredVariable, Variable
-from prompeteer.utils.utils import normalize_keys, create_declared_variable_list
+from prompeteer.providers.llm_request import LLMRequest
+from prompeteer.utils.utils import normalize_keys, get_declared_variables
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 class PromptConfig:
-    def __init__(self, version: str, name: str, llm_provider: LLMProvider, llm_request_config: Dict[str, Any],
+    def __init__(self, version: str, name: str, llm_provider: LLMProvider, prompt_config_dict: Dict[str, Any],
                  variables: List[Dict], schema_version: str):
         self.version: str = version
         self.name: str = name
         self.schema_version: str = schema_version
         self.llm_provider: LLMProvider = llm_provider
-        self.llm_request_config: Dict[str, Any] = llm_request_config
-        self.declared_variables: List[DeclaredVariable] = create_declared_variable_list(variables)
+        self.llm_request: Dict[str, Any] = prompt_config_dict
+        self.declared_variables: List[DeclaredVariable] = get_declared_variables(variables)
 
-    def to_llm_request(self, variables_to_inject: List[Variable]) -> ILLMRequest:
+    def to_llm_request(self, variables_to_inject: Optional[List[Variable]] = None) -> LLMRequest:
         if self.llm_provider == LLMProvider.azure:
-            return AzureLLMRequest(variables_to_inject, self.declared_variables, **self.llm_request_config)
+            llm_request: LLMRequest = AzureLLMRequest(**self.llm_request,
+                                                      declared_variables=self.declared_variables)
         elif self.llm_provider == LLMProvider.aws:
-            return AWSLLMRequest(variables_to_inject, self.declared_variables, **self.llm_request_config)
+            llm_request: LLMRequest = AWSLLMRequest(**self.llm_request,
+                                                    declared_variables=self.declared_variables)
         else:
             logger.error("Unsupported LLM")
             raise ValueError("Unsupported LLM")
-
-
-def load_prompt_config(prompt_config_file_path) -> PromptConfig:
-    with open(prompt_config_file_path, 'r') as file:
-        prompt_config = yaml.safe_load(file)
-        # Normalize keys to snake_case
-        prompt_config = normalize_keys(prompt_config)
-
-        name = prompt_config['name']
-        version = prompt_config['version']
-        schema_version = prompt_config['schema_version']
-        try:
-            provider = LLMProvider[prompt_config['provider']]
-        except KeyError as e:
-            logger.error(f"LLM Provider key missing: {e}")
-            raise
-        except ValueError as e:
-            logger.error(f"LLM Provider not supported: {e}")
-            raise
-        request = prompt_config['request']
-        variables = prompt_config['variables']
-        return PromptConfig(name=name,
-                            version=version,
-                            llm_provider=provider,
-                            llm_request_config=request,
-                            variables=variables,
-                            schema_version=schema_version)
+        if variables_to_inject is not None:
+            logger.debug("starting variable injection")
+            llm_request.validate_variables_to_inject(variables_to_inject)
+            llm_request.inject_variables(variables_to_inject=variables_to_inject)
+            logger.debug("variable injection done")
+        return llm_request
+
+    @classmethod
+    def from_file(cls, prompt_config_file_path) -> 'PromptConfig':
+        with open(prompt_config_file_path, 'r') as file:
+            prompt_config = yaml.safe_load(file)
+            # Normalize keys to snake_case
+            prompt_config = normalize_keys(prompt_config)
+
+            name = prompt_config['name']
+            version = prompt_config['version']
+            schema_version = prompt_config['schema_version']
+            try:
+                provider = LLMProvider[prompt_config['provider']]
+            except KeyError as e:
+                logger.error(f"LLM Provider key missing: {e}")
+                raise
+            except ValueError as e:
+                logger.error(f"LLM Provider not supported: {e}")
+                raise
+            prompt_config_dict = prompt_config['request']
+            variables = prompt_config['variables']
+            return cls(name=name,
+                       version=version,
+                       llm_provider=provider,
+                       prompt_config_dict=prompt_config_dict,
+                       variables=variables,
+                       schema_version=schema_version)
```

### Comparing `prompeteer-0.3.1/prompeteer/providers/aws_bedrock/aws_bedrock_client.py` & `prompeteer-0.3.2/prompeteer/providers/aws_bedrock/aws_bedrock_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 
 from prompeteer.providers.aws_bedrock.aws_llm_request import AWSLLMRequest
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 from tenacity import retry, stop_after_attempt, wait_exponential, retry_if_exception
 
-from prompeteer.providers.llm_client import ILLMClient
+from prompeteer.providers.llm_client import LLMClient
 
 
-class AwsBedrockClient(ILLMClient):
+class Message:
+    def __init__(self, content: str, role: str):
+        self.content: str = content
+        self.role: str = role
+
+
+class AwsBedrockClient(LLMClient):
     def __init__(self):
         self.client = boto3.client(service_name='bedrock-runtime', region_name='us-east-1')
 
     @retry(stop=stop_after_attempt(7), wait=wait_exponential(multiplier=1, min=2, max=10),
            retry=retry_if_exception(lambda e: True))
     def call(self, llm_request: AWSLLMRequest) -> str:
         try:
```

### Comparing `prompeteer-0.3.1/prompeteer/providers/azure_openai/azure_openai_client.py` & `prompeteer-0.3.2/prompeteer/providers/azure_openai/azure_openai_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from typing import Dict, Any
 
 from azure.identity import DefaultAzureCredential, get_bearer_token_provider
 from openai import AzureOpenAI
 from openai.types.chat import ChatCompletion
 
 from prompeteer.providers.azure_openai.azure_llm_request import AzureLLMRequest
-from prompeteer.providers.llm_client import ILLMClient
+from prompeteer.providers.llm_client import LLMClient
 
 token_provider = get_bearer_token_provider(
     DefaultAzureCredential(), "https://cognitiveservices.azure.com/.default"
 )
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
-class AzureOpenAiClient(ILLMClient):
+class AzureOpenAiClient(LLMClient):
     def __init__(self):
         self.azure_resource_to_client_map: Dict[str, AzureOpenAI] = {}
 
     def call(self, llm_request: AzureLLMRequest) -> str:
         azure_resource_name = os.getenv('AZURE_OPENAI_RESOURCE_NAME')
         if azure_resource_name is None:
             logger.error("AZURE_OPENAI_RESOURCE_NAME environment variable is not set")
@@ -61,11 +61,11 @@
             raise Exception('Failed to call Azure OpenAI Chat response')
         return response.choices[0].message.content
 
     def get_client_for_resource(self, azure_resource_name: str) -> AzureOpenAI:
         if azure_resource_name not in self.azure_resource_to_client_map:
             self.azure_resource_to_client_map[azure_resource_name] = AzureOpenAI(
                 api_version="2024-02-01",
-                azure_endpoint=f"https://{azure_resource_name}.openai.azure.com/",
+                azure_endpoint=f"https://{azure_resource_name}.openai.azure.com",
                 azure_ad_token_provider=token_provider
             )
         return self.azure_resource_to_client_map[azure_resource_name]
```

### Comparing `prompeteer-0.3.1/prompeteer/providers/llm_client.py` & `prompeteer-0.3.2/prompeteer/providers/llm_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 import logging
 from abc import abstractmethod, ABC
 from typing import Dict
 
 from prompeteer.prompt.prompt import LLMProvider
-from prompeteer.providers.llm_request import ILLMRequest
+from prompeteer.providers.llm_request import LLMRequest
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
-class ILLMClient(ABC):
+class LLMClient(ABC):
+    clients: Dict[str, 'LLMClient'] = {}
+
     @abstractmethod
-    def call(self, llm_request: ILLMRequest) -> str:
+    def call(self, llm_request: LLMRequest) -> str:
         raise NotImplementedError("LLM provider not implemented")
 
-
-clients: Dict[str, ILLMClient] = {}
-
-
-def _init_llm_client(provider: LLMProvider) -> ILLMClient:
-    if provider == LLMProvider.azure:
-        logger.info("Initializing Azure OpenAI LLM Client")
-        from prompeteer.providers.azure_openai.azure_openai_client import AzureOpenAiClient
-        return AzureOpenAiClient()
-    elif provider == LLMProvider.aws:
-        logger.info("Initializing AWS Bedrock LLM Client")
-        from prompeteer.providers.aws_bedrock.aws_bedrock_client import AwsBedrockClient
-        return AwsBedrockClient()
-    else:
-        logger.error(f"Unknown LLM Provider {provider}")
-        raise Exception(f"Unknown LLM Provider {provider}")
-
-
-def get_llm_client(provider: LLMProvider) -> ILLMClient:
-    assert provider is not None, "Provider must be provided"
-    global clients
-    if provider.value not in clients:
-        clients[provider.value] = _init_llm_client(provider)
-        logger.info(f"LLM Client for {provider} successfully initialized")
-    return clients[provider.value]
+    @classmethod
+    def get_client_by_provider(cls, provider: LLMProvider) -> 'LLMClient':
+        assert provider is not None, "Provider must be provided"
+        if provider.value not in cls.clients:
+            if provider == LLMProvider.azure:
+                logger.info("Initializing Azure OpenAI LLM Client")
+                from prompeteer.providers.azure_openai.azure_openai_client import AzureOpenAiClient
+                return AzureOpenAiClient()
+            elif provider == LLMProvider.aws:
+                logger.info("Initializing AWS Bedrock LLM Client")
+                from prompeteer.providers.aws_bedrock.aws_bedrock_client import AwsBedrockClient
+                return AwsBedrockClient()
+            else:
+                logger.error(f"Unknown LLM Provider {provider}")
+                raise Exception(f"Unknown LLM Provider {provider}")
+        logger.info(f"LLM Client for {provider} initialized successfully")
+        return cls.clients[provider.value]
```

### Comparing `prompeteer-0.3.1/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.3.2/prompeteer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.3.1
+Version: 0.3.2
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.3.1/prompeteer.egg-info/SOURCES.txt` & `prompeteer-0.3.2/prompeteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.1/public_README.md` & `prompeteer-0.3.2/public_README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.1/setup.py` & `prompeteer-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("public_README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.3.1',
+    version='0.3.2',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests', 'tests.*', 'README.md']),  # Include all packages
     py_modules=['prompeteer'],
```


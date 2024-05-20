# Comparing `tmp/equivalent_llm-0.2.0.tar.gz` & `tmp/equivalent_llm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equivalent_llm-0.2.0.tar", last modified: Thu Apr 18 07:32:27 2024, max compression
+gzip compressed data, was "equivalent_llm-0.3.0.tar", last modified: Mon May 20 05:52:51 2024, max compression
```

## Comparing `equivalent_llm-0.2.0.tar` & `equivalent_llm-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0     1469 2024-04-18 07:32:09.404541 equivalent_llm-0.2.0/LICENSE
--rw-r--r--   0        0        0     5155 2024-04-18 07:32:09.404541 equivalent_llm-0.2.0/README.md
--rw-r--r--   0        0        0     2050 2024-04-18 07:32:27.192814 equivalent_llm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9641 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/__init__.py
--rw-r--r--   0        0        0     5896 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/function/__init__.py
--rw-r--r--   0        0        0     7487 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/function_call/__init__.py
--rw-r--r--   0        0        0    13831 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/function_call/v1/__init__.py
--rw-r--r--   0        0        0     4203 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/function_call/v2/__init__.py
--rw-r--r--   0        0        0     8506 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/reservation.py
--rw-r--r--   0        0        0    14507 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/testers/__init__.py
--rw-r--r--   0        0        0     2738 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/src/equivalent_llm/user.py
--rw-r--r--   0        0        0        0 2024-04-18 07:32:09.408542 equivalent_llm-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     6040 1970-01-01 00:00:00.000000 equivalent_llm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1469 2024-05-20 05:52:37.239201 equivalent_llm-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7297 2024-05-20 05:52:37.239201 equivalent_llm-0.3.0/README.md
+-rw-r--r--   0        0        0     2050 2024-05-20 05:52:51.335234 equivalent_llm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13172 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/engine/__init__.py
+-rw-r--r--   0        0        0     1289 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/engine/openai.py
+-rw-r--r--   0        0        0     2966 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/engine/pet.py
+-rw-r--r--   0        0        0     5896 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function/v1/__init__.py
+-rw-r--r--   0        0        0     7402 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function/v2/__init__.py
+-rw-r--r--   0        0        0     7547 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function_call/__init__.py
+-rw-r--r--   0        0        0    13831 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function_call/v1/__init__.py
+-rw-r--r--   0        0        0    12430 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/function_call/v2/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/parse/__init__.py
+-rw-r--r--   0        0        0     8544 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/reservation.py
+-rw-r--r--   0        0        0    13183 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/testers/__init__.py
+-rw-r--r--   0        0        0     2667 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/src/equivalent_llm/user.py
+-rw-r--r--   0        0        0        0 2024-05-20 05:52:37.259201 equivalent_llm-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     8182 1970-01-01 00:00:00.000000 equivalent_llm-0.3.0/PKG-INFO
```

### Comparing `equivalent_llm-0.2.0/LICENSE` & `equivalent_llm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.2.0/README.md` & `equivalent_llm-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 # Validation tool to compare a generated context by sLLM to reference context
 
-생성된 문장(Function call 또는 Reservation Board (a.k.a Formatted output))과 기준이 되는 문장을 비교하여 두 문자열이 동일한지 여부를 확인합니다.
+Generated sentence by sLLM is compared to the reference sentence to check whether the generated sentence is equivalent to the reference sentence or not.
 
 ## Validataion criteria
 
 ### Equivalence test
 
-tests whether the generated sentence is equivalent to the reference sentence or not
+Tests whether the generated sentence is equivalent to the reference sentence or not
+
+> eg. 신설동 주변 영화관 vs 신설동 근처 극장
 
 ### Consistency test
 
-tests whether the generated sentence is consistent with the given information or not
+Tests whether the generated sentence is consistent with the given information or not
+
+> eg. 2024 5/10 이후 주말 -> 2024-05-11 00:00:00 - 2024-05-12 23:59:59
 
 ### Grammar test
 
-tests whether the generated sentence is grammatically correct or not
+Tests whether the generated sentence is grammatically correct or not
+
+> eg. "배트맨 영화는 고담 시티에서 범죄를 억류하는 두 년 만에, 달마다 살인범 리더(다노)를 추적하는 중에 도시의 부패를 밝혀내는 과정에서 시민을 위협하는 실제 형사를 찾아내는 책임을 맡게 됩니다." (???) -> "배트맨 영화는 고담 시티에서 범죄와 싸우는 지 2년 된 배트맨이 리들러라는 연쇄 살인범을 추적하면서 도시의 부패를 밝혀내는 내용입니다."
 
 ### Elegant test
 
-tests whether the generated sentence is firmly well-structed to human readablity or not
+Tests whether the generated sentence is firmly well-structed to human readablity or not
+
+> eg. "내일 '아쿠아맨과 로스트 킹덤'을 관람하실 수 있는 시간을 조회했습니다. 어느 시간에 예약을 도와드릴까요?" -> "홍대입구 상영관에서 '아쿠아맨과 로스트 킹덤' 영화 예약을 도와드릴까요? 언제 관람하시길 원하세요?"
 
 ### Etc
 
 -   Function name matching
 -   Arugments matching
 -   Required arguments
 
 ## Input data format
 
+Three kinds of information are required for the validation. The input data is composed of the following 3 items.
+
+-   Context: The context of previously processed sentences
+-   Reference (a.k.a. Answer): The reference sentence for function call or reservation board (a.k.a. formatted output) related message
+-   Generated: The generated sentence for function call or reservation board related message
+
 ### JSON string
 
+Example
+
 ```json
 {
     "context": "<s>[INST] <<SYS>>\nYou are a helpful and respectful movie ticketing assistant.\nYou\"re actively involved in a three-way conversation with \"user\", \"function\" (the function helper other than you), ...",
     "answer": "{\"function_call\": {\"name\": \"extract_date_time\", \"arguments\": \"{\\\"query\\\":\\\"현재 시간을 알려주세요~\\\"}\"}, \"role\": \"assistant\", \"content\": null} ",
     "generated": "{\"function_call\": {\"name\": \"extract_date_time\", \"arguments\": \"{\\\"query\\\":\\\"현재 시간을 알려주세요\\\"}\"}, \"role\": \"assistant\", \"content\": null} "
 }
 ```
@@ -41,37 +57,73 @@
 ### CSV file
 
 ```csv
 index, context, answer, generated
 0,<s>[INST] <<SYS>>\nYou are a...,{"function_call": {...,{"function_call": {...
 ```
 
+### Supported LLM models
+
+-   Llama 3 (default)
+-   Llama 2
+-   Mistral
+-   A.X
+
 ## Installation
 
 ```bash
 pip install equivalent_llm
 ```
 
-## OpenAI API key
+## Prompt Engines
+
+### Azure@GIP
 
-It use ChatGPT 4-turbo API. You need to set your API key to use this tool. You can set the API key in two ways: in command line or in python.
+It uses Prompt Engineering Tool (PET) based on Azure@GIP. You need to set your configurations. You can set the API key in two ways: in command line or in python.
+
+If PET_ID, PET_URL, or PET_TIMEOUT is not set, default values are used.
+PET_ID is related to OpenAI model directly. Default PET_ID uses ChatGPT 4 (gpt-4-1106).
+Default PET_URL is only accessible on restricted network (eg. DeDVI).
+
+In command line:
+
+```bash
+export PET_URL="pet_ip:port"
+export PET_ID="your-id"
+export PET_TIMEOUT=60
+```
+
+In python:
+
+```python
+import os
+os.environ["PET_URL"] = "pet_ip:port"
+os.environ["PET_ID"] = "your-id"
+os.environ["PET_TIMEOUT"] = "60"
+```
+
+### OpenAI API key (deprecated)
+
+It uses ChatGPT 4-turbo API on default. You need to set your API key to use this tool. You can set the API key in two ways: in command line or in python.
 
 In command line:
 
 ```bash
 export OPENAI_API_KEY="your-api-key"
 ```
 
 In python:
 
 ```python
 import os
 os.environ["OPENAI_API_KEY"] = "your-api-key"
 ```
 
+Also, you should run commands with **prompt_engine='OpenAI'** option.
+
 ## Usage
 
 For the validation set, you can use the following code:
 
 ```python
 import equivalent_llm
```

### Comparing `equivalent_llm-0.2.0/pyproject.toml` & `equivalent_llm-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -95,21 +95,21 @@
 max-complexity = 10
 
 [tool.pdm]
 distribution = true
 
 [project]
 name = "equivalent_llm"
-version = "0.2.0"
+version = "0.3.0"
 description = "Validation tool to compare a generated context by sLLM to reference context"
 authors = [
     { name = "Sung Gon Yi", email = "skonmeme@sk.com" },
 ]
 dependencies = [
-    "langchain-core~=0.1.30",
+    "langchain-core>=0.1.30",
     "langchain>=0.1.11",
     "langchain-community>=0.0.27",
     "langchain-openai>=0.0.8",
     "openai>=1.13.3",
     "pydantic>=2.6.3",
     "pytest>=8.1.1",
     "pytest-mock>=3.12.0",
```

### Comparing `equivalent_llm-0.2.0/src/equivalent_llm/__init__.py` & `equivalent_llm-0.3.0/src/equivalent_llm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,84 +4,145 @@
 import re
 from typing import Optional, Union
 
 from tqdm import tqdm
 
 from langchain_openai import ChatOpenAI
 
-from equivalent_llm import function, function_call, reservation, user
+from equivalent_llm import function_call, reservation, user
+from equivalent_llm.engine.openai import OpenAI
+from equivalent_llm.engine.pet import PET
+from equivalent_llm.function import v1 as function_v1
+from equivalent_llm.function import v2 as function_v2
+from equivalent_llm.parse import json_loads
 
 class EquvalentLLM:
 
+    openai_configurations = {
+        'temperature': 0.0,
+        'model': 'gpt-4-turbo',
+        'top_p': 1.0,
+    }
+
     configurations = {
-        'temperature': 0.15,
-        'model': 'gpt-4-0125-preview',
-        'prompt_engine': 'OpenAI',
-        'parse_instruction': True,
-        'test_consistency': True,
-        'test_grammar': True,
-        'test_elegance': True,
-        'api': 'v1',
+        'prompt_engine': 'PET',
+        'api': 'v2',
+        'llm_type': 'llama3',
+        'json_warning': False,
     }
 
     # initialization
     instructions = []
     instruction: dict = {}
     parsed_instructions: list = []
     parsed_reference = None
     parsed_generated = None
 
-    def __load_open_ai(self) -> ChatOpenAI:
-        return ChatOpenAI(
-            temperature = self.configurations['temperature'],
-            model = self.configurations['model']
-        )
-
     def __json_loads(self, json_str: str) -> dict:
-        parsed = json.loads(json_str)
+        parsed = json_loads(json_str, self.configurations['json_warning'])
         #if isinstance(parsed, list) and len(parsed) == 1:
         if isinstance(parsed, list):
             return parsed[0]
         else:
             return parsed
 
     def __parse_preknowledge(self, preknowledge: str) -> None:
-        contents = preknowledge.replace('\n','').split('</s>')
-        messages = [
-            list(filter(lambda x: x is not None and x.strip() != '',
-                re.sub('.*<</SYS>>', '', content)
-                .replace('<s>[INST]', '')
-                .split('[/INST]')))
-            for content in contents
-        ]
-        self.instructions = list(itertools.chain([ self.__json_loads(m) for message in messages[:-1] for m in message ]))
-        self.instruction = self.__json_loads(messages[-1][0])
-        self.instructions.append(self.instruction)
+        match self.configurations['llm_type'].lower():
+            case 'llama3':
+                preknowledge = re.sub(r"<\|begin_of_text\|>", '', preknowledge)
+                contents = preknowledge.replace('\n','').split('<|eot_id|>')[1:]
+                messages = list(filter(lambda x: x is not None and x.strip() != '',
+                    [
+                        re.sub(r"<\|start_header_id\|>.+<\|end_header_id\|>", '', content)
+                        for content in contents
+                    ]))
+                self.instructions = [ self.__json_loads(message) for message in messages[:-1] ]
+                self.instruction = self.__json_loads(messages[-1])
+                self.instructions.append(self.instruction)
+            case 'llama2':
+                contents = preknowledge.replace('\n','').split('</s>')
+                messages = [
+                    list(filter(lambda x: x is not None and x.strip() != '',
+                        re.sub('.*<</SYS>>', '', content)
+                        .replace('<s>[INST]', '')
+                        .split('[/INST]')))
+                    for content in contents
+                ]
+                self.instructions = list(itertools.chain([ self.__json_loads(m) for message in messages[:-1] for m in message ]))
+                self.instruction = self.__json_loads(messages[-1][0])
+                self.instructions.append(self.instruction)
+            case 'a.x':
+                contents = (
+                    preknowledge
+                        .replace('\n','')
+                        .replace('<|endoftext|><|endoftext|>', '</|endoftext|><|endoftext|>')
+                        .split('</|endoftext|>')
+                )
+                messages = [
+                    list(filter(lambda x: x is not None and x.strip() != '',
+                        re.sub('.*<</SYS>>', '', content)
+                        .replace('<|endoftext|>[INST]', '')
+                        .split('[/INST]')))
+                    for content in contents
+                ]
+                self.instructions = list(itertools.chain([ self.__json_loads(m) for message in messages[:-1] for m in message ]))
+                self.instruction = self.__json_loads(messages[-1][0])
+                self.instructions.append(self.instruction)
+            case 'mistral':
+                f_region = r".*\}\]\[" # tricky
+                r_region = r"["
+                contents = preknowledge.replace('\n','').replace('</s>', '</s><s>').split('</s>')
+                messages = [
+                    list(filter(lambda x: x is not None and x.strip() != '',
+                        re.sub(f_region, r_region, content)
+                        .replace('<s>[INST]', '')
+                        .split('[/INST]')))
+                    for content in contents
+                ]
+                self.instructions = list(itertools.chain([ self.__json_loads(m) for message in messages[:-1] for m in message ]))
+                self.instruction = self.__json_loads(messages[-1][0])
+                self.instructions.append(self.instruction)
+            case _:
+                raise ValueError(f"Unknown LLM model type: {self.configurations['llm_type']}")
 
     def __init__(self, preknowledge, reference, generated, logger = None, **kwargs):
         self.preknowledge = preknowledge
         self.reference = reference
         self.generated = generated
 
         self.logger = logger if logger is not None else logging.getLogger(__name__)
 
-        self.configurations.update(kwargs)
-        if self.configurations['prompt_engine'] == 'OpenAI':
-            self.prompt_engine = self.__load_open_ai()
+        self.update_configurations(**kwargs)
+        if self.configurations['prompt_engine'] == 'PET':
+            self.prompt_engine = PET(logger=self.logger, **self.configurations)
+        elif self.configurations['prompt_engine'] == 'OpenAI':
+            self.update_openai_configurations(**kwargs)
+            self.prompt_engine = OpenAI(logger=self.logger, **self.openai_configurations)
         else:
             raise ValueError(f"Unknown prompt engine: {self.configurations['prompt_engine']}")
 
         self.__parse_preknowledge(self.preknowledge)
 
     def update_configurations(self, **kwargs) -> None:
         self.configurations.update(kwargs)
         self.logger.debug(self.configurations)
 
+    def update_openai_configurations(self, **kwargs) -> None:
+        self.openai_configurations.update(kwargs)
+        self.openai_configurations.pop('prompt_engine', None)
+        self.openai_configurations.pop('api', None)
+        self.openai_configurations.pop('llm_type', None)
+
     def parse_instructions(self) -> None:
         parsed_instructions = []
+        match self.configurations['api']:
+            case 'v1':
+                function = function_v1
+            case _:
+                function = function_v2
         for index, instruction in enumerate(self.instructions):
             match instruction.get('role'):
                 case 'user':
                     parsed_instructions.append(
                         user.get_entities(instruction['content'], parsed_instructions[0:index], self.prompt_engine, self.logger)
                     )
                 case 'function':
@@ -92,22 +153,22 @@
                 case _:
                     raise ValueError(f"Unknown role: {instruction}")
         self.parsed_instructions = parsed_instructions
         self.logger.debug(self.parsed_instructions)
 
     def parse_llm(self, string: str, reference: bool = False) -> dict:
         try:
-            json_parsed = json.loads(string)
+            json_parsed = json_loads(string, self.configurations['json_warning'])
             if json_parsed.get('function_call') is not None:
                 # function call generation
                 function = json_parsed['function_call']
                 parsed = {
                     'type': 'function_call',
                     'name': function['name'],
-                    'arguments': json.loads(function['arguments']),
+                    'arguments': json_loads(function['arguments'], self.configurations['json_warning']),
                     'role': 'assistant',
                 }
                 if reference:
                     self.validation_type = 'function_call'
             else:
                 # reservation generation
                 status = 'valid'
@@ -117,28 +178,28 @@
                 doubled_content = re.findall(r'(?<=})\n?{.*', content, flags=re.DOTALL)
                 if len(doubled_content) > 0:
                     content = doubled_content[-1]
                     status = 'doubled'
                 parsed = {
                     'type': 'reservation',
                     'name': 'reservation',
-                    'reservation': json.loads(content),
+                    'reservation': json_loads(content, self.configurations['json_warning']),
                     'status': status,
                     'role': 'assistant',
                 }
                 if reference:
                     self.validation_type = 'reservation'
             self.logger.debug(f"Parsing LLM: {parsed}")
             return parsed
         except json.JSONDecodeError as e:
             return { 'status': 'fail', 'error': e }
 
 
     def validate(self, **kwargs) -> dict:
-        if self.configurations['parse_instruction'] and len(self.parsed_instructions) == 0:
+        if len(self.parsed_instructions) == 0:
             self.parse_instructions()
         if self.parsed_reference is None:
             self.parsed_reference = self.parse_llm(self.reference, True)
         if self.parsed_generated is None:
             self.parsed_generated = self.parse_llm(self.generated)
 
         if self.parsed_reference.get('status') == 'fail':
@@ -214,25 +275,28 @@
     csv_path: Optional[str] = None,
     columns = {
         'preknowledge': 'context',
         'reference': 'answer',
         'generated': 'generated',
     },
     indexes: Optional[Union[list, range, int]] = None,
+    index: Optional[Union[list, range, int]] = None,
     print_result: bool = False,
     logger = logging.getLogger(), **kwargs
 ) -> dict:
     if isinstance(llm_list, str) and csv_path is None:
         csv_path = llm_list
         llm_list = None
     if llm_list is None:
         if csv_path is None:
             raise ValueError("Either llm_list or csv_path should be provided.")
         llm_list = __csv_to_list(csv_path, kwargs.get('encoding', 'utf-8'), logger)
 
+    if indexes is None:
+        indexes = index
     if isinstance(indexes, int):
         indexes = [indexes]
     elif isinstance(indexes, range):
         indexes = list(indexes)
     elif indexes is None:
         indexes = range(len(llm_list))
     llms = [llm_list[index] for index in indexes]
```

### Comparing `equivalent_llm-0.2.0/src/equivalent_llm/function/__init__.py` & `equivalent_llm-0.3.0/src/equivalent_llm/function/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.2.0/src/equivalent_llm/function_call/__init__.py` & `equivalent_llm-0.3.0/src/equivalent_llm/function_call/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,16 @@
 
     # argument paried to reference
     paired_arguments_result = check_paired_arguments(generated['arguments'].keys(), reference['arguments'].keys())
     reports['tests']['paired_arguments'] = paired_arguments_result
     etc_counter.count(paired_arguments_result)
 
     # value type
-    for name in generated['arguments']:
+    logger.debug(f"FUNCTION_NAME: {function_name.upper()}")
+    for name in reference['arguments']:
         definition = DEFINITION['parameters'].get(name)
 
         # equivalence tests
         equivalence_result = equivalence_test(
             generated['arguments'].get(name),
             reference['arguments'].get(name),
             instructions,
```

### Comparing `equivalent_llm-0.2.0/src/equivalent_llm/function_call/v1/__init__.py` & `equivalent_llm-0.3.0/src/equivalent_llm/function_call/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `equivalent_llm-0.2.0/src/equivalent_llm/reservation.py` & `equivalent_llm-0.3.0/src/equivalent_llm/reservation.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         return {'passed': False, 'counts': {'total': {'passed': 0, 'total': 1}}, 'tests': {}, 'reason': 'reservation is not generated ', 'level': 'fatal'}
 
     equivalence_counter = testers.TestCounter()
     consistency_counter = testers.TestCounter()
     grammar_counter = testers.TestCounter()
     elegance_counter = testers.TestCounter()
 
+    logger.debug("RESERVATION BOARD")
     for element in elements:
         if (
             RESERVATION_BOARD.get(element) and
             (
                 (
                     generated['reservation'].get(element) is not None and
                     generated['reservation'][element] != ''
```

### Comparing `equivalent_llm-0.2.0/src/equivalent_llm/testers/__init__.py` & `equivalent_llm-0.3.0/src/equivalent_llm/testers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     ChatPromptTemplate,
     SystemMessagePromptTemplate,
     AIMessagePromptTemplate,
     HumanMessagePromptTemplate,
 )
 from pydantic.v1 import BaseModel, Field
 
+from equivalent_llm.engine import PromptEngine
+
 class TestCounter:
 
     passed: int = 0
     total: int = 0
 
     def __iadd__(self, counter):
         self.passed += counter.passed
@@ -50,15 +52,15 @@
 """
 class EquivalenceResult(BaseModel):
     passed: bool = Field(description="Whether equivalent or not")
     score: int = Field(description="Equivalence score from 0 to 100")
     evidence: str = Field(description="The evidence of passed value")
 equivalence_parser = PydanticOutputParser(pydantic_object=EquivalenceResult)
 
-def get_equivalence_tester(definition: dict, prompt_engine: Any) -> Callable:
+def get_equivalence_tester(definition: dict, prompt_engine: PromptEngine) -> Callable:
     # currently fixed to use ChatOpenAI
     def equivalence_tester(value: Any, reference_value: Any, instructions: list, logger: Logger) -> dict:
         try:
             system_template = SystemMessagePromptTemplate.from_template(FormatTemplate)
             ai_template = AIMessagePromptTemplate.from_template(PreknowledgeTemplate)
             human_template = HumanMessagePromptTemplate.from_template(EquivalenceTemplate)
             prompt_template = ChatPromptTemplate.from_messages(
@@ -69,21 +71,15 @@
                 generated=value,
                 category=definition['category'],
                 comment=definition.get('comment', ''),
                 information=instructions if instructions is not None else "No information",
                 format_instructions=equivalence_parser.get_format_instructions(),
             ).to_messages()
             logger.debug(f"Equivalence Prompt: {final_prompt}")
-            result = prompt_engine(final_prompt)
-
-            # markdown json format
-            if result.content.startswith("```json"):
-                return json.loads(result.content.split("```json")[1].split("```")[0])
-            else:
-                return json.loads(result.content)
+            return prompt_engine.invoke(final_prompt)
         except Exception as e:
             logger.debug(f"Equvalence Error: {e}")
             return {
                 'passed': False,
                 'level': 'fatal',
                 'evidence': {
                     'type': 'validation process',
@@ -97,15 +93,15 @@
 LatestRequestedTemplate = """- Given information: {given_information}"""
 NumberConsistencyTemplate = """- Answer a question by true or false of passed with concrete evidence.
 - Question: Is below a value is consistently matched with given information? {range_sentence}
 {comment}
 - target value: {generated}
 """
 
-def get_number_consistency_tester(definition: dict, prompt_engine: Any) -> Callable:
+def get_number_consistency_tester(definition: dict, prompt_engine: PromptEngine) -> Callable:
     def number_tester(value: Any, reference_value: Any, instructions: list, logger: Logger) -> dict:
         range_sentence = ''
         if definition.get('range') is not None:
             if definition['range'][0] == -math.inf:
                 range_sentence = f"Also, is the value less or equal than {definition['range'][1]}?"
             elif definition['range'][1] == math.inf:
                 range_sentence = f"Also, is the value greater or equal than {definition['range'][0]}?"
@@ -123,21 +119,15 @@
                 generated=value,
                 given_information=instructions if instructions is not None else "No information",
                 range_sentence=range_sentence,
                 comment=definition.get('comment', ''),
                 format_instructions=equivalence_parser.get_format_instructions(),
             ).to_messages()
             logger.debug(f"Number Consistency Prompt: {final_prompt}")
-            result = prompt_engine(final_prompt)
-
-            # markdown json format
-            if result.content.startswith("```json"):
-                return json.loads(result.content.split("```json")[1].split("```")[0])
-            else:
-                return json.loads(result.content)
+            return prompt_engine.invoke(final_prompt)
         except Exception as e:
             logger.debug(f"Number Consistency Error: {e}")
             return {
                 'passed': False,
                 'level': 'fatal',
                 'evidence': {
                     'type': 'validation process',
@@ -148,15 +138,15 @@
 
 CategoryConsistencyTemplate = """- Answer a question by true or false of passed with concrete evidence.
 - Question: Is below phrase is matched with given information of following categories: {category_sentence}?
   {comment}
 - target sentence: {generated}
 """
 
-def get_category_consistency_tester(definition: dict, prompt_engine: Any) -> Callable:
+def get_category_consistency_tester(definition: dict, prompt_engine: PromptEngine) -> Callable:
     def category_tester(value: Any, reference_value: Any, instructions: list, logger: Logger) -> dict:
         try:
             system_template = SystemMessagePromptTemplate.from_template(FormatTemplate)
             ai_template = AIMessagePromptTemplate.from_template(LatestRequestedTemplate)
             human_template = HumanMessagePromptTemplate.from_template(CategoryConsistencyTemplate)
             prompt_template = ChatPromptTemplate.from_messages(
                 [system_template, ai_template, human_template]
@@ -165,20 +155,15 @@
                 generated=value,
                 given_information=instructions if instructions is not None else "No information",
                 category_sentence=definition['category'],
                 comment=definition.get('comment', ''),
                 format_instructions=equivalence_parser.get_format_instructions(),
             ).to_messages()
             logger.debug(f"Category Consistency Prompt: {final_prompt}")
-            result = prompt_engine(final_prompt)
-            # markdown json format
-            if result.content.startswith("```json"):
-                return json.loads(result.content.split("```json")[1].split("```")[0])
-            else:
-                return json.loads(result.content)
+            return prompt_engine.invoke(final_prompt)
         except Exception as e:
             logger.debug(f"Category Consistency Error: {e}")
             return {
                 'passed': value == reference_value,
                 'evidence': {
                     'type': 'validation process',
                     'message': str(e),
@@ -188,15 +173,15 @@
 
 EnumConsistencyTemplate = """- Answer a question by true or false of passed with concrete evidence.
 - Question: Is below phrase is matched with given enum items: {enum_items}?
   {comment}
 - target sentence: {generated}
 """
 
-def get_enum_consistency_tester(definition: dict, prompt_engine: Any) -> Callable:
+def get_enum_consistency_tester(definition: dict, prompt_engine: PromptEngine) -> Callable:
     def enum_tester(value: Any, reference_value: Any, instructions: list, logger: Logger) -> dict:
         try:
             system_template = SystemMessagePromptTemplate.from_template(FormatTemplate)
             ai_template = AIMessagePromptTemplate.from_template(LatestRequestedTemplate)
             human_template = HumanMessagePromptTemplate.from_template(EnumConsistencyTemplate)
             prompt_template = ChatPromptTemplate.from_messages(
                 [system_template, ai_template, human_template]
@@ -205,20 +190,15 @@
                 generated=value,
                 given_information=instructions if instructions is not None else "No information",
                 enum_items=definition['items'],
                 comment=definition.get('comment', ''),
                 format_instructions=equivalence_parser.get_format_instructions(),
             ).to_messages()
             logger.debug(f"Enum Consistency Prompt: {final_prompt}")
-            result = prompt_engine(final_prompt)
-            # markdown json format
-            if result.content.startswith("```json"):
-                return json.loads(result.content.split("```json")[1].split("```")[0])
-            else:
-                return json.loads(result.content)
+            return prompt_engine.invoke(final_prompt)
         except Exception as e:
             logger.debug(f"Enum Consistency Error: {e}")
             return {
                 'passed': value == reference_value,
                 'evidence': {
                     'type': 'validation process',
                     'message': str(e),
@@ -230,35 +210,29 @@
 - Answer a question by true or false of passed with concrete evidence.
 - Question: Is below sentence is composed with STRICTLY correct grammar for Korean, English, or mixture of Korean and English, is it acceptable to read naturally?
   If sentence is just a word, it is considered as correct.
   {comment}
 - target sentence: {generated}
 """
 
-def get_grammar_tester(definition: dict, prompt_engine: Any) -> Callable:
+def get_grammar_tester(definition: dict, prompt_engine: PromptEngine) -> Callable:
     def grammar_tester(value: Any, reference_value: Any, instructions: Optional[list], logger: Logger) -> dict:
         try:
             system_template = SystemMessagePromptTemplate.from_template(FormatTemplate)
             human_template = HumanMessagePromptTemplate.from_template(GrammarTemplate)
             prompt_template = ChatPromptTemplate.from_messages(
                 [system_template, human_template]
             )
             final_prompt = prompt_template.format_prompt(
                 generated=value,
                 comment=definition.get('comment', ''),
                 format_instructions=equivalence_parser.get_format_instructions(),
             ).to_messages()
             logger.debug(f"Grammar Prompt: {final_prompt}")
-            result = prompt_engine(final_prompt)
-
-            # markdown json format
-            if result.content.startswith("```json"):
-                return json.loads(result.content.split("```json")[1].split("```")[0])
-            else:
-                return json.loads(result.content)
+            return prompt_engine.invoke(final_prompt)
         except Exception as e:
             logger.debug(f"Grammar Error: {e}")
             return {
                 'passed': value == reference_value,
                 'evidence': {
                     'type': 'validation process',
                     'message': str(e),
@@ -278,15 +252,15 @@
 - Question: Is below target sentence centainly superior elegant than, reference sentence?
   Please provide a elegant and human readable alternative as well by orignial language of target sentence with same tone.
   {comment}
 - target sentence: {generated}
 """
 
 "Is the sentence below equivalent to, or even more elegant than, the standard sentence? Please provide a fluid and refined alternative as well."
-def get_elegance_tester(definition: dict, prompt_engine: Any) -> Callable:
+def get_elegance_tester(definition: dict, prompt_engine: PromptEngine) -> Callable:
     # currently fixed to use ChatOpenAI
     def elegance_tester(value: Any, reference_value: Any, instructions: list, logger: Logger) -> dict:
         try:
             system_template = SystemMessagePromptTemplate.from_template(FormatTemplate)
             ai_template = AIMessagePromptTemplate.from_template(PreknowledgeTemplate)
             human_template = HumanMessagePromptTemplate.from_template(EleganceTemplate)
             prompt_template = ChatPromptTemplate.from_messages(
@@ -296,21 +270,15 @@
                 reference=reference_value,
                 generated=value,
                 comment=definition.get('comment', ''),
                 information=instructions if instructions is not None else "No information",
                 format_instructions=elegance_parser.get_format_instructions(),
             ).to_messages()
             logger.debug(f"Elegance Prompt: {final_prompt}")
-            result = prompt_engine(final_prompt)
-
-            # markdown json format
-            if result.content.startswith("```json"):
-                return json.loads(result.content.split("```json")[1].split("```")[0])
-            else:
-                return json.loads(result.content)
+            return prompt_engine.invoke(final_prompt)
         except Exception as e:
             logger.debug(f"Elegance Error: {e}")
             return {
                 'passed': False,
                 'level': 'fatal',
                 'evidence': {
                     'type': 'validation process',
```

### Comparing `equivalent_llm-0.2.0/src/equivalent_llm/user.py` & `equivalent_llm-0.3.0/src/equivalent_llm/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import json
 from logging import Logger
 
 from langchain.prompts import ChatPromptTemplate, SystemMessagePromptTemplate, HumanMessagePromptTemplate
 from langchain.output_parsers import PydanticOutputParser
-from langchain_openai import ChatOpenAI
 
 from pydantic.v1 import BaseModel, Field
 
+from equivalent_llm.engine import PromptEngine
+
 __system_template = '''
 - format instructions: {format_instructions}
 - When you reserve a movie at movie theater, you should think following considerations.
 - DATETIME: time, data, and datetime
 - THEATER': theater name. Specially it includes LOCATION + '극장', LOCATION + '상영관', or LOCATION + 'THEATER'.
 - LOCATION': district, place name, landmark, and company name near by theater, and so on. MUST NOT include theater name.
 - COORDINATES: coordinates by longitude and latitude
@@ -35,27 +35,26 @@
     entity: str = Field(desription="Entity type in user input message")
     keyword: str = Field(description="Core keyword of entity")
     evidence: str = Field(description="Evidence of decision")
 
 class ListOfUserEntity(BaseModel):
     entities: list[UserEntity] = Field(description="List of entities")
 
-def get_entities(message: str, instructions: list, prompt_engine: ChatOpenAI, logger: Logger) -> dict:
+def get_entities(message: str, instructions: list, prompt_engine: PromptEngine, logger: Logger) -> dict:
     system_template = SystemMessagePromptTemplate.from_template(__system_template)
     human_template = HumanMessagePromptTemplate.from_template(__human_template)
     chat_prompt_template = ChatPromptTemplate.from_messages(
         [system_template, human_template]
     )
 
     parser = PydanticOutputParser(pydantic_object=ListOfUserEntity)
     final_prompt = chat_prompt_template.format_prompt(
         message=message,
         format_instructions=parser.get_format_instructions()
     ).to_messages()
     logger.debug(f"Prompt for user input message: {final_prompt}")
 
-    result = prompt_engine(final_prompt)
-    parsed = json.loads(result.content.split("```json")[1].split("```")[0])
+    parsed = prompt_engine.invoke(final_prompt)
     parsed['role'] = 'user'
     parsed['name'] = 'user'
     parsed['request'] = message
     return parsed
```

### Comparing `equivalent_llm-0.2.0/PKG-INFO` & `equivalent_llm-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 Metadata-Version: 2.1
 Name: equivalent_llm
-Version: 0.2.0
+Version: 0.3.0
 Summary: Validation tool to compare a generated context by sLLM to reference context
 Author-Email: Sung Gon Yi <skonmeme@sk.com>
 License: BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/sktaiflow/equivalent_llm
 Project-URL: Issues, https://github.com/sktaiflow/equivalent_llm/issues
 Requires-Python: >=3.10
-Requires-Dist: langchain-core~=0.1.30
+Requires-Dist: langchain-core>=0.1.30
 Requires-Dist: langchain>=0.1.11
 Requires-Dist: langchain-community>=0.0.27
 Requires-Dist: langchain-openai>=0.0.8
 Requires-Dist: openai>=1.13.3
 Requires-Dist: pydantic>=2.6.3
 Requires-Dist: pytest>=8.1.1
 Requires-Dist: pytest-mock>=3.12.0
 Requires-Dist: ruff>=0.3.2
 Requires-Dist: tqdm>=4.66.2
 Description-Content-Type: text/markdown
 
 # Validation tool to compare a generated context by sLLM to reference context
 
-생성된 문장(Function call 또는 Reservation Board (a.k.a Formatted output))과 기준이 되는 문장을 비교하여 두 문자열이 동일한지 여부를 확인합니다.
+Generated sentence by sLLM is compared to the reference sentence to check whether the generated sentence is equivalent to the reference sentence or not.
 
 ## Validataion criteria
 
 ### Equivalence test
 
-tests whether the generated sentence is equivalent to the reference sentence or not
+Tests whether the generated sentence is equivalent to the reference sentence or not
+
+> eg. 신설동 주변 영화관 vs 신설동 근처 극장
 
 ### Consistency test
 
-tests whether the generated sentence is consistent with the given information or not
+Tests whether the generated sentence is consistent with the given information or not
+
+> eg. 2024 5/10 이후 주말 -> 2024-05-11 00:00:00 - 2024-05-12 23:59:59
 
 ### Grammar test
 
-tests whether the generated sentence is grammatically correct or not
+Tests whether the generated sentence is grammatically correct or not
+
+> eg. "배트맨 영화는 고담 시티에서 범죄를 억류하는 두 년 만에, 달마다 살인범 리더(다노)를 추적하는 중에 도시의 부패를 밝혀내는 과정에서 시민을 위협하는 실제 형사를 찾아내는 책임을 맡게 됩니다." (???) -> "배트맨 영화는 고담 시티에서 범죄와 싸우는 지 2년 된 배트맨이 리들러라는 연쇄 살인범을 추적하면서 도시의 부패를 밝혀내는 내용입니다."
 
 ### Elegant test
 
-tests whether the generated sentence is firmly well-structed to human readablity or not
+Tests whether the generated sentence is firmly well-structed to human readablity or not
+
+> eg. "내일 '아쿠아맨과 로스트 킹덤'을 관람하실 수 있는 시간을 조회했습니다. 어느 시간에 예약을 도와드릴까요?" -> "홍대입구 상영관에서 '아쿠아맨과 로스트 킹덤' 영화 예약을 도와드릴까요? 언제 관람하시길 원하세요?"
 
 ### Etc
 
 -   Function name matching
 -   Arugments matching
 -   Required arguments
 
 ## Input data format
 
+Three kinds of information are required for the validation. The input data is composed of the following 3 items.
+
+-   Context: The context of previously processed sentences
+-   Reference (a.k.a. Answer): The reference sentence for function call or reservation board (a.k.a. formatted output) related message
+-   Generated: The generated sentence for function call or reservation board related message
+
 ### JSON string
 
+Example
+
 ```json
 {
     "context": "<s>[INST] <<SYS>>\nYou are a helpful and respectful movie ticketing assistant.\nYou\"re actively involved in a three-way conversation with \"user\", \"function\" (the function helper other than you), ...",
     "answer": "{\"function_call\": {\"name\": \"extract_date_time\", \"arguments\": \"{\\\"query\\\":\\\"현재 시간을 알려주세요~\\\"}\"}, \"role\": \"assistant\", \"content\": null} ",
     "generated": "{\"function_call\": {\"name\": \"extract_date_time\", \"arguments\": \"{\\\"query\\\":\\\"현재 시간을 알려주세요\\\"}\"}, \"role\": \"assistant\", \"content\": null} "
 }
 ```
@@ -65,37 +81,73 @@
 ### CSV file
 
 ```csv
 index, context, answer, generated
 0,<s>[INST] <<SYS>>\nYou are a...,{"function_call": {...,{"function_call": {...
 ```
 
+### Supported LLM models
+
+-   Llama 3 (default)
+-   Llama 2
+-   Mistral
+-   A.X
+
 ## Installation
 
 ```bash
 pip install equivalent_llm
 ```
 
-## OpenAI API key
+## Prompt Engines
+
+### Azure@GIP
 
-It use ChatGPT 4-turbo API. You need to set your API key to use this tool. You can set the API key in two ways: in command line or in python.
+It uses Prompt Engineering Tool (PET) based on Azure@GIP. You need to set your configurations. You can set the API key in two ways: in command line or in python.
+
+If PET_ID, PET_URL, or PET_TIMEOUT is not set, default values are used.
+PET_ID is related to OpenAI model directly. Default PET_ID uses ChatGPT 4 (gpt-4-1106).
+Default PET_URL is only accessible on restricted network (eg. DeDVI).
+
+In command line:
+
+```bash
+export PET_URL="pet_ip:port"
+export PET_ID="your-id"
+export PET_TIMEOUT=60
+```
+
+In python:
+
+```python
+import os
+os.environ["PET_URL"] = "pet_ip:port"
+os.environ["PET_ID"] = "your-id"
+os.environ["PET_TIMEOUT"] = "60"
+```
+
+### OpenAI API key (deprecated)
+
+It uses ChatGPT 4-turbo API on default. You need to set your API key to use this tool. You can set the API key in two ways: in command line or in python.
 
 In command line:
 
 ```bash
 export OPENAI_API_KEY="your-api-key"
 ```
 
 In python:
 
 ```python
 import os
 os.environ["OPENAI_API_KEY"] = "your-api-key"
 ```
 
+Also, you should run commands with **prompt_engine='OpenAI'** option.
+
 ## Usage
 
 For the validation set, you can use the following code:
 
 ```python
 import equivalent_llm
```


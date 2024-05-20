# Comparing `tmp/examon_core-1.5.0.tar.gz` & `tmp/examon_core-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.5.0.tar", max compression
+gzip compressed data, was "examon_core-2.0.0.tar", max compression
```

## Comparing `examon_core-1.5.0.tar` & `examon_core-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,45 @@
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661414 examon_core-1.5.0/examon_core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661649 examon_core-1.5.0/examon_core/code_execution/__init__.py
--rw-r--r--   0        0        0      179 2024-05-09 16:51:06.661857 examon_core-1.5.0/examon_core/code_execution/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1192 2024-05-09 16:51:06.661998 examon_core-1.5.0/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc
--rw-r--r--   0        0        0     1558 2024-05-09 16:51:06.662136 examon_core-1.5.0/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc
--rw-r--r--   0        0        0     1381 2024-05-09 16:51:06.662279 examon_core-1.5.0/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc
--rw-r--r--   0        0        0      320 2024-05-09 16:51:06.662408 examon_core-1.5.0/examon_core/code_execution/sandbox.py
--rw-r--r--   0        0        0      899 2024-05-10 00:29:45.323471 examon_core-1.5.0/examon_core/code_execution/unrestricted_driver.py
--rw-r--r--   0        0        0      192 2024-05-09 16:51:06.662652 examon_core-1.5.0/examon_core/examon_filter_options.py
--rwxr-xr-x   0        0        0     2029 2024-05-09 16:51:06.662762 examon_core-1.5.0/examon_core/examon_in_memory_db.py
--rwxr-xr-x   0        0        0     1343 2024-05-09 23:36:29.257714 examon_core-1.5.0/examon_core/examon_item.py
--rw-r--r--   0        0        0      199 2024-05-09 16:51:06.663045 examon_core-1.5.0/examon_core/examon_serializer.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.664432 examon_core-1.5.0/examon_core/factories/__init__.py
--rw-r--r--   0        0        0      592 2024-05-09 23:31:08.718261 examon_core-1.5.0/examon_core/factories/base_question.py
--rwxr-xr-x   0        0        0     1845 2024-05-09 21:57:52.629036 examon_core-1.5.0/examon_core/factories/code_to_string.py
--rw-r--r--   0        0        0      851 2024-05-09 23:31:08.719491 examon_core-1.5.0/examon_core/factories/input_param_question.py
--rw-r--r--   0        0        0     4595 2024-05-10 00:59:57.509738 examon_core-1.5.0/examon_core/factories/item.py
--rw-r--r--   0        0        0     1474 2024-05-10 00:29:38.872822 examon_core-1.5.0/examon_core/factories/metrics.py
--rw-r--r--   0        0        0      796 2024-05-10 00:48:21.153689 examon_core-1.5.0/examon_core/factories/multi_choice.py
--rw-r--r--   0        0        0     1160 2024-05-10 00:29:45.339058 examon_core-1.5.0/examon_core/factories/multi_choice_question.py
--rw-r--r--   0        0        0      336 2024-05-10 00:56:12.636130 examon_core-1.5.0/examon_core/generate_unique_id.py
--rw-r--r--   0        0        0      816 2024-05-10 00:59:57.509901 examon_core-1.5.0/examon_core/global_settings.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663463 examon_core-1.5.0/examon_core/metrics/__init__.py
--rw-r--r--   0        0        0      740 2024-05-10 00:42:15.716582 examon_core-1.5.0/examon_core/metrics/calc_standard.py
--rw-r--r--   0        0        0      568 2024-05-10 00:29:38.862117 examon_core-1.5.0/examon_core/metrics/categorize_difficulty.py
--rw-r--r--   0        0        0     1399 2024-05-09 17:44:54.417048 examon_core-1.5.0/examon_core/metrics/code_analysis_visitor.py
--rw-r--r--   0        0        0     1340 2024-05-09 16:51:06.663807 examon_core-1.5.0/examon_core/metrics/visit_methods.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663934 examon_core-1.5.0/examon_core/models/__init__.py
--rw-r--r--   0        0        0      171 2024-05-09 16:51:06.664099 examon_core-1.5.0/examon_core/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      558 2024-05-09 16:51:06.664204 examon_core-1.5.0/examon_core/models/__pycache__/question_response.cpython-39.pyc
--rw-r--r--   0        0        0      824 2024-05-09 17:08:36.258277 examon_core-1.5.0/examon_core/models/code_metrics.py
--rwxr-xr-x   0        0        0      926 2024-05-09 17:09:48.272669 examon_core-1.5.0/examon_core/models/question.py
--rwxr-xr-x   0        0        0      191 2024-05-09 16:51:06.665480 examon_core-1.5.0/examon_core/models/question_response.py
--rw-r--r--   0        0        0      463 2024-05-09 16:51:06.666697 examon_core-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-18 14:31:03.633904 examon_core-2.0.0/examon_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661649 examon_core-2.0.0/examon_core/code_execution/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-09 16:51:06.661857 examon_core-2.0.0/examon_core/code_execution/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1192 2024-05-09 16:51:06.661998 examon_core-2.0.0/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc
+-rw-r--r--   0        0        0     1558 2024-05-09 16:51:06.662136 examon_core-2.0.0/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc
+-rw-r--r--   0        0        0     1381 2024-05-09 16:51:06.662279 examon_core-2.0.0/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc
+-rw-r--r--   0        0        0      431 2024-05-19 04:26:54.793493 examon_core-2.0.0/examon_core/code_execution/code_execution_sandbox.py
+-rw-r--r--   0        0        0      870 2024-05-19 04:26:54.804105 examon_core-2.0.0/examon_core/code_execution/unrestricted_driver.py
+-rwxr-xr-x   0        0        0     1764 2024-05-20 01:48:53.993256 examon_core-2.0.0/examon_core/examon.py
+-rw-r--r--   0        0        0        0 2024-05-19 00:55:24.523321 examon_core-2.0.0/examon_core/factories/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-19 04:45:32.637915 examon_core-2.0.0/examon_core/factories/default_code_to_string_factory.py
+-rw-r--r--   0        0        0     4261 2024-05-20 02:02:18.019024 examon_core-2.0.0/examon_core/factories/examon.py
+-rw-r--r--   0        0        0     1427 2024-05-20 01:50:38.841503 examon_core-2.0.0/examon_core/factories/metrics.py
+-rw-r--r--   0        0        0      519 2024-05-20 01:51:38.500379 examon_core-2.0.0/examon_core/factories/multi_choice.py
+-rw-r--r--   0        0        0      565 2024-05-20 01:34:12.947319 examon_core-2.0.0/examon_core/factories/question.py
+-rw-r--r--   0        0        0      220 2024-05-20 01:39:45.912421 examon_core-2.0.0/examon_core/filter_options.py
+-rw-r--r--   0        0        0      276 2024-05-18 23:56:59.870681 examon_core-2.0.0/examon_core/generate_unique_id.py
+-rw-r--r--   0        0        0      859 2024-05-20 01:45:29.939643 examon_core-2.0.0/examon_core/global_settings.py
+-rw-r--r--   0        0        0     1915 2024-05-20 01:25:50.546495 examon_core-2.0.0/examon_core/gof/decorators.py
+-rwxr-xr-x   0        0        0     2225 2024-05-20 01:59:06.149962 examon_core-2.0.0/examon_core/in_memory_db.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663463 examon_core-2.0.0/examon_core/metrics/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-20 01:37:01.972038 examon_core-2.0.0/examon_core/metrics/calc_standard_metrics.py
+-rw-r--r--   0        0        0      459 2024-05-20 01:52:59.926637 examon_core-2.0.0/examon_core/metrics/categorize_difficulty.py
+-rw-r--r--   0        0        0     1431 2024-05-19 00:25:48.026342 examon_core-2.0.0/examon_core/metrics/code_analysis_visitor.py
+-rw-r--r--   0        0        0     1340 2024-05-09 16:51:06.663807 examon_core-2.0.0/examon_core/metrics/visit_methods.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663934 examon_core-2.0.0/examon_core/models/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-09 16:51:06.664099 examon_core-2.0.0/examon_core/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      558 2024-05-09 16:51:06.664204 examon_core-2.0.0/examon_core/models/__pycache__/question_response.cpython-39.pyc
+-rw-r--r--   0        0        0      831 2024-05-19 00:25:51.055946 examon_core-2.0.0/examon_core/models/code_metrics.py
+-rwxr-xr-x   0        0        0     1828 2024-05-19 04:49:09.718330 examon_core-2.0.0/examon_core/models/python_code_convertor.py
+-rwxr-xr-x   0        0        0      476 2024-05-20 01:59:07.304041 examon_core-2.0.0/examon_core/models/question.py
+-rwxr-xr-x   0        0        0      183 2024-05-20 01:34:12.943789 examon_core-2.0.0/examon_core/models/question_response.py
+-rw-r--r--   0        0        0      630 2024-05-20 01:40:58.773783 examon_core-2.0.0/examon_core/protocols/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-19 04:49:09.721246 examon_core-2.0.0/examon_core/protocols/code_decorator.py
+-rw-r--r--   0        0        0      203 2024-05-19 00:44:19.220131 examon_core-2.0.0/examon_core/protocols/code_execution_driver_protocol.py
+-rw-r--r--   0        0        0      116 2024-05-19 04:40:01.985333 examon_core-2.0.0/examon_core/protocols/code_metrics_protocol.py
+-rw-r--r--   0        0        0       96 2024-05-19 04:46:21.579121 examon_core-2.0.0/examon_core/protocols/difficulty_protocol.py
+-rw-r--r--   0        0        0      115 2024-05-19 04:45:34.871822 examon_core-2.0.0/examon_core/protocols/function_to_string_protocol.py
+-rw-r--r--   0        0        0      497 2024-05-20 01:35:31.253050 examon_core-2.0.0/examon_core/protocols/item_factory_protocol.py
+-rw-r--r--   0        0        0      111 2024-05-19 04:46:30.516801 examon_core-2.0.0/examon_core/protocols/multi_choice_protocol.py
+-rw-r--r--   0        0        0      188 2024-05-20 01:38:12.228860 examon_core-2.0.0/examon_core/protocols/question.py
+-rw-r--r--   0        0        0      113 2024-05-18 23:40:49.036245 examon_core-2.0.0/examon_core/protocols/unique_id.py
+-rw-r--r--   0        0        0      193 2024-05-20 01:44:56.733479 examon_core-2.0.0/examon_core/serializer.py
+-rw-r--r--   0        0        0      463 2024-05-20 02:08:03.835389 examon_core-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-2.0.0/PKG-INFO
```

### Comparing `examon_core-1.5.0/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc` & `examon_core-2.0.0/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-1.5.0/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc` & `examon_core-2.0.0/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-1.5.0/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc` & `examon_core-2.0.0/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-1.5.0/examon_core/code_execution/unrestricted_driver.py` & `examon_core-2.0.0/examon_core/code_execution/unrestricted_driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import builtins
 import io
 from contextlib import redirect_stdout
-from typing import List, Protocol
+from typing import List
 
+from examon_core.protocols.code_execution_driver_protocol import (
+    CodeExecutionDriverProtocol,
+)
 
-class DriverProtocol(Protocol):
-    def setup(self) -> None: ...
 
-    def teardown(self) -> None: ...
-
-    def execute(self, source_code: str) -> List[str]: ...
-
-
-class UnrestrictedDriver(DriverProtocol):
-    def __init__(self):
+class UnrestrictedDriver(CodeExecutionDriverProtocol):
+    def __init__(self) -> None:
         self.default_print = builtins.print
 
-    def setup(self):
+    def setup(self) -> None:
         builtins.print = self.default_print
 
-    def teardown(self):
+    def teardown(self) -> None:
         builtins.print = self.default_print
 
-    def execute(self, source_code):
+    def execute(self, code: str) -> List[str]:
         logs = []
 
         def new_print(*args, **kwargs):
             f = io.StringIO()
             with redirect_stdout(f):
                 self.default_print(*args, **kwargs)
             out = f.getvalue().rstrip()
             logs.append(out)
             return None
 
         builtins.print = new_print
-        exec(source_code)
+        exec(code)
         return logs
```

### Comparing `examon_core-1.5.0/examon_core/examon_in_memory_db.py` & `examon_core-2.0.0/examon_core/in_memory_db.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 import logging
 import random
+from typing import List
 
+from examon_core.filter_options import FilterOptions
+from examon_core.models.question import Question
 
-class ExamonInMemoryDatabase:
+
+class InMemoryDatabase:
     __registry = []
     __tags = []
 
     @classmethod
-    def add(cls, examon_item):
+    def add(cls, examon_item) -> None:
         logging.debug(f"Adding {examon_item} to registry")
         cls.__registry.append(examon_item)
-        for tag in examon_item.tags:
-            if tag not in cls.__tags:
-                cls.__tags.append(tag)
+        cls.__tags.extend(tag for tag in examon_item.tags if tag not in cls.__tags)
 
     @classmethod
-    def purge(cls):
+    def purge(cls) -> None:
         cls.__registry = []
-        cls.__filter = None
         cls.__tags = []
 
     @classmethod
-    def shuffle(cls):
+    def shuffle(cls) -> None:
         random.shuffle(cls.__registry)
 
     @classmethod
-    def load(cls, examon_filter=None):
+    def load(cls, filter_options: FilterOptions = None) -> List[Question]:
         results = cls.__registry
-        if examon_filter is None:
+        if filter_options is None:
             return results
 
-        def intersection(lst1, lst2):
+        def intersection(lst1: list[str], lst2: list[str]) -> list[str]:
             return list(set(lst1) & set(lst2))
 
-        def array_contains_any(array, has_one):
+        def array_contains_any(array: list[str], has_one: list[str]) -> bool:
             return len(intersection(array, has_one)) > 0
 
-        def array_contains_all(array, has_one):
-            return len(intersection(array, has_one)) == len(has_one)
+        def array_contains_all(array: list[str], has_all: list[str]) -> bool:
+            return len(intersection(array, has_all)) == len(has_all)
 
-        if examon_filter.tags_any is not None:
+        if filter_options.tags_any is not None:
             results = [
-                py_quiz_data
-                for py_quiz_data in cls.__registry
-                if array_contains_any(examon_filter.tags_any, py_quiz_data.tags)
+                questions
+                for questions in cls.__registry
+                if array_contains_any(filter_options.tags_any, questions.tags)
             ]
-        if examon_filter.tags_all is not None:
+        if filter_options.tags_all is not None:
             results = [
-                py_quiz_data
-                for py_quiz_data in cls.__registry
-                if array_contains_all(examon_filter.tags_all, py_quiz_data.tags)
+                questions
+                for questions in cls.__registry
+                if array_contains_all(filter_options.tags_all, questions.tags)
             ]
-        if examon_filter.difficulty_category is not None:
+        if filter_options.difficulty_category is not None:
             results = [
-                py_quiz_data
-                for py_quiz_data in cls.__registry
-                if examon_filter.difficulty_category
-                == py_quiz_data.metrics.categorised_difficulty
+                questions
+                for questions in cls.__registry
+                if filter_options.difficulty_category
+                == questions.metrics.categorised_difficulty
             ]
 
-        if examon_filter.max_questions is not None:
-            return results[0 : examon_filter.max_questions]
-        else:
-            return results
+        if filter_options.max_questions is not None:
+            results = results[: filter_options.max_questions]
+        return results
 
     @classmethod
-    def unique_tags(cls):
+    def unique_tags(cls) -> List[str]:
         return cls.__tags
```

### Comparing `examon_core-1.5.0/examon_core/factories/base_question.py` & `examon_core-2.0.0/examon_core/factories/question.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from ..models.question import BaseQuestion
-from .code_to_string import default_code_as_string_factory
+from ..code_execution.code_execution_sandbox import CodeExecutionSandbox
+from ..models.question import Question
 
 
-class BaseQuestionFactory:
+class QuestionFactory(object):
 
-    def __init__(self, code_execution_sandbox):
+    def __init__(self, code_execution_sandbox: CodeExecutionSandbox) -> None:
         self.code_execution_sandbox = code_execution_sandbox
 
-    def build(self, function):
-        function_src = default_code_as_string_factory(function)
-        print_logs = self.code_execution_sandbox.execute(function_src)
-        question = BaseQuestion(
-            function_src=function_src,
+    def build(self, code: str) -> Question:
+        print_logs = self.code_execution_sandbox.execute(code)
+        question = Question(
+            function_src=code,
             print_logs=print_logs,
             correct_answer=print_logs[-1],
         )
         return question
```

### Comparing `examon_core-1.5.0/examon_core/factories/code_to_string.py` & `examon_core-2.0.0/examon_core/models/python_code_convertor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,51 @@
 import inspect
 import logging
+from typing import List
 
+from ..protocols import CodeDecoratorProtocol
+from ..protocols.function_to_string_protocol import FunctionToStringProtocol
 
-class CodeAsStringFactory:
-    def __init__(self, decorators=None):
+
+class PythonCodeConvertor(FunctionToStringProtocol):
+    def __init__(self, decorators: List = None) -> None:
         self.decorators = [] if decorators is None else decorators
 
-    def build(self, function):
-        src_code = CodeAsStringFactory.function_src(function)
+    def build(self, function) -> str:
+        src_code = self.function_src(function)
         for decorator in self.decorators:
-            logging.debug(f"CodeAsStringFactory.build: {decorator}")
+            logging.debug(f"PythonCodeConvertor.build: {decorator}")
             src_code = decorator.decorate(src_code)
-            logging.debug(f"CodeAsStringFactory.build: {src_code}")
+            logging.debug(f"PythonCodeConvertor.build: {src_code}")
 
-        logging.debug(f"CodeAsStringFactory.build: {src_code}")
+        logging.debug(f"PythonCodeConvertor.build: {src_code}")
         return src_code
 
-    @staticmethod
-    def function_src(function):
-        logging.debug(f"CodeAsStringFactory.function_src: {function}")
+    def function_src(self, function):
+        logging.debug(f"PythonCodeConvertor.function_src: {function}")
         return inspect.getsource(function).strip()
 
 
-class SourceCodeCommentsDecorator:
-    def __init__(self, hints):
-        self.hints = hints
-
-    def decorate(self, src_code):
-        all_hints = ""
-        if self.hints is None:
-            return all_hints
-        else:
-            for hint in self.hints:
-                all_hints += f"# {hint}\n"
-        all_hints = f"# Hints:\n{all_hints}\n\n"
-        return all_hints + src_code
+class SourceCodeCommentsDecorator(CodeDecoratorProtocol):
+    def __init__(self, hints: List[str]) -> None:
+        self.hints = hints or []
+
+    def decorate(self, src_code) -> str:
+        all_hints = "\n".join(f"# {hint}" for hint in self.hints)
+        return f"# Hints:\n{all_hints}\n\n{src_code}" if all_hints else src_code
 
 
-class RemoveQuizItemDecorator:
-    def decorate(self, src_code):
+class RemoveQuizItemDecorator(CodeDecoratorProtocol):
+    def decorate(self, src_code) -> str:
         return src_code[src_code.find("def") :]
 
 
-class AppendPrintDecorator:
-    def __init__(self, function_name, param=""):
+class AppendPrintDecorator(CodeDecoratorProtocol):
+    def __init__(self, function_name, param="") -> None:
         self.function_name = function_name
         self.param = param
 
-    def decorate(self, src_code):
+    def decorate(self, src_code) -> str:
         if isinstance(self.param, str) and self.param != "":
             self.param = f"'{self.param}'"
         println = f"\n\nprint({self.function_name}({self.param}))"
         return src_code + println
-
-
-def default_code_as_string_factory(function, param=""):
-    return CodeAsStringFactory(
-        [RemoveQuizItemDecorator(), AppendPrintDecorator(function.__name__, param)]
-    ).build(function)
```

### Comparing `examon_core-1.5.0/examon_core/factories/item.py` & `examon_core-2.0.0/examon_core/factories/examon.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,126 +1,105 @@
 import logging
-from typing import Any, List, Protocol
+from typing import Callable, List, Type
 
-from examon_core.code_execution.unrestricted_driver import DriverProtocol
-from examon_core.factories.multi_choice import MultiChoiceProtocol
-from examon_core.generate_unique_id import GenerateUniqueIdProtocol
-from examon_core.metrics.calc_standard import CalcStandardMetricsProtocol
-from examon_core.metrics.categorize_difficulty import CategorizeDifficultyProtocol
+from examon_core.protocols.function_to_string_protocol import FunctionToStringProtocol
 
-from ..code_execution.sandbox import CodeExecutionSandbox
+from ..code_execution.code_execution_sandbox import CodeExecutionSandbox
 from ..global_settings import ExamonGlobalSettings
-from .base_question import BaseQuestionFactory
-from .input_param_question import InputParamQuestionFactory
+from ..protocols import (
+    CodeExecutionDriverProtocol,
+    CodeMetricsProtocol,
+    DifficultyProtocol,
+    ItemFactoryProtocol,
+    MultiChoiceProtocol,
+    UniqueIdProtocol,
+)
 from .metrics import CodeMetricsFactory
-from .multi_choice_question import MultiChoiceQuestionFactory
+from .question import QuestionFactory
 
 
-class InvalidAnswerException(Exception):
-    pass
-
-
-class ItemFactoryProtocol(Protocol):
-    def build(
-        self,
-        function=None,
-        tags=None,
-        internal_id=None,
-        hints=None,
-        param1=None,
-        choices=None,
-        choice_list=None,
-        repository=None,
-        version=None,
-        metrics=None,
-    ) -> Any:
-        pass
-
-    def choice_list_as_string(self, choices) -> List[str]:
-        pass
-
-
-class ItemFactory(ItemFactoryProtocol):
+class ExamonFactory(ItemFactoryProtocol):
     def __init__(
         self,
-        code_execution_driver_class: DriverProtocol = None,
-        multi_choice_factory_class: MultiChoiceProtocol = None,
-        calc_standard_metrics_class: CalcStandardMetricsProtocol = None,
-        categorize_difficulty_class: CategorizeDifficultyProtocol = None,
-        unique_id_strategy: GenerateUniqueIdProtocol = None,
+        code_execution_driver_class: Type[CodeExecutionDriverProtocol] = None,
+        multi_choice_class: Type[MultiChoiceProtocol] = None,
+        calc_standard_metrics_class: Type[CodeMetricsProtocol] = None,
+        categorize_difficulty_class: Type[DifficultyProtocol] = None,
+        unique_id_strategy: Type[UniqueIdProtocol] = None,
+        code_to_string: Type[FunctionToStringProtocol] = None,
     ) -> None:
         self.code_execution_driver_class = code_execution_driver_class
-        self.multi_chioce_factory_class = multi_choice_factory_class
+        self.multi_choice_class = multi_choice_class
         self.calc_standard_metrics_strategy = calc_standard_metrics_class
         self.categorize_difficulty_strategy = categorize_difficulty_class
         self.unique_id_strategy = unique_id_strategy
+        self.code_to_string = code_to_string
 
     def build(
         self,
-        function=None,
-        tags=None,
-        internal_id=None,
-        hints=None,
-        param1=None,
-        choices=None,
-        choice_list=None,
-        repository=None,
-        version=None,
-        metrics=None,
+        function: Callable = None,
+        tags: List[str] = None,
+        internal_id: str = None,
+        hints: List[str] = None,
+        choices: List[str] = None,
+        choice_list: List[str] = None,
+        repository: str = None,
+        version: str = None,
+        metrics: bool = None,
     ):
 
         result_choice_list = self.choice_list_as_string(choices or choice_list)
         ces = CodeExecutionSandbox(self.code_execution_driver_class)
 
-        # Build
-        if param1 is not None:
-            question = InputParamQuestionFactory(ces).build(function, param1)
-        elif result_choice_list:
-            question = MultiChoiceQuestionFactory(
-                code_execution_sandbox=ces,
-                multi_choice_factory_class=self.multi_chioce_factory_class,
-            ).build(function, result_choice_list)
-        else:
-            question = BaseQuestionFactory(ces).build(function)
+        function_src = self.code_to_string().build(function)
+
+        question = QuestionFactory(ces).build(function_src)
+
+        if result_choice_list:
+            question.choices = self.multi_choice_class(
+                question.print_logs[-1], choice_list or choices
+            ).build()
 
         if metrics:
             question.metrics = CodeMetricsFactory(
-                calc_standard_metrics_strategy=self.calc_standard_metrics_strategy,
-                categorize_difficulty_strategy=self.categorize_difficulty_strategy,
+                calc_standard_metrics_class=self.calc_standard_metrics_strategy,
+                categorize_difficulty_class=self.categorize_difficulty_strategy,
             ).build(question.function_src)
 
         question.hints = hints
         question.internal_id = internal_id
         question.tags = tags
         question.repository = repository
         question.version = version
 
         question.unique_id = self.unique_id_strategy().run(question.function_src)
         logging.debug(f"QuestionFactory.build: {question}")
         return question
 
-    def choice_list_as_string(self, choices):
+    def choice_list_as_string(self, choices) -> List[str]:
         result_choice_list = []
         if choices:
             result_choice_list = list(map(lambda x: str(x), choices))
         return result_choice_list
 
     @staticmethod
     def default_instance(
-        code_execution_driver_class=None,
-        multi_chioce_factory_class=None,
-        calc_standard_metrics_strategy=None,
-        categorize_difficulty_strategy=None,
-        unique_id_strategy=None,
-    ):
-        return ItemFactory(
+        code_execution_driver_class: Type[CodeExecutionDriverProtocol] = None,
+        multi_choice_factory_class: Type[MultiChoiceProtocol] = None,
+        calc_standard_metrics_strategy: Type[CodeMetricsProtocol] = None,
+        categorize_difficulty_strategy: Type[DifficultyProtocol] = None,
+        unique_id_strategy: Type[UniqueIdProtocol] = None,
+        code_to_string: Type[FunctionToStringProtocol] = None,
+    ) -> ItemFactoryProtocol:
+        return ExamonFactory(
             code_execution_driver_class=code_execution_driver_class
             or ExamonGlobalSettings.code_execution_driver_class,
-            multi_choice_factory_class=multi_chioce_factory_class
-            or ExamonGlobalSettings.multi_choice_factory_class,
+            multi_choice_class=multi_choice_factory_class
+            or ExamonGlobalSettings.multi_choice_class,
             calc_standard_metrics_class=calc_standard_metrics_strategy
             or ExamonGlobalSettings.calc_standard_metrics_strategy,
             categorize_difficulty_class=categorize_difficulty_strategy
             or ExamonGlobalSettings.categorize_difficulty_strategy,
             unique_id_strategy=unique_id_strategy
             or ExamonGlobalSettings.unique_id_strategy,
+            code_to_string=code_to_string or ExamonGlobalSettings.code_to_string,
         )
```

### Comparing `examon_core-1.5.0/examon_core/factories/metrics.py` & `examon_core-2.0.0/examon_core/factories/metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import ast
 import logging
+from typing import Type
 
-from ..metrics.calc_standard import CalcStandardMetrics
-from ..metrics.categorize_difficulty import CategorizeDifficulty
 from ..metrics.code_analysis_visitor import CodeAnalysisVisitor
 from ..models.code_metrics import CodeMetrics
+from ..protocols import CodeMetricsProtocol, DifficultyProtocol
 
 
-class CodeMetricsFactory:
+class CodeMetricsFactory(object):
     def __init__(
         self,
-        calc_standard_metrics_strategy=CalcStandardMetrics,
-        categorize_difficulty_strategy=CategorizeDifficulty,
-    ):
-        self.calc_standard_metrics_strategy = calc_standard_metrics_strategy
-        self.categorize_difficulty_strategy = categorize_difficulty_strategy
+        calc_standard_metrics_class: Type[CodeMetricsProtocol],
+        categorize_difficulty_class: Type[DifficultyProtocol],
+    ) -> None:
+        self.calc_standard_metrics_strategy = calc_standard_metrics_class
+        self.categorize_difficulty_strategy = categorize_difficulty_class
 
-    def build(self, code_as_string):
-        if code_as_string == "" or code_as_string is None:
+    def build(self, code: str) -> CodeMetrics:
+        if code == "" or code is None:
             raise Exception("Cannot use empty string")
         cm = CodeMetrics()
 
-        standard_metrics = self.calc_standard_metrics_strategy(code_as_string).run()
+        standard_metrics = self.calc_standard_metrics_strategy(code).run()
 
         cm.difficulty = standard_metrics["difficulty"]
         cm.no_of_functions = standard_metrics["no_of_functions"]
         cm.loc = standard_metrics["loc"]
         cm.lloc = standard_metrics["lloc"]
         cm.sloc = standard_metrics["sloc"]
         cm.categorised_difficulty = self.categorize_difficulty_strategy(cm).run()
 
-        tree = ast.parse(code_as_string)
+        tree = ast.parse(code)
         m = CodeAnalysisVisitor()
         m.visit(tree)
 
         cm.imports = list(m.modules)
         cm.calls = list(m.calls)
         cm.extra = list(m.counts)
         logging.debug(f"CodeMetricsFactory.build: {cm}")
```

### Comparing `examon_core-1.5.0/examon_core/global_settings.py` & `examon_core-2.0.0/examon_core/global_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from .code_execution.unrestricted_driver import UnrestrictedDriver
-from .examon_in_memory_db import ExamonInMemoryDatabase
+from .factories.default_code_to_string_factory import DefaultCodeToStringFactory
 from .factories.multi_choice import MultiChoiceFactory
 from .generate_unique_id import GenerateUniqueId
-from .metrics.calc_standard import CalcStandardMetrics
+from .in_memory_db import InMemoryDatabase
+from .metrics.calc_standard_metrics import CalcStandardMetrics
 from .metrics.categorize_difficulty import CategorizeDifficulty
 
 
 class ExamonGlobalSettings:
-    # Global properties
     record_metrics = True
     repository = None
     version = None
 
-    # QuestionFactory
     code_execution_driver_class = UnrestrictedDriver
-    multi_choice_factory_class = MultiChoiceFactory
+    multi_choice_class = MultiChoiceFactory
     calc_standard_metrics_strategy = CalcStandardMetrics
     categorize_difficulty_strategy = CategorizeDifficulty
     unique_id_strategy = GenerateUniqueId
+    code_to_string = DefaultCodeToStringFactory
 
-    # Save the items
-    in_memory_db = ExamonInMemoryDatabase
+    in_memory_db = InMemoryDatabase
```

### Comparing `examon_core-1.5.0/examon_core/metrics/code_analysis_visitor.py` & `examon_core-2.0.0/examon_core/metrics/code_analysis_visitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import defaultdict
 from types import MethodType
 
 from .visit_methods import visit_methods
 
 
 class CodeAnalysisVisitor(ast.NodeVisitor):
-    def __init__(self):
+    def __init__(self) -> None:
         self.functions = set()
         self.calls = set()
         self.modules = set()
         self.counts = defaultdict(int)
         for visit_method in visit_methods:
             env_setter = self.make_visit(visit_method)
             method = MethodType(env_setter, self)
@@ -20,26 +20,26 @@
         self.counts[type(node).__name__] += 1
 
     # record
     def visit_FunctionDef(self, node):
         self.functions.add(node.name)
         self.generic_visit(node)
 
-    def visit_Call(self, node):
+    def visit_Call(self, node) -> None:
         if node.func.__class__ == ast.Name:
             self.calls.add(node.func.id)
         elif node.func.__class__ == ast.Attribute:
             self.calls.add(node.func.attr)
         self.generic_visit(node)
 
-    def visit_Import(self, node):
+    def visit_Import(self, node) -> None:
         for name in node.names:
             self.modules.add(name.name.split(".")[0])
 
-    def visit_ImportFrom(self, node):
+    def visit_ImportFrom(self, node) -> None:
         if node.module is not None and node.level == 0:
             self.modules.add(node.module.split(".")[0])
 
     @staticmethod
     def make_visit(_):
         def visit(self, node):
             self.record(node)
```

### Comparing `examon_core-1.5.0/examon_core/metrics/visit_methods.py` & `examon_core-2.0.0/examon_core/metrics/visit_methods.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.5.0/examon_core/models/__pycache__/question_response.cpython-39.pyc` & `examon_core-2.0.0/examon_core/models/__pycache__/question_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-1.5.0/examon_core/models/code_metrics.py` & `examon_core-2.0.0/examon_core/models/code_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     sloc: int = None
     difficulty: float = None
     categorised_difficulty: str = None
     imports: list[str] = None
     calls: list[str] = None
     counts: dict[str, int] = None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"CodeMetrics(difficulty: {self.difficulty},"
             f"no_of_functions: {self.no_of_functions}, "
             f"loc: {self.loc}, "
             f"lloc: {self.lloc}, "
             f"sloc: {self.sloc}, "
             f"difficulty: {self.difficulty}, "
```


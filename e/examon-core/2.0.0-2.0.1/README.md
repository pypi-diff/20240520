# Comparing `tmp/examon_core-2.0.0.tar.gz` & `tmp/examon_core-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-2.0.0.tar", max compression
+gzip compressed data, was "examon_core-2.0.1.tar", max compression
```

## Comparing `examon_core-2.0.0.tar` & `examon_core-2.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0        0 2024-05-18 14:31:03.633904 examon_core-2.0.0/examon_core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661649 examon_core-2.0.0/examon_core/code_execution/__init__.py
--rw-r--r--   0        0        0      179 2024-05-09 16:51:06.661857 examon_core-2.0.0/examon_core/code_execution/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1192 2024-05-09 16:51:06.661998 examon_core-2.0.0/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc
--rw-r--r--   0        0        0     1558 2024-05-09 16:51:06.662136 examon_core-2.0.0/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc
--rw-r--r--   0        0        0     1381 2024-05-09 16:51:06.662279 examon_core-2.0.0/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc
--rw-r--r--   0        0        0      431 2024-05-19 04:26:54.793493 examon_core-2.0.0/examon_core/code_execution/code_execution_sandbox.py
--rw-r--r--   0        0        0      870 2024-05-19 04:26:54.804105 examon_core-2.0.0/examon_core/code_execution/unrestricted_driver.py
--rwxr-xr-x   0        0        0     1764 2024-05-20 01:48:53.993256 examon_core-2.0.0/examon_core/examon.py
--rw-r--r--   0        0        0        0 2024-05-19 00:55:24.523321 examon_core-2.0.0/examon_core/factories/__init__.py
--rw-r--r--   0        0        0      491 2024-05-19 04:45:32.637915 examon_core-2.0.0/examon_core/factories/default_code_to_string_factory.py
--rw-r--r--   0        0        0     4261 2024-05-20 02:02:18.019024 examon_core-2.0.0/examon_core/factories/examon.py
--rw-r--r--   0        0        0     1427 2024-05-20 01:50:38.841503 examon_core-2.0.0/examon_core/factories/metrics.py
--rw-r--r--   0        0        0      519 2024-05-20 01:51:38.500379 examon_core-2.0.0/examon_core/factories/multi_choice.py
--rw-r--r--   0        0        0      565 2024-05-20 01:34:12.947319 examon_core-2.0.0/examon_core/factories/question.py
--rw-r--r--   0        0        0      220 2024-05-20 01:39:45.912421 examon_core-2.0.0/examon_core/filter_options.py
--rw-r--r--   0        0        0      276 2024-05-18 23:56:59.870681 examon_core-2.0.0/examon_core/generate_unique_id.py
--rw-r--r--   0        0        0      859 2024-05-20 01:45:29.939643 examon_core-2.0.0/examon_core/global_settings.py
--rw-r--r--   0        0        0     1915 2024-05-20 01:25:50.546495 examon_core-2.0.0/examon_core/gof/decorators.py
--rwxr-xr-x   0        0        0     2225 2024-05-20 01:59:06.149962 examon_core-2.0.0/examon_core/in_memory_db.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663463 examon_core-2.0.0/examon_core/metrics/__init__.py
--rw-r--r--   0        0        0      609 2024-05-20 01:37:01.972038 examon_core-2.0.0/examon_core/metrics/calc_standard_metrics.py
--rw-r--r--   0        0        0      459 2024-05-20 01:52:59.926637 examon_core-2.0.0/examon_core/metrics/categorize_difficulty.py
--rw-r--r--   0        0        0     1431 2024-05-19 00:25:48.026342 examon_core-2.0.0/examon_core/metrics/code_analysis_visitor.py
--rw-r--r--   0        0        0     1340 2024-05-09 16:51:06.663807 examon_core-2.0.0/examon_core/metrics/visit_methods.py
--rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663934 examon_core-2.0.0/examon_core/models/__init__.py
--rw-r--r--   0        0        0      171 2024-05-09 16:51:06.664099 examon_core-2.0.0/examon_core/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      558 2024-05-09 16:51:06.664204 examon_core-2.0.0/examon_core/models/__pycache__/question_response.cpython-39.pyc
--rw-r--r--   0        0        0      831 2024-05-19 00:25:51.055946 examon_core-2.0.0/examon_core/models/code_metrics.py
--rwxr-xr-x   0        0        0     1828 2024-05-19 04:49:09.718330 examon_core-2.0.0/examon_core/models/python_code_convertor.py
--rwxr-xr-x   0        0        0      476 2024-05-20 01:59:07.304041 examon_core-2.0.0/examon_core/models/question.py
--rwxr-xr-x   0        0        0      183 2024-05-20 01:34:12.943789 examon_core-2.0.0/examon_core/models/question_response.py
--rw-r--r--   0        0        0      630 2024-05-20 01:40:58.773783 examon_core-2.0.0/examon_core/protocols/__init__.py
--rw-r--r--   0        0        0      115 2024-05-19 04:49:09.721246 examon_core-2.0.0/examon_core/protocols/code_decorator.py
--rw-r--r--   0        0        0      203 2024-05-19 00:44:19.220131 examon_core-2.0.0/examon_core/protocols/code_execution_driver_protocol.py
--rw-r--r--   0        0        0      116 2024-05-19 04:40:01.985333 examon_core-2.0.0/examon_core/protocols/code_metrics_protocol.py
--rw-r--r--   0        0        0       96 2024-05-19 04:46:21.579121 examon_core-2.0.0/examon_core/protocols/difficulty_protocol.py
--rw-r--r--   0        0        0      115 2024-05-19 04:45:34.871822 examon_core-2.0.0/examon_core/protocols/function_to_string_protocol.py
--rw-r--r--   0        0        0      497 2024-05-20 01:35:31.253050 examon_core-2.0.0/examon_core/protocols/item_factory_protocol.py
--rw-r--r--   0        0        0      111 2024-05-19 04:46:30.516801 examon_core-2.0.0/examon_core/protocols/multi_choice_protocol.py
--rw-r--r--   0        0        0      188 2024-05-20 01:38:12.228860 examon_core-2.0.0/examon_core/protocols/question.py
--rw-r--r--   0        0        0      113 2024-05-18 23:40:49.036245 examon_core-2.0.0/examon_core/protocols/unique_id.py
--rw-r--r--   0        0        0      193 2024-05-20 01:44:56.733479 examon_core-2.0.0/examon_core/serializer.py
--rw-r--r--   0        0        0      463 2024-05-20 02:08:03.835389 examon_core-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-18 14:31:03.633904 examon_core-2.0.1/examon_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.661649 examon_core-2.0.1/examon_core/code_execution/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-09 16:51:06.661857 examon_core-2.0.1/examon_core/code_execution/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1192 2024-05-09 16:51:06.661998 examon_core-2.0.1/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc
+-rw-r--r--   0        0        0     1558 2024-05-09 16:51:06.662136 examon_core-2.0.1/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc
+-rw-r--r--   0        0        0     1381 2024-05-09 16:51:06.662279 examon_core-2.0.1/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc
+-rw-r--r--   0        0        0      431 2024-05-19 04:26:54.793493 examon_core-2.0.1/examon_core/code_execution/code_execution_sandbox.py
+-rw-r--r--   0        0        0      870 2024-05-19 04:26:54.804105 examon_core-2.0.1/examon_core/code_execution/unrestricted_driver.py
+-rwxr-xr-x   0        0        0     1798 2024-05-20 03:05:37.574514 examon_core-2.0.1/examon_core/examon.py
+-rw-r--r--   0        0        0        0 2024-05-19 00:55:24.523321 examon_core-2.0.1/examon_core/factories/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-19 04:45:32.637915 examon_core-2.0.1/examon_core/factories/default_code_to_string_factory.py
+-rw-r--r--   0        0        0     4291 2024-05-20 03:07:24.029505 examon_core-2.0.1/examon_core/factories/examon.py
+-rw-r--r--   0        0        0     1457 2024-05-20 03:07:24.031498 examon_core-2.0.1/examon_core/factories/metrics.py
+-rw-r--r--   0        0        0      529 2024-05-20 03:07:24.027027 examon_core-2.0.1/examon_core/factories/multi_choice.py
+-rw-r--r--   0        0        0      585 2024-05-20 03:07:24.036386 examon_core-2.0.1/examon_core/factories/question.py
+-rw-r--r--   0        0        0      220 2024-05-20 01:39:45.912421 examon_core-2.0.1/examon_core/filter_options.py
+-rw-r--r--   0        0        0      276 2024-05-18 23:56:59.870681 examon_core-2.0.1/examon_core/generate_unique_id.py
+-rw-r--r--   0        0        0      924 2024-05-20 03:04:14.951626 examon_core-2.0.1/examon_core/global_settings.py
+-rw-r--r--   0        0        0     1915 2024-05-20 01:25:50.546495 examon_core-2.0.1/examon_core/gof/decorators.py
+-rwxr-xr-x   0        0        0     2219 2024-05-20 02:59:35.917403 examon_core-2.0.1/examon_core/in_memory_db.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663463 examon_core-2.0.1/examon_core/metrics/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-20 01:37:01.972038 examon_core-2.0.1/examon_core/metrics/calc_standard_metrics.py
+-rw-r--r--   0        0        0      459 2024-05-20 01:52:59.926637 examon_core-2.0.1/examon_core/metrics/categorize_difficulty.py
+-rw-r--r--   0        0        0     1450 2024-05-20 03:07:24.033821 examon_core-2.0.1/examon_core/metrics/code_analysis_visitor.py
+-rw-r--r--   0        0        0     1340 2024-05-09 16:51:06.663807 examon_core-2.0.1/examon_core/metrics/visit_methods.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:51:06.663934 examon_core-2.0.1/examon_core/models/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-09 16:51:06.664099 examon_core-2.0.1/examon_core/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      558 2024-05-09 16:51:06.664204 examon_core-2.0.1/examon_core/models/__pycache__/question_response.cpython-39.pyc
+-rw-r--r--   0        0        0      831 2024-05-19 00:25:51.055946 examon_core-2.0.1/examon_core/models/code_metrics.py
+-rwxr-xr-x   0        0        0     1848 2024-05-20 03:05:54.150617 examon_core-2.0.1/examon_core/models/python_code_convertor.py
+-rwxr-xr-x   0        0        0      494 2024-05-20 03:05:37.571308 examon_core-2.0.1/examon_core/models/question.py
+-rwxr-xr-x   0        0        0      201 2024-05-20 03:05:37.567459 examon_core-2.0.1/examon_core/models/question_response.py
+-rw-r--r--   0        0        0      630 2024-05-20 01:40:58.773783 examon_core-2.0.1/examon_core/protocols/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-19 04:49:09.721246 examon_core-2.0.1/examon_core/protocols/code_decorator.py
+-rw-r--r--   0        0        0      203 2024-05-19 00:44:19.220131 examon_core-2.0.1/examon_core/protocols/code_execution_driver_protocol.py
+-rw-r--r--   0        0        0      116 2024-05-19 04:40:01.985333 examon_core-2.0.1/examon_core/protocols/code_metrics_protocol.py
+-rw-r--r--   0        0        0       96 2024-05-19 04:46:21.579121 examon_core-2.0.1/examon_core/protocols/difficulty_protocol.py
+-rw-r--r--   0        0        0      115 2024-05-19 04:45:34.871822 examon_core-2.0.1/examon_core/protocols/function_to_string_protocol.py
+-rw-r--r--   0        0        0      497 2024-05-20 01:35:31.253050 examon_core-2.0.1/examon_core/protocols/item_factory_protocol.py
+-rw-r--r--   0        0        0      111 2024-05-19 04:46:30.516801 examon_core-2.0.1/examon_core/protocols/multi_choice_protocol.py
+-rw-r--r--   0        0        0      188 2024-05-20 01:38:12.228860 examon_core-2.0.1/examon_core/protocols/question.py
+-rw-r--r--   0        0        0      113 2024-05-18 23:40:49.036245 examon_core-2.0.1/examon_core/protocols/unique_id.py
+-rw-r--r--   0        0        0      193 2024-05-20 01:44:56.733479 examon_core-2.0.1/examon_core/serializer.py
+-rw-r--r--   0        0        0      463 2024-05-20 03:07:50.002606 examon_core-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 examon_core-2.0.1/PKG-INFO
```

### Comparing `examon_core-2.0.0/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc` & `examon_core-2.0.1/examon_core/code_execution/__pycache__/print_collector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc` & `examon_core-2.0.1/examon_core/code_execution/__pycache__/restricted_python_driver.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc` & `examon_core-2.0.1/examon_core/code_execution/__pycache__/unrestricted_driver.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/code_execution/unrestricted_driver.py` & `examon_core-2.0.1/examon_core/code_execution/unrestricted_driver.py`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/examon.py` & `examon_core-2.0.1/examon_core/examon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, List
 
-from protocols import (
+from examon_core.protocols import (
     CodeExecutionDriverProtocol,
     CodeMetricsProtocol,
     DifficultyProtocol,
     FunctionToStringProtocol,
     UniqueIdProtocol,
 )
 
-from .factories.examon import ExamonFactory
-from .global_settings import ExamonGlobalSettings
+from examon_core.factories.examon import ExamonFactory
+from examon_core.global_settings import ExamonGlobalSettings
 
 
 def examon(
     internal_id: str = None,
     choices: List[Any] = None,
     choice_list: List[Any] = None,
     tags: List[str] = None,
```

### Comparing `examon_core-2.0.0/examon_core/factories/examon.py` & `examon_core-2.0.1/examon_core/factories/examon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Callable, List, Type
 
 from examon_core.protocols.function_to_string_protocol import FunctionToStringProtocol
 
-from ..code_execution.code_execution_sandbox import CodeExecutionSandbox
-from ..global_settings import ExamonGlobalSettings
-from ..protocols import (
+from examon_core.code_execution.code_execution_sandbox import CodeExecutionSandbox
+from examon_core.global_settings import ExamonGlobalSettings
+from examon_core.protocols import (
     CodeExecutionDriverProtocol,
     CodeMetricsProtocol,
     DifficultyProtocol,
     ItemFactoryProtocol,
     MultiChoiceProtocol,
     UniqueIdProtocol,
 )
```

### Comparing `examon_core-2.0.0/examon_core/factories/metrics.py` & `examon_core-2.0.1/examon_core/factories/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import logging
 from typing import Type
 
-from ..metrics.code_analysis_visitor import CodeAnalysisVisitor
-from ..models.code_metrics import CodeMetrics
-from ..protocols import CodeMetricsProtocol, DifficultyProtocol
+from examon_core.metrics.code_analysis_visitor import CodeAnalysisVisitor
+from examon_core.models.code_metrics import CodeMetrics
+from examon_core.protocols import CodeMetricsProtocol, DifficultyProtocol
 
 
 class CodeMetricsFactory(object):
     def __init__(
         self,
         calc_standard_metrics_class: Type[CodeMetricsProtocol],
         categorize_difficulty_class: Type[DifficultyProtocol],
```

### Comparing `examon_core-2.0.0/examon_core/factories/multi_choice.py` & `examon_core-2.0.1/examon_core/factories/multi_choice.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from ..protocols.multi_choice_protocol import MultiChoiceProtocol
+from examon_core.protocols.multi_choice_protocol import MultiChoiceProtocol
 
 
 class MultiChoiceFactory(MultiChoiceProtocol):
     def __init__(self, correct_answer, choice_list=None) -> None:
         self.correct_answer = correct_answer
         self.choice_list = choice_list
```

### Comparing `examon_core-2.0.0/examon_core/factories/question.py` & `examon_core-2.0.1/examon_core/factories/question.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..code_execution.code_execution_sandbox import CodeExecutionSandbox
-from ..models.question import Question
+from examon_core.code_execution.code_execution_sandbox import CodeExecutionSandbox
+from examon_core.models.question import Question
 
 
 class QuestionFactory(object):
 
     def __init__(self, code_execution_sandbox: CodeExecutionSandbox) -> None:
         self.code_execution_sandbox = code_execution_sandbox
```

### Comparing `examon_core-2.0.0/examon_core/gof/decorators.py` & `examon_core-2.0.1/examon_core/gof/decorators.py`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/in_memory_db.py` & `examon_core-2.0.1/examon_core/in_memory_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import random
 from typing import List
 
 from examon_core.filter_options import FilterOptions
 from examon_core.models.question import Question
 
 
-class InMemoryDatabase:
+class InMemoryDB:
     __registry = []
     __tags = []
 
     @classmethod
     def add(cls, examon_item) -> None:
         logging.debug(f"Adding {examon_item} to registry")
         cls.__registry.append(examon_item)
```

### Comparing `examon_core-2.0.0/examon_core/metrics/calc_standard_metrics.py` & `examon_core-2.0.1/examon_core/metrics/calc_standard_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/metrics/code_analysis_visitor.py` & `examon_core-2.0.1/examon_core/metrics/code_analysis_visitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 from collections import defaultdict
 from types import MethodType
 
-from .visit_methods import visit_methods
+from examon_core.metrics.visit_methods import visit_methods
 
 
 class CodeAnalysisVisitor(ast.NodeVisitor):
     def __init__(self) -> None:
         self.functions = set()
         self.calls = set()
         self.modules = set()
```

### Comparing `examon_core-2.0.0/examon_core/metrics/visit_methods.py` & `examon_core-2.0.1/examon_core/metrics/visit_methods.py`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/models/__pycache__/question_response.cpython-39.pyc` & `examon_core-2.0.1/examon_core/models/__pycache__/question_response.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/models/code_metrics.py` & `examon_core-2.0.1/examon_core/models/code_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-2.0.0/examon_core/models/python_code_convertor.py` & `examon_core-2.0.1/examon_core/models/python_code_convertor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import logging
 from typing import List
 
-from ..protocols import CodeDecoratorProtocol
-from ..protocols.function_to_string_protocol import FunctionToStringProtocol
+from examon_core.protocols import CodeDecoratorProtocol
+from examon_core.protocols.function_to_string_protocol import FunctionToStringProtocol
 
 
 class PythonCodeConvertor(FunctionToStringProtocol):
     def __init__(self, decorators: List = None) -> None:
         self.decorators = [] if decorators is None else decorators
 
     def build(self, function) -> str:
```

### Comparing `examon_core-2.0.0/examon_core/protocols/__init__.py` & `examon_core-2.0.1/examon_core/protocols/__init__.py`

 * *Files identical despite different names*


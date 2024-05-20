# Comparing `tmp/cybertron_framework-0.0.1.tar.gz` & `tmp/cybertron_framework-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybertron_framework-0.0.1.tar", max compression
+gzip compressed data, was "cybertron_framework-0.0.2.tar", max compression
```

## Comparing `cybertron_framework-0.0.1.tar` & `cybertron_framework-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0    35149 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/LICENSE
--rw-r--r--   0        0        0    15554 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/environment/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/environment/__tests__/__init__.py
--rw-r--r--   0        0        0     2358 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/environment/__tests__/test_environment.py
--rw-r--r--   0        0        0     1764 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/environment/__tests__/test_environment_interface.py
--rw-r--r--   0        0        0     1421 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/environment/environment.py
--rw-r--r--   0        0        0      851 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/environment/environment_interface.py
--rw-r--r--   0        0        0      493 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/exception/abort_process_exception.py
--rw-r--r--   0        0        0      294 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/exception/no_data_to_process_exception.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/helper/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/helper/__tests__/__init__.py
--rw-r--r--   0        0        0      976 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/helper/__tests__/test_benchmark.py
--rw-r--r--   0        0        0     1767 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/helper/__tests__/test_logger.py
--rw-r--r--   0        0        0      344 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/helper/benchmark.py
--rw-r--r--   0        0        0     1012 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/helper/logger.py
--rw-r--r--   0        0        0      361 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/input/input_manager_interface.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/__tests__/__init__.py
--rw-r--r--   0        0        0     3065 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/__tests__/test_abstract_orchestrator.py
--rw-r--r--   0        0        0     2566 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/abstract_orchestrator.py
--rw-r--r--   0        0        0     1012 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/orchestrator_interface.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/types/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/types/__tests__/__init__.py
--rw-r--r--   0        0        0     5991 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/types/__tests__/test_synchronous.py
--rw-r--r--   0        0        0     3386 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/orchestrator/types/synchronous.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/output/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/output/__tests__/__init__.py
--rw-r--r--   0        0        0      871 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/output/__tests__/test_output_manager_interface.py
--rw-r--r--   0        0        0      364 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/output/output_manager_interface.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/transformer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/transformer/__tests__/__init__.py
--rw-r--r--   0        0        0      977 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/transformer/__tests__/test_transformer_manager_interface.py
--rw-r--r--   0        0        0      375 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/cybertron_framework/transformer/transformer_manager_interface.py
--rw-r--r--   0        0        0      799 2024-04-29 10:51:36.743420 cybertron_framework-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    16277 1970-01-01 00:00:00.000000 cybertron_framework-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-20 10:52:37.792438 cybertron_framework-0.0.2/LICENSE
+-rw-r--r--   0        0        0    17340 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/environment/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/environment/__tests__/__init__.py
+-rw-r--r--   0        0        0     2359 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/environment/__tests__/test_environment.py
+-rw-r--r--   0        0        0     1764 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/environment/__tests__/test_environment_interface.py
+-rw-r--r--   0        0        0     1422 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/environment/environment.py
+-rw-r--r--   0        0        0      851 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/environment/environment_interface.py
+-rw-r--r--   0        0        0      493 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/exception/abort_process_exception.py
+-rw-r--r--   0        0        0      294 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/exception/no_data_to_process_exception.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/helper/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/helper/__tests__/__init__.py
+-rw-r--r--   0        0        0      976 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/helper/__tests__/test_benchmark.py
+-rw-r--r--   0        0        0     1782 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/helper/__tests__/test_logger.py
+-rw-r--r--   0        0        0      344 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/helper/benchmark.py
+-rw-r--r--   0        0        0      930 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/helper/logger.py
+-rw-r--r--   0        0        0      361 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/input/input_manager_interface.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/__tests__/__init__.py
+-rw-r--r--   0        0        0     3065 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/__tests__/test_abstract_orchestrator.py
+-rw-r--r--   0        0        0     2575 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/abstract_orchestrator.py
+-rw-r--r--   0        0        0     1012 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/orchestrator_interface.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/types/__tests__/__init__.py
+-rw-r--r--   0        0        0     5545 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/types/__tests__/test_sequence.py
+-rw-r--r--   0        0        0     5939 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/types/__tests__/test_synchronous.py
+-rw-r--r--   0        0        0     3676 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/types/sequence.py
+-rw-r--r--   0        0        0     3376 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/orchestrator/types/synchronous.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/output/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/output/__tests__/__init__.py
+-rw-r--r--   0        0        0      871 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/output/__tests__/test_output_manager_interface.py
+-rw-r--r--   0        0        0      365 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/output/output_manager_interface.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/transformer/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/transformer/__tests__/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/transformer/__tests__/test_transformer_manager_interface.py
+-rw-r--r--   0        0        0      376 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/cybertron_framework/transformer/transformer_manager_interface.py
+-rw-r--r--   0        0        0      798 2024-05-20 10:52:37.796438 cybertron_framework-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    18063 1970-01-01 00:00:00.000000 cybertron_framework-0.0.2/PKG-INFO
```

### Comparing `cybertron_framework-0.0.1/LICENSE` & `cybertron_framework-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cybertron_framework-0.0.1/README.md` & `cybertron_framework-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,52 @@
 # Cybertron: Transformation framework
 Cybertron is a framework intended for retrieving data from one or several repositories, transforming it, and storing in output repositories.
 For this purpose, pipelines are defined to manage the different stages of the process.
 
+[![GoodCod3 - cybertron-framework](https://img.shields.io/static/v1?label=GoodCod3&message=cybertron-framework&color=blue&logo=github)](https://github.com/GoodCod3/cybertron-framework "Go to GitHub repo")
+[![GitHub tag](https://img.shields.io/github/tag/GoodCod3/cybertron-framework?include_prereleases=&sort=semver&color=blue)](https://github.com/GoodCod3/cybertron-framework/releases/)
+[![License](https://img.shields.io/badge/License-GNU_General_Public-blue)](#license)
+
 ## Authors
 * Eduardo Martos Gómez <<emartos@natiboo.es>>
 * Jonathan Rodríguez Alejos <<jonathan.rodriguez@goodcodesolution.com>>
 
 ## Pipeline
 A pipeline refers to a series of steps (`Input`, `Transform`, `Mapper` and `Output`). Each process can have 1 or many pipelines and the orchestrator will decide how they will be executed.
 
 ## Orchestrator
 It is responsible for executing the different steps of each pipeline. The core defines different types of orchestrator that can be imported from our code to specify how the steps of each process or set of pipelines will be executed.
 
 ### We have different types of orchestrators
 #### Synchronous
 The same process can have 1 or more pipeline defined, when it is executed it will do so sequentially, executing the same step for each pipeline. That is, first it will execute the Input of all the pipelines, then the transform together with the mapper of each pipeline and finally the output of each pipeline.
 
+#### Sequence
+This orchestrator allows us to better define the sequence of a pipeline. We can execute a `Transformer` with the data returned by another transformer or even indicate several of them.
+If a transformer depends on more than 1 `Transformer` or `Input` step, then in the "transform" method we will receive a tuple with each set of data.
+It also allows us to execute all Inputs in parallel to optimize the pipeline execution speed.
+
+The way to define the pipeline for this orchestrator is as follows:
+
+```python
+from cybertron_framework.orchestrator.types.sequence import SequenceOrchestrator
+
+pipeline_steps = [
+    {"id": "input1", "type": "input", "manager": InputBigqueryManager()},
+    {"id": "input2", "type": "input", "manager": InputPostgresManager()},
+    {"id": "transformer1", "type": "transformer", "manager": TransformerBigqueryManager(), "inputs": ["input1"]},
+    {"id": "transformer2", "type": "transformer", "manager": TransformerPostgresManager(), "inputs": ["input2"]},
+    {"id": "transformer3", "type": "transformer", "manager": FinalTransformerManager(), "inputs": ["transformer1", "transformer2"]},
+    {"id": "output1", "type": "output", "manager": FirstOutputManager(), "inputs": ["transformer3"]},
+]
+
+orchestrator = SequenceOrchestrator()
+orchestrator.run(pipeline_steps)
+```
+
 ---
 
 
 ## Pipeline stages
 
 There are three different stages in the process:
```

### Comparing `cybertron_framework-0.0.1/cybertron_framework/environment/__tests__/test_environment.py` & `cybertron_framework-0.0.2/cybertron_framework/environment/__tests__/test_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 # from cybertron_framework.test_setup import *  # noqa: F401, F403
 from unittest.mock import Mock, mock_open, patch
 
 from cybertron_framework.environment.environment import Environment
 
 
 class TestEnvironmentManager(unittest.TestCase):
```

### Comparing `cybertron_framework-0.0.1/cybertron_framework/environment/__tests__/test_environment_interface.py` & `cybertron_framework-0.0.2/cybertron_framework/environment/__tests__/test_environment_interface.py`

 * *Files identical despite different names*

### Comparing `cybertron_framework-0.0.1/cybertron_framework/environment/environment.py` & `cybertron_framework-0.0.2/cybertron_framework/environment/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
 import yaml
+
 from cybertron_framework.environment.environment_interface import IEnvironment
 
 DEFAULT_VARIABLE_VALUE = None
 
 
 class Environment(IEnvironment):
     """
```

### Comparing `cybertron_framework-0.0.1/cybertron_framework/environment/environment_interface.py` & `cybertron_framework-0.0.2/cybertron_framework/environment/environment_interface.py`

 * *Files identical despite different names*

### Comparing `cybertron_framework-0.0.1/cybertron_framework/helper/__tests__/test_benchmark.py` & `cybertron_framework-0.0.2/cybertron_framework/helper/__tests__/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `cybertron_framework-0.0.1/cybertron_framework/orchestrator/__tests__/test_abstract_orchestrator.py` & `cybertron_framework-0.0.2/cybertron_framework/orchestrator/__tests__/test_abstract_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cybertron_framework-0.0.1/cybertron_framework/orchestrator/abstract_orchestrator.py` & `cybertron_framework-0.0.2/cybertron_framework/orchestrator/abstract_orchestrator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from cybertron_framework.helper.benchmark import Benchmark
 from cybertron_framework.helper.logger import Logger
 from cybertron_framework.input.input_manager_interface import IInputManager
-from cybertron_framework.orchestrator.orchestrator_interface import IOrchestrator  # noqa: E501
+from cybertron_framework.orchestrator.orchestrator_interface import (  # noqa: E501
+    IOrchestrator,
+)
 from cybertron_framework.output.output_manager_interface import IOutputManager
 from cybertron_framework.transformer.transformer_manager_interface import (
     ITransformerManager,
 )
 
 
 class AbstractOrchestrator(IOrchestrator):
```

### Comparing `cybertron_framework-0.0.1/cybertron_framework/orchestrator/orchestrator_interface.py` & `cybertron_framework-0.0.2/cybertron_framework/orchestrator/orchestrator_interface.py`

 * *Files identical despite different names*

### Comparing `cybertron_framework-0.0.1/cybertron_framework/orchestrator/types/__tests__/test_synchronous.py` & `cybertron_framework-0.0.2/cybertron_framework/orchestrator/types/__tests__/test_synchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import unittest
-# from code.test_setup import *  # noqa: F401, F403
 from unittest.mock import MagicMock
 
 from cybertron_framework.input.input_manager_interface import IInputManager
 from cybertron_framework.orchestrator.types.synchronous import Orchestrator
 from cybertron_framework.output.output_manager_interface import IOutputManager
 from cybertron_framework.transformer.transformer_manager_interface import (
     ITransformerManager,
```

### Comparing `cybertron_framework-0.0.1/cybertron_framework/orchestrator/types/synchronous.py` & `cybertron_framework-0.0.2/cybertron_framework/orchestrator/types/synchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,18 @@
             self.logger.info(
                 f"-- Transformer manager {transformer_manager_id} ({i + 1}/{len(self.transformer_manager)})."  # noqa: E501
             )
             transformer_manager = self.transformer_manager[
                 transformer_manager_id
             ]
 
-            transformed_data[transformer_manager.get_id()] = (
-                transformer_manager.transform(
-                    input_data[transformer_manager_id]
-                )
+            transformed_data[
+                transformer_manager.get_id()
+            ] = transformer_manager.transform(
+                input_data[transformer_manager_id]
             )
 
         self.elapsed_transform = self.benchmark.end("transform")
         self.logger.info("Finished the transformation process.")
 
         return transformed_data
```

### Comparing `cybertron_framework-0.0.1/cybertron_framework/output/__tests__/test_output_manager_interface.py` & `cybertron_framework-0.0.2/cybertron_framework/output/__tests__/test_output_manager_interface.py`

 * *Files identical despite different names*

### Comparing `cybertron_framework-0.0.1/cybertron_framework/transformer/__tests__/test_transformer_manager_interface.py` & `cybertron_framework-0.0.2/cybertron_framework/transformer/__tests__/test_transformer_manager_interface.py`

 * *Files identical despite different names*

### Comparing `cybertron_framework-0.0.1/pyproject.toml` & `cybertron_framework-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cybertron_framework"
-version = "0.0.1"
+version = "0.0.2"
 description = "Cybertron is a framework intended for retrieving data from one or several repositories, transforming it, and storing in output repositories"
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "cybertron_framework"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
@@ -26,8 +26,7 @@
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 79
-
```

### Comparing `cybertron_framework-0.0.1/PKG-INFO` & `cybertron_framework-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybertron_framework
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cybertron is a framework intended for retrieving data from one or several repositories, transforming it, and storing in output repositories
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,28 +15,55 @@
 Requires-Dist: pre-commit (>=3.1.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Cybertron: Transformation framework
 Cybertron is a framework intended for retrieving data from one or several repositories, transforming it, and storing in output repositories.
 For this purpose, pipelines are defined to manage the different stages of the process.
 
+[![GoodCod3 - cybertron-framework](https://img.shields.io/static/v1?label=GoodCod3&message=cybertron-framework&color=blue&logo=github)](https://github.com/GoodCod3/cybertron-framework "Go to GitHub repo")
+[![GitHub tag](https://img.shields.io/github/tag/GoodCod3/cybertron-framework?include_prereleases=&sort=semver&color=blue)](https://github.com/GoodCod3/cybertron-framework/releases/)
+[![License](https://img.shields.io/badge/License-GNU_General_Public-blue)](#license)
+
 ## Authors
 * Eduardo Martos Gómez <<emartos@natiboo.es>>
 * Jonathan Rodríguez Alejos <<jonathan.rodriguez@goodcodesolution.com>>
 
 ## Pipeline
 A pipeline refers to a series of steps (`Input`, `Transform`, `Mapper` and `Output`). Each process can have 1 or many pipelines and the orchestrator will decide how they will be executed.
 
 ## Orchestrator
 It is responsible for executing the different steps of each pipeline. The core defines different types of orchestrator that can be imported from our code to specify how the steps of each process or set of pipelines will be executed.
 
 ### We have different types of orchestrators
 #### Synchronous
 The same process can have 1 or more pipeline defined, when it is executed it will do so sequentially, executing the same step for each pipeline. That is, first it will execute the Input of all the pipelines, then the transform together with the mapper of each pipeline and finally the output of each pipeline.
 
+#### Sequence
+This orchestrator allows us to better define the sequence of a pipeline. We can execute a `Transformer` with the data returned by another transformer or even indicate several of them.
+If a transformer depends on more than 1 `Transformer` or `Input` step, then in the "transform" method we will receive a tuple with each set of data.
+It also allows us to execute all Inputs in parallel to optimize the pipeline execution speed.
+
+The way to define the pipeline for this orchestrator is as follows:
+
+```python
+from cybertron_framework.orchestrator.types.sequence import SequenceOrchestrator
+
+pipeline_steps = [
+    {"id": "input1", "type": "input", "manager": InputBigqueryManager()},
+    {"id": "input2", "type": "input", "manager": InputPostgresManager()},
+    {"id": "transformer1", "type": "transformer", "manager": TransformerBigqueryManager(), "inputs": ["input1"]},
+    {"id": "transformer2", "type": "transformer", "manager": TransformerPostgresManager(), "inputs": ["input2"]},
+    {"id": "transformer3", "type": "transformer", "manager": FinalTransformerManager(), "inputs": ["transformer1", "transformer2"]},
+    {"id": "output1", "type": "output", "manager": FirstOutputManager(), "inputs": ["transformer3"]},
+]
+
+orchestrator = SequenceOrchestrator()
+orchestrator.run(pipeline_steps)
+```
+
 ---
 
 
 ## Pipeline stages
 
 There are three different stages in the process:
```


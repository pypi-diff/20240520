# Comparing `tmp/strangeworks_optimization_models-0.1.8.tar.gz` & `tmp/strangeworks_optimization_models-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_optimization_models-0.1.8.tar", max compression
+gzip compressed data, was "strangeworks_optimization_models-0.1.9.tar", max compression
```

## Comparing `strangeworks_optimization_models-0.1.8.tar` & `strangeworks_optimization_models-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       94 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/README.md
--rw-r--r--   0        0        0      515 2023-08-28 12:49:17.239895 strangeworks_optimization_models-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/__init__.py
--rw-r--r--   0        0        0     2844 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/converter_models.py
--rw-r--r--   0        0        0    15237 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/parameter_models.py
--rw-r--r--   0        0        0    18773 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/problem_models.py
--rw-r--r--   0        0        0        0 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/py.typed
--rw-r--r--   0        0        0     3143 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/solution_models.py
--rw-r--r--   0        0        0     2669 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/solver_models.py
--rw-r--r--   0        0        0     7576 2023-08-28 12:48:58.679872 strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/strangeworks_models.py
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 strangeworks_optimization_models-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/README.md
+-rw-r--r--   0        0        0      515 2023-08-29 19:02:28.228412 strangeworks_optimization_models-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/__init__.py
+-rw-r--r--   0        0        0     2864 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/converter_models.py
+-rw-r--r--   0        0        0    15237 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/parameter_models.py
+-rw-r--r--   0        0        0    18773 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/problem_models.py
+-rw-r--r--   0        0        0        0 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/py.typed
+-rw-r--r--   0        0        0     3143 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/solution_models.py
+-rw-r--r--   0        0        0     2669 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/solver_models.py
+-rw-r--r--   0        0        0     7576 2023-08-29 19:02:14.804391 strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/strangeworks_models.py
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 strangeworks_optimization_models-0.1.9/PKG-INFO
```

### Comparing `strangeworks_optimization_models-0.1.8/pyproject.toml` & `strangeworks_optimization_models-0.1.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-optimization-models"
-version = "0.1.8"
+version = "0.1.9"
 description = "Pydantic models for strangeworks optimization SDK and application"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2"
 readme = "README.md"
 packages = [
     {include = "strangeworks_optimization_models"},
     {include = "strangeworks_optimization_models/py.typed"}
```

### Comparing `strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/converter_models.py` & `strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/converter_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,17 @@
 class StrangeworksBinaryQuadraticModelQuboDictConverter(StrangeworksConverter):
     def __init__(self, model: BinaryQuadraticModel):
         self.model = model
 
     def convert(self) -> dict:
         qubo = {}
         for lin in self.model.linear:
-            qubo[(lin, lin)] = self.model.linear[lin]
+            qubo[(str(lin), str(lin))] = self.model.linear[lin]
         for quad in self.model.quadratic:
-            qubo[(quad[0], quad[1])] = self.model.quadratic[quad]
+            qubo[(str(quad[0]), str(quad[1]))] = self.model.quadratic[quad]
         return qubo
 
 
 class StrangeworksConverterFactory:
     @staticmethod
     def from_model(model_from: Any, model_to: Any) -> StrangeworksConverter:
         if isinstance(model_from, BinaryQuadraticModel) and model_to == jm.Problem:
```

### Comparing `strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/parameter_models.py` & `strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/parameter_models.py`

 * *Files identical despite different names*

### Comparing `strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/problem_models.py` & `strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/problem_models.py`

 * *Files identical despite different names*

### Comparing `strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/solution_models.py` & `strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/solution_models.py`

 * *Files identical despite different names*

### Comparing `strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/solver_models.py` & `strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/solver_models.py`

 * *Files identical despite different names*

### Comparing `strangeworks_optimization_models-0.1.8/strangeworks_optimization_models/strangeworks_models.py` & `strangeworks_optimization_models-0.1.9/strangeworks_optimization_models/strangeworks_models.py`

 * *Files identical despite different names*

### Comparing `strangeworks_optimization_models-0.1.8/PKG-INFO` & `strangeworks_optimization_models-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-optimization-models
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pydantic models for strangeworks optimization SDK and application
 License: Apache-2
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


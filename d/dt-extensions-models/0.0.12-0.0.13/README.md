# Comparing `tmp/dt_extensions_models-0.0.12.tar.gz` & `tmp/dt_extensions_models-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt_extensions_models-0.0.12.tar", max compression
+gzip compressed data, was "dt_extensions_models-0.0.13.tar", max compression
```

## Comparing `dt_extensions_models-0.0.12.tar` & `dt_extensions_models-0.0.13.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-05-15 14:42:35.098390 dt_extensions_models-0.0.12/LICENSE
--rw-r--r--   0        0        0      564 2024-05-15 14:47:07.075159 dt_extensions_models-0.0.12/README.md
--rw-r--r--   0        0        0      286 2024-05-15 20:05:27.552330 dt_extensions_models-0.0.12/dynatrace_extension_models/__init__.py
--rw-r--r--   0        0        0     4680 2024-05-15 20:48:55.636925 dt_extensions_models-0.0.12/dynatrace_extension_models/metric_base_model.py
--rw-r--r--   0        0        0      732 2024-05-15 20:12:57.233100 dt_extensions_models-0.0.12/dynatrace_extension_models/metric_info.py
--rw-r--r--   0        0        0     8769 2024-05-15 20:16:32.381383 dt_extensions_models-0.0.12/dynatrace_extension_models/pydantic_interop.py
--rw-r--r--   0        0        0     1023 2024-05-15 20:03:29.165053 dt_extensions_models-0.0.12/pyproject.toml
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 dt_extensions_models-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 14:42:35.098390 dt_extensions_models-0.0.13/LICENSE
+-rw-r--r--   0        0        0      564 2024-05-15 14:47:07.075159 dt_extensions_models-0.0.13/README.md
+-rw-r--r--   0        0        0      286 2024-05-15 20:05:27.552330 dt_extensions_models-0.0.13/dynatrace_extension_models/__init__.py
+-rw-r--r--   0        0        0     4905 2024-05-19 23:17:58.668222 dt_extensions_models-0.0.13/dynatrace_extension_models/metric_base_model.py
+-rw-r--r--   0        0        0      732 2024-05-15 20:12:57.233100 dt_extensions_models-0.0.13/dynatrace_extension_models/metric_info.py
+-rw-r--r--   0        0        0     8769 2024-05-15 20:16:32.381383 dt_extensions_models-0.0.13/dynatrace_extension_models/pydantic_interop.py
+-rw-r--r--   0        0        0     1023 2024-05-19 23:18:08.889919 dt_extensions_models-0.0.13/pyproject.toml
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 dt_extensions_models-0.0.13/PKG-INFO
```

### Comparing `dt_extensions_models-0.0.12/LICENSE` & `dt_extensions_models-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `dt_extensions_models-0.0.12/README.md` & `dt_extensions_models-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `dt_extensions_models-0.0.12/dynatrace_extension_models/metric_base_model.py` & `dt_extensions_models-0.0.13/dynatrace_extension_models/metric_base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from datetime import datetime
 from typing import Any, Callable
 
-from dynatrace_extension import Metric
+from dynatrace_extension import Metric, MetricType
 from pydantic import BaseModel
 
 from .metric_info import MetricInfo
 
 
 def _compute_dimensions(
     dimensions_definition: Callable | list | None = None,
@@ -27,14 +28,15 @@
 
 
 def _to_metrics(
     data: Any,
     parent: BaseModel | None = None,
     metric_info: MetricInfo | None = None,
     dimensions: dict[str, str] | None = None,
+    timestamp: datetime | None = None,
 ) -> list[Metric]:
     """Turn any type of data into a list of Metric objects by traversing it recursively.
     """
     metrics: list[Metric] = []
             
     # Compute dimensions for this field
     ignore_parent_dimensions = getattr(metric_info, "ignore_parent_dimensions", False)
@@ -102,19 +104,23 @@
         else:
             value = data
 
         # If computed value is None, do not report it
         if value is None:
             return metrics
 
+        if metric_info.type == MetricType.COUNT and timestamp is None:
+            timestamp = datetime.now()
+
         metric = Metric(
             key=metric_info.key,
             value=value,
             dimensions=dimensions,
             metric_type=metric_info.type,
+            timestamp=timestamp,
         )
         metrics.append(metric)
 
     return metrics
 
 
 class MetricBaseModel(BaseModel):
```

### Comparing `dt_extensions_models-0.0.12/dynatrace_extension_models/metric_info.py` & `dt_extensions_models-0.0.13/dynatrace_extension_models/metric_info.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_models-0.0.12/dynatrace_extension_models/pydantic_interop.py` & `dt_extensions_models-0.0.13/dynatrace_extension_models/pydantic_interop.py`

 * *Files identical despite different names*

### Comparing `dt_extensions_models-0.0.12/pyproject.toml` & `dt_extensions_models-0.0.13/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 maintainers = ["Vagiz Duseev <vagiz.duseev@dynatrace.com>"]
 name = "dt-extensions-models"
 packages = [
   {include = "dynatrace_extension_models"},
 ]
 readme = "README.md"
 repository = "https://github.com/dynatrace-extensions/dt-extensions-python-models"
-version = "0.0.12"
+version = "0.0.13"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dt-extensions-sdk = "^1.1"
 pydantic = "^2.7"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `dt_extensions_models-0.0.12/PKG-INFO` & `dt_extensions_models-0.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dt-extensions-models
-Version: 0.0.12
+Version: 0.0.13
 Summary: Helper library implementing best practices for strongly typed models and reporting metrics
 Home-page: https://github.com/dynatrace-extensions/dt-extensions-models
 License: Apache-2.0
 Keywords: dynatrace,extensions
 Author: Vagiz Duseev
 Author-email: vagiz.duseev@dynatrace.com
 Maintainer: Vagiz Duseev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dt-extensions-models Version: 0.0.12 Summary:
+Metadata-Version: 2.1 Name: dt-extensions-models Version: 0.0.13 Summary:
 Helper library implementing best practices for strongly typed models and
 reporting metrics Home-page: https://github.com/dynatrace-extensions/dt-
 extensions-models License: Apache-2.0 Keywords: dynatrace,extensions Author:
 Vagiz Duseev Author-email: vagiz.duseev@dynatrace.com Maintainer: Vagiz Duseev
 Maintainer-email: vagiz.duseev@dynatrace.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```


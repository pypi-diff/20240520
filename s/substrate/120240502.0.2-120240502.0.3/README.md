# Comparing `tmp/substrate-120240502.0.2.tar.gz` & `tmp/substrate-120240502.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240502.0.2.tar", max compression
+gzip compressed data, was "substrate-120240502.0.3.tar", max compression
```

## Comparing `substrate-120240502.0.2.tar` & `substrate-120240502.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240502.0.2/LICENSE
--rw-r--r--   0        0        0     2715 2024-05-01 20:59:44.017862 substrate-120240502.0.2/README.md
--rw-r--r--   0        0        0     2079 2024-05-07 18:33:22.925402 substrate-120240502.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240502.0.2/substrate/.keep
--rw-r--r--   0        0        0       17 2024-05-02 15:36:22.000000 substrate-120240502.0.2/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2188 2024-05-02 15:36:23.000000 substrate-120240502.0.2/substrate/__init__.py
--rw-r--r--   0        0        0     5773 2024-05-06 20:31:04.737347 substrate-120240502.0.2/substrate/_client.py
--rw-r--r--   0        0        0       29 2024-05-07 18:33:22.926841 substrate-120240502.0.2/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-05-06 18:17:22.557192 substrate-120240502.0.2/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-05-06 18:17:22.556974 substrate-120240502.0.2/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-05-06 18:17:22.557750 substrate-120240502.0.2/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-05-06 18:17:22.558969 substrate-120240502.0.2/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-05-06 18:17:22.559173 substrate-120240502.0.2/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-05-06 18:17:22.559372 substrate-120240502.0.2/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-05-06 18:17:22.558706 substrate-120240502.0.2/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-05-06 18:17:22.557488 substrate-120240502.0.2/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2212 2024-05-06 18:17:22.552509 substrate-120240502.0.2/substrate/core/corenode.py
--rw-r--r--   0        0        0     1587 2024-05-06 18:17:22.557988 substrate-120240502.0.2/substrate/core/future_directive.py
--rw-r--r--   0        0        0      894 2024-05-06 18:17:22.552230 substrate-120240502.0.2/substrate/core/id_generator.py
--rw-r--r--   0        0        0    37176 2024-05-06 18:17:22.556197 substrate-120240502.0.2/substrate/core/models.py
--rw-r--r--   0        0        0     3798 2024-05-06 18:17:22.551865 substrate-120240502.0.2/substrate/core/sb.py
--rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240502.0.2/substrate/dataclass_models.py
--rw-r--r--   0        0        0    47757 2024-05-02 15:36:20.000000 substrate-120240502.0.2/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    42949 2024-05-02 15:36:23.000000 substrate-120240502.0.2/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240502.0.2/substrate/py.typed
--rw-r--r--   0        0        0     2196 2024-05-06 18:16:14.492293 substrate-120240502.0.2/substrate/substrate.py
--rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-120240502.0.2/substrate/substrate_response.py
--rw-r--r--   0        0        0    37584 2024-05-02 15:36:18.000000 substrate-120240502.0.2/substrate/typeddict_models.py
--rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-120240502.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-01 19:52:58.550017 substrate-120240502.0.3/LICENSE
+-rw-r--r--   0        0        0     2715 2024-05-07 14:55:29.245125 substrate-120240502.0.3/README.md
+-rw-r--r--   0        0        0     2079 2024-05-20 15:26:28.899939 substrate-120240502.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 17:39:17.445476 substrate-120240502.0.3/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-05-07 14:55:29.246970 substrate-120240502.0.3/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2188 2024-05-07 14:55:29.247076 substrate-120240502.0.3/substrate/__init__.py
+-rw-r--r--   0        0        0     5885 2024-05-20 15:23:21.502856 substrate-120240502.0.3/substrate/_client.py
+-rw-r--r--   0        0        0       29 2024-05-20 15:26:28.900395 substrate-120240502.0.3/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-01 19:52:58.552158 substrate-120240502.0.3/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-01 19:52:58.552245 substrate-120240502.0.3/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-04-17 17:39:17.446324 substrate-120240502.0.3/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:52:58.552427 substrate-120240502.0.3/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-01 19:52:58.552528 substrate-120240502.0.3/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-04-17 17:39:17.446448 substrate-120240502.0.3/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-01 19:52:58.552701 substrate-120240502.0.3/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-01 19:52:58.552792 substrate-120240502.0.3/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2212 2024-05-07 14:55:29.247367 substrate-120240502.0.3/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1587 2024-05-07 14:55:29.247795 substrate-120240502.0.3/substrate/core/future_directive.py
+-rw-r--r--   0        0        0     1095 2024-05-20 15:23:21.503310 substrate-120240502.0.3/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    37176 2024-05-07 14:55:29.248214 substrate-120240502.0.3/substrate/core/models.py
+-rw-r--r--   0        0        0     3798 2024-05-07 14:55:29.248358 substrate-120240502.0.3/substrate/core/sb.py
+-rw-r--r--   0        0        0    32553 2024-04-19 22:14:10.804912 substrate-120240502.0.3/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    47757 2024-05-07 14:55:29.248641 substrate-120240502.0.3/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    42949 2024-05-07 14:55:29.248958 substrate-120240502.0.3/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:52:58.553826 substrate-120240502.0.3/substrate/py.typed
+-rw-r--r--   0        0        0     2196 2024-05-20 14:53:03.816270 substrate-120240502.0.3/substrate/substrate.py
+-rw-r--r--   0        0        0     1015 2024-05-07 14:55:29.249194 substrate-120240502.0.3/substrate/substrate_response.py
+-rw-r--r--   0        0        0    37584 2024-05-07 14:55:29.249408 substrate-120240502.0.3/substrate/typeddict_models.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-120240502.0.3/PKG-INFO
```

### Comparing `substrate-120240502.0.2/LICENSE` & `substrate-120240502.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/README.md` & `substrate-120240502.0.3/README.md`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/pyproject.toml` & `substrate-120240502.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240502.0.2"
+version = "120240502.0.3"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240502.0.2/substrate/__init__.py` & `substrate-120240502.0.3/substrate/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/_client.py` & `substrate-120240502.0.3/substrate/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import platform
 from typing import Any, Dict, Union, Optional
 from typing_extensions import Literal
+from .core.id_generator import IDGenerator
 
 import httpx
 import distro
 
 from ._version import __version__
 
 log: logging.Logger = logging.getLogger(__name__)
@@ -165,14 +166,15 @@
     @property
     def default_headers(self) -> Dict[str, str]:
         return {
             "Accept": "application/json",
             "Content-Type": "application/json",
             "User-Agent": self.user_agent,
             "X-Substrate-Backend": self._backend,
+            "X-Substrate-Request-Id": IDGenerator.random_string(32),
             **self.platform_headers,
             **self.auth_headers,
             **self._additional_headers,
         }
 
     def post_compose(self, dag: Dict[str, Any]) -> APIResponse:
         url = f"{self._base_url}/compose"
```

### Comparing `substrate-120240502.0.2/substrate/core/base_future.py` & `substrate-120240502.0.3/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/core/client/find_futures_client.py` & `substrate-120240502.0.3/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/core/client/future.py` & `substrate-120240502.0.3/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/core/client/graph.py` & `substrate-120240502.0.3/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/core/coregraph.py` & `substrate-120240502.0.3/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/core/corenode.py` & `substrate-120240502.0.3/substrate/core/corenode.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/core/future_directive.py` & `substrate-120240502.0.3/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/core/id_generator.py` & `substrate-120240502.0.3/substrate/core/id_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,31 @@
 from threading import Lock
 
 
 class IDGenerator:
     _generators: Dict[str, "IDGenerator"] = {}
     _lock = Lock()
 
-    def __init__(self, prefix: str):
+    def __init__(self, prefix: str, length: int = 8):
         self.prefix = prefix
         self.n = 1
+        self.length = length
 
     def get_next_id(self):
         with IDGenerator._lock:
-            alphabet = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_-"
-            random_string = "".join(random.choices(alphabet, k=8))
+            random_string = IDGenerator.random_string(self.length)
             next_id = f"{self.prefix}{self.n}_{random_string}"
             self.n += 1
             return next_id
 
     @staticmethod
+    def random_string(length: int) -> str:
+        alphabet = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_-"
+        random_string = "".join(random.choices(alphabet, k=length))
+        return random_string
+
+    @staticmethod
     def get_instance(class_name: str) -> "IDGenerator":
         with IDGenerator._lock:
             if class_name not in IDGenerator._generators:
                 IDGenerator._generators[class_name] = IDGenerator(class_name)
             return IDGenerator._generators[class_name]
```

### Comparing `substrate-120240502.0.2/substrate/core/models.py` & `substrate-120240502.0.3/substrate/core/models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/core/sb.py` & `substrate-120240502.0.3/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/dataclass_models.py` & `substrate-120240502.0.3/substrate/dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/future_dataclass_models.py` & `substrate-120240502.0.3/substrate/future_dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/nodes.py` & `substrate-120240502.0.3/substrate/nodes.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/substrate.py` & `substrate-120240502.0.3/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/substrate_response.py` & `substrate-120240502.0.3/substrate/substrate_response.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/substrate/typeddict_models.py` & `substrate-120240502.0.3/substrate/typeddict_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.2/PKG-INFO` & `substrate-120240502.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240502.0.2
+Version: 120240502.0.3
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


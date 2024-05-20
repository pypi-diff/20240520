# Comparing `tmp/datamaxi-0.2.0.tar.gz` & `tmp/datamaxi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaxi-0.2.0.tar", last modified: Wed May  8 07:44:30 2024, max compression
+gzip compressed data, was "datamaxi-0.3.0.tar", last modified: Mon May 20 02:53:40 2024, max compression
```

## Comparing `datamaxi-0.2.0.tar` & `datamaxi-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.348146 datamaxi-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 07:44:24.000000 datamaxi-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 07:44:24.000000 datamaxi-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-08 07:44:30.348146 datamaxi-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-08 07:44:24.000000 datamaxi-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/binance/
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/binance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/bithumb/
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/bithumb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/bybit/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/bybit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/coinone/
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/coinone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/defillama/
--rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/defillama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/google/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/huobi/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/huobi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/naver/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/naver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/okx/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/okx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/datamaxi/upbit/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 07:44:24.000000 datamaxi-0.2.0/datamaxi/upbit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.348146 datamaxi-0.2.0/datamaxi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 07:44:30.000000 datamaxi-0.2.0/datamaxi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-08 07:44:24.000000 datamaxi-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.344146 datamaxi-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 07:44:24.000000 datamaxi-0.2.0/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 07:44:30.348146 datamaxi-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:30.348146 datamaxi-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-08 07:44:24.000000 datamaxi-0.2.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.609599 datamaxi-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 02:53:36.000000 datamaxi-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 02:53:36.000000 datamaxi-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-20 02:53:40.609599 datamaxi-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-20 02:53:36.000000 datamaxi-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.601599 datamaxi-0.3.0/datamaxi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/binance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/binance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/bithumb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/bithumb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/bybit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/bybit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/coinone/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/coinone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/defillama/
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/defillama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/google/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/huobi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/huobi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/naver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/naver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/okx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/okx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi/upbit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 02:53:36.000000 datamaxi-0.3.0/datamaxi/upbit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/datamaxi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-20 02:53:40.000000 datamaxi-0.3.0/datamaxi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-20 02:53:40.000000 datamaxi-0.3.0/datamaxi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:53:40.000000 datamaxi-0.3.0/datamaxi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 02:53:40.000000 datamaxi-0.3.0/datamaxi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 02:53:40.000000 datamaxi-0.3.0/datamaxi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-20 02:53:36.000000 datamaxi-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 02:53:36.000000 datamaxi-0.3.0/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-20 02:53:40.609599 datamaxi-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:53:40.605599 datamaxi-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-20 02:53:36.000000 datamaxi-0.3.0/tests/test_api.py
```

### Comparing `datamaxi-0.2.0/LICENSE` & `datamaxi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/PKG-INFO` & `datamaxi-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaxi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Official Python client for DataMaxi+ API
 Author-email: Bisonai <business@bisonai.com>
 Project-URL: Homepage, https://github.com/bisonai/datamaxi-python
 Project-URL: Issues, https://github.com/bisonai/datamaxi-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaxi-0.2.0/README.md` & `datamaxi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi/api.py` & `datamaxi-0.3.0/datamaxi/api.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi/binance/__init__.py` & `datamaxi-0.3.0/datamaxi/binance/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi/bithumb/__init__.py` & `datamaxi-0.3.0/datamaxi/bithumb/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi/bybit/__init__.py` & `datamaxi-0.3.0/datamaxi/bybit/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi/coinone/__init__.py` & `datamaxi-0.3.0/datamaxi/coinone/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi/error.py` & `datamaxi-0.3.0/datamaxi/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,7 +24,12 @@
 
 class ParameterRequiredError(Error):
     def __init__(self, params):
         self.params = params
 
     def __str__(self):
         return "%s is mandatory, but received empty." % (", ".join(self.params))
+
+
+class AtLeastOneParameterRequiredError(Error):
+    def __str__(self):
+        return "At least one parameter is required."
```

### Comparing `datamaxi-0.2.0/datamaxi/google/__init__.py` & `datamaxi-0.3.0/datamaxi/google/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
         Args:
             api_key (str): The DataMaxi+ API key
             **kwargs: Keyword arguments used by `datamaxi.api.API`.
         """
         if "base_url" not in kwargs:
             kwargs["base_url"] = BASE_URL
-            super().__init__(api_key, **kwargs)
+        super().__init__(api_key, **kwargs)
 
     def keywords(self) -> List[str]:
         """Get Google trend supported keywords
 
         `GET /v1/google/keywords`
 
         <https://docs.datamaxi.finance/google/keywords>
```

### Comparing `datamaxi-0.2.0/datamaxi/huobi/__init__.py` & `datamaxi-0.3.0/datamaxi/huobi/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi/lib/utils.py` & `datamaxi-0.3.0/datamaxi/lib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List
 from urllib.parse import urlencode
 import pandas as pd
 from functools import wraps
 from datamaxi.error import ParameterRequiredError
+from datamaxi.error import AtLeastOneParameterRequiredError
 
 
 def to_float(x):
     return float(x)
 
 
 def to_int(x):
@@ -34,14 +35,28 @@
     ]
 
     """
     for p in params:
         check_required_parameter(p[0], p[1])
 
 
+def check_at_least_one_set_parameters(params):
+    at_least_one_set = False
+    for p in params:
+        try:
+            check_required_parameter(p[0], p[1])
+            at_least_one_set = True
+            break
+        except:  # noqa: E722
+            pass
+
+    if not at_least_one_set:
+        raise AtLeastOneParameterRequiredError()
+
+
 def check_required_parameter_list(values: List, name: str):
     if len(values) == 0:
         raise ParameterRequiredError([name])
 
     for value in values:
         check_required_parameter(value, name)
```

### Comparing `datamaxi-0.2.0/datamaxi/naver/__init__.py` & `datamaxi-0.3.0/datamaxi/naver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
         Args:
             api_key (str): The DataMaxi+ API key
             **kwargs: Keyword arguments used by `datamaxi.api.API`.
         """
         if "base_url" not in kwargs:
             kwargs["base_url"] = BASE_URL
-            super().__init__(api_key, **kwargs)
+        super().__init__(api_key, **kwargs)
 
     def keywords(self) -> List[str]:
         """Get Naver trend supported keywords
 
         `GET /v1/naver/keywords`
 
         <https://docs.datamaxi.finance/naver/keywords>
```

### Comparing `datamaxi-0.2.0/datamaxi/okx/__init__.py` & `datamaxi-0.3.0/datamaxi/okx/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi/upbit/__init__.py` & `datamaxi-0.3.0/datamaxi/upbit/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/datamaxi.egg-info/PKG-INFO` & `datamaxi-0.3.0/datamaxi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaxi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Official Python client for DataMaxi+ API
 Author-email: Bisonai <business@bisonai.com>
 Project-URL: Homepage, https://github.com/bisonai/datamaxi-python
 Project-URL: Issues, https://github.com/bisonai/datamaxi-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaxi-0.2.0/datamaxi.egg-info/SOURCES.txt` & `datamaxi-0.3.0/datamaxi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datamaxi-0.2.0/pyproject.toml` & `datamaxi-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datamaxi"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Bisonai", email="business@bisonai.com" },
 ]
 description = "Official Python client for DataMaxi+ API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `datamaxi-0.2.0/tests/test_api.py` & `datamaxi-0.3.0/tests/test_api.py`

 * *Files identical despite different names*


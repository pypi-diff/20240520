# Comparing `tmp/pypomes_core-1.0.4.tar.gz` & `tmp/pypomes_core-1.0.5.tar.gz`

## Comparing `pypomes_core-1.0.4.tar` & `pypomes_core-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24661 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24661 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.5/PKG-INFO
```

### Comparing `pypomes_core-1.0.4/src/pypomes_core/.ruff.toml` & `pypomes_core-1.0.5/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/__init__.py` & `pypomes_core-1.0.5/src/pypomes_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     APP_PREFIX,
     env_get_str, env_get_int, env_get_bool, env_get_float, env_get_path,
 )
 from .exception_pomes import (
     exc_format,
 )
 from .file_pomes import (
-    TEMP_DIR,
+    TEMP_FOLDER,
     file_from_request, file_get_data
 )
 from .json_pomes import (
     json_normalize_dict, json_normalize_iterable,
 )
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
@@ -70,15 +70,15 @@
     "encode_ascii_hex", "decode_ascii_hex",
     # env_pomes
     "APP_PREFIX",
     "env_get_str", "env_get_int", "env_get_bool", "env_get_float", "env_get_path",
     # exception_pomes
     "exc_format",
     # file_pomes
-    "TEMP_DIR",
+    "TEMP_FOLDER",
     "file_from_request", "file_get_data",
     # json_pomes
     "json_normalize_dict", "json_normalize_iterable",
     # list_pomes
     "list_compare", "list_flatten", "list_unflatten",
     "list_find_coupled", "list_elem_starting_with", "list_transform",
     # str_pomes
```

### Comparing `pypomes_core-1.0.4/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/email_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/env_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/file_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/file_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Final
 from werkzeug.datastructures import FileStorage
 
 from .env_pomes import APP_PREFIX, env_get_path
 
-TEMP_DIR: Final[Path] = env_get_path(f"{APP_PREFIX}_TEMP_DIR", Path(gettempdir()))
+TEMP_FOLDER: Final[Path] = env_get_path(f"{APP_PREFIX}_TEMP_FOLDER", Path(gettempdir()))
 
 
 def file_from_request(request: Request,
                       file_name: str = None,
                       file_seq: int = 0) -> bytes:
     """
     Retrieve and return the contents of the file returned in the response to a request.
```

### Comparing `pypomes_core-1.0.4/src/pypomes_core/json_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/list_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/str_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.0.5/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.0.5/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/LICENSE` & `pypomes_core-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.4/pyproject.toml` & `pypomes_core-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.0.4/PKG-INFO` & `pypomes_core-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


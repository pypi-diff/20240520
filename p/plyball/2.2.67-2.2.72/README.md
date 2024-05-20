# Comparing `tmp/plyball-2.2.67.tar.gz` & `tmp/plyball-2.2.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyball-2.2.67.tar", max compression
+gzip compressed data, was "plyball-2.2.72.tar", max compression
```

## Comparing `plyball-2.2.67.tar` & `plyball-2.2.72.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1076 2024-05-20 15:10:28.732353 plyball-2.2.67/LICENSE.txt
--rw-r--r--   0        0        0      819 2024-05-20 15:10:28.732353 plyball-2.2.67/README.md
--rw-r--r--   0        0        0       22 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/__init__.py
--rw-r--r--   0        0        0       48 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/baseballreference/__init__.py
--rw-r--r--   0        0        0     9610 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/baseballreference/baseballreference.py
--rw-r--r--   0        0        0       33 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/fangraphs/__init__.py
--rw-r--r--   0        0        0    15578 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/fangraphs/fangraphs.py
--rw-r--r--   0        0        0       26 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/lahman/__init__.py
--rw-r--r--   0        0        0    10203 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/lahman/lahman.py
--rw-r--r--   0        0        0     6013 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/mlb/__init__.py
--rw-r--r--   0        0        0       28 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/ottoneu/__init__.py
--rw-r--r--   0        0        0    13950 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/ottoneu/ottoneu.py
--rw-r--r--   0        0        0        0 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/pipeline/__init__.py
--rw-r--r--   0        0        0     3019 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/pipeline/evaluation.py
--rw-r--r--   0        0        0     3517 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/player_id_lookup.py
--rw-r--r--   0        0        0      268 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/player_map.py
--rw-r--r--   0        0        0       35 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/retrosheet/__init__.py
--rw-r--r--   0        0        0     8085 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/retrosheet/retrosheet.py
--rw-r--r--   0        0        0       30 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/statcast/__init__.py
--rw-r--r--   0        0        0    14792 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/statcast/statcast.py
--rw-r--r--   0        0        0     4433 2024-05-20 15:10:28.732353 plyball-2.2.67/plyball/utils.py
--rw-r--r--   0        0        0     2875 2024-05-20 15:10:28.736353 plyball-2.2.67/pyproject.toml
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 plyball-2.2.67/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-20 15:24:21.366633 plyball-2.2.72/LICENSE.txt
+-rw-r--r--   0        0        0      819 2024-05-20 15:24:21.366633 plyball-2.2.72/README.md
+-rw-r--r--   0        0        0       22 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/baseballreference/__init__.py
+-rw-r--r--   0        0        0     9610 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/baseballreference/baseballreference.py
+-rw-r--r--   0        0        0       33 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/fangraphs/__init__.py
+-rw-r--r--   0        0        0    15578 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/fangraphs/fangraphs.py
+-rw-r--r--   0        0        0       26 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/lahman/__init__.py
+-rw-r--r--   0        0        0    10203 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/lahman/lahman.py
+-rw-r--r--   0        0        0     6013 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/mlb/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/ottoneu/__init__.py
+-rw-r--r--   0        0        0    13950 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/ottoneu/ottoneu.py
+-rw-r--r--   0        0        0        0 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/pipeline/__init__.py
+-rw-r--r--   0        0        0     3019 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/pipeline/evaluation.py
+-rw-r--r--   0        0        0     3517 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/player_id_lookup.py
+-rw-r--r--   0        0        0      268 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/player_map.py
+-rw-r--r--   0        0        0       35 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/retrosheet/__init__.py
+-rw-r--r--   0        0        0     8085 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/retrosheet/retrosheet.py
+-rw-r--r--   0        0        0       30 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/statcast/__init__.py
+-rw-r--r--   0        0        0    14792 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/statcast/statcast.py
+-rw-r--r--   0        0        0     4433 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/utils.py
+-rw-r--r--   0        0        0     2907 2024-05-20 15:24:31.946653 plyball-2.2.72/pyproject.toml
+-rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 plyball-2.2.72/PKG-INFO
```

### Comparing `plyball-2.2.67/LICENSE.txt` & `plyball-2.2.72/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/README.md` & `plyball-2.2.72/README.md`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/baseballreference/baseballreference.py` & `plyball-2.2.72/plyball/baseballreference/baseballreference.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/fangraphs/fangraphs.py` & `plyball-2.2.72/plyball/fangraphs/fangraphs.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/lahman/lahman.py` & `plyball-2.2.72/plyball/lahman/lahman.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/mlb/__init__.py` & `plyball-2.2.72/plyball/mlb/__init__.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/ottoneu/ottoneu.py` & `plyball-2.2.72/plyball/ottoneu/ottoneu.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/pipeline/evaluation.py` & `plyball-2.2.72/plyball/pipeline/evaluation.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/player_id_lookup.py` & `plyball-2.2.72/plyball/player_id_lookup.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/retrosheet/retrosheet.py` & `plyball-2.2.72/plyball/retrosheet/retrosheet.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/statcast/statcast.py` & `plyball-2.2.72/plyball/statcast/statcast.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/plyball/utils.py` & `plyball-2.2.72/plyball/utils.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.67/pyproject.toml` & `plyball-2.2.72/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plyball"
-version = "2.2.67"
+version = "2.2.72"
 description = ""
 authors = ["W. Aaron Morris <waaronmorris@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 alabaster = "0.7.13"
@@ -56,17 +56,19 @@
 commitizen = "^3.26.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
+version_toml = [
+    "pyproject.toml:tool.poetry.version",
+]
 version_variable = [
     "plyball/__init__.py:__version__",
-    "pyproject.toml:version"
 ]
 assets = []
 build_command_env = []
 commit_message = "chore(release): release  {version}\n\nAutomatically generated by python-semantic-release"
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
```

### Comparing `plyball-2.2.67/PKG-INFO` & `plyball-2.2.72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plyball
-Version: 2.2.67
+Version: 2.2.72
 Summary: 
 Author: W. Aaron Morris
 Author-email: waaronmorris@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


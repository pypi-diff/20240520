# Comparing `tmp/digitalhub-0.4.0b8.tar.gz` & `tmp/digitalhub-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-0.4.0b8.tar", last modified: Tue May 14 09:32:59 2024, max compression
+gzip compressed data, was "digitalhub-0.5.0b0.tar", last modified: Mon May 20 12:46:19 2024, max compression
```

## Comparing `digitalhub-0.4.0b8.tar` & `digitalhub-0.5.0b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 09:32:59.421637 digitalhub-0.4.0b8/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.4.0b8/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-05-14 09:32:59.421637 digitalhub-0.4.0b8/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.4.0b8/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 09:32:59.413637 digitalhub-0.4.0b8/digitalhub/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2218 2024-05-13 12:39:44.000000 digitalhub-0.4.0b8/digitalhub/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 09:32:59.417637 digitalhub-0.4.0b8/digitalhub.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      166 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1547 2024-05-13 12:41:00.000000 digitalhub-0.4.0b8/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-14 09:32:59.421637 digitalhub-0.4.0b8/setup.cfg
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 09:32:59.417637 digitalhub-0.4.0b8/test/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_artifacts.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_dataitems.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_functions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_runs.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_tasks.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.4.0b8/test/test_imports.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.4.0b8/test/testkfp.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.4.0b8/test/testkfp_pipeline.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:46:19.279416 digitalhub-0.5.0b0/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.5.0b0/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-05-20 12:46:19.279416 digitalhub-0.5.0b0/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.5.0b0/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:46:19.271416 digitalhub-0.5.0b0/digitalhub/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2218 2024-05-20 09:51:09.000000 digitalhub-0.5.0b0/digitalhub/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:46:19.275416 digitalhub-0.5.0b0/digitalhub.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-05-20 12:46:19.000000 digitalhub-0.5.0b0/digitalhub.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-05-20 12:46:19.000000 digitalhub-0.5.0b0/digitalhub.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-20 12:46:19.000000 digitalhub-0.5.0b0/digitalhub.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      166 2024-05-20 12:46:19.000000 digitalhub-0.5.0b0/digitalhub.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-05-20 12:46:19.000000 digitalhub-0.5.0b0/digitalhub.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1547 2024-05-20 07:16:51.000000 digitalhub-0.5.0b0/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-20 12:46:19.279416 digitalhub-0.5.0b0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:46:19.275416 digitalhub-0.5.0b0/test/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-05-09 07:33:31.000000 digitalhub-0.5.0b0/test/test_crud_artifacts.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-05-09 07:33:31.000000 digitalhub-0.5.0b0/test/test_crud_dataitems.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-05-09 07:33:31.000000 digitalhub-0.5.0b0/test/test_crud_functions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-05-09 07:33:31.000000 digitalhub-0.5.0b0/test/test_crud_runs.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-05-09 07:33:31.000000 digitalhub-0.5.0b0/test/test_crud_tasks.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.5.0b0/test/test_imports.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.5.0b0/test/testkfp.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.5.0b0/test/testkfp_pipeline.py
```

### Comparing `digitalhub-0.4.0b8/LICENSE.txt` & `digitalhub-0.5.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/PKG-INFO` & `digitalhub-0.5.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.4.0b8
+Version: 0.5.0b0
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,25 +224,25 @@
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: digitalhub-core~=0.3
+Requires-Dist: digitalhub-core~=0.5
 Provides-Extra: all
-Requires-Dist: digitalhub-data~=0.3; extra == "all"
-Requires-Dist: digitalhub-ml~=0.3; extra == "all"
-Requires-Dist: digitalhub-ai~=0.3; extra == "all"
+Requires-Dist: digitalhub-data~=0.5; extra == "all"
+Requires-Dist: digitalhub-ml~=0.5; extra == "all"
+Requires-Dist: digitalhub-ai~=0.5; extra == "all"
 Provides-Extra: ml
-Requires-Dist: digitalhub-ml~=0.3; extra == "ml"
+Requires-Dist: digitalhub-ml~=0.5; extra == "ml"
 Provides-Extra: ai
-Requires-Dist: digitalhub-ai~=0.3; extra == "ai"
+Requires-Dist: digitalhub-ai~=0.5; extra == "ai"
 Provides-Extra: data
-Requires-Dist: digitalhub-data~=0.3; extra == "data"
+Requires-Dist: digitalhub-data~=0.5; extra == "data"
 
 # Digitalhub Library
 
 The Digitalhub SDK library is used to manage entities and executions in Digitalhub from Python.
 It comes with a suite of tools to help you manage your projects and executions. It exposes CRUD methods to create, read, update and delete entities, and objects methods to excute functions or workflows, collect or store execution results and data.
 
 A more detailed description of the library can be found in the [official documentation](https://scc-digitalhub.github.io/docs/) of Digitalhub.
```

### Comparing `digitalhub-0.4.0b8/digitalhub/__init__.py` & `digitalhub-0.5.0b0/digitalhub/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/digitalhub.egg-info/PKG-INFO` & `digitalhub-0.5.0b0/digitalhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.4.0b8
+Version: 0.5.0b0
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,25 +224,25 @@
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: digitalhub-core~=0.3
+Requires-Dist: digitalhub-core~=0.5
 Provides-Extra: all
-Requires-Dist: digitalhub-data~=0.3; extra == "all"
-Requires-Dist: digitalhub-ml~=0.3; extra == "all"
-Requires-Dist: digitalhub-ai~=0.3; extra == "all"
+Requires-Dist: digitalhub-data~=0.5; extra == "all"
+Requires-Dist: digitalhub-ml~=0.5; extra == "all"
+Requires-Dist: digitalhub-ai~=0.5; extra == "all"
 Provides-Extra: ml
-Requires-Dist: digitalhub-ml~=0.3; extra == "ml"
+Requires-Dist: digitalhub-ml~=0.5; extra == "ml"
 Provides-Extra: ai
-Requires-Dist: digitalhub-ai~=0.3; extra == "ai"
+Requires-Dist: digitalhub-ai~=0.5; extra == "ai"
 Provides-Extra: data
-Requires-Dist: digitalhub-data~=0.3; extra == "data"
+Requires-Dist: digitalhub-data~=0.5; extra == "data"
 
 # Digitalhub Library
 
 The Digitalhub SDK library is used to manage entities and executions in Digitalhub from Python.
 It comes with a suite of tools to help you manage your projects and executions. It exposes CRUD methods to create, read, update and delete entities, and objects methods to excute functions or workflows, collect or store execution results and data.
 
 A more detailed description of the library can be found in the [official documentation](https://scc-digitalhub.github.io/docs/) of Digitalhub.
```

### Comparing `digitalhub-0.4.0b8/pyproject.toml` & `digitalhub-0.5.0b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub"
-version = "0.4.0b8"
+version = "0.5.0b0"
 description = "Python SDK for DigitalHub"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -16,26 +16,26 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["data", "dataops", "kubernetes"]
 requires-python = ">=3.9"
 dependencies = [
-"digitalhub-core~=0.3",
+"digitalhub-core~=0.5",
 ]
 
 [project.optional-dependencies]
 all = [
-    "digitalhub-data~=0.3",
-    "digitalhub-ml~=0.3",
-    "digitalhub-ai~=0.3",
+    "digitalhub-data~=0.5",
+    "digitalhub-ml~=0.5",
+    "digitalhub-ai~=0.5",
 ]
-ml = ["digitalhub-ml~=0.3"]
-ai = ["digitalhub-ai~=0.3"]
-data = ["digitalhub-data~=0.3"]
+ml = ["digitalhub-ml~=0.5"]
+ai = ["digitalhub-ai~=0.5"]
+data = ["digitalhub-data~=0.5"]
 
 [project.urls]
 Homepage = "https://github.com/scc-digitalhub/digitalhub-sdk"
 
 [tool.setuptools.packages.find]
 exclude = ["ai*", "wrapper*", "ml*", "core*", "data*"]
 
@@ -48,15 +48,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.4.0b8"
+current_version = "0.5.0b0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digitalhub-0.4.0b8/test/test_crud_artifacts.py` & `digitalhub-0.5.0b0/test/test_crud_artifacts.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/test/test_crud_dataitems.py` & `digitalhub-0.5.0b0/test/test_crud_dataitems.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/test/test_crud_functions.py` & `digitalhub-0.5.0b0/test/test_crud_functions.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/test/test_crud_runs.py` & `digitalhub-0.5.0b0/test/test_crud_runs.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/test/test_crud_tasks.py` & `digitalhub-0.5.0b0/test/test_crud_tasks.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/test/test_imports.py` & `digitalhub-0.5.0b0/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/test/testkfp.py` & `digitalhub-0.5.0b0/test/testkfp.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b8/test/testkfp_pipeline.py` & `digitalhub-0.5.0b0/test/testkfp_pipeline.py`

 * *Files identical despite different names*


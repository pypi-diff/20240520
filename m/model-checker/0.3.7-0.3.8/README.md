# Comparing `tmp/model_checker-0.3.7.tar.gz` & `tmp/model_checker-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.3.7.tar", last modified: Mon May 20 21:27:12 2024, max compression
+gzip compressed data, was "model_checker-0.3.8.tar", last modified: Mon May 20 21:30:42 2024, max compression
```

## Comparing `model_checker-0.3.7.tar` & `model_checker-0.3.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.7/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:27:12.396851 model_checker-0.3.7/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     5437 2024-05-20 20:33:25.000000 model_checker-0.3.7/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)      937 2024-05-20 21:26:50.000000 model_checker-0.3.7/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-20 21:27:12.396851 model_checker-0.3.7/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/src/
--rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:07.000000 model_checker-0.3.7/src/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    10262 2024-05-20 21:23:26.000000 model_checker-0.3.7/src/__main__.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      482 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       52 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       26 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/src/modules/
--rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:54.000000 model_checker-0.3.7/src/modules/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19988 2024-05-20 20:33:25.000000 model_checker-0.3.7/src/modules/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    23975 2024-05-20 21:23:26.000000 model_checker-0.3.7/src/modules/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.7/src/modules/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.7/src/modules/syntax.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/test/
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.7/test/test.py
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.7/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.223677 model_checker-0.3.8/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.8/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:30:42.223677 model_checker-0.3.8/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     5437 2024-05-20 20:33:25.000000 model_checker-0.3.8/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)      933 2024-05-20 21:30:32.000000 model_checker-0.3.8/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-20 21:30:42.223677 model_checker-0.3.8/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.222677 model_checker-0.3.8/src/
+-rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:07.000000 model_checker-0.3.8/src/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    10262 2024-05-20 21:23:26.000000 model_checker-0.3.8/src/__main__.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.223677 model_checker-0.3.8/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      482 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       48 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       26 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.223677 model_checker-0.3.8/src/modules/
+-rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:54.000000 model_checker-0.3.8/src/modules/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19988 2024-05-20 20:33:25.000000 model_checker-0.3.8/src/modules/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    23975 2024-05-20 21:23:26.000000 model_checker-0.3.8/src/modules/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.8/src/modules/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.8/src/modules/syntax.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.223677 model_checker-0.3.8/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.8/test/test.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.8/test/test_examples.py
```

### Comparing `model_checker-0.3.7/LICENCE` & `model_checker-0.3.8/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.7/PKG-INFO` & `model_checker-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.7
+Version: 0.3.8
 Summary: A hyperintensional theorem prover for counterfactual conditionals and modal operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.3.7/README.md` & `model_checker-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.7/pyproject.toml` & `model_checker-0.3.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.3.7"
+version = "0.3.8"
 description = "A hyperintensional theorem prover for counterfactual conditionals and modal operators."
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
@@ -23,8 +23,8 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/benbrastmckie/ModelChecker"
 Issues = "https://github.com/benbrastmckie/ModelChecker/issues"
 
 [project.scripts]
-model-checker = "src.__main__:main"
+model-checker = "__main__:main"
```

### Comparing `model_checker-0.3.7/src/__main__.py` & `model_checker-0.3.8/src/__main__.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.7/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.3.8/src/model_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.7
+Version: 0.3.8
 Summary: A hyperintensional theorem prover for counterfactual conditionals and modal operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.3.7/src/modules/model_definitions.py` & `model_checker-0.3.8/src/modules/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.7/src/modules/model_structure.py` & `model_checker-0.3.8/src/modules/model_structure.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.7/src/modules/semantics.py` & `model_checker-0.3.8/src/modules/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.7/src/modules/syntax.py` & `model_checker-0.3.8/src/modules/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.7/test/test.py` & `model_checker-0.3.8/test/test.py`

 * *Files identical despite different names*


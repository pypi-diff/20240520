# Comparing `tmp/model_checker-0.3.8.tar.gz` & `tmp/model_checker-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.3.8.tar", last modified: Mon May 20 21:30:42 2024, max compression
+gzip compressed data, was "model_checker-0.3.9.tar", last modified: Mon May 20 21:36:04 2024, max compression
```

## Comparing `model_checker-0.3.8.tar` & `model_checker-0.3.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.223677 model_checker-0.3.8/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.8/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:30:42.223677 model_checker-0.3.8/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     5437 2024-05-20 20:33:25.000000 model_checker-0.3.8/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)      933 2024-05-20 21:30:32.000000 model_checker-0.3.8/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-20 21:30:42.223677 model_checker-0.3.8/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.222677 model_checker-0.3.8/src/
--rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:07.000000 model_checker-0.3.8/src/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    10262 2024-05-20 21:23:26.000000 model_checker-0.3.8/src/__main__.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.223677 model_checker-0.3.8/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      482 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       48 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       26 2024-05-20 21:30:42.000000 model_checker-0.3.8/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.223677 model_checker-0.3.8/src/modules/
--rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:54.000000 model_checker-0.3.8/src/modules/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19988 2024-05-20 20:33:25.000000 model_checker-0.3.8/src/modules/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    23975 2024-05-20 21:23:26.000000 model_checker-0.3.8/src/modules/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.8/src/modules/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.8/src/modules/syntax.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:30:42.223677 model_checker-0.3.8/test/
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.8/test/test.py
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.8/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.365435 model_checker-0.3.9/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.9/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:36:04.365435 model_checker-0.3.9/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     5437 2024-05-20 20:33:25.000000 model_checker-0.3.9/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)      947 2024-05-20 21:33:49.000000 model_checker-0.3.9/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-20 21:36:04.365435 model_checker-0.3.9/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.364435 model_checker-0.3.9/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.365435 model_checker-0.3.9/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:07.000000 model_checker-0.3.9/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    10264 2024-05-20 21:33:49.000000 model_checker-0.3.9/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19988 2024-05-20 20:33:25.000000 model_checker-0.3.9/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    23981 2024-05-20 21:34:33.000000 model_checker-0.3.9/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.9/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.9/src/model_checker/syntax.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.365435 model_checker-0.3.9/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      510 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.365435 model_checker-0.3.9/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.9/test/test.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.9/test/test_examples.py
```

### Comparing `model_checker-0.3.8/LICENCE` & `model_checker-0.3.9/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.8/PKG-INFO` & `model_checker-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.8
+Version: 0.3.9
 Summary: A hyperintensional theorem prover for counterfactual conditionals and modal operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.3.8/README.md` & `model_checker-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.8/pyproject.toml` & `model_checker-0.3.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.3.8"
+version = "0.3.9"
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
-model-checker = "__main__:main"
+model-checker = "model_checker.__main__:main"
```

### Comparing `model_checker-0.3.8/src/__main__.py` & `model_checker-0.3.9/src/model_checker/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 current_dir = os.path.dirname(__file__)
 # Construct the full path to your project root
 project_root = os.path.abspath(os.path.join(current_dir, ".."))
 # Add the project root to the Python path
 sys.path.append(project_root)
 
 # from model_structure import (
-from src.modules.model_structure import ( # for packaging
+from model_checker.model_structure import ( # for packaging
     StateSpace,
     make_model_for,
     )
 
 script_template = Template("""
 '''
 Model Checker: ${name}
```

### Comparing `model_checker-0.3.8/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.3.9/src/model_checker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.8
+Version: 0.3.9
 Summary: A hyperintensional theorem prover for counterfactual conditionals and modal operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.3.8/src/modules/model_definitions.py` & `model_checker-0.3.9/src/model_checker/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.8/src/modules/model_structure.py` & `model_checker-0.3.9/src/model_checker/model_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     Function,
     BitVecSort,
     BoolSort,
     BitVec,
     BitVecVal
 )
 
-from src.modules.semantics import ( # for packaging
+from model_checker.semantics import ( # for packaging
 # from semantics import (
     make_constraints,
     solve_constraints,
 )
-from src.modules.model_definitions import ( # for packaging
+from model_checker.model_definitions import ( # for packaging
 # from model_definitions import (
     find_compatible_parts,
     atomic_propositions_dict_maker,
     find_all_bits,
     find_max_comp_ver_parts,
     find_poss_bits,
     find_subsentences,
@@ -31,15 +31,15 @@
     pretty_set_print,
     bit_part,
     bitvec_to_substates,
     int_to_binary,
     true_and_false_worlds_for_cf,
     find_complex_proposition,
 )
-from src.modules.syntax import ( # for packaging
+from model_checker.syntax import ( # for packaging
 # from syntax import (
     AtomSort,
     infix,
     prefix,
     add_backslashes_to_infix,
 )
```

### Comparing `model_checker-0.3.8/src/modules/semantics.py` & `model_checker-0.3.9/src/model_checker/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.8/src/modules/syntax.py` & `model_checker-0.3.9/src/model_checker/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.8/test/test.py` & `model_checker-0.3.9/test/test.py`

 * *Files identical despite different names*


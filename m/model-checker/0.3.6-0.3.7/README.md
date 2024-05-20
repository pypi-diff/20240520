# Comparing `tmp/model_checker-0.3.6.tar.gz` & `tmp/model_checker-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.3.6.tar", last modified: Mon May 20 19:57:14 2024, max compression
+gzip compressed data, was "model_checker-0.3.7.tar", last modified: Mon May 20 21:27:12 2024, max compression
```

## Comparing `model_checker-0.3.6.tar` & `model_checker-0.3.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.631812 model_checker-0.3.6/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.6/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     6148 2024-05-20 19:57:14.631812 model_checker-0.3.6/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     5439 2024-05-20 19:10:52.000000 model_checker-0.3.6/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)      925 2024-05-20 19:56:28.000000 model_checker-0.3.6/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-20 19:57:14.631812 model_checker-0.3.6/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.630812 model_checker-0.3.6/src/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.630812 model_checker-0.3.6/src/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)       86 2024-05-08 21:34:17.000000 model_checker-0.3.6/src/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)     9994 2024-05-20 19:56:04.000000 model_checker-0.3.6/src/model_checker/__main__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19988 2024-05-20 19:17:58.000000 model_checker-0.3.6/src/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    23981 2024-05-20 19:56:16.000000 model_checker-0.3.6/src/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.6/src/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.6/src/model_checker/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     1864 2024-05-08 20:49:46.000000 model_checker-0.3.6/src/model_checker/temp.py
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.6/src/model_checker/test.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.631812 model_checker-0.3.6/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     6148 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      549 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.631812 model_checker-0.3.6/test/
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.6/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.7/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:27:12.396851 model_checker-0.3.7/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     5437 2024-05-20 20:33:25.000000 model_checker-0.3.7/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)      937 2024-05-20 21:26:50.000000 model_checker-0.3.7/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-20 21:27:12.396851 model_checker-0.3.7/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/src/
+-rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:07.000000 model_checker-0.3.7/src/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    10262 2024-05-20 21:23:26.000000 model_checker-0.3.7/src/__main__.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      482 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       52 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       26 2024-05-20 21:27:12.000000 model_checker-0.3.7/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/src/modules/
+-rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:54.000000 model_checker-0.3.7/src/modules/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19988 2024-05-20 20:33:25.000000 model_checker-0.3.7/src/modules/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    23975 2024-05-20 21:23:26.000000 model_checker-0.3.7/src/modules/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.7/src/modules/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.7/src/modules/syntax.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:27:12.396851 model_checker-0.3.7/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.7/test/test.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.7/test/test_examples.py
```

### Comparing `model_checker-0.3.6/LICENCE` & `model_checker-0.3.7/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.6/PKG-INFO` & `model_checker-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.6
-Summary: A hyperintensional model checker for counterfactual conditionals
+Version: 0.3.7
+Summary: A hyperintensional theorem prover for counterfactual conditionals and modal operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 License-File: LICENCE
 Requires-Dist: z3-solver
 
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for proving theorems and finding countermodels for counterfactual conditional and modal claims.
 
-Detailed [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
+Accessible [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
 
 ## Instructions
 
 To generate a test file run `model-checker` without arguments.
 
 Alternatively, run `model-checker path/to/test_file.py` if the `test_file.py` already exists.
 
@@ -59,15 +59,15 @@
 States are named by lowercase letters for the sake of printing readable countermodels.
 Fusions are printed using `.` so that `a.b` is the fusion of the states `a` and `b`.
 A state `a` is _part_ of a state `b` just in case `a.b = b`.
 States may be either _possible_ or _impossible_ where the null state is required to be possible and every part of a possible state is possible.
 The states `a` and `b` are _compatible_ just in case `a.b` is possible.
 A _world state_ is any state that is both possible and includes every compatible state as a part.
 
-Sentences are assigned _verifier states_ and _falsifier states_ where the both the verifiers and falsifiers are required to be closed under fusion.
+Sentences are assigned _verifier states_ and _falsifier states_ where both the verifiers and falsifiers are required to be closed under fusion.
 A sentence is _true at_ a world state `w` just in case `w` includes a verifier for that sentence as a part and _false at_ `w` just in case `w` includes a falsifier for that sentence as a part.
 In order to ensure that sentence letters have at most one truth-value at each world state, a fusion `a.b` is required to be impossible whenever `a` is verifier for a sentence letter `A` and `b` is a falsifier for `A`.
 Additionally, sentence letters have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
 
 Negated sentences are verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 Conjunctions are verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 Conjunction and disjunction are dual operators obeying the standard idempotent and De Morgan laws.
```

### Comparing `model_checker-0.3.6/README.md` & `model_checker-0.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for proving theorems and finding countermodels for counterfactual conditional and modal claims.
 
-Detailed [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
+Accessible [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
 
 ## Instructions
 
 To generate a test file run `model-checker` without arguments.
 
 Alternatively, run `model-checker path/to/test_file.py` if the `test_file.py` already exists.
 
@@ -43,15 +43,15 @@
 States are named by lowercase letters for the sake of printing readable countermodels.
 Fusions are printed using `.` so that `a.b` is the fusion of the states `a` and `b`.
 A state `a` is _part_ of a state `b` just in case `a.b = b`.
 States may be either _possible_ or _impossible_ where the null state is required to be possible and every part of a possible state is possible.
 The states `a` and `b` are _compatible_ just in case `a.b` is possible.
 A _world state_ is any state that is both possible and includes every compatible state as a part.
 
-Sentences are assigned _verifier states_ and _falsifier states_ where the both the verifiers and falsifiers are required to be closed under fusion.
+Sentences are assigned _verifier states_ and _falsifier states_ where both the verifiers and falsifiers are required to be closed under fusion.
 A sentence is _true at_ a world state `w` just in case `w` includes a verifier for that sentence as a part and _false at_ `w` just in case `w` includes a falsifier for that sentence as a part.
 In order to ensure that sentence letters have at most one truth-value at each world state, a fusion `a.b` is required to be impossible whenever `a` is verifier for a sentence letter `A` and `b` is a falsifier for `A`.
 Additionally, sentence letters have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
 
 Negated sentences are verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 Conjunctions are verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 Conjunction and disjunction are dual operators obeying the standard idempotent and De Morgan laws.
```

### Comparing `model_checker-0.3.6/pyproject.toml` & `model_checker-0.3.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.3.6"
-description = "A hyperintensional model checker for counterfactual conditionals"
+version = "0.3.7"
+description = "A hyperintensional theorem prover for counterfactual conditionals and modal operators."
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
@@ -23,8 +23,8 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/benbrastmckie/ModelChecker"
 Issues = "https://github.com/benbrastmckie/ModelChecker/issues"
 
 [project.scripts]
-model-checker = "model_checker.__main__:main"
+model-checker = "src.__main__:main"
```

### Comparing `model_checker-0.3.6/src/model_checker/__main__.py` & `model_checker-0.3.7/src/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 '''
 file specifies premises, conclusions, and settings.
 running the file finds a model and prints the result.
 '''
 
-# import cProfile
-# import pstats
+import sys
+import os
 from string import Template
 import argparse
 import importlib.util
-import sys
-import os
+# import cProfile
+# import pstats
+
+# Get the directory path of the current file
+current_dir = os.path.dirname(__file__)
+# Construct the full path to your project root
+project_root = os.path.abspath(os.path.join(current_dir, ".."))
+# Add the project root to the Python path
+sys.path.append(project_root)
+
 # from model_structure import (
-from model_checker.model_structure import ( # for packaging
+from src.modules.model_structure import ( # for packaging
     StateSpace,
     make_model_for,
     )
 
 script_template = Template("""
 '''
 Model Checker: ${name}
```

### Comparing `model_checker-0.3.6/src/model_checker/model_definitions.py` & `model_checker-0.3.7/src/modules/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.6/src/model_checker/model_structure.py` & `model_checker-0.3.7/src/modules/model_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     Function,
     BitVecSort,
     BoolSort,
     BitVec,
     BitVecVal
 )
 
-from model_checker.semantics import ( # for packaging
+from src.modules.semantics import ( # for packaging
 # from semantics import (
     make_constraints,
     solve_constraints,
 )
-from model_checker.model_definitions import ( # for packaging
+from src.modules.model_definitions import ( # for packaging
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
-from model_checker.syntax import ( # for packaging
+from src.modules.syntax import ( # for packaging
 # from syntax import (
     AtomSort,
     infix,
     prefix,
     add_backslashes_to_infix,
 )
```

### Comparing `model_checker-0.3.6/src/model_checker/semantics.py` & `model_checker-0.3.7/src/modules/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.6/src/model_checker/syntax.py` & `model_checker-0.3.7/src/modules/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.6/src/model_checker/test.py` & `model_checker-0.3.7/test/test.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.6/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.3.7/src/model_checker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.6
-Summary: A hyperintensional model checker for counterfactual conditionals
+Version: 0.3.7
+Summary: A hyperintensional theorem prover for counterfactual conditionals and modal operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 License-File: LICENCE
 Requires-Dist: z3-solver
 
 # Model Checker
 
 This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for proving theorems and finding countermodels for counterfactual conditional and modal claims.
 
-Detailed [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
+Accessible [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
 
 ## Instructions
 
 To generate a test file run `model-checker` without arguments.
 
 Alternatively, run `model-checker path/to/test_file.py` if the `test_file.py` already exists.
 
@@ -59,15 +59,15 @@
 States are named by lowercase letters for the sake of printing readable countermodels.
 Fusions are printed using `.` so that `a.b` is the fusion of the states `a` and `b`.
 A state `a` is _part_ of a state `b` just in case `a.b = b`.
 States may be either _possible_ or _impossible_ where the null state is required to be possible and every part of a possible state is possible.
 The states `a` and `b` are _compatible_ just in case `a.b` is possible.
 A _world state_ is any state that is both possible and includes every compatible state as a part.
 
-Sentences are assigned _verifier states_ and _falsifier states_ where the both the verifiers and falsifiers are required to be closed under fusion.
+Sentences are assigned _verifier states_ and _falsifier states_ where both the verifiers and falsifiers are required to be closed under fusion.
 A sentence is _true at_ a world state `w` just in case `w` includes a verifier for that sentence as a part and _false at_ `w` just in case `w` includes a falsifier for that sentence as a part.
 In order to ensure that sentence letters have at most one truth-value at each world state, a fusion `a.b` is required to be impossible whenever `a` is verifier for a sentence letter `A` and `b` is a falsifier for `A`.
 Additionally, sentence letters have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
 
 Negated sentences are verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 Conjunctions are verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
 Conjunction and disjunction are dual operators obeying the standard idempotent and De Morgan laws.
```


# Comparing `tmp/model_checker-0.3.5.tar.gz` & `tmp/model_checker-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.3.5.tar", last modified: Sat May 18 15:34:55 2024, max compression
+gzip compressed data, was "model_checker-0.3.6.tar", last modified: Mon May 20 19:57:14 2024, max compression
```

## Comparing `model_checker-0.3.5.tar` & `model_checker-0.3.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:34:55.559044 model_checker-0.3.5/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.5/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     5371 2024-05-18 15:34:55.559044 model_checker-0.3.5/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     4662 2024-05-12 17:17:50.000000 model_checker-0.3.5/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)      925 2024-05-18 15:34:37.000000 model_checker-0.3.5/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-18 15:34:55.559044 model_checker-0.3.5/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:34:55.558044 model_checker-0.3.5/src/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:34:55.559044 model_checker-0.3.5/src/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)       86 2024-05-08 21:34:17.000000 model_checker-0.3.5/src/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)     9631 2024-05-18 15:34:29.000000 model_checker-0.3.5/src/model_checker/__main__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19680 2024-05-18 15:02:56.000000 model_checker-0.3.5/src/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    26125 2024-05-18 15:29:14.000000 model_checker-0.3.5/src/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.5/src/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.5/src/model_checker/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     1864 2024-05-08 20:49:46.000000 model_checker-0.3.5/src/model_checker/temp.py
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.5/src/model_checker/test.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:34:55.559044 model_checker-0.3.5/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     5371 2024-05-18 15:34:55.000000 model_checker-0.3.5/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      549 2024-05-18 15:34:55.000000 model_checker-0.3.5/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-18 15:34:55.000000 model_checker-0.3.5/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-18 15:34:55.000000 model_checker-0.3.5/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-18 15:34:55.000000 model_checker-0.3.5/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-18 15:34:55.000000 model_checker-0.3.5/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-18 15:34:55.559044 model_checker-0.3.5/test/
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.5/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.631812 model_checker-0.3.6/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.6/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     6148 2024-05-20 19:57:14.631812 model_checker-0.3.6/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     5439 2024-05-20 19:10:52.000000 model_checker-0.3.6/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)      925 2024-05-20 19:56:28.000000 model_checker-0.3.6/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-20 19:57:14.631812 model_checker-0.3.6/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.630812 model_checker-0.3.6/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.630812 model_checker-0.3.6/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)       86 2024-05-08 21:34:17.000000 model_checker-0.3.6/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     9994 2024-05-20 19:56:04.000000 model_checker-0.3.6/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19988 2024-05-20 19:17:58.000000 model_checker-0.3.6/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    23981 2024-05-20 19:56:16.000000 model_checker-0.3.6/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.6/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.6/src/model_checker/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     1864 2024-05-08 20:49:46.000000 model_checker-0.3.6/src/model_checker/temp.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.6/src/model_checker/test.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.631812 model_checker-0.3.6/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     6148 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      549 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-20 19:57:14.000000 model_checker-0.3.6/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 19:57:14.631812 model_checker-0.3.6/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.6/test/test_examples.py
```

### Comparing `model_checker-0.3.5/LICENCE` & `model_checker-0.3.6/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.5/PKG-INFO` & `model_checker-0.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.5
+Version: 0.3.6
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
@@ -60,21 +60,25 @@
 Fusions are printed using `.` so that `a.b` is the fusion of the states `a` and `b`.
 A state `a` is _part_ of a state `b` just in case `a.b = b`.
 States may be either _possible_ or _impossible_ where the null state is required to be possible and every part of a possible state is possible.
 The states `a` and `b` are _compatible_ just in case `a.b` is possible.
 A _world state_ is any state that is both possible and includes every compatible state as a part.
 
 Sentences are assigned _verifier states_ and _falsifier states_ where the both the verifiers and falsifiers are required to be closed under fusion.
+A sentence is _true at_ a world state `w` just in case `w` includes a verifier for that sentence as a part and _false at_ `w` just in case `w` includes a falsifier for that sentence as a part.
 In order to ensure that sentence letters have at most one truth-value at each world state, a fusion `a.b` is required to be impossible whenever `a` is verifier for a sentence letter `A` and `b` is a falsifier for `A`.
 Additionally, sentence letters have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
-These definitions were originally provided in [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 
 Negated sentences are verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 Conjunctions are verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
-Conjunction and disjunction are dual operators obeying the standard De Morgan laws.
-The absorption laws do not hold, nor does conjunction distribute over disjunction, or _vice versa_.
-True counterfactual and modal sentences are verified by the null state and falsified by no states.
+Conjunction and disjunction are dual operators obeying the standard idempotent and De Morgan laws.
+The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
+For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
+
+A modal sentence `Box A` is true at a world just in case every world state includes a part that verifies `A`, where `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
+Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include `s` along with a maximal part of `w` that is compatible with `s` as parts.
+A counterfactual conditional sentences `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 
-The semantic theory for counterfactual conditionals is motivated and further elaborated in this [manuscript](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
-For the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
+The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
+This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker).
```

### Comparing `model_checker-0.3.5/README.md` & `model_checker-0.3.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -44,21 +44,25 @@
 Fusions are printed using `.` so that `a.b` is the fusion of the states `a` and `b`.
 A state `a` is _part_ of a state `b` just in case `a.b = b`.
 States may be either _possible_ or _impossible_ where the null state is required to be possible and every part of a possible state is possible.
 The states `a` and `b` are _compatible_ just in case `a.b` is possible.
 A _world state_ is any state that is both possible and includes every compatible state as a part.
 
 Sentences are assigned _verifier states_ and _falsifier states_ where the both the verifiers and falsifiers are required to be closed under fusion.
+A sentence is _true at_ a world state `w` just in case `w` includes a verifier for that sentence as a part and _false at_ `w` just in case `w` includes a falsifier for that sentence as a part.
 In order to ensure that sentence letters have at most one truth-value at each world state, a fusion `a.b` is required to be impossible whenever `a` is verifier for a sentence letter `A` and `b` is a falsifier for `A`.
 Additionally, sentence letters have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
-These definitions were originally provided in [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 
 Negated sentences are verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 Conjunctions are verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
-Conjunction and disjunction are dual operators obeying the standard De Morgan laws.
-The absorption laws do not hold, nor does conjunction distribute over disjunction, or _vice versa_.
-True counterfactual and modal sentences are verified by the null state and falsified by no states.
+Conjunction and disjunction are dual operators obeying the standard idempotent and De Morgan laws.
+The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
+For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
-The semantic theory for counterfactual conditionals is motivated and further elaborated in this [manuscript](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
-For the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
+A modal sentence `Box A` is true at a world just in case every world state includes a part that verifies `A`, where `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
+Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include `s` along with a maximal part of `w` that is compatible with `s` as parts.
+A counterfactual conditional sentences `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
+
+The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
+This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker).
```

### Comparing `model_checker-0.3.5/pyproject.toml` & `model_checker-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.3.5"
+version = "0.3.6"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
```

### Comparing `model_checker-0.3.5/src/model_checker/__main__.py` & `model_checker-0.3.6/src/model_checker/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 '''
 file specifies premises, conclusions, and settings.
 running the file finds a model and prints the result.
 '''
 
+# import cProfile
+# import pstats
 from string import Template
 import argparse
 import importlib.util
 import sys
 import os
-# from model_structure import StateSpace, make_model_for
+# from model_structure import (
 from model_checker.model_structure import ( # for packaging
     StateSpace,
     make_model_for,
     )
 
 script_template = Template("""
 '''
@@ -22,15 +24,15 @@
 parent_directory = os.path.dirname(__file__)
 file_name = os.path.basename(__file__)
 
 ################################
 ########## SETTINGS ############
 ################################
 
-# length of bitvectors
+# number of atomic states
 N = 3
 
 # print all Z3 constraints if a model is found
 print_cons_bool = False
 
 # print core unsatisfiable Z3 constraints if no model exists
 print_unsat_core_bool = True
@@ -267,7 +269,19 @@
     if save_model:
         file_name, print_cons = ask_save()
         no_model_save_or_append(module, model_structure, file_name, print_unsat, print_imposs)
 
 
 if __name__ == "__main__":
     main()
+    # cProfile.run('main()')
+    # cProfile.run('main()', 'profile_results')
+
+
+# # Load the profiling data
+# with open('profile_results', 'r') as f:
+#     # profiler = pstats.Stats(f)
+#     filename = 'profile_results'
+#     profiler = pstats.Stats(filename)
+#
+# # Sort and print the profiling data by time
+# profiler.sort_stats('time').print_stats()
```

### Comparing `model_checker-0.3.5/src/model_checker/model_definitions.py` & `model_checker-0.3.6/src/model_checker/model_definitions.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,21 +19,18 @@
 #     '''finds the null bit'''
 #     return [BitVecVal(0, size)]
 
 def find_all_bits(size):
     '''extract all bitvectors from the input model
     imported by model_structure'''
     all_bits = []
-    max_bit_number = summation(
-        size + 1, lambda x: 2**x
-    )  # this should hopefully be enough to cover all states
+    max_bit_number = summation(size + 1, lambda x: 2**x)
     for val in range(max_bit_number):
         test_bit = BitVecVal(val, size)
         if test_bit in all_bits:
-        # break once bits start to repeat
             continue
         all_bits.append(test_bit)
     return all_bits
 
 
 def find_poss_bits(z3_model, all_bits, possible):
     '''extract all possible bitvectors from all_bits given the model
@@ -55,22 +52,14 @@
         for test in poss_bits:
             if bit_part(test, potential_world):
                 continue
             if bit_proper_part(potential_world, test):
                 not_worlds.append(potential_world)
                 break
     world_bits = [world for world in poss_bits if world not in not_worlds]
-    # for world in world_bits:
-    #     print(model.evaluate(is_world(world)))
-    #     if not model.evaluate(is_world(world)):
-    #         raise ValueError(f'{world} was in world_bits but is not a world per the model')
-    # for not_world in not_worlds:
-    #     print(model.evaluate(is_world(not_world)))
-    #     # if model.evaluate(is_world(not_world)):
-    #     #     raise ValueError(f'{not_world} was not in world_bits but is a world per the model')
     return world_bits
 
 
 def find_compatible_parts(verifier_bit, poss_bits, eval_world):
     """
     Finds the parts of the eval_world compatible with the verifier_bit.
     Used in find_alt_bits() method in ModelStructure class
@@ -105,81 +94,73 @@
     DOES NOT CHECK IF THESE ARE POSSIBLE. """
     relation_set = set()
     for bit in all_bits:
         if z3_model.evaluate(relation(bit, z3_model[sentence])):
             relation_set.add(bit)
     return relation_set
 
-def find_true_and_false_in_alt(alt_bit, model_structure):
-    """returns two sets as a tuple, one being the set of sentences true in the alt world and the other the set being false.
-    Used in evaluate_mainclause_cf_expr()"""
-    extensional_sentences = model_structure.extensional_subsentences
-    # B: is this still true once modal and counterfactual prop_objects include verifiers and falsifiers?
-    # TODO: below creates problem with nested counterfactuals
-    # TODO: I think this was resolved
-    # extensional_sentences = parent_model_structure.all_subsentences
-    all_bits = model_structure.all_bits
-    true_in_alt = []
-    for R in extensional_sentences:
-        for bit in all_bits:
-            # print(model.evaluate(extended_verify(bit, R, evaluate=True), model_completion=True))
-            # print(type(model.evaluate(extended_verify(bit, R, evaluate=True), model_completion=True)))
-            if bit in find_complex_proposition(model_structure, R, alt_bit)[0] and bit_part(bit, alt_bit):
-                true_in_alt.append(R)
-                break  # returns to the for loop over sentence_letters
-    false_in_alt = [R for R in extensional_sentences if not R in true_in_alt] # replace with
-    return (repeats_removed(true_in_alt), repeats_removed(false_in_alt))
-    # was giving repeats for some reason? Wasn't previously. fixed it up with repeats_removed
+# def find_true_and_false_in_alt(alt_bit, model_structure):
+#     """returns two sets as a tuple, one being the set of sentences true in the alt world and the other the set being false.
+#     Used in evaluate_mainclause_cf_expr()"""
+#     all_subsentences = model_structure.all_subsentences
+#     # extensional_sentences = parent_model_structure.all_subsentences
+#     all_bits = model_structure.all_bits
+#     true_in_alt = []
+#     for sub in all_subsentences:
+#         for bit in all_bits:
+#             # print(model.evaluate(extended_verify(bit, R, evaluate=True), model_completion=True))
+#             # print(type(model.evaluate(extended_verify(bit, R, evaluate=True), model_completion=True)))
+#             if bit in find_complex_proposition(model_structure, sub, alt_bit)[0] and bit_part(bit, alt_bit):
+#                 true_in_alt.append(sub)
+#                 break  # returns to the for loop over sentence_letters
+#     false_in_alt = [R for R in all_subsentences if not R in true_in_alt] # replace with
+#     return (repeats_removed(true_in_alt), repeats_removed(false_in_alt))
+#     # was giving repeats for some reason? Wasn't previously. fixed it up with repeats_removed
 
 
 def pretty_set_print(set_with_strings):
-    """input a set with strings
-    print that same set but with no quotation marks around each individual string, and also with the set in order
-    returns the set as a string
+    """input a set with strings print that same set but with no quotation marks around each
+    individual string, and also with the set in order returns the set as a string
     Used in print_vers_and_fals() and print_alt_worlds()"""
     sorted_set = sorted(list(set_with_strings))  # actually type list, not set
     print_str = "{"
     for i, elem in enumerate(sorted_set):
         print_str += elem
         if i != len(sorted_set) - 1:
             print_str += ", "
     print_str += "}"
     return print_str
 
 def product(set_A, set_B):
+    """set of pairwise fusions of elements in set_A and set_B"""
     product_set = set()
     for a in set_A:
         for b in set_B:
             product_set.add(bit_fusion(a,b))
     return product_set
 
 def coproduct(set_A, set_B):
+    """union closed under pairwise fusion"""
     A_U_B = set_A.union(set_B)
     return A_U_B.union(product(set_A, set_B))
 
-def atomic_propositions_dict_maker(ms_object):
-    all_bits = ms_object.all_bits
-    sentence_letters = ms_object.sentence_letters
-    z3_model = ms_object.z3_model
-    verify = ms_object.verify
-    falsify = ms_object.falsify
+def atomic_propositions_dict_maker(state_space):
+    """assigns sentence_letters to propositions"""
+    all_bits = state_space.all_bits
+    sentence_letters = state_space.sentence_letters
+    z3_model = state_space.z3_model
+    verify = state_space.verify
+    falsify = state_space.falsify
     atomic_VFs_dict = {}
     for letter in sentence_letters:
         ver_bits = relate_sents_and_states(all_bits, letter, z3_model, verify)
         fal_bits = relate_sents_and_states(all_bits, letter, z3_model, falsify)
         atomic_VFs_dict[letter] = (ver_bits, fal_bits)
     return atomic_VFs_dict
 
-
-#############################################
-######### MOVED FROM DEFINITIONS.PY #########
-#############################################
-        
-
-
 def bit_fusion(bit_s, bit_t):
     """the result of taking the maximum for each index in _s and _t"""
     return simplify(bit_s | bit_t)
     # NOTE: this does seem to make a difference, otherwise no comp_parts
 
 def bit_part(bit_s, bit_t):
     """the fusion of _s and _t is identical to bit_t"""
@@ -270,144 +251,166 @@
 def prefix_combine(prefix_premises, prefix_conclusions):
     '''negates and disjoins the prefix conclusions, combining the result with
     prefix premises to form a new list'''
     neg_conclusions = [['\\neg ', con] for con in prefix_conclusions]
     disjoin_neg_conclusions = disjoin_prefix(neg_conclusions)
     return prefix_premises + disjoin_neg_conclusions
 
-#################################
-##### MOVED FROM SEMANTICS ######
-#################################
-
-def is_counterfactual(prefix_sentence):
-    '''returns a boolean to say whether a given sentence is a counterfactual
-    used in find_extensional_subsentences'''
-    if len(prefix_sentence) == 1:
-        return False
-    if len(prefix_sentence) == 2:
-        return is_counterfactual(prefix_sentence[1])
-    if 'boxright' in prefix_sentence[0]:
-        return True
-    return is_counterfactual(prefix_sentence[1]) or is_counterfactual(prefix_sentence[2])
+# def is_counterfactual(prefix_sentence):
+#     '''returns a boolean to say whether a given sentence is a counterfactual
+#     used in find_extensional_subsentences'''
+#     if len(prefix_sentence) == 1:
+#         return False
+#     if len(prefix_sentence) == 2:
+#         return is_counterfactual(prefix_sentence[1])
+#     if 'boxright' in prefix_sentence[0]:
+#         return True
+#     return is_counterfactual(prefix_sentence[1]) or is_counterfactual(prefix_sentence[2])
+
+# def is_modal(prefix_sentence):
+#     '''returns a boolean to say whether a given sentence is a counterfactual
+#     used in find_extensional_subsentences'''
+#     if len(prefix_sentence) == 1:
+#         return False
+#     op = prefix_sentence[0]
+#     if len(prefix_sentence) == 2:
+#         if 'Box' in op or 'Diamond' in op:
+#             return True
+#         return is_modal(prefix_sentence[1])
+#     return is_modal(prefix_sentence[1]) or is_modal(prefix_sentence[2])
+
+# def is_extensional(prefix_sentence):
+#     return not is_modal(prefix_sentence) and not is_counterfactual(prefix_sentence)
+
+# def all_subsentences_of_a_sentence(prefix_sentence, progress=[]):
+#     '''finds all the subsentence of a prefix sentence
+#     returns these as a set
+#     used in find_extensional_subsentences'''
+#     if progress is False:
+#         progress = []
+#     progress.append(prefix_sentence)
+#     if len(prefix_sentence) == 1:
+#         return progress
+#     if len(prefix_sentence) == 2:
+#         return all_subsentences_of_a_sentence(prefix_sentence[1], progress)
+#     if len(prefix_sentence) == 3:
+#         left_subsentences = all_subsentences_of_a_sentence(prefix_sentence[1], progress)
+#         right_subsentences = all_subsentences_of_a_sentence(prefix_sentence[2], progress)
+#         all_subsentences = left_subsentences + right_subsentences
+#         return all_subsentences
+
+# def find_subsentences_of_kind(prefix_sentences, kind):
+#     '''used to find the extensional, modal, and counterfactual sentences. 
+#     kind is a string, either "extensional", "modal", "counterfactual", or 'all' for a tuple of
+#     of the three kinds in the order extensional, modal, counterfactual, and then all the subsents
+#     returns a list of that kind'''
+#     rr = repeats_removed
+#     all_subsentences = []
+#     for prefix_sent in prefix_sentences:
+#         all_subsentences.extend(all_subsentences_of_a_sentence(prefix_sent))
+#     if kind == 'extensional':
+#         return_list = [sent for sent in all_subsentences if is_extensional(sent)]
+#     if kind == 'modal':
+#         return_list = [sent for sent in all_subsentences if is_modal(sent)]
+#     if kind == 'counterfactual':
+#         return_list = [sent for sent in all_subsentences if is_counterfactual(sent)]
+#     if kind == 'all':
+#         counterfactual = rr([sent for sent in all_subsentences if is_counterfactual(sent)])
+#         modal = rr([sent for sent in all_subsentences if is_modal(sent)])
+#         extensional = rr([sent for sent in all_subsentences if sent not in counterfactual and sent not in modal])
+#         return (extensional, modal, counterfactual, all_subsentences)
+#     return rr(return_list)
 
-def is_modal(prefix_sentence):
-    '''returns a boolean to say whether a given sentence is a counterfactual
-    used in find_extensional_subsentences'''
-    if len(prefix_sentence) == 1:
-        return False
-    op = prefix_sentence[0]
-    if len(prefix_sentence) == 2:
-        if 'Box' in op or 'Diamond' in op:
-            return True
-        return is_modal(prefix_sentence[1])
-    return is_modal(prefix_sentence[1]) or is_modal(prefix_sentence[2])
-
-def is_extensional(prefix_sentence):
-    return not is_modal(prefix_sentence) and not is_counterfactual(prefix_sentence)
-
-# TODO: linter says all or none of the returns should be an expression
-def all_subsentences_of_a_sentence(prefix_sentence, progress=False):
+def subsentences_of(prefix_sentence):
     '''finds all the subsentence of a prefix sentence
     returns these as a set
     used in find_extensional_subsentences'''
-    if progress is False:
-        progress = []
-    # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
+    progress = []
     progress.append(prefix_sentence)
-    if len(prefix_sentence) == 1:
-        return progress
     if len(prefix_sentence) == 2:
-        # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-        return all_subsentences_of_a_sentence(prefix_sentence[1], progress)
+        sub_sentsentences = subsentences_of(prefix_sentence[1])
+        return progress + sub_sentsentences
     if len(prefix_sentence) == 3:
-        # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-        left_subsentences = all_subsentences_of_a_sentence(prefix_sentence[1], progress)
-        # TODO: linter says cannot access member "append" for type "Literal[True]" Member "append" is unknown
-        right_subsentences = all_subsentences_of_a_sentence(prefix_sentence[2], progress)
-        all_subsentences = left_subsentences + right_subsentences
-        return all_subsentences
-
-def find_subsentences_of_kind(prefix_sentences, kind):
-    '''used to find the extensional, modal, and counterfactual sentences. 
-    kind is a string, either "extensional", "modal", "counterfactual", or 'all' for a tuple of
-    of the three kinds in the order extensional, modal, counterfactual, and then all the subsents
-    returns a list of that kind'''
-    rr = repeats_removed
+        left_subsentences = subsentences_of(prefix_sentence[1])
+        right_subsentences = subsentences_of(prefix_sentence[2])
+        all_subsentences = left_subsentences + right_subsentences + progress
+        return repeats_removed(all_subsentences)
+    return progress
+
+def find_subsentences(prefix_sentences):
+    """take a set of prefix sentences and returns a set of all subsentences"""
     all_subsentences = []
     for prefix_sent in prefix_sentences:
-        all_subsentences.extend(all_subsentences_of_a_sentence(prefix_sent))
-    if kind == 'extensional':
-        return_list = [sent for sent in all_subsentences if is_extensional(sent)]
-    if kind == 'modal':
-        return_list = [sent for sent in all_subsentences if is_modal(sent)]
-    if kind == 'counterfactual':
-        return_list = [sent for sent in all_subsentences if is_counterfactual(sent)]
-    if kind == 'all':
-        counterfactual = rr([sent for sent in all_subsentences if is_counterfactual(sent)])
-        modal = rr([sent for sent in all_subsentences if is_modal(sent)])
-        extensional = rr([sent for sent in all_subsentences if sent not in counterfactual and sent not in modal])
-        return (extensional, modal, counterfactual, all_subsentences)
-    return rr(return_list)
+        all_prefix_subs = subsentences_of(prefix_sent)
+        all_subsentences.extend(all_prefix_subs)
+    return repeats_removed(all_subsentences)
 
-def repeats_removed(L):
+def repeats_removed(sentences):
     '''takes a list and removes the repeats in it.
     used in find_all_constraints'''
     seen = []
-    for obj in L:
+    for obj in sentences:
         if obj not in seen:
             seen.append(obj)
     return seen
 
 
-########################################
-###### MOVED FROM model_structure ######
-########################################
-
 def evaluate_modal_expr(model_structure, prefix_modal, eval_world):
     '''evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
     used to initialize Counterfactuals
     returns a bool representing whether the counterfactual is true at the world or not'''
     op, argument = prefix_modal[0], prefix_modal[1]
-    if is_modal(argument):
-        if model_structure.evaluate_modal_expr(prefix_modal) is True: # ie, verifiers is null state
-            return True # both Box and Diamond will return true, since verifiers is not empty
-        return False
+    # if is_modal(argument):
+    #     if model_structure.evaluate_modal_expr(prefix_modal) is True: # ie, verifiers is null state
+    #         return True # both Box and Diamond will return true, since verifiers is not empty
+    #     return False
     if 'Diamond' in op:
-        # TODO: linter error: uninitalized is not iterable  "__iter__" does not return object
         for poss in model_structure.poss_bits:
             if poss in find_complex_proposition(model_structure, argument, eval_world)[0]:
                 return True
         return False
     if 'Box' in op:
-        # TODO: linter error: uninitalized is not iterable  "__iter__" does not return object
         for poss in model_structure.poss_bits:
             if poss in find_complex_proposition(model_structure, argument, eval_world)[1]:
                 return False
         return True
 
-def evaluate_mainclause_cf_expr(model_structure, prefix_cf, eval_world):
+def evaluate_cf_expr(state_space, prefix_cf, eval_world):
     """evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
     used to initialize Counterfactuals
     returns a bool representing whether the counterfactual is true at the world or not
     """
-    op = prefix_cf[0]
-    assert "boxright" in op, f"{prefix_cf} is not a main-clause counterfactual!"
-    ant_expr, consequent_expr = prefix_cf[1], prefix_cf[2]
-    # assert is_extensional(ant_expr), f"the antecedent {ant_expr} is not extensional!"
-    ant_verifiers = find_complex_proposition(model_structure, ant_expr, eval_world)[0]
-    ant_alts_to_eval_world = model_structure.find_alt_bits(ant_verifiers, eval_world)
-    for u in ant_alts_to_eval_world:
-        # QUESTION: why is string required? Is Z3 removing the lists?
-        if is_counterfactual(consequent_expr):
-            if not find_complex_proposition(model_structure, consequent_expr, u)[0]:
-                return False
-        elif str(consequent_expr) not in str(find_true_and_false_in_alt(u, model_structure)[0]):
-            return False
+    antecedent, consequent = prefix_cf[1], prefix_cf[2]
+    ant_verifiers = find_complex_proposition(state_space, antecedent, eval_world)[0]
+    con_falsifiers = find_complex_proposition(state_space, consequent, eval_world)[1]
+    antecedent_alts = state_space.find_alt_bits(ant_verifiers, eval_world)
+    if any(bit_part(con_fal, u) for u in antecedent_alts for con_fal in con_falsifiers):
+        return False
     return True
 
+# def evaluate_mainclause_cf_expr(model_structure, prefix_cf, eval_world):
+#     """evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
+#     used to initialize Counterfactuals
+#     returns a bool representing whether the counterfactual is true at the world or not
+#     """
+#     op = prefix_cf[0]
+#     assert "boxright" in op, f"{prefix_cf} is not a main-clause counterfactual!"
+#     ant_expr, consequent_expr = prefix_cf[1], prefix_cf[2]
+#     # assert is_extensional(ant_expr), f"the antecedent {ant_expr} is not extensional!"
+#     ant_verifiers = find_complex_proposition(model_structure, ant_expr, eval_world)[0]
+#     ant_alts_to_eval_world = model_structure.find_alt_bits(ant_verifiers, eval_world)
+#     for u in ant_alts_to_eval_world:
+#         # QUESTION: why is string required? Is Z3 removing the lists?
+#         if is_counterfactual(consequent_expr):
+#             if not find_complex_proposition(model_structure, consequent_expr, u)[0]:
+#                 return False
+#         elif str(consequent_expr) not in str(find_true_and_false_in_alt(u, model_structure)[0]):
+#             return False
+#     return True
+
 def true_and_false_worlds_for_cf(model_structure, complex_cf_sent):
     '''used in find_complex_proposition'''
     worlds_true_at, worlds_false_at = set(), set()
     for world in model_structure.world_bits:
         if find_complex_proposition(model_structure, complex_cf_sent, world)[0]:
             worlds_true_at.add(world)
             continue
@@ -449,11 +452,12 @@
         return (
             product(coproduct(Y_F, Z_V), coproduct(Y_V, Z_F)),
             coproduct(product(Y_V, Z_F), product(Y_F, Z_V)),
         )
     if "rightarrow" in op:
         return (coproduct(Y_F, Z_V), product(Y_V, Z_F))
     if "boxright" in op:
-        if evaluate_mainclause_cf_expr(model_structure, complex_sentence, eval_world):
+        # if evaluate_mainclause_cf_expr(model_structure, complex_sentence, eval_world):
+        if evaluate_cf_expr(model_structure, complex_sentence, eval_world):
             return (null_state, set())
         return (set(), null_state)
     raise ValueError(f"Don't know how to handle {op} operator")
```

### Comparing `model_checker-0.3.5/src/model_checker/model_structure.py` & `model_checker-0.3.6/src/model_checker/model_structure.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,21 @@
 from model_checker.model_definitions import ( # for packaging
 # from model_definitions import (
     find_compatible_parts,
     atomic_propositions_dict_maker,
     find_all_bits,
     find_max_comp_ver_parts,
     find_poss_bits,
+    find_subsentences,
     find_world_bits,
     prefix_combine,
     pretty_set_print,
     bit_part,
     bitvec_to_substates,
     int_to_binary,
-    find_subsentences_of_kind,
-    is_counterfactual,
     true_and_false_worlds_for_cf,
     find_complex_proposition,
 )
 from model_checker.syntax import ( # for packaging
 # from syntax import (
     AtomSort,
     infix,
@@ -116,19 +115,15 @@
             self.assign,
             self.N,
             self.w
         )
         constraints, sentence_letters = find_constraints_func(self.prefix_sentences)
         self.sentence_letters = sentence_letters
         self.constraints = constraints
-        ext, modal, cf, altogether = find_subsentences_of_kind(self.prefix_sentences, 'all')
-        self.extensional_subsentences = ext
-        self.counterfactual_subsentences = cf
-        self.modal_subsentences = modal
-        self.all_subsentences = altogether # in prefix form
+        self.all_subsentences = find_subsentences(self.prefix_sentences)
 
     # def constraints_func(self):
     #     """returns constraints_func"""
     #     return self.find_constraints_func
 
     def solve(self):
         """solves for the model, returns None
@@ -160,18 +155,14 @@
         self.model_status = model_status
         self.model_setup = model_setup
         self.z3_model = z3_model
         self.model_runtime = model_runtime
         self.infix_premises = model_setup.infix_premises
         self.infix_conclusions = model_setup.infix_conclusions
         self.N = model_setup.N
-        self.prefix_premises = [prefix(prem) for prem in model_setup.infix_premises]
-        # M: I think below is a problem
-        self.prefix_conclusions = [prefix(con) for con in model_setup.infix_conclusions]
-        self.prefix_sentences = prefix_combine(self.prefix_premises, self.prefix_conclusions)
 
     def build_test_file(self, output):
         """generates a test file from input to be saved"""
         inputs_data = {
             "N": self.model_setup.N,
             "premises": self.infix_premises,
             "conclusions": self.infix_conclusions,
@@ -246,29 +237,27 @@
         self.all_bits = find_all_bits(self.N)
         self.poss_bits = find_poss_bits(self.z3_model, self.all_bits, model_setup.possible)
         self.world_bits = find_world_bits(self.poss_bits)
         self.main_world = self.z3_model[self.main_world]
         self.sentence_letters = model_setup.sentence_letters
         self.verify = model_setup.verify
         self.falsify = model_setup.falsify
+        self.all_subsentences = model_setup.all_subsentences
         self.atomic_props_dict = atomic_propositions_dict_maker(self)
-
-        # TODO: one attribute for all propositions (check)
-        # self.all_subsentences = model_setup.all_subsentences
-        self.extensional_subsentences = model_setup.extensional_subsentences
-        self.extensional_propositions = [Proposition(ext_subsent, self, self.main_world)
-                                        for ext_subsent in model_setup.extensional_subsentences]
-        self.counterfactual_propositions = [Proposition(cf_subsent, self, self.main_world)
-                                        for cf_subsent in model_setup.counterfactual_subsentences]
-        self.modal_propositions = [Proposition(modal_subsent, self, self.main_world)
-                                    for modal_subsent in model_setup.modal_subsentences]
-        self.all_propositions = (self.extensional_propositions +
-                                 self.counterfactual_propositions + self.modal_propositions)
-        self.premise_propositions = self.find_propositions(model_structure.prefix_premises, True)
-        self.conclusion_propositions = self.find_propositions(model_structure.prefix_conclusions, True)
+        self.all_propositions = [
+            Proposition(sent, self, self.main_world) for sent in model_setup.all_subsentences
+        ]
+        self.premise_propositions = [
+            Proposition(sent, self, self.main_world) for sent in model_setup.prefix_premises
+        ]
+        self.conclusion_propositions = [
+            Proposition(sent, self, self.main_world) for sent in model_setup.prefix_conclusions
+        ]
+        # self.premise_propositions = self.find_propositions(model_setup.prefix_premises, True)
+        # self.conclusion_propositions = self.find_propositions(model_setup.prefix_conclusions, True)
 
     def find_alt_bits(self, verifier_bits, evaulation_world=None):
         """
         Finds the alternative bits given verifier bits of an extensional proposition,
         possible states, worlds, and the evaluation world.
         Used in evaluate_cf_expression() and rec_print().
         """
@@ -288,61 +277,57 @@
         return alt_bits
 
     # Useful to user now that can search an infix expression
     def find_proposition_object(self, expression, prefix_search=False):
         """given a sentence, finds the Proposition object in the model that corresponds
         to it. Can optionally search through only the extensional sentences
         Also defaults to searching an infix sentence, though internally it always searches
-        prefix. 
+        prefix.
         If search infix, make sure you put double backslashes always!!
         returns a Proposition object"""
-        search_list = self.all_propositions
-        if prefix_search:
-            for prop_object in search_list:
-                if prop_object["prefix expression"] == expression:
-                    return prop_object
-        else:
-            for prop_object in search_list:
-                if str(prop_object) == add_backslashes_to_infix(expression):
-                    return prop_object
+        # search_list = self.all_propositions
+        # if prefix_search:
+        #     for prop_object in search_list:
+        #         if prop_object["prefix expression"] == expression:
+        #             return prop_object
+        # else:
+        #     for prop_object in search_list:
+        #         if str(prop_object) == add_backslashes_to_infix(expression):
+        #             return prop_object
+        for prop_object in self.all_propositions:
+            if prop_object["prefix expression"] == expression:
+                return prop_object
         raise ValueError(
             f"there is no Proposition with expression {expression}")
 
-    # Useful to user now that can search infix expressions
-    def find_propositions(self, sentences, prefix_search=False):
-        """finds all the Proposition objects in a ModelStructure
-        that correspond to the prefix sentences in sentences.
-        returns them as a list"""
-        propositions = []
-        for sent in sentences:
-            propositions.append(self.find_proposition_object(sent, prefix_search=prefix_search))
-        return propositions
+    # # Useful to user now that can search infix expressions
+    # def find_propositions(self, sentences, prefix_search=False):
+    #     """finds all the Proposition objects in a ModelStructure
+    #     that correspond to the prefix sentences in sentences.
+    #     returns them as a list"""
+    #     propositions = []
+    #     for sent in sentences:
+    #         propositions.append(self.find_proposition_object(sent, prefix_search=prefix_search))
+    #     return propositions
 
     def print_evaluation(self, output=sys.__stdout__):
         """print the evaluation world and all sentences letters that true/false
         in that world"""
-        # TODO: all this seems to do is print the sentences true/false in each world.
-        # can this be simplified? might it make sense to store sentence letters true
-        # at the designated world and the sentence letters false at the designated
-        # world in the class? then those could be easily called here.
         N = self.model_setup.N
         sentence_letters = self.sentence_letters
         main_world = self.main_world
         print(
             f"\nThe evaluation world is {bitvec_to_substates(main_world, N)}:",
             file=output,
         )
         true_in_eval = set()
         for sent in sentence_letters:
-            # TODO: linter error: "Uninitalized" is not iterable  "__iter__" method does not return an object
             for bit in self.all_bits:
-                # TODO: linter error: expected 0 positional arguments
                 ver_bool = self.model_setup.verify(bit, self.z3_model[sent])
                 part_bool = bit_part(bit, main_world)
-                # TODO: linter error: invalid conditional operand band-aid fixed with bool
                 if bool(self.z3_model.evaluate(ver_bool) and part_bool):
                     true_in_eval.add(sent)
                     break  # exits the first for loop
         false_in_eval = {R for R in sentence_letters if not R in true_in_eval}
         if true_in_eval:
             true_eval_list = sorted([str(sent) for sent in true_in_eval])
             true_eval_string = ", ".join(true_eval_list)
@@ -415,17 +400,14 @@
         if 'Diamond' in op or 'Box' in op:
             for u in self.world_bits:
                 self.rec_print(first_subprop, u, print_impossible, output, indent)
             return
         left_subprop = first_subprop
         right_subprop = self.find_proposition_object(prefix_expr[2], prefix_search=True)
         if "boxright" in op:
-            # assert (
-            #     left_subprop in self.extensional_propositions
-            # ), f"{prop_obj} is not a valid cf because antecedent {left_subprop} is not extensional"
             left_subprop_vers = left_subprop['verifiers']
             phi_alt_worlds_to_world_bit = self.find_alt_bits(left_subprop_vers, world_bit)
             alt_worlds_as_strings = {bitvec_to_substates(u,N) for u in phi_alt_worlds_to_world_bit}
             self.rec_print(left_subprop, world_bit, print_impossible, output, indent)
             print(
                 f'{"  " * indent}'
                 f'{left_subprop}-alternatives to {bitvec_to_substates(world_bit, N)} = '
@@ -471,38 +453,30 @@
         N = self.model_setup.N
         print(f"There is a {N}-model of:\n", file=output)
         self.model_structure.print_enumerate(output)
         self.print_states(print_impossible, output)
         self.print_evaluation(output)
         self.print_inputs_recursively(print_impossible, output)
 
-
-
-
 class Proposition:
     """class for propositions to store their verifiers, falsifiers, alt worlds, etc
     has two subclasses Extensional and Counterfactual—Counterfactual is a Proposition
     subclass to make stuff easier"""
 
     def __init__(self, prefix_expr, model_structure, eval_world):
         """for modals and counterfactuals, if they're true then the verifiers
         are only the null state and falsifiers are nothing; if they're false the opposite"""
         self.prop_dict = {}
         self.prop_dict["prefix expression"] = prefix_expr
         self.model_structure = model_structure
         verifiers, falsifiers = find_complex_proposition(model_structure, prefix_expr, eval_world)
-        self.world_bits = model_structure.world_bits # NOTE: this isn't being called anywhere
         self.prop_dict["verifiers"] = verifiers
         self.prop_dict["falsifiers"] = falsifiers
-        # if is_modal(prefix_expr):
-        #     arg = prefix_expr[1]
-        #     arg_worlds, non_arg_worlds = find_complex_proposition(model_structure, arg, eval_world)
-        #     self['arg worlds'] = arg_worlds
-        #     self['non arg worlds'] = non_arg_worlds
-        if is_counterfactual(prefix_expr):
+        # if is_counterfactual(prefix_expr):
+        if 'boxright' in str(prefix_expr[0]):
             self.current_eval_world = eval_world
             true_worlds, false_worlds = true_and_false_worlds_for_cf(model_structure, prefix_expr)
             self['worlds cf true at'] = true_worlds
             self['worlds cf false at'] = false_worlds
 
     def __setitem__(self, key, value):
         self.prop_dict[key] = value
@@ -511,34 +485,36 @@
         '''NOTE: If a user wants to access a modal or counterfactual Proposition's verifiers, 
         THEY SHOULD NOT. They should instead use the truth_value_at() method'''
         return self.prop_dict[key]
 
     def __str__(self):
         return infix(self["prefix expression"])
 
-    def update_verifiers(self, new_world):
-        if not is_counterfactual(self['prefix expression']):
-            raise AttributeError(f'You can only update verifiers for CFs, and {self} is not a CF.')
+    def update_verifiers(self, eval_world):
+        """updates the evaluation world for counterfactuals"""
+        # if not is_counterfactual(self['prefix expression']):
+        #     raise AttributeError(f'You can only update verifiers for CFs, and {self} is not a CF.')
         N = self.model_structure.N
-        if new_world == self.current_eval_world:
-            return 
-        if new_world in self['worlds cf true at']:
+        if eval_world == self.current_eval_world:
+            return
+        if eval_world in self['worlds cf true at']:
             self['verifiers'], self['falsifiers'] = {BitVecVal(0,N)}, set()
             return
         self['verifiers'], self['falsifiers'] = set(), {BitVecVal(0,N)}
         return
 
     def print_verifiers_and_falsifiers(self, eval_world, print_impossible=False, indent=0, output=sys.__stdout__):
         """prints the possible verifiers and falsifier states for a sentence.
         used in: rec_print() 
         ensures eval_world is in fact the eval_world for CFs"""
         N = self.model_structure.N
         truth_value = self.truth_value_at(eval_world)
-        if self in self.model_structure.counterfactual_propositions:
-            self.update_verifiers(eval_world)
+        # prefix_expr_op = self.prop_dict["prefix expression"][0]
+        # if 'boxright' in str(prefix_expr_op):
+        #     self.update_verifiers(eval_world)
         indent_num = indent
         possible = self.model_structure.model_setup.possible
         z3_model = self.model_structure.z3_model
         ver_prints = '∅'
         ver_states = {
             bitvec_to_substates(bit, N)
             for bit in self["verifiers"]
@@ -562,20 +538,14 @@
             f"  ({truth_value} in {world_state})",
             file=output,
         )
 
     def truth_value_at(self, eval_world):
         '''Given a world, returns the truth value of the Proposition at that world.
         Used in print_verifiers_and_falsifiers.'''
-        prefix_expr = self['prefix expression']
-        if is_counterfactual(prefix_expr):
-            return True if eval_world in self['worlds cf true at'] else False
-        # if is_modal(prefix_expr):
-        #     return True if self["verifiers"] else False
-         # else case: extensional. Last to be computationally efficient (see def of is_extensional)
         for verifier in self["verifiers"]:
             if bit_part(verifier, eval_world):
                 return True
         return False
 
 
 def make_model_for(N, premises, conclusions):
```

### Comparing `model_checker-0.3.5/src/model_checker/semantics.py` & `model_checker-0.3.6/src/model_checker/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.5/src/model_checker/syntax.py` & `model_checker-0.3.6/src/model_checker/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.5/src/model_checker/temp.py` & `model_checker-0.3.6/src/model_checker/temp.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.5/src/model_checker/test.py` & `model_checker-0.3.6/src/model_checker/test.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.5/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.3.6/src/model_checker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.5
+Version: 0.3.6
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
@@ -60,21 +60,25 @@
 Fusions are printed using `.` so that `a.b` is the fusion of the states `a` and `b`.
 A state `a` is _part_ of a state `b` just in case `a.b = b`.
 States may be either _possible_ or _impossible_ where the null state is required to be possible and every part of a possible state is possible.
 The states `a` and `b` are _compatible_ just in case `a.b` is possible.
 A _world state_ is any state that is both possible and includes every compatible state as a part.
 
 Sentences are assigned _verifier states_ and _falsifier states_ where the both the verifiers and falsifiers are required to be closed under fusion.
+A sentence is _true at_ a world state `w` just in case `w` includes a verifier for that sentence as a part and _false at_ `w` just in case `w` includes a falsifier for that sentence as a part.
 In order to ensure that sentence letters have at most one truth-value at each world state, a fusion `a.b` is required to be impossible whenever `a` is verifier for a sentence letter `A` and `b` is a falsifier for `A`.
 Additionally, sentence letters have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
-These definitions were originally provided in [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 
 Negated sentences are verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
 Conjunctions are verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
-Conjunction and disjunction are dual operators obeying the standard De Morgan laws.
-The absorption laws do not hold, nor does conjunction distribute over disjunction, or _vice versa_.
-True counterfactual and modal sentences are verified by the null state and falsified by no states.
+Conjunction and disjunction are dual operators obeying the standard idempotent and De Morgan laws.
+The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
+For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
+
+A modal sentence `Box A` is true at a world just in case every world state includes a part that verifies `A`, where `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
+Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include `s` along with a maximal part of `w` that is compatible with `s` as parts.
+A counterfactual conditional sentences `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
 
-The semantic theory for counterfactual conditionals is motivated and further elaborated in this [manuscript](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
-For the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
+The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
+This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
 More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker).
```

### Comparing `model_checker-0.3.5/src/model_checker.egg-info/SOURCES.txt` & `model_checker-0.3.6/src/model_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/casepy-0.0.6.tar.gz` & `tmp/casepy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casepy-0.0.6.tar", last modified: Sat Apr 20 07:19:00 2024, max compression
+gzip compressed data, was "casepy-0.0.7.tar", last modified: Mon May 20 03:02:00 2024, max compression
```

## Comparing `casepy-0.0.6.tar` & `casepy-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:19:00.323166 casepy-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-20 07:18:49.000000 casepy-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-20 07:19:00.323166 casepy-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-20 07:18:49.000000 casepy-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 07:19:00.323166 casepy-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-20 07:18:49.000000 casepy-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:19:00.323166 casepy-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:19:00.323166 casepy-0.0.6/src/casepy/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 07:18:49.000000 casepy-0.0.6/src/casepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-20 07:18:49.000000 casepy-0.0.6/src/casepy/combination_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-20 07:18:49.000000 casepy-0.0.6/src/casepy/permutation_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-20 07:18:49.000000 casepy-0.0.6/src/casepy/simple_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 07:19:00.323166 casepy-0.0.6/src/casepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-20 07:19:00.000000 casepy-0.0.6/src/casepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-20 07:19:00.000000 casepy-0.0.6/src/casepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 07:19:00.000000 casepy-0.0.6/src/casepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 07:19:00.000000 casepy-0.0.6/src/casepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:02:00.324767 casepy-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 03:01:53.000000 casepy-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-20 03:02:00.324767 casepy-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-20 03:01:53.000000 casepy-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 03:02:00.324767 casepy-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-20 03:01:53.000000 casepy-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:02:00.320767 casepy-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:02:00.324767 casepy-0.0.7/src/casepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/combination_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/permutation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/simple_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 03:01:53.000000 casepy-0.0.7/src/casepy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:02:00.324767 casepy-0.0.7/src/casepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-20 03:02:00.000000 casepy-0.0.7/src/casepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-20 03:02:00.000000 casepy-0.0.7/src/casepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:02:00.000000 casepy-0.0.7/src/casepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 03:02:00.000000 casepy-0.0.7/src/casepy.egg-info/top_level.txt
```

### Comparing `casepy-0.0.6/LICENSE` & `casepy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `casepy-0.0.6/PKG-INFO` & `casepy-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -20,16 +20,17 @@
     - Generator Core class for combination
 - PermutationGenerator
     - Generator Core class for permutation
 
 - set_parameters(a, b)
     - initialize generator with essential parameters
     - a: number of element to select (ex: 3)
-    - b: list of element (ex: [1,2,3,4,5])
-- set_must_have_elements(list)
+    - b: list of element - duplication is ok (ex: [1,2,3,4,4,5]) 
+
+- ~~set_must_have_elements(list)~~
     - set elements that should be included in results.
     - list: list of necessary elements.
     - ex) set_must_have_elements([2,5]) -> all results will include 2 and 5; in PermutationGenerator, the order will be kept.
 
 - all_case
     - return list of all possible combinations based on the parameters.
 - random_case
```

### Comparing `casepy-0.0.6/README.md` & `casepy-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,17 @@
     - Generator Core class for combination
 - PermutationGenerator
     - Generator Core class for permutation
 
 - set_parameters(a, b)
     - initialize generator with essential parameters
     - a: number of element to select (ex: 3)
-    - b: list of element (ex: [1,2,3,4,5])
-- set_must_have_elements(list)
+    - b: list of element - duplication is ok (ex: [1,2,3,4,4,5]) 
+
+- ~~set_must_have_elements(list)~~
     - set elements that should be included in results.
     - list: list of necessary elements.
     - ex) set_must_have_elements([2,5]) -> all results will include 2 and 5; in PermutationGenerator, the order will be kept.
 
 - all_case
     - return list of all possible combinations based on the parameters.
 - random_case
```

### Comparing `casepy-0.0.6/src/casepy/combination_generator.py` & `casepy-0.0.7/src/casepy/combination_generator.py`

 * *Files identical despite different names*

### Comparing `casepy-0.0.6/src/casepy.egg-info/PKG-INFO` & `casepy-0.0.7/src/casepy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -20,16 +20,17 @@
     - Generator Core class for combination
 - PermutationGenerator
     - Generator Core class for permutation
 
 - set_parameters(a, b)
     - initialize generator with essential parameters
     - a: number of element to select (ex: 3)
-    - b: list of element (ex: [1,2,3,4,5])
-- set_must_have_elements(list)
+    - b: list of element - duplication is ok (ex: [1,2,3,4,4,5]) 
+
+- ~~set_must_have_elements(list)~~
     - set elements that should be included in results.
     - list: list of necessary elements.
     - ex) set_must_have_elements([2,5]) -> all results will include 2 and 5; in PermutationGenerator, the order will be kept.
 
 - all_case
     - return list of all possible combinations based on the parameters.
 - random_case
```


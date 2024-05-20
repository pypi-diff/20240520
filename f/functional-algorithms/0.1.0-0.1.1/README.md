# Comparing `tmp/functional_algorithms-0.1.0.tar.gz` & `tmp/functional_algorithms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functional_algorithms-0.1.0.tar", last modified: Sun May 19 18:05:47 2024, max compression
+gzip compressed data, was "functional_algorithms-0.1.1.tar", last modified: Mon May 20 10:53:23 2024, max compression
```

## Comparing `functional_algorithms-0.1.0.tar` & `functional_algorithms-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.740001 functional_algorithms-0.1.0/.github/
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.744001 functional_algorithms-0.1.0/.github/workflows/
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     1301 2024-05-17 13:31:35.000000 functional_algorithms-0.1.0/.github/workflows/python-package.yml
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     1084 2024-05-17 13:22:10.000000 functional_algorithms-0.1.0/.github/workflows/python-publish.yml
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     3081 2024-05-15 13:29:49.000000 functional_algorithms-0.1.0/.gitignore
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     1501 2024-05-13 19:31:52.000000 functional_algorithms-0.1.0/LICENSE
--rw-r--r--   0 pearu     (1000) pearu     (1000)    14605 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/PKG-INFO
--rw-rw-r--   0 pearu     (1000) pearu     (1000)    11930 2024-05-17 13:16:42.000000 functional_algorithms-0.1.0/README.md
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.744001 functional_algorithms-0.1.0/functional_algorithms/
--rw-rw-r--   0 pearu     (1000) pearu     (1000)      328 2024-05-15 09:45:05.000000 functional_algorithms-0.1.0/functional_algorithms/__init__.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)      411 2024-05-19 18:05:47.000000 functional_algorithms-0.1.0/functional_algorithms/_version.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)    10546 2024-05-17 13:12:10.000000 functional_algorithms-0.1.0/functional_algorithms/algorithms.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)    12664 2024-05-17 13:22:44.000000 functional_algorithms-0.1.0/functional_algorithms/context.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)    18655 2024-05-15 09:45:06.000000 functional_algorithms-0.1.0/functional_algorithms/expr.py
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.744001 functional_algorithms-0.1.0/functional_algorithms/targets/
--rw-rw-r--   0 pearu     (1000) pearu     (1000)       39 2024-05-15 10:08:50.000000 functional_algorithms-0.1.0/functional_algorithms/targets/__init__.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     7385 2024-05-17 13:03:43.000000 functional_algorithms-0.1.0/functional_algorithms/targets/numpy.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     5219 2024-05-15 13:37:59.000000 functional_algorithms-0.1.0/functional_algorithms/targets/python.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     6113 2024-05-16 14:44:46.000000 functional_algorithms-0.1.0/functional_algorithms/targets/stablehlo.py
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/functional_algorithms/tests/
--rw-rw-r--   0 pearu     (1000) pearu     (1000)       87 2024-05-15 09:47:37.000000 functional_algorithms-0.1.0/functional_algorithms/tests/__init__.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     3051 2024-05-15 10:14:47.000000 functional_algorithms-0.1.0/functional_algorithms/tests/test_algorithms.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)      161 2024-05-15 09:45:05.000000 functional_algorithms-0.1.0/functional_algorithms/tests/test_context.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)      205 2024-05-15 09:45:05.000000 functional_algorithms-0.1.0/functional_algorithms/tests/test_expr.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     4627 2024-05-15 20:20:30.000000 functional_algorithms-0.1.0/functional_algorithms/tests/test_functional_algorithms.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     9217 2024-05-15 09:45:05.000000 functional_algorithms-0.1.0/functional_algorithms/tests/test_utils.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     3037 2024-05-15 09:45:05.000000 functional_algorithms-0.1.0/functional_algorithms/typesystem.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)    22211 2024-05-19 15:56:00.000000 functional_algorithms-0.1.0/functional_algorithms/utils.py
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/functional_algorithms.egg-info/
--rw-r--r--   0 pearu     (1000) pearu     (1000)    14605 2024-05-19 18:05:47.000000 functional_algorithms-0.1.0/functional_algorithms.egg-info/PKG-INFO
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     1268 2024-05-19 18:05:47.000000 functional_algorithms-0.1.0/functional_algorithms.egg-info/SOURCES.txt
--rw-rw-r--   0 pearu     (1000) pearu     (1000)        1 2024-05-19 18:05:47.000000 functional_algorithms-0.1.0/functional_algorithms.egg-info/dependency_links.txt
--rw-rw-r--   0 pearu     (1000) pearu     (1000)       73 2024-05-19 18:05:47.000000 functional_algorithms-0.1.0/functional_algorithms.egg-info/requires.txt
--rw-rw-r--   0 pearu     (1000) pearu     (1000)       22 2024-05-19 18:05:47.000000 functional_algorithms-0.1.0/functional_algorithms.egg-info/top_level.txt
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     1479 2024-05-17 13:30:57.000000 functional_algorithms-0.1.0/pyproject.toml
--rw-rw-r--   0 pearu     (1000) pearu     (1000)       19 2024-05-17 13:27:41.000000 functional_algorithms-0.1.0/requirements.txt
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/results/
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/results/numpy/
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     9660 2024-05-17 13:02:08.000000 functional_algorithms-0.1.0/results/numpy/asin.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     1855 2024-05-15 13:38:02.000000 functional_algorithms-0.1.0/results/numpy/hypot.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     1984 2024-05-17 13:02:08.000000 functional_algorithms-0.1.0/results/numpy/square.py
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/results/python/
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     3070 2024-05-15 13:38:02.000000 functional_algorithms-0.1.0/results/python/asin.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)      472 2024-05-15 13:38:02.000000 functional_algorithms-0.1.0/results/python/hypot.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)      428 2024-05-15 13:38:02.000000 functional_algorithms-0.1.0/results/python/square.py
-drwxrwxr-x   0 pearu     (1000) pearu     (1000)        0 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/results/stablehlo/
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     8298 2024-05-17 13:02:08.000000 functional_algorithms-0.1.0/results/stablehlo/asin.td
--rw-rw-r--   0 pearu     (1000) pearu     (1000)      835 2024-05-15 20:10:57.000000 functional_algorithms-0.1.0/results/stablehlo/hypot.td
--rw-rw-r--   0 pearu     (1000) pearu     (1000)      810 2024-05-15 20:10:57.000000 functional_algorithms-0.1.0/results/stablehlo/square.td
--rw-rw-r--   0 pearu     (1000) pearu     (1000)     1844 2024-05-17 13:06:05.000000 functional_algorithms-0.1.0/results/update.py
--rw-rw-r--   0 pearu     (1000) pearu     (1000)       38 2024-05-19 18:05:47.748001 functional_algorithms-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.559147 functional_algorithms-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.559147 functional_algorithms-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/functional_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18655 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/expr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/functional_algorithms/targets/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/targets/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/targets/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/targets/stablehlo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/functional_algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_functional_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/typesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22211 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/functional_algorithms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/functional_algorithms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 10:53:23.000000 functional_algorithms-0.1.1/functional_algorithms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/results/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/numpy/asin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/numpy/hypot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/numpy/square.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.563147 functional_algorithms-0.1.1/results/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/python/asin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/python/hypot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/python/square.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/results/stablehlo/
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/stablehlo/asin.td
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/stablehlo/hypot.td
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/stablehlo/square.td
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-20 10:53:13.000000 functional_algorithms-0.1.1/results/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:53:23.567147 functional_algorithms-0.1.1/setup.cfg
```

### Comparing `functional_algorithms-0.1.0/.github/workflows/python-package.yml` & `functional_algorithms-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/.github/workflows/python-publish.yml` & `functional_algorithms-0.1.1/.github/workflows/python-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install build
+        pip install build setuptools_scm
+        python -c "from setuptools_scm import get_version;print('SETUPTOOLS_SCM_PRETEND_VERSION_FUNCTIONAL_ALGORITHMS='+get_version())" >> $GITHUB_ENV
     - name: Build package
-      run: python -m build
+      run: |
+        python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `functional_algorithms-0.1.0/.gitignore` & `functional_algorithms-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/LICENSE` & `functional_algorithms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/PKG-INFO` & `functional_algorithms-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional_algorithms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functional algorithms and implementations
 Author-email: Pearu Peterson <pearu.peterson@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Pearu Peterson
         
         Redistribution and use in source and binary forms, with or without
@@ -72,27 +72,29 @@
 whole complex plane or real line.
 
 The motivation for this project raises from the need to implement
 sophisticated algorithms for various math libraries that otherwise can
 be a tedious and errorprone task when done manually using LISP-like
 languages. For instance, the definition of the algorithm for computing
 arcus sine for Python or NumPy target has LOC about 45 but for the
-StableHLO target the LOC is 186. Implementing such an algorithm for
-StableHLO by hand would be just unhuman.
+StableHLO target the LOC is 186. Implementing arcus sine algorithm for
+StableHLO by hand would be very hard.
 
 
 ## Supported algorithms
 
 Currently, [the definitions of
 algorithms](functional_algorithms/algorithms.py) are provided for the
 following math functions:
 
 - `square(z: complex | float)`
 - `hypot(x: float, y: float)`
-- `asin(z: complex)`, using modified [Hull et al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm.
+- `asin(z: complex | float)`, using modified [Hull et
+  al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm for
+  complex `asin`.
 
 ## Supported targets
 
 Currently, the implementations of supported algorithms are provided
 for the following [target libraries and languages](functional_algorithms/targets/):
 
 - [Python](https://www.python.org/), using [math](https://docs.python.org/3/library/math.html) functions on real inputs
```

### Comparing `functional_algorithms-0.1.0/README.md` & `functional_algorithms-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,29 @@
 whole complex plane or real line.
 
 The motivation for this project raises from the need to implement
 sophisticated algorithms for various math libraries that otherwise can
 be a tedious and errorprone task when done manually using LISP-like
 languages. For instance, the definition of the algorithm for computing
 arcus sine for Python or NumPy target has LOC about 45 but for the
-StableHLO target the LOC is 186. Implementing such an algorithm for
-StableHLO by hand would be just unhuman.
+StableHLO target the LOC is 186. Implementing arcus sine algorithm for
+StableHLO by hand would be very hard.
 
 
 ## Supported algorithms
 
 Currently, [the definitions of
 algorithms](functional_algorithms/algorithms.py) are provided for the
 following math functions:
 
 - `square(z: complex | float)`
 - `hypot(x: float, y: float)`
-- `asin(z: complex)`, using modified [Hull et al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm.
+- `asin(z: complex | float)`, using modified [Hull et
+  al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm for
+  complex `asin`.
 
 ## Supported targets
 
 Currently, the implementations of supported algorithms are provided
 for the following [target libraries and languages](functional_algorithms/targets/):
 
 - [Python](https://www.python.org/), using [math](https://docs.python.org/3/library/math.html) functions on real inputs
```

### Comparing `functional_algorithms-0.1.0/functional_algorithms/algorithms.py` & `functional_algorithms-0.1.1/functional_algorithms/algorithms.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/context.py` & `functional_algorithms-0.1.1/functional_algorithms/context.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/expr.py` & `functional_algorithms-0.1.1/functional_algorithms/expr.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/targets/numpy.py` & `functional_algorithms-0.1.1/functional_algorithms/targets/numpy.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/targets/python.py` & `functional_algorithms-0.1.1/functional_algorithms/targets/python.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/targets/stablehlo.py` & `functional_algorithms-0.1.1/functional_algorithms/targets/stablehlo.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,31 @@
 
 from . import stablehlo as this_module
 
 source_file_header = ""
 
 
 trace_arguments = dict(
-    asin=[(":complex",)],
+    asin=[(":float",), (":complex",)],
     hypot=[(":float", ":float")],
     square=[(":float",), (":complex",)],
 )
 
 
 source_file_extension = ".td"
 
 
 def make_comment(message):
-    return "// " + "\n// ".join(message.splitlines()) + "\n"
+    lst = []
+    for line in message.splitlines():
+        if line.strip():
+            lst.append("// " + line)
+        else:
+            lst.append("//")
+    return "\n".join(lst) + "\n"
 
 
 kind_to_target = dict(
     abs="StableHLO_AbsOp",
     negative="StableHLO_NegOp",
     positive="StableHLO_PosOp",
     add="StableHLO_AddOp",
```

### Comparing `functional_algorithms-0.1.0/functional_algorithms/tests/test_algorithms.py` & `functional_algorithms-0.1.1/functional_algorithms/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/tests/test_functional_algorithms.py` & `functional_algorithms-0.1.1/functional_algorithms/tests/test_functional_algorithms.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/tests/test_utils.py` & `functional_algorithms-0.1.1/functional_algorithms/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/typesystem.py` & `functional_algorithms-0.1.1/functional_algorithms/typesystem.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms/utils.py` & `functional_algorithms-0.1.1/functional_algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/functional_algorithms.egg-info/PKG-INFO` & `functional_algorithms-0.1.1/functional_algorithms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: functional_algorithms
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functional algorithms and implementations
 Author-email: Pearu Peterson <pearu.peterson@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Pearu Peterson
         
         Redistribution and use in source and binary forms, with or without
@@ -72,27 +72,29 @@
 whole complex plane or real line.
 
 The motivation for this project raises from the need to implement
 sophisticated algorithms for various math libraries that otherwise can
 be a tedious and errorprone task when done manually using LISP-like
 languages. For instance, the definition of the algorithm for computing
 arcus sine for Python or NumPy target has LOC about 45 but for the
-StableHLO target the LOC is 186. Implementing such an algorithm for
-StableHLO by hand would be just unhuman.
+StableHLO target the LOC is 186. Implementing arcus sine algorithm for
+StableHLO by hand would be very hard.
 
 
 ## Supported algorithms
 
 Currently, [the definitions of
 algorithms](functional_algorithms/algorithms.py) are provided for the
 following math functions:
 
 - `square(z: complex | float)`
 - `hypot(x: float, y: float)`
-- `asin(z: complex)`, using modified [Hull et al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm.
+- `asin(z: complex | float)`, using modified [Hull et
+  al](https://dl.acm.org/doi/10.1145/275323.275324) algorithm for
+  complex `asin`.
 
 ## Supported targets
 
 Currently, the implementations of supported algorithms are provided
 for the following [target libraries and languages](functional_algorithms/targets/):
 
 - [Python](https://www.python.org/), using [math](https://docs.python.org/3/library/math.html) functions on real inputs
```

### Comparing `functional_algorithms-0.1.0/functional_algorithms.egg-info/SOURCES.txt` & `functional_algorithms-0.1.1/functional_algorithms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/pyproject.toml` & `functional_algorithms-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/results/numpy/asin.py` & `functional_algorithms-0.1.1/results/numpy/asin.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/results/numpy/hypot.py` & `functional_algorithms-0.1.1/results/numpy/hypot.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/results/numpy/square.py` & `functional_algorithms-0.1.1/results/numpy/square.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/results/python/asin.py` & `functional_algorithms-0.1.1/results/python/asin.py`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/results/stablehlo/asin.td` & `functional_algorithms-0.1.1/results/stablehlo/asin.td`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 // This file is generated using functional_algorithms tool (0.1.dev6+g8b58236), see
 //   https://github.com/pearu/functional_algorithms
 // for more information.
 
 
 
 
-def : Pat<(asin_0 ComplexElementType:$z),
+def : Pat<(asin_0 NonComplexElementType:$z),
+  (StableHLO_MulOp
+    (StableHLO_ConstantLike<"2"> $z),
+    (StableHLO_Atan2Op
+      $z,
+      (StableHLO_AddOp
+        (StableHLO_ConstantLike<"1">:$constant_1 $z),
+        (StableHLO_SqrtOp
+          (StableHLO_SubtractOp
+            $constant_1,
+            (StableHLO_MulOp $z, $z))))))>;
+
+def : Pat<(asin_1 ComplexElementType:$z),
   (StableHLO_ComplexOp
     (StableHLO_Atan2Op:$real
       (StableHLO_RealOp:$signed_x $z),
       (StableHLO_SelectOp
         (StableHLO_CompareOp
          (StableHLO_MaxOp
            (StableHLO_AbsOp:$x $signed_x),
```

### Comparing `functional_algorithms-0.1.0/results/stablehlo/hypot.td` & `functional_algorithms-0.1.1/results/stablehlo/hypot.td`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/results/stablehlo/square.td` & `functional_algorithms-0.1.1/results/stablehlo/square.td`

 * *Files identical despite different names*

### Comparing `functional_algorithms-0.1.0/results/update.py` & `functional_algorithms-0.1.1/results/update.py`

 * *Files identical despite different names*


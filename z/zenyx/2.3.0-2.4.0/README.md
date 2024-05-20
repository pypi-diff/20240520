# Comparing `tmp/zenyx-2.3.0.tar.gz` & `tmp/zenyx-2.4.0.tar.gz`

## Comparing `zenyx-2.3.0.tar` & `zenyx-2.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 zenyx-2.3.0/.editorconfig
--rw-r--r--   0        0        0   641847 2020-02-02 00:00:00.000000 zenyx-2.3.0/pyon.debug.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zenyx-2.3.0/requirements.txt
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 zenyx-2.3.0/src/zenyx/__init__.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 zenyx-2.3.0/src/zenyx/args.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 zenyx-2.3.0/src/zenyx/console.py
--rw-r--r--   0        0        0    15148 2020-02-02 00:00:00.000000 zenyx-2.3.0/src/zenyx/pyon.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 zenyx-2.3.0/src/zenyx/require.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 zenyx-2.3.0/src/zenyx/streams.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zenyx-2.3.0/tests/databank.py
--rw-r--r--   0        0        0   144790 2020-02-02 00:00:00.000000 zenyx-2.3.0/tests/pyon.debug.md
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 zenyx-2.3.0/tests/test_main.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zenyx-2.3.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 zenyx-2.3.0/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zenyx-2.3.0/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 zenyx-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 zenyx-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 zenyx-2.4.0/.editorconfig
+-rw-r--r--   0        0        0   641847 2020-02-02 00:00:00.000000 zenyx-2.4.0/pyon.debug.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zenyx-2.4.0/requirements.txt
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 zenyx-2.4.0/src/zenyx/__init__.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 zenyx-2.4.0/src/zenyx/args.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 zenyx-2.4.0/src/zenyx/console.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 zenyx-2.4.0/src/zenyx/pipe.py
+-rw-r--r--   0        0        0    15148 2020-02-02 00:00:00.000000 zenyx-2.4.0/src/zenyx/pyon.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 zenyx-2.4.0/src/zenyx/require.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 zenyx-2.4.0/src/zenyx/streams.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zenyx-2.4.0/tests/databank.py
+-rw-r--r--   0        0        0   144790 2020-02-02 00:00:00.000000 zenyx-2.4.0/tests/pyon.debug.md
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 zenyx-2.4.0/tests/test_main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zenyx-2.4.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 zenyx-2.4.0/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zenyx-2.4.0/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 zenyx-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 zenyx-2.4.0/PKG-INFO
```

### Comparing `zenyx-2.3.0/pyon.debug.md` & `zenyx-2.4.0/pyon.debug.md`

 * *Files identical despite different names*

### Comparing `zenyx-2.3.0/src/zenyx/__init__.py` & `zenyx-2.4.0/src/zenyx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 - `printf.endl(<amount = 0>)` -> An easy way to print multiple `\n`s
 - `printf.title(<content>, <line_char>)` -> Prints the title to the middle of the console using the line_char as the spacing chartacter
 """
 
 from zenyx import pyon, require, streams
 from zenyx.console import printf
 from zenyx.args import Arguments
-
+from zenyx.pipe import Pipe
```

### Comparing `zenyx-2.3.0/src/zenyx/args.py` & `zenyx-2.4.0/src/zenyx/args.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.3.0/src/zenyx/console.py` & `zenyx-2.4.0/src/zenyx/console.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.3.0/src/zenyx/pyon.py` & `zenyx-2.4.0/src/zenyx/pyon.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.3.0/src/zenyx/require.py` & `zenyx-2.4.0/src/zenyx/require.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.3.0/src/zenyx/streams.py` & `zenyx-2.4.0/src/zenyx/streams.py`

 * *Files identical despite different names*

### Comparing `zenyx-2.3.0/tests/pyon.debug.md` & `zenyx-2.4.0/tests/pyon.debug.md`

 * *Files identical despite different names*

### Comparing `zenyx-2.3.0/LICENSE` & `zenyx-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zenyx-2.3.0/pyproject.toml` & `zenyx-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zenyx"
-version = "2.3.0"
+version = "2.4.0"
 authors = [
   { name="zewenn", email="zc.fallens@gamil.com" },
 ]
 description = "A multitool python object notation package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


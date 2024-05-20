# Comparing `tmp/apertium_lint-1.0.7.tar.gz` & `tmp/apertium_lint-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apertium_lint-1.0.7.tar", last modified: Sat Jan  6 19:22:57 2024, max compression
+gzip compressed data, was "apertium_lint-1.0.8.tar", last modified: Mon May 20 20:48:01 2024, max compression
```

## Comparing `apertium_lint-1.0.7.tar` & `apertium_lint-1.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-01-06 19:22:57.554036 apertium_lint-1.0.7/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2021-03-01 02:56:44.000000 apertium_lint-1.0.7/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1820 2024-01-06 19:22:57.554036 apertium_lint-1.0.7/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1441 2022-12-27 16:33:47.000000 apertium_lint-1.0.7/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-01-06 19:22:57.546036 apertium_lint-1.0.7/apertium_lint/
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)     4427 2024-01-06 19:21:49.000000 apertium_lint-1.0.7/apertium_lint/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9231 2023-03-15 16:13:32.000000 apertium_lint-1.0.7/apertium_lint/file_linter.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-01-06 19:22:57.550036 apertium_lint-1.0.7/apertium_lint/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1573 2022-12-23 17:14:07.000000 apertium_lint-1.0.7/apertium_lint/tests/base.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      275 2022-12-23 17:32:13.000000 apertium_lint-1.0.7/apertium_lint/tests/test_cg.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      336 2023-07-18 18:45:04.000000 apertium_lint-1.0.7/apertium_lint/tests/test_lexc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      901 2024-01-03 04:20:49.000000 apertium_lint-1.0.7/apertium_lint/tests/test_lexd.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      460 2022-12-23 17:32:19.000000 apertium_lint-1.0.7/apertium_lint/tests/test_modes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      444 2022-12-23 17:29:39.000000 apertium_lint-1.0.7/apertium_lint/tests/test_rtx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1661 2022-12-23 17:32:28.000000 apertium_lint-1.0.7/apertium_lint/tests/test_transfer.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      392 2023-03-15 16:13:16.000000 apertium_lint-1.0.7/apertium_lint/tests/test_twolc.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-01-06 19:22:57.554036 apertium_lint-1.0.7/apertium_lint/tree_sitter/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/tree_sitter/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1240 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/tree_sitter/cg.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6934 2023-07-18 18:56:48.000000 apertium_lint-1.0.7/apertium_lint/tree_sitter/lexc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6150 2024-01-03 04:22:33.000000 apertium_lint-1.0.7/apertium_lint/tree_sitter/lexd.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4290 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/tree_sitter/rtx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1904 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/tree_sitter/tree_sitter_linter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6338 2023-03-15 16:13:36.000000 apertium_lint-1.0.7/apertium_lint/tree_sitter/twolc.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-01-06 19:22:57.554036 apertium_lint-1.0.7/apertium_lint/xml/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/xml/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10037 2023-04-02 20:54:00.000000 apertium_lint-1.0.7/apertium_lint/xml/dix.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3302 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/xml/lrx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2839 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/xml/modes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3249 2023-06-26 19:14:41.000000 apertium_lint-1.0.7/apertium_lint/xml/transfer.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1042 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/apertium_lint/xml/xml.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-01-06 19:22:57.554036 apertium_lint-1.0.7/apertium_lint.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1820 2024-01-06 19:22:57.000000 apertium_lint-1.0.7/apertium_lint.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1040 2024-01-06 19:22:57.000000 apertium_lint-1.0.7/apertium_lint.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-01-06 19:22:57.000000 apertium_lint-1.0.7/apertium_lint.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2024-01-06 19:22:57.000000 apertium_lint-1.0.7/apertium_lint.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       33 2024-01-06 19:22:57.000000 apertium_lint-1.0.7/apertium_lint.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2024-01-06 19:22:57.000000 apertium_lint-1.0.7/apertium_lint.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      546 2024-01-06 19:22:57.554036 apertium_lint-1.0.7/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2022-12-23 16:33:02.000000 apertium_lint-1.0.7/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-20 20:48:01.833427 apertium_lint-1.0.8/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2021-03-01 02:56:44.000000 apertium_lint-1.0.8/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1820 2024-05-20 20:48:01.833427 apertium_lint-1.0.8/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1441 2022-12-27 16:33:47.000000 apertium_lint-1.0.8/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-20 20:48:01.825426 apertium_lint-1.0.8/apertium_lint/
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)     4427 2024-01-06 19:21:49.000000 apertium_lint-1.0.8/apertium_lint/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9231 2024-05-20 20:46:37.000000 apertium_lint-1.0.8/apertium_lint/file_linter.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-20 20:48:01.829427 apertium_lint-1.0.8/apertium_lint/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1573 2022-12-23 17:14:07.000000 apertium_lint-1.0.8/apertium_lint/tests/base.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      275 2022-12-23 17:32:13.000000 apertium_lint-1.0.8/apertium_lint/tests/test_cg.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      336 2023-07-18 18:45:04.000000 apertium_lint-1.0.8/apertium_lint/tests/test_lexc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      901 2024-01-03 04:20:49.000000 apertium_lint-1.0.8/apertium_lint/tests/test_lexd.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      460 2022-12-23 17:32:19.000000 apertium_lint-1.0.8/apertium_lint/tests/test_modes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      444 2022-12-23 17:29:39.000000 apertium_lint-1.0.8/apertium_lint/tests/test_rtx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1661 2022-12-23 17:32:28.000000 apertium_lint-1.0.8/apertium_lint/tests/test_transfer.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      392 2023-03-15 16:13:16.000000 apertium_lint-1.0.8/apertium_lint/tests/test_twolc.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-20 20:48:01.829427 apertium_lint-1.0.8/apertium_lint/tree_sitter/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/tree_sitter/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1240 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/tree_sitter/cg.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6934 2023-07-18 18:56:48.000000 apertium_lint-1.0.8/apertium_lint/tree_sitter/lexc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6150 2024-01-03 04:22:33.000000 apertium_lint-1.0.8/apertium_lint/tree_sitter/lexd.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4290 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/tree_sitter/rtx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1904 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/tree_sitter/tree_sitter_linter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6338 2023-03-15 16:13:36.000000 apertium_lint-1.0.8/apertium_lint/tree_sitter/twolc.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-20 20:48:01.833427 apertium_lint-1.0.8/apertium_lint/xml/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/xml/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10037 2023-04-02 20:54:00.000000 apertium_lint-1.0.8/apertium_lint/xml/dix.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3302 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/xml/lrx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2839 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/xml/modes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5358 2024-05-20 20:45:14.000000 apertium_lint-1.0.8/apertium_lint/xml/transfer.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1042 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/apertium_lint/xml/xml.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-20 20:48:01.833427 apertium_lint-1.0.8/apertium_lint.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1820 2024-05-20 20:48:01.000000 apertium_lint-1.0.8/apertium_lint.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1040 2024-05-20 20:48:01.000000 apertium_lint-1.0.8/apertium_lint.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-20 20:48:01.000000 apertium_lint-1.0.8/apertium_lint.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2024-05-20 20:48:01.000000 apertium_lint-1.0.8/apertium_lint.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       33 2024-05-20 20:48:01.000000 apertium_lint-1.0.8/apertium_lint.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2024-05-20 20:48:01.000000 apertium_lint-1.0.8/apertium_lint.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      546 2024-05-20 20:48:01.833427 apertium_lint-1.0.8/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2022-12-23 16:33:02.000000 apertium_lint-1.0.8/setup.py
```

### Comparing `apertium_lint-1.0.7/LICENSE` & `apertium_lint-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/PKG-INFO` & `apertium_lint-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium_lint
-Version: 1.0.7
+Version: 1.0.8
 Summary: static analysis of Apertium files
 Home-page: http://github.com/apertium/apertium-lint
 Author: Daniel Swanson
 Author-email: apertium@dangswan.com
 License: GPLv3+
 Keywords: apertium,linter
 Description-Content-Type: text/markdown
```

### Comparing `apertium_lint-1.0.7/README.md` & `apertium_lint-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/__init__.py` & `apertium_lint-1.0.8/apertium_lint/__init__.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/file_linter.py` & `apertium_lint-1.0.8/apertium_lint/file_linter.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tests/base.py` & `apertium_lint-1.0.8/apertium_lint/tests/base.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tests/test_lexd.py` & `apertium_lint-1.0.8/apertium_lint/tests/test_lexd.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tests/test_transfer.py` & `apertium_lint-1.0.8/apertium_lint/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tree_sitter/cg.py` & `apertium_lint-1.0.8/apertium_lint/tree_sitter/cg.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tree_sitter/lexc.py` & `apertium_lint-1.0.8/apertium_lint/tree_sitter/lexc.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tree_sitter/lexd.py` & `apertium_lint-1.0.8/apertium_lint/tree_sitter/lexd.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tree_sitter/rtx.py` & `apertium_lint-1.0.8/apertium_lint/tree_sitter/rtx.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tree_sitter/tree_sitter_linter.py` & `apertium_lint-1.0.8/apertium_lint/tree_sitter/tree_sitter_linter.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/tree_sitter/twolc.py` & `apertium_lint-1.0.8/apertium_lint/tree_sitter/twolc.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/xml/dix.py` & `apertium_lint-1.0.8/apertium_lint/xml/dix.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/xml/lrx.py` & `apertium_lint-1.0.8/apertium_lint/xml/lrx.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/xml/modes.py` & `apertium_lint-1.0.8/apertium_lint/xml/modes.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint/xml/xml.py` & `apertium_lint-1.0.8/apertium_lint/xml/xml.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/apertium_lint.egg-info/PKG-INFO` & `apertium_lint-1.0.8/apertium_lint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium_lint
-Version: 1.0.7
+Version: 1.0.8
 Summary: static analysis of Apertium files
 Home-page: http://github.com/apertium/apertium-lint
 Author: Daniel Swanson
 Author-email: apertium@dangswan.com
 License: GPLv3+
 Keywords: apertium,linter
 Description-Content-Type: text/markdown
```

### Comparing `apertium_lint-1.0.7/apertium_lint.egg-info/SOURCES.txt` & `apertium_lint-1.0.8/apertium_lint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.7/setup.cfg` & `apertium_lint-1.0.8/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apertium_lint
-version = 1.0.7
+version = 1.0.8
 description = static analysis of Apertium files
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = apertium, linter
 license = GPLv3+
 license_files = LICENSE
 author = Daniel Swanson
```


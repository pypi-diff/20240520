# Comparing `tmp/tk_lint-0.1.0.tar.gz` & `tmp/tk_lint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tk_lint-0.1.0.tar", max compression
+gzip compressed data, was "tk_lint-0.1.1.tar", max compression
```

## Comparing `tk_lint-0.1.0.tar` & `tk_lint-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      525 2024-05-17 15:30:23.983137 tk_lint-0.1.0/README.md
--rw-r--r--   0        0        0      354 2024-05-17 11:45:42.092109 tk_lint-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 11:45:42.092462 tk_lint-0.1.0/tk_lint/__init__.py
--rw-r--r--   0        0        0      481 2024-05-17 15:30:23.983768 tk_lint-0.1.0/tk_lint/cli.py
--rw-r--r--   0        0        0      350 2024-05-17 15:30:23.984345 tk_lint-0.1.0/tk_lint/ruff.toml
--rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 tk_lint-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      525 2024-05-17 15:30:23.983137 tk_lint-0.1.1/README.md
+-rw-r--r--   0        0        0      368 2024-05-20 13:34:58.801167 tk_lint-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 11:45:42.092462 tk_lint-0.1.1/tk_lint/__init__.py
+-rw-r--r--   0        0        0      517 2024-05-20 13:34:21.750220 tk_lint-0.1.1/tk_lint/cli.py
+-rw-r--r--   0        0        0      350 2024-05-20 13:34:21.750520 tk_lint-0.1.1/tk_lint/config/ruff.toml
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 tk_lint-0.1.1/PKG-INFO
```

### Comparing `tk_lint-0.1.0/README.md` & `tk_lint-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tk_lint-0.1.0/PKG-INFO` & `tk_lint-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: tk-lint
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Eslam Odeh
 Author-email: eslamodeh@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: ruff (>=0,<1)
+Requires-Dist: ruff (<1)
+Requires-Dist: toml (<1)
 Description-Content-Type: text/markdown
 
 # TK Lint
 
 
 TK Lint is a package/CLI the includes different linting rules such as Ruff, MyPy, etc.. to be used as a standard across repositories. It's built using [poetry](https://python-poetry.org/)
```


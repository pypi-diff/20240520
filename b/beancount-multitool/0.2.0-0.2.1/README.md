# Comparing `tmp/beancount_multitool-0.2.0.tar.gz` & `tmp/beancount_multitool-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_multitool-0.2.0.tar", max compression
+gzip compressed data, was "beancount_multitool-0.2.1.tar", max compression
```

## Comparing `beancount_multitool-0.2.0.tar` & `beancount_multitool-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.2.0/LICENSE
--rw-r--r--   0        0        0     2498 2024-05-19 14:48:29.553748 beancount_multitool-0.2.0/README.md
--rw-r--r--   0        0        0     1183 2024-05-19 14:44:09.227258 beancount_multitool-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      152 2024-05-18 06:24:03.000000 beancount_multitool-0.2.0/src/beancount_multitool/Institution.py
--rw-r--r--   0        0        0     4777 2024-05-18 12:42:08.000000 beancount_multitool-0.2.0/src/beancount_multitool/JABank.py
--rw-r--r--   0        0        0     4022 2024-05-18 06:34:16.000000 beancount_multitool-0.2.0/src/beancount_multitool/RakutenBank.py
--rw-r--r--   0        0        0     3853 2024-05-18 08:40:03.000000 beancount_multitool-0.2.0/src/beancount_multitool/RakutenCard.py
--rw-r--r--   0        0        0     4683 2024-05-18 08:33:38.000000 beancount_multitool-0.2.0/src/beancount_multitool/ShinseiBank.py
--rw-r--r--   0        0        0      454 2024-05-19 14:27:19.202196 beancount_multitool-0.2.0/src/beancount_multitool/__init__.py
--rw-r--r--   0        0        0       89 2024-05-18 12:52:29.000000 beancount_multitool-0.2.0/src/beancount_multitool/__main__.py
--rw-r--r--   0        0        0       22 2024-05-19 14:44:02.886647 beancount_multitool-0.2.0/src/beancount_multitool/__version__.py
--rw-r--r--   0        0        0     1219 2024-05-17 14:23:38.000000 beancount_multitool-0.2.0/src/beancount_multitool/as_transaction.py
--rw-r--r--   0        0        0     1576 2024-05-19 14:38:01.059850 beancount_multitool-0.2.0/src/beancount_multitool/cli.py
--rw-r--r--   0        0        0      588 2024-05-18 08:03:00.000000 beancount_multitool-0.2.0/src/beancount_multitool/read_config.py
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 beancount_multitool-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2611 2024-05-19 15:16:51.720665 beancount_multitool-0.2.1/README.md
+-rw-r--r--   0        0        0     1183 2024-05-19 15:02:22.655285 beancount_multitool-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-05-18 06:24:03.000000 beancount_multitool-0.2.1/src/beancount_multitool/Institution.py
+-rw-r--r--   0        0        0     4777 2024-05-18 12:42:08.000000 beancount_multitool-0.2.1/src/beancount_multitool/JABank.py
+-rw-r--r--   0        0        0     4022 2024-05-18 06:34:16.000000 beancount_multitool-0.2.1/src/beancount_multitool/RakutenBank.py
+-rw-r--r--   0        0        0     3853 2024-05-18 08:40:03.000000 beancount_multitool-0.2.1/src/beancount_multitool/RakutenCard.py
+-rw-r--r--   0        0        0     4683 2024-05-18 08:33:38.000000 beancount_multitool-0.2.1/src/beancount_multitool/ShinseiBank.py
+-rw-r--r--   0        0        0      454 2024-05-19 14:27:19.202196 beancount_multitool-0.2.1/src/beancount_multitool/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-19 15:35:13.028794 beancount_multitool-0.2.1/src/beancount_multitool/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-19 15:02:27.855020 beancount_multitool-0.2.1/src/beancount_multitool/__version__.py
+-rw-r--r--   0        0        0     1219 2024-05-17 14:23:38.000000 beancount_multitool-0.2.1/src/beancount_multitool/as_transaction.py
+-rw-r--r--   0        0        0     1636 2024-05-19 15:23:56.461296 beancount_multitool-0.2.1/src/beancount_multitool/cli.py
+-rw-r--r--   0        0        0      588 2024-05-18 08:03:00.000000 beancount_multitool-0.2.1/src/beancount_multitool/read_config.py
+-rw-r--r--   0        0        0     3929 1970-01-01 00:00:00.000000 beancount_multitool-0.2.1/PKG-INFO
```

### Comparing `beancount_multitool-0.2.0/LICENSE` & `beancount_multitool-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.2.0/README.md` & `beancount_multitool-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Beancount Multitool
 
-![Tests badge](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml/badge.svg)
-![pypi version](https://img.shields.io/pypi/v/beancount-multitool
-)
-![python version required](https://img.shields.io/pypi/pyversions/beancount-multitool
-)
+[![Tests badge](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml/badge.svg)](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/beancount-multitool)](https://pypi.org/project/beancount-multitool/)
+![python version required](https://img.shields.io/pypi/pyversions/beancount-multitool)
 ![static coverage badge](https://img.shields.io/badge/Coverage-97%25-blue)
 
 Beancount Multitool is a command-line-interface (CLI) tool that converts financial data from financial institutions to Beancount files.
 
 The following institutions are supported:
 
 * Japan
@@ -72,22 +70,22 @@
 1. Download the raw CSV files from a financial institutions.
 2. Run `bean-mt`.
 3. Include the `output.bean` file in my ledger.
 4. Manually edit that Beancount file to my needs.
 
 config.toml:
 
-There is a default config.toml per financial institutions. Examples are in the test [data folder](./tests/data/).
+There is a default config.toml per financial institutions. Examples are in the test [data folder](tests/data).
 
 ## Requirements
 
 * Python 3.9 or higher.
 
 ## More
 
-* [Todo](./todo.md)
-* [Changelog](./changelog.md)
-* [Development](./development.md)
+* [Todo](todo.md)
+* [Changelog](changelog.md)
+* [Development](development.md)
 
 ## License
 
 MIT License
```

### Comparing `beancount_multitool-0.2.0/pyproject.toml` & `beancount_multitool-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-multitool"
-version = "0.2.0"
+version = "0.2.1"
 description = "A CLI tool that converts financial data to Beancount files"
 authors = ["Rick Lan <rlan@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rlan/beancount-multitool"
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `beancount_multitool-0.2.0/src/beancount_multitool/JABank.py` & `beancount_multitool-0.2.1/src/beancount_multitool/JABank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.2.0/src/beancount_multitool/RakutenBank.py` & `beancount_multitool-0.2.1/src/beancount_multitool/RakutenBank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.2.0/src/beancount_multitool/RakutenCard.py` & `beancount_multitool-0.2.1/src/beancount_multitool/RakutenCard.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.2.0/src/beancount_multitool/ShinseiBank.py` & `beancount_multitool-0.2.1/src/beancount_multitool/ShinseiBank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.2.0/src/beancount_multitool/as_transaction.py` & `beancount_multitool-0.2.1/src/beancount_multitool/as_transaction.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.2.0/src/beancount_multitool/cli.py` & `beancount_multitool-0.2.1/src/beancount_multitool/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-
 import click
+import sys
 
 # Get available finanicial institutions
 from beancount_multitool import __INSTITUTIONS__
 
 from beancount_multitool import JABank
 from beancount_multitool import RakutenBank
 from beancount_multitool import RakutenCard
@@ -38,7 +38,11 @@
         tool = RakutenBank(config)
     elif name == RakutenCard.NAME:
         tool = RakutenCard(config)
     elif name == ShinseiBank.NAME:
         tool = ShinseiBank(config)
 
     tool.convert(data, output)
+
+
+if __name__ == "__main__":
+    sys.exit(main())
```

### Comparing `beancount_multitool-0.2.0/src/beancount_multitool/read_config.py` & `beancount_multitool-0.2.1/src/beancount_multitool/read_config.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.2.0/PKG-INFO` & `beancount_multitool-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-multitool
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI tool that converts financial data to Beancount files
 Home-page: https://github.com/rlan/beancount-multitool
 License: MIT
 Author: Rick Lan
 Author-email: rlan@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -27,19 +27,17 @@
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/rlan/beancount-multitool
 Description-Content-Type: text/markdown
 
 # Beancount Multitool
 
-![Tests badge](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml/badge.svg)
-![pypi version](https://img.shields.io/pypi/v/beancount-multitool
-)
-![python version required](https://img.shields.io/pypi/pyversions/beancount-multitool
-)
+[![Tests badge](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml/badge.svg)](https://github.com/rlan/beancount-multitool/actions/workflows/tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/beancount-multitool)](https://pypi.org/project/beancount-multitool/)
+![python version required](https://img.shields.io/pypi/pyversions/beancount-multitool)
 ![static coverage badge](https://img.shields.io/badge/Coverage-97%25-blue)
 
 Beancount Multitool is a command-line-interface (CLI) tool that converts financial data from financial institutions to Beancount files.
 
 The following institutions are supported:
 
 * Japan
@@ -103,23 +101,23 @@
 1. Download the raw CSV files from a financial institutions.
 2. Run `bean-mt`.
 3. Include the `output.bean` file in my ledger.
 4. Manually edit that Beancount file to my needs.
 
 config.toml:
 
-There is a default config.toml per financial institutions. Examples are in the test [data folder](./tests/data/).
+There is a default config.toml per financial institutions. Examples are in the test [data folder](tests/data).
 
 ## Requirements
 
 * Python 3.9 or higher.
 
 ## More
 
-* [Todo](./todo.md)
-* [Changelog](./changelog.md)
-* [Development](./development.md)
+* [Todo](todo.md)
+* [Changelog](changelog.md)
+* [Development](development.md)
 
 ## License
 
 MIT License
```


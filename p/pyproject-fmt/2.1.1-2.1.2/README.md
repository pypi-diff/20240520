# Comparing `tmp/pyproject_fmt-2.1.1.tar.gz` & `tmp/pyproject_fmt-2.1.2.tar.gz`

## Comparing `pyproject_fmt-2.1.1.tar` & `pyproject_fmt-2.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/tox.ini
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/src/pyproject_fmt/__init__.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/src/pyproject_fmt/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/src/pyproject_fmt/_version.py
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/src/pyproject_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/src/pyproject_fmt/py.typed
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/tests/test_cli.py
--rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/tests/test_main.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/tests/test_pyproject_toml_fmt.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/LICENSE.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/README.md
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/tox.ini
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/src/pyproject_fmt/__init__.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/src/pyproject_fmt/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/src/pyproject_fmt/_version.py
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/src/pyproject_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/src/pyproject_fmt/py.typed
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/tests/test_cli.py
+-rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/tests/test_main.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/tests/test_pyproject_toml_fmt.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/README.md
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 pyproject_fmt-2.1.2/PKG-INFO
```

### Comparing `pyproject_fmt-2.1.1/tox.ini` & `pyproject_fmt-2.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.1.1/src/pyproject_fmt/__main__.py` & `pyproject_fmt-2.1.2/src/pyproject_fmt/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.1.1/src/pyproject_fmt/cli.py` & `pyproject_fmt-2.1.2/src/pyproject_fmt/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.1.1/tests/test_cli.py` & `pyproject_fmt-2.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.1.1/tests/test_main.py` & `pyproject_fmt-2.1.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.1.1/LICENSE.txt` & `pyproject_fmt-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.1.1/README.md` & `pyproject_fmt-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.1.1/pyproject.toml` & `pyproject_fmt-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "pyproject-fmt-rust==1.1.1",
+  "pyproject-fmt-rust==1.1.2",
   "tomli>=2.0.1; python_version<'3.11'",
 ]
 optional-dependencies.docs = [
   "furo>=2024.5.6",
   "sphinx>=7.3.7",
   "sphinx-argparse-cli>=1.15",
   "sphinx-autodoc-typehints>=2.1",
```

### Comparing `pyproject_fmt-2.1.1/PKG-INFO` & `pyproject_fmt-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt
-Version: 2.1.1
+Version: 2.1.2
 Summary: Format your pyproject.toml file
 Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt/issues
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt/releases
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a
@@ -33,15 +33,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: pyproject-fmt-rust==1.1.1
+Requires-Dist: pyproject-fmt-rust==1.1.2
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Provides-Extra: docs
 Requires-Dist: furo>=2024.5.6; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.15; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints>=2.1; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx>=7.3.7; extra == 'docs'
```


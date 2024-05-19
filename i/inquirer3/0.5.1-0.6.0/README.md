# Comparing `tmp/inquirer3-0.5.1.tar.gz` & `tmp/inquirer3-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inquirer3-0.5.1.tar", max compression
+gzip compressed data, was "inquirer3-0.6.0.tar", max compression
```

## Comparing `inquirer3-0.5.1.tar` & `inquirer3-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1090 2024-05-07 01:51:58.291837 inquirer3-0.5.1/LICENSE
--rw-r--r--   0        0        0     5331 2024-05-07 01:51:58.291837 inquirer3-0.5.1/README.md
--rw-r--r--   0        0        0     1878 2024-05-07 01:52:12.331941 inquirer3-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      974 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/__init__.py
--rw-r--r--   0        0        0      412 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/errors.py
--rw-r--r--   0        0        0      351 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/events.py
--rw-r--r--   0        0        0      439 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/prompt.py
--rw-r--r--   0        0        0    12339 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/questions.py
--rw-r--r--   0        0        0      315 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/__init__.py
--rw-r--r--   0        0        0     6678 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/__init__.py
--rw-r--r--   0        0        0     5368 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/_checkbox.py
--rw-r--r--   0        0        0      726 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/_confirm.py
--rw-r--r--   0        0        0     1091 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/_editor.py
--rw-r--r--   0        0        0     3550 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/_list.py
--rw-r--r--   0        0        0      103 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/_other.py
--rw-r--r--   0        0        0      382 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/_password.py
--rw-r--r--   0        0        0       77 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/_path.py
--rw-r--r--   0        0        0     2483 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/_text.py
--rw-r--r--   0        0        0     1314 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/render/console/base.py
--rw-r--r--   0        0        0     6034 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/shortcuts.py
--rw-r--r--   0        0        0     4484 2024-05-07 01:51:58.295837 inquirer3-0.5.1/src/inquirer3/themes.py
--rw-r--r--   0        0        0     6624 1970-01-01 00:00:00.000000 inquirer3-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-19 23:32:21.207370 inquirer3-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5269 2024-05-19 23:32:21.207370 inquirer3-0.6.0/README.md
+-rw-r--r--   0        0        0     1871 2024-05-19 23:32:30.095406 inquirer3-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      974 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/errors.py
+-rw-r--r--   0        0        0      351 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/events.py
+-rw-r--r--   0        0        0      439 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/prompt.py
+-rw-r--r--   0        0        0    12339 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/questions.py
+-rw-r--r--   0        0        0      315 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/__init__.py
+-rw-r--r--   0        0        0     6678 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/__init__.py
+-rw-r--r--   0        0        0     5368 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/_checkbox.py
+-rw-r--r--   0        0        0      726 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/_confirm.py
+-rw-r--r--   0        0        0     1066 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/_editor.py
+-rw-r--r--   0        0        0     3550 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/_list.py
+-rw-r--r--   0        0        0      103 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/_other.py
+-rw-r--r--   0        0        0      382 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/_password.py
+-rw-r--r--   0        0        0       77 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/_path.py
+-rw-r--r--   0        0        0     2483 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/_text.py
+-rw-r--r--   0        0        0     1314 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/render/console/base.py
+-rw-r--r--   0        0        0     6034 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/shortcuts.py
+-rw-r--r--   0        0        0     4484 2024-05-19 23:32:21.215370 inquirer3-0.6.0/src/inquirer3/themes.py
+-rw-r--r--   0        0        0     6555 1970-01-01 00:00:00.000000 inquirer3-0.6.0/PKG-INFO
```

### Comparing `inquirer3-0.5.1/LICENSE` & `inquirer3-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/README.md` & `inquirer3-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-[![PyPI](https://img.shields.io/pypi/v/inquirer3.svg)][pypi status]
-[![Status](https://img.shields.io/pypi/status/inquirer3.svg)][pypi status]
+<div align="center">
+
+[![PyPI](https://img.shields.io/pypi/v/inquirer3?&color=blue&logo=pypi&logoColor=%23FFFBEF)][pypi status]
+[![Downloads](https://static.pepy.tech/badge/inquirer3?color=green)][pypi downloads]
+[![Read the documentation at https://python-inquirer3.readthedocs.io/](https://img.shields.io/readthedocs/python-inquirer/latest.svg?label=docs)][read the docs]
+
+[![Tests](https://github.com/guysalt/python-inquirer3/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/guysalt/python-inquirer3/branch/main/graph/badge.svg)][codecov]
 [![Python Version](https://img.shields.io/pypi/pyversions/inquirer3.svg)][pypi status]
 [![License](https://img.shields.io/pypi/l/inquirer3.svg)][license]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
-<br>
-[![Read the documentation at https://python-inquirer3.readthedocs.io/](https://img.shields.io/readthedocs/python-inquirer/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/guysalt/python-inquirer3/workflows/Tests/badge.svg)][tests]
-[![Codecov](https://codecov.io/gh/guysalt/python-inquirer3/branch/main/graph/badge.svg)][codecov]
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 
 [pypi status]: https://pypi.org/project/inquirer3/
+[pypi downloads]: https://pepy.tech/project/inquirer3
 [read the docs]: https://python-inquirer3.readthedocs.io/
 [tests]: https://github.com/guysalt/python-inquirer3/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/guysalt/python-inquirer3
-[pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
+</div>
+
 # python-inquirer3
 
 This is a fork of [magmax/python-inquirer]. This one is hopefully more responsive (Issues/PRs/...).
 
 Collection of common interactive command line user interfaces, based on [magmax/python-inquirer].
 
 ### Goal and Philosophy
```

### Comparing `inquirer3-0.5.1/pyproject.toml` & `inquirer3-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inquirer3"
-version = "0.5.1"
+version = "0.6.0"
 description = "Collection of common interactive command line user interfaces, based on Inquirer.js"
 authors = ["Guy Salton <guy123121@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/guysalt/python-inquirer3"
 repository = "https://github.com/guysalt/python-inquirer3"
 documentation = "https://python-inquirer3.readthedocs.io/en/latest/"
@@ -23,15 +23,15 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 blessed = "^1.20.0"
 readchar = "^4.0.6"
-python-editor = "^1.0.4"
+editor = "^1.6.6"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.8"
 flake8 = "^7.0.0"
 flake8-docstrings = "^1.7.0"
 furo = "^2024.4.27"
 isort = "^5.13.2"
```

### Comparing `inquirer3-0.5.1/src/inquirer3/__init__.py` & `inquirer3-0.6.0/src/inquirer3/__init__.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/questions.py` & `inquirer3-0.6.0/src/inquirer3/questions.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/render/console/__init__.py` & `inquirer3-0.6.0/src/inquirer3/render/console/__init__.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/render/console/_checkbox.py` & `inquirer3-0.6.0/src/inquirer3/render/console/_checkbox.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/render/console/_confirm.py` & `inquirer3-0.6.0/src/inquirer3/render/console/_confirm.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/render/console/_editor.py` & `inquirer3-0.6.0/src/inquirer3/render/console/_editor.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,13 +24,13 @@
         return f"Entered value is not a valid {self.question.name}."
 
     def process_input(self, pressed):
         if pressed == key.CTRL_C:
             raise KeyboardInterrupt()
 
         if pressed in (key.CR, key.LF, key.ENTER):
-            data = editor.edit(contents=self.question.default or "")
-            raise errors.EndOfInput(data.decode("utf-8"))
+            data = editor(text=self.question.default or "")
+            raise errors.EndOfInput(data)
 
         raise errors.ValidationError(
             "You have pressed unknown key! " "Press <enter> to open editor or " "CTRL+C to exit."
         )
```

### Comparing `inquirer3-0.5.1/src/inquirer3/render/console/_list.py` & `inquirer3-0.6.0/src/inquirer3/render/console/_list.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/render/console/_text.py` & `inquirer3-0.6.0/src/inquirer3/render/console/_text.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/render/console/base.py` & `inquirer3-0.6.0/src/inquirer3/render/console/base.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/shortcuts.py` & `inquirer3-0.6.0/src/inquirer3/shortcuts.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/src/inquirer3/themes.py` & `inquirer3-0.6.0/src/inquirer3/themes.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.5.1/PKG-INFO` & `inquirer3-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inquirer3
-Version: 0.5.1
+Version: 0.6.0
 Summary: Collection of common interactive command line user interfaces, based on Inquirer.js
 Home-page: https://github.com/guysalt/python-inquirer3
 License: MIT
 Author: Guy Salton
 Author-email: guy123121@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,38 +17,41 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Dist: blessed (>=1.20.0,<2.0.0)
-Requires-Dist: python-editor (>=1.0.4,<2.0.0)
+Requires-Dist: editor (>=1.6.6,<2.0.0)
 Requires-Dist: readchar (>=4.0.6,<5.0.0)
 Project-URL: Documentation, https://python-inquirer3.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/guysalt/python-inquirer3
 Description-Content-Type: text/markdown
 
-[![PyPI](https://img.shields.io/pypi/v/inquirer3.svg)][pypi status]
-[![Status](https://img.shields.io/pypi/status/inquirer3.svg)][pypi status]
+<div align="center">
+
+[![PyPI](https://img.shields.io/pypi/v/inquirer3?&color=blue&logo=pypi&logoColor=%23FFFBEF)][pypi status]
+[![Downloads](https://static.pepy.tech/badge/inquirer3?color=green)][pypi downloads]
+[![Read the documentation at https://python-inquirer3.readthedocs.io/](https://img.shields.io/readthedocs/python-inquirer/latest.svg?label=docs)][read the docs]
+
+[![Tests](https://github.com/guysalt/python-inquirer3/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/guysalt/python-inquirer3/branch/main/graph/badge.svg)][codecov]
 [![Python Version](https://img.shields.io/pypi/pyversions/inquirer3.svg)][pypi status]
 [![License](https://img.shields.io/pypi/l/inquirer3.svg)][license]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
-<br>
-[![Read the documentation at https://python-inquirer3.readthedocs.io/](https://img.shields.io/readthedocs/python-inquirer/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/guysalt/python-inquirer3/workflows/Tests/badge.svg)][tests]
-[![Codecov](https://codecov.io/gh/guysalt/python-inquirer3/branch/main/graph/badge.svg)][codecov]
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 
 [pypi status]: https://pypi.org/project/inquirer3/
+[pypi downloads]: https://pepy.tech/project/inquirer3
 [read the docs]: https://python-inquirer3.readthedocs.io/
 [tests]: https://github.com/guysalt/python-inquirer3/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/guysalt/python-inquirer3
-[pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
+</div>
+
 # python-inquirer3
 
 This is a fork of [magmax/python-inquirer]. This one is hopefully more responsive (Issues/PRs/...).
 
 Collection of common interactive command line user interfaces, based on [magmax/python-inquirer].
 
 ### Goal and Philosophy
```


# Comparing `tmp/settngs-0.9.2.tar.gz` & `tmp/settngs-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "settngs-0.9.2.tar", last modified: Mon Dec 18 02:28:15 2023, max compression
+gzip compressed data, was "settngs-0.9.3.tar", last modified: Thu Feb 22 22:50:50 2024, max compression
```

## Comparing `settngs-0.9.2.tar` & `settngs-0.9.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:15.128903 settngs-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:15.124903 settngs-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:15.128903 settngs-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-18 02:28:00.000000 settngs-0.9.2/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-18 02:28:00.000000 settngs-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-12-18 02:28:00.000000 settngs-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-12-18 02:28:00.000000 settngs-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-12-18 02:28:15.128903 settngs-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-12-18 02:28:00.000000 settngs-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-18 02:28:00.000000 settngs-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 02:28:00.000000 settngs-0.9.2/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:15.128903 settngs-0.9.2/settngs/
--rw-r--r--   0 runner    (1001) docker     (127)    36349 2023-12-18 02:28:00.000000 settngs-0.9.2/settngs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-18 02:28:00.000000 settngs-0.9.2/settngs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:00.000000 settngs-0.9.2/settngs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:15.128903 settngs-0.9.2/settngs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-12-18 02:28:15.000000 settngs-0.9.2/settngs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-18 02:28:15.000000 settngs-0.9.2/settngs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 02:28:15.000000 settngs-0.9.2/settngs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-18 02:28:15.000000 settngs-0.9.2/settngs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-18 02:28:15.000000 settngs-0.9.2/settngs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2023-12-18 02:28:15.132903 settngs-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-18 02:28:00.000000 settngs-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:15.128903 settngs-0.9.2/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:00.000000 settngs-0.9.2/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2023-12-18 02:28:00.000000 settngs-0.9.2/testing/settngs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:15.128903 settngs-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:00.000000 settngs-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33588 2023-12-18 02:28:00.000000 settngs-0.9.2/tests/settngs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 02:28:15.128903 settngs-0.9.2/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-12-18 02:28:00.000000 settngs-0.9.2/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2023-12-18 02:28:00.000000 settngs-0.9.2/workflows/package.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:50.896527 settngs-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:50.892527 settngs-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:50.892527 settngs-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-22 22:50:39.000000 settngs-0.9.3/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-22 22:50:39.000000 settngs-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-22 22:50:39.000000 settngs-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-22 22:50:39.000000 settngs-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-02-22 22:50:50.896527 settngs-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-02-22 22:50:39.000000 settngs-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-22 22:50:39.000000 settngs-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 22:50:39.000000 settngs-0.9.3/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:50.892527 settngs-0.9.3/settngs/
+-rw-r--r--   0 runner    (1001) docker     (127)    37371 2024-02-22 22:50:39.000000 settngs-0.9.3/settngs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 22:50:39.000000 settngs-0.9.3/settngs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:39.000000 settngs-0.9.3/settngs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:50.896527 settngs-0.9.3/settngs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-02-22 22:50:50.000000 settngs-0.9.3/settngs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-22 22:50:50.000000 settngs-0.9.3/settngs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 22:50:50.000000 settngs-0.9.3/settngs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 22:50:50.000000 settngs-0.9.3/settngs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-22 22:50:50.000000 settngs-0.9.3/settngs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-02-22 22:50:50.896527 settngs-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-22 22:50:39.000000 settngs-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:50.892527 settngs-0.9.3/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:39.000000 settngs-0.9.3/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-02-22 22:50:39.000000 settngs-0.9.3/testing/settngs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:50.896527 settngs-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:39.000000 settngs-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33588 2024-02-22 22:50:39.000000 settngs-0.9.3/tests/settngs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 22:50:50.896527 settngs-0.9.3/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-02-22 22:50:39.000000 settngs-0.9.3/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-02-22 22:50:39.000000 settngs-0.9.3/workflows/package.yaml
```

### Comparing `settngs-0.9.2/.github/workflows/build.yaml` & `settngs-0.9.3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `settngs-0.9.2/.gitignore` & `settngs-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `settngs-0.9.2/.pre-commit-config.yaml` & `settngs-0.9.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,24 @@
     -   id: add-trailing-comma
         args: [--py36-plus]
 -   repo: https://github.com/asottile/dead
     rev: v1.5.2
     hooks:
     -   id: dead
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.1
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/hhatto/autopep8
     rev: v2.0.4
     hooks:
     -   id: autopep8
 -   repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
         additional_dependencies: [flake8-encodings, flake8-warnings, flake8-builtins, flake8-length, flake8-print]
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.0
+    rev: v1.8.0
     hooks:
     -   id: mypy
```

### Comparing `settngs-0.9.2/LICENSE` & `settngs-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `settngs-0.9.2/PKG-INFO` & `settngs-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.9.2
+Version: 0.9.3
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.9.2/README.md` & `settngs-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `settngs-0.9.2/settngs/__init__.py` & `settngs-0.9.3/settngs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import sys
 import typing
 from argparse import Namespace
 from collections import defaultdict
 from collections.abc import Sequence
 from typing import Any
 from typing import Callable
+from typing import cast
 from typing import Dict
 from typing import Generic
 from typing import NoReturn
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
@@ -80,14 +81,28 @@
 else:  # pragma: no cover
     List = list
     from types import GenericAlias as types_GenericAlias
     from argparse import BooleanOptionalAction
     removeprefix = str.removeprefix
 
 
+def _isnamedtupleinstance(x: Any) -> bool:
+    t = type(x)
+    b = t.__bases__
+
+    if len(b) != 1 or b[0] != tuple:
+        return False
+
+    f = getattr(t, '_fields', None)
+    if not isinstance(f, tuple):
+        return False
+
+    return all(isinstance(n, str) for n in f)
+
+
 class Setting:
     def __init__(
         self,
         # From argparse
         *names: str,
         action: type[argparse.Action] | str | None = None,
         nargs: str | int | None = None,
@@ -195,26 +210,36 @@
         if self.type is None and self.action is None:
             if self.cmdline:
                 if self.nargs in ('+', '*') or isinstance(self.nargs, int) and self.nargs > 1:
                     return List[str]
                 return str
             else:
                 if not self.cmdline and self.default is not None:
+                    if not isinstance(self.default, str) and not _isnamedtupleinstance(self.default) and isinstance(self.default, Sequence) and self.default and self.default[0]:
+                        try:
+                            return cast(type, type(self.default)[type(self.default[0])])
+                        except Exception:
+                            ...
                     return type(self.default)
                 return 'Any'
 
         if isinstance(self.type, type):
             return self.type
 
         if self.type is not None:
             type_hints = typing.get_type_hints(self.type)
             if 'return' in type_hints:
                 t: type | str = type_hints['return']
                 return t
             if self.default is not None:
+                if not isinstance(self.default, str) and not _isnamedtupleinstance(self.default) and isinstance(self.default, Sequence) and self.default and self.default[0]:
+                    try:
+                        return cast(type, type(self.default)[type(self.default[0])])
+                    except Exception:
+                        ...
                 return type(self.default)
             return 'Any'
 
         if self.action in ('store_true', 'store_false', BooleanOptionalAction):
             return bool
 
         if self.action in ('store_const',):
```

### Comparing `settngs-0.9.2/settngs.egg-info/PKG-INFO` & `settngs-0.9.3/settngs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: settngs
-Version: 0.9.2
+Version: 0.9.3
 Summary: A library for managing settings
 Home-page: https://github.com/lordwelch/settngs
 Author: Timmy Welch
 Author-email: timmy@narnian.us
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `settngs-0.9.2/setup.cfg` & `settngs-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `settngs-0.9.2/testing/settngs.py` & `settngs-0.9.3/testing/settngs.py`

 * *Files identical despite different names*

### Comparing `settngs-0.9.2/tests/settngs_test.py` & `settngs-0.9.3/tests/settngs_test.py`

 * *Files identical despite different names*

### Comparing `settngs-0.9.2/workflows/build.yaml` & `settngs-0.9.3/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `settngs-0.9.2/workflows/package.yaml` & `settngs-0.9.3/workflows/package.yaml`

 * *Files identical despite different names*


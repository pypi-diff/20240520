# Comparing `tmp/cmplib-1.0.0.tar.gz` & `tmp/cmplib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmplib-1.0.0.tar", max compression
+gzip compressed data, was "cmplib-1.1.0.tar", max compression
```

## Comparing `cmplib-1.0.0.tar` & `cmplib-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    32473 2024-03-09 23:56:37.614949 cmplib-1.0.0/LICENSE
--rw-r--r--   0        0        0     7486 2024-03-09 23:49:21.724241 cmplib-1.0.0/README.md
--rw-r--r--   0        0        0      887 2024-03-09 23:54:46.198264 cmplib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9069 2024-03-09 23:46:10.371054 cmplib-1.0.0/src/cmplib/__init__.py
--rw-r--r--   0        0        0     8342 1970-01-01 00:00:00.000000 cmplib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-05-20 08:31:27.632749 cmplib-1.1.0/LICENSE
+-rw-r--r--   0        0        0    32473 2024-05-20 08:30:32.204401 cmplib-1.1.0/LICENSE-GPL-3.0
+-rw-r--r--   0        0        0     7844 2024-05-20 08:41:49.964658 cmplib-1.1.0/README.md
+-rw-r--r--   0        0        0      888 2024-05-20 08:32:41.425213 cmplib-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9262 2024-05-20 08:43:04.313125 cmplib-1.1.0/src/cmplib/__init__.py
+-rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 cmplib-1.1.0/PKG-INFO
```

### Comparing `cmplib-1.0.0/LICENSE` & `cmplib-1.1.0/LICENSE-GPL-3.0`

 * *Files identical despite different names*

### Comparing `cmplib-1.0.0/README.md` & `cmplib-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,25 @@
 
 assert False == Not(Truish())
 assert True != Not(Truish())
 assert 1 == Not(Gt(1))
 assert 1 == Not(2)
 ```
 
+### Is
+
+Check whether a value is the same object as the one stored in a matcher.
+
+```python
+obj = object()
+
+assert obj == Is(obj)
+assert list() != Is(list())
+```
+
 ### IsNone
 
 Check whether a value is `None`.
 
 ```python
 assert None == IsNone()
 assert 0 == Not(IsNone())
@@ -297,10 +308,20 @@
 return a boolean, but instead its return value is casted to boolean.
 
 ```python
 assert 1 == Fn(lambda x: x == 1)
 assert "1" == Fn((lambda x: x), coerce=True)
 ```
 
+### SKIP
+
+`SKIP` is a sentinel which always matches true and can be used to mark not
+interesing items.
+
+```python
+assert [1, 2, 3] == [SKIP, SKIP, SKIP]
+assert [1, 2, 3] == [1, SKIP, SKIP]
+```
+
 ## License
 
-cmplib is licensed under the terms of GPLv3.
+cmplib is licensed under the terms of LGPLv3.
```

### Comparing `cmplib-1.0.0/pyproject.toml` & `cmplib-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["poetry-core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cmplib"
-version = "1.0.0"
+version = "1.1.0"
 description = "Library for writing composable predicates"
 authors = ["Michal Goral <dev@goral.net.pl>"]
-license = "GPL-3.0-only"
+license = "LGPL-3.0-only"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
 ]
 readme = "README.md"
 packages = [
     { include = "cmplib", from = "src" },
```

### Comparing `cmplib-1.0.0/src/cmplib/__init__.py` & `cmplib-1.1.0/src/cmplib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# SPDX-License-Identifier: GPL-3.0-only
+# SPDX-License-Identifier: LGPL-3.0-only
 # Copyright (C) 2023 Michał Góral.
 
-from typing import Any, Callable, Optional, Dict
-
 import importlib.metadata as importlib_metadata
-
 from datetime import date, datetime
-
+from typing import Any, Callable, Dict, Optional
 
 __title__ = "cmplib"
 __description__ = "Writing composable matchers"
 __author__ = "Michał Góral (dev@goral.net.pl)"
 __version__ = importlib_metadata.version("cmplib")
 __copyright__ = "Copyright (c) Michał Góral"
-__license__ = "GPL-3.0-only"
+__license__ = "LGPL-3.0-only"
 
 
 class Cmp:
     def match(self, other: Any) -> bool:
         raise NotImplementedError
 
     def __eq__(self, other: Any) -> bool:
@@ -180,14 +177,25 @@
     def match(self, other):
         return bool(other)
 
     def __repr__(self):
         return "maps to true"
 
 
+class Is(Cmp):
+    def __init__(self, val):
+        self.val = val
+
+    def match(self, other):
+        return self.val is other
+
+    def __repr__(self):
+        return f"is {repr(self.val)}"
+
+
 class IsNone(Cmp):
     def match(self, other):
         return other is None
 
     def __repr__(self):
         return "is None"
```

### Comparing `cmplib-1.0.0/PKG-INFO` & `cmplib-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cmplib
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library for writing composable predicates
 Home-page: https://git.goral.net.pl/cmplib.git/about
-License: GPL-3.0-only
+License: LGPL-3.0-only
 Author: Michal Goral
 Author-email: dev@goral.net.pl
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://git.goral.net.pl/cmplib.git/about
 Project-URL: Repository, https://git.goral.net.pl/cmplib.git
 Description-Content-Type: text/markdown
 
 # cmplib
 
 cmplib is a library used for writing composable matchers for your tests,
@@ -44,14 +45,25 @@
 
 assert False == Not(Truish())
 assert True != Not(Truish())
 assert 1 == Not(Gt(1))
 assert 1 == Not(2)
 ```
 
+### Is
+
+Check whether a value is the same object as the one stored in a matcher.
+
+```python
+obj = object()
+
+assert obj == Is(obj)
+assert list() != Is(list())
+```
+
 ### IsNone
 
 Check whether a value is `None`.
 
 ```python
 assert None == IsNone()
 assert 0 == Not(IsNone())
@@ -318,11 +330,21 @@
 return a boolean, but instead its return value is casted to boolean.
 
 ```python
 assert 1 == Fn(lambda x: x == 1)
 assert "1" == Fn((lambda x: x), coerce=True)
 ```
 
+### SKIP
+
+`SKIP` is a sentinel which always matches true and can be used to mark not
+interesing items.
+
+```python
+assert [1, 2, 3] == [SKIP, SKIP, SKIP]
+assert [1, 2, 3] == [1, SKIP, SKIP]
+```
+
 ## License
 
-cmplib is licensed under the terms of GPLv3.
+cmplib is licensed under the terms of LGPLv3.
```


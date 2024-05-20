# Comparing `tmp/mypy_boto3_controltower-1.34.109.tar.gz` & `tmp/mypy-boto3-controltower-1.34.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_controltower-1.34.109.tar", last modified: Mon May 20 19:47:05 2024, max compression
+gzip compressed data, was "mypy-boto3-controltower-1.34.42.tar", last modified: Wed Feb 14 20:32:18 2024, max compression
```

## Comparing `mypy_boto3_controltower-1.34.109.tar` & `mypy-boto3-controltower-1.34.42.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:47:05.388549 mypy_boto3_controltower-1.34.109/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13596 2024-05-20 19:47:05.388549 mypy_boto3_controltower-1.34.109/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:47:05.388549 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21233 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21230 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-05-20 19:46:41.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-05-20 19:46:41.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22035 2024-05-20 19:46:41.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22035 2024-05-20 19:46:41.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:47:05.388549 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13596 2024-05-20 19:47:05.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-20 19:47:05.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:47:05.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:47:05.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 19:47:05.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 19:47:05.000000 mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:47:05.388549 mypy_boto3_controltower-1.34.109/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-20 19:46:40.000000 mypy_boto3_controltower-1.34.109/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 20:32:18.943383 mypy-boto3-controltower-1.34.42/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-02-14 20:32:18.943383 mypy-boto3-controltower-1.34.42/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 20:32:18.943383 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19916 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-02-14 20:32:04.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-02-14 20:32:04.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-02-14 20:32:04.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 20:32:18.943383 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-02-14 20:32:18.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-14 20:32:18.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 20:32:18.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 20:32:18.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-14 20:32:18.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-14 20:32:18.000000 mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 20:32:18.943383 mypy-boto3-controltower-1.34.42/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-02-14 20:32:03.000000 mypy-boto3-controltower-1.34.42/setup.py
```

### Comparing `mypy_boto3_controltower-1.34.109/LICENSE` & `mypy-boto3-controltower-1.34.42/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_controltower-1.34.109/PKG-INFO` & `mypy-boto3-controltower-1.34.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-controltower
-Version: 1.34.109
-Summary: Type annotations for boto3.ControlTower 1.34.109 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.42
+Summary: Type annotations for boto3.ControlTower 1.34.42 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-controltower.svg?color=blue)](https://pypi.org/project/mypy-boto3-controltower)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-controltower)](https://pepy.tech/project/mypy-boto3-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ControlTower 1.34.109](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[boto3.ControlTower 1.34.42](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-controltower docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,28 +282,24 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_controltower import ControlTowerClient
 from mypy_boto3_controltower.paginator import (
     ListBaselinesPaginator,
-    ListControlOperationsPaginator,
     ListEnabledBaselinesPaginator,
     ListEnabledControlsPaginator,
     ListLandingZonesPaginator,
 )
 
 client: ControlTowerClient = Session().client("controltower")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_baselines_paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")
-list_control_operations_paginator: ListControlOperationsPaginator = client.get_paginator(
-    "list_control_operations"
-)
 list_enabled_baselines_paginator: ListEnabledBaselinesPaginator = client.get_paginator(
     "list_enabled_baselines"
 )
 list_enabled_controls_paginator: ListEnabledControlsPaginator = client.get_paginator(
     "list_enabled_controls"
 )
 list_landing_zones_paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")
```

### Comparing `mypy_boto3_controltower-1.34.109/README.md` & `mypy-boto3-controltower-1.34.42/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-controltower.svg?color=blue)](https://pypi.org/project/mypy-boto3-controltower)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-controltower)](https://pepy.tech/project/mypy-boto3-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ControlTower 1.34.109](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[boto3.ControlTower 1.34.42](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-controltower docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -249,28 +249,24 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_controltower import ControlTowerClient
 from mypy_boto3_controltower.paginator import (
     ListBaselinesPaginator,
-    ListControlOperationsPaginator,
     ListEnabledBaselinesPaginator,
     ListEnabledControlsPaginator,
     ListLandingZonesPaginator,
 )
 
 client: ControlTowerClient = Session().client("controltower")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_baselines_paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")
-list_control_operations_paginator: ListControlOperationsPaginator = client.get_paginator(
-    "list_control_operations"
-)
 list_enabled_baselines_paginator: ListEnabledBaselinesPaginator = client.get_paginator(
     "list_enabled_baselines"
 )
 list_enabled_controls_paginator: ListEnabledControlsPaginator = client.get_paginator(
     "list_enabled_controls"
 )
 list_landing_zones_paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/__init__.py` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,44 +5,40 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_controltower import (
         Client,
         ControlTowerClient,
         ListBaselinesPaginator,
-        ListControlOperationsPaginator,
         ListEnabledBaselinesPaginator,
         ListEnabledControlsPaginator,
         ListLandingZonesPaginator,
     )
 
     session = Session()
     client: ControlTowerClient = session.client("controltower")
 
     list_baselines_paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")
-    list_control_operations_paginator: ListControlOperationsPaginator = client.get_paginator("list_control_operations")
     list_enabled_baselines_paginator: ListEnabledBaselinesPaginator = client.get_paginator("list_enabled_baselines")
     list_enabled_controls_paginator: ListEnabledControlsPaginator = client.get_paginator("list_enabled_controls")
     list_landing_zones_paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")
     ```
 """
 
 from .client import ControlTowerClient
 from .paginator import (
     ListBaselinesPaginator,
-    ListControlOperationsPaginator,
     ListEnabledBaselinesPaginator,
     ListEnabledControlsPaginator,
     ListLandingZonesPaginator,
 )
 
 Client = ControlTowerClient
 
 __all__ = (
     "Client",
     "ControlTowerClient",
     "ListBaselinesPaginator",
-    "ListControlOperationsPaginator",
     "ListEnabledBaselinesPaginator",
     "ListEnabledControlsPaginator",
     "ListLandingZonesPaginator",
 )
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/__init__.pyi` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/__init__.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -5,44 +5,40 @@
 
     ```python
     from boto3.session import Session
     from mypy_boto3_controltower import (
         Client,
         ControlTowerClient,
         ListBaselinesPaginator,
-        ListControlOperationsPaginator,
         ListEnabledBaselinesPaginator,
         ListEnabledControlsPaginator,
         ListLandingZonesPaginator,
     )
 
     session = Session()
     client: ControlTowerClient = session.client("controltower")
 
     list_baselines_paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")
-    list_control_operations_paginator: ListControlOperationsPaginator = client.get_paginator("list_control_operations")
     list_enabled_baselines_paginator: ListEnabledBaselinesPaginator = client.get_paginator("list_enabled_baselines")
     list_enabled_controls_paginator: ListEnabledControlsPaginator = client.get_paginator("list_enabled_controls")
     list_landing_zones_paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")
     ```
 """
 
 from .client import ControlTowerClient
 from .paginator import (
     ListBaselinesPaginator,
-    ListControlOperationsPaginator,
     ListEnabledBaselinesPaginator,
     ListEnabledControlsPaginator,
     ListLandingZonesPaginator,
 )
 
 Client = ControlTowerClient
 
 __all__ = (
     "Client",
     "ControlTowerClient",
     "ListBaselinesPaginator",
-    "ListControlOperationsPaginator",
     "ListEnabledBaselinesPaginator",
     "ListEnabledControlsPaginator",
     "ListLandingZonesPaginator",
 )
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/__main__.py` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ControlTower 1.34.109\n"
-        "Version:         1.34.109\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.ControlTower 1.34.42\n"
+        "Version:         1.34.42\n"
+        "Builder version: 7.23.1\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.109")
+    print("1.34.42")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/client.py` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,40 +17,36 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListBaselinesPaginator,
-    ListControlOperationsPaginator,
     ListEnabledBaselinesPaginator,
     ListEnabledControlsPaginator,
     ListLandingZonesPaginator,
 )
 from .type_defs import (
-    ControlOperationFilterTypeDef,
     CreateLandingZoneOutputTypeDef,
     DeleteLandingZoneOutputTypeDef,
     DisableBaselineOutputTypeDef,
     DisableControlOutputTypeDef,
     EnableBaselineOutputTypeDef,
     EnableControlOutputTypeDef,
     EnabledBaselineFilterTypeDef,
     EnabledBaselineParameterTypeDef,
-    EnabledControlFilterTypeDef,
     EnabledControlParameterTypeDef,
     GetBaselineOperationOutputTypeDef,
     GetBaselineOutputTypeDef,
     GetControlOperationOutputTypeDef,
     GetEnabledBaselineOutputTypeDef,
     GetEnabledControlOutputTypeDef,
     GetLandingZoneOperationOutputTypeDef,
     GetLandingZoneOutputTypeDef,
     ListBaselinesOutputTypeDef,
-    ListControlOperationsOutputTypeDef,
     ListEnabledBaselinesOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
     ListLandingZonesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ResetEnabledBaselineOutputTypeDef,
     ResetLandingZoneOutputTypeDef,
     UpdateEnabledBaselineOutputTypeDef,
@@ -275,28 +271,14 @@
         """
         Returns a summary list of all available baselines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_baselines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#list_baselines)
         """
 
-    def list_control_operations(
-        self,
-        *,
-        filter: ControlOperationFilterTypeDef = ...,
-        maxResults: int = ...,
-        nextToken: str = ...,
-    ) -> ListControlOperationsOutputTypeDef:
-        """
-        Provides a list of operations in progress or queued.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_control_operations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#list_control_operations)
-        """
-
     def list_enabled_baselines(
         self,
         *,
         filter: EnabledBaselineFilterTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
     ) -> ListEnabledBaselinesOutputTypeDef:
@@ -304,20 +286,15 @@
         Returns a list of summaries describing `EnabledBaseline` resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_enabled_baselines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#list_enabled_baselines)
         """
 
     def list_enabled_controls(
-        self,
-        *,
-        filter: EnabledControlFilterTypeDef = ...,
-        maxResults: int = ...,
-        nextToken: str = ...,
-        targetIdentifier: str = ...,
+        self, *, targetIdentifier: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListEnabledControlsOutputTypeDef:
         """
         Lists the controls enabled by Amazon Web Services Control Tower on the
         specified organizational unit and the accounts it
         contains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_enabled_controls)
@@ -416,23 +393,14 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
-        self, operation_name: Literal["list_control_operations"]
-    ) -> ListControlOperationsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#get_paginator)
-        """
-
-    @overload
-    def get_paginator(
         self, operation_name: Literal["list_enabled_baselines"]
     ) -> ListEnabledBaselinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#get_paginator)
         """
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/client.pyi` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,40 +17,36 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListBaselinesPaginator,
-    ListControlOperationsPaginator,
     ListEnabledBaselinesPaginator,
     ListEnabledControlsPaginator,
     ListLandingZonesPaginator,
 )
 from .type_defs import (
-    ControlOperationFilterTypeDef,
     CreateLandingZoneOutputTypeDef,
     DeleteLandingZoneOutputTypeDef,
     DisableBaselineOutputTypeDef,
     DisableControlOutputTypeDef,
     EnableBaselineOutputTypeDef,
     EnableControlOutputTypeDef,
     EnabledBaselineFilterTypeDef,
     EnabledBaselineParameterTypeDef,
-    EnabledControlFilterTypeDef,
     EnabledControlParameterTypeDef,
     GetBaselineOperationOutputTypeDef,
     GetBaselineOutputTypeDef,
     GetControlOperationOutputTypeDef,
     GetEnabledBaselineOutputTypeDef,
     GetEnabledControlOutputTypeDef,
     GetLandingZoneOperationOutputTypeDef,
     GetLandingZoneOutputTypeDef,
     ListBaselinesOutputTypeDef,
-    ListControlOperationsOutputTypeDef,
     ListEnabledBaselinesOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
     ListLandingZonesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ResetEnabledBaselineOutputTypeDef,
     ResetLandingZoneOutputTypeDef,
     UpdateEnabledBaselineOutputTypeDef,
@@ -272,28 +268,14 @@
         """
         Returns a summary list of all available baselines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_baselines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#list_baselines)
         """
 
-    def list_control_operations(
-        self,
-        *,
-        filter: ControlOperationFilterTypeDef = ...,
-        maxResults: int = ...,
-        nextToken: str = ...,
-    ) -> ListControlOperationsOutputTypeDef:
-        """
-        Provides a list of operations in progress or queued.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_control_operations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#list_control_operations)
-        """
-
     def list_enabled_baselines(
         self,
         *,
         filter: EnabledBaselineFilterTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
     ) -> ListEnabledBaselinesOutputTypeDef:
@@ -301,20 +283,15 @@
         Returns a list of summaries describing `EnabledBaseline` resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_enabled_baselines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#list_enabled_baselines)
         """
 
     def list_enabled_controls(
-        self,
-        *,
-        filter: EnabledControlFilterTypeDef = ...,
-        maxResults: int = ...,
-        nextToken: str = ...,
-        targetIdentifier: str = ...,
+        self, *, targetIdentifier: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListEnabledControlsOutputTypeDef:
         """
         Lists the controls enabled by Amazon Web Services Control Tower on the
         specified organizational unit and the accounts it
         contains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.list_enabled_controls)
@@ -413,23 +390,14 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
-        self, operation_name: Literal["list_control_operations"]
-    ) -> ListControlOperationsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#get_paginator)
-        """
-
-    @overload
-    def get_paginator(
         self, operation_name: Literal["list_enabled_baselines"]
     ) -> ListEnabledBaselinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/client/#get_paginator)
         """
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/literals.py` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     "DriftStatusType",
     "EnablementStatusType",
     "LandingZoneDriftStatusType",
     "LandingZoneOperationStatusType",
     "LandingZoneOperationTypeType",
     "LandingZoneStatusType",
     "ListBaselinesPaginatorName",
-    "ListControlOperationsPaginatorName",
     "ListEnabledBaselinesPaginatorName",
     "ListEnabledControlsPaginatorName",
     "ListLandingZonesPaginatorName",
     "ControlTowerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
@@ -51,15 +50,14 @@
 DriftStatusType = Literal["DRIFTED", "IN_SYNC", "NOT_CHECKING", "UNKNOWN"]
 EnablementStatusType = Literal["FAILED", "SUCCEEDED", "UNDER_CHANGE"]
 LandingZoneDriftStatusType = Literal["DRIFTED", "IN_SYNC"]
 LandingZoneOperationStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 LandingZoneOperationTypeType = Literal["CREATE", "DELETE", "RESET", "UPDATE"]
 LandingZoneStatusType = Literal["ACTIVE", "FAILED", "PROCESSING"]
 ListBaselinesPaginatorName = Literal["list_baselines"]
-ListControlOperationsPaginatorName = Literal["list_control_operations"]
 ListEnabledBaselinesPaginatorName = Literal["list_enabled_baselines"]
 ListEnabledControlsPaginatorName = Literal["list_enabled_controls"]
 ListLandingZonesPaginatorName = Literal["list_landing_zones"]
 ControlTowerServiceName = Literal["controltower"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -82,15 +80,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -101,15 +98,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -127,15 +123,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -148,26 +143,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -228,14 +221,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -364,15 +358,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -416,15 +409,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -454,34 +446,29 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_baselines",
-    "list_control_operations",
-    "list_enabled_baselines",
-    "list_enabled_controls",
-    "list_landing_zones",
+    "list_baselines", "list_enabled_baselines", "list_enabled_controls", "list_landing_zones"
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
-    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/literals.pyi` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     "DriftStatusType",
     "EnablementStatusType",
     "LandingZoneDriftStatusType",
     "LandingZoneOperationStatusType",
     "LandingZoneOperationTypeType",
     "LandingZoneStatusType",
     "ListBaselinesPaginatorName",
-    "ListControlOperationsPaginatorName",
     "ListEnabledBaselinesPaginatorName",
     "ListEnabledControlsPaginatorName",
     "ListLandingZonesPaginatorName",
     "ControlTowerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
@@ -51,15 +50,14 @@
 DriftStatusType = Literal["DRIFTED", "IN_SYNC", "NOT_CHECKING", "UNKNOWN"]
 EnablementStatusType = Literal["FAILED", "SUCCEEDED", "UNDER_CHANGE"]
 LandingZoneDriftStatusType = Literal["DRIFTED", "IN_SYNC"]
 LandingZoneOperationStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 LandingZoneOperationTypeType = Literal["CREATE", "DELETE", "RESET", "UPDATE"]
 LandingZoneStatusType = Literal["ACTIVE", "FAILED", "PROCESSING"]
 ListBaselinesPaginatorName = Literal["list_baselines"]
-ListControlOperationsPaginatorName = Literal["list_control_operations"]
 ListEnabledBaselinesPaginatorName = Literal["list_enabled_baselines"]
 ListEnabledControlsPaginatorName = Literal["list_enabled_controls"]
 ListLandingZonesPaginatorName = Literal["list_landing_zones"]
 ControlTowerServiceName = Literal["controltower"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -82,15 +80,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -101,15 +98,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -127,15 +123,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -148,26 +143,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -228,14 +221,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -364,15 +358,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -416,15 +409,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -454,34 +446,29 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_baselines",
-    "list_control_operations",
-    "list_enabled_baselines",
-    "list_enabled_controls",
-    "list_landing_zones",
+    "list_baselines", "list_enabled_baselines", "list_enabled_controls", "list_landing_zones"
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
-    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/paginator.py` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/paginator.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,50 +7,44 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_controltower.client import ControlTowerClient
     from mypy_boto3_controltower.paginator import (
         ListBaselinesPaginator,
-        ListControlOperationsPaginator,
         ListEnabledBaselinesPaginator,
         ListEnabledControlsPaginator,
         ListLandingZonesPaginator,
     )
 
     session = Session()
     client: ControlTowerClient = session.client("controltower")
 
     list_baselines_paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")
-    list_control_operations_paginator: ListControlOperationsPaginator = client.get_paginator("list_control_operations")
     list_enabled_baselines_paginator: ListEnabledBaselinesPaginator = client.get_paginator("list_enabled_baselines")
     list_enabled_controls_paginator: ListEnabledControlsPaginator = client.get_paginator("list_enabled_controls")
     list_landing_zones_paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ControlOperationFilterTypeDef,
     EnabledBaselineFilterTypeDef,
-    EnabledControlFilterTypeDef,
     ListBaselinesOutputTypeDef,
-    ListControlOperationsOutputTypeDef,
     ListEnabledBaselinesOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
     ListLandingZonesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListBaselinesPaginator",
-    "ListControlOperationsPaginator",
     "ListEnabledBaselinesPaginator",
     "ListEnabledControlsPaginator",
     "ListLandingZonesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -73,32 +67,14 @@
     ) -> _PageIterator[ListBaselinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListBaselines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listbaselinespaginator)
         """
 
 
-class ListControlOperationsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListControlOperations)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listcontroloperationspaginator)
-    """
-
-    def paginate(
-        self,
-        *,
-        filter: ControlOperationFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListControlOperationsOutputTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListControlOperations.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listcontroloperationspaginator)
-        """
-
-
 class ListEnabledBaselinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledBaselines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledbaselinespaginator)
     """
 
     def paginate(
@@ -116,19 +92,15 @@
 class ListEnabledControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledcontrolspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        filter: EnabledControlFilterTypeDef = ...,
-        targetIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...,
+        self, *, targetIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnabledControlsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledcontrolspaginator)
         """
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/paginator.pyi` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/paginator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -7,50 +7,44 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_controltower.client import ControlTowerClient
     from mypy_boto3_controltower.paginator import (
         ListBaselinesPaginator,
-        ListControlOperationsPaginator,
         ListEnabledBaselinesPaginator,
         ListEnabledControlsPaginator,
         ListLandingZonesPaginator,
     )
 
     session = Session()
     client: ControlTowerClient = session.client("controltower")
 
     list_baselines_paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")
-    list_control_operations_paginator: ListControlOperationsPaginator = client.get_paginator("list_control_operations")
     list_enabled_baselines_paginator: ListEnabledBaselinesPaginator = client.get_paginator("list_enabled_baselines")
     list_enabled_controls_paginator: ListEnabledControlsPaginator = client.get_paginator("list_enabled_controls")
     list_landing_zones_paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ControlOperationFilterTypeDef,
     EnabledBaselineFilterTypeDef,
-    EnabledControlFilterTypeDef,
     ListBaselinesOutputTypeDef,
-    ListControlOperationsOutputTypeDef,
     ListEnabledBaselinesOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
     ListLandingZonesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListBaselinesPaginator",
-    "ListControlOperationsPaginator",
     "ListEnabledBaselinesPaginator",
     "ListEnabledControlsPaginator",
     "ListLandingZonesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -70,31 +64,14 @@
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBaselinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListBaselines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listbaselinespaginator)
         """
 
-class ListControlOperationsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListControlOperations)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listcontroloperationspaginator)
-    """
-
-    def paginate(
-        self,
-        *,
-        filter: ControlOperationFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListControlOperationsOutputTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListControlOperations.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listcontroloperationspaginator)
-        """
-
 class ListEnabledBaselinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledBaselines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledbaselinespaginator)
     """
 
     def paginate(
@@ -111,19 +88,15 @@
 class ListEnabledControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledcontrolspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        filter: EnabledControlFilterTypeDef = ...,
-        targetIdentifier: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...,
+        self, *, targetIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnabledControlsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledcontrolspaginator)
         """
 
 class ListLandingZonesPaginator(Paginator):
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/type_defs.py` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,62 +37,58 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BaselineOperationTypeDef",
     "BaselineSummaryTypeDef",
-    "ControlOperationFilterTypeDef",
-    "ControlOperationSummaryTypeDef",
     "ControlOperationTypeDef",
     "CreateLandingZoneInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteLandingZoneInputRequestTypeDef",
     "DisableBaselineInputRequestTypeDef",
     "DisableControlInputRequestTypeDef",
     "DriftStatusSummaryTypeDef",
     "EnabledBaselineParameterTypeDef",
     "EnabledControlParameterTypeDef",
     "EnabledBaselineParameterSummaryTypeDef",
     "EnablementStatusSummaryTypeDef",
     "EnabledBaselineFilterTypeDef",
     "EnabledControlParameterSummaryTypeDef",
     "RegionTypeDef",
-    "EnabledControlFilterTypeDef",
     "GetBaselineInputRequestTypeDef",
     "GetBaselineOperationInputRequestTypeDef",
     "GetControlOperationInputRequestTypeDef",
     "GetEnabledBaselineInputRequestTypeDef",
     "GetEnabledControlInputRequestTypeDef",
     "GetLandingZoneInputRequestTypeDef",
     "GetLandingZoneOperationInputRequestTypeDef",
     "LandingZoneOperationDetailTypeDef",
     "LandingZoneDriftStatusSummaryTypeDef",
     "LandingZoneSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListBaselinesInputRequestTypeDef",
+    "ListEnabledControlsInputRequestTypeDef",
     "ListLandingZonesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ResetEnabledBaselineInputRequestTypeDef",
     "ResetLandingZoneInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateLandingZoneInputRequestTypeDef",
-    "ListControlOperationsInputRequestTypeDef",
     "CreateLandingZoneOutputTypeDef",
     "DeleteLandingZoneOutputTypeDef",
     "DisableBaselineOutputTypeDef",
     "DisableControlOutputTypeDef",
     "EnableBaselineOutputTypeDef",
     "EnableControlOutputTypeDef",
     "GetBaselineOperationOutputTypeDef",
     "GetBaselineOutputTypeDef",
     "GetControlOperationOutputTypeDef",
     "ListBaselinesOutputTypeDef",
-    "ListControlOperationsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ResetEnabledBaselineOutputTypeDef",
     "ResetLandingZoneOutputTypeDef",
     "UpdateEnabledBaselineOutputTypeDef",
     "UpdateEnabledControlOutputTypeDef",
     "UpdateLandingZoneOutputTypeDef",
     "EnableBaselineInputRequestTypeDef",
@@ -100,20 +96,18 @@
     "EnableControlInputRequestTypeDef",
     "UpdateEnabledControlInputRequestTypeDef",
     "EnabledBaselineDetailsTypeDef",
     "EnabledBaselineSummaryTypeDef",
     "EnabledControlSummaryTypeDef",
     "ListEnabledBaselinesInputRequestTypeDef",
     "EnabledControlDetailsTypeDef",
-    "ListEnabledControlsInputRequestTypeDef",
     "GetLandingZoneOperationOutputTypeDef",
     "LandingZoneDetailTypeDef",
     "ListLandingZonesOutputTypeDef",
     "ListBaselinesInputListBaselinesPaginateTypeDef",
-    "ListControlOperationsInputListControlOperationsPaginateTypeDef",
     "ListEnabledBaselinesInputListEnabledBaselinesPaginateTypeDef",
     "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
     "ListLandingZonesInputListLandingZonesPaginateTypeDef",
     "GetEnabledBaselineOutputTypeDef",
     "ListEnabledBaselinesOutputTypeDef",
     "ListEnabledControlsOutputTypeDef",
     "GetEnabledControlOutputTypeDef",
@@ -135,68 +129,40 @@
     "BaselineSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": NotRequired[str],
     },
 )
-ControlOperationFilterTypeDef = TypedDict(
-    "ControlOperationFilterTypeDef",
-    {
-        "controlIdentifiers": NotRequired[Sequence[str]],
-        "controlOperationTypes": NotRequired[Sequence[ControlOperationTypeType]],
-        "enabledControlIdentifiers": NotRequired[Sequence[str]],
-        "statuses": NotRequired[Sequence[ControlOperationStatusType]],
-        "targetIdentifiers": NotRequired[Sequence[str]],
-    },
-)
-ControlOperationSummaryTypeDef = TypedDict(
-    "ControlOperationSummaryTypeDef",
-    {
-        "controlIdentifier": NotRequired[str],
-        "enabledControlIdentifier": NotRequired[str],
-        "endTime": NotRequired[datetime],
-        "operationIdentifier": NotRequired[str],
-        "operationType": NotRequired[ControlOperationTypeType],
-        "startTime": NotRequired[datetime],
-        "status": NotRequired[ControlOperationStatusType],
-        "statusMessage": NotRequired[str],
-        "targetIdentifier": NotRequired[str],
-    },
-)
 ControlOperationTypeDef = TypedDict(
     "ControlOperationTypeDef",
     {
-        "controlIdentifier": NotRequired[str],
-        "enabledControlIdentifier": NotRequired[str],
         "endTime": NotRequired[datetime],
-        "operationIdentifier": NotRequired[str],
         "operationType": NotRequired[ControlOperationTypeType],
         "startTime": NotRequired[datetime],
         "status": NotRequired[ControlOperationStatusType],
         "statusMessage": NotRequired[str],
-        "targetIdentifier": NotRequired[str],
     },
 )
 CreateLandingZoneInputRequestTypeDef = TypedDict(
     "CreateLandingZoneInputRequestTypeDef",
     {
         "manifest": Mapping[str, Any],
         "version": str,
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 DeleteLandingZoneInputRequestTypeDef = TypedDict(
     "DeleteLandingZoneInputRequestTypeDef",
     {
         "landingZoneIdentifier": str,
     },
@@ -264,22 +230,14 @@
 )
 RegionTypeDef = TypedDict(
     "RegionTypeDef",
     {
         "name": NotRequired[str],
     },
 )
-EnabledControlFilterTypeDef = TypedDict(
-    "EnabledControlFilterTypeDef",
-    {
-        "controlIdentifiers": NotRequired[Sequence[str]],
-        "driftStatuses": NotRequired[Sequence[DriftStatusType]],
-        "statuses": NotRequired[Sequence[EnablementStatusType]],
-    },
-)
 GetBaselineInputRequestTypeDef = TypedDict(
     "GetBaselineInputRequestTypeDef",
     {
         "baselineIdentifier": str,
     },
 )
 GetBaselineOperationInputRequestTypeDef = TypedDict(
@@ -351,14 +309,22 @@
 ListBaselinesInputRequestTypeDef = TypedDict(
     "ListBaselinesInputRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListEnabledControlsInputRequestTypeDef = TypedDict(
+    "ListEnabledControlsInputRequestTypeDef",
+    {
+        "targetIdentifier": str,
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListLandingZonesInputRequestTypeDef = TypedDict(
     "ListLandingZonesInputRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
@@ -398,22 +364,14 @@
     "UpdateLandingZoneInputRequestTypeDef",
     {
         "landingZoneIdentifier": str,
         "manifest": Mapping[str, Any],
         "version": str,
     },
 )
-ListControlOperationsInputRequestTypeDef = TypedDict(
-    "ListControlOperationsInputRequestTypeDef",
-    {
-        "filter": NotRequired[ControlOperationFilterTypeDef],
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
 CreateLandingZoneOutputTypeDef = TypedDict(
     "CreateLandingZoneOutputTypeDef",
     {
         "arn": str,
         "operationIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -482,22 +440,14 @@
     "ListBaselinesOutputTypeDef",
     {
         "baselines": List[BaselineSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListControlOperationsOutputTypeDef = TypedDict(
-    "ListControlOperationsOutputTypeDef",
-    {
-        "controlOperations": List[ControlOperationSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -617,23 +567,14 @@
         "driftStatusSummary": NotRequired[DriftStatusSummaryTypeDef],
         "parameters": NotRequired[List[EnabledControlParameterSummaryTypeDef]],
         "statusSummary": NotRequired[EnablementStatusSummaryTypeDef],
         "targetIdentifier": NotRequired[str],
         "targetRegions": NotRequired[List[RegionTypeDef]],
     },
 )
-ListEnabledControlsInputRequestTypeDef = TypedDict(
-    "ListEnabledControlsInputRequestTypeDef",
-    {
-        "filter": NotRequired[EnabledControlFilterTypeDef],
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-        "targetIdentifier": NotRequired[str],
-    },
-)
 GetLandingZoneOperationOutputTypeDef = TypedDict(
     "GetLandingZoneOperationOutputTypeDef",
     {
         "operationDetails": LandingZoneOperationDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -658,33 +599,25 @@
 )
 ListBaselinesInputListBaselinesPaginateTypeDef = TypedDict(
     "ListBaselinesInputListBaselinesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListControlOperationsInputListControlOperationsPaginateTypeDef = TypedDict(
-    "ListControlOperationsInputListControlOperationsPaginateTypeDef",
-    {
-        "filter": NotRequired[ControlOperationFilterTypeDef],
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-    },
-)
 ListEnabledBaselinesInputListEnabledBaselinesPaginateTypeDef = TypedDict(
     "ListEnabledBaselinesInputListEnabledBaselinesPaginateTypeDef",
     {
         "filter": NotRequired[EnabledBaselineFilterTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
     "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
     {
-        "filter": NotRequired[EnabledControlFilterTypeDef],
-        "targetIdentifier": NotRequired[str],
+        "targetIdentifier": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListLandingZonesInputListLandingZonesPaginateTypeDef = TypedDict(
     "ListLandingZonesInputListLandingZonesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower/type_defs.pyi` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -37,62 +37,58 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BaselineOperationTypeDef",
     "BaselineSummaryTypeDef",
-    "ControlOperationFilterTypeDef",
-    "ControlOperationSummaryTypeDef",
     "ControlOperationTypeDef",
     "CreateLandingZoneInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteLandingZoneInputRequestTypeDef",
     "DisableBaselineInputRequestTypeDef",
     "DisableControlInputRequestTypeDef",
     "DriftStatusSummaryTypeDef",
     "EnabledBaselineParameterTypeDef",
     "EnabledControlParameterTypeDef",
     "EnabledBaselineParameterSummaryTypeDef",
     "EnablementStatusSummaryTypeDef",
     "EnabledBaselineFilterTypeDef",
     "EnabledControlParameterSummaryTypeDef",
     "RegionTypeDef",
-    "EnabledControlFilterTypeDef",
     "GetBaselineInputRequestTypeDef",
     "GetBaselineOperationInputRequestTypeDef",
     "GetControlOperationInputRequestTypeDef",
     "GetEnabledBaselineInputRequestTypeDef",
     "GetEnabledControlInputRequestTypeDef",
     "GetLandingZoneInputRequestTypeDef",
     "GetLandingZoneOperationInputRequestTypeDef",
     "LandingZoneOperationDetailTypeDef",
     "LandingZoneDriftStatusSummaryTypeDef",
     "LandingZoneSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListBaselinesInputRequestTypeDef",
+    "ListEnabledControlsInputRequestTypeDef",
     "ListLandingZonesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ResetEnabledBaselineInputRequestTypeDef",
     "ResetLandingZoneInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateLandingZoneInputRequestTypeDef",
-    "ListControlOperationsInputRequestTypeDef",
     "CreateLandingZoneOutputTypeDef",
     "DeleteLandingZoneOutputTypeDef",
     "DisableBaselineOutputTypeDef",
     "DisableControlOutputTypeDef",
     "EnableBaselineOutputTypeDef",
     "EnableControlOutputTypeDef",
     "GetBaselineOperationOutputTypeDef",
     "GetBaselineOutputTypeDef",
     "GetControlOperationOutputTypeDef",
     "ListBaselinesOutputTypeDef",
-    "ListControlOperationsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ResetEnabledBaselineOutputTypeDef",
     "ResetLandingZoneOutputTypeDef",
     "UpdateEnabledBaselineOutputTypeDef",
     "UpdateEnabledControlOutputTypeDef",
     "UpdateLandingZoneOutputTypeDef",
     "EnableBaselineInputRequestTypeDef",
@@ -100,20 +96,18 @@
     "EnableControlInputRequestTypeDef",
     "UpdateEnabledControlInputRequestTypeDef",
     "EnabledBaselineDetailsTypeDef",
     "EnabledBaselineSummaryTypeDef",
     "EnabledControlSummaryTypeDef",
     "ListEnabledBaselinesInputRequestTypeDef",
     "EnabledControlDetailsTypeDef",
-    "ListEnabledControlsInputRequestTypeDef",
     "GetLandingZoneOperationOutputTypeDef",
     "LandingZoneDetailTypeDef",
     "ListLandingZonesOutputTypeDef",
     "ListBaselinesInputListBaselinesPaginateTypeDef",
-    "ListControlOperationsInputListControlOperationsPaginateTypeDef",
     "ListEnabledBaselinesInputListEnabledBaselinesPaginateTypeDef",
     "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
     "ListLandingZonesInputListLandingZonesPaginateTypeDef",
     "GetEnabledBaselineOutputTypeDef",
     "ListEnabledBaselinesOutputTypeDef",
     "ListEnabledControlsOutputTypeDef",
     "GetEnabledControlOutputTypeDef",
@@ -135,68 +129,40 @@
     "BaselineSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": NotRequired[str],
     },
 )
-ControlOperationFilterTypeDef = TypedDict(
-    "ControlOperationFilterTypeDef",
-    {
-        "controlIdentifiers": NotRequired[Sequence[str]],
-        "controlOperationTypes": NotRequired[Sequence[ControlOperationTypeType]],
-        "enabledControlIdentifiers": NotRequired[Sequence[str]],
-        "statuses": NotRequired[Sequence[ControlOperationStatusType]],
-        "targetIdentifiers": NotRequired[Sequence[str]],
-    },
-)
-ControlOperationSummaryTypeDef = TypedDict(
-    "ControlOperationSummaryTypeDef",
-    {
-        "controlIdentifier": NotRequired[str],
-        "enabledControlIdentifier": NotRequired[str],
-        "endTime": NotRequired[datetime],
-        "operationIdentifier": NotRequired[str],
-        "operationType": NotRequired[ControlOperationTypeType],
-        "startTime": NotRequired[datetime],
-        "status": NotRequired[ControlOperationStatusType],
-        "statusMessage": NotRequired[str],
-        "targetIdentifier": NotRequired[str],
-    },
-)
 ControlOperationTypeDef = TypedDict(
     "ControlOperationTypeDef",
     {
-        "controlIdentifier": NotRequired[str],
-        "enabledControlIdentifier": NotRequired[str],
         "endTime": NotRequired[datetime],
-        "operationIdentifier": NotRequired[str],
         "operationType": NotRequired[ControlOperationTypeType],
         "startTime": NotRequired[datetime],
         "status": NotRequired[ControlOperationStatusType],
         "statusMessage": NotRequired[str],
-        "targetIdentifier": NotRequired[str],
     },
 )
 CreateLandingZoneInputRequestTypeDef = TypedDict(
     "CreateLandingZoneInputRequestTypeDef",
     {
         "manifest": Mapping[str, Any],
         "version": str,
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 DeleteLandingZoneInputRequestTypeDef = TypedDict(
     "DeleteLandingZoneInputRequestTypeDef",
     {
         "landingZoneIdentifier": str,
     },
@@ -264,22 +230,14 @@
 )
 RegionTypeDef = TypedDict(
     "RegionTypeDef",
     {
         "name": NotRequired[str],
     },
 )
-EnabledControlFilterTypeDef = TypedDict(
-    "EnabledControlFilterTypeDef",
-    {
-        "controlIdentifiers": NotRequired[Sequence[str]],
-        "driftStatuses": NotRequired[Sequence[DriftStatusType]],
-        "statuses": NotRequired[Sequence[EnablementStatusType]],
-    },
-)
 GetBaselineInputRequestTypeDef = TypedDict(
     "GetBaselineInputRequestTypeDef",
     {
         "baselineIdentifier": str,
     },
 )
 GetBaselineOperationInputRequestTypeDef = TypedDict(
@@ -351,14 +309,22 @@
 ListBaselinesInputRequestTypeDef = TypedDict(
     "ListBaselinesInputRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListEnabledControlsInputRequestTypeDef = TypedDict(
+    "ListEnabledControlsInputRequestTypeDef",
+    {
+        "targetIdentifier": str,
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListLandingZonesInputRequestTypeDef = TypedDict(
     "ListLandingZonesInputRequestTypeDef",
     {
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
@@ -398,22 +364,14 @@
     "UpdateLandingZoneInputRequestTypeDef",
     {
         "landingZoneIdentifier": str,
         "manifest": Mapping[str, Any],
         "version": str,
     },
 )
-ListControlOperationsInputRequestTypeDef = TypedDict(
-    "ListControlOperationsInputRequestTypeDef",
-    {
-        "filter": NotRequired[ControlOperationFilterTypeDef],
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-    },
-)
 CreateLandingZoneOutputTypeDef = TypedDict(
     "CreateLandingZoneOutputTypeDef",
     {
         "arn": str,
         "operationIdentifier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -482,22 +440,14 @@
     "ListBaselinesOutputTypeDef",
     {
         "baselines": List[BaselineSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ListControlOperationsOutputTypeDef = TypedDict(
-    "ListControlOperationsOutputTypeDef",
-    {
-        "controlOperations": List[ControlOperationSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -617,23 +567,14 @@
         "driftStatusSummary": NotRequired[DriftStatusSummaryTypeDef],
         "parameters": NotRequired[List[EnabledControlParameterSummaryTypeDef]],
         "statusSummary": NotRequired[EnablementStatusSummaryTypeDef],
         "targetIdentifier": NotRequired[str],
         "targetRegions": NotRequired[List[RegionTypeDef]],
     },
 )
-ListEnabledControlsInputRequestTypeDef = TypedDict(
-    "ListEnabledControlsInputRequestTypeDef",
-    {
-        "filter": NotRequired[EnabledControlFilterTypeDef],
-        "maxResults": NotRequired[int],
-        "nextToken": NotRequired[str],
-        "targetIdentifier": NotRequired[str],
-    },
-)
 GetLandingZoneOperationOutputTypeDef = TypedDict(
     "GetLandingZoneOperationOutputTypeDef",
     {
         "operationDetails": LandingZoneOperationDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -658,33 +599,25 @@
 )
 ListBaselinesInputListBaselinesPaginateTypeDef = TypedDict(
     "ListBaselinesInputListBaselinesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-ListControlOperationsInputListControlOperationsPaginateTypeDef = TypedDict(
-    "ListControlOperationsInputListControlOperationsPaginateTypeDef",
-    {
-        "filter": NotRequired[ControlOperationFilterTypeDef],
-        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
-    },
-)
 ListEnabledBaselinesInputListEnabledBaselinesPaginateTypeDef = TypedDict(
     "ListEnabledBaselinesInputListEnabledBaselinesPaginateTypeDef",
     {
         "filter": NotRequired[EnabledBaselineFilterTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
     "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
     {
-        "filter": NotRequired[EnabledControlFilterTypeDef],
-        "targetIdentifier": NotRequired[str],
+        "targetIdentifier": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListLandingZonesInputListLandingZonesPaginateTypeDef = TypedDict(
     "ListLandingZonesInputListLandingZonesPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/PKG-INFO` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-controltower
-Version: 1.34.109
-Summary: Type annotations for boto3.ControlTower 1.34.109 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.42
+Summary: Type annotations for boto3.ControlTower 1.34.42 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-controltower.svg?color=blue)](https://pypi.org/project/mypy-boto3-controltower)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-controltower)](https://pepy.tech/project/mypy-boto3-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ControlTower 1.34.109](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[boto3.ControlTower 1.34.42](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-controltower docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,28 +282,24 @@
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_controltower import ControlTowerClient
 from mypy_boto3_controltower.paginator import (
     ListBaselinesPaginator,
-    ListControlOperationsPaginator,
     ListEnabledBaselinesPaginator,
     ListEnabledControlsPaginator,
     ListLandingZonesPaginator,
 )
 
 client: ControlTowerClient = Session().client("controltower")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_baselines_paginator: ListBaselinesPaginator = client.get_paginator("list_baselines")
-list_control_operations_paginator: ListControlOperationsPaginator = client.get_paginator(
-    "list_control_operations"
-)
 list_enabled_baselines_paginator: ListEnabledBaselinesPaginator = client.get_paginator(
     "list_enabled_baselines"
 )
 list_enabled_controls_paginator: ListEnabledControlsPaginator = client.get_paginator(
     "list_enabled_controls"
 )
 list_landing_zones_paginator: ListLandingZonesPaginator = client.get_paginator("list_landing_zones")
```

### Comparing `mypy_boto3_controltower-1.34.109/mypy_boto3_controltower.egg-info/SOURCES.txt` & `mypy-boto3-controltower-1.34.42/mypy_boto3_controltower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_controltower-1.34.109/setup.py` & `mypy-boto3-controltower-1.34.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-controltower",
-    version="1.34.109",
+    version="1.34.42",
     packages=["mypy_boto3_controltower"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ControlTower 1.34.109 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.ControlTower 1.34.42 service generated with mypy-boto3-builder 7.23.1",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


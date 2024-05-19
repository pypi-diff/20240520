# Comparing `tmp/pyboiler_anonoei-0.0.5.tar.gz` & `tmp/pyboiler_anonoei-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboiler_anonoei-0.0.5.tar", last modified: Sun May 12 23:48:16 2024, max compression
+gzip compressed data, was "pyboiler_anonoei-0.3.0.tar", last modified: Sun May 19 23:33:27 2024, max compression
```

## Comparing `pyboiler_anonoei-0.0.5.tar` & `pyboiler_anonoei-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,48 @@
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 23:48:16.629079 pyboiler_anonoei-0.0.5/
--rw-r--r--   0 anonoei    (501) staff       (20)     1051 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.5/LICENSE
--rw-r--r--   0 anonoei    (501) staff       (20)     1281 2024-05-12 23:48:16.628739 pyboiler_anonoei-0.0.5/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)      281 2024-05-12 13:44:40.000000 pyboiler_anonoei-0.0.5/README.md
--rw-r--r--   0 anonoei    (501) staff       (20)     1405 2024-05-12 23:47:13.000000 pyboiler_anonoei-0.0.5/pyproject.toml
--rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-12 23:48:16.629134 pyboiler_anonoei-0.0.5/setup.cfg
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 23:48:16.618833 pyboiler_anonoei-0.0.5/src/
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 23:48:16.624487 pyboiler_anonoei-0.0.5/src/pyboiler/
--rw-r--r--   0 anonoei    (501) staff       (20)      736 2024-05-12 23:47:13.000000 pyboiler_anonoei-0.0.5/src/pyboiler/__init__.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 23:48:16.626482 pyboiler_anonoei-0.0.5/src/pyboiler/_log/
--rw-r--r--   0 anonoei    (501) staff       (20)      220 2024-05-12 12:42:29.000000 pyboiler_anonoei-0.0.5/src/pyboiler/_log/__init__.py
--rw-r--r--   0 anonoei    (501) staff       (20)      129 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.5/src/pyboiler/_log/filter.py
--rw-r--r--   0 anonoei    (501) staff       (20)      421 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.5/src/pyboiler/_log/format.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1778 2024-05-12 12:42:43.000000 pyboiler_anonoei-0.0.5/src/pyboiler/_log/handler.py
--rw-r--r--   0 anonoei    (501) staff       (20)      878 2024-05-12 12:03:41.000000 pyboiler_anonoei-0.0.5/src/pyboiler/_log/level.py
--rw-r--r--   0 anonoei    (501) staff       (20)       77 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.5/src/pyboiler/_log/record.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1331 2024-05-12 23:15:42.000000 pyboiler_anonoei-0.0.5/src/pyboiler/changelog.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2313 2024-05-12 10:43:02.000000 pyboiler_anonoei-0.0.5/src/pyboiler/config.py
--rw-r--r--   0 anonoei    (501) staff       (20)      660 2024-05-12 23:46:14.000000 pyboiler_anonoei-0.0.5/src/pyboiler/error.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2603 2024-05-12 23:17:24.000000 pyboiler_anonoei-0.0.5/src/pyboiler/generic.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2908 2024-05-12 10:51:41.000000 pyboiler_anonoei-0.0.5/src/pyboiler/hml.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1103 2024-05-12 10:24:59.000000 pyboiler_anonoei-0.0.5/src/pyboiler/hson.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2358 2024-05-12 22:55:29.000000 pyboiler_anonoei-0.0.5/src/pyboiler/imports.py
--rw-r--r--   0 anonoei    (501) staff       (20)     3393 2024-05-12 18:34:49.000000 pyboiler_anonoei-0.0.5/src/pyboiler/logger.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1583 2024-05-12 13:26:11.000000 pyboiler_anonoei-0.0.5/src/pyboiler/logging.py
--rw-r--r--   0 anonoei    (501) staff       (20)      571 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.5/src/pyboiler/platform.py
--rw-r--r--   0 anonoei    (501) staff       (20)      594 2024-05-12 10:40:35.000000 pyboiler_anonoei-0.0.5/src/pyboiler/profiler.py
--rw-r--r--   0 anonoei    (501) staff       (20)     3531 2024-05-12 13:29:41.000000 pyboiler_anonoei-0.0.5/src/pyboiler/settings.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1893 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.5/src/pyboiler/version.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 23:48:16.628098 pyboiler_anonoei-0.0.5/src/pyboiler_anonoei.egg-info/
--rw-r--r--   0 anonoei    (501) staff       (20)     1281 2024-05-12 23:48:16.000000 pyboiler_anonoei-0.0.5/src/pyboiler_anonoei.egg-info/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)      776 2024-05-12 23:48:16.000000 pyboiler_anonoei-0.0.5/src/pyboiler_anonoei.egg-info/SOURCES.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        1 2024-05-12 23:48:16.000000 pyboiler_anonoei-0.0.5/src/pyboiler_anonoei.egg-info/dependency_links.txt
--rw-r--r--   0 anonoei    (501) staff       (20)       34 2024-05-12 23:48:16.000000 pyboiler_anonoei-0.0.5/src/pyboiler_anonoei.egg-info/requires.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        9 2024-05-12 23:48:16.000000 pyboiler_anonoei-0.0.5/src/pyboiler_anonoei.egg-info/top_level.txt
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 23:48:16.627680 pyboiler_anonoei-0.0.5/tests/
--rw-r--r--   0 anonoei    (501) staff       (20)      306 2024-05-12 23:16:15.000000 pyboiler_anonoei-0.0.5/tests/test_changelog.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.479337 pyboiler_anonoei-0.3.0/
+-rwxrwx---   0 anonoei    (501) staff       (20)     1051 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.0/LICENSE
+-rw-r--r--   0 anonoei    (501) staff       (20)     1355 2024-05-19 23:33:27.478987 pyboiler_anonoei-0.3.0/PKG-INFO
+-rwxrwx---   0 anonoei    (501) staff       (20)      281 2024-05-12 13:44:40.000000 pyboiler_anonoei-0.3.0/README.md
+-rwxrwx---   0 anonoei    (501) staff       (20)     1423 2024-05-19 23:33:22.000000 pyboiler_anonoei-0.3.0/pyproject.toml
+-rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-19 23:33:27.479397 pyboiler_anonoei-0.3.0/setup.cfg
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.468031 pyboiler_anonoei-0.3.0/src/
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.473396 pyboiler_anonoei-0.3.0/src/pyboiler/
+-rwxrwx---   0 anonoei    (501) staff       (20)      813 2024-05-19 23:31:32.000000 pyboiler_anonoei-0.3.0/src/pyboiler/__init__.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.473630 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-17 22:45:41.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/__init__.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.474548 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/
+-rwxrwx---   0 anonoei    (501) staff       (20)       48 2024-05-18 00:12:37.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/__init__.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2474 2024-05-19 22:15:06.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/colors.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      272 2024-05-19 21:50:23.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/config.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1032 2024-05-19 21:38:25.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/parse.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.476437 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/
+-rwxrwx---   0 anonoei    (501) staff       (20)      256 2024-05-18 09:15:43.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/__init__.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      416 2024-05-19 22:46:14.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/config.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      478 2024-05-18 02:02:44.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/filter.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     3836 2024-05-19 22:17:46.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/format.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2959 2024-05-19 23:10:46.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/handler.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      610 2024-05-19 19:07:04.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/inspect.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1200 2024-05-19 21:55:02.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/level.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      517 2024-05-18 09:40:31.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/record.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1331 2024-05-12 23:15:42.000000 pyboiler_anonoei-0.3.0/src/pyboiler/changelog.py
+-rwxrwx---   0 anonoei    (501) staff       (20)       74 2024-05-18 00:12:59.000000 pyboiler_anonoei-0.3.0/src/pyboiler/color.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2313 2024-05-12 10:43:02.000000 pyboiler_anonoei-0.3.0/src/pyboiler/config.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1041 2024-05-17 18:25:19.000000 pyboiler_anonoei-0.3.0/src/pyboiler/decor.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      660 2024-05-12 23:46:14.000000 pyboiler_anonoei-0.3.0/src/pyboiler/error.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     4227 2024-05-19 23:26:23.000000 pyboiler_anonoei-0.3.0/src/pyboiler/generic.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2908 2024-05-12 10:51:41.000000 pyboiler_anonoei-0.3.0/src/pyboiler/hml.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1103 2024-05-12 10:24:59.000000 pyboiler_anonoei-0.3.0/src/pyboiler/hson.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2358 2024-05-17 23:04:07.000000 pyboiler_anonoei-0.3.0/src/pyboiler/imports.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     3464 2024-05-19 23:23:53.000000 pyboiler_anonoei-0.3.0/src/pyboiler/logger.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2597 2024-05-19 23:08:07.000000 pyboiler_anonoei-0.3.0/src/pyboiler/logging.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      571 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.0/src/pyboiler/platform.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      594 2024-05-12 10:40:35.000000 pyboiler_anonoei-0.3.0/src/pyboiler/profiler.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     3531 2024-05-12 13:29:41.000000 pyboiler_anonoei-0.3.0/src/pyboiler/settings.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1893 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.0/src/pyboiler/version.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.478149 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/
+-rw-r--r--   0 anonoei    (501) staff       (20)     1355 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/PKG-INFO
+-rwxrwx---   0 anonoei    (501) staff       (20)     1141 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/SOURCES.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)        1 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/dependency_links.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)       46 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/requires.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)        9 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/top_level.txt
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.477801 pyboiler_anonoei-0.3.0/tests/
+-rwxrwx---   0 anonoei    (501) staff       (20)      306 2024-05-12 23:16:15.000000 pyboiler_anonoei-0.3.0/tests/test_changelog.py
```

### Comparing `pyboiler_anonoei-0.0.5/LICENSE` & `pyboiler_anonoei-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/PKG-INFO` & `pyboiler_anonoei-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboiler_anonoei
-Version: 0.0.5
+Version: 0.3.0
 Summary: Various generic python helpers so I don't keep rewriting them
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pyboiler
 Project-URL: Documentation, https://anonoei.github.io/pyboiler/
 Project-URL: Repository, https://github.com/Anonoei/pyboiler.git
 Project-URL: Issues, https://github.com/Anonoei/pyboiler/issues
 Project-URL: Source, https://github.com/anonoei/pyboiler
@@ -14,14 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pdoc3; extra == "dev"
 
 # pyboiler
  Various generic python helpers so I don't keep rewriting them
```

### Comparing `pyboiler_anonoei-0.0.5/pyproject.toml` & `pyboiler_anonoei-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyboiler_anonoei"
-version = "0.0.5"
+version = "0.3.0"
 description = "Various generic python helpers so I don't keep rewriting them"
 dependencies = []
 requires-python = ">=3.6"
 authors = [
     {name = "Anonoei", email="dev@anonoei.com"}
 ]
 readme = "README.md"
@@ -28,18 +28,18 @@
 Homepage = "https://github.com/anonoei/pyboiler"
 Documentation = "https://anonoei.github.io/pyboiler/"
 Repository = "https://github.com/Anonoei/pyboiler.git"
 Issues = "https://github.com/Anonoei/pyboiler/issues"
 Source = "https://github.com/anonoei/pyboiler"
 
 [project.optional-dependencies]
-dev = ["black", "bumpver", "pytest", "pdoc3"]
+dev = ["twine", "build", "black", "bumpver", "pytest", "pdoc3"]
 
 [tool.bumpver]
-current_version = "0.0.5"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/__init__.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 
  Imports all files in src/pyboiler/* so they can be imported as
  `pyboiler.config`
 """
 
 import pathlib
 
-__version__ = "0.0.5"
+__version__ = "0.3.0"
 __author__ = "Anonoei <dev@anonoei.com>"
+init_run = False
 
 
-def __init():
+def __init(_val=[]):
     """Import all files in `import_path`"""
+    if _val:
+        return
+    _val.append(True)
     from .config import config
     from .imports import get_imports
 
     import_path = pathlib.Path(__file__).parent
 
     # print(f"Running __init on {import_path}")
     for k, v in get_imports(import_path).items():
         globals()[k] = v
 
     globals()["settings"].Settings().deserialize()
 
 
-__init()
-
-
-def dir():
-    """List all available pyboiler imports"""
+def view():
+    """View all available pyboiler imports"""
+    __init()
     imports = globals()["imports"].get_locals(globals())
     imports.sort()
     return imports
```

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/changelog.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/changelog.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/config.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/config.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/error.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/error.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/generic.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,125 @@
-"""Generic class implementations that can be extended in user code"""
+"""pyboiler.settings file"""
 
 from typing import TYPE_CHECKING
 
-from .imports import get_locals
+from .config import config
 
-
-class storage:
-    """Used to save values similar to a C struct
-
-    ```
-    from pyboiler.generic import storage
-    stor = storage()
-    stor.value = "example"
-    ```
-    """
-
-    _ignore = set(("_:", "json"))
+if config().SERIAL == "json":
+    from .hson import dumps, loads
+else:
+    from .hml import dumps, loads
+
+from .generic import hierarchy
+
+
+class Settings(hierarchy):
+    """Global settings, intended to be edited by users"""
+
+    __instance = None
+
+    def __new__(cls):
+        if cls.__instance is None:
+            cls.__instance = object.__new__(cls)
+            cls._str_name = "Settings"
+            cls._defaults = {}
+            cls._settings = {}
+        return cls.__instance
+
+    def __init__(self):
+        pass
+
+    def Child(self, name: str):
+        sets_inst = getattr(self, name, config().SENTINEL)
+
+        if sets_inst is config().SENTINEL:
+            sets_inst = _Settings(name, self)
+            self._settings[name] = sets_inst
+            self._defaults[name] = sets_inst
+            setattr(self, name, sets_inst)
+        elif not isinstance(sets_inst, _Settings):
+            raise Exception(f"Child '{name}' is not _Settings instance")
+        return sets_inst
+
+    def get(self, key, default=config().SENTINEL):
+        if default is config().SENTINEL:
+            _get = self._settings.get(key, config().SENTINEL)
+            if _get is config().SENTINEL:
+                _get = self._defaults.get(key)
+            return _get
+        return self._settings.get(key, default)
+
+    def set(self, key, val):
+        self._defaults[key] = val
+        setattr(self, key, lambda s=self, k=key: s.get(k))
+
+    def softSet(self, key, val):
+        self._settings[key] = val
+
+    def init(self, name: str, default):
+        self.set(name, default)
+
+    def serialize(self) -> None:
+        s_data = None
+        config().FILEPATH_SETTINGS.write_text(dumps(self._json()))
+
+    def deserialize(self) -> None:
+        if not config().FILEPATH_SETTINGS.exists():
+            return
+        self.from_dict(loads(config().FILEPATH_SETTINGS.read_text()))
+
+    def from_dict(self, d: dict):
+        for k, v in d.items():
+            if isinstance(v, dict):
+                _child = self.Child(k)
+                _child.from_dict(v)
+            else:
+                if v is None:
+                    v = config().SENTINEL
+                self.softSet(k, v)
 
     def json(self) -> dict:
-        """Return attributes as dictionary for json serialization
-        Instances of `type(self)` are returned as dictionaries
-        """
+        """Return attributes as dictionary for json serialization"""
         fmt = {}
-        for k in get_locals(self, self._ignore):
-            v = getattr(self, k)
-            if isinstance(v, type(self)):
+        for k, v in self._defaults.items():
+            if isinstance(v, _Settings):
                 fmt[k] = v.json()
             else:
                 fmt[k] = v
         return fmt
 
-    if TYPE_CHECKING:
+    def _json(self) -> dict:
+        """Internal serialization method for writing to settings.json"""
+        fmt = {}
+        for k, v in self._defaults.items():
+            if isinstance(v, _Settings):
+                fmt[k] = v._json()
+            else:
+                fmt[k] = self.get(k, None)
+        return fmt
 
-        def __getattr__(self, key):
-            return lambda msg: print(msg)
+    def u_fmt_k(self, *args, **kwargs):
+        raise NotImplementedError()
 
+    def u_fmt_v(self, *args, **kwargs):
+        raise NotImplementedError()
 
-class hierarchy(storage):
-    """Dynamically create a hierarchical structure from a dict
+    def _i_init(self, *args, **kwargs):
+        raise NotImplementedError()
 
-    u_* methods are intended to be overridden by children
+    if TYPE_CHECKING:
+
+        def __getattr__(self, key):
+            return lambda msg: print(msg)
 
-    ```python
-    from pyboiler.generic import hierarchy
-    h_dict = {"these": {"are": "nested"}, "dicts": "hierarchy"}
-    hier = hierarchy("root", None, h_dict)
-    print(hier.these.are) # Returns "nested"
-    print(hier.json()) # Returns h_dict
-    ```
-    """
 
-    _parent = None
-    _str_name = None
+class _Settings(Settings):
+    def __new__(cls, *args, **kwargs):
+        obj = object.__new__(cls)
+        obj.__init__(*args, **kwargs)
+        return obj
 
-    def __init__(self, name: str, parent, heir: dict):
+    def __init__(self, name: str, parent):
         self._parent = parent
         self._str_name = name
-        self._ignore = set(("_:", "json", "u_:"))
-        self._i_init(heir)
-
-    def __repr__(self) -> str:
-        return f"<{self._str_name}>"
-
-    @property
-    def _name(self) -> str:
-        if self._parent is None:
-            return f"{type(self).__name__}.{self._str_name}"
-        elif isinstance(self._parent, type(self)):
-            return f"{self._parent._name}.{self._str_name}"
-        return f"{type(self._parent).__name__}.{self._str_name}"
-
-    def _i_init(self, heir: dict):
-        """Internal init so it can be called outside of __init__"""
-        for key, val in heir.items():
-            k = self.u_fmt_k(key, val)
-            v = self.u_fmt_v(k, val)
-            setattr(self, k, v)
-
-    def u_fmt_k(self, k, v):
-        """Format keys before setattr"""
-        return k
-
-    def u_fmt_v(self, k, v):
-        """Format v before setattr.
-
-        Use `v = super().u_fmt(k, v)` if `isinstance(v, dict)` isn't implemented in child methods
-        """
-        if isinstance(v, dict):
-            return type(self)(k, self, v)
-        return v
-
-    if TYPE_CHECKING:
-
-        def __getattr__(self, key):
-            return lambda msg: print(msg)
+        self._defaults = {}
+        self._settings = {}
```

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/hml.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/hml.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/hson.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/hson.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/imports.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/imports.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/logger.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,110 +7,121 @@
 Logger("MyProject", Level().WARN)
 Logger().trace("This is a trace")
 subm = Logger().Child("Submodule")
 subm.trace("And another!")  # Or Logger().subm.trace("And another!")
 ```
 """
 
-import logging as _logging
 import pathlib
-from logging import Manager
-from typing import TYPE_CHECKING
 
+from .generic import storage
 from .config import config
 from .logging import Level, logging
 
 
-class Logger:
+class Logger(storage):
     """Project root logger"""
 
-    __instance = None
-
-    _parent = None
-    _str_name: str = None  # type: ignore
-    _log: logging = None  # type: ignore
+    __slots__ = ["_internal", "_parent", "_str_name", "_logger"]
 
-    def Child(self, name: str, level=None):
-        if level is None:
-            level = self._level
-        log_inst = _Logger(self, name)
-        log_inst._init(Logger().manager.getLogger(log_inst._name), level)
-        setattr(self, name, log_inst)
-
-    @property
-    def _level(self) -> Level:
-        return self._log.level
-
-    @_level.setter
-    def _level(self, level):
-        self._log.level = level
+    __instance = None
 
-    def __new__(cls, name=None, level=Level.TRACE):
+    def __new__(cls, name=None, level: Level = None):
         if cls.__instance is None:
-            cls.__instance = object.__new__(cls)
+            inst = object.__new__(cls)
             if name is None:
                 name = "Logger"
-            cls._str_name = name
-            cls._log = logging(name, level)
-            cls._addHandlers(cls.__instance)
-            cls.manager = Manager(cls._log._log)  # type: ignore
-            cls._setLogs(cls.__instance)
+            if level is None:
+                level = Level.TRACE
+
+            inst._internal = {}
+            inst._parent = None
+            inst._str_name = name
+            inst._logger = logging(name, Level.get(level))
+            inst._addHandlers()
+            cls.__instance = inst
         return cls.__instance
 
-    def _addHandlers(self, level=config().SENTINEL):
-        if level is config().SENTINEL:
-            level = self._level
-        self._log.addHandler(logging.handlers()["StdoutHandler"](level=level))
-        self._log.addHandler(logging.handlers()["FileHandler"](self._logPath()))
+    def __init__(self, *args, **kwargs):
+        pass
 
-    @property
-    def _name(self) -> str:
+    def Child(self, name: str, level=None):
+        """Create a child logger"""
+        if level is None:
+            level = self.get_level()
+        log_inst = _Logger(self, name, level)
+        self._internal[name] = log_inst
+
+    def get_level(self) -> Level:
+        """Get log level"""
+        return self._logger.level
+
+    def set_level(self, level):
+        """Set log level"""
+        self._logger.level = level
+
+    def _addHandlers(self, lvl: Level = config().SENTINEL):  # type: ignore
+        if lvl is config().SENTINEL:
+            lvl: Level = self.get_level()
+        self._logger.mk_handler("stdout", lvl)
+        self._logger.mk_handler("file", self._log_path(), lvl)
+
+    def name(self) -> str:
+        """Return structured name"""
         if self._parent is None:
-            return str(self._str_name)
-        return f"{self._parent._name}.{self._str_name}"
+            return self._str_name
+        return f"{self._parent.name}.{self._str_name}"
 
-    def _logPath(self) -> pathlib.Path:
-        path_sep = self._name.split(".")
+    def _log_path(self) -> pathlib.Path:
+        path_sep = self.name().split(".")
         if len(path_sep) > 1:
             path_sep = path_sep[1:]
         log_path = config().PATH_LOGS
         for idx, item in enumerate(path_sep):
             if idx == len(path_sep) - 1:
                 log_path.mkdir(exist_ok=True, parents=True)
                 item = f"{item}.log"
             log_path /= item
             # print(f"{log_path = }")
         return log_path
 
-    def _setLogs(self):
-        for level in self._log.levels():
-            lname = level.name.lower()
-            log_cmd = (
-                lambda msg, log=self._log, lvl=level.value, *args, **kwargs: log.log(
-                    lvl, msg, *args, **kwargs
-                )
-            )
-            setattr(self, lname, log_cmd)
-
-    if TYPE_CHECKING:
-
-        def __getattr__(self, key):
-            return lambda msg: print(msg)
+    def trace(self, msg):
+        """log.trace"""
+        self._logger.trace(msg)
+
+    def debug(self, msg):
+        """log.debug"""
+        self._logger.debug(msg)
+
+    def info(self, msg):
+        """log.info"""
+        self._logger.info(msg)
+
+    def warn(self, msg):
+        """log.warn"""
+        self._logger.warn(msg)
+
+    def error(self, msg):
+        """log.error"""
+        self._logger.error(msg)
+
+    def exception(self, msg):
+        """log.exception"""
+        self._logger.exception(msg)
 
 
 class _Logger(Logger):
     """Child Logger class"""
 
+    __slots__ = ["_internal", "_parent", "_str_name", "_logger"]
+
     def __new__(cls, *args, **kwargs):
-        return object.__new__(cls)
+        inst = object.__new__(cls)
+        inst.__init__(*args, **kwargs)
+        return inst
 
-    def __init__(self, parent, name):
+    def __init__(self, parent, name: str, level: Level):
+        self._internal = {}
         self._parent = parent
         self._str_name = name
-
-    def _init(self, logger: _logging.Logger, level):
-        self._log = logging(self._name, level, logger)
-        # print(f"{self._log._log.handlers}")
+        self._logger = logging(self.name, level)
         self._addHandlers()
-        # print(f"{self._log._log.handlers}")
-        self._logPath()
-        self._setLogs()
```

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/platform.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/platform.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/profiler.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/profiler.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler/version.py` & `pyboiler_anonoei-0.3.0/src/pyboiler/version.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.5/src/pyboiler_anonoei.egg-info/PKG-INFO` & `pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboiler_anonoei
-Version: 0.0.5
+Version: 0.3.0
 Summary: Various generic python helpers so I don't keep rewriting them
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pyboiler
 Project-URL: Documentation, https://anonoei.github.io/pyboiler/
 Project-URL: Repository, https://github.com/Anonoei/pyboiler.git
 Project-URL: Issues, https://github.com/Anonoei/pyboiler/issues
 Project-URL: Source, https://github.com/anonoei/pyboiler
@@ -14,14 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pdoc3; extra == "dev"
 
 # pyboiler
  Various generic python helpers so I don't keep rewriting them
```


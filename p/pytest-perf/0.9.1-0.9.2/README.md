# Comparing `tmp/pytest-perf-0.9.1.tar.gz` & `tmp/pytest-perf-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-perf-0.9.1.tar", last modified: Sat Jun 26 23:17:02 2021, max compression
+gzip compressed data, was "pytest-perf-0.9.2.tar", last modified: Sat Jun 26 23:49:05 2021, max compression
```

## Comparing `pytest-perf-0.9.1.tar` & `pytest-perf-0.9.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 23:17:02.729092 pytest-perf-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 23:17:02.725092 pytest-perf-0.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 23:17:02.725092 pytest-perf-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-06-26 23:17:02.729092 pytest-perf-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      808 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 23:17:02.725092 pytest-perf-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      814 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      368 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/exercises.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 23:17:02.725092 pytest-perf-0.9.1/pytest_perf/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/pytest_perf/deco.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/pytest_perf/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/pytest_perf/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-26 23:17:02.729092 pytest-perf-0.9.1/pytest_perf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-06-26 23:17:02.000000 pytest-perf-0.9.1/pytest_perf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-06-26 23:17:02.000000 pytest-perf-0.9.1/pytest_perf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-26 23:17:02.000000 pytest-perf-0.9.1/pytest_perf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-26 23:17:02.000000 pytest-perf-0.9.1/pytest_perf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      315 2021-06-26 23:17:02.000000 pytest-perf-0.9.1/pytest_perf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-06-26 23:17:02.000000 pytest-perf-0.9.1/pytest_perf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-06-26 23:17:02.729092 pytest-perf-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2021-06-26 23:16:39.000000 pytest-perf-0.9.1/tox.ini
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2021-06-26 23:49:05.439052 pytest-perf-0.9.2/
+-rw-r--r--   0 jaraco     (501) staff       (20)       99 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/.coveragerc
+-rw-r--r--   0 jaraco     (501) staff       (20)      195 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/.editorconfig
+-rw-r--r--   0 jaraco     (501) staff       (20)      136 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/.flake8
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2021-06-26 23:49:05.433683 pytest-perf-0.9.2/.github/
+-rw-r--r--   0 jaraco     (501) staff       (20)      148 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/.github/dependabot.yml
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2021-06-26 23:49:05.434117 pytest-perf-0.9.2/.github/workflows/
+-rw-r--r--   0 jaraco     (501) staff       (20)     1075 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/.github/workflows/main.yml
+-rw-r--r--   0 jaraco     (501) staff       (20)      175 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 jaraco     (501) staff       (20)       79 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/.readthedocs.yml
+-rw-r--r--   0 jaraco     (501) staff       (20)     1390 2021-06-26 23:47:33.000000 pytest-perf-0.9.2/CHANGES.rst
+-rw-r--r--   0 jaraco     (501) staff       (20)     1050 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/LICENSE
+-rw-r--r--   0 jaraco     (501) staff       (20)     1372 2021-06-26 23:49:05.439281 pytest-perf-0.9.2/PKG-INFO
+-rw-r--r--   0 jaraco     (501) staff       (20)      808 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/README.rst
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2021-06-26 23:49:05.435292 pytest-perf-0.9.2/docs/
+-rw-r--r--   0 jaraco     (501) staff       (20)      814 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/docs/conf.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       81 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/docs/history.rst
+-rw-r--r--   0 jaraco     (501) staff       (20)      295 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/docs/index.rst
+-rw-r--r--   0 jaraco     (501) staff       (20)      368 2021-06-26 22:37:47.000000 pytest-perf-0.9.2/exercises.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       37 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/mypy.ini
+-rw-r--r--   0 jaraco     (501) staff       (20)      367 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/pyproject.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)      416 2021-06-20 01:45:06.000000 pytest-perf-0.9.2/pytest.ini
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2021-06-26 23:49:05.436190 pytest-perf-0.9.2/pytest_perf/
+-rw-r--r--   0 jaraco     (501) staff       (20)      356 2021-06-26 22:37:47.000000 pytest-perf-0.9.2/pytest_perf/deco.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     2939 2021-06-26 23:45:20.000000 pytest-perf-0.9.2/pytest_perf/plugin.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     2812 2021-06-26 22:37:47.000000 pytest-perf-0.9.2/pytest_perf/runner.py
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2021-06-26 23:49:05.438495 pytest-perf-0.9.2/pytest_perf.egg-info/
+-rw-r--r--   0 jaraco     (501) staff       (20)     1372 2021-06-26 23:49:05.000000 pytest-perf-0.9.2/pytest_perf.egg-info/PKG-INFO
+-rw-r--r--   0 jaraco     (501) staff       (20)      551 2021-06-26 23:49:05.000000 pytest-perf-0.9.2/pytest_perf.egg-info/SOURCES.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)        1 2021-06-26 23:49:05.000000 pytest-perf-0.9.2/pytest_perf.egg-info/dependency_links.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)       38 2021-06-26 23:49:05.000000 pytest-perf-0.9.2/pytest_perf.egg-info/entry_points.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)      330 2021-06-26 23:49:05.000000 pytest-perf-0.9.2/pytest_perf.egg-info/requires.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)       12 2021-06-26 23:49:05.000000 pytest-perf-0.9.2/pytest_perf.egg-info/top_level.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)     1137 2021-06-26 23:49:05.440273 pytest-perf-0.9.2/setup.cfg
+-rw-r--r--   0 jaraco     (501) staff       (20)       92 2021-05-29 17:46:53.000000 pytest-perf-0.9.2/setup.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      748 2021-06-20 01:45:06.000000 pytest-perf-0.9.2/tox.ini
```

### Comparing `pytest-perf-0.9.1/.github/workflows/main.yml` & `pytest-perf-0.9.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest-perf-0.9.1/CHANGES.rst` & `pytest-perf-0.9.2/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v0.9.2
+======
+
+Rely on lower level ``importlib.util`` functions to reduce
+the effect of loading a module. Require that modules
+contain 'pytest_perf' in them to be loaded.
+
 v0.9.1
 ======
 
 Suppress exceptions when modules cannot be imported.
 
 v0.9.0
 ======
```

### Comparing `pytest-perf-0.9.1/LICENSE` & `pytest-perf-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-perf-0.9.1/PKG-INFO` & `pytest-perf-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-perf
-Version: 0.9.1
+Version: 0.9.2
 Summary: pytest-perf
 Home-page: https://github.com/jaraco/pytest-perf
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytest-perf-0.9.1/README.rst` & `pytest-perf-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-perf-0.9.1/docs/conf.py` & `pytest-perf-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-perf-0.9.1/pytest_perf/plugin.py` & `pytest-perf-0.9.2/pytest_perf/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import re
 import inspect
 import textwrap
 import contextlib
 
 from typing import List
 from jaraco.functools import assign_params, pass_none, apply
+from jaraco.context import suppress
 from more_itertools import peekable
 
 from pytest_perf import runner
 
 
 def pytest_collect_file(parent, path):
-    if path.basename.endswith('.py'):
+    if path.basename.endswith('.py') and 'pytest_perf' in path.read_text(encoding='utf-8'):
         return File.from_parent(parent, fspath=path)
 
 
 def pytest_terminal_summary(terminalreporter, config):
     items = peekable(filter(None, Experiment._instances))
     items and terminalreporter.section('perf')
     for line in map(str, items):
@@ -39,22 +40,26 @@
             for spec in map(spec_from_func, funcs_from_name(self.name))
         )
 
 
 runner_factory = functools.lru_cache()(runner.BenchmarkRunner)
 
 
+@suppress(Exception)
+def load_module(name):
+    spec = importlib.util.find_spec(name)
+    mod = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(mod)
+    return mod
+
+
 def funcs_from_name(name):
     mod_path, sep, rest = name.rpartition('.')
     mod_name = mod_path.replace('/', '.')
-    try:
-        mod = importlib.import_module(mod_name)
-    except ImportError:
-        # for now, suppress exceptions when a module can't be imported
-        mod = None
+    mod = load_module(mod_name)
     return (
         getattr(mod, name) for name in dir(mod) if re.search(r'(\b|_)perf(\b|_)', name)
     )
 
 
 def first_line(text):
     lines = (line.strip() for line in text.splitlines())
```

### Comparing `pytest-perf-0.9.1/pytest_perf/runner.py` & `pytest-perf-0.9.2/pytest_perf/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-perf-0.9.1/pytest_perf.egg-info/PKG-INFO` & `pytest-perf-0.9.2/pytest_perf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-perf
-Version: 0.9.1
+Version: 0.9.2
 Summary: pytest-perf
 Home-page: https://github.com/jaraco/pytest-perf
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytest-perf-0.9.1/pytest_perf.egg-info/SOURCES.txt` & `pytest-perf-0.9.2/pytest_perf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-perf-0.9.1/setup.cfg` & `pytest-perf-0.9.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	pip-run>=8.5
 	tempora>=4.1
 	jaraco.functools
 	more_itertools
+	jaraco.context
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
```

### Comparing `pytest-perf-0.9.1/tox.ini` & `pytest-perf-0.9.2/tox.ini`

 * *Files identical despite different names*


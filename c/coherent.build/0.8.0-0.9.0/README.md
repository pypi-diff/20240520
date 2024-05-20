# Comparing `tmp/coherent_build-0.8.0.tar.gz` & `tmp/coherent_build-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.8.0.tar", last modified: Sat May 18 18:46:43 2024, max compression
+gzip compressed data, was "coherent_build-0.9.0.tar", last modified: Sat May 18 21:29:04 2024, max compression
```

## Comparing `coherent_build-0.8.0.tar` & `coherent_build-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-18 18:46:42.502695 coherent_build-0.8.0/
--rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.8.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)      268 2024-05-18 18:04:29.832212 coherent_build-0.8.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.8.0/__init__.py.orig
--rw-r--r--   0 jaraco     (501) staff       (20)      533 2024-05-18 18:41:00.726383 coherent_build-0.8.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     5482 2024-05-18 18:04:29.832430 coherent_build-0.8.0/backend.py
--rw-r--r--   0 jaraco     (501) staff       (20)     4436 2024-05-18 18:44:04.428362 coherent_build-0.8.0/discovery.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-18 18:46:42.502769 coherent_build-0.8.0/pyproject.toml
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.8.0/system.toml
--rw-r--r--   0        0        0      611 2024-05-18 18:46:43.826281 coherent_build-0.8.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-18 21:29:03.217234 coherent_build-0.9.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.9.0/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)      268 2024-05-18 18:04:29.832212 coherent_build-0.9.0/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.9.0/__init__.py.orig
+-rw-r--r--   0 jaraco     (501) staff       (20)      533 2024-05-18 18:41:00.726383 coherent_build-0.9.0/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     5605 2024-05-18 20:54:15.887732 coherent_build-0.9.0/backend.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     4885 2024-05-18 21:25:12.307654 coherent_build-0.9.0/discovery.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-18 21:29:03.217311 coherent_build-0.9.0/pyproject.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.9.0/system.toml
+-rw-r--r--   0        0        0      611 2024-05-18 21:29:04.511209 coherent_build-0.9.0/PKG-INFO
```

### Comparing `coherent_build-0.8.0/__init__.py.orig` & `coherent_build-0.9.0/__init__.py.orig`

 * *Files identical despite different names*

### Comparing `coherent_build-0.8.0/__main__.py` & `coherent_build-0.9.0/__main__.py`

 * *Files identical despite different names*

### Comparing `coherent_build-0.8.0/backend.py` & `coherent_build-0.9.0/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,16 +145,19 @@
     def _discover_fields():
         yield 'Metadata-Version', '2.3'
         yield 'Name', discovery.best_name()
         yield 'Version', discovery.version_from_vcs()
         yield 'Author-Email', discovery.author_from_vcs()
         yield 'Summary', discovery.summary_from_github()
         yield 'Requires-Python', discovery.python_requires_supported()
-        for dep in discovery.read_deps():
+        deps = list(discovery.read_deps())
+        for dep in deps:
             yield 'Requires-Dist', dep
+        for extra in discovery.extras_from_deps(deps):
+            yield 'Provides-Extra', extra
         yield 'Project-URL', f'Homepage, {discovery.source_url()}'
         yield from discovery.description_from_readme()
 
     @classmethod
     def from_sdist(cls):
         sdist_metadata = importlib.metadata.PathDistribution(pathlib.Path()).metadata
         return (sdist_metadata or None) and cls(sdist_metadata)
```

### Comparing `coherent_build-0.8.0/discovery.py` & `coherent_build-0.9.0/discovery.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import contextlib
 import functools
 import json
 import logging
+import operator
 import pathlib
 import subprocess
 import types
 import mimetypes
 from collections.abc import Mapping
 
 import jaraco.functools
+import packaging.requirements
 import requests
 import setuptools_scm
 from jaraco.context import suppress
 from pip_run import scripts
 
 
 log = logging.getLogger(__name__)
@@ -116,14 +118,30 @@
 def read_deps():
     """
     Read deps from ``__init__.py``.
     """
     return scripts.DepsReader.search(['__init__.py'])
 
 
+def extras_from_dep(dep):
+    try:
+        markers = packaging.requirements.Requirement(dep).marker._markers
+    except AttributeError:
+        markers = ()
+    return set(
+        marker[2].value
+        for marker in markers
+        if isinstance(marker, tuple) and marker[0].value == 'extra'
+    )
+
+
+def extras_from_deps(deps):
+    return functools.reduce(operator.or_, map(extras_from_dep, deps))
+
+
 def _to_mapping(fame):
     return (dict(zip(fame['columns'], row)) for row in fame['data'])
 
 
 class Contributor(types.SimpleNamespace):
     @property
     def combined_detail(self):
```

### Comparing `coherent_build-0.8.0/PKG-INFO` & `coherent_build-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coherent.build
-Version: 0.8.0
+Version: 0.9.0
 Author-Email: "Jason R. Coombs" <jaraco@jaraco.com>
 Summary: A zero-config Python project build backend
 Requires-Python: >= 3.8
 Requires-Dist: wheel
 Requires-Dist: pip-run
 Requires-Dist: setuptools_scm
 Requires-Dist: build
```


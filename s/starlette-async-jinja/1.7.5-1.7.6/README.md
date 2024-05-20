# Comparing `tmp/starlette_async_jinja-1.7.5.tar.gz` & `tmp/starlette_async_jinja-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_async_jinja-1.7.5.tar", last modified: Fri May 17 14:27:10 2024, max compression
+gzip compressed data, was "starlette_async_jinja-1.7.6.tar", last modified: Mon May 20 11:07:50 2024, max compression
```

## Comparing `starlette_async_jinja-1.7.5.tar` & `starlette_async_jinja-1.7.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 starlette_async_jinja-1.7.5/LICENSE
--rw-r--r--   0        0        0     1535 2024-02-26 07:33:43.485098 starlette_async_jinja-1.7.5/README.md
--rw-r--r--   0        0        0     2353 2024-05-17 14:27:10.694274 starlette_async_jinja-1.7.5/pyproject.toml
--rw-r--r--   0        0        0      211 2023-06-11 12:03:37.580220 starlette_async_jinja-1.7.5/starlette_async_jinja/__init__.py
--rw-r--r--   0        0        0     6344 2024-03-18 08:09:07.321729 starlette_async_jinja-1.7.5/starlette_async_jinja/responses.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 starlette_async_jinja-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 starlette_async_jinja-1.7.6/LICENSE
+-rw-r--r--   0        0        0     1535 2024-02-26 07:33:43.485098 starlette_async_jinja-1.7.6/README.md
+-rw-r--r--   0        0        0     2353 2024-05-20 11:07:50.729989 starlette_async_jinja-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-06-11 12:03:37.580220 starlette_async_jinja-1.7.6/starlette_async_jinja/__init__.py
+-rw-r--r--   0        0        0     6344 2024-03-18 08:09:07.321729 starlette_async_jinja-1.7.6/starlette_async_jinja/responses.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 starlette_async_jinja-1.7.6/PKG-INFO
```

### Comparing `starlette_async_jinja-1.7.5/LICENSE` & `starlette_async_jinja-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.5/README.md` & `starlette_async_jinja-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.5/pyproject.toml` & `starlette_async_jinja-1.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 config = [
     "python.use_venv",
     "true",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "crackerjack>=0.7.19",
+    "crackerjack>=0.7.34",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
@@ -38,33 +38,33 @@
 [tool.creosote]
 paths = [
     "starlette_async_jinja",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
     "pre-commit",
-    "pdm",
-    "pdm-bump",
     "pytest",
-    "python-ulid",
+    "pdm-bump",
     "autotyping",
+    "pdm",
+    "python-ulid",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "starlette_async_jinja",
 ]
 skips = [
     "B404",
+    "B113",
     "B403",
     "B603",
-    "B113",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "starlette_async_jinja",
 ]
@@ -85,20 +85,20 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "starlette-async-jinja"
-version = "1.7.5"
+version = "1.7.6"
 description = ""
 dependencies = [
-    "starlette>=0.34.0",
-    "jinja2>=3.1.2",
-    "jinja2-async-environment>=0.4.2",
+    "starlette>=0.37.2",
+    "jinja2>=3.1.4",
+    "jinja2-async-environment>=0.7.4",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 classifiers = [
```

### Comparing `starlette_async_jinja-1.7.5/starlette_async_jinja/responses.py` & `starlette_async_jinja-1.7.6/starlette_async_jinja/responses.py`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.5/PKG-INFO` & `starlette_async_jinja-1.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-async-jinja
-Version: 1.7.5
+Version: 1.7.6
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
@@ -12,17 +12,17 @@
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Project-URL: Homepage, https://github.com/lesleslie/starlette-async-jinja
 Project-URL: Documentation, https://github.com/lesleslie/starlette-async-jinja
 Project-URL: Repository, https://github.com/lesleslie/starlette-async-jinja
 Requires-Python: >=3.12
-Requires-Dist: starlette>=0.34.0
-Requires-Dist: jinja2>=3.1.2
-Requires-Dist: jinja2-async-environment>=0.4.2
+Requires-Dist: starlette>=0.37.2
+Requires-Dist: jinja2>=3.1.4
+Requires-Dist: jinja2-async-environment>=0.7.4
 Description-Content-Type: text/markdown
 
 # starlette-async-jinja
 
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 ### Jinja2 is_async template support for Starlette +
```


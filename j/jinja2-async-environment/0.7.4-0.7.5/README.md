# Comparing `tmp/jinja2_async_environment-0.7.4.tar.gz` & `tmp/jinja2_async_environment-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_async_environment-0.7.4.tar", last modified: Fri May 17 12:52:31 2024, max compression
+gzip compressed data, was "jinja2_async_environment-0.7.5.tar", last modified: Mon May 20 11:02:56 2024, max compression
```

## Comparing `jinja2_async_environment-0.7.4.tar` & `jinja2_async_environment-0.7.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.7.4/LICENSE
--rw-r--r--   0        0        0      256 2023-08-18 15:51:25.740188 jinja2_async_environment-0.7.4/README.md
--rw-r--r--   0        0        0      497 2023-06-08 14:36:19.764543 jinja2_async_environment-0.7.4/jinja2_async_environment/__init__.py
--rw-r--r--   0        0        0     1419 2024-03-03 12:44:33.505857 jinja2_async_environment-0.7.4/jinja2_async_environment/bccache.py
--rw-r--r--   0        0        0     4669 2024-03-03 08:37:52.586610 jinja2_async_environment-0.7.4/jinja2_async_environment/compiler.py
--rw-r--r--   0        0        0     3524 2024-03-03 13:52:16.395020 jinja2_async_environment-0.7.4/jinja2_async_environment/environment.py
--rw-r--r--   0        0        0     8520 2024-03-03 12:44:33.500636 jinja2_async_environment-0.7.4/jinja2_async_environment/loaders.py
--rw-r--r--   0        0        0     2095 2024-05-17 12:52:31.033753 jinja2_async_environment-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 jinja2_async_environment-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.7.5/LICENSE
+-rw-r--r--   0        0        0      256 2023-08-18 15:51:25.740188 jinja2_async_environment-0.7.5/README.md
+-rw-r--r--   0        0        0      497 2023-06-08 14:36:19.764543 jinja2_async_environment-0.7.5/jinja2_async_environment/__init__.py
+-rw-r--r--   0        0        0     1419 2024-03-03 12:44:33.505857 jinja2_async_environment-0.7.5/jinja2_async_environment/bccache.py
+-rw-r--r--   0        0        0     4669 2024-03-03 08:37:52.586610 jinja2_async_environment-0.7.5/jinja2_async_environment/compiler.py
+-rw-r--r--   0        0        0     3524 2024-03-03 13:52:16.395020 jinja2_async_environment-0.7.5/jinja2_async_environment/environment.py
+-rw-r--r--   0        0        0     8520 2024-03-03 12:44:33.500636 jinja2_async_environment-0.7.5/jinja2_async_environment/loaders.py
+-rw-r--r--   0        0        0     2087 2024-05-20 11:02:56.493043 jinja2_async_environment-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 jinja2_async_environment-0.7.5/PKG-INFO
```

### Comparing `jinja2_async_environment-0.7.4/LICENSE` & `jinja2_async_environment-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.4/jinja2_async_environment/bccache.py` & `jinja2_async_environment-0.7.5/jinja2_async_environment/bccache.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.4/jinja2_async_environment/compiler.py` & `jinja2_async_environment-0.7.5/jinja2_async_environment/compiler.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.4/jinja2_async_environment/environment.py` & `jinja2_async_environment-0.7.5/jinja2_async_environment/environment.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.4/jinja2_async_environment/loaders.py` & `jinja2_async_environment-0.7.5/jinja2_async_environment/loaders.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.4/pyproject.toml` & `jinja2_async_environment-0.7.5/pyproject.toml`

 * *Files 8% similar despite different names*

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
@@ -37,33 +37,33 @@
 
 [tool.creosote]
 paths = [
     "jinja2_async_environment",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pre-commit",
-    "pdm-bump",
-    "pdm",
     "autotyping",
     "pytest",
+    "pdm",
+    "pre-commit",
+    "pdm-bump",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "jinja2_async_environment",
 ]
 skips = [
+    "B603",
     "B403",
     "B113",
     "B404",
-    "B603",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "jinja2_async_environment",
 ]
@@ -84,19 +84,19 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "jinja2-async-environment"
-version = "0.7.4"
+version = "0.7.5"
 description = ""
 dependencies = [
-    "jinja2>=3.1.2",
-    "redis!=5.0.1,>=5.0.0",
+    "jinja2>=3.1.4",
+    "redis>=5.0.4",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 classifiers = [
```

### Comparing `jinja2_async_environment-0.7.4/PKG-INFO` & `jinja2_async_environment-0.7.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: jinja2-async-environment
-Version: 0.7.4
+Version: 0.7.5
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
 Classifier: Framework :: AsyncIO
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.12
-Requires-Dist: jinja2>=3.1.2
-Requires-Dist: redis!=5.0.1,>=5.0.0
+Requires-Dist: jinja2>=3.1.4
+Requires-Dist: redis>=5.0.4
 Description-Content-Type: text/markdown
 
 # jinja2-async-environment
 
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 ### Asynchronous Jinja2 environment and loaders
```


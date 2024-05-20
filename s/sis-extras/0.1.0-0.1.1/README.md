# Comparing `tmp/sis_extras-0.1.0.tar.gz` & `tmp/sis_extras-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sis_extras-0.1.0.tar", last modified: Thu May 16 13:42:53 2024, max compression
+gzip compressed data, was "sis_extras-0.1.1.tar", last modified: Mon May 20 15:22:25 2024, max compression
```

## Comparing `sis_extras-0.1.0.tar` & `sis_extras-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0       13 2024-05-16 13:42:39.451716 sis_extras-0.1.0/README.md
--rw-r--r--   0        0        0      979 2024-05-16 13:42:53.787623 sis_extras-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      204 2024-05-16 13:42:39.451716 sis_extras-0.1.0/src/sis_extras/__init__.py
--rw-r--r--   0        0        0     7992 2024-05-16 13:42:39.451716 sis_extras-0.1.0/src/sis_extras/connection.py
--rw-r--r--   0        0        0     6491 2024-05-16 13:42:39.451716 sis_extras-0.1.0/src/sis_extras/formatting.py
--rw-r--r--   0        0        0        0 2024-05-16 13:42:39.451716 sis_extras-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      111 2024-05-16 13:42:39.451716 sis_extras-0.1.0/tests/test_sis_extras.py
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 sis_extras-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2376 2024-05-20 15:22:10.824790 sis_extras-0.1.1/README.md
+-rw-r--r--   0        0        0     1042 2024-05-20 15:22:25.104809 sis_extras-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      204 2024-05-20 15:22:10.828790 sis_extras-0.1.1/src/sis_extras/__init__.py
+-rw-r--r--   0        0        0     7992 2024-05-20 15:22:10.828790 sis_extras-0.1.1/src/sis_extras/connection.py
+-rw-r--r--   0        0        0     6491 2024-05-20 15:22:10.828790 sis_extras-0.1.1/src/sis_extras/formatting.py
+-rw-r--r--   0        0        0        0 2024-05-20 15:22:10.828790 sis_extras-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      338 2024-05-20 15:22:10.828790 sis_extras-0.1.1/tests/example_app_formatting.py
+-rw-r--r--   0        0        0      523 2024-05-20 15:22:10.828790 sis_extras-0.1.1/tests/test_example_app.py
+-rw-r--r--   0        0        0      111 2024-05-20 15:22:10.828790 sis_extras-0.1.1/tests/test_sis_extras.py
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 sis_extras-0.1.1/PKG-INFO
```

### Comparing `sis_extras-0.1.0/pyproject.toml` & `sis_extras-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [project]
 name = "sis-extras"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python package to make it easy to develop beautiful, performant streamlit-in-snowflake apps"
 authors = [
     { name = "Zachary Blackwood", email = "zblackwo@gmail.com" },
 ]
 dependencies = [
-    "streamlit==1.26.0",
+    "streamlit==1.31.1",
     "snowflake-snowpark-python>=1.13.0",
     "plotly>=5.20.0",
 ]
 requires-python = "==3.8.*"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
+[project.optional-dependencies]
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
+plugins = [
+    "pdm-bump",
+]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.2.0",
 ]
 
 [tool.ruff]
```

### Comparing `sis_extras-0.1.0/src/sis_extras/connection.py` & `sis_extras-0.1.1/src/sis_extras/connection.py`

 * *Files identical despite different names*

### Comparing `sis_extras-0.1.0/src/sis_extras/formatting.py` & `sis_extras-0.1.1/src/sis_extras/formatting.py`

 * *Files identical despite different names*


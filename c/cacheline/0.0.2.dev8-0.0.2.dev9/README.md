# Comparing `tmp/cacheline-0.0.2.dev8.tar.gz` & `tmp/cacheline-0.0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacheline-0.0.2.dev8.tar", max compression
+gzip compressed data, was "cacheline-0.0.2.dev9.tar", max compression
```

## Comparing `cacheline-0.0.2.dev8.tar` & `cacheline-0.0.2.dev9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev8/README.md
--rw-r--r--   0        0        0     1426 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev8/build.py
--rw-r--r--   0        0        0      594 2024-01-08 06:07:46.837360 cacheline-0.0.2.dev8/pyproject.toml
--rw-r--r--   0        0        0       75 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev8/src/cacheline/__init__.py
--rw-r--r--   0        0        0     1721 2024-01-08 06:07:46.837360 cacheline-0.0.2.dev8/src/cacheline/_debug.py
--rw-r--r--   0        0        0       91 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev8/src/cacheline/_internal/tunnel.py
--rw-r--r--   0        0        0      160 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev8/src/cacheline/tests/test_so_import.py
--rw-r--r--   0        0        0     1368 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev8/src/cacheline/web_console.py
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 cacheline-0.0.2.dev8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev9/README.md
+-rw-r--r--   0        0        0     1426 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev9/build.py
+-rw-r--r--   0        0        0      594 2024-01-09 02:22:58.972911 cacheline-0.0.2.dev9/pyproject.toml
+-rw-r--r--   0        0        0       77 2024-01-09 02:22:58.972911 cacheline-0.0.2.dev9/src/cacheline/__init__.py
+-rw-r--r--   0        0        0     2107 2024-01-09 02:22:58.972911 cacheline-0.0.2.dev9/src/cacheline/_debug.py
+-rw-r--r--   0        0        0       91 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev9/src/cacheline/_internal/tunnel.py
+-rw-r--r--   0        0        0      160 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev9/src/cacheline/tests/test_so_import.py
+-rw-r--r--   0        0        0     1368 2023-11-21 23:35:37.428626 cacheline-0.0.2.dev9/src/cacheline/web_console.py
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 cacheline-0.0.2.dev9/PKG-INFO
```

### Comparing `cacheline-0.0.2.dev8/build.py` & `cacheline-0.0.2.dev9/build.py`

 * *Files identical despite different names*

### Comparing `cacheline-0.0.2.dev8/pyproject.toml` & `cacheline-0.0.2.dev9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cacheline"
-version = "0.0.2.dev8"
+version = "0.0.2.dev9"
 description = ""
 authors = ["cache-missing <cache@cache-miss.tech>"]
 readme = "README.md"
 packages = [{ include = "cacheline", from = "src" }]
 include = ["src/cacheline/*.so"]
 build = "build.py"
```

### Comparing `cacheline-0.0.2.dev8/src/cacheline/web_console.py` & `cacheline-0.0.2.dev9/src/cacheline/web_console.py`

 * *Files identical despite different names*

### Comparing `cacheline-0.0.2.dev8/PKG-INFO` & `cacheline-0.0.2.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacheline
-Version: 0.0.2.dev8
+Version: 0.0.2.dev9
 Summary: 
 Author: cache-missing
 Author-email: cache@cache-miss.tech
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


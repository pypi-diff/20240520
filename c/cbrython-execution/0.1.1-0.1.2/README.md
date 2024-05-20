# Comparing `tmp/cbrython_execution-0.1.1.tar.gz` & `tmp/cbrython_execution-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbrython_execution-0.1.1.tar", max compression
+gzip compressed data, was "cbrython_execution-0.1.2.tar", max compression
```

## Comparing `cbrython_execution-0.1.1.tar` & `cbrython_execution-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-17 09:24:21.363693 cbrython_execution-0.1.1/cbrython_execution/__init__.py
--rw-r--r--   0        0        0     2273 2024-05-17 09:24:21.329179 cbrython_execution-0.1.1/cbrython_execution/execution.py
--rw-r--r--   0        0        0      403 2024-05-17 11:28:11.005522 cbrython_execution-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      493 2024-05-17 11:25:39.610131 cbrython_execution-0.1.1/README.md
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 cbrython_execution-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-17 09:24:21.363693 cbrython_execution-0.1.2/cbrython_execution/__init__.py
+-rw-r--r--   0        0        0     2273 2024-05-17 09:24:21.329179 cbrython_execution-0.1.2/cbrython_execution/execution.py
+-rw-r--r--   0        0        0      426 2024-05-20 08:06:26.969970 cbrython_execution-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      493 2024-05-17 11:25:39.610131 cbrython_execution-0.1.2/README.md
+-rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 cbrython_execution-0.1.2/PKG-INFO
```

### Comparing `cbrython_execution-0.1.1/cbrython_execution/execution.py` & `cbrython_execution-0.1.2/cbrython_execution/execution.py`

 * *Files identical despite different names*


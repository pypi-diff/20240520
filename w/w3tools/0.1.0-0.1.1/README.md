# Comparing `tmp/w3tools-0.1.0.tar.gz` & `tmp/w3tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3tools-0.1.0.tar", max compression
+gzip compressed data, was "w3tools-0.1.1.tar", max compression
```

## Comparing `w3tools-0.1.0.tar` & `w3tools-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      870 2024-05-20 11:39:43.544635 w3tools-0.1.0/README.md
--rw-r--r--   0        0        0      339 2024-05-20 11:39:43.544635 w3tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 11:39:43.544635 w3tools-0.1.0/w3tools/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-20 11:39:43.544635 w3tools-0.1.0/w3tools/chain.py
--rw-r--r--   0        0        0      786 2024-05-20 11:39:43.544635 w3tools-0.1.0/w3tools/rpc.py
--rw-r--r--   0        0        0     4161 2024-05-20 11:39:43.544635 w3tools-0.1.0/w3tools/w3.py
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 w3tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      870 2024-05-20 12:01:09.709086 w3tools-0.1.1/README.md
+-rw-r--r--   0        0        0      443 2024-05-20 12:01:09.709086 w3tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 12:01:09.709086 w3tools-0.1.1/w3tools/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-20 12:01:09.709086 w3tools-0.1.1/w3tools/chain.py
+-rw-r--r--   0        0        0      960 2024-05-20 12:01:09.709086 w3tools-0.1.1/w3tools/rpc.py
+-rw-r--r--   0        0        0     4161 2024-05-20 12:01:09.709086 w3tools-0.1.1/w3tools/w3.py
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 w3tools-0.1.1/PKG-INFO
```

### Comparing `w3tools-0.1.0/README.md` & `w3tools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `w3tools-0.1.0/w3tools/chain.py` & `w3tools-0.1.1/w3tools/chain.py`

 * *Files identical despite different names*

### Comparing `w3tools-0.1.0/w3tools/w3.py` & `w3tools-0.1.1/w3tools/w3.py`

 * *Files identical despite different names*

### Comparing `w3tools-0.1.0/PKG-INFO` & `w3tools-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: w3tools
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: w3tools is a Python library that provides a set of tools to enhance the development of Web3 applications
 License: MIT
 Author: wanger
 Author-email: wangereth@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


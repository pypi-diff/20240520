# Comparing `tmp/lib_version_urlphishing-2.2.9.tar.gz` & `tmp/lib_version_urlphishing-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-2.2.9.tar", max compression
+gzip compressed data, was "lib_version_urlphishing-2.3.1.tar", max compression
```

## Comparing `lib_version_urlphishing-2.2.9.tar` & `lib_version_urlphishing-2.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      348 2024-05-20 10:42:14.492831 lib_version_urlphishing-2.2.9/README.md
--rw-r--r--   0        0        0        0 2024-05-20 10:42:14.492831 lib_version_urlphishing-2.2.9/lib_version_URLPhishing/__init__.py
--rw-r--r--   0        0        0       22 2024-05-20 10:42:30.628827 lib_version_urlphishing-2.2.9/lib_version_URLPhishing/version.py
--rw-r--r--   0        0        0      122 2024-05-20 10:42:14.492831 lib_version_urlphishing-2.2.9/lib_version_URLPhishing/version_util.py
--rw-r--r--   0        0        0      827 2024-05-20 10:42:30.552827 lib_version_urlphishing-2.2.9/pyproject.toml
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.2.9/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-05-20 10:55:40.293701 lib_version_urlphishing-2.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 10:55:40.293701 lib_version_urlphishing-2.3.1/lib_version_URLPhishing/__init__.py
+-rw-r--r--   0        0        0       17 2024-05-20 10:55:53.569801 lib_version_urlphishing-2.3.1/lib_version_URLPhishing/version.py
+-rw-r--r--   0        0        0      122 2024-05-20 10:55:40.293701 lib_version_urlphishing-2.3.1/lib_version_URLPhishing/version_util.py
+-rw-r--r--   0        0        0      827 2024-05-20 10:55:54.905810 lib_version_urlphishing-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.3.1/PKG-INFO
```

### Comparing `lib_version_urlphishing-2.2.9/pyproject.toml` & `lib_version_urlphishing-2.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-version-urlphishing"
-version = "2.2.9"
+version = "2.3.1"
 description = "A library to manage and track versions of software components"
 authors = ["Marianna Louizidou <M.Louizidou@student.tudelft.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `lib_version_urlphishing-2.2.9/PKG-INFO` & `lib_version_urlphishing-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-version-urlphishing
-Version: 2.2.9
+Version: 2.3.1
 Summary: A library to manage and track versions of software components
 License: Apache-2.0
 Author: Marianna Louizidou
 Author-email: M.Louizidou@student.tudelft.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```


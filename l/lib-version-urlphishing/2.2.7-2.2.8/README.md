# Comparing `tmp/lib_version_urlphishing-2.2.7.tar.gz` & `tmp/lib_version_urlphishing-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-2.2.7.tar", max compression
+gzip compressed data, was "lib_version_urlphishing-2.2.8.tar", max compression
```

## Comparing `lib_version_urlphishing-2.2.7.tar` & `lib_version_urlphishing-2.2.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      348 2024-05-20 10:16:39.649158 lib_version_urlphishing-2.2.7/README.md
--rw-r--r--   0        0        0        0 2024-05-20 10:16:39.649158 lib_version_urlphishing-2.2.7/lib_version_URLPhishing/__init__.py
--rw-r--r--   0        0        0       22 2024-05-20 10:16:54.213163 lib_version_urlphishing-2.2.7/lib_version_URLPhishing/version.py
--rw-r--r--   0        0        0      122 2024-05-20 10:16:39.649158 lib_version_urlphishing-2.2.7/lib_version_URLPhishing/version_util.py
--rw-r--r--   0        0        0      827 2024-05-20 10:16:54.141163 lib_version_urlphishing-2.2.7/pyproject.toml
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.2.7/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-05-20 10:23:40.587248 lib_version_urlphishing-2.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 10:23:40.587248 lib_version_urlphishing-2.2.8/lib_version_URLPhishing/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-20 10:23:53.991307 lib_version_urlphishing-2.2.8/lib_version_URLPhishing/version.py
+-rw-r--r--   0        0        0      122 2024-05-20 10:23:40.591248 lib_version_urlphishing-2.2.8/lib_version_URLPhishing/version_util.py
+-rw-r--r--   0        0        0      827 2024-05-20 10:23:53.915306 lib_version_urlphishing-2.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.2.8/PKG-INFO
```

### Comparing `lib_version_urlphishing-2.2.7/pyproject.toml` & `lib_version_urlphishing-2.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-version-urlphishing"
-version = "2.2.7"
+version = "2.2.8"
 description = "A library to manage and track versions of software components"
 authors = ["Marianna Louizidou <M.Louizidou@student.tudelft.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `lib_version_urlphishing-2.2.7/PKG-INFO` & `lib_version_urlphishing-2.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-version-urlphishing
-Version: 2.2.7
+Version: 2.2.8
 Summary: A library to manage and track versions of software components
 License: Apache-2.0
 Author: Marianna Louizidou
 Author-email: M.Louizidou@student.tudelft.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

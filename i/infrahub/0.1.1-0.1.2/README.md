# Comparing `tmp/infrahub-0.1.1.tar.gz` & `tmp/infrahub-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahub-0.1.1.tar", max compression
+gzip compressed data, was "infrahub-0.1.2.tar", max compression
```

## Comparing `infrahub-0.1.1.tar` & `infrahub-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0    11340 2024-05-17 09:26:17.612333 infrahub-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1849 2024-05-17 09:20:42.959873 infrahub-0.1.1/README.md
--rw-r--r--   0        0        0       60 2024-05-17 09:20:42.960080 infrahub-0.1.1/infrahub/cli.py
--rw-r--r--   0        0        0      786 2024-05-17 09:20:42.960221 infrahub-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 infrahub-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1849 2024-05-17 09:20:42.959873 infrahub-0.1.2/README.md
+-rw-r--r--   0        0        0       60 2024-05-17 09:20:42.960080 infrahub-0.1.2/infrahub/cli.py
+-rw-r--r--   0        0        0      786 2024-05-20 08:05:06.096987 infrahub-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 infrahub-0.1.2/PKG-INFO
```

### Comparing `infrahub-0.1.1/README.md` & `infrahub-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `infrahub-0.1.1/pyproject.toml` & `infrahub-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "infrahub"
-version = "0.1.1"
+version = "0.1.2"
 description = "Infrahub by OpsMill"
 authors = ["OpsMill <info@opsmill.com>"]
 readme = "README.md"
 packages = [{include = "infrahub"}]
 homepage = "https://opsmill.com"
 repository = "https://github.com/opsmill/infrahub"
 documentation = "https://docs.infrahub.app/"
```

### Comparing `infrahub-0.1.1/PKG-INFO` & `infrahub-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrahub
-Version: 0.1.1
+Version: 0.1.2
 Summary: Infrahub by OpsMill
 Home-page: https://opsmill.com
 Author: OpsMill
 Author-email: info@opsmill.com
 Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```


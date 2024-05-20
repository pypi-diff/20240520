# Comparing `tmp/mypy-boto3-secretsmanager-1.34.7.tar.gz` & `tmp/mypy-boto3-secretsmanager-1.34.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-secretsmanager-1.34.7.tar", last modified: Fri Dec 22 20:32:32 2023, max compression
+gzip compressed data, was "mypy-boto3-secretsmanager-1.34.72.tar", last modified: Wed Mar 27 19:47:06 2024, max compression
```

## Comparing `mypy-boto3-secretsmanager-1.34.7.tar` & `mypy-boto3-secretsmanager-1.34.72.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:32.180704 mypy-boto3-secretsmanager-1.34.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-22 20:32:17.000000 mypy-boto3-secretsmanager-1.34.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13018 2023-12-22 20:32:32.180704 mypy-boto3-secretsmanager-1.34.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2023-12-22 20:32:17.000000 mypy-boto3-secretsmanager-1.34.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:32.180704 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-12-22 20:32:17.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-12-22 20:32:17.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-12-22 20:32:17.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19554 2023-12-22 20:32:18.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19551 2023-12-22 20:32:18.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2023-12-22 20:32:18.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2023-12-22 20:32:18.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-12-22 20:32:18.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-22 20:32:18.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:17.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18274 2023-12-22 20:32:18.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18274 2023-12-22 20:32:18.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-22 20:32:17.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:32.180704 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13018 2023-12-22 20:32:32.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-22 20:32:32.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:32.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:32.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 20:32:32.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-22 20:32:32.000000 mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 20:32:32.180704 mypy-boto3-secretsmanager-1.34.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-12-22 20:32:17.000000 mypy-boto3-secretsmanager-1.34.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:06.378899 mypy-boto3-secretsmanager-1.34.72/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-03-27 19:47:06.378899 mypy-boto3-secretsmanager-1.34.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:06.374899 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19554 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19551 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18287 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18287 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-27 19:46:54.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:47:06.378899 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-03-27 19:47:06.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-27 19:47:06.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:47:06.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:47:06.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 19:47:06.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-27 19:47:06.000000 mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:47:06.378899 mypy-boto3-secretsmanager-1.34.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-27 19:46:53.000000 mypy-boto3-secretsmanager-1.34.72/setup.py
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/LICENSE` & `mypy-boto3-secretsmanager-1.34.72/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/PKG-INFO` & `mypy-boto3-secretsmanager-1.34.72/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.34.7
-Summary: Type annotations for boto3.SecretsManager 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.72
+Summary: Type annotations for boto3.SecretsManager 1.34.72 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-secretsmanager"></a>
 
 # mypy-boto3-secretsmanager
 
 [![PyPI - mypy-boto3-secretsmanager](https://img.shields.io/pypi/v/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-secretsmanager)](https://pepy.tech/project/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/README.md` & `mypy-boto3-secretsmanager-1.34.72/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-secretsmanager)](https://pepy.tech/project/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/__init__.py` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/__init__.pyi` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/__main__.py` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecretsManager 1.34.7\nVersion:         1.34.7\nBuilder"
-        " version: 7.23.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.SecretsManager 1.34.72\n"
+        "Version:         1.34.72\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.7")
+    print("1.34.72")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/client.py` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/client.pyi` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/literals.py` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -78,14 +79,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -201,15 +203,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -383,19 +384,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/literals.pyi` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -78,14 +79,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -201,15 +203,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -383,19 +384,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/paginator.py` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/paginator.pyi` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/type_defs.py` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,18 +106,18 @@
         "Values": NotRequired[Sequence[str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 SecretValueEntryTypeDef = TypedDict(
     "SecretValueEntryTypeDef",
     {
         "ARN": NotRequired[str],
         "Name": NotRequired[str],
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager/type_defs.pyi` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -106,18 +106,18 @@
         "Values": NotRequired[Sequence[str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 SecretValueEntryTypeDef = TypedDict(
     "SecretValueEntryTypeDef",
     {
         "ARN": NotRequired[str],
         "Name": NotRequired[str],
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/PKG-INFO` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-secretsmanager
-Version: 1.34.7
-Summary: Type annotations for boto3.SecretsManager 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.72
+Summary: Type annotations for boto3.SecretsManager 1.34.72 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-secretsmanager"></a>
 
 # mypy-boto3-secretsmanager
 
 [![PyPI - mypy-boto3-secretsmanager](https://img.shields.io/pypi/v/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-secretsmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-secretsmanager)](https://pepy.tech/project/mypy-boto3-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecretsManager 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
+[boto3.SecretsManager 1.34.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-secretsmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_secretsmanager/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-secretsmanager-1.34.7/mypy_boto3_secretsmanager.egg-info/SOURCES.txt` & `mypy-boto3-secretsmanager-1.34.72/mypy_boto3_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-secretsmanager-1.34.7/setup.py` & `mypy-boto3-secretsmanager-1.34.72/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-secretsmanager",
-    version="1.34.7",
+    version="1.34.72",
     packages=["mypy_boto3_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.SecretsManager 1.34.7 service generated with mypy-boto3-builder"
-        " 7.23.0"
-    ),
+    description="Type annotations for boto3.SecretsManager 1.34.72 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


# Comparing `tmp/mypy_boto3_bedrock_agent_runtime-1.34.89.tar.gz` & `tmp/mypy_boto3_bedrock_agent_runtime-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_bedrock_agent_runtime-1.34.89.tar", last modified: Mon Apr 22 19:19:11 2024, max compression
+gzip compressed data, was "mypy_boto3_bedrock_agent_runtime-1.34.90.tar", last modified: Tue Apr 23 19:34:19 2024, max compression
```

## Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89.tar` & `mypy_boto3_bedrock_agent_runtime-1.34.90.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:11.975683 mypy_boto3_bedrock_agent_runtime-1.34.89/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-04-22 19:19:11.975683 mypy_boto3_bedrock_agent_runtime-1.34.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11905 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:11.975683 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21820 2024-04-22 19:18:33.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21820 2024-04-22 19:18:33.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:11.975683 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:19:11.975683 mypy_boto3_bedrock_agent_runtime-1.34.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent_runtime-1.34.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.648559 mypy_boto3_bedrock_agent_runtime-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-04-23 19:34:19.648559 mypy_boto3_bedrock_agent_runtime-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11905 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.648559 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23344 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23344 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:11.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.648559 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:19.648559 mypy_boto3_bedrock_agent_runtime-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent_runtime-1.34.90/setup.py
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/LICENSE` & `mypy_boto3_bedrock_agent_runtime-1.34.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/PKG-INFO` & `mypy_boto3_bedrock_agent_runtime-1.34.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent-runtime
-Version: 1.34.89
-Summary: Type annotations for boto3.AgentsforBedrockRuntime 1.34.89 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.AgentsforBedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-agent-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrockRuntime 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
+[boto3.AgentsforBedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/README.md` & `mypy_boto3_bedrock_agent_runtime-1.34.90/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-agent-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrockRuntime 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
+[boto3.AgentsforBedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/__init__.py` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/__init__.pyi` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/__main__.py` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AgentsforBedrockRuntime 1.34.89\n"
-        "Version:         1.34.89\n"
+        "Type annotations for boto3.AgentsforBedrockRuntime 1.34.90\n"
+        "Version:         1.34.90\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent_runtime//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.89")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/client.py` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/client.pyi` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/literals.py` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "CreationModeType",
+    "ExternalSourceTypeType",
     "InvocationTypeType",
     "PromptTypeType",
     "ResponseStateType",
     "RetrievalResultLocationTypeType",
     "RetrieveAndGenerateTypeType",
     "RetrievePaginatorName",
     "SearchTypeType",
@@ -33,21 +34,22 @@
     "AgentsforBedrockRuntimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 CreationModeType = Literal["DEFAULT", "OVERRIDDEN"]
+ExternalSourceTypeType = Literal["BYTE_CONTENT", "S3"]
 InvocationTypeType = Literal["ACTION_GROUP", "FINISH", "KNOWLEDGE_BASE"]
 PromptTypeType = Literal[
     "KNOWLEDGE_BASE_RESPONSE_GENERATION", "ORCHESTRATION", "POST_PROCESSING", "PRE_PROCESSING"
 ]
 ResponseStateType = Literal["FAILURE", "REPROMPT"]
 RetrievalResultLocationTypeType = Literal["S3"]
-RetrieveAndGenerateTypeType = Literal["KNOWLEDGE_BASE"]
+RetrieveAndGenerateTypeType = Literal["EXTERNAL_SOURCES", "KNOWLEDGE_BASE"]
 RetrievePaginatorName = Literal["retrieve"]
 SearchTypeType = Literal["HYBRID", "SEMANTIC"]
 SourceType = Literal["ACTION_GROUP", "KNOWLEDGE_BASE", "PARSER"]
 TypeType = Literal["ACTION_GROUP", "ASK_USER", "FINISH", "KNOWLEDGE_BASE", "REPROMPT"]
 AgentsforBedrockRuntimeServiceName = Literal["bedrock-agent-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/literals.pyi` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "CreationModeType",
+    "ExternalSourceTypeType",
     "InvocationTypeType",
     "PromptTypeType",
     "ResponseStateType",
     "RetrievalResultLocationTypeType",
     "RetrieveAndGenerateTypeType",
     "RetrievePaginatorName",
     "SearchTypeType",
@@ -33,21 +34,22 @@
     "AgentsforBedrockRuntimeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 CreationModeType = Literal["DEFAULT", "OVERRIDDEN"]
+ExternalSourceTypeType = Literal["BYTE_CONTENT", "S3"]
 InvocationTypeType = Literal["ACTION_GROUP", "FINISH", "KNOWLEDGE_BASE"]
 PromptTypeType = Literal[
     "KNOWLEDGE_BASE_RESPONSE_GENERATION", "ORCHESTRATION", "POST_PROCESSING", "PRE_PROCESSING"
 ]
 ResponseStateType = Literal["FAILURE", "REPROMPT"]
 RetrievalResultLocationTypeType = Literal["S3"]
-RetrieveAndGenerateTypeType = Literal["KNOWLEDGE_BASE"]
+RetrieveAndGenerateTypeType = Literal["EXTERNAL_SOURCES", "KNOWLEDGE_BASE"]
 RetrievePaginatorName = Literal["retrieve"]
 SearchTypeType = Literal["HYBRID", "SEMANTIC"]
 SourceType = Literal["ACTION_GROUP", "KNOWLEDGE_BASE", "PARSER"]
 TypeType = Literal["ACTION_GROUP", "ASK_USER", "FINISH", "KNOWLEDGE_BASE", "REPROMPT"]
 AgentsforBedrockRuntimeServiceName = Literal["bedrock-agent-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/paginator.py` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/paginator.pyi` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/type_defs.py` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,26 @@
     from mypy_boto3_bedrock_agent_runtime.type_defs import AccessDeniedExceptionTypeDef
 
     data: AccessDeniedExceptionTypeDef = ...
     ```
 """
 
 import sys
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.eventstream import EventStream
+from botocore.response import StreamingBody
 
 from .literals import (
     CreationModeType,
+    ExternalSourceTypeType,
     InvocationTypeType,
     PromptTypeType,
     ResponseStateType,
+    RetrieveAndGenerateTypeType,
     SearchTypeType,
     SourceType,
     TypeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -43,21 +46,23 @@
 __all__ = (
     "AccessDeniedExceptionTypeDef",
     "ParameterTypeDef",
     "ActionGroupInvocationOutputTypeDef",
     "ApiParameterTypeDef",
     "ContentBodyTypeDef",
     "BadGatewayExceptionTypeDef",
+    "BlobTypeDef",
     "ConflictExceptionTypeDef",
     "DependencyFailedExceptionTypeDef",
+    "S3ObjectDocTypeDef",
+    "PromptTemplateTypeDef",
     "FailureTraceTypeDef",
     "FilterAttributeTypeDef",
     "FinalResponseTypeDef",
     "FunctionParameterTypeDef",
-    "PromptTemplateTypeDef",
     "InferenceConfigurationTypeDef",
     "InternalServerExceptionTypeDef",
     "KnowledgeBaseLookupInputTypeDef",
     "ResponseMetadataTypeDef",
     "KnowledgeBaseQueryTypeDef",
     "KnowledgeBaseVectorSearchConfigurationTypeDef",
     "RetrievalResultContentTypeDef",
@@ -75,48 +80,52 @@
     "RetrieveAndGenerateOutputTypeDef",
     "RetrieveAndGenerateSessionConfigurationTypeDef",
     "SpanTypeDef",
     "PropertyParametersTypeDef",
     "RequestBodyTypeDef",
     "ApiResultTypeDef",
     "FunctionResultTypeDef",
+    "ByteContentDocTypeDef",
+    "ExternalSourcesGenerationConfigurationTypeDef",
+    "GenerationConfigurationTypeDef",
     "RetrievalFilterTypeDef",
     "FunctionInvocationInputTypeDef",
-    "GenerationConfigurationTypeDef",
     "ModelInvocationInputTypeDef",
     "KnowledgeBaseRetrievalConfigurationTypeDef",
     "PostProcessingModelInvocationOutputTypeDef",
     "PreProcessingModelInvocationOutputTypeDef",
     "RetrievalResultLocationTypeDef",
     "TextResponsePartTypeDef",
     "ApiRequestBodyTypeDef",
     "ActionGroupInvocationInputTypeDef",
     "InvocationResultMemberTypeDef",
+    "ExternalSourceTypeDef",
     "KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef",
     "RetrieveRequestRequestTypeDef",
     "RetrieveRequestRetrievePaginateTypeDef",
     "PostProcessingTraceTypeDef",
     "PreProcessingTraceTypeDef",
     "KnowledgeBaseRetrievalResultTypeDef",
     "RetrievedReferenceTypeDef",
     "GeneratedResponsePartTypeDef",
     "ApiInvocationInputTypeDef",
     "InvocationInputTypeDef",
     "SessionStateTypeDef",
-    "RetrieveAndGenerateConfigurationTypeDef",
+    "ExternalSourcesRetrieveAndGenerateConfigurationTypeDef",
     "RetrieveResponseTypeDef",
     "KnowledgeBaseLookupOutputTypeDef",
     "CitationTypeDef",
     "InvocationInputMemberTypeDef",
     "InvokeAgentRequestRequestTypeDef",
-    "RetrieveAndGenerateRequestRequestTypeDef",
+    "RetrieveAndGenerateConfigurationTypeDef",
     "ObservationTypeDef",
     "AttributionTypeDef",
     "RetrieveAndGenerateResponseTypeDef",
     "ReturnControlPayloadTypeDef",
+    "RetrieveAndGenerateRequestRequestTypeDef",
     "OrchestrationTraceTypeDef",
     "PayloadPartTypeDef",
     "TraceTypeDef",
     "TracePartTypeDef",
     "ResponseStreamTypeDef",
     "InvokeAgentResponseTypeDef",
 )
@@ -158,27 +167,40 @@
 BadGatewayExceptionTypeDef = TypedDict(
     "BadGatewayExceptionTypeDef",
     {
         "message": NotRequired[str],
         "resourceName": NotRequired[str],
     },
 )
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConflictExceptionTypeDef = TypedDict(
     "ConflictExceptionTypeDef",
     {
         "message": NotRequired[str],
     },
 )
 DependencyFailedExceptionTypeDef = TypedDict(
     "DependencyFailedExceptionTypeDef",
     {
         "message": NotRequired[str],
         "resourceName": NotRequired[str],
     },
 )
+S3ObjectDocTypeDef = TypedDict(
+    "S3ObjectDocTypeDef",
+    {
+        "uri": str,
+    },
+)
+PromptTemplateTypeDef = TypedDict(
+    "PromptTemplateTypeDef",
+    {
+        "textPromptTemplate": NotRequired[str],
+    },
+)
 FailureTraceTypeDef = TypedDict(
     "FailureTraceTypeDef",
     {
         "failureReason": NotRequired[str],
         "traceId": NotRequired[str],
     },
 )
@@ -199,20 +221,14 @@
     "FunctionParameterTypeDef",
     {
         "name": NotRequired[str],
         "type": NotRequired[str],
         "value": NotRequired[str],
     },
 )
-PromptTemplateTypeDef = TypedDict(
-    "PromptTemplateTypeDef",
-    {
-        "textPromptTemplate": NotRequired[str],
-    },
-)
 InferenceConfigurationTypeDef = TypedDict(
     "InferenceConfigurationTypeDef",
     {
         "maximumLength": NotRequired[int],
         "stopSequences": NotRequired[List[str]],
         "temperature": NotRequired[float],
         "topK": NotRequired[int],
@@ -380,14 +396,34 @@
     {
         "actionGroup": str,
         "function": NotRequired[str],
         "responseBody": NotRequired[Mapping[str, ContentBodyTypeDef]],
         "responseState": NotRequired[ResponseStateType],
     },
 )
+ByteContentDocTypeDef = TypedDict(
+    "ByteContentDocTypeDef",
+    {
+        "contentType": str,
+        "data": BlobTypeDef,
+        "identifier": str,
+    },
+)
+ExternalSourcesGenerationConfigurationTypeDef = TypedDict(
+    "ExternalSourcesGenerationConfigurationTypeDef",
+    {
+        "promptTemplate": NotRequired[PromptTemplateTypeDef],
+    },
+)
+GenerationConfigurationTypeDef = TypedDict(
+    "GenerationConfigurationTypeDef",
+    {
+        "promptTemplate": NotRequired[PromptTemplateTypeDef],
+    },
+)
 RetrievalFilterTypeDef = TypedDict(
     "RetrievalFilterTypeDef",
     {
         "andAll": NotRequired[Sequence[Dict[str, Any]]],
         "equals": NotRequired[FilterAttributeTypeDef],
         "greaterThan": NotRequired[FilterAttributeTypeDef],
         "greaterThanOrEquals": NotRequired[FilterAttributeTypeDef],
@@ -404,20 +440,14 @@
     "FunctionInvocationInputTypeDef",
     {
         "actionGroup": str,
         "function": NotRequired[str],
         "parameters": NotRequired[List[FunctionParameterTypeDef]],
     },
 )
-GenerationConfigurationTypeDef = TypedDict(
-    "GenerationConfigurationTypeDef",
-    {
-        "promptTemplate": NotRequired[PromptTemplateTypeDef],
-    },
-)
 ModelInvocationInputTypeDef = TypedDict(
     "ModelInvocationInputTypeDef",
     {
         "inferenceConfiguration": NotRequired[InferenceConfigurationTypeDef],
         "overrideLambda": NotRequired[str],
         "parserMode": NotRequired[CreationModeType],
         "promptCreationMode": NotRequired[CreationModeType],
@@ -480,14 +510,22 @@
 InvocationResultMemberTypeDef = TypedDict(
     "InvocationResultMemberTypeDef",
     {
         "apiResult": NotRequired[ApiResultTypeDef],
         "functionResult": NotRequired[FunctionResultTypeDef],
     },
 )
+ExternalSourceTypeDef = TypedDict(
+    "ExternalSourceTypeDef",
+    {
+        "sourceType": ExternalSourceTypeType,
+        "byteContent": NotRequired[ByteContentDocTypeDef],
+        "s3Location": NotRequired[S3ObjectDocTypeDef],
+    },
+)
 KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef = TypedDict(
     "KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef",
     {
         "knowledgeBaseId": str,
         "modelArn": str,
         "generationConfiguration": NotRequired[GenerationConfigurationTypeDef],
         "retrievalConfiguration": NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],
@@ -572,21 +610,20 @@
     {
         "invocationId": NotRequired[str],
         "promptSessionAttributes": NotRequired[Mapping[str, str]],
         "returnControlInvocationResults": NotRequired[Sequence[InvocationResultMemberTypeDef]],
         "sessionAttributes": NotRequired[Mapping[str, str]],
     },
 )
-RetrieveAndGenerateConfigurationTypeDef = TypedDict(
-    "RetrieveAndGenerateConfigurationTypeDef",
+ExternalSourcesRetrieveAndGenerateConfigurationTypeDef = TypedDict(
+    "ExternalSourcesRetrieveAndGenerateConfigurationTypeDef",
     {
-        "type": Literal["KNOWLEDGE_BASE"],
-        "knowledgeBaseConfiguration": NotRequired[
-            KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef
-        ],
+        "modelArn": str,
+        "sources": Sequence[ExternalSourceTypeDef],
+        "generationConfiguration": NotRequired[ExternalSourcesGenerationConfigurationTypeDef],
     },
 )
 RetrieveResponseTypeDef = TypedDict(
     "RetrieveResponseTypeDef",
     {
         "nextToken": str,
         "retrievalResults": List[KnowledgeBaseRetrievalResultTypeDef],
@@ -621,21 +658,24 @@
         "sessionId": str,
         "enableTrace": NotRequired[bool],
         "endSession": NotRequired[bool],
         "inputText": NotRequired[str],
         "sessionState": NotRequired[SessionStateTypeDef],
     },
 )
-RetrieveAndGenerateRequestRequestTypeDef = TypedDict(
-    "RetrieveAndGenerateRequestRequestTypeDef",
+RetrieveAndGenerateConfigurationTypeDef = TypedDict(
+    "RetrieveAndGenerateConfigurationTypeDef",
     {
-        "input": RetrieveAndGenerateInputTypeDef,
-        "retrieveAndGenerateConfiguration": NotRequired[RetrieveAndGenerateConfigurationTypeDef],
-        "sessionConfiguration": NotRequired[RetrieveAndGenerateSessionConfigurationTypeDef],
-        "sessionId": NotRequired[str],
+        "type": RetrieveAndGenerateTypeType,
+        "externalSourcesConfiguration": NotRequired[
+            ExternalSourcesRetrieveAndGenerateConfigurationTypeDef
+        ],
+        "knowledgeBaseConfiguration": NotRequired[
+            KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef
+        ],
     },
 )
 ObservationTypeDef = TypedDict(
     "ObservationTypeDef",
     {
         "actionGroupInvocationOutput": NotRequired[ActionGroupInvocationOutputTypeDef],
         "finalResponse": NotRequired[FinalResponseTypeDef],
@@ -663,14 +703,23 @@
 ReturnControlPayloadTypeDef = TypedDict(
     "ReturnControlPayloadTypeDef",
     {
         "invocationId": NotRequired[str],
         "invocationInputs": NotRequired[List[InvocationInputMemberTypeDef]],
     },
 )
+RetrieveAndGenerateRequestRequestTypeDef = TypedDict(
+    "RetrieveAndGenerateRequestRequestTypeDef",
+    {
+        "input": RetrieveAndGenerateInputTypeDef,
+        "retrieveAndGenerateConfiguration": NotRequired[RetrieveAndGenerateConfigurationTypeDef],
+        "sessionConfiguration": NotRequired[RetrieveAndGenerateSessionConfigurationTypeDef],
+        "sessionId": NotRequired[str],
+    },
+)
 OrchestrationTraceTypeDef = TypedDict(
     "OrchestrationTraceTypeDef",
     {
         "invocationInput": NotRequired[InvocationInputTypeDef],
         "modelInvocationInput": NotRequired[ModelInvocationInputTypeDef],
         "observation": NotRequired[ObservationTypeDef],
         "rationale": NotRequired[RationaleTypeDef],
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime/type_defs.pyi` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,26 @@
     from mypy_boto3_bedrock_agent_runtime.type_defs import AccessDeniedExceptionTypeDef
 
     data: AccessDeniedExceptionTypeDef = ...
     ```
 """
 
 import sys
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.eventstream import EventStream
+from botocore.response import StreamingBody
 
 from .literals import (
     CreationModeType,
+    ExternalSourceTypeType,
     InvocationTypeType,
     PromptTypeType,
     ResponseStateType,
+    RetrieveAndGenerateTypeType,
     SearchTypeType,
     SourceType,
     TypeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -43,21 +46,23 @@
 __all__ = (
     "AccessDeniedExceptionTypeDef",
     "ParameterTypeDef",
     "ActionGroupInvocationOutputTypeDef",
     "ApiParameterTypeDef",
     "ContentBodyTypeDef",
     "BadGatewayExceptionTypeDef",
+    "BlobTypeDef",
     "ConflictExceptionTypeDef",
     "DependencyFailedExceptionTypeDef",
+    "S3ObjectDocTypeDef",
+    "PromptTemplateTypeDef",
     "FailureTraceTypeDef",
     "FilterAttributeTypeDef",
     "FinalResponseTypeDef",
     "FunctionParameterTypeDef",
-    "PromptTemplateTypeDef",
     "InferenceConfigurationTypeDef",
     "InternalServerExceptionTypeDef",
     "KnowledgeBaseLookupInputTypeDef",
     "ResponseMetadataTypeDef",
     "KnowledgeBaseQueryTypeDef",
     "KnowledgeBaseVectorSearchConfigurationTypeDef",
     "RetrievalResultContentTypeDef",
@@ -75,48 +80,52 @@
     "RetrieveAndGenerateOutputTypeDef",
     "RetrieveAndGenerateSessionConfigurationTypeDef",
     "SpanTypeDef",
     "PropertyParametersTypeDef",
     "RequestBodyTypeDef",
     "ApiResultTypeDef",
     "FunctionResultTypeDef",
+    "ByteContentDocTypeDef",
+    "ExternalSourcesGenerationConfigurationTypeDef",
+    "GenerationConfigurationTypeDef",
     "RetrievalFilterTypeDef",
     "FunctionInvocationInputTypeDef",
-    "GenerationConfigurationTypeDef",
     "ModelInvocationInputTypeDef",
     "KnowledgeBaseRetrievalConfigurationTypeDef",
     "PostProcessingModelInvocationOutputTypeDef",
     "PreProcessingModelInvocationOutputTypeDef",
     "RetrievalResultLocationTypeDef",
     "TextResponsePartTypeDef",
     "ApiRequestBodyTypeDef",
     "ActionGroupInvocationInputTypeDef",
     "InvocationResultMemberTypeDef",
+    "ExternalSourceTypeDef",
     "KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef",
     "RetrieveRequestRequestTypeDef",
     "RetrieveRequestRetrievePaginateTypeDef",
     "PostProcessingTraceTypeDef",
     "PreProcessingTraceTypeDef",
     "KnowledgeBaseRetrievalResultTypeDef",
     "RetrievedReferenceTypeDef",
     "GeneratedResponsePartTypeDef",
     "ApiInvocationInputTypeDef",
     "InvocationInputTypeDef",
     "SessionStateTypeDef",
-    "RetrieveAndGenerateConfigurationTypeDef",
+    "ExternalSourcesRetrieveAndGenerateConfigurationTypeDef",
     "RetrieveResponseTypeDef",
     "KnowledgeBaseLookupOutputTypeDef",
     "CitationTypeDef",
     "InvocationInputMemberTypeDef",
     "InvokeAgentRequestRequestTypeDef",
-    "RetrieveAndGenerateRequestRequestTypeDef",
+    "RetrieveAndGenerateConfigurationTypeDef",
     "ObservationTypeDef",
     "AttributionTypeDef",
     "RetrieveAndGenerateResponseTypeDef",
     "ReturnControlPayloadTypeDef",
+    "RetrieveAndGenerateRequestRequestTypeDef",
     "OrchestrationTraceTypeDef",
     "PayloadPartTypeDef",
     "TraceTypeDef",
     "TracePartTypeDef",
     "ResponseStreamTypeDef",
     "InvokeAgentResponseTypeDef",
 )
@@ -158,27 +167,40 @@
 BadGatewayExceptionTypeDef = TypedDict(
     "BadGatewayExceptionTypeDef",
     {
         "message": NotRequired[str],
         "resourceName": NotRequired[str],
     },
 )
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConflictExceptionTypeDef = TypedDict(
     "ConflictExceptionTypeDef",
     {
         "message": NotRequired[str],
     },
 )
 DependencyFailedExceptionTypeDef = TypedDict(
     "DependencyFailedExceptionTypeDef",
     {
         "message": NotRequired[str],
         "resourceName": NotRequired[str],
     },
 )
+S3ObjectDocTypeDef = TypedDict(
+    "S3ObjectDocTypeDef",
+    {
+        "uri": str,
+    },
+)
+PromptTemplateTypeDef = TypedDict(
+    "PromptTemplateTypeDef",
+    {
+        "textPromptTemplate": NotRequired[str],
+    },
+)
 FailureTraceTypeDef = TypedDict(
     "FailureTraceTypeDef",
     {
         "failureReason": NotRequired[str],
         "traceId": NotRequired[str],
     },
 )
@@ -199,20 +221,14 @@
     "FunctionParameterTypeDef",
     {
         "name": NotRequired[str],
         "type": NotRequired[str],
         "value": NotRequired[str],
     },
 )
-PromptTemplateTypeDef = TypedDict(
-    "PromptTemplateTypeDef",
-    {
-        "textPromptTemplate": NotRequired[str],
-    },
-)
 InferenceConfigurationTypeDef = TypedDict(
     "InferenceConfigurationTypeDef",
     {
         "maximumLength": NotRequired[int],
         "stopSequences": NotRequired[List[str]],
         "temperature": NotRequired[float],
         "topK": NotRequired[int],
@@ -380,14 +396,34 @@
     {
         "actionGroup": str,
         "function": NotRequired[str],
         "responseBody": NotRequired[Mapping[str, ContentBodyTypeDef]],
         "responseState": NotRequired[ResponseStateType],
     },
 )
+ByteContentDocTypeDef = TypedDict(
+    "ByteContentDocTypeDef",
+    {
+        "contentType": str,
+        "data": BlobTypeDef,
+        "identifier": str,
+    },
+)
+ExternalSourcesGenerationConfigurationTypeDef = TypedDict(
+    "ExternalSourcesGenerationConfigurationTypeDef",
+    {
+        "promptTemplate": NotRequired[PromptTemplateTypeDef],
+    },
+)
+GenerationConfigurationTypeDef = TypedDict(
+    "GenerationConfigurationTypeDef",
+    {
+        "promptTemplate": NotRequired[PromptTemplateTypeDef],
+    },
+)
 RetrievalFilterTypeDef = TypedDict(
     "RetrievalFilterTypeDef",
     {
         "andAll": NotRequired[Sequence[Dict[str, Any]]],
         "equals": NotRequired[FilterAttributeTypeDef],
         "greaterThan": NotRequired[FilterAttributeTypeDef],
         "greaterThanOrEquals": NotRequired[FilterAttributeTypeDef],
@@ -404,20 +440,14 @@
     "FunctionInvocationInputTypeDef",
     {
         "actionGroup": str,
         "function": NotRequired[str],
         "parameters": NotRequired[List[FunctionParameterTypeDef]],
     },
 )
-GenerationConfigurationTypeDef = TypedDict(
-    "GenerationConfigurationTypeDef",
-    {
-        "promptTemplate": NotRequired[PromptTemplateTypeDef],
-    },
-)
 ModelInvocationInputTypeDef = TypedDict(
     "ModelInvocationInputTypeDef",
     {
         "inferenceConfiguration": NotRequired[InferenceConfigurationTypeDef],
         "overrideLambda": NotRequired[str],
         "parserMode": NotRequired[CreationModeType],
         "promptCreationMode": NotRequired[CreationModeType],
@@ -480,14 +510,22 @@
 InvocationResultMemberTypeDef = TypedDict(
     "InvocationResultMemberTypeDef",
     {
         "apiResult": NotRequired[ApiResultTypeDef],
         "functionResult": NotRequired[FunctionResultTypeDef],
     },
 )
+ExternalSourceTypeDef = TypedDict(
+    "ExternalSourceTypeDef",
+    {
+        "sourceType": ExternalSourceTypeType,
+        "byteContent": NotRequired[ByteContentDocTypeDef],
+        "s3Location": NotRequired[S3ObjectDocTypeDef],
+    },
+)
 KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef = TypedDict(
     "KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef",
     {
         "knowledgeBaseId": str,
         "modelArn": str,
         "generationConfiguration": NotRequired[GenerationConfigurationTypeDef],
         "retrievalConfiguration": NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],
@@ -572,21 +610,20 @@
     {
         "invocationId": NotRequired[str],
         "promptSessionAttributes": NotRequired[Mapping[str, str]],
         "returnControlInvocationResults": NotRequired[Sequence[InvocationResultMemberTypeDef]],
         "sessionAttributes": NotRequired[Mapping[str, str]],
     },
 )
-RetrieveAndGenerateConfigurationTypeDef = TypedDict(
-    "RetrieveAndGenerateConfigurationTypeDef",
+ExternalSourcesRetrieveAndGenerateConfigurationTypeDef = TypedDict(
+    "ExternalSourcesRetrieveAndGenerateConfigurationTypeDef",
     {
-        "type": Literal["KNOWLEDGE_BASE"],
-        "knowledgeBaseConfiguration": NotRequired[
-            KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef
-        ],
+        "modelArn": str,
+        "sources": Sequence[ExternalSourceTypeDef],
+        "generationConfiguration": NotRequired[ExternalSourcesGenerationConfigurationTypeDef],
     },
 )
 RetrieveResponseTypeDef = TypedDict(
     "RetrieveResponseTypeDef",
     {
         "nextToken": str,
         "retrievalResults": List[KnowledgeBaseRetrievalResultTypeDef],
@@ -621,21 +658,24 @@
         "sessionId": str,
         "enableTrace": NotRequired[bool],
         "endSession": NotRequired[bool],
         "inputText": NotRequired[str],
         "sessionState": NotRequired[SessionStateTypeDef],
     },
 )
-RetrieveAndGenerateRequestRequestTypeDef = TypedDict(
-    "RetrieveAndGenerateRequestRequestTypeDef",
+RetrieveAndGenerateConfigurationTypeDef = TypedDict(
+    "RetrieveAndGenerateConfigurationTypeDef",
     {
-        "input": RetrieveAndGenerateInputTypeDef,
-        "retrieveAndGenerateConfiguration": NotRequired[RetrieveAndGenerateConfigurationTypeDef],
-        "sessionConfiguration": NotRequired[RetrieveAndGenerateSessionConfigurationTypeDef],
-        "sessionId": NotRequired[str],
+        "type": RetrieveAndGenerateTypeType,
+        "externalSourcesConfiguration": NotRequired[
+            ExternalSourcesRetrieveAndGenerateConfigurationTypeDef
+        ],
+        "knowledgeBaseConfiguration": NotRequired[
+            KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef
+        ],
     },
 )
 ObservationTypeDef = TypedDict(
     "ObservationTypeDef",
     {
         "actionGroupInvocationOutput": NotRequired[ActionGroupInvocationOutputTypeDef],
         "finalResponse": NotRequired[FinalResponseTypeDef],
@@ -663,14 +703,23 @@
 ReturnControlPayloadTypeDef = TypedDict(
     "ReturnControlPayloadTypeDef",
     {
         "invocationId": NotRequired[str],
         "invocationInputs": NotRequired[List[InvocationInputMemberTypeDef]],
     },
 )
+RetrieveAndGenerateRequestRequestTypeDef = TypedDict(
+    "RetrieveAndGenerateRequestRequestTypeDef",
+    {
+        "input": RetrieveAndGenerateInputTypeDef,
+        "retrieveAndGenerateConfiguration": NotRequired[RetrieveAndGenerateConfigurationTypeDef],
+        "sessionConfiguration": NotRequired[RetrieveAndGenerateSessionConfigurationTypeDef],
+        "sessionId": NotRequired[str],
+    },
+)
 OrchestrationTraceTypeDef = TypedDict(
     "OrchestrationTraceTypeDef",
     {
         "invocationInput": NotRequired[InvocationInputTypeDef],
         "modelInvocationInput": NotRequired[ModelInvocationInputTypeDef],
         "observation": NotRequired[ObservationTypeDef],
         "rationale": NotRequired[RationaleTypeDef],
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/PKG-INFO` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent-runtime
-Version: 1.34.89
-Summary: Type annotations for boto3.AgentsforBedrockRuntime 1.34.89 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.AgentsforBedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent-runtime)](https://pepy.tech/project/mypy-boto3-bedrock-agent-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrockRuntime 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
+[boto3.AgentsforBedrockRuntime 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/mypy_boto3_bedrock_agent_runtime.egg-info/SOURCES.txt` & `mypy_boto3_bedrock_agent_runtime-1.34.90/mypy_boto3_bedrock_agent_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent_runtime-1.34.89/setup.py` & `mypy_boto3_bedrock_agent_runtime-1.34.90/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-bedrock-agent-runtime",
-    version="1.34.89",
+    version="1.34.90",
     packages=["mypy_boto3_bedrock_agent_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.AgentsforBedrockRuntime 1.34.89 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.AgentsforBedrockRuntime 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```


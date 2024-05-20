# Comparing `tmp/reasonify_headless-0.1.0a6.tar.gz` & `tmp/reasonify_headless-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasonify_headless-0.1.0a6.tar", last modified: Mon May 20 05:58:47 2024, max compression
+gzip compressed data, was "reasonify_headless-0.1.0a7.tar", last modified: Mon May 20 10:33:42 2024, max compression
```

## Comparing `reasonify_headless-0.1.0a6.tar` & `reasonify_headless-0.1.0a7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1231 2024-05-20 05:58:47.560312 reasonify_headless-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/__init__.py
--rw-r--r--   0        0        0     2392 2024-05-20 04:51:28.420660 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/core/loop.py
--rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/__init__.py
--rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/async.yaml
--rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/date.yaml
--rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/dir.yaml
--rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/search.yaml
--rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/simple_ask.yaml
--rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/models/shot.py
--rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/__init__.py
--rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/chat.j2
--rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/main.j2
--rw-r--r--   0        0        0      235 2024-05-20 04:51:32.391086 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/__init__.py
--rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/fetch.py
--rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/input.py
--rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/install.py
--rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/component.py
--rw-r--r--   0        0        0     1976 2024-05-20 05:44:37.361696 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/context.py
--rw-r--r--   0        0        0     1187 2024-05-20 03:17:42.705230 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/inject.py
--rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/queue.py
--rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/run.py
--rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/serialize.py
--rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/tool.py
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1260 2024-05-20 10:33:42.685641 reasonify_headless-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/__init__.py
+-rw-r--r--   0        0        0     2392 2024-05-20 04:51:28.420660 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/core/loop.py
+-rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/async.yaml
+-rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/date.yaml
+-rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/dir.yaml
+-rw-r--r--   0        0        0      498 2024-05-20 10:13:22.067039 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/file.yaml
+-rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/search.yaml
+-rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/simple_ask.yaml
+-rw-r--r--   0        0        0     1242 2024-05-20 10:12:00.953910 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/models/shot.py
+-rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/templates/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/templates/chat.j2
+-rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/templates/main.j2
+-rw-r--r--   0        0        0      235 2024-05-20 04:51:32.391086 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/tools/__init__.py
+-rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/tools/fetch.py
+-rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/tools/input.py
+-rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/tools/install.py
+-rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/component.py
+-rw-r--r--   0        0        0     1976 2024-05-20 05:44:37.361696 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/context.py
+-rw-r--r--   0        0        0     1187 2024-05-20 03:17:42.705230 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/inject.py
+-rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/queue.py
+-rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/run.py
+-rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/serialize.py
+-rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/tool.py
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a7/PKG-INFO
```

### Comparing `reasonify_headless-0.1.0a6/pyproject.toml` & `reasonify_headless-0.1.0a7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "pyodide-py~=0.26.0a4 ; sys_platform != 'emscripten'",
     "promplate~=0.3.4.7",
     "python-box~=7.1.1",
     "promptools[validation]~=0.1.3.4",
     "promplate-recipes~=0.2.2.1",
     "pyyaml~=6.0.1",
 ]
-version = "0.1.0a6"
+version = "0.1.0a7"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -39,14 +39,15 @@
 dev = [
     "black>=24.4.2",
     "isort>=5.13.2",
     "ruff>=0.4.4",
     "watchfiles>=0.21.0",
     "micropip~=0.6.0",
     "webtypy~=0.1.7",
+    "python-slugify~=8.0.4",
 ]
 
 [tool.pdm.scripts.fmt]
 composite = [
     "ruff check --fix --exit-zero",
     "isort .",
     "black .",
```

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/core/loop.py` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/core/loop.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/async.yaml` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/async.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/search.yaml` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/examples/search.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/models/shot.py` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/models/shot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+from typing import Literal
+
 from promplate.prompt.chat import Message, assistant, system, user
 from pydantic import BaseModel, Field
 
 from ..utils.run import run
 from ..utils.serialize import json
 
 
 class Run(BaseModel):
     source: str
-    result: dict | None = None
+    result: dict | Literal[False] | None = None
 
-    async def ensure_result(self) -> dict:
-        return self.result if self.result is not None else await run(self.source)
+    async def ensure_result(self) -> dict | str:
+        match self.result:
+            case False:
+                return "<omitted>"
+            case None:
+                return await run(self.source)
+            case _:
+                return self.result
 
 
 class Shot(BaseModel):
     title: str = Field(pattern=r"[a-z_0-9]+")
 
     interactions: list[list[Run] | str]
```

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/__init__.py` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/main.j2` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/templates/main.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/fetch.py` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/tools/fetch.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/context.py` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/context.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/inject.py` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/inject.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/run.py` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/run.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/tool.py` & `reasonify_headless-0.1.0a7/reasonify-headless/reasonify/utils/tool.py`

 * *Files identical despite different names*


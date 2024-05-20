# Comparing `tmp/reasonify_headless-0.1.0a5.tar.gz` & `tmp/reasonify_headless-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasonify_headless-0.1.0a5.tar", last modified: Mon May 20 04:02:40 2024, max compression
+gzip compressed data, was "reasonify_headless-0.1.0a6.tar", last modified: Mon May 20 05:58:47 2024, max compression
```

## Comparing `reasonify_headless-0.1.0a5.tar` & `reasonify_headless-0.1.0a6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1231 2024-05-20 04:02:40.244475 reasonify_headless-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/__init__.py
--rw-r--r--   0        0        0     2376 2024-05-20 03:58:36.431514 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/core/loop.py
--rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/__init__.py
--rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/async.yaml
--rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/date.yaml
--rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/dir.yaml
--rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/search.yaml
--rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/simple_ask.yaml
--rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/models/shot.py
--rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/__init__.py
--rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/chat.j2
--rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/main.j2
--rw-r--r--   0        0        0      242 2024-05-19 12:29:46.617624 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/__init__.py
--rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/fetch.py
--rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/input.py
--rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/install.py
--rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/component.py
--rw-r--r--   0        0        0     2110 2024-05-20 03:55:46.008842 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/context.py
--rw-r--r--   0        0        0     1187 2024-05-20 03:17:42.705230 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/inject.py
--rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/queue.py
--rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/run.py
--rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/serialize.py
--rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/tool.py
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1231 2024-05-20 05:58:47.560312 reasonify_headless-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/__init__.py
+-rw-r--r--   0        0        0     2392 2024-05-20 04:51:28.420660 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/core/loop.py
+-rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/async.yaml
+-rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/date.yaml
+-rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/dir.yaml
+-rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/search.yaml
+-rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/simple_ask.yaml
+-rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/models/shot.py
+-rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/chat.j2
+-rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/main.j2
+-rw-r--r--   0        0        0      235 2024-05-20 04:51:32.391086 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/__init__.py
+-rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/fetch.py
+-rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/input.py
+-rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/install.py
+-rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/component.py
+-rw-r--r--   0        0        0     1976 2024-05-20 05:44:37.361696 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/context.py
+-rw-r--r--   0        0        0     1187 2024-05-20 03:17:42.705230 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/inject.py
+-rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/queue.py
+-rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/run.py
+-rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/serialize.py
+-rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/tool.py
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a6/PKG-INFO
```

### Comparing `reasonify_headless-0.1.0a5/pyproject.toml` & `reasonify_headless-0.1.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "pyodide-py~=0.26.0a4 ; sys_platform != 'emscripten'",
     "promplate~=0.3.4.7",
     "python-box~=7.1.1",
     "promptools[validation]~=0.1.3.4",
     "promplate-recipes~=0.2.2.1",
     "pyyaml~=6.0.1",
 ]
-version = "0.1.0a5"
+version = "0.1.0a6"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/core/loop.py` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/core/loop.py`

 * *Files identical despite different names*

```diff
@@ -72,15 +72,15 @@
 
 @main.end_process
 @dispatch_context
 async def _(c: Context, queue: QueueWrapper, future: Future, messages: list[Message], response: list, sources: list, results: list):
     queue.end()
     await future
 
-    del c["future"], c["queue"]
+    del c["future"], c["queue"], c["pure_text"]
 
     if sources:
         messages.append(assistant > json(sources))
         messages.append(system @ "results" > json(results))
 
     if not response:
         return  # next round
```

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/async.yaml` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/async.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/search.yaml` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/examples/search.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/models/shot.py` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/models/shot.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/__init__.py` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/main.j2` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/templates/main.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/fetch.py` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/tools/fetch.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/context.py` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from contextlib import suppress
 from functools import partial
 from typing import TYPE_CHECKING
 
 from partial_json_parser import ALL
 from promplate import ChainContext
 from promptools.extractors.json import extract_json
 
@@ -14,22 +13,24 @@
         super().__init__(context)
 
     @property
     def snapshots(self) -> list[dict]:
         return self["snapshots"]
 
     def __setitem__(self, key, value):
-        with suppress(IndexError):
+        try:
             self.snapshots[0][key] = value
-        super().__setitem__(key, value)
+        except IndexError:
+            super().__setitem__(key, value)
 
     def __delitem__(self, key: str):
-        with suppress(KeyError):
+        try:
             del self.snapshots[0][key]
-        super().__delitem__(key)
+        except KeyError:
+            super().__delitem__(key)
 
     def __getitem__(self, key: str):
         if key != "snapshots":
             for snapshot in self.snapshots:
                 if key in snapshot:
                     return snapshot[key]
         return super().__getitem__(key)
@@ -54,13 +55,8 @@
                 return extract_json(self.result, fallback, expect, allow_partial)
             except NameError:  # pydantic v1
                 # NameError: Field name "schema" shadows a BaseModel attribute; use a different field name with "alias='schema'".
                 return extract_json(self.result, fallback, allow_partial=allow_partial)
 
 
 def new_checkpoint(context):
-    c = Context.ensure(context)
-    with suppress(KeyError):
-        # log the raw result to the snapshot
-        c["result"] = c.result
-
-    c.snapshots.insert(0, {})
+    Context.ensure(context).snapshots.insert(0, {})
```

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/inject.py` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/inject.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/run.py` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/run.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/tool.py` & `reasonify_headless-0.1.0a6/reasonify-headless/reasonify/utils/tool.py`

 * *Files identical despite different names*


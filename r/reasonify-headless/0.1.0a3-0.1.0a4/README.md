# Comparing `tmp/reasonify_headless-0.1.0a3.tar.gz` & `tmp/reasonify_headless-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasonify_headless-0.1.0a3.tar", last modified: Sun May 19 20:21:54 2024, max compression
+gzip compressed data, was "reasonify_headless-0.1.0a4.tar", last modified: Mon May 20 03:26:32 2024, max compression
```

## Comparing `reasonify_headless-0.1.0a3.tar` & `reasonify_headless-0.1.0a4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1231 2024-05-19 20:21:54.813357 reasonify_headless-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/__init__.py
--rw-r--r--   0        0        0     2238 2024-05-19 20:08:43.262838 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/core/loop.py
--rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/__init__.py
--rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/async.yaml
--rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/date.yaml
--rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/dir.yaml
--rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/search.yaml
--rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/simple_ask.yaml
--rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/models/shot.py
--rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/__init__.py
--rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/chat.j2
--rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/main.j2
--rw-r--r--   0        0        0      242 2024-05-19 12:29:46.617624 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/__init__.py
--rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/fetch.py
--rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/input.py
--rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/install.py
--rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/component.py
--rw-r--r--   0        0        0     1923 2024-05-18 13:59:37.528777 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/context.py
--rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/queue.py
--rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/run.py
--rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/serialize.py
--rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/tool.py
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1231 2024-05-20 03:26:32.410879 reasonify_headless-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/__init__.py
+-rw-r--r--   0        0        0     2361 2024-05-20 03:17:07.904420 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/core/loop.py
+-rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/async.yaml
+-rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/date.yaml
+-rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/dir.yaml
+-rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/search.yaml
+-rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/simple_ask.yaml
+-rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/models/shot.py
+-rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/chat.j2
+-rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/main.j2
+-rw-r--r--   0        0        0      242 2024-05-19 12:29:46.617624 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/__init__.py
+-rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/fetch.py
+-rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/input.py
+-rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/install.py
+-rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/component.py
+-rw-r--r--   0        0        0     2112 2024-05-20 03:15:24.415110 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/context.py
+-rw-r--r--   0        0        0     1187 2024-05-20 03:17:42.705230 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/inject.py
+-rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/queue.py
+-rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/run.py
+-rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/serialize.py
+-rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/tool.py
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a4/PKG-INFO
```

### Comparing `reasonify_headless-0.1.0a3/pyproject.toml` & `reasonify_headless-0.1.0a4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 dynamic = []
 requires-python = ">=3.12"
 authors = [
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = [
     "pyodide-py~=0.26.0a4 ; sys_platform != 'emscripten'",
-    "promplate~=0.3.4.5",
+    "promplate~=0.3.4.7",
     "python-box~=7.1.1",
     "promptools[validation]~=0.1.3.4",
     "promplate-recipes~=0.2.2.1",
     "pyyaml~=6.0.1",
 ]
-version = "0.1.0a3"
+version = "0.1.0a4"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/core/loop.py` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/core/loop.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,90 @@
-from asyncio import ensure_future
+from asyncio import Future, ensure_future
 from operator import call
 
 from partial_json_parser import Allow
 from promplate import Chain, Jump, Loop, Message, Node
 from promplate.prompt.chat import assistant, system
 from promplate_recipes.functional.node import SimpleNode
 
 from ..examples import get_examples
 from ..templates import main
 from ..utils.context import Context, new_checkpoint
+from ..utils.inject import dispatch_context
 from ..utils.queue import QueueWrapper
 from ..utils.run import get_context, run
 from ..utils.serialize import json
 from ..utils.tool import tool
 
 
 @SimpleNode
-async def intro(context):
-    context["few_shot"] = await get_examples()
-
-    new_checkpoint(context)
-    c = Context(context)
-
-    c.setdefault("response", [])
+@dispatch_context
+async def intro(c: Context):
+    response = c["response"] = []
 
     @tool
     def reply(message: str):
         """talk to the user"""
-        c["response"] += [message]
+        response.append(message)
 
     get_context()["reply"] = reply
 
 
+@intro.pre_process
+async def _(context: dict):
+    context["few_shot"] = await get_examples()
+    new_checkpoint(context)
+
+
 main_loop = Chain(intro, Loop(main := Node(main)))
 
 
 @main.pre_process
-def _(context):
-    c = Context(context)
-    c["queue"] = queue = QueueWrapper[str]()
-    c["index"] = 0
-    c["results"] = []
+@dispatch_context
+def _():
+    queue = QueueWrapper[str]()
+    results = list[dict]()
 
     @ensure_future
     @call
     async def job():
         async for source in queue:
-            result = await run(source)
-            c["results"] += [result]
+            results.append(await run(source))
 
-    c["future"] = job
+    return {"future": job, "index": 0, "queue": queue, "results": results}
 
 
 @main.mid_process
-def _(context):
-    c = Context(context)
+@dispatch_context
+def _(c: Context, index: int, queue: QueueWrapper[str], response: list[str], pure_text=False):
     c["sources"] = c.extract_json([])
 
-    if c.get("pure_text", False):
-        c["response"][-1] = c.result
+    if pure_text:
+        response[-1] = c.result
         return
 
-    queue: QueueWrapper[str] = c["queue"]
-
-    sources = c.extract_json(False, list[str], ~Allow.STR)
-    if sources is False:
-        c["response"] += [c.result]
-        c["pure_text"] = True
+    sources = c.extract_json(None, list[str], ~Allow.STR)
+    if sources is None:
+        response.append(c.result)
+        return {"pure_text": True}
 
-    for source in c.extract_json([], list[str], ~Allow.STR)[c["index"] :]:
+    for source in sources[index:]:
         queue.put(source)
         c["index"] += 1
 
 
 @main.end_process
-async def _(context):
-    c = Context(context)
-    c["queue"].end()
-    await c["future"]
-
-    messages: list[Message] = c["messages"]
-
-    if "sources" in c:
-        messages.append(assistant > json(c["sources"]))
-        messages.append(system @ "results" > json(c["results"]))
+@dispatch_context
+async def _(c: Context, queue: QueueWrapper, future: Future, messages: list[Message], response: list, sources: list, results: list):
+    queue.end()
+    await future
 
     del c["future"], c["queue"]
 
-    if c["response"] or not c["sources"]:
-        raise Jump(out_of=main_loop)
+    if sources:
+        messages.append(assistant > json(sources))
+        messages.append(system @ "results" > json(results))
+
+    if not response:
+        return  # next round
+
+    raise Jump(out_of=main_loop)  # already responded or nothing generated
```

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/async.yaml` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/async.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/search.yaml` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/search.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/models/shot.py` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/models/shot.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/__init__.py` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/main.j2` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/main.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/fetch.py` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/fetch.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/context.py` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from contextlib import suppress
 from functools import partial
-from typing import TYPE_CHECKING, TypeVar
+from typing import TYPE_CHECKING
 
 from partial_json_parser import ALL
 from promplate import ChainContext
 from promptools.extractors.json import extract_json
 
-T = TypeVar("T")
-
 
 class Context(ChainContext):
     def __init__(self, context: ChainContext):
         if not isinstance(context.get("snapshots"), list):
             context["snapshots"] = []
         super().__init__(context)
 
@@ -32,14 +30,21 @@
     def __getitem__(self, key: str):
         if key != "snapshots":
             for snapshot in self.snapshots:
                 if key in snapshot:
                     return snapshot[key]
         return super().__getitem__(key)
 
+    def __contains__(self, key):
+        if key != "snapshots":
+            for snapshot in self.snapshots:
+                if key in snapshot:
+                    return True
+        return super().__contains__(key)
+
     if TYPE_CHECKING:
 
         @property
         def extract_json(self):
             return partial(extract_json, self.result)
 
     else:
@@ -48,14 +53,14 @@
             try:
                 return extract_json(self.result, fallback, expect, allow_partial)
             except NameError:  # pydantic v1
                 # NameError: Field name "schema" shadows a BaseModel attribute; use a different field name with "alias='schema'".
                 return extract_json(self.result, fallback, allow_partial=allow_partial)
 
 
-def new_checkpoint(context: ChainContext):
-    c = Context(context)
+def new_checkpoint(context):
+    c = Context.ensure(context)
     with suppress(KeyError):
         # log the raw result to the snapshot
         c["result"] = c.result
 
     c.snapshots.insert(0, {})
```

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/run.py` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/run.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/tool.py` & `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/tool.py`

 * *Files identical despite different names*


# Comparing `tmp/reasonify_headless-0.1.0a4.tar.gz` & `tmp/reasonify_headless-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasonify_headless-0.1.0a4.tar", last modified: Mon May 20 03:26:32 2024, max compression
+gzip compressed data, was "reasonify_headless-0.1.0a5.tar", last modified: Mon May 20 04:02:40 2024, max compression
```

## Comparing `reasonify_headless-0.1.0a4.tar` & `reasonify_headless-0.1.0a5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1231 2024-05-20 03:26:32.410879 reasonify_headless-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/__init__.py
--rw-r--r--   0        0        0     2361 2024-05-20 03:17:07.904420 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/core/loop.py
--rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/__init__.py
--rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/async.yaml
--rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/date.yaml
--rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/dir.yaml
--rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/search.yaml
--rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/simple_ask.yaml
--rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/models/shot.py
--rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/__init__.py
--rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/chat.j2
--rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/main.j2
--rw-r--r--   0        0        0      242 2024-05-19 12:29:46.617624 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/__init__.py
--rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/fetch.py
--rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/input.py
--rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/install.py
--rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/component.py
--rw-r--r--   0        0        0     2112 2024-05-20 03:15:24.415110 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/context.py
--rw-r--r--   0        0        0     1187 2024-05-20 03:17:42.705230 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/inject.py
--rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/queue.py
--rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/run.py
--rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/serialize.py
--rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/tool.py
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1231 2024-05-20 04:02:40.244475 reasonify_headless-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/__init__.py
+-rw-r--r--   0        0        0     2376 2024-05-20 03:58:36.431514 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/core/loop.py
+-rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/async.yaml
+-rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/date.yaml
+-rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/dir.yaml
+-rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/search.yaml
+-rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/simple_ask.yaml
+-rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/models/shot.py
+-rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/chat.j2
+-rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/main.j2
+-rw-r--r--   0        0        0      242 2024-05-19 12:29:46.617624 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/__init__.py
+-rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/fetch.py
+-rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/input.py
+-rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/install.py
+-rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/component.py
+-rw-r--r--   0        0        0     2110 2024-05-20 03:55:46.008842 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/context.py
+-rw-r--r--   0        0        0     1187 2024-05-20 03:17:42.705230 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/inject.py
+-rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/queue.py
+-rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/run.py
+-rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/serialize.py
+-rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/tool.py
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a5/PKG-INFO
```

### Comparing `reasonify_headless-0.1.0a4/pyproject.toml` & `reasonify_headless-0.1.0a5/pyproject.toml`

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
-version = "0.1.0a4"
+version = "0.1.0a5"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/core/loop.py` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/core/loop.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from promplate import Chain, Jump, Loop, Message, Node
 from promplate.prompt.chat import assistant, system
 from promplate_recipes.functional.node import SimpleNode
 
 from ..examples import get_examples
 from ..templates import main
 from ..utils.context import Context, new_checkpoint
-from ..utils.inject import dispatch_context
+from ..utils.inject import dispatch_context, inject
 from ..utils.queue import QueueWrapper
 from ..utils.run import get_context, run
 from ..utils.serialize import json
 from ..utils.tool import tool
 
 
 @SimpleNode
@@ -36,40 +36,38 @@
 
 
 main_loop = Chain(intro, Loop(main := Node(main)))
 
 
 @main.pre_process
 @dispatch_context
-def _():
-    queue = QueueWrapper[str]()
-    results = list[dict]()
+def _(c: Context, queue=inject(lambda: QueueWrapper[str]()), results=inject(lambda: list[dict]())):
 
     @ensure_future
     @call
     async def job():
         async for source in queue:
             results.append(await run(source))
 
-    return {"future": job, "index": 0, "queue": queue, "results": results}
+    c.update({"future": job, "index": 0})
 
 
 @main.mid_process
 @dispatch_context
 def _(c: Context, index: int, queue: QueueWrapper[str], response: list[str], pure_text=False):
     c["sources"] = c.extract_json([])
 
     if pure_text:
         response[-1] = c.result
         return
 
     sources = c.extract_json(None, list[str], ~Allow.STR)
     if sources is None:
         response.append(c.result)
-        return {"pure_text": True}
+        return c.update({"pure_text": True})
 
     for source in sources[index:]:
         queue.put(source)
         c["index"] += 1
 
 
 @main.end_process
```

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/async.yaml` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/async.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/examples/search.yaml` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/examples/search.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/models/shot.py` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/models/shot.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/__init__.py` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/templates/main.j2` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/templates/main.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/tools/fetch.py` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/tools/fetch.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/context.py` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __setitem__(self, key, value):
         with suppress(IndexError):
             self.snapshots[0][key] = value
         super().__setitem__(key, value)
 
     def __delitem__(self, key: str):
-        with suppress(IndexError):
+        with suppress(KeyError):
             del self.snapshots[0][key]
         super().__delitem__(key)
 
     def __getitem__(self, key: str):
         if key != "snapshots":
             for snapshot in self.snapshots:
                 if key in snapshot:
```

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/inject.py` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/inject.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/run.py` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/run.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a4/reasonify-headless/reasonify/utils/tool.py` & `reasonify_headless-0.1.0a5/reasonify-headless/reasonify/utils/tool.py`

 * *Files identical despite different names*


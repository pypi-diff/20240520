# Comparing `tmp/reasonify_headless-0.1.0a2.tar.gz` & `tmp/reasonify_headless-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasonify_headless-0.1.0a2.tar", last modified: Sun May 19 13:47:54 2024, max compression
+gzip compressed data, was "reasonify_headless-0.1.0a3.tar", last modified: Sun May 19 20:21:54 2024, max compression
```

## Comparing `reasonify_headless-0.1.0a2.tar` & `reasonify_headless-0.1.0a3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1231 2024-05-19 13:47:54.020065 reasonify_headless-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/__init__.py
--rw-r--r--   0        0        0     1971 2024-05-18 15:03:23.548088 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/core/loop.py
--rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/__init__.py
--rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/async.yaml
--rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/date.yaml
--rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/dir.yaml
--rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/simple_ask.yaml
--rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/models/shot.py
--rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/__init__.py
--rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/chat.j2
--rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/main.j2
--rw-r--r--   0        0        0      242 2024-05-19 12:29:46.617624 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/tools/__init__.py
--rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/tools/input.py
--rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/tools/install.py
--rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/component.py
--rw-r--r--   0        0        0     1923 2024-05-18 13:59:37.528777 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/context.py
--rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/queue.py
--rw-r--r--   0        0        0     1812 2024-05-18 15:20:17.969376 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/run.py
--rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/serialize.py
--rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/tool.py
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1231 2024-05-19 20:21:54.813357 reasonify_headless-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/__init__.py
+-rw-r--r--   0        0        0     2238 2024-05-19 20:08:43.262838 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/core/loop.py
+-rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/async.yaml
+-rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/date.yaml
+-rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/dir.yaml
+-rw-r--r--   0        0        0      616 2024-05-19 20:10:02.086670 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/search.yaml
+-rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/simple_ask.yaml
+-rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/models/shot.py
+-rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/chat.j2
+-rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/main.j2
+-rw-r--r--   0        0        0      242 2024-05-19 12:29:46.617624 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/__init__.py
+-rw-r--r--   0        0        0     1403 2024-05-19 17:32:52.012174 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/fetch.py
+-rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/input.py
+-rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/tools/install.py
+-rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/component.py
+-rw-r--r--   0        0        0     1923 2024-05-18 13:59:37.528777 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/context.py
+-rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/queue.py
+-rw-r--r--   0        0        0     1809 2024-05-19 15:19:31.747906 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/run.py
+-rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/serialize.py
+-rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/tool.py
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a3/PKG-INFO
```

### Comparing `reasonify_headless-0.1.0a2/pyproject.toml` & `reasonify_headless-0.1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "pyodide-py~=0.26.0a4 ; sys_platform != 'emscripten'",
     "promplate~=0.3.4.5",
     "python-box~=7.1.1",
     "promptools[validation]~=0.1.3.4",
     "promplate-recipes~=0.2.2.1",
     "pyyaml~=6.0.1",
 ]
-version = "0.1.0a2"
+version = "0.1.0a3"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/core/loop.py` & `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/core/loop.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,33 +12,35 @@
 from ..utils.queue import QueueWrapper
 from ..utils.run import get_context, run
 from ..utils.serialize import json
 from ..utils.tool import tool
 
 
 @SimpleNode
-async def intro(context: dict):
+async def intro(context):
     context["few_shot"] = await get_examples()
-    context["response"] = []
+
+    new_checkpoint(context)
+    c = Context(context)
+
+    c.setdefault("response", [])
 
     @tool
     def reply(message: str):
         """talk to the user"""
-        context["response"] += [message]
+        c["response"] += [message]
 
     get_context()["reply"] = reply
 
 
 main_loop = Chain(intro, Loop(main := Node(main)))
 
 
 @main.pre_process
 def _(context):
-    new_checkpoint(context)
-
     c = Context(context)
     c["queue"] = queue = QueueWrapper[str]()
     c["index"] = 0
     c["results"] = []
 
     @ensure_future
     @call
@@ -51,16 +53,25 @@
 
 
 @main.mid_process
 def _(context):
     c = Context(context)
     c["sources"] = c.extract_json([])
 
+    if c.get("pure_text", False):
+        c["response"][-1] = c.result
+        return
+
     queue: QueueWrapper[str] = c["queue"]
 
+    sources = c.extract_json(False, list[str], ~Allow.STR)
+    if sources is False:
+        c["response"] += [c.result]
+        c["pure_text"] = True
+
     for source in c.extract_json([], list[str], ~Allow.STR)[c["index"] :]:
         queue.put(source)
         c["index"] += 1
 
 
 @main.end_process
 async def _(context):
@@ -70,11 +81,11 @@
 
     messages: list[Message] = c["messages"]
 
     if "sources" in c:
         messages.append(assistant > json(c["sources"]))
         messages.append(system @ "results" > json(c["results"]))
 
+    del c["future"], c["queue"]
+
     if c["response"] or not c["sources"]:
         raise Jump(out_of=main_loop)
-
-    del c["future"], c["queue"]
```

### Comparing `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/async.yaml` & `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/examples/async.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/models/shot.py` & `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/models/shot.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/__init__.py` & `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/main.j2` & `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/templates/main.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/context.py` & `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/context.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/run.py` & `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     if result is not None:
         try:
             if result not in diff.values():
                 out["return"] = result
         except ValueError as e:
             print(format_exception_only(e))
-            if all(isinstance(e, t) for t in (ValueError, TypeError)):
+            if all(is_different(result, v) for v in diff.values()):
                 out["return"] = str(result)
 
     return loads(json(out))  # ensure serializable
 
 
 def register[T: Callable](function: T) -> T:
     get_context()[function.__name__] = function
```

### Comparing `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/tool.py` & `reasonify_headless-0.1.0a3/reasonify-headless/reasonify/utils/tool.py`

 * *Files identical despite different names*


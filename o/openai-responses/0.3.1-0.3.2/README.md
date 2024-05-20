# Comparing `tmp/openai_responses-0.3.1.tar.gz` & `tmp/openai_responses-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.3.1.tar", max compression
+gzip compressed data, was "openai_responses-0.3.2.tar", max compression
```

## Comparing `openai_responses-0.3.1.tar` & `openai_responses-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.3.1/LICENSE
--rw-r--r--   0        0        0     3016 2024-05-14 18:14:24.699878 openai_responses-0.3.1/README.md
--rw-r--r--   0        0        0     1234 2024-05-16 18:37:32.685674 openai_responses-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      310 2024-05-03 15:30:48.556901 openai_responses-0.3.1/src/openai_responses/__init__.py
--rw-r--r--   0        0        0      606 2024-05-10 15:24:55.095526 openai_responses-0.3.1/src/openai_responses/_api.py
--rw-r--r--   0        0        0     1845 2024-05-14 15:18:04.142883 openai_responses-0.3.1/src/openai_responses/_mock.py
--rw-r--r--   0        0        0     3864 2024-05-13 15:32:42.633551 openai_responses-0.3.1/src/openai_responses/_routes/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-14 17:51:42.173434 openai_responses-0.3.1/src/openai_responses/_routes/_base.py
--rw-r--r--   0        0        0     6208 2024-05-16 18:36:55.630698 openai_responses-0.3.1/src/openai_responses/_routes/assistants.py
--rw-r--r--   0        0        0     1123 2024-05-16 18:36:55.631029 openai_responses-0.3.1/src/openai_responses/_routes/chat.py
--rw-r--r--   0        0        0     1385 2024-05-16 18:36:55.631618 openai_responses-0.3.1/src/openai_responses/_routes/embeddings.py
--rw-r--r--   0        0        0     4978 2024-05-03 18:04:28.339502 openai_responses-0.3.1/src/openai_responses/_routes/files.py
--rw-r--r--   0        0        0     8041 2024-05-16 18:36:55.631992 openai_responses-0.3.1/src/openai_responses/_routes/messages.py
--rw-r--r--   0        0        0     3767 2024-05-13 15:31:22.122002 openai_responses-0.3.1/src/openai_responses/_routes/run_steps.py
--rw-r--r--   0        0        0    11511 2024-05-16 18:36:55.632301 openai_responses-0.3.1/src/openai_responses/_routes/runs.py
--rw-r--r--   0        0        0     5291 2024-05-16 18:36:55.632549 openai_responses-0.3.1/src/openai_responses/_routes/threads.py
--rw-r--r--   0        0        0       62 2024-05-02 16:25:57.355893 openai_responses-0.3.1/src/openai_responses/_stores/__init__.py
--rw-r--r--   0        0        0     6151 2024-05-16 18:37:01.157176 openai_responses-0.3.1/src/openai_responses/_stores/state_store.py
--rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.3.1/src/openai_responses/_types/generics.py
--rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.3.1/src/openai_responses/_types/partials/assistants.py
--rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.3.1/src/openai_responses/_types/partials/chat.py
--rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.3.1/src/openai_responses/_types/partials/embeddings.py
--rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.3.1/src/openai_responses/_types/partials/files.py
--rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.3.1/src/openai_responses/_types/partials/messages.py
--rw-r--r--   0        0        0     2945 2024-05-13 15:43:24.432019 openai_responses-0.3.1/src/openai_responses/_types/partials/run_steps.py
--rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.3.1/src/openai_responses/_types/partials/runs.py
--rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.3.1/src/openai_responses/_types/partials/threads.py
--rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.3.1/src/openai_responses/_utils/copy.py
--rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.3.1/src/openai_responses/_utils/faker.py
--rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.3.1/src/openai_responses/_utils/serde.py
--rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.3.1/src/openai_responses/_utils/time.py
--rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.3.1/src/openai_responses/helpers/builders/_base.py
--rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.3.1/src/openai_responses/helpers/builders/assistants.py
--rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.3.1/src/openai_responses/helpers/builders/chat.py
--rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.3.1/src/openai_responses/helpers/builders/embeddings.py
--rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.3.1/src/openai_responses/helpers/builders/messages.py
--rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.3.1/src/openai_responses/helpers/builders/run_steps.py
--rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.3.1/src/openai_responses/helpers/builders/runs.py
--rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.3.1/src/openai_responses/helpers/builders/threads.py
--rw-r--r--   0        0        0     1271 2024-05-16 18:04:24.511337 openai_responses-0.3.1/src/openai_responses/helpers/state_store.py
--rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.3.1/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.3.1/src/openai_responses/py.typed
--rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 openai_responses-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3016 2024-05-14 18:14:24.699878 openai_responses-0.3.2/README.md
+-rw-r--r--   0        0        0     1234 2024-05-20 16:24:51.334193 openai_responses-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-03 15:30:48.556901 openai_responses-0.3.2/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-10 15:24:55.095526 openai_responses-0.3.2/src/openai_responses/_api.py
+-rw-r--r--   0        0        0     1922 2024-05-20 16:30:34.412727 openai_responses-0.3.2/src/openai_responses/_mock.py
+-rw-r--r--   0        0        0     3864 2024-05-13 15:32:42.633551 openai_responses-0.3.2/src/openai_responses/_routes/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-14 17:51:42.173434 openai_responses-0.3.2/src/openai_responses/_routes/_base.py
+-rw-r--r--   0        0        0     6208 2024-05-16 18:36:55.630698 openai_responses-0.3.2/src/openai_responses/_routes/assistants.py
+-rw-r--r--   0        0        0     1123 2024-05-16 18:36:55.631029 openai_responses-0.3.2/src/openai_responses/_routes/chat.py
+-rw-r--r--   0        0        0     1385 2024-05-16 18:36:55.631618 openai_responses-0.3.2/src/openai_responses/_routes/embeddings.py
+-rw-r--r--   0        0        0     4978 2024-05-03 18:04:28.339502 openai_responses-0.3.2/src/openai_responses/_routes/files.py
+-rw-r--r--   0        0        0     8041 2024-05-16 18:36:55.631992 openai_responses-0.3.2/src/openai_responses/_routes/messages.py
+-rw-r--r--   0        0        0     3767 2024-05-13 15:31:22.122002 openai_responses-0.3.2/src/openai_responses/_routes/run_steps.py
+-rw-r--r--   0        0        0    11511 2024-05-16 18:36:55.632301 openai_responses-0.3.2/src/openai_responses/_routes/runs.py
+-rw-r--r--   0        0        0     5291 2024-05-16 18:36:55.632549 openai_responses-0.3.2/src/openai_responses/_routes/threads.py
+-rw-r--r--   0        0        0       62 2024-05-02 16:25:57.355893 openai_responses-0.3.2/src/openai_responses/_stores/__init__.py
+-rw-r--r--   0        0        0     6151 2024-05-16 18:37:01.157176 openai_responses-0.3.2/src/openai_responses/_stores/state_store.py
+-rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.3.2/src/openai_responses/_types/generics.py
+-rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.3.2/src/openai_responses/_types/partials/assistants.py
+-rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.3.2/src/openai_responses/_types/partials/chat.py
+-rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.3.2/src/openai_responses/_types/partials/embeddings.py
+-rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.3.2/src/openai_responses/_types/partials/files.py
+-rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.3.2/src/openai_responses/_types/partials/messages.py
+-rw-r--r--   0        0        0     2945 2024-05-13 15:43:24.432019 openai_responses-0.3.2/src/openai_responses/_types/partials/run_steps.py
+-rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.3.2/src/openai_responses/_types/partials/runs.py
+-rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.3.2/src/openai_responses/_types/partials/threads.py
+-rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.3.2/src/openai_responses/_utils/copy.py
+-rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.3.2/src/openai_responses/_utils/faker.py
+-rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.3.2/src/openai_responses/_utils/serde.py
+-rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.3.2/src/openai_responses/_utils/time.py
+-rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.3.2/src/openai_responses/helpers/builders/_base.py
+-rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.3.2/src/openai_responses/helpers/builders/assistants.py
+-rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.3.2/src/openai_responses/helpers/builders/chat.py
+-rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.3.2/src/openai_responses/helpers/builders/embeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.3.2/src/openai_responses/helpers/builders/messages.py
+-rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.3.2/src/openai_responses/helpers/builders/run_steps.py
+-rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.3.2/src/openai_responses/helpers/builders/runs.py
+-rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.3.2/src/openai_responses/helpers/builders/threads.py
+-rw-r--r--   0        0        0      317 2024-05-20 16:30:34.412882 openai_responses-0.3.2/src/openai_responses/helpers/mergers/_base.py
+-rw-r--r--   0        0        0      290 2024-05-20 16:30:34.413017 openai_responses-0.3.2/src/openai_responses/helpers/mergers/runs.py
+-rw-r--r--   0        0        0     1271 2024-05-16 18:04:24.511337 openai_responses-0.3.2/src/openai_responses/helpers/state_store.py
+-rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.3.2/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.3.2/src/openai_responses/py.typed
+-rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 openai_responses-0.3.2/PKG-INFO
```

### Comparing `openai_responses-0.3.1/LICENSE` & `openai_responses-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/README.md` & `openai_responses-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/pyproject.toml` & `openai_responses-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.3.1"
+version = "0.3.2"
 description = "Automatically mock OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
 homepage = "https://mharrisb1.github.io/openai-responses-python/"
 documentation = "https://mharrisb1.github.io/openai-responses-python/"
```

### Comparing `openai_responses-0.3.1/src/openai_responses/_api.py` & `openai_responses-0.3.2/src/openai_responses/_api.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_mock.py` & `openai_responses-0.3.2/src/openai_responses/_mock.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,32 +24,35 @@
         self.chat = ChatRoutes(self._router)
         self.embeddings = EmbeddingsRoutes(self._router)
         self.files = FileRoutes(self._router, self._state)
 
         # NOTE: need to sort routes to avoid match conflicts
         self._router.routes._routes.sort(key=lambda r: len(repr(r._pattern)), reverse=True)  # type: ignore
 
+    @property
+    def router(self) -> respx.MockRouter:
+        """[RESPX](https://lundberg.github.io/respx) router with patched OpenAI routes"""
+        return self._router
+
     def _start_mock(self):
         def wrapper(fn: Callable[..., Any]):
             is_async = inspect.iscoroutinefunction(fn)
             argspec = inspect.getfullargspec(fn)
             needs_ref = "openai_mock" in argspec.args
 
             @wraps(fn)
             async def async_wrapper(*args: Any, **kwargs: Any):
                 if needs_ref:
                     kwargs["openai_mock"] = self
-                assert self._router is not None
-                with self._router:
+                with self.router:
                     return await fn(*args, **kwargs)
 
             @wraps(fn)
             def sync_wrapper(*args: Any, **kwargs: Any):
                 if needs_ref:
                     kwargs["openai_mock"] = self
-                assert self._router is not None
-                with self._router:
+                with self.router:
                     return fn(*args, **kwargs)
 
             return async_wrapper if is_async else sync_wrapper
 
         return wrapper
```

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/__init__.py` & `openai_responses-0.3.2/src/openai_responses/_routes/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/_base.py` & `openai_responses-0.3.2/src/openai_responses/_routes/_base.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/assistants.py` & `openai_responses-0.3.2/src/openai_responses/_routes/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/chat.py` & `openai_responses-0.3.2/src/openai_responses/_routes/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/embeddings.py` & `openai_responses-0.3.2/src/openai_responses/_routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/files.py` & `openai_responses-0.3.2/src/openai_responses/_routes/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/messages.py` & `openai_responses-0.3.2/src/openai_responses/_routes/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/run_steps.py` & `openai_responses-0.3.2/src/openai_responses/_routes/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/runs.py` & `openai_responses-0.3.2/src/openai_responses/_routes/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_routes/threads.py` & `openai_responses-0.3.2/src/openai_responses/_routes/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_stores/state_store.py` & `openai_responses-0.3.2/src/openai_responses/_stores/state_store.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_types/partials/assistants.py` & `openai_responses-0.3.2/src/openai_responses/_types/partials/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_types/partials/chat.py` & `openai_responses-0.3.2/src/openai_responses/_types/partials/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_types/partials/embeddings.py` & `openai_responses-0.3.2/src/openai_responses/_types/partials/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_types/partials/files.py` & `openai_responses-0.3.2/src/openai_responses/_types/partials/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_types/partials/messages.py` & `openai_responses-0.3.2/src/openai_responses/_types/partials/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_types/partials/run_steps.py` & `openai_responses-0.3.2/src/openai_responses/_types/partials/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_types/partials/runs.py` & `openai_responses-0.3.2/src/openai_responses/_types/partials/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_types/partials/threads.py` & `openai_responses-0.3.2/src/openai_responses/_types/partials/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/_utils/serde.py` & `openai_responses-0.3.2/src/openai_responses/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/helpers/builders/chat.py` & `openai_responses-0.3.2/src/openai_responses/helpers/builders/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/helpers/builders/embeddings.py` & `openai_responses-0.3.2/src/openai_responses/helpers/builders/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/helpers/builders/messages.py` & `openai_responses-0.3.2/src/openai_responses/helpers/builders/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/helpers/builders/run_steps.py` & `openai_responses-0.3.2/src/openai_responses/helpers/builders/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/helpers/builders/runs.py` & `openai_responses-0.3.2/src/openai_responses/helpers/builders/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/src/openai_responses/helpers/state_store.py` & `openai_responses-0.3.2/src/openai_responses/helpers/state_store.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.1/PKG-INFO` & `openai_responses-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-responses
-Version: 0.3.1
+Version: 0.3.2
 Summary: Automatically mock OpenAI requests
 Home-page: https://mharrisb1.github.io/openai-responses-python/
 License: MIT
 Author: Michael Harris
 Author-email: mharris@definite.app
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


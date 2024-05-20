# Comparing `tmp/together-1.1.5.tar.gz` & `tmp/together-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together-1.1.5.tar", max compression
+gzip compressed data, was "together-1.2.0.tar", max compression
```

## Comparing `together-1.1.5.tar` & `together-1.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-05-08 02:38:09.291025 together-1.1.5/LICENSE
--rw-r--r--   0        0        0    10365 2024-05-08 02:38:09.291025 together-1.1.5/README.md
--rw-r--r--   0        0        0     2590 2024-05-08 02:38:09.291025 together-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1401 2024-05-08 02:38:09.291025 together-1.1.5/src/together/__init__.py
--rw-r--r--   0        0        0       57 2024-05-08 02:38:09.291025 together-1.1.5/src/together/abstract/__init__.py
--rw-r--r--   0        0        0    25103 2024-05-08 02:38:09.291025 together-1.1.5/src/together/abstract/api_requestor.py
--rw-r--r--   0        0        0        0 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/__init__.py
--rw-r--r--   0        0        0     9170 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/chat.py
--rw-r--r--   0        0        0     4199 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/completions.py
--rw-r--r--   0        0        0     3186 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/files.py
--rw-r--r--   0        0        0     5417 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/finetune.py
--rw-r--r--   0        0        0     2363 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/images.py
--rw-r--r--   0        0        0     1126 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/models.py
--rw-r--r--   0        0        0     1977 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/cli.py
--rw-r--r--   0        0        0     4774 2024-05-08 02:38:09.291025 together-1.1.5/src/together/client.py
--rw-r--r--   0        0        0      908 2024-05-08 02:38:09.291025 together-1.1.5/src/together/constants.py
--rw-r--r--   0        0        0     5329 2024-05-08 02:38:09.295025 together-1.1.5/src/together/error.py
--rw-r--r--   0        0        0    11269 2024-05-08 02:38:09.295025 together-1.1.5/src/together/filemanager.py
--rw-r--r--   0        0        0        0 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/__init__.py
--rw-r--r--   0        0        0      727 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/base.py
--rw-r--r--   0        0        0     2343 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/complete.py
--rw-r--r--   0        0        0      591 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/embeddings.py
--rw-r--r--   0        0        0     3863 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/files.py
--rw-r--r--   0        0        0     4917 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/finetune.py
--rw-r--r--   0        0        0      582 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/images.py
--rw-r--r--   0        0        0     1053 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/models.py
--rw-r--r--   0        0        0      701 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/__init__.py
--rw-r--r--   0        0        0      617 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/chat/__init__.py
--rw-r--r--   0        0        0    14084 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/chat/completions.py
--rw-r--r--   0        0        0    11353 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/completions.py
--rw-r--r--   0        0        0     2546 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/embeddings.py
--rw-r--r--   0        0        0     4593 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/files.py
--rw-r--r--   0        0        0    12416 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/finetune.py
--rw-r--r--   0        0        0     4775 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/images.py
--rw-r--r--   0        0        0     1786 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/models.py
--rw-r--r--   0        0        0     1319 2024-05-08 02:38:09.295025 together-1.1.5/src/together/together_response.py
--rw-r--r--   0        0        0     1432 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/__init__.py
--rw-r--r--   0        0        0      642 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/abstract.py
--rw-r--r--   0        0        0     4335 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/chat_completions.py
--rw-r--r--   0        0        0     1491 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/common.py
--rw-r--r--   0        0        0     2887 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/completions.py
--rw-r--r--   0        0        0      751 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/embeddings.py
--rw-r--r--   0        0        0      370 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/error.py
--rw-r--r--   0        0        0     1954 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/files.py
--rw-r--r--   0        0        0     5775 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/finetune.py
--rw-r--r--   0        0        0      915 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/images.py
--rw-r--r--   0        0        0     1013 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/models.py
--rw-r--r--   0        0        0      662 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/__init__.py
--rw-r--r--   0        0        0     1665 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/_log.py
--rw-r--r--   0        0        0     2407 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/api_helpers.py
--rw-r--r--   0        0        0     7165 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/files.py
--rw-r--r--   0        0        0     1788 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/tools.py
--rw-r--r--   0        0        0      126 2024-05-08 02:38:09.295025 together-1.1.5/src/together/version.py
--rw-r--r--   0        0        0    11812 1970-01-01 00:00:00.000000 together-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-20 16:34:14.079935 together-1.2.0/LICENSE
+-rw-r--r--   0        0        0    10365 2024-05-20 16:34:14.079935 together-1.2.0/README.md
+-rw-r--r--   0        0        0     2590 2024-05-20 16:34:14.083936 together-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-05-20 16:34:14.083936 together-1.2.0/src/together/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-20 16:34:14.083936 together-1.2.0/src/together/abstract/__init__.py
+-rw-r--r--   0        0        0    25103 2024-05-20 16:34:14.083936 together-1.2.0/src/together/abstract/api_requestor.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/api/__init__.py
+-rw-r--r--   0        0        0     9170 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/api/chat.py
+-rw-r--r--   0        0        0     4199 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/api/completions.py
+-rw-r--r--   0        0        0     3329 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/api/files.py
+-rw-r--r--   0        0        0     5417 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/api/finetune.py
+-rw-r--r--   0        0        0     2363 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/api/images.py
+-rw-r--r--   0        0        0     1126 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/api/models.py
+-rw-r--r--   0        0        0     1977 2024-05-20 16:34:14.083936 together-1.2.0/src/together/cli/cli.py
+-rw-r--r--   0        0        0     4774 2024-05-20 16:34:14.083936 together-1.2.0/src/together/client.py
+-rw-r--r--   0        0        0      908 2024-05-20 16:34:14.083936 together-1.2.0/src/together/constants.py
+-rw-r--r--   0        0        0     5402 2024-05-20 16:34:14.083936 together-1.2.0/src/together/error.py
+-rw-r--r--   0        0        0    11269 2024-05-20 16:34:14.083936 together-1.2.0/src/together/filemanager.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:34:14.083936 together-1.2.0/src/together/legacy/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-20 16:34:14.083936 together-1.2.0/src/together/legacy/base.py
+-rw-r--r--   0        0        0     2343 2024-05-20 16:34:14.083936 together-1.2.0/src/together/legacy/complete.py
+-rw-r--r--   0        0        0      591 2024-05-20 16:34:14.083936 together-1.2.0/src/together/legacy/embeddings.py
+-rw-r--r--   0        0        0     3959 2024-05-20 16:34:14.083936 together-1.2.0/src/together/legacy/files.py
+-rw-r--r--   0        0        0     4917 2024-05-20 16:34:14.083936 together-1.2.0/src/together/legacy/finetune.py
+-rw-r--r--   0        0        0      582 2024-05-20 16:34:14.083936 together-1.2.0/src/together/legacy/images.py
+-rw-r--r--   0        0        0     1053 2024-05-20 16:34:14.083936 together-1.2.0/src/together/legacy/models.py
+-rw-r--r--   0        0        0      701 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/chat/__init__.py
+-rw-r--r--   0        0        0    14084 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/chat/completions.py
+-rw-r--r--   0        0        0    11353 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/completions.py
+-rw-r--r--   0        0        0     2546 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/embeddings.py
+-rw-r--r--   0        0        0     4990 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/files.py
+-rw-r--r--   0        0        0    12416 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/finetune.py
+-rw-r--r--   0        0        0     4775 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/images.py
+-rw-r--r--   0        0        0     1786 2024-05-20 16:34:14.083936 together-1.2.0/src/together/resources/models.py
+-rw-r--r--   0        0        0     1319 2024-05-20 16:34:14.083936 together-1.2.0/src/together/together_response.py
+-rw-r--r--   0        0        0     1432 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/abstract.py
+-rw-r--r--   0        0        0     4335 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/chat_completions.py
+-rw-r--r--   0        0        0     1491 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/common.py
+-rw-r--r--   0        0        0     2887 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/completions.py
+-rw-r--r--   0        0        0      751 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/embeddings.py
+-rw-r--r--   0        0        0      370 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/error.py
+-rw-r--r--   0        0        0     1954 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/files.py
+-rw-r--r--   0        0        0     5775 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/finetune.py
+-rw-r--r--   0        0        0      915 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/images.py
+-rw-r--r--   0        0        0     1013 2024-05-20 16:34:14.083936 together-1.2.0/src/together/types/models.py
+-rw-r--r--   0        0        0      662 2024-05-20 16:34:14.083936 together-1.2.0/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1665 2024-05-20 16:34:14.083936 together-1.2.0/src/together/utils/_log.py
+-rw-r--r--   0        0        0     2407 2024-05-20 16:34:14.083936 together-1.2.0/src/together/utils/api_helpers.py
+-rw-r--r--   0        0        0     7165 2024-05-20 16:34:14.083936 together-1.2.0/src/together/utils/files.py
+-rw-r--r--   0        0        0     1788 2024-05-20 16:34:14.083936 together-1.2.0/src/together/utils/tools.py
+-rw-r--r--   0        0        0      126 2024-05-20 16:34:14.083936 together-1.2.0/src/together/version.py
+-rw-r--r--   0        0        0    11812 1970-01-01 00:00:00.000000 together-1.2.0/PKG-INFO
```

### Comparing `together-1.1.5/LICENSE` & `together-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `together-1.1.5/README.md` & `together-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `together-1.1.5/pyproject.toml` & `together-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "oldest-supported-numpy>=0.14; python_version<'3.9'",
     "numpy>=1.25; python_version>='3.9'",
 ]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "together"
-version = "1.1.5"
+version = "1.2.0"
 authors = [
     "Together AI <support@together.ai>"
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `together-1.1.5/src/together/__init__.py` & `together-1.2.0/src/together/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/abstract/api_requestor.py` & `together-1.2.0/src/together/abstract/api_requestor.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/cli/api/chat.py` & `together-1.2.0/src/together/cli/api/chat.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/cli/api/completions.py` & `together-1.2.0/src/together/cli/api/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/cli/api/files.py` & `together-1.2.0/src/together/cli/api/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,25 @@
 )
 @click.option(
     "--purpose",
     type=str,
     default=FilePurpose.FineTune.value,
     help="Purpose of file upload. Acceptable values in enum `together.types.FilePurpose`. Defaults to `fine-tunes`.",
 )
-def upload(ctx: click.Context, file: pathlib.Path, purpose: str) -> None:
+@click.option(
+    "--check/--no-check",
+    default=True,
+    help="Whether to check the file before uploading.",
+)
+def upload(ctx: click.Context, file: pathlib.Path, purpose: str, check: bool) -> None:
     """Upload file"""
 
     client: Together = ctx.obj
 
-    response = client.files.upload(file=file, purpose=purpose)
+    response = client.files.upload(file=file, purpose=purpose, check=check)
 
     click.echo(json.dumps(response.model_dump(), indent=4))
 
 
 @files.command()
 @click.pass_context
 def list(ctx: click.Context) -> None:
```

### Comparing `together-1.1.5/src/together/cli/api/finetune.py` & `together-1.2.0/src/together/cli/api/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/cli/api/images.py` & `together-1.2.0/src/together/cli/api/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/cli/api/models.py` & `together-1.2.0/src/together/cli/api/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/cli/cli.py` & `together-1.2.0/src/together/cli/cli.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/client.py` & `together-1.2.0/src/together/client.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/constants.py` & `together-1.2.0/src/together/constants.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/error.py` & `together-1.2.0/src/together/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,20 @@
         http_status: int | None = None,
     ) -> None:
         _message = (
             json.dumps(message.model_dump())
             if isinstance(message, TogetherErrorResponse)
             else message
         )
-        self._message = f"Error code: {http_status} - {_message}"
+        if http_status is not None:
+            self._message = f"Error code: {http_status} - {_message}"
+        else:
+            self._message = str(_message)
 
-        super(TogetherException, self).__init__(self._message)
+        super().__init__(self._message)
 
         self.http_status = http_status
         self.headers = headers or {}
         self.request_id = request_id
 
     def __repr__(self) -> str:
         repr_message = json.dumps(
```

### Comparing `together-1.1.5/src/together/filemanager.py` & `together-1.2.0/src/together/filemanager.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/legacy/base.py` & `together-1.2.0/src/together/legacy/base.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/legacy/complete.py` & `together-1.2.0/src/together/legacy/complete.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/legacy/embeddings.py` & `together-1.2.0/src/together/legacy/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/legacy/files.py` & `together-1.2.0/src/together/legacy/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,19 @@
             if not report_dict["is_check_passed"]:
                 raise together.error.FileTypeError(
                     f"Invalid file supplied. Failed to upload.\nReport:\n {report_dict}"
                 )
 
         client = together.Together(api_key=api_key)
 
-        response = client.files.upload(file=file).model_dump()
+        # disabling the check, because it was run previously
+        response = client.files.upload(file=file, check=False).model_dump()
 
-        response["report_dict"] = report_dict
+        if check:
+            response["report_dict"] = report_dict
 
         return response
 
     @classmethod
     @deprecated  # type: ignore
     def delete(
         cls,
```

### Comparing `together-1.1.5/src/together/legacy/finetune.py` & `together-1.2.0/src/together/legacy/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/legacy/images.py` & `together-1.2.0/src/together/legacy/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/legacy/models.py` & `together-1.2.0/src/together/legacy/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/resources/__init__.py` & `together-1.2.0/src/together/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/resources/chat/__init__.py` & `together-1.2.0/src/together/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/resources/chat/completions.py` & `together-1.2.0/src/together/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/resources/completions.py` & `together-1.2.0/src/together/resources/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/resources/embeddings.py` & `together-1.2.0/src/together/resources/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/resources/files.py` & `together-1.2.0/src/together/resources/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 from __future__ import annotations
 
 from pathlib import Path
+from pprint import pformat
 
 from together.abstract import api_requestor
+from together.error import FileTypeError
 from together.filemanager import DownloadManager, UploadManager
 from together.together_response import TogetherResponse
 from together.types import (
     FileDeleteResponse,
     FileList,
     FileObject,
     FilePurpose,
     FileResponse,
     TogetherClient,
     TogetherRequest,
 )
-from together.utils import normalize_key
+from together.utils import check_file, normalize_key
 
 
 class Files:
     def __init__(self, client: TogetherClient) -> None:
         self._client = client
 
     def upload(
-        self, file: Path | str, *, purpose: FilePurpose | str = FilePurpose.FineTune
+        self,
+        file: Path | str,
+        *,
+        purpose: FilePurpose | str = FilePurpose.FineTune,
+        check: bool = True,
     ) -> FileResponse:
         upload_manager = UploadManager(self._client)
 
+        if check:
+            report_dict = check_file(file)
+            if not report_dict["is_check_passed"]:
+                raise FileTypeError(
+                    f"Invalid file supplied, failed to upload. Report:\n{pformat(report_dict)}"
+                )
+
         if isinstance(file, str):
             file = Path(file)
 
         if isinstance(purpose, str):
             purpose = FilePurpose(purpose)
 
         assert isinstance(purpose, FilePurpose)
```

### Comparing `together-1.1.5/src/together/resources/finetune.py` & `together-1.2.0/src/together/resources/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/resources/images.py` & `together-1.2.0/src/together/resources/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/resources/models.py` & `together-1.2.0/src/together/resources/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/together_response.py` & `together-1.2.0/src/together/together_response.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/__init__.py` & `together-1.2.0/src/together/types/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/abstract.py` & `together-1.2.0/src/together/types/abstract.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/chat_completions.py` & `together-1.2.0/src/together/types/chat_completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/common.py` & `together-1.2.0/src/together/types/common.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/completions.py` & `together-1.2.0/src/together/types/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/embeddings.py` & `together-1.2.0/src/together/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/files.py` & `together-1.2.0/src/together/types/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/finetune.py` & `together-1.2.0/src/together/types/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/images.py` & `together-1.2.0/src/together/types/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/types/models.py` & `together-1.2.0/src/together/types/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/utils/__init__.py` & `together-1.2.0/src/together/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/utils/_log.py` & `together-1.2.0/src/together/utils/_log.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/utils/api_helpers.py` & `together-1.2.0/src/together/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/utils/files.py` & `together-1.2.0/src/together/utils/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/src/together/utils/tools.py` & `together-1.2.0/src/together/utils/tools.py`

 * *Files identical despite different names*

### Comparing `together-1.1.5/PKG-INFO` & `together-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together
-Version: 1.1.5
+Version: 1.2.0
 Summary: Python client for Together's Cloud Platform!
 Home-page: https://github.com/togethercomputer/together-python
 License: Apache-2.0
 Author: Together AI
 Author-email: support@together.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: together Version: 1.1.5 Summary: Python client for
+Metadata-Version: 2.1 Name: together Version: 1.2.0 Summary: Python client for
 Together's Cloud Platform! Home-page: https://github.com/togethercomputer/
 together-python License: Apache-2.0 Author: Together AI Author-email:
 support@together.ai Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```


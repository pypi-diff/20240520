# Comparing `tmp/uploadthing_py-0.1.1.tar.gz` & `tmp/uploadthing_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadthing_py-0.1.1.tar", max compression
+gzip compressed data, was "uploadthing_py-0.1.2.tar", max compression
```

## Comparing `uploadthing_py-0.1.1.tar` & `uploadthing_py-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-19 15:22:38.340742 uploadthing_py-0.1.1/README.md
--rw-r--r--   0        0        0      555 2024-05-19 21:39:23.893185 uploadthing_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      298 2024-05-19 21:37:22.451857 uploadthing_py-0.1.1/uploadthing_py/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.1.1/uploadthing_py/py.typed
--rw-r--r--   0        0        0     2507 2024-05-19 21:12:18.711453 uploadthing_py-0.1.1/uploadthing_py/types.py
--rw-r--r--   0        0        0     5393 2024-05-19 21:37:39.542526 uploadthing_py-0.1.1/uploadthing_py/utapi.py
--rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.1.1/uploadthing_py/utils.py
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 uploadthing_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      584 2024-05-19 21:49:00.388489 uploadthing_py-0.1.2/README.md
+-rw-r--r--   0        0        0      555 2024-05-19 21:53:39.892909 uploadthing_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      298 2024-05-19 21:37:22.451857 uploadthing_py-0.1.2/uploadthing_py/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.1.2/uploadthing_py/py.typed
+-rw-r--r--   0        0        0     2507 2024-05-19 21:52:42.750217 uploadthing_py-0.1.2/uploadthing_py/types.py
+-rw-r--r--   0        0        0     5536 2024-05-19 21:53:13.103110 uploadthing_py-0.1.2/uploadthing_py/utapi.py
+-rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.1.2/uploadthing_py/utils.py
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 uploadthing_py-0.1.2/PKG-INFO
```

### Comparing `uploadthing_py-0.1.1/pyproject.toml` & `uploadthing_py-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uploadthing.py"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python SDK for UploadThing"
 authors = ["juliusmarminge <julius0216@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "uploadthing_py" }]
 license = "MIT"
```

### Comparing `uploadthing_py-0.1.1/uploadthing_py/types.py` & `uploadthing_py-0.1.2/uploadthing_py/types.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.1.1/uploadthing_py/utapi.py` & `uploadthing_py-0.1.2/uploadthing_py/utapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,19 @@
         )
 
         if response.status_code != 200:
             raise HttpError(response)
 
         return response.json()
 
+    async def upload_files(
+        self, files: MaybeList[t.Any], options: t.Optional[t.Any] = None
+    ):
+        raise NotImplementedError
+
     async def delete_files(
         self,
         keys: MaybeList[str],
         options: t.Optional[DeleteFiles.DeleteFileOptions] = None,
     ):
         if not isinstance(keys, t.List):
             keys = [keys]
```

### Comparing `uploadthing_py-0.1.1/uploadthing_py/utils.py` & `uploadthing_py-0.1.2/uploadthing_py/utils.py`

 * *Files identical despite different names*


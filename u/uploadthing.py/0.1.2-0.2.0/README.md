# Comparing `tmp/uploadthing_py-0.1.2.tar.gz` & `tmp/uploadthing_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadthing_py-0.1.2.tar", max compression
+gzip compressed data, was "uploadthing_py-0.2.0.tar", max compression
```

## Comparing `uploadthing_py-0.1.2.tar` & `uploadthing_py-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      584 2024-05-19 21:49:00.388489 uploadthing_py-0.1.2/README.md
--rw-r--r--   0        0        0      555 2024-05-19 21:53:39.892909 uploadthing_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      298 2024-05-19 21:37:22.451857 uploadthing_py-0.1.2/uploadthing_py/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.1.2/uploadthing_py/py.typed
--rw-r--r--   0        0        0     2507 2024-05-19 21:52:42.750217 uploadthing_py-0.1.2/uploadthing_py/types.py
--rw-r--r--   0        0        0     5536 2024-05-19 21:53:13.103110 uploadthing_py-0.1.2/uploadthing_py/utapi.py
--rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.1.2/uploadthing_py/utils.py
--rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 uploadthing_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2113 2024-05-20 12:34:36.771116 uploadthing_py-0.2.0/README.md
+-rw-r--r--   0        0        0      616 2024-05-20 12:42:58.601953 uploadthing_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      663 2024-05-20 12:38:08.833457 uploadthing_py-0.2.0/uploadthing_py/__init__.py
+-rw-r--r--   0        0        0     1413 2024-05-20 12:20:41.191897 uploadthing_py-0.2.0/uploadthing_py/builder.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.2.0/uploadthing_py/py.typed
+-rw-r--r--   0        0        0     9725 2024-05-20 12:36:13.921275 uploadthing_py-0.2.0/uploadthing_py/request_handler.py
+-rw-r--r--   0        0        0     3367 2024-05-20 12:42:07.140803 uploadthing_py-0.2.0/uploadthing_py/types.py
+-rw-r--r--   0        0        0     5539 2024-05-20 12:37:33.373772 uploadthing_py-0.2.0/uploadthing_py/utapi.py
+-rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.2.0/uploadthing_py/utils.py
+-rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 uploadthing_py-0.2.0/PKG-INFO
```

### Comparing `uploadthing_py-0.1.2/pyproject.toml` & `uploadthing_py-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "uploadthing.py"
-version = "0.1.2"
+version = "0.2.0"
 description = "Python SDK for UploadThing"
 authors = ["juliusmarminge <julius0216@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "uploadthing_py" }]
 license = "MIT"
 
 
 [tool.poetry.dependencies]
 python = "^3.12"
 httpx = "^0.27.0"
-
+pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 pytest-asyncio = "^0.23.7"
+fastapi = "^0.111.0"
+uvicorn = "^0.29.0"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
```

### Comparing `uploadthing_py-0.1.2/uploadthing_py/types.py` & `uploadthing_py-0.2.0/uploadthing_py/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-import typing as t
+from typing import Any, Literal, Union, TypedDict
 from dataclasses import dataclass
+from pydantic import BaseModel
 
+type MaybeList[T] = Union[list[T], T]
 
-type MaybeList[T] = t.Union[t.List[T], T]
+type ACL = Literal["public-read", "private"]
 
-type ACL = t.Literal["public-read", "private"]
+
+#
+# UTApi Types
+#
 
 
 @dataclass
 class File:
     id: str
     custom_id: str
     key: str
     name: str
     status: str
 
     @classmethod
-    def from_api_response(cls, api_response: t.Dict) -> "File":
+    def from_api_response(cls, api_response: dict) -> "File":
         return File(
             id=api_response["id"],
             custom_id=api_response["customId"],
             key=api_response["key"],
             name=api_response["name"],
             status=api_response["status"],
         )
 
 
-class KeyTypeOptions(t.TypedDict):
-    key_type: t.Literal["custom_id", "file_key"]
+class KeyTypeOptions(TypedDict):
+    key_type: Literal["custom_id", "file_key"]
 
 
 class DeleteFiles:
     @dataclass
     class DeleteFileOptions(KeyTypeOptions):
         pass
 
@@ -39,40 +44,40 @@
     class DeleteFileResponse:
         success: bool
 
 
 class ListFiles:
     @dataclass
     class ListFilesOptions:
-        limit: t.Optional[int] = None
-        offset: t.Optional[int] = None
+        limit: int | None = None
+        offset: int | None = None
 
     @dataclass
     class ListFilesResponse:
-        class RawFile(t.TypedDict):
+        class RawFile(TypedDict):
             id: str
             customId: str
             key: str
             name: str
             status: str
 
         hasMore: bool
-        files: t.List[RawFile]
+        files: list[RawFile]
 
 
-class RenameFile:
-    class KeyRename(t.TypedDict):
+class RenameFiles:
+    class KeyRename(TypedDict):
         key: str
         new_name: str
 
-    class CustomIdRename(t.TypedDict):
+    class CustomIdRename(TypedDict):
         custom_id: str
         new_name: str
 
-    type RenameFileOptions = MaybeList[t.Union[KeyRename, CustomIdRename]]
+    type RenameFileOptions = MaybeList[Union[KeyRename, CustomIdRename]]
 
     @dataclass
     class RenameFileResponse:
         success: bool
 
 
 class GetUsageInfo:
@@ -85,32 +90,85 @@
         total_bytes: int
         app_total_bytes: int
         files_uploaded: int
         limit_bytes: int
 
         @classmethod
         def from_api_response(
-            cls, api_response: t.Dict
+            cls, api_response: dict
         ) -> "GetUsageInfo.GetUsageInfoResponse":
             return GetUsageInfo.GetUsageInfoResponse(
                 total_bytes=api_response["totalBytes"],
                 app_total_bytes=api_response["appTotalBytes"],
                 files_uploaded=api_response["filesUploaded"],
                 limit_bytes=api_response["limitBytes"],
             )
 
 
 class GetSignedUrl:
     class GetSignedUrlOptions(KeyTypeOptions):
-        expires_in: t.Optional[int] = None
+        expires_in: int | None = None
 
     class GetSignedUrlResponse:
         url: str
 
 
 class UpdateACL:
     class UpdateACLOptions(KeyTypeOptions):
         acl: ACL
 
     @dataclass
     class UpdateACLResponse:
         success: bool
+
+
+#
+# Handler Types
+#
+
+
+class FileUploadData(BaseModel):
+    name: str
+    size: int
+    type: str
+
+
+class UploadRequest(BaseModel):
+    files: list[FileUploadData]
+
+
+class UploadedFileData(BaseModel):
+    name: str
+    size: int
+    type: str
+    customId: str | None = None
+    key: str
+    url: str
+
+
+class CallbackRequest(BaseModel):
+    metadata: dict[str, Any]
+    status: str
+    file: UploadedFileData
+
+
+class ETag(BaseModel):
+    tag: str
+    partNumber: int
+
+
+class CompleteMPURequest(BaseModel):
+    etags: list[ETag]
+    fileKey: str
+    uploadId: str
+
+
+class FailureRequest(BaseModel):
+    fileKey: str
+    uploadId: str | None = None
+    fileName: str
+    storageProviderError: str | None = None
+
+
+UploadThingRequestBody = Union[
+    UploadRequest, CallbackRequest, CompleteMPURequest, FailureRequest
+]
```

### Comparing `uploadthing_py-0.1.2/uploadthing_py/utapi.py` & `uploadthing_py-0.2.0/uploadthing_py/utapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uploadthing_py
 from uploadthing_py.types import (
     ACL,
     MaybeList,
     File,
     ListFiles,
     DeleteFiles,
-    RenameFile,
+    RenameFiles,
     GetUsageInfo,
     GetSignedUrl,
     UpdateACL,
 )
 from uploadthing_py.utils import json_stringify, del_none
 
 
@@ -95,15 +95,15 @@
         api_response = await self._request_ut_api("/v6/listFiles", options)
         response = ListFiles.ListFilesResponse(**api_response)
 
         files = [File.from_api_response(file) for file in response.files]
 
         return files
 
-    async def rename_files(self, updates: RenameFile.RenameFileOptions):
+    async def rename_files(self, updates: RenameFiles.RenameFileOptions):
         if not isinstance(updates, t.List):
             updates = [updates]
         self._logger.debug(f"Rename files: {updates}")
 
         updates = [
             (
                 {
@@ -118,15 +118,15 @@
             )
             for update in updates
         ]
 
         api_response = await self._request_ut_api(
             "/v6/renameFiles", {"updates": updates}
         )
-        response = RenameFile.RenameFileResponse(**api_response)
+        response = RenameFiles.RenameFileResponse(**api_response)
 
         return response
 
     async def get_usage_info(self):
         api_response = await self._request_ut_api("/v6/getUsageInfo")
         response = GetUsageInfo.GetUsageInfoResponse.from_api_response(api_response)
```

### Comparing `uploadthing_py-0.1.2/uploadthing_py/utils.py` & `uploadthing_py-0.2.0/uploadthing_py/utils.py`

 * *Files identical despite different names*


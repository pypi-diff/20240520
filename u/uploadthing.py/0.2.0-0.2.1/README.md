# Comparing `tmp/uploadthing_py-0.2.0.tar.gz` & `tmp/uploadthing_py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadthing_py-0.2.0.tar", max compression
+gzip compressed data, was "uploadthing_py-0.2.1.tar", max compression
```

## Comparing `uploadthing_py-0.2.0.tar` & `uploadthing_py-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2113 2024-05-20 12:34:36.771116 uploadthing_py-0.2.0/README.md
--rw-r--r--   0        0        0      616 2024-05-20 12:42:58.601953 uploadthing_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      663 2024-05-20 12:38:08.833457 uploadthing_py-0.2.0/uploadthing_py/__init__.py
--rw-r--r--   0        0        0     1413 2024-05-20 12:20:41.191897 uploadthing_py-0.2.0/uploadthing_py/builder.py
--rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.2.0/uploadthing_py/py.typed
--rw-r--r--   0        0        0     9725 2024-05-20 12:36:13.921275 uploadthing_py-0.2.0/uploadthing_py/request_handler.py
--rw-r--r--   0        0        0     3367 2024-05-20 12:42:07.140803 uploadthing_py-0.2.0/uploadthing_py/types.py
--rw-r--r--   0        0        0     5539 2024-05-20 12:37:33.373772 uploadthing_py-0.2.0/uploadthing_py/utapi.py
--rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.2.0/uploadthing_py/utils.py
--rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 uploadthing_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2247 2024-05-20 12:55:39.057094 uploadthing_py-0.2.1/README.md
+-rw-r--r--   0        0        0      616 2024-05-20 12:57:49.517228 uploadthing_py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      663 2024-05-20 12:38:08.833457 uploadthing_py-0.2.1/uploadthing_py/__init__.py
+-rw-r--r--   0        0        0     1413 2024-05-20 12:20:41.191897 uploadthing_py-0.2.1/uploadthing_py/builder.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.2.1/uploadthing_py/py.typed
+-rw-r--r--   0        0        0    11427 2024-05-20 12:57:24.105021 uploadthing_py-0.2.1/uploadthing_py/request_handler.py
+-rw-r--r--   0        0        0     3367 2024-05-20 12:42:07.140803 uploadthing_py-0.2.1/uploadthing_py/types.py
+-rw-r--r--   0        0        0     5539 2024-05-20 12:37:33.373772 uploadthing_py-0.2.1/uploadthing_py/utapi.py
+-rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.2.1/uploadthing_py/utils.py
+-rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 uploadthing_py-0.2.1/PKG-INFO
```

### Comparing `uploadthing_py-0.2.0/README.md` & `uploadthing_py-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from fastapi import FastAPI, Request, Response
 from uploadthing_py import (
     create_uploadthing,
     UploadThingRequestBody,
     create_route_handler,
 )
 from fastapi.middleware.cors import CORSMiddleware
-
+import os
 
 app = FastAPI()
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_methods=["*"],
     allow_headers=["*"],
@@ -69,15 +69,19 @@
             "image/png": {"max_file_size": "4MB"},
             "image/heic": {"max_file_size": "16MB"},
         }
     )
     .middleware(lambda req: {"user_id": req.headers["x-user-id"]})
     .on_upload_complete(lambda file, metadata: print(f"Upload complete for {metadata['user_id']}"))
 }
-handlers = create_route_handler(router=upload_router)
+handlers = create_route_handler(
+    router=upload_router,
+    api_key=os.getenv("UPLOADTHING_SECRET"),
+    is_dev=os.getenv("ENVIRONMENT", "development") == "development",
+)
 
 
 @app.get("/api")
 async def greeting():
     return "Hello from FastAPI"
```

### Comparing `uploadthing_py-0.2.0/pyproject.toml` & `uploadthing_py-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uploadthing.py"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python SDK for UploadThing"
 authors = ["juliusmarminge <julius0216@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "uploadthing_py" }]
 license = "MIT"
```

### Comparing `uploadthing_py-0.2.0/uploadthing_py/__init__.py` & `uploadthing_py-0.2.1/uploadthing_py/__init__.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.0/uploadthing_py/builder.py` & `uploadthing_py-0.2.1/uploadthing_py/builder.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.0/uploadthing_py/request_handler.py` & `uploadthing_py-0.2.1/uploadthing_py/request_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,21 @@
-"""
-Request handler for client-side uploads.
-
-Example usage (FastAPI):
-```py
-from fastapi import FastAPI, Request
-from uploadthing_py import create_route_handler
-
-app = FastAPI()
-
-upload_router = {
-    "image_uploader": {
-        "image": {}
-    }
-}
-
-ut_get, ut_post = create_route_handler(router=upload_router)
-
-@app.post("/uploadthing")
-async def upload(request: Request):
-    return await handleRequest(request)
-```
-"""
-
 from fastapi import Request, Response
 from httpx import AsyncClient
 from uploadthing_py.utils import json_stringify
 from uploadthing_py.builder import UploadThingBuilder
 import asyncio
 import json
 from uploadthing_py.types import (
     UploadRequest,
     CallbackRequest,
     CompleteMPURequest,
     FailureRequest,
 )
 from typing import Union
 
-API_KEY = "sk_live_b77b7544845a29227044105952e9e98c9521a7d9670f54be41a0ee4b4cd8094d"
-
 
 def extract_router_config(router: dict[str, UploadThingBuilder]):
     routes = []
     for slug, config in router.items():
         route_config = {"slug": slug, "config": {}}
 
         for file_type, type_options in config.config.items():
@@ -120,15 +94,20 @@
         )
         print(
             "[DEV_HOOK CALLBACK]", callback_response.status_code, callback_response.text
         )
 
 
 async def handle_upload_request(
-    uploader: UploadThingBuilder, request: Request, body: UploadRequest, slug: str
+    uploader: UploadThingBuilder,
+    request: Request,
+    body: UploadRequest,
+    slug: str,
+    api_key: str,
+    is_dev: bool,
 ):
     # Run middleware to verify permission to upload
     try:
         metadata = uploader.callbacks["middleware"](request)
     except Exception as e:
         print("Middleware error", e)
         return {"error": "Unauthorized"}
@@ -159,33 +138,37 @@
         }
     )
     async with AsyncClient() as client:
         response = await client.post(
             "https://api.uploadthing.com/v7/prepareUpload",
             content=payload,
             headers={
-                "x-uploadthing-api-key": API_KEY,
+                "x-uploadthing-api-key": api_key,
                 "x-uploadthing-be-adapter": "uploadthing.py@",
                 "x-uploadthing-version": "6.10.0",
                 "Content-Type": "application/json",
             },
         )
         print("[PRESIGNEDS]", response.status_code, response.text)
+        if response.status_code != 200:
+            return {"error": "Failed to get presigned URLs"}
+
         presigned_urls = response.json()["data"]
 
-        isDev = True
-        if isDev:
+        if is_dev:
             asyncio.gather(
-                *[dev_hook(presigned["key"], API_KEY) for presigned in presigned_urls]
+                *[dev_hook(presigned["key"], api_key) for presigned in presigned_urls]
             )
 
         return presigned_urls
 
 
-async def handle_callback_request(uploader: UploadThingBuilder, body: CallbackRequest):
+async def handle_callback_request(
+    uploader: UploadThingBuilder, body: CallbackRequest, api_key: str
+):
     # (TODO) Validate payload signature
 
     try:
         server_data = uploader.callbacks["on_upload_complete"](
             file=body.file, metadata=body.metadata
         )
     except Exception as e:
@@ -195,76 +178,150 @@
     payload = json_stringify({"fileKey": body.file.key, "callbackData": server_data})
     async with AsyncClient() as client:
         response = await client.post(
             "https://api.uploadthing.com/v6/serverCallback",
             content=payload,
             headers={
                 "Content-Type": "application/json",
-                "x-uploadthing-api-key": API_KEY,
+                "x-uploadthing-api-key": api_key,
                 "x-uploadthing-version": "6.10.0",
             },
         )
         print("[CALLBACK]", response.status_code, response.text)
 
         return {"success": True}
 
 
-async def handle_complete_mpu_request(body: CompleteMPURequest):
+async def handle_complete_mpu_request(body: CompleteMPURequest, api_key: str):
     async with AsyncClient() as client:
         response = await client.post(
             "https://api.uploadthing.com/v6/completeMultipart",
             content=body.model_dump_json(),
             headers={
                 "Content-Type": "application/json",
-                "x-uploadthing-api-key": API_KEY,
+                "x-uploadthing-api-key": api_key,
                 "x-uploadthing-version": "6.10.0",
             },
         )
         print("[MPU COMPLETE]", response.status_code, response.text)
 
         return {"success": True}
 
 
-async def handle_failure_request(uploader: UploadThingBuilder, body: FailureRequest):
+async def handle_failure_request(
+    uploader: UploadThingBuilder, body: FailureRequest, api_key: str
+):
     payload = json_stringify(
         {
             "fileKey": body.fileKey,
             "uploadId": body.uploadId,
         }
     )
     async with AsyncClient() as client:
         response = await client.post(
             "https://api.uploadthing.com/v6/failureCallback",
             content=payload,
             headers={
                 "Content-Type": "application/json",
-                "x-uploadthing-api-key": API_KEY,
+                "x-uploadthing-api-key": api_key,
                 "x-uploadthing-version": "6.10.0",
             },
         )
         print("[MPU FAILURE]", response.status_code, response.text)
 
     try:
         uploader.callbacks["on_upload_error"](file_key=body.fileKey)
     except Exception as e:
         print("on_upload_error error", e)
         return {"error": "Failed to run error callback"}
 
     return {"success": True}
 
 
-def create_route_handler(router: dict[str, UploadThingBuilder]):
+def create_route_handler(
+    router: dict[str, UploadThingBuilder], api_key: str, is_dev: bool
+):
+    """
+    Create request handlers for client side uploads
+
+    ### Example usage:
+    ```py
+    from fastapi import FastAPI, Request, Response
+    from uploadthing_py import (
+        create_uploadthing,
+        UploadThingRequestBody,
+        create_route_handler,
+    )
+    from fastapi.middleware.cors import CORSMiddleware
+    import os
+
+    app = FastAPI()
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=["*"],
+        allow_methods=["*"],
+        allow_headers=["*"],
+    )
+
+    f = create_uploadthing()
+
+
+    upload_router = {
+        "videoAndImage": f(
+            {
+                "image/png": {"max_file_size": "4MB"},
+                "image/heic": {"max_file_size": "16MB"},
+            }
+        )
+        .middleware(lambda req: {"user_id": req.headers["x-user-id"]})
+        .on_upload_complete(lambda file, metadata: print(f"Upload complete for {metadata['user_id']}"))
+    }
+    handlers = create_route_handler(
+        router=upload_router,
+        api_key=os.getenv("UPLOADTHING_SECRET"),
+        is_dev=os.getenv("ENVIRONMENT", "development") == "development",
+    )
+
+
+    @app.get("/api")
+    async def greeting():
+        return "Hello from FastAPI"
+    
+    
+    @app.get("/api/uploadthing")
+    async def ut_get():
+        return handlers["GET"]()
+    
+    
+    @app.post("/api/uploadthing")
+    async def ut_post(
+        request: Request,
+        response: Response,
+        body: UploadThingRequestBody,
+    ):
+        return await handlers["POST"](
+            request=request,
+            response=response,
+            body=body,
+        )
+    ```
+    """
+    
     def ut_get():
         return extract_router_config(router)
 
     async def ut_post(
         request: Request,
         response: Response,
         body: Union[UploadRequest, CallbackRequest, CompleteMPURequest],
     ):
+        if not api_key:
+            response.status_code = 500
+            return {"error": "No API key provided"}
+
         if "slug" not in request.query_params:
             response.status_code = 400
             return {"error": "Missing slug parameter"}
         slug = request.query_params["slug"]
 
         if slug not in router:
             response.status_code = 404
@@ -280,23 +337,32 @@
             request.headers["uploadthing-hook"]
             if "uploadthing-hook" in request.headers
             else None
         )
 
         match [uploadthing_hook, action_type]:
             case ["callback", None]:
-                return await handle_callback_request(uploader=uploader, body=body)
+                return await handle_callback_request(
+                    uploader=uploader, body=body, api_key=api_key
+                )
             case [None, "upload"]:
                 return await handle_upload_request(
-                    uploader=uploader, request=request, body=body, slug=slug
+                    uploader=uploader,
+                    request=request,
+                    body=body,
+                    slug=slug,
+                    api_key=api_key,
+                    is_dev=is_dev,
                 )
             case [None, "failure"]:
-                return await handle_failure_request(uploader=uploader, body=body)
+                return await handle_failure_request(
+                    uploader=uploader, body=body, api_key=api_key
+                )
             case [None, "multipart-complete"]:
-                return await handle_complete_mpu_request(body=body)
+                return await handle_complete_mpu_request(body=body, api_key=api_key)
             case _:
                 response.status_code = 400
                 return {
                     "error": "Bad request. Invalid hook header or actionType parameter"
                 }
 
     return {"GET": ut_get, "POST": ut_post}
```

### Comparing `uploadthing_py-0.2.0/uploadthing_py/types.py` & `uploadthing_py-0.2.1/uploadthing_py/types.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.0/uploadthing_py/utapi.py` & `uploadthing_py-0.2.1/uploadthing_py/utapi.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.0/uploadthing_py/utils.py` & `uploadthing_py-0.2.1/uploadthing_py/utils.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.2.0/PKG-INFO` & `uploadthing_py-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uploadthing.py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for UploadThing
 License: MIT
 Author: juliusmarminge
 Author-email: julius0216@outlook.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -61,15 +61,15 @@
 from fastapi import FastAPI, Request, Response
 from uploadthing_py import (
     create_uploadthing,
     UploadThingRequestBody,
     create_route_handler,
 )
 from fastapi.middleware.cors import CORSMiddleware
-
+import os
 
 app = FastAPI()
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_methods=["*"],
     allow_headers=["*"],
@@ -84,15 +84,19 @@
             "image/png": {"max_file_size": "4MB"},
             "image/heic": {"max_file_size": "16MB"},
         }
     )
     .middleware(lambda req: {"user_id": req.headers["x-user-id"]})
     .on_upload_complete(lambda file, metadata: print(f"Upload complete for {metadata['user_id']}"))
 }
-handlers = create_route_handler(router=upload_router)
+handlers = create_route_handler(
+    router=upload_router,
+    api_key=os.getenv("UPLOADTHING_SECRET"),
+    is_dev=os.getenv("ENVIRONMENT", "development") == "development",
+)
 
 
 @app.get("/api")
 async def greeting():
     return "Hello from FastAPI"
```


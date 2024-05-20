# Comparing `tmp/gen_wrappers-0.4.1.tar.gz` & `tmp/gen_wrappers-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.4.1.tar", last modified: Mon May 20 14:37:23 2024, max compression
+gzip compressed data, was "gen_wrappers-0.4.2.tar", last modified: Mon May 20 15:23:43 2024, max compression
```

## Comparing `gen_wrappers-0.4.1.tar` & `gen_wrappers-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.429890 gen_wrappers-0.4.1/
--rw-rw-rw-   0        0        0      847 2024-05-20 14:37:23.428449 gen_wrappers-0.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.151712 gen_wrappers-0.4.1/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.1/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.203138 gen_wrappers-0.4.1/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.1/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6045 2024-05-20 14:25:08.000000 gen_wrappers-0.4.1/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.1/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.1/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.262553 gen_wrappers-0.4.1/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.1/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1582 2024-05-20 14:12:32.000000 gen_wrappers-0.4.1/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.4.1/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.1/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.1/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.290011 gen_wrappers-0.4.1/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.1/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9805 2024-05-20 14:30:44.000000 gen_wrappers-0.4.1/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    16238 2024-05-20 14:12:32.000000 gen_wrappers-0.4.1/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.1/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.337563 gen_wrappers-0.4.1/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.1/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6813 2024-05-20 14:30:44.000000 gen_wrappers-0.4.1/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.4.1/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.1/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.361023 gen_wrappers-0.4.1/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.1/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.1/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.424444 gen_wrappers-0.4.1/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-20 14:37:22.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-20 14:37:23.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 14:37:22.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-20 14:37:22.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 14:37:22.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 14:37:23.429890 gen_wrappers-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-20 14:32:51.000000 gen_wrappers-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.189585 gen_wrappers-0.4.2/
+-rw-rw-rw-   0        0        0      847 2024-05-20 15:23:43.188217 gen_wrappers-0.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 15:23:42.771813 gen_wrappers-0.4.2/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.2/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:23:42.843507 gen_wrappers-0.4.2/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.2/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     7135 2024-05-20 15:04:33.000000 gen_wrappers-0.4.2/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.2/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.2/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:23:42.934893 gen_wrappers-0.4.2/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.2/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1582 2024-05-20 14:12:32.000000 gen_wrappers-0.4.2/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.4.2/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.2/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.2/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.013774 gen_wrappers-0.4.2/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.2/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9850 2024-05-20 15:04:33.000000 gen_wrappers-0.4.2/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    16238 2024-05-20 14:12:32.000000 gen_wrappers-0.4.2/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.2/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.108579 gen_wrappers-0.4.2/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.2/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6853 2024-05-20 15:04:33.000000 gen_wrappers-0.4.2/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.4.2/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.2/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.115508 gen_wrappers-0.4.2/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.2/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.2/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.184884 gen_wrappers-0.4.2/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 15:23:43.190603 gen_wrappers-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-20 15:07:41.000000 gen_wrappers-0.4.2/setup.py
```

### Comparing `gen_wrappers-0.4.1/PKG-INFO` & `gen_wrappers-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.4.1
+Version: 0.4.2
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.1/creator/auto/creator_auto.py` & `gen_wrappers-0.4.2/creator/auto/creator_auto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import json
 import logging
 import os
 import traceback
 from typing import Any, List, Union
 
 import httpx
 
@@ -25,20 +26,32 @@
         super().__init__()
         auto_port = os.environ.get("PORT_AUTO", 8081)
         if isinstance(auto_port, str):
             auto_port = int(auto_port)
         self.jobs = {}
         self.output = {}
         self.api_base_url = f"http://0.0.0.0:{auto_port}/sdapi"
+        app_config_path = "/opt/rd/apps/stable-diffusion-webui/config.json"
+        if os.path.exists(app_config_path):
+            with open(app_config_path, "r") as f:
+                app_config = json.load(f)
+                default_checkpoint = app_config.get("sd_model_checkpoint", None)
+                if default_checkpoint:
+                    self.loaded_models.append(default_checkpoint)
 
     async def create(self, params: Union[AutoTxt2Img, AutoImg2Img], job_id=None) -> BaseResponse:
         print(f"Creating job with params: {params}")
         endpoint_name = "txt2img" if isinstance(params, AutoTxt2Img) else "img2img"
         url = f"{self.api_base_url}/agent-scheduler/v1/{endpoint_name}"
         data = params.model_dump()
+        checkpoint = data.get("sd_model_checkpoint", None)
+        if checkpoint and checkpoint not in self.loaded_models:
+            self.loaded_models.append(checkpoint)
+            if len(self.loaded_models) > 3:
+                self.loaded_models.pop(0)
         headers = {'Content-Type': 'application/json'}
         async with httpx.AsyncClient() as client:
             response = await client.post(url, data=data, headers=headers)
             response.raise_for_status()
         output = response.json()
         task_id = output.get("task_id", None)
         print(f"Response received: {output}")
@@ -50,14 +63,19 @@
             return result
 
     async def create_async(self, params: Union[AutoTxt2Img, AutoImg2Img]) -> BaseResponse:
         endpoint_name = "txt2img" if isinstance(params, AutoTxt2Img) else "img2img"
         url = f"{self.api_base_url}/agent-scheduler/v1/queue/{endpoint_name}"
         data = params.model_dump()
         headers = {'Content-Type': 'application/json'}
+        checkpoint = data.get("sd_model_checkpoint", None)
+        if checkpoint and checkpoint not in self.loaded_models:
+            self.loaded_models.append(checkpoint)
+            if len(self.loaded_models) > 3:
+                self.loaded_models.pop(0)
         try:
             async with httpx.AsyncClient() as client:
                 response = await client.post(url, data=data, headers=headers)
                 response.raise_for_status()
             output = response.json()
             task_id = output.get("task_id", None)
             if task_id:
@@ -119,25 +137,26 @@
         async with httpx.AsyncClient() as client:
             response = await client.get(url)
             if response.status_code == 200:
                 return BaseResponse.active()
             else:
                 return BaseResponse.error("Error testing connection")
 
-    async def cache_model(self, model: str) -> bool:
-        #"sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"
+    async def cache_model(self, model: str = "Juggernaut-XI-Prototype.safetensors") -> bool:
         request = {
             "sd_model_checkpoint": model
         }
+        if model not in self.loaded_models:
+            self.loaded_models.append(model)
+        if len(self.loaded_models) > 3:
+            self.loaded_models.pop(0)
         url = f"{self.api_base_url}/sdapi/v1/options"
         headers = {'Content-Type': 'application/json'}
         async with httpx.AsyncClient() as client:
             response = await client.post(url, json=request, headers=headers)
             response.raise_for_status()
             if response.status_code == 200:
                 # Sleep for 15 seconds to allow the model to be cached
                 await asyncio.sleep(15)
                 return True
             print(f"Error caching model: {response.text}")
         return False
-
-
```

### Comparing `gen_wrappers-0.4.1/creator/auto/request_auto.py` & `gen_wrappers-0.4.2/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/creator/auto/response_auto.py` & `gen_wrappers-0.4.2/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/creator/base/base_app.py` & `gen_wrappers-0.4.2/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/creator/base/base_request.py` & `gen_wrappers-0.4.2/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/creator/base/base_response.py` & `gen_wrappers-0.4.2/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.4.2/creator/cmfy/creator_cmfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
                         self.loaded_models.append(model_name)
             except KeyError:
                 continue
         max_cached_models = os.environ.get("MAX_CACHED_MODELS", 3)
         if len(self.loaded_models) > max_cached_models:
             self.loaded_models = self.loaded_models[-max_cached_models:]
 
-    async def cache_model(self, model) -> bool:
+    async def cache_model(self, model: str = "Juggernaut-XI-Prototype.safetensors") -> bool:
         request_json = model_load_json
         request_json["1"]['inputs']['ckpt_name'] = model
         request = CmfyWorkflow(workflow_json=json.dumps(request_json))
         self._check_loaded_model(request_json)
         response = await self.create(request)
         if response.status == JobStatus.FINISHED:
             return True
```

### Comparing `gen_wrappers-0.4.1/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.4.2/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.4.2/creator/fcus_api/creator_fcus_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             if status is None:
                 return None
             if status != "Finished":
                 return []
             outputs = [result.get('base64') for result in response_json.get('job_result', []) if result.get('finish_reason', "UNKNOWN") == "SUCCESS"]
             return outputs
 
-    async def cache_model(self, model: str) -> bool:
+    async def cache_model(self, model: str = "Juggernaut-XI-Prototype.safetensors") -> bool:
         # FCUS_API doesn't have a specific endpoint for caching models, so we just
         # Run a txt2img job with a very low resolution to load the model
         request = FcusTxt2Img(prompt="a", negative_prompt="b", image_number=1, base_model_name=model, aspect_ratio_slection="64*64")
         response = await self.create(request)
         if response.status == JobStatus.FINISHED:
             return True
         return False
```

### Comparing `gen_wrappers-0.4.1/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.4.2/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.4.2/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/creator/util/helper.py` & `gen_wrappers-0.4.2/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.1/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.4.2/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.4.1
+Version: 0.4.2
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.1/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.4.2/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*


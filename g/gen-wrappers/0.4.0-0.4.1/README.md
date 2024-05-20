# Comparing `tmp/gen_wrappers-0.4.0.tar.gz` & `tmp/gen_wrappers-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.4.0.tar", last modified: Sun May 19 17:58:41 2024, max compression
+gzip compressed data, was "gen_wrappers-0.4.1.tar", last modified: Mon May 20 14:37:23 2024, max compression
```

## Comparing `gen_wrappers-0.4.0.tar` & `gen_wrappers-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 17:58:41.149246 gen_wrappers-0.4.0/
--rw-rw-rw-   0        0        0      847 2024-05-19 17:58:41.147246 gen_wrappers-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 17:58:40.807706 gen_wrappers-0.4.0/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.0/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:58:40.875093 gen_wrappers-0.4.0/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.0/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5302 2024-05-14 15:42:23.000000 gen_wrappers-0.4.0/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.0/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.0/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:58:40.943376 gen_wrappers-0.4.0/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.0/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1491 2024-05-14 15:42:23.000000 gen_wrappers-0.4.0/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.4.0/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.0/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.0/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:58:40.986465 gen_wrappers-0.4.0/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.0/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9355 2024-05-17 02:24:46.000000 gen_wrappers-0.4.0/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    12644 2024-05-19 17:58:23.000000 gen_wrappers-0.4.0/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.0/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:58:41.052863 gen_wrappers-0.4.0/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.0/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6273 2024-05-14 15:42:23.000000 gen_wrappers-0.4.0/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.4.0/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.0/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:58:41.073847 gen_wrappers-0.4.0/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.0/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.0/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:58:41.143798 gen_wrappers-0.4.0/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 17:58:41.149246 gen_wrappers-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-19 17:58:23.000000 gen_wrappers-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.429890 gen_wrappers-0.4.1/
+-rw-rw-rw-   0        0        0      847 2024-05-20 14:37:23.428449 gen_wrappers-0.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.151712 gen_wrappers-0.4.1/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.1/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.203138 gen_wrappers-0.4.1/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.1/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6045 2024-05-20 14:25:08.000000 gen_wrappers-0.4.1/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.1/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.1/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.262553 gen_wrappers-0.4.1/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.1/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1582 2024-05-20 14:12:32.000000 gen_wrappers-0.4.1/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.4.1/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.1/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.1/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.290011 gen_wrappers-0.4.1/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.1/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9805 2024-05-20 14:30:44.000000 gen_wrappers-0.4.1/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    16238 2024-05-20 14:12:32.000000 gen_wrappers-0.4.1/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.1/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.337563 gen_wrappers-0.4.1/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.1/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6813 2024-05-20 14:30:44.000000 gen_wrappers-0.4.1/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.4.1/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.1/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.361023 gen_wrappers-0.4.1/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.1/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.1/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:37:23.424444 gen_wrappers-0.4.1/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-20 14:37:22.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-20 14:37:23.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:37:22.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-20 14:37:22.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 14:37:22.000000 gen_wrappers-0.4.1/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:37:23.429890 gen_wrappers-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-20 14:32:51.000000 gen_wrappers-0.4.1/setup.py
```

### Comparing `gen_wrappers-0.4.0/PKG-INFO` & `gen_wrappers-0.4.1/gen_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gen_wrappers
-Version: 0.4.0
+Name: gen-wrappers
+Version: 0.4.1
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.0/creator/auto/creator_auto.py` & `gen_wrappers-0.4.1/creator/auto/creator_auto.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,8 +119,25 @@
         async with httpx.AsyncClient() as client:
             response = await client.get(url)
             if response.status_code == 200:
                 return BaseResponse.active()
             else:
                 return BaseResponse.error("Error testing connection")
 
+    async def cache_model(self, model: str) -> bool:
+        #"sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"
+        request = {
+            "sd_model_checkpoint": model
+        }
+        url = f"{self.api_base_url}/sdapi/v1/options"
+        headers = {'Content-Type': 'application/json'}
+        async with httpx.AsyncClient() as client:
+            response = await client.post(url, json=request, headers=headers)
+            response.raise_for_status()
+            if response.status_code == 200:
+                # Sleep for 15 seconds to allow the model to be cached
+                await asyncio.sleep(15)
+                return True
+            print(f"Error caching model: {response.text}")
+        return False
+
```

### Comparing `gen_wrappers-0.4.0/creator/auto/request_auto.py` & `gen_wrappers-0.4.1/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.0/creator/auto/response_auto.py` & `gen_wrappers-0.4.1/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.0/creator/base/base_app.py` & `gen_wrappers-0.4.1/creator/base/base_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,18 @@
         """Get the status of an asynchronous job."""
         pass
 
     @abstractmethod
     async def get_models(self) -> List[Any]:
         pass
 
+    @abstractmethod
+    async def cache_model(self, model: str) -> bool:
+        pass
+
     async def get_loaded_models(self) -> BaseResponse:
         base_response = BaseResponse(status=JobStatus.FINISHED)
         base_response_data = ResponseData(data=self.loaded_models, data_type=ResponseDataType.TEXT, total_count=len(self.loaded_models))
         base_response.output = base_response_data
         return base_response
 
     @abstractmethod
```

### Comparing `gen_wrappers-0.4.0/creator/base/base_request.py` & `gen_wrappers-0.4.1/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.0/creator/base/base_response.py` & `gen_wrappers-0.4.1/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.0/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.4.1/creator/cmfy/creator_cmfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import httpx
 import requests
 
 from creator.base.base_app import BaseApp
 from creator.base.base_response import ResponseDataType, ResponseData, BaseResponse
 from creator.base.job_status import JobStatus
-from creator.cmfy.request_cmfy import CmfyWorkflow, CmfyWorkflowFcus
+from creator.cmfy.request_cmfy import CmfyWorkflow, CmfyWorkflowFcus, model_load_json
 from creator.cmfy.response_cmfy import ResponseCmfy
 
 logger = logging.getLogger(__name__)
 
 
 class AppCmfy(BaseApp):
     param_classes = [CmfyWorkflow, CmfyWorkflowFcus]
@@ -183,16 +183,27 @@
         except Exception as e:
             logger.error(f"Failed to retrieve or encode image: {e}")
             return None
 
     def _check_loaded_model(self, workflow: Dict[str, Any]):
         for node_id, node in workflow.items():
             try:
-                if node['class_type'] == "CheckpointLoaderSimple":
-                    model_name = node['inputs']['ckpt_name']
+                if node['class_type'].contains("CheckpointLoaderSimple"):
+                    model_name = node['inputs'].get('ckpt_name', None)
                     if model_name and model_name not in self.loaded_models:
                         self.loaded_models.append(model_name)
             except KeyError:
                 continue
         max_cached_models = os.environ.get("MAX_CACHED_MODELS", 3)
         if len(self.loaded_models) > max_cached_models:
             self.loaded_models = self.loaded_models[-max_cached_models:]
+
+    async def cache_model(self, model) -> bool:
+        request_json = model_load_json
+        request_json["1"]['inputs']['ckpt_name'] = model
+        request = CmfyWorkflow(workflow_json=json.dumps(request_json))
+        self._check_loaded_model(request_json)
+        response = await self.create(request)
+        if response.status == JobStatus.FINISHED:
+            return True
+        return False
+
```

### Comparing `gen_wrappers-0.4.0/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.4.1/creator/cmfy/request_cmfy.py`

 * *Files 20% similar despite different names*

```diff
@@ -111,420 +111,479 @@
         "_meta": {
             "title": "Save Image"
         }
     }
 }
 
 default_workflow_json_2 = {
-  "21": {
-    "inputs": {
-      "width": 1920,
-      "height": 1080,
-      "batch_size": 2
-    },
-    "class_type": "EmptyLatentImage",
-    "_meta": {
-      "title": "Empty Latent Image"
-    }
-  },
-  "67": {
-    "inputs": {
-      "samples": [
-        "132",
-        0
-      ],
-      "vae": [
-        "135",
-        2
-      ]
-    },
-    "class_type": "VAEDecode",
-    "_meta": {
-      "title": "VAE Decode"
-    }
-  },
-  "99": {
-    "inputs": {
-      "seed": 1011799137402762
-    },
-    "class_type": "CR Seed",
-    "_meta": {
-      "title": "🌱 CR Seed"
-    }
-  },
-  "100": {
-    "inputs": {
-      "text": [
-        "114:0",
-        0
-      ],
-      "seed": [
-        "99",
-        0
-      ],
-      "log_prompt": "No"
-    },
-    "class_type": "PromptExpansion",
-    "_meta": {
-      "title": "Prompt Expansion"
-    }
-  },
-  "101": {
-    "inputs": {
-      "text": [
-        "144",
-        0
-      ]
-    },
-    "class_type": "ShowText|pysssss",
-    "_meta": {
-      "title": "Show Text 🐍"
-    }
-  },
-  "102": {
-    "inputs": {
-      "text": [
-        "145",
-        0
-      ]
-    },
-    "class_type": "ShowText|pysssss",
-    "_meta": {
-      "title": "Show Text 🐍"
-    }
-  },
-  "120": {
-    "inputs": {
-      "b1": 1.01,
-      "b2": 1.02,
-      "s1": 0.99,
-      "s2": 0.9500000000000001,
-      "model": [
-        "135",
-        0
-      ]
-    },
-    "class_type": "FreeU_V2",
-    "_meta": {
-      "title": "FreeU_V2"
-    }
-  },
-  "132": {
-    "inputs": {
-      "add_noise": False,
-      "noise_seed": [
-        "99",
-        0
-      ],
-      "steps": 15,
-      "cfg": 4,
-      "sampler_name": "euler_ancestral",
-      "scheduler": "karras",
-      "start_at_step": 0,
-      "end_at_step": 10000,
-      "noise_mode": "CPU",
-      "return_with_leftover_noise": False,
-      "batch_seed_mode": "incremental",
-      "variation_seed": 0,
-      "variation_strength": 0,
-      "model": [
-        "134",
-        0
-      ],
-      "positive": [
-        "138:1",
-        0
-      ],
-      "negative": [
-        "138:0",
-        0
-      ],
-      "latent_image": [
-        "21",
-        0
-      ]
-    },
-    "class_type": "KSamplerAdvanced //Inspire",
-    "_meta": {
-      "title": "KSamplerAdvanced (inspire)"
-    }
-  },
-  "134": {
-    "inputs": {
-      "ds_depth_1": 3,
-      "ds_depth_2": 3,
-      "ds_timestep_1": 900,
-      "ds_timestep_2": 650,
-      "resize_scale_1": 2,
-      "resize_scale_2": 2,
-      "model": [
-        "120",
-        0
-      ]
-    },
-    "class_type": "Hires",
-    "_meta": {
-      "title": "Apply Kohya's HiresFix"
-    }
-  },
-  "135": {
-    "inputs": {
-      "ckpt_name": "Juggernaut-XI-Prototype.safetensors",
-      "key_opt": "",
-      "mode": "Auto"
-    },
-    "class_type": "CheckpointLoaderSimpleShared //Inspire",
-    "_meta": {
-      "title": "Shared Checkpoint Loader (Inspire)"
-    }
-  },
-  "139": {
-    "inputs": {
-      "prompt": "three squirrels in business suits having a meeting at a tiny table in a park"
-    },
-    "class_type": "CR Prompt Text",
-    "_meta": {
-      "title": "⚙️ CR Prompt Text"
-    }
-  },
-  "140": {
-    "inputs": {
-      "prompt": "blurry, bad eyes, bad hands, deformed, low quality"
-    },
-    "class_type": "CR Prompt Text",
-    "_meta": {
-      "title": "⚙️ CR Prompt Text"
-    }
-  },
-  "144": {
-    "inputs": {
-      "action": "replace",
-      "tidy_tags": "yes",
-      "text_a": [
-        "100",
-        0
-      ],
-      "text_b": "",
-      "text_c": "",
-      "result": "three squirrels in business suits having a meeting at a tiny table in a park, professional photograph, bokeh, 8k detailed, 35mm, vintage, highly detailed, found footage, cinematic still, emotional, harmonious, vignette, 4k detailed, sharp focus, high budget, epic, gorgeous, film grain, three squirrels in business suits having a meeting at a tiny table in a park, professional photograph, bokeh, 8k detailed, 35mm, vintage, highly detailed, found footage, cinematic still, emotional, harmonious, vignette, 4k detailed, sharp focus, high budget, epic, gorgeous, film grain, atmosphere, bright, rich vivid colors"
-    },
-    "class_type": "StringFunction|pysssss",
-    "_meta": {
-      "title": "String Function 🐍"
-    }
-  },
-  "145": {
-    "inputs": {
-      "action": "replace",
-      "tidy_tags": "yes",
-      "text_a": [
-        "114:1",
-        0
-      ],
-      "text_b": "",
-      "text_c": "",
-      "result": "blurry, bad eyes, bad hands, deformed, low quality, blurry, cropped, bad face, saturated, contrast, deformed iris, deformed pupils, semi-realistic, cgi, 3d, render, sketch, cartoon, drawing, anime, text, cropped, out of frame, worst quality, low quality, jpeg artifacts, ugly, duplicate, morbid, mutilated, extra fingers, mutated hands, poorly drawn hands, poorly drawn face, mutation, deformed, dehydrated, bad anatomy, bad proportions, extra limbs, cloned face, disfigured, gross proportions, malformed limbs, missing arms, missing legs, extra arms, extra legs, fused fingers, too many fingers, long neck, anime, cartoon, graphic, (blur, blurry, bokeh), text, painting, crayon, graphite, abstract, glitch, deformed, mutated, ugly, disfigured, deformed, bad anatomy, disfigured, poorly drawn face, mutated, extra limb, ugly, poorly drawn hands, missing limb, floating limbs, disconnected limbs, disconnected head, malformed hands, long neck, mutated hands and fingers, bad hands, missing fingers, cropped, worst quality, low quality, mutation, poorly drawn, huge calf, bad hands, fused hand, missing hand, disappearing arms, disappearing thigh, disappearing calf, disappearing legs, missing fingers, fused fingers, abnormal eye proportion, Abnormal hands, abnormal legs, abnormal feet, abnormal fingers, drawing, painting, crayon, sketch, graphite, impressionist, noisy, blurry, soft, deformed, ugly, anime, cartoon, graphic, text, painting, crayon, graphite, abstract, glitch"
-    },
-    "class_type": "StringFunction|pysssss",
-    "_meta": {
-      "title": "String Function 🐍"
-    }
-  },
-  "148": {
-    "inputs": {
-      "filename_prefix": [
-        "139",
-        0
-      ],
-      "images": [
-        "67",
-        0
-      ]
-    },
-    "class_type": "SaveImage",
-    "_meta": {
-      "title": "Save Image"
-    }
-  },
-  "119:0": {
-    "inputs": {
-      "text_positive": "",
-      "text_negative": "",
-      "style": "Fooocus Photograph",
-      "log_prompt": True,
-      "style_positive": True,
-      "style_negative": True
-    },
-    "class_type": "SDXLPromptStyler",
-    "_meta": {
-      "title": "SDXL Prompt Styler"
-    }
-  },
-  "119:1": {
-    "inputs": {
-      "text_positive": "",
-      "text_negative": "",
-      "style": "Fooocus Sharp",
-      "log_prompt": True,
-      "style_positive": True,
-      "style_negative": True
-    },
-    "class_type": "SDXLPromptStyler",
-    "_meta": {
-      "title": "SDXL Prompt Styler"
-    }
-  },
-  "119:2": {
-    "inputs": {
-      "text_positive": "",
-      "text_negative": "",
-      "style": "Fooocus Negative",
-      "log_prompt": True,
-      "style_positive": True,
-      "style_negative": True
-    },
-    "class_type": "SDXLPromptStyler",
-    "_meta": {
-      "title": "SDXL Prompt Styler"
-    }
-  },
-  "133:1": {
-    "inputs": {
-      "text1": [
-        "140",
-        0
-      ],
-      "text2": [
-        "119:0",
-        1
-      ],
-      "separator": ", "
-    },
-    "class_type": "CR Text Concatenate",
-    "_meta": {
-      "title": "🔤 CR Text Concatenate"
-    }
-  },
-  "133:2": {
-    "inputs": {
-      "text1": [
-        "119:1",
-        0
-      ],
-      "text2": [
-        "119:2",
-        0
-      ],
-      "separator": ", "
-    },
-    "class_type": "CR Text Concatenate",
-    "_meta": {
-      "title": "🔤 CR Text Concatenate"
-    }
-  },
-  "133:3": {
-    "inputs": {
-      "text1": [
-        "119:1",
-        1
-      ],
-      "text2": [
-        "119:2",
-        1
-      ],
-      "separator": ", "
-    },
-    "class_type": "CR Text Concatenate",
-    "_meta": {
-      "title": "🔤 CR Text Concatenate"
-    }
-  },
-  "133:0": {
-    "inputs": {
-      "text1": [
-        "139",
-        0
-      ],
-      "text2": [
-        "119:0",
-        0
-      ],
-      "separator": ", "
-    },
-    "class_type": "CR Text Concatenate",
-    "_meta": {
-      "title": "🔤 CR Text Concatenate"
-    }
-  },
-  "114:1": {
-    "inputs": {
-      "text1": [
-        "133:1",
-        0
-      ],
-      "text2": [
-        "133:3",
-        0
-      ],
-      "separator": ", "
-    },
-    "class_type": "CR Text Concatenate",
-    "_meta": {
-      "title": "🔤 CR Text Concatenate"
-    }
-  },
-  "114:0": {
-    "inputs": {
-      "text1": [
-        "133:0",
-        0
-      ],
-      "text2": [
-        "133:2",
-        0
-      ],
-      "separator": ", "
-    },
-    "class_type": "CR Text Concatenate",
-    "_meta": {
-      "title": "🔤 CR Text Concatenate"
-    }
-  },
-  "138:0": {
-    "inputs": {
-      "text": [
-        "102",
-        0
-      ],
-      "clip": [
-        "135",
-        1
-      ]
-    },
-    "class_type": "CLIPTextEncode",
-    "_meta": {
-      "title": "CLIP Text Encode (Prompt)"
+    "21": {
+        "inputs": {
+            "width": 1920,
+            "height": 1080,
+            "batch_size": 2
+        },
+        "class_type": "EmptyLatentImage",
+        "_meta": {
+            "title": "Empty Latent Image"
+        }
+    },
+    "67": {
+        "inputs": {
+            "samples": [
+                "132",
+                0
+            ],
+            "vae": [
+                "135",
+                2
+            ]
+        },
+        "class_type": "VAEDecode",
+        "_meta": {
+            "title": "VAE Decode"
+        }
+    },
+    "99": {
+        "inputs": {
+            "seed": 1011799137402762
+        },
+        "class_type": "CR Seed",
+        "_meta": {
+            "title": "🌱 CR Seed"
+        }
+    },
+    "100": {
+        "inputs": {
+            "text": [
+                "114:0",
+                0
+            ],
+            "seed": [
+                "99",
+                0
+            ],
+            "log_prompt": "No"
+        },
+        "class_type": "PromptExpansion",
+        "_meta": {
+            "title": "Prompt Expansion"
+        }
+    },
+    "101": {
+        "inputs": {
+            "text": [
+                "144",
+                0
+            ]
+        },
+        "class_type": "ShowText|pysssss",
+        "_meta": {
+            "title": "Show Text 🐍"
+        }
+    },
+    "102": {
+        "inputs": {
+            "text": [
+                "145",
+                0
+            ]
+        },
+        "class_type": "ShowText|pysssss",
+        "_meta": {
+            "title": "Show Text 🐍"
+        }
+    },
+    "120": {
+        "inputs": {
+            "b1": 1.01,
+            "b2": 1.02,
+            "s1": 0.99,
+            "s2": 0.9500000000000001,
+            "model": [
+                "135",
+                0
+            ]
+        },
+        "class_type": "FreeU_V2",
+        "_meta": {
+            "title": "FreeU_V2"
+        }
+    },
+    "132": {
+        "inputs": {
+            "add_noise": False,
+            "noise_seed": [
+                "99",
+                0
+            ],
+            "steps": 15,
+            "cfg": 4,
+            "sampler_name": "euler_ancestral",
+            "scheduler": "karras",
+            "start_at_step": 0,
+            "end_at_step": 10000,
+            "noise_mode": "CPU",
+            "return_with_leftover_noise": False,
+            "batch_seed_mode": "incremental",
+            "variation_seed": 0,
+            "variation_strength": 0,
+            "model": [
+                "134",
+                0
+            ],
+            "positive": [
+                "138:1",
+                0
+            ],
+            "negative": [
+                "138:0",
+                0
+            ],
+            "latent_image": [
+                "21",
+                0
+            ]
+        },
+        "class_type": "KSamplerAdvanced //Inspire",
+        "_meta": {
+            "title": "KSamplerAdvanced (inspire)"
+        }
+    },
+    "134": {
+        "inputs": {
+            "ds_depth_1": 3,
+            "ds_depth_2": 3,
+            "ds_timestep_1": 900,
+            "ds_timestep_2": 650,
+            "resize_scale_1": 2,
+            "resize_scale_2": 2,
+            "model": [
+                "120",
+                0
+            ]
+        },
+        "class_type": "Hires",
+        "_meta": {
+            "title": "Apply Kohya's HiresFix"
+        }
+    },
+    "135": {
+        "inputs": {
+            "ckpt_name": "Juggernaut-XI-Prototype.safetensors",
+            "key_opt": "",
+            "mode": "Auto"
+        },
+        "class_type": "CheckpointLoaderSimpleShared //Inspire",
+        "_meta": {
+            "title": "Shared Checkpoint Loader (Inspire)"
+        }
+    },
+    "139": {
+        "inputs": {
+            "prompt": "three squirrels in business suits having a meeting at a tiny table in a park"
+        },
+        "class_type": "CR Prompt Text",
+        "_meta": {
+            "title": "⚙️ CR Prompt Text"
+        }
+    },
+    "140": {
+        "inputs": {
+            "prompt": "blurry, bad eyes, bad hands, deformed, low quality"
+        },
+        "class_type": "CR Prompt Text",
+        "_meta": {
+            "title": "⚙️ CR Prompt Text"
+        }
+    },
+    "144": {
+        "inputs": {
+            "action": "replace",
+            "tidy_tags": "yes",
+            "text_a": [
+                "100",
+                0
+            ],
+            "text_b": "",
+            "text_c": "",
+            "result": "three squirrels in business suits having a meeting at a tiny table in a park, professional photograph, bokeh, 8k detailed, 35mm, vintage, highly detailed, found footage, cinematic still, emotional, harmonious, vignette, 4k detailed, sharp focus, high budget, epic, gorgeous, film grain, three squirrels in business suits having a meeting at a tiny table in a park, professional photograph, bokeh, 8k detailed, 35mm, vintage, highly detailed, found footage, cinematic still, emotional, harmonious, vignette, 4k detailed, sharp focus, high budget, epic, gorgeous, film grain, atmosphere, bright, rich vivid colors"
+        },
+        "class_type": "StringFunction|pysssss",
+        "_meta": {
+            "title": "String Function 🐍"
+        }
+    },
+    "145": {
+        "inputs": {
+            "action": "replace",
+            "tidy_tags": "yes",
+            "text_a": [
+                "114:1",
+                0
+            ],
+            "text_b": "",
+            "text_c": "",
+            "result": "blurry, bad eyes, bad hands, deformed, low quality, blurry, cropped, bad face, saturated, contrast, deformed iris, deformed pupils, semi-realistic, cgi, 3d, render, sketch, cartoon, drawing, anime, text, cropped, out of frame, worst quality, low quality, jpeg artifacts, ugly, duplicate, morbid, mutilated, extra fingers, mutated hands, poorly drawn hands, poorly drawn face, mutation, deformed, dehydrated, bad anatomy, bad proportions, extra limbs, cloned face, disfigured, gross proportions, malformed limbs, missing arms, missing legs, extra arms, extra legs, fused fingers, too many fingers, long neck, anime, cartoon, graphic, (blur, blurry, bokeh), text, painting, crayon, graphite, abstract, glitch, deformed, mutated, ugly, disfigured, deformed, bad anatomy, disfigured, poorly drawn face, mutated, extra limb, ugly, poorly drawn hands, missing limb, floating limbs, disconnected limbs, disconnected head, malformed hands, long neck, mutated hands and fingers, bad hands, missing fingers, cropped, worst quality, low quality, mutation, poorly drawn, huge calf, bad hands, fused hand, missing hand, disappearing arms, disappearing thigh, disappearing calf, disappearing legs, missing fingers, fused fingers, abnormal eye proportion, Abnormal hands, abnormal legs, abnormal feet, abnormal fingers, drawing, painting, crayon, sketch, graphite, impressionist, noisy, blurry, soft, deformed, ugly, anime, cartoon, graphic, text, painting, crayon, graphite, abstract, glitch"
+        },
+        "class_type": "StringFunction|pysssss",
+        "_meta": {
+            "title": "String Function 🐍"
+        }
+    },
+    "148": {
+        "inputs": {
+            "filename_prefix": [
+                "139",
+                0
+            ],
+            "images": [
+                "67",
+                0
+            ]
+        },
+        "class_type": "SaveImage",
+        "_meta": {
+            "title": "Save Image"
+        }
+    },
+    "119:0": {
+        "inputs": {
+            "text_positive": "",
+            "text_negative": "",
+            "style": "Fooocus Photograph",
+            "log_prompt": True,
+            "style_positive": True,
+            "style_negative": True
+        },
+        "class_type": "SDXLPromptStyler",
+        "_meta": {
+            "title": "SDXL Prompt Styler"
+        }
+    },
+    "119:1": {
+        "inputs": {
+            "text_positive": "",
+            "text_negative": "",
+            "style": "Fooocus Sharp",
+            "log_prompt": True,
+            "style_positive": True,
+            "style_negative": True
+        },
+        "class_type": "SDXLPromptStyler",
+        "_meta": {
+            "title": "SDXL Prompt Styler"
+        }
+    },
+    "119:2": {
+        "inputs": {
+            "text_positive": "",
+            "text_negative": "",
+            "style": "Fooocus Negative",
+            "log_prompt": True,
+            "style_positive": True,
+            "style_negative": True
+        },
+        "class_type": "SDXLPromptStyler",
+        "_meta": {
+            "title": "SDXL Prompt Styler"
+        }
+    },
+    "133:1": {
+        "inputs": {
+            "text1": [
+                "140",
+                0
+            ],
+            "text2": [
+                "119:0",
+                1
+            ],
+            "separator": ", "
+        },
+        "class_type": "CR Text Concatenate",
+        "_meta": {
+            "title": "🔤 CR Text Concatenate"
+        }
+    },
+    "133:2": {
+        "inputs": {
+            "text1": [
+                "119:1",
+                0
+            ],
+            "text2": [
+                "119:2",
+                0
+            ],
+            "separator": ", "
+        },
+        "class_type": "CR Text Concatenate",
+        "_meta": {
+            "title": "🔤 CR Text Concatenate"
+        }
+    },
+    "133:3": {
+        "inputs": {
+            "text1": [
+                "119:1",
+                1
+            ],
+            "text2": [
+                "119:2",
+                1
+            ],
+            "separator": ", "
+        },
+        "class_type": "CR Text Concatenate",
+        "_meta": {
+            "title": "🔤 CR Text Concatenate"
+        }
+    },
+    "133:0": {
+        "inputs": {
+            "text1": [
+                "139",
+                0
+            ],
+            "text2": [
+                "119:0",
+                0
+            ],
+            "separator": ", "
+        },
+        "class_type": "CR Text Concatenate",
+        "_meta": {
+            "title": "🔤 CR Text Concatenate"
+        }
+    },
+    "114:1": {
+        "inputs": {
+            "text1": [
+                "133:1",
+                0
+            ],
+            "text2": [
+                "133:3",
+                0
+            ],
+            "separator": ", "
+        },
+        "class_type": "CR Text Concatenate",
+        "_meta": {
+            "title": "🔤 CR Text Concatenate"
+        }
+    },
+    "114:0": {
+        "inputs": {
+            "text1": [
+                "133:0",
+                0
+            ],
+            "text2": [
+                "133:2",
+                0
+            ],
+            "separator": ", "
+        },
+        "class_type": "CR Text Concatenate",
+        "_meta": {
+            "title": "🔤 CR Text Concatenate"
+        }
+    },
+    "138:0": {
+        "inputs": {
+            "text": [
+                "102",
+                0
+            ],
+            "clip": [
+                "135",
+                1
+            ]
+        },
+        "class_type": "CLIPTextEncode",
+        "_meta": {
+            "title": "CLIP Text Encode (Prompt)"
+        }
+    },
+    "138:1": {
+        "inputs": {
+            "text": [
+                "101",
+                0
+            ],
+            "clip": [
+                "135",
+                1
+            ]
+        },
+        "class_type": "CLIPTextEncode",
+        "_meta": {
+            "title": "CLIP Text Encode (Prompt)"
+        }
     }
-  },
-  "138:1": {
-    "inputs": {
-      "text": [
-        "101",
-        0
-      ],
-      "clip": [
-        "135",
-        1
-      ]
-    },
-    "class_type": "CLIPTextEncode",
-    "_meta": {
-      "title": "CLIP Text Encode (Prompt)"
+}
+
+model_load_json = {
+    "1": {
+        "inputs": {
+            "ckpt_name": "Juggernaut-XI-Prototype.safetensors",
+            "key_opt": "",
+            "mode": "Auto"
+        },
+        "class_type": "CheckpointLoaderSimpleShared //Inspire",
+        "_meta": {
+            "title": "Shared Checkpoint Loader (Inspire)"
+        }
+    },
+    "3": {
+        "inputs": {
+            "text": "",
+            "clip": [
+                "1",
+                1
+            ]
+        },
+        "class_type": "CLIPTextEncode",
+        "_meta": {
+            "title": "CLIP Text Encode (Prompt)"
+        }
+    },
+    "4": {
+        "inputs": {
+            "root_dir": "output",
+            "file": "file.txt",
+            "append": "append",
+            "insert": True,
+            "text": [
+                "10",
+                2
+            ]
+        },
+        "class_type": "SaveText|pysssss",
+        "_meta": {
+            "title": "Save Text 🐍"
+        }
+    },
+    "10": {
+        "inputs": {
+            "latent_suffix": "6934042_cache",
+            "image_suffix": "8568828_cache",
+            "conditioning_suffix": "91602225_cache",
+            "output_path": "/opt/rd/apps/ComfyUI/custom_nodes/was-node-suite-comfyui/cache",
+            "conditioning": [
+                "3",
+                0
+            ]
+        },
+        "class_type": "Cache Node",
+        "_meta": {
+            "title": "Cache Node"
+        }
     }
-  }
 }
 
 
 class CmfyWorkflow(BaseRequest):
     workflow_json: str = Field("", examples=[json.dumps(default_workflow_json)])
```

### Comparing `gen_wrappers-0.4.0/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.4.1/creator/fcus_api/creator_fcus_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import httpx
 import requests
 
 from creator.base.base_app import BaseApp
 from creator.base.base_request import BaseRequest
 from creator.base.base_response import BaseResponse, ResponseDataType, ResponseData
+from creator.base.job_status import JobStatus
 from creator.fcus_api.request_fcus_api import FcusTxt2Img, FcusUpscaleOrVary, FcusInpaintOrOutpaint
 from creator.fcus_api.response_fcus_api import ResponseFcusApi
 
 logger = logging.getLogger(__name__)
 
 
 class AppFcusApi(BaseApp):
@@ -130,8 +131,17 @@
             status = response_json.get('job_status')
             logger.debug(f"Status: {status}")
             if status is None:
                 return None
             if status != "Finished":
                 return []
             outputs = [result.get('base64') for result in response_json.get('job_result', []) if result.get('finish_reason', "UNKNOWN") == "SUCCESS"]
-            return outputs
+            return outputs
+
+    async def cache_model(self, model: str) -> bool:
+        # FCUS_API doesn't have a specific endpoint for caching models, so we just
+        # Run a txt2img job with a very low resolution to load the model
+        request = FcusTxt2Img(prompt="a", negative_prompt="b", image_number=1, base_model_name=model, aspect_ratio_slection="64*64")
+        response = await self.create(request)
+        if response.status == JobStatus.FINISHED:
+            return True
+        return False
```

### Comparing `gen_wrappers-0.4.0/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.4.1/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.0/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.4.1/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.0/creator/util/helper.py` & `gen_wrappers-0.4.1/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.0/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gen-wrappers
-Version: 0.4.0
+Name: gen_wrappers
+Version: 0.4.1
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.0/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.4.1/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.0/setup.py` & `gen_wrappers-0.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.4.0',
+    version='0.4.1',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```


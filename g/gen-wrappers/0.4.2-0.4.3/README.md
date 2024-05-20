# Comparing `tmp/gen_wrappers-0.4.2.tar.gz` & `tmp/gen_wrappers-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.4.2.tar", last modified: Mon May 20 15:23:43 2024, max compression
+gzip compressed data, was "gen_wrappers-0.4.3.tar", last modified: Mon May 20 16:15:29 2024, max compression
```

## Comparing `gen_wrappers-0.4.2.tar` & `gen_wrappers-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.189585 gen_wrappers-0.4.2/
--rw-rw-rw-   0        0        0      847 2024-05-20 15:23:43.188217 gen_wrappers-0.4.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 15:23:42.771813 gen_wrappers-0.4.2/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.2/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 15:23:42.843507 gen_wrappers-0.4.2/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.2/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     7135 2024-05-20 15:04:33.000000 gen_wrappers-0.4.2/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.2/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.2/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-20 15:23:42.934893 gen_wrappers-0.4.2/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.2/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1582 2024-05-20 14:12:32.000000 gen_wrappers-0.4.2/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.4.2/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.2/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.2/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.013774 gen_wrappers-0.4.2/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.2/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9850 2024-05-20 15:04:33.000000 gen_wrappers-0.4.2/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    16238 2024-05-20 14:12:32.000000 gen_wrappers-0.4.2/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.2/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.108579 gen_wrappers-0.4.2/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.2/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6853 2024-05-20 15:04:33.000000 gen_wrappers-0.4.2/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.4.2/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.2/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.115508 gen_wrappers-0.4.2/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.2/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.2/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-20 15:23:43.184884 gen_wrappers-0.4.2/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 15:23:42.000000 gen_wrappers-0.4.2/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 15:23:43.190603 gen_wrappers-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-20 15:07:41.000000 gen_wrappers-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:29.597216 gen_wrappers-0.4.3/
+-rw-rw-rw-   0        0        0      847 2024-05-20 16:15:29.594937 gen_wrappers-0.4.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:29.500147 gen_wrappers-0.4.3/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.3/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:29.519339 gen_wrappers-0.4.3/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.3/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     7129 2024-05-20 16:09:49.000000 gen_wrappers-0.4.3/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.3/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.3/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:29.530876 gen_wrappers-0.4.3/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.3/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1582 2024-05-20 14:12:32.000000 gen_wrappers-0.4.3/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.4.3/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.3/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.3/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:29.541203 gen_wrappers-0.4.3/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.3/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9870 2024-05-20 16:15:03.000000 gen_wrappers-0.4.3/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    16238 2024-05-20 14:12:32.000000 gen_wrappers-0.4.3/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.3/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:29.550701 gen_wrappers-0.4.3/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.3/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6876 2024-05-20 16:13:18.000000 gen_wrappers-0.4.3/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.4.3/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.3/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:29.555235 gen_wrappers-0.4.3/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.3/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.3/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:29.590416 gen_wrappers-0.4.3/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-20 16:15:29.000000 gen_wrappers-0.4.3/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-20 16:15:29.000000 gen_wrappers-0.4.3/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 16:15:29.000000 gen_wrappers-0.4.3/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-20 16:15:29.000000 gen_wrappers-0.4.3/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 16:15:29.000000 gen_wrappers-0.4.3/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 16:15:29.598225 gen_wrappers-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-20 16:15:03.000000 gen_wrappers-0.4.3/setup.py
```

### Comparing `gen_wrappers-0.4.2/PKG-INFO` & `gen_wrappers-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.4.2
+Version: 0.4.3
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.2/creator/auto/creator_auto.py` & `gen_wrappers-0.4.3/creator/auto/creator_auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def __init__(self):
         super().__init__()
         auto_port = os.environ.get("PORT_AUTO", 8081)
         if isinstance(auto_port, str):
             auto_port = int(auto_port)
         self.jobs = {}
         self.output = {}
-        self.api_base_url = f"http://0.0.0.0:{auto_port}/sdapi"
+        self.api_base_url = f"http://0.0.0.0:{auto_port}"
         app_config_path = "/opt/rd/apps/stable-diffusion-webui/config.json"
         if os.path.exists(app_config_path):
             with open(app_config_path, "r") as f:
                 app_config = json.load(f)
                 default_checkpoint = app_config.get("sd_model_checkpoint", None)
                 if default_checkpoint:
                     self.loaded_models.append(default_checkpoint)
```

### Comparing `gen_wrappers-0.4.2/creator/auto/request_auto.py` & `gen_wrappers-0.4.3/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/creator/auto/response_auto.py` & `gen_wrappers-0.4.3/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/creator/base/base_app.py` & `gen_wrappers-0.4.3/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/creator/base/base_request.py` & `gen_wrappers-0.4.3/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/creator/base/base_response.py` & `gen_wrappers-0.4.3/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.4.3/creator/cmfy/creator_cmfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         max_cached_models = os.environ.get("MAX_CACHED_MODELS", 3)
         if len(self.loaded_models) > max_cached_models:
             self.loaded_models = self.loaded_models[-max_cached_models:]
 
     async def cache_model(self, model: str = "Juggernaut-XI-Prototype.safetensors") -> bool:
         request_json = model_load_json
         request_json["1"]['inputs']['ckpt_name'] = model
-        request = CmfyWorkflow(workflow_json=json.dumps(request_json))
+        request = CmfyWorkflow()
+        request.workflow_json = json.dumps(request_json)
         self._check_loaded_model(request_json)
         response = await self.create(request)
         if response.status == JobStatus.FINISHED:
             return True
         return False
```

### Comparing `gen_wrappers-0.4.2/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.4.3/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.4.3/creator/fcus_api/creator_fcus_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -136,12 +136,15 @@
                 return []
             outputs = [result.get('base64') for result in response_json.get('job_result', []) if result.get('finish_reason', "UNKNOWN") == "SUCCESS"]
             return outputs
 
     async def cache_model(self, model: str = "Juggernaut-XI-Prototype.safetensors") -> bool:
         # FCUS_API doesn't have a specific endpoint for caching models, so we just
         # Run a txt2img job with a very low resolution to load the model
-        request = FcusTxt2Img(prompt="a", negative_prompt="b", image_number=1, base_model_name=model, aspect_ratio_slection="64*64")
+        request = FcusTxt2Img()
+        request.prompt = "foo"
+        request.base_model_name = model
+        request.aspect_ratios_selection = "64*64"
         response = await self.create(request)
         if response.status == JobStatus.FINISHED:
             return True
         return False
```

### Comparing `gen_wrappers-0.4.2/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.4.3/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.4.3/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/creator/util/helper.py` & `gen_wrappers-0.4.3/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.4.3/gen_wrappers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.4.2
+Version: 0.4.3
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.2/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.4.3/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.2/setup.py` & `gen_wrappers-0.4.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.4.2',
+    version='0.4.3',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```


# Comparing `tmp/gen_wrappers-0.4.4.tar.gz` & `tmp/gen_wrappers-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.4.4.tar", last modified: Mon May 20 16:21:14 2024, max compression
+gzip compressed data, was "gen_wrappers-0.4.5.tar", last modified: Mon May 20 16:37:33 2024, max compression
```

## Comparing `gen_wrappers-0.4.4.tar` & `gen_wrappers-0.4.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 16:21:14.386284 gen_wrappers-0.4.4/
--rw-rw-rw-   0        0        0      847 2024-05-20 16:21:14.384280 gen_wrappers-0.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 16:21:14.353680 gen_wrappers-0.4.4/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.4/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:21:14.357681 gen_wrappers-0.4.4/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.4/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     7129 2024-05-20 16:09:49.000000 gen_wrappers-0.4.4/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.4/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.4/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:21:14.361679 gen_wrappers-0.4.4/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.4/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1582 2024-05-20 14:12:32.000000 gen_wrappers-0.4.4/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.4.4/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.4/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.4/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:21:14.365679 gen_wrappers-0.4.4/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.4/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9880 2024-05-20 16:20:28.000000 gen_wrappers-0.4.4/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    16238 2024-05-20 14:12:32.000000 gen_wrappers-0.4.4/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.4/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:21:14.368679 gen_wrappers-0.4.4/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.4/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6886 2024-05-20 16:20:28.000000 gen_wrappers-0.4.4/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.4.4/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.4/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:21:14.370275 gen_wrappers-0.4.4/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.4/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.4/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:21:14.383280 gen_wrappers-0.4.4/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-20 16:21:14.000000 gen_wrappers-0.4.4/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-20 16:21:14.000000 gen_wrappers-0.4.4/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 16:21:14.000000 gen_wrappers-0.4.4/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-20 16:21:14.000000 gen_wrappers-0.4.4/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 16:21:14.000000 gen_wrappers-0.4.4/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 16:21:14.386284 gen_wrappers-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-20 16:20:39.000000 gen_wrappers-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:37:33.904981 gen_wrappers-0.4.5/
+-rw-rw-rw-   0        0        0      847 2024-05-20 16:37:33.903959 gen_wrappers-0.4.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 16:37:33.870868 gen_wrappers-0.4.5/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.5/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:37:33.874868 gen_wrappers-0.4.5/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.5/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     7040 2024-05-20 16:27:37.000000 gen_wrappers-0.4.5/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.5/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.5/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:37:33.879868 gen_wrappers-0.4.5/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.5/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1582 2024-05-20 14:12:32.000000 gen_wrappers-0.4.5/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      466 2024-05-20 16:37:31.000000 gen_wrappers-0.4.5/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.5/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.5/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:37:33.885311 gen_wrappers-0.4.5/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.5/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9880 2024-05-20 16:20:28.000000 gen_wrappers-0.4.5/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    16238 2024-05-20 14:12:32.000000 gen_wrappers-0.4.5/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.5/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:37:33.888969 gen_wrappers-0.4.5/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.5/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6886 2024-05-20 16:20:28.000000 gen_wrappers-0.4.5/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3934 2024-05-20 16:34:32.000000 gen_wrappers-0.4.5/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.5/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:37:33.890574 gen_wrappers-0.4.5/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.5/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.5/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:37:33.902962 gen_wrappers-0.4.5/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-20 16:37:33.000000 gen_wrappers-0.4.5/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-20 16:37:33.000000 gen_wrappers-0.4.5/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 16:37:33.000000 gen_wrappers-0.4.5/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-20 16:37:33.000000 gen_wrappers-0.4.5/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 16:37:33.000000 gen_wrappers-0.4.5/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 16:37:33.905960 gen_wrappers-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-20 16:37:31.000000 gen_wrappers-0.4.5/setup.py
```

### Comparing `gen_wrappers-0.4.4/PKG-INFO` & `gen_wrappers-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.4.4
+Version: 0.4.5
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.4/creator/auto/creator_auto.py` & `gen_wrappers-0.4.5/creator/auto/creator_auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,14 @@
         }
         if model not in self.loaded_models:
             self.loaded_models.append(model)
         if len(self.loaded_models) > 3:
             self.loaded_models.pop(0)
         url = f"{self.api_base_url}/sdapi/v1/options"
         headers = {'Content-Type': 'application/json'}
-        async with httpx.AsyncClient() as client:
-            response = await client.post(url, json=request, headers=headers)
+        async with httpx.AsyncClient(timeout=300) as client:
+            response = await client.post(url, json=request, headers=headers, timeout=300)
             response.raise_for_status()
             if response.status_code == 200:
-                # Sleep for 15 seconds to allow the model to be cached
-                await asyncio.sleep(15)
                 return True
             print(f"Error caching model: {response.text}")
         return False
```

### Comparing `gen_wrappers-0.4.4/creator/auto/request_auto.py` & `gen_wrappers-0.4.5/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/creator/auto/response_auto.py` & `gen_wrappers-0.4.5/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/creator/base/base_app.py` & `gen_wrappers-0.4.5/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/creator/base/base_response.py` & `gen_wrappers-0.4.5/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.4.5/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.4.5/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.4.5/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.4.5/creator/fcus_api/request_fcus_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
     model_name: str = ""
     weight: float = 1.0
 
 
 class FcusTxt2Img(BaseRequest):
     prompt: str = ""
     negative_prompt: str = ""
-    style_selections: List[str] = Field(default_factory=list,
-                                        examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
+    style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = "Speed"
     aspect_ratios_selection: str = "1152*896"
     image_number: int = 2
     image_seed: int = -1
     sharpness: float = 0.0
     guidance_scale: float = 7.5
     base_model_name: str = "Juggernaut-XI-Prototype.safetensors"
```

### Comparing `gen_wrappers-0.4.4/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.4.5/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/creator/util/helper.py` & `gen_wrappers-0.4.5/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.4.5/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.4.4
+Version: 0.4.5
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.4.4/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.4.5/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.4.4/setup.py` & `gen_wrappers-0.4.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.4.4',
+    version='0.4.5',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```


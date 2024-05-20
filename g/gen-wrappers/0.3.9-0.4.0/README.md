# Comparing `tmp/gen_wrappers-0.3.9.tar.gz` & `tmp/gen_wrappers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.3.9.tar", last modified: Tue May 14 17:32:08 2024, max compression
+gzip compressed data, was "gen_wrappers-0.4.0.tar", last modified: Sun May 19 17:58:41 2024, max compression
```

## Comparing `gen_wrappers-0.3.9.tar` & `gen_wrappers-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:32:08.506346 gen_wrappers-0.3.9/
--rw-rw-rw-   0        0        0      847 2024-05-14 17:32:08.500909 gen_wrappers-0.3.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 17:32:08.407824 gen_wrappers-0.3.9/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.9/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:32:08.426247 gen_wrappers-0.3.9/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.9/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5302 2024-05-14 15:42:23.000000 gen_wrappers-0.3.9/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.3.9/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.9/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:32:08.437801 gen_wrappers-0.3.9/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.9/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1491 2024-05-14 15:42:23.000000 gen_wrappers-0.3.9/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.9/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.9/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.9/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:32:08.445728 gen_wrappers-0.3.9/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.9/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9421 2024-05-14 17:31:43.000000 gen_wrappers-0.3.9/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0    10342 2024-05-14 17:06:38.000000 gen_wrappers-0.3.9/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.9/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:32:08.453655 gen_wrappers-0.3.9/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.9/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6273 2024-05-14 15:42:23.000000 gen_wrappers-0.3.9/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.9/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.9/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:32:08.457654 gen_wrappers-0.3.9/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.9/creator/util/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.3.9/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:32:08.497816 gen_wrappers-0.3.9/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-14 17:32:08.000000 gen_wrappers-0.3.9/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-14 17:32:08.000000 gen_wrappers-0.3.9/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:32:08.000000 gen_wrappers-0.3.9/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-14 17:32:08.000000 gen_wrappers-0.3.9/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-14 17:32:08.000000 gen_wrappers-0.3.9/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 17:32:08.507717 gen_wrappers-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-14 17:31:59.000000 gen_wrappers-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:58:41.149246 gen_wrappers-0.4.0/
+-rw-rw-rw-   0        0        0      847 2024-05-19 17:58:41.147246 gen_wrappers-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 17:58:40.807706 gen_wrappers-0.4.0/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.4.0/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:58:40.875093 gen_wrappers-0.4.0/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.4.0/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5302 2024-05-14 15:42:23.000000 gen_wrappers-0.4.0/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4055 2024-05-14 16:10:12.000000 gen_wrappers-0.4.0/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.4.0/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:58:40.943376 gen_wrappers-0.4.0/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.4.0/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1491 2024-05-14 15:42:23.000000 gen_wrappers-0.4.0/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.4.0/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.4.0/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.4.0/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:58:40.986465 gen_wrappers-0.4.0/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.4.0/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9355 2024-05-17 02:24:46.000000 gen_wrappers-0.4.0/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0    12644 2024-05-19 17:58:23.000000 gen_wrappers-0.4.0/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.4.0/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:58:41.052863 gen_wrappers-0.4.0/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.4.0/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6273 2024-05-14 15:42:23.000000 gen_wrappers-0.4.0/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.4.0/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.4.0/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:58:41.073847 gen_wrappers-0.4.0/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.4.0/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     5073 2024-05-14 13:53:25.000000 gen_wrappers-0.4.0/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:58:41.143798 gen_wrappers-0.4.0/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 17:58:40.000000 gen_wrappers-0.4.0/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:58:41.149246 gen_wrappers-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-19 17:58:23.000000 gen_wrappers-0.4.0/setup.py
```

### Comparing `gen_wrappers-0.3.9/PKG-INFO` & `gen_wrappers-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.3.9
+Version: 0.4.0
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.9/creator/auto/creator_auto.py` & `gen_wrappers-0.4.0/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/auto/request_auto.py` & `gen_wrappers-0.4.0/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/auto/response_auto.py` & `gen_wrappers-0.4.0/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/base/base_app.py` & `gen_wrappers-0.4.0/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/base/base_request.py` & `gen_wrappers-0.4.0/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/base/base_response.py` & `gen_wrappers-0.4.0/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.4.0/creator/cmfy/creator_cmfy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import asyncio
 import base64
-import dataclasses
 import json
 import logging
 import os
 import urllib
 import urllib.parse
 import urllib.request
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 import requests
 
 from creator.base.base_app import BaseApp
-from creator.base.base_request import BaseRequest
 from creator.base.base_response import ResponseDataType, ResponseData, BaseResponse
 from creator.base.job_status import JobStatus
 from creator.cmfy.request_cmfy import CmfyWorkflow, CmfyWorkflowFcus
 from creator.cmfy.response_cmfy import ResponseCmfy
 
 logger = logging.getLogger(__name__)
 
@@ -128,15 +126,15 @@
                     logger.debug(f"Getting image: {image['filename']}")
                     print(f"Getting image: {image['filename']}")
                     image_data = await self._get_image(image['filename'], image['subfolder'], image['type'])
                     images_output.append(image_data)
                 print(f"We are returning {len(images_output)} images")
                 response_data = ResponseData(data=images_output, data_type=ResponseDataType.IMAGE,
                                              total_count=len(images_output))
-                return ResponseCmfy.success(response_data)
+                return ResponseCmfy.success(data=response_data)
         response = ResponseCmfy.running(job_id)
         return response
 
     async def get_models(self) -> List[Any]:
         url = f"http://localhost:{os.environ.get('PORT_CMFY', 8889)}/object_info"
         async with httpx.AsyncClient() as client:
             response = await client.get(url)
```

### Comparing `gen_wrappers-0.3.9/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.4.0/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.4.0/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.4.0/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/creator/util/helper.py` & `gen_wrappers-0.4.0/creator/util/helper.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.4.0/gen_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.3.9
+Version: 0.4.0
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.3.9/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.4.0/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.3.9/setup.py` & `gen_wrappers-0.4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.3.9',
+    version='0.4.0',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```


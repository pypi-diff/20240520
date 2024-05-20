# Comparing `tmp/alibabacloud_tingwu20230930-2.0.8.tar.gz` & `tmp/alibabacloud_tingwu20230930-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tingwu20230930-2.0.8.tar", last modified: Fri Apr 12 03:56:08 2024, max compression
+gzip compressed data, was "dist/alibabacloud_tingwu20230930-2.0.9.tar", last modified: Wed May 15 03:20:20 2024, max compression
```

## Comparing `alibabacloud_tingwu20230930-2.0.8.tar` & `alibabacloud_tingwu20230930-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:56:08.000000 alibabacloud_tingwu20230930-2.0.8/
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2422 2024-04-12 03:56:08.000000 alibabacloud_tingwu20230930-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1107 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1192 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:56:08.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21480 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930/client.py
--rw-r--r--   0 root         (0) root         (0)    53934 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:56:08.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2422 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 03:56:08.000000 alibabacloud_tingwu20230930-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2626 2024-04-12 03:56:07.000000 alibabacloud_tingwu20230930-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1107 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1192 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26852 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)    57345 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-05-15 03:20:20.000000 alibabacloud_tingwu20230930-2.0.9/setup.py
```

### Comparing `alibabacloud_tingwu20230930-2.0.8/ChangeLog.md` & `alibabacloud_tingwu20230930-2.0.9/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-12 Version: 2.0.8
+- Update API GetTaskInfo: update response param.
+
+
 2024-04-10 Version: 2.0.7
 - Update API GetTaskInfo: update response param.
 
 
 2024-03-18 Version: 2.0.6
 - Update API CreateTask: update param body.
 - Update API CreateTask: update response param.
```

### Comparing `alibabacloud_tingwu20230930-2.0.8/LICENSE` & `alibabacloud_tingwu20230930-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930-2.0.8/PKG-INFO` & `alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_tingwu20230930
-Version: 2.0.8
+Name: alibabacloud-tingwu20230930
+Version: 2.0.9
 Summary: Alibaba Cloud tingwu (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tingwu20230930-2.0.8/README-CN.md` & `alibabacloud_tingwu20230930-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930-2.0.8/README.md` & `alibabacloud_tingwu20230930-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930/client.py` & `alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,14 +43,22 @@
 
     def create_task_with_options(
         self,
         request: tingwu_20230930_models.CreateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.CreateTaskResponse:
+        """
+        @summary 创建听悟任务
+        
+        @param request: CreateTaskRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.operation):
             query['operation'] = request.operation
         if not UtilClient.is_unset(request.type):
             query['type'] = request.type
         body = {}
@@ -83,14 +91,22 @@
 
     async def create_task_with_options_async(
         self,
         request: tingwu_20230930_models.CreateTaskRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.CreateTaskResponse:
+        """
+        @summary 创建听悟任务
+        
+        @param request: CreateTaskRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.operation):
             query['operation'] = request.operation
         if not UtilClient.is_unset(request.type):
             query['type'] = request.type
         body = {}
@@ -121,32 +137,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_task(
         self,
         request: tingwu_20230930_models.CreateTaskRequest,
     ) -> tingwu_20230930_models.CreateTaskResponse:
+        """
+        @summary 创建听悟任务
+        
+        @param request: CreateTaskRequest
+        @return: CreateTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_task_with_options(request, headers, runtime)
 
     async def create_task_async(
         self,
         request: tingwu_20230930_models.CreateTaskRequest,
     ) -> tingwu_20230930_models.CreateTaskResponse:
+        """
+        @summary 创建听悟任务
+        
+        @param request: CreateTaskRequest
+        @return: CreateTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_task_with_options_async(request, headers, runtime)
 
     def create_transcription_phrases_with_options(
         self,
         request: tingwu_20230930_models.CreateTranscriptionPhrasesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.CreateTranscriptionPhrasesResponse:
+        """
+        @summary 创建热词词表
+        
+        @param request: CreateTranscriptionPhrasesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTranscriptionPhrasesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.word_weights):
@@ -173,14 +209,22 @@
 
     async def create_transcription_phrases_with_options_async(
         self,
         request: tingwu_20230930_models.CreateTranscriptionPhrasesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.CreateTranscriptionPhrasesResponse:
+        """
+        @summary 创建热词词表
+        
+        @param request: CreateTranscriptionPhrasesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTranscriptionPhrasesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.word_weights):
@@ -205,32 +249,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_transcription_phrases(
         self,
         request: tingwu_20230930_models.CreateTranscriptionPhrasesRequest,
     ) -> tingwu_20230930_models.CreateTranscriptionPhrasesResponse:
+        """
+        @summary 创建热词词表
+        
+        @param request: CreateTranscriptionPhrasesRequest
+        @return: CreateTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_transcription_phrases_with_options(request, headers, runtime)
 
     async def create_transcription_phrases_async(
         self,
         request: tingwu_20230930_models.CreateTranscriptionPhrasesRequest,
     ) -> tingwu_20230930_models.CreateTranscriptionPhrasesResponse:
+        """
+        @summary 创建热词词表
+        
+        @param request: CreateTranscriptionPhrasesRequest
+        @return: CreateTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_transcription_phrases_with_options_async(request, headers, runtime)
 
     def delete_transcription_phrases_with_options(
         self,
         phrase_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.DeleteTranscriptionPhrasesResponse:
+        """
+        @summary 删除词表
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTranscriptionPhrasesResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteTranscriptionPhrases',
             version='2023-09-30',
             protocol='HTTPS',
@@ -248,14 +311,21 @@
 
     async def delete_transcription_phrases_with_options_async(
         self,
         phrase_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.DeleteTranscriptionPhrasesResponse:
+        """
+        @summary 删除词表
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTranscriptionPhrasesResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='DeleteTranscriptionPhrases',
             version='2023-09-30',
             protocol='HTTPS',
@@ -271,32 +341,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_transcription_phrases(
         self,
         phrase_id: str,
     ) -> tingwu_20230930_models.DeleteTranscriptionPhrasesResponse:
+        """
+        @summary 删除词表
+        
+        @return: DeleteTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.delete_transcription_phrases_with_options(phrase_id, headers, runtime)
 
     async def delete_transcription_phrases_async(
         self,
         phrase_id: str,
     ) -> tingwu_20230930_models.DeleteTranscriptionPhrasesResponse:
+        """
+        @summary 删除词表
+        
+        @return: DeleteTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_transcription_phrases_with_options_async(phrase_id, headers, runtime)
 
     def get_task_info_with_options(
         self,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.GetTaskInfoResponse:
+        """
+        @summary 查询听悟任务信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskInfoResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskInfo',
             version='2023-09-30',
             protocol='HTTPS',
@@ -314,14 +401,21 @@
 
     async def get_task_info_with_options_async(
         self,
         task_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.GetTaskInfoResponse:
+        """
+        @summary 查询听悟任务信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTaskInfoResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTaskInfo',
             version='2023-09-30',
             protocol='HTTPS',
@@ -337,32 +431,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_task_info(
         self,
         task_id: str,
     ) -> tingwu_20230930_models.GetTaskInfoResponse:
+        """
+        @summary 查询听悟任务信息
+        
+        @return: GetTaskInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_task_info_with_options(task_id, headers, runtime)
 
     async def get_task_info_async(
         self,
         task_id: str,
     ) -> tingwu_20230930_models.GetTaskInfoResponse:
+        """
+        @summary 查询听悟任务信息
+        
+        @return: GetTaskInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_task_info_with_options_async(task_id, headers, runtime)
 
     def get_transcription_phrases_with_options(
         self,
         phrase_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.GetTranscriptionPhrasesResponse:
+        """
+        @summary 查询热词词表信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTranscriptionPhrasesResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTranscriptionPhrases',
             version='2023-09-30',
             protocol='HTTPS',
@@ -380,14 +491,21 @@
 
     async def get_transcription_phrases_with_options_async(
         self,
         phrase_id: str,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.GetTranscriptionPhrasesResponse:
+        """
+        @summary 查询热词词表信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTranscriptionPhrasesResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='GetTranscriptionPhrases',
             version='2023-09-30',
             protocol='HTTPS',
@@ -403,31 +521,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_transcription_phrases(
         self,
         phrase_id: str,
     ) -> tingwu_20230930_models.GetTranscriptionPhrasesResponse:
+        """
+        @summary 查询热词词表信息
+        
+        @return: GetTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_transcription_phrases_with_options(phrase_id, headers, runtime)
 
     async def get_transcription_phrases_async(
         self,
         phrase_id: str,
     ) -> tingwu_20230930_models.GetTranscriptionPhrasesResponse:
+        """
+        @summary 查询热词词表信息
+        
+        @return: GetTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_transcription_phrases_with_options_async(phrase_id, headers, runtime)
 
     def list_transcription_phrases_with_options(
         self,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.ListTranscriptionPhrasesResponse:
+        """
+        @summary 列举用户所有热词词表信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTranscriptionPhrasesResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListTranscriptionPhrases',
             version='2023-09-30',
             protocol='HTTPS',
@@ -444,14 +579,21 @@
         )
 
     async def list_transcription_phrases_with_options_async(
         self,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.ListTranscriptionPhrasesResponse:
+        """
+        @summary 列举用户所有热词词表信息
+        
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTranscriptionPhrasesResponse
+        """
         req = open_api_models.OpenApiRequest(
             headers=headers
         )
         params = open_api_models.Params(
             action='ListTranscriptionPhrases',
             version='2023-09-30',
             protocol='HTTPS',
@@ -464,30 +606,48 @@
         )
         return TeaCore.from_map(
             tingwu_20230930_models.ListTranscriptionPhrasesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_transcription_phrases(self) -> tingwu_20230930_models.ListTranscriptionPhrasesResponse:
+        """
+        @summary 列举用户所有热词词表信息
+        
+        @return: ListTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.list_transcription_phrases_with_options(headers, runtime)
 
     async def list_transcription_phrases_async(self) -> tingwu_20230930_models.ListTranscriptionPhrasesResponse:
+        """
+        @summary 列举用户所有热词词表信息
+        
+        @return: ListTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_transcription_phrases_with_options_async(headers, runtime)
 
     def update_transcription_phrases_with_options(
         self,
         phrase_id: str,
         request: tingwu_20230930_models.UpdateTranscriptionPhrasesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.UpdateTranscriptionPhrasesResponse:
+        """
+        @summary 更新热词词表
+        
+        @param request: UpdateTranscriptionPhrasesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTranscriptionPhrasesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.word_weights):
@@ -515,14 +675,22 @@
     async def update_transcription_phrases_with_options_async(
         self,
         phrase_id: str,
         request: tingwu_20230930_models.UpdateTranscriptionPhrasesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tingwu_20230930_models.UpdateTranscriptionPhrasesResponse:
+        """
+        @summary 更新热词词表
+        
+        @param request: UpdateTranscriptionPhrasesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateTranscriptionPhrasesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.word_weights):
@@ -548,19 +716,31 @@
         )
 
     def update_transcription_phrases(
         self,
         phrase_id: str,
         request: tingwu_20230930_models.UpdateTranscriptionPhrasesRequest,
     ) -> tingwu_20230930_models.UpdateTranscriptionPhrasesResponse:
+        """
+        @summary 更新热词词表
+        
+        @param request: UpdateTranscriptionPhrasesRequest
+        @return: UpdateTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_transcription_phrases_with_options(phrase_id, request, headers, runtime)
 
     async def update_transcription_phrases_async(
         self,
         phrase_id: str,
         request: tingwu_20230930_models.UpdateTranscriptionPhrasesRequest,
     ) -> tingwu_20230930_models.UpdateTranscriptionPhrasesResponse:
+        """
+        @summary 更新热词词表
+        
+        @param request: UpdateTranscriptionPhrasesRequest
+        @return: UpdateTranscriptionPhrasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_transcription_phrases_with_options_async(phrase_id, request, headers, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930/models.py` & `alibabacloud_tingwu20230930-2.0.9/alibabacloud_tingwu20230930/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         task_key: str = None,
     ):
         self.file_url = file_url
         self.format = format
         self.multiple_streams_enabled = multiple_streams_enabled
         self.progressive_callbacks_enabled = progressive_callbacks_enabled
         self.sample_rate = sample_rate
+        # This parameter is required.
         self.source_language = source_language
         self.task_id = task_id
         self.task_key = task_key
 
     def validate(self):
         pass
 
@@ -69,14 +70,96 @@
         if m.get('TaskId') is not None:
             self.task_id = m.get('TaskId')
         if m.get('TaskKey') is not None:
             self.task_key = m.get('TaskKey')
         return self
 
 
+class CreateTaskRequestParametersCustomPromptContents(TeaModel):
+    def __init__(
+        self,
+        model: str = None,
+        name: str = None,
+        prompt: str = None,
+        trans_type: str = None,
+    ):
+        self.model = model
+        # This parameter is required.
+        self.name = name
+        # This parameter is required.
+        self.prompt = prompt
+        self.trans_type = trans_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.model is not None:
+            result['Model'] = self.model
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.prompt is not None:
+            result['Prompt'] = self.prompt
+        if self.trans_type is not None:
+            result['TransType'] = self.trans_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Model') is not None:
+            self.model = m.get('Model')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Prompt') is not None:
+            self.prompt = m.get('Prompt')
+        if m.get('TransType') is not None:
+            self.trans_type = m.get('TransType')
+        return self
+
+
+class CreateTaskRequestParametersCustomPrompt(TeaModel):
+    def __init__(
+        self,
+        contents: List[CreateTaskRequestParametersCustomPromptContents] = None,
+    ):
+        self.contents = contents
+
+    def validate(self):
+        if self.contents:
+            for k in self.contents:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Contents'] = []
+        if self.contents is not None:
+            for k in self.contents:
+                result['Contents'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.contents = []
+        if m.get('Contents') is not None:
+            for k in m.get('Contents'):
+                temp_model = CreateTaskRequestParametersCustomPromptContents()
+                self.contents.append(temp_model.from_map(k))
+        return self
+
+
 class CreateTaskRequestParametersExtraParams(TeaModel):
     def __init__(
         self,
         nfix_enabled: bool = None,
     ):
         self.nfix_enabled = nfix_enabled
 
@@ -324,40 +407,46 @@
         return self
 
 
 class CreateTaskRequestParameters(TeaModel):
     def __init__(
         self,
         auto_chapters_enabled: bool = None,
+        custom_prompt: CreateTaskRequestParametersCustomPrompt = None,
+        custom_prompt_enabled: bool = None,
         extra_params: CreateTaskRequestParametersExtraParams = None,
         meeting_assistance: CreateTaskRequestParametersMeetingAssistance = None,
         meeting_assistance_enabled: bool = None,
         ppt_extraction_enabled: bool = None,
         summarization: CreateTaskRequestParametersSummarization = None,
         summarization_enabled: bool = None,
         text_polish_enabled: bool = None,
         transcoding: CreateTaskRequestParametersTranscoding = None,
         transcription: CreateTaskRequestParametersTranscription = None,
         translation: CreateTaskRequestParametersTranslation = None,
         translation_enabled: bool = None,
     ):
         self.auto_chapters_enabled = auto_chapters_enabled
+        self.custom_prompt = custom_prompt
+        self.custom_prompt_enabled = custom_prompt_enabled
         self.extra_params = extra_params
         self.meeting_assistance = meeting_assistance
         self.meeting_assistance_enabled = meeting_assistance_enabled
         self.ppt_extraction_enabled = ppt_extraction_enabled
         self.summarization = summarization
         self.summarization_enabled = summarization_enabled
         self.text_polish_enabled = text_polish_enabled
         self.transcoding = transcoding
         self.transcription = transcription
         self.translation = translation
         self.translation_enabled = translation_enabled
 
     def validate(self):
+        if self.custom_prompt:
+            self.custom_prompt.validate()
         if self.extra_params:
             self.extra_params.validate()
         if self.meeting_assistance:
             self.meeting_assistance.validate()
         if self.summarization:
             self.summarization.validate()
         if self.transcoding:
@@ -371,14 +460,18 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auto_chapters_enabled is not None:
             result['AutoChaptersEnabled'] = self.auto_chapters_enabled
+        if self.custom_prompt is not None:
+            result['CustomPrompt'] = self.custom_prompt.to_map()
+        if self.custom_prompt_enabled is not None:
+            result['CustomPromptEnabled'] = self.custom_prompt_enabled
         if self.extra_params is not None:
             result['ExtraParams'] = self.extra_params.to_map()
         if self.meeting_assistance is not None:
             result['MeetingAssistance'] = self.meeting_assistance.to_map()
         if self.meeting_assistance_enabled is not None:
             result['MeetingAssistanceEnabled'] = self.meeting_assistance_enabled
         if self.ppt_extraction_enabled is not None:
@@ -399,14 +492,19 @@
             result['TranslationEnabled'] = self.translation_enabled
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AutoChaptersEnabled') is not None:
             self.auto_chapters_enabled = m.get('AutoChaptersEnabled')
+        if m.get('CustomPrompt') is not None:
+            temp_model = CreateTaskRequestParametersCustomPrompt()
+            self.custom_prompt = temp_model.from_map(m['CustomPrompt'])
+        if m.get('CustomPromptEnabled') is not None:
+            self.custom_prompt_enabled = m.get('CustomPromptEnabled')
         if m.get('ExtraParams') is not None:
             temp_model = CreateTaskRequestParametersExtraParams()
             self.extra_params = temp_model.from_map(m['ExtraParams'])
         if m.get('MeetingAssistance') is not None:
             temp_model = CreateTaskRequestParametersMeetingAssistance()
             self.meeting_assistance = temp_model.from_map(m['MeetingAssistance'])
         if m.get('MeetingAssistanceEnabled') is not None:
@@ -443,14 +541,15 @@
         operation: str = None,
         type: str = None,
     ):
         self.app_key = app_key
         self.input = input
         self.parameters = parameters
         self.operation = operation
+        # This parameter is required.
         self.type = type
 
     def validate(self):
         if self.input:
             self.input.validate()
         if self.parameters:
             self.parameters.validate()
@@ -627,15 +726,17 @@
     def __init__(
         self,
         description: str = None,
         name: str = None,
         word_weights: str = None,
     ):
         self.description = description
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.word_weights = word_weights
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1482,15 +1583,17 @@
     def __init__(
         self,
         description: str = None,
         name: str = None,
         word_weights: str = None,
     ):
         self.description = description
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.word_weights = word_weights
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_tingwu20230930-2.0.8/alibabacloud_tingwu20230930.egg-info/PKG-INFO` & `alibabacloud_tingwu20230930-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-tingwu20230930
-Version: 2.0.8
+Name: alibabacloud_tingwu20230930
+Version: 2.0.9
 Summary: Alibaba Cloud tingwu (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tingwu20230930-2.0.8/setup.py` & `alibabacloud_tingwu20230930-2.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_tingwu20230930.
 
-Created on 12/04/2024
+Created on 15/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_tingwu20230930"
 NAME = "alibabacloud_tingwu20230930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud tingwu (20230930) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```


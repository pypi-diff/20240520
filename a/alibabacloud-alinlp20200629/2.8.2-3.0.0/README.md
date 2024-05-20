# Comparing `tmp/alibabacloud_alinlp20200629-2.8.2.tar.gz` & `tmp/alibabacloud_alinlp20200629-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alinlp20200629-2.8.2.tar", last modified: Wed Apr 10 07:17:17 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alinlp20200629-3.0.0.tar", last modified: Mon May 20 08:01:56 2024, max compression
```

## Comparing `alibabacloud_alinlp20200629-2.8.2.tar` & `alibabacloud_alinlp20200629-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2422 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1107 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1192 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629/__init__.py
--rw-r--r--   0 root         (0) root         (0)   218326 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629/client.py
--rw-r--r--   0 root         (0) root         (0)   249323 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2422 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2626 2024-04-10 07:17:17.000000 alibabacloud_alinlp20200629-2.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1107 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1192 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   266086 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629/client.py
+-rw-r--r--   0 root         (0) root         (0)   256331 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-05-20 08:01:56.000000 alibabacloud_alinlp20200629-3.0.0/setup.py
```

### Comparing `alibabacloud_alinlp20200629-2.8.2/ChangeLog.md` & `alibabacloud_alinlp20200629-3.0.0/ChangeLog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-10 Version: 2.8.2
+- Generated python 2020-06-29 for alinlp.
+
 2024-04-10 Version: 2.8.1
 - Update API PostMSSearchEnhance: add param MinScore.
 
 
 2024-03-29 Version: 2.8.0
 - Support API PostMSServiceDataImport.
```

### Comparing `alibabacloud_alinlp20200629-2.8.2/LICENSE` & `alibabacloud_alinlp20200629-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629-2.8.2/PKG-INFO` & `alibabacloud_alinlp20200629-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alinlp20200629
-Version: 2.8.2
+Version: 3.0.0
 Summary: Alibaba Cloud alinlp (20200629) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alinlp20200629-2.8.2/README-CN.md` & `alibabacloud_alinlp20200629-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629-2.8.2/README.md` & `alibabacloud_alinlp20200629-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629/client.py` & `alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,14 +42,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def a_dclock_with_options(
         self,
         request: alinlp_20200629_models.ADClockRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ADClockResponse:
+        """
+        @summary ad画钟算法处理算法
+        
+        @param request: ADClockRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ADClockResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -72,14 +79,21 @@
         )
 
     async def a_dclock_with_options_async(
         self,
         request: alinlp_20200629_models.ADClockRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ADClockResponse:
+        """
+        @summary ad画钟算法处理算法
+        
+        @param request: ADClockRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ADClockResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -101,29 +115,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def a_dclock(
         self,
         request: alinlp_20200629_models.ADClockRequest,
     ) -> alinlp_20200629_models.ADClockResponse:
+        """
+        @summary ad画钟算法处理算法
+        
+        @param request: ADClockRequest
+        @return: ADClockResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.a_dclock_with_options(request, runtime)
 
     async def a_dclock_async(
         self,
         request: alinlp_20200629_models.ADClockRequest,
     ) -> alinlp_20200629_models.ADClockResponse:
+        """
+        @summary ad画钟算法处理算法
+        
+        @param request: ADClockRequest
+        @return: ADClockResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.a_dclock_with_options_async(request, runtime)
 
     def a_dmmuwith_options(
         self,
         request: alinlp_20200629_models.ADMMURequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ADMMUResponse:
+        """
+        @summary ad语音处理算法
+        
+        @param request: ADMMURequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ADMMUResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -146,14 +179,21 @@
         )
 
     async def a_dmmuwith_options_async(
         self,
         request: alinlp_20200629_models.ADMMURequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ADMMUResponse:
+        """
+        @summary ad语音处理算法
+        
+        @param request: ADMMURequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ADMMUResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -175,29 +215,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def a_dmmu(
         self,
         request: alinlp_20200629_models.ADMMURequest,
     ) -> alinlp_20200629_models.ADMMUResponse:
+        """
+        @summary ad语音处理算法
+        
+        @param request: ADMMURequest
+        @return: ADMMUResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.a_dmmuwith_options(request, runtime)
 
     async def a_dmmu_async(
         self,
         request: alinlp_20200629_models.ADMMURequest,
     ) -> alinlp_20200629_models.ADMMUResponse:
+        """
+        @summary ad语音处理算法
+        
+        @param request: ADMMURequest
+        @return: ADMMUResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.a_dmmuwith_options_async(request, runtime)
 
     def a_dmini_cog_with_options(
         self,
         request: alinlp_20200629_models.ADMiniCogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ADMiniCogResponse:
+        """
+        @summary AD筛查能力，处理用户传入的答题音频和画钟图片从而计算风险结果
+        
+        @param request: ADMiniCogRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ADMiniCogResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -220,14 +279,21 @@
         )
 
     async def a_dmini_cog_with_options_async(
         self,
         request: alinlp_20200629_models.ADMiniCogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ADMiniCogResponse:
+        """
+        @summary AD筛查能力，处理用户传入的答题音频和画钟图片从而计算风险结果
+        
+        @param request: ADMiniCogRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ADMiniCogResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -249,29 +315,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def a_dmini_cog(
         self,
         request: alinlp_20200629_models.ADMiniCogRequest,
     ) -> alinlp_20200629_models.ADMiniCogResponse:
+        """
+        @summary AD筛查能力，处理用户传入的答题音频和画钟图片从而计算风险结果
+        
+        @param request: ADMiniCogRequest
+        @return: ADMiniCogResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.a_dmini_cog_with_options(request, runtime)
 
     async def a_dmini_cog_async(
         self,
         request: alinlp_20200629_models.ADMiniCogRequest,
     ) -> alinlp_20200629_models.ADMiniCogResponse:
+        """
+        @summary AD筛查能力，处理用户传入的答题音频和画钟图片从而计算风险结果
+        
+        @param request: ADMiniCogRequest
+        @return: ADMiniCogResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.a_dmini_cog_with_options_async(request, runtime)
 
     def a_dmini_cog_result_with_options(
         self,
         request: alinlp_20200629_models.ADMiniCogResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ADMiniCogResultResponse:
+        """
+        @summary AD筛查能力,提供给用户查询筛查结果，筛查结果来源自接口ADMIniCog
+        
+        @param request: ADMiniCogResultRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ADMiniCogResultResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -294,14 +379,21 @@
         )
 
     async def a_dmini_cog_result_with_options_async(
         self,
         request: alinlp_20200629_models.ADMiniCogResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ADMiniCogResultResponse:
+        """
+        @summary AD筛查能力,提供给用户查询筛查结果，筛查结果来源自接口ADMIniCog
+        
+        @param request: ADMiniCogResultRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ADMiniCogResultResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -323,39 +415,60 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def a_dmini_cog_result(
         self,
         request: alinlp_20200629_models.ADMiniCogResultRequest,
     ) -> alinlp_20200629_models.ADMiniCogResultResponse:
+        """
+        @summary AD筛查能力,提供给用户查询筛查结果，筛查结果来源自接口ADMIniCog
+        
+        @param request: ADMiniCogResultRequest
+        @return: ADMiniCogResultResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.a_dmini_cog_result_with_options(request, runtime)
 
     async def a_dmini_cog_result_async(
         self,
         request: alinlp_20200629_models.ADMiniCogResultRequest,
     ) -> alinlp_20200629_models.ADMiniCogResultResponse:
+        """
+        @summary AD筛查能力,提供给用户查询筛查结果，筛查结果来源自接口ADMIniCog
+        
+        @param request: ADMiniCogResultRequest
+        @return: ADMiniCogResultResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.a_dmini_cog_result_with_options_async(request, runtime)
 
     def delete_service_data_by_conditions_with_options(
         self,
         tmp_req: alinlp_20200629_models.DeleteServiceDataByConditionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.DeleteServiceDataByConditionsResponse:
+        """
+        @summary 根据条件删除服务数据
+        
+        @param tmp_req: DeleteServiceDataByConditionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteServiceDataByConditionsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.DeleteServiceDataByConditionsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.conditions):
             request.conditions_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.conditions, 'Conditions', 'json')
         body = {}
         if not UtilClient.is_unset(request.conditions_shrink):
             body['Conditions'] = request.conditions_shrink
         if not UtilClient.is_unset(request.service_id):
             body['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.x_dash_scope_open_apisource):
+            body['X-DashScope-OpenAPISource'] = request.x_dash_scope_open_apisource
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteServiceDataByConditions',
             version='2020-06-29',
             protocol='HTTPS',
@@ -372,24 +485,33 @@
         )
 
     async def delete_service_data_by_conditions_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.DeleteServiceDataByConditionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.DeleteServiceDataByConditionsResponse:
+        """
+        @summary 根据条件删除服务数据
+        
+        @param tmp_req: DeleteServiceDataByConditionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteServiceDataByConditionsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.DeleteServiceDataByConditionsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.conditions):
             request.conditions_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.conditions, 'Conditions', 'json')
         body = {}
         if not UtilClient.is_unset(request.conditions_shrink):
             body['Conditions'] = request.conditions_shrink
         if not UtilClient.is_unset(request.service_id):
             body['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.x_dash_scope_open_apisource):
+            body['X-DashScope-OpenAPISource'] = request.x_dash_scope_open_apisource
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DeleteServiceDataByConditions',
             version='2020-06-29',
             protocol='HTTPS',
@@ -405,29 +527,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_service_data_by_conditions(
         self,
         request: alinlp_20200629_models.DeleteServiceDataByConditionsRequest,
     ) -> alinlp_20200629_models.DeleteServiceDataByConditionsResponse:
+        """
+        @summary 根据条件删除服务数据
+        
+        @param request: DeleteServiceDataByConditionsRequest
+        @return: DeleteServiceDataByConditionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_service_data_by_conditions_with_options(request, runtime)
 
     async def delete_service_data_by_conditions_async(
         self,
         request: alinlp_20200629_models.DeleteServiceDataByConditionsRequest,
     ) -> alinlp_20200629_models.DeleteServiceDataByConditionsResponse:
+        """
+        @summary 根据条件删除服务数据
+        
+        @param request: DeleteServiceDataByConditionsRequest
+        @return: DeleteServiceDataByConditionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_service_data_by_conditions_with_options_async(request, runtime)
 
     def delete_service_data_by_ids_with_options(
         self,
         tmp_req: alinlp_20200629_models.DeleteServiceDataByIdsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.DeleteServiceDataByIdsResponse:
+        """
+        @summary 根据ids删除服务数据
+        
+        @param tmp_req: DeleteServiceDataByIdsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteServiceDataByIdsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.DeleteServiceDataByIdsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.ids):
             request.ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ids, 'Ids', 'json')
         body = {}
         if not UtilClient.is_unset(request.ids_shrink):
@@ -454,14 +595,21 @@
         )
 
     async def delete_service_data_by_ids_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.DeleteServiceDataByIdsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.DeleteServiceDataByIdsResponse:
+        """
+        @summary 根据ids删除服务数据
+        
+        @param tmp_req: DeleteServiceDataByIdsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteServiceDataByIdsResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.DeleteServiceDataByIdsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.ids):
             request.ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ids, 'Ids', 'json')
         body = {}
         if not UtilClient.is_unset(request.ids_shrink):
@@ -487,29 +635,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_service_data_by_ids(
         self,
         request: alinlp_20200629_models.DeleteServiceDataByIdsRequest,
     ) -> alinlp_20200629_models.DeleteServiceDataByIdsResponse:
+        """
+        @summary 根据ids删除服务数据
+        
+        @param request: DeleteServiceDataByIdsRequest
+        @return: DeleteServiceDataByIdsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_service_data_by_ids_with_options(request, runtime)
 
     async def delete_service_data_by_ids_async(
         self,
         request: alinlp_20200629_models.DeleteServiceDataByIdsRequest,
     ) -> alinlp_20200629_models.DeleteServiceDataByIdsResponse:
+        """
+        @summary 根据ids删除服务数据
+        
+        @param request: DeleteServiceDataByIdsRequest
+        @return: DeleteServiceDataByIdsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_service_data_by_ids_with_options_async(request, runtime)
 
     def get_brand_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetBrandChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetBrandChEcomResponse:
+        """
+        @summary 品牌预测
+        
+        @param request: GetBrandChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetBrandChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.image_url):
             body['ImageUrl'] = request.image_url
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -534,14 +701,21 @@
         )
 
     async def get_brand_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetBrandChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetBrandChEcomResponse:
+        """
+        @summary 品牌预测
+        
+        @param request: GetBrandChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetBrandChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.image_url):
             body['ImageUrl'] = request.image_url
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -565,29 +739,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_brand_ch_ecom(
         self,
         request: alinlp_20200629_models.GetBrandChEcomRequest,
     ) -> alinlp_20200629_models.GetBrandChEcomResponse:
+        """
+        @summary 品牌预测
+        
+        @param request: GetBrandChEcomRequest
+        @return: GetBrandChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_brand_ch_ecom_with_options(request, runtime)
 
     async def get_brand_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetBrandChEcomRequest,
     ) -> alinlp_20200629_models.GetBrandChEcomResponse:
+        """
+        @summary 品牌预测
+        
+        @param request: GetBrandChEcomRequest
+        @return: GetBrandChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_brand_ch_ecom_with_options_async(request, runtime)
 
     def get_cate_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetCateChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetCateChEcomResponse:
+        """
+        @summary 类目预测
+        
+        @param request: GetCateChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetCateChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.image_url):
             body['ImageUrl'] = request.image_url
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -612,14 +805,21 @@
         )
 
     async def get_cate_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetCateChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetCateChEcomResponse:
+        """
+        @summary 类目预测
+        
+        @param request: GetCateChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetCateChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.image_url):
             body['ImageUrl'] = request.image_url
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -643,29 +843,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_cate_ch_ecom(
         self,
         request: alinlp_20200629_models.GetCateChEcomRequest,
     ) -> alinlp_20200629_models.GetCateChEcomResponse:
+        """
+        @summary 类目预测
+        
+        @param request: GetCateChEcomRequest
+        @return: GetCateChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_cate_ch_ecom_with_options(request, runtime)
 
     async def get_cate_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetCateChEcomRequest,
     ) -> alinlp_20200629_models.GetCateChEcomResponse:
+        """
+        @summary 类目预测
+        
+        @param request: GetCateChEcomRequest
+        @return: GetCateChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_cate_ch_ecom_with_options_async(request, runtime)
 
     def get_check_duplication_ch_medical_with_options(
         self,
         request: alinlp_20200629_models.GetCheckDuplicationChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetCheckDuplicationChMedicalResponse:
+        """
+        @param request: GetCheckDuplicationChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetCheckDuplicationChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.origin_q):
             body['OriginQ'] = request.origin_q
         if not UtilClient.is_unset(request.origin_t):
             body['OriginT'] = request.origin_t
         if not UtilClient.is_unset(request.service_code):
@@ -690,14 +907,19 @@
         )
 
     async def get_check_duplication_ch_medical_with_options_async(
         self,
         request: alinlp_20200629_models.GetCheckDuplicationChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetCheckDuplicationChMedicalResponse:
+        """
+        @param request: GetCheckDuplicationChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetCheckDuplicationChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.origin_q):
             body['OriginQ'] = request.origin_q
         if not UtilClient.is_unset(request.origin_t):
             body['OriginT'] = request.origin_t
         if not UtilClient.is_unset(request.service_code):
@@ -721,29 +943,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_check_duplication_ch_medical(
         self,
         request: alinlp_20200629_models.GetCheckDuplicationChMedicalRequest,
     ) -> alinlp_20200629_models.GetCheckDuplicationChMedicalResponse:
+        """
+        @param request: GetCheckDuplicationChMedicalRequest
+        @return: GetCheckDuplicationChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_check_duplication_ch_medical_with_options(request, runtime)
 
     async def get_check_duplication_ch_medical_async(
         self,
         request: alinlp_20200629_models.GetCheckDuplicationChMedicalRequest,
     ) -> alinlp_20200629_models.GetCheckDuplicationChMedicalResponse:
+        """
+        @param request: GetCheckDuplicationChMedicalRequest
+        @return: GetCheckDuplicationChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_check_duplication_ch_medical_with_options_async(request, runtime)
 
     def get_diagnosis_ch_medical_with_options(
         self,
         request: alinlp_20200629_models.GetDiagnosisChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetDiagnosisChMedicalResponse:
+        """
+        @param request: GetDiagnosisChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDiagnosisChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -766,14 +1001,19 @@
         )
 
     async def get_diagnosis_ch_medical_with_options_async(
         self,
         request: alinlp_20200629_models.GetDiagnosisChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetDiagnosisChMedicalResponse:
+        """
+        @param request: GetDiagnosisChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDiagnosisChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -795,29 +1035,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_diagnosis_ch_medical(
         self,
         request: alinlp_20200629_models.GetDiagnosisChMedicalRequest,
     ) -> alinlp_20200629_models.GetDiagnosisChMedicalResponse:
+        """
+        @param request: GetDiagnosisChMedicalRequest
+        @return: GetDiagnosisChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_diagnosis_ch_medical_with_options(request, runtime)
 
     async def get_diagnosis_ch_medical_async(
         self,
         request: alinlp_20200629_models.GetDiagnosisChMedicalRequest,
     ) -> alinlp_20200629_models.GetDiagnosisChMedicalResponse:
+        """
+        @param request: GetDiagnosisChMedicalRequest
+        @return: GetDiagnosisChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_diagnosis_ch_medical_with_options_async(request, runtime)
 
     def get_dp_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetDpChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetDpChEcomResponse:
+        """
+        @param request: GetDpChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDpChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -840,14 +1093,19 @@
         )
 
     async def get_dp_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetDpChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetDpChEcomResponse:
+        """
+        @param request: GetDpChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDpChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -869,29 +1127,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_dp_ch_ecom(
         self,
         request: alinlp_20200629_models.GetDpChEcomRequest,
     ) -> alinlp_20200629_models.GetDpChEcomResponse:
+        """
+        @param request: GetDpChEcomRequest
+        @return: GetDpChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_dp_ch_ecom_with_options(request, runtime)
 
     async def get_dp_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetDpChEcomRequest,
     ) -> alinlp_20200629_models.GetDpChEcomResponse:
+        """
+        @param request: GetDpChEcomRequest
+        @return: GetDpChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_dp_ch_ecom_with_options_async(request, runtime)
 
     def get_dp_ch_general_ctbwith_options(
         self,
         request: alinlp_20200629_models.GetDpChGeneralCTBRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetDpChGeneralCTBResponse:
+        """
+        @param request: GetDpChGeneralCTBRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDpChGeneralCTBResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -914,14 +1185,19 @@
         )
 
     async def get_dp_ch_general_ctbwith_options_async(
         self,
         request: alinlp_20200629_models.GetDpChGeneralCTBRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetDpChGeneralCTBResponse:
+        """
+        @param request: GetDpChGeneralCTBRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDpChGeneralCTBResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -943,29 +1219,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_dp_ch_general_ctb(
         self,
         request: alinlp_20200629_models.GetDpChGeneralCTBRequest,
     ) -> alinlp_20200629_models.GetDpChGeneralCTBResponse:
+        """
+        @param request: GetDpChGeneralCTBRequest
+        @return: GetDpChGeneralCTBResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_dp_ch_general_ctbwith_options(request, runtime)
 
     async def get_dp_ch_general_ctb_async(
         self,
         request: alinlp_20200629_models.GetDpChGeneralCTBRequest,
     ) -> alinlp_20200629_models.GetDpChGeneralCTBResponse:
+        """
+        @param request: GetDpChGeneralCTBRequest
+        @return: GetDpChGeneralCTBResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_dp_ch_general_ctbwith_options_async(request, runtime)
 
     def get_dp_ch_general_stanford_with_options(
         self,
         request: alinlp_20200629_models.GetDpChGeneralStanfordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetDpChGeneralStanfordResponse:
+        """
+        @param request: GetDpChGeneralStanfordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDpChGeneralStanfordResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -988,14 +1277,19 @@
         )
 
     async def get_dp_ch_general_stanford_with_options_async(
         self,
         request: alinlp_20200629_models.GetDpChGeneralStanfordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetDpChGeneralStanfordResponse:
+        """
+        @param request: GetDpChGeneralStanfordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDpChGeneralStanfordResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1017,29 +1311,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_dp_ch_general_stanford(
         self,
         request: alinlp_20200629_models.GetDpChGeneralStanfordRequest,
     ) -> alinlp_20200629_models.GetDpChGeneralStanfordResponse:
+        """
+        @param request: GetDpChGeneralStanfordRequest
+        @return: GetDpChGeneralStanfordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_dp_ch_general_stanford_with_options(request, runtime)
 
     async def get_dp_ch_general_stanford_async(
         self,
         request: alinlp_20200629_models.GetDpChGeneralStanfordRequest,
     ) -> alinlp_20200629_models.GetDpChGeneralStanfordResponse:
+        """
+        @param request: GetDpChGeneralStanfordRequest
+        @return: GetDpChGeneralStanfordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_dp_ch_general_stanford_with_options_async(request, runtime)
 
     def get_ec_ch_general_with_options(
         self,
         request: alinlp_20200629_models.GetEcChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetEcChGeneralResponse:
+        """
+        @param request: GetEcChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetEcChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1062,14 +1369,19 @@
         )
 
     async def get_ec_ch_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetEcChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetEcChGeneralResponse:
+        """
+        @param request: GetEcChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetEcChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1091,29 +1403,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ec_ch_general(
         self,
         request: alinlp_20200629_models.GetEcChGeneralRequest,
     ) -> alinlp_20200629_models.GetEcChGeneralResponse:
+        """
+        @param request: GetEcChGeneralRequest
+        @return: GetEcChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ec_ch_general_with_options(request, runtime)
 
     async def get_ec_ch_general_async(
         self,
         request: alinlp_20200629_models.GetEcChGeneralRequest,
     ) -> alinlp_20200629_models.GetEcChGeneralResponse:
+        """
+        @param request: GetEcChGeneralRequest
+        @return: GetEcChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ec_ch_general_with_options_async(request, runtime)
 
     def get_ec_en_general_with_options(
         self,
         request: alinlp_20200629_models.GetEcEnGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetEcEnGeneralResponse:
+        """
+        @param request: GetEcEnGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetEcEnGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1136,14 +1461,19 @@
         )
 
     async def get_ec_en_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetEcEnGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetEcEnGeneralResponse:
+        """
+        @param request: GetEcEnGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetEcEnGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1165,29 +1495,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ec_en_general(
         self,
         request: alinlp_20200629_models.GetEcEnGeneralRequest,
     ) -> alinlp_20200629_models.GetEcEnGeneralResponse:
+        """
+        @param request: GetEcEnGeneralRequest
+        @return: GetEcEnGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ec_en_general_with_options(request, runtime)
 
     async def get_ec_en_general_async(
         self,
         request: alinlp_20200629_models.GetEcEnGeneralRequest,
     ) -> alinlp_20200629_models.GetEcEnGeneralResponse:
+        """
+        @param request: GetEcEnGeneralRequest
+        @return: GetEcEnGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ec_en_general_with_options_async(request, runtime)
 
     def get_embedding_with_options(
         self,
         request: alinlp_20200629_models.GetEmbeddingRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetEmbeddingResponse:
+        """
+        @summary embedding
+        
+        @param request: GetEmbeddingRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetEmbeddingResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         if not UtilClient.is_unset(request.text_type):
@@ -1212,14 +1557,21 @@
         )
 
     async def get_embedding_with_options_async(
         self,
         request: alinlp_20200629_models.GetEmbeddingRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetEmbeddingResponse:
+        """
+        @summary embedding
+        
+        @param request: GetEmbeddingRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetEmbeddingResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         if not UtilClient.is_unset(request.text_type):
@@ -1243,29 +1595,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_embedding(
         self,
         request: alinlp_20200629_models.GetEmbeddingRequest,
     ) -> alinlp_20200629_models.GetEmbeddingResponse:
+        """
+        @summary embedding
+        
+        @param request: GetEmbeddingRequest
+        @return: GetEmbeddingResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_embedding_with_options(request, runtime)
 
     async def get_embedding_async(
         self,
         request: alinlp_20200629_models.GetEmbeddingRequest,
     ) -> alinlp_20200629_models.GetEmbeddingResponse:
+        """
+        @summary embedding
+        
+        @param request: GetEmbeddingRequest
+        @return: GetEmbeddingResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_embedding_with_options_async(request, runtime)
 
     def get_item_pub_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetItemPubChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetItemPubChEcomResponse:
+        """
+        @summary 微购整合接口
+        
+        @param request: GetItemPubChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetItemPubChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.image_url):
             body['ImageUrl'] = request.image_url
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1290,14 +1661,21 @@
         )
 
     async def get_item_pub_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetItemPubChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetItemPubChEcomResponse:
+        """
+        @summary 微购整合接口
+        
+        @param request: GetItemPubChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetItemPubChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.image_url):
             body['ImageUrl'] = request.image_url
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1321,29 +1699,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_item_pub_ch_ecom(
         self,
         request: alinlp_20200629_models.GetItemPubChEcomRequest,
     ) -> alinlp_20200629_models.GetItemPubChEcomResponse:
+        """
+        @summary 微购整合接口
+        
+        @param request: GetItemPubChEcomRequest
+        @return: GetItemPubChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_item_pub_ch_ecom_with_options(request, runtime)
 
     async def get_item_pub_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetItemPubChEcomRequest,
     ) -> alinlp_20200629_models.GetItemPubChEcomResponse:
+        """
+        @summary 微购整合接口
+        
+        @param request: GetItemPubChEcomRequest
+        @return: GetItemPubChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_item_pub_ch_ecom_with_options_async(request, runtime)
 
     def get_keyword_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetKeywordChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetKeywordChEcomResponse:
+        """
+        @param request: GetKeywordChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetKeywordChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.api_version):
             body['ApiVersion'] = request.api_version
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1368,14 +1763,19 @@
         )
 
     async def get_keyword_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetKeywordChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetKeywordChEcomResponse:
+        """
+        @param request: GetKeywordChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetKeywordChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.api_version):
             body['ApiVersion'] = request.api_version
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1399,29 +1799,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_keyword_ch_ecom(
         self,
         request: alinlp_20200629_models.GetKeywordChEcomRequest,
     ) -> alinlp_20200629_models.GetKeywordChEcomResponse:
+        """
+        @param request: GetKeywordChEcomRequest
+        @return: GetKeywordChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_keyword_ch_ecom_with_options(request, runtime)
 
     async def get_keyword_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetKeywordChEcomRequest,
     ) -> alinlp_20200629_models.GetKeywordChEcomResponse:
+        """
+        @param request: GetKeywordChEcomRequest
+        @return: GetKeywordChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_keyword_ch_ecom_with_options_async(request, runtime)
 
     def get_keyword_en_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetKeywordEnEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetKeywordEnEcomResponse:
+        """
+        @param request: GetKeywordEnEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetKeywordEnEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1444,14 +1857,19 @@
         )
 
     async def get_keyword_en_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetKeywordEnEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetKeywordEnEcomResponse:
+        """
+        @param request: GetKeywordEnEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetKeywordEnEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1473,29 +1891,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_keyword_en_ecom(
         self,
         request: alinlp_20200629_models.GetKeywordEnEcomRequest,
     ) -> alinlp_20200629_models.GetKeywordEnEcomResponse:
+        """
+        @param request: GetKeywordEnEcomRequest
+        @return: GetKeywordEnEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_keyword_en_ecom_with_options(request, runtime)
 
     async def get_keyword_en_ecom_async(
         self,
         request: alinlp_20200629_models.GetKeywordEnEcomRequest,
     ) -> alinlp_20200629_models.GetKeywordEnEcomResponse:
+        """
+        @param request: GetKeywordEnEcomRequest
+        @return: GetKeywordEnEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_keyword_en_ecom_with_options_async(request, runtime)
 
     def get_medicine_ch_medical_with_options(
         self,
         request: alinlp_20200629_models.GetMedicineChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetMedicineChMedicalResponse:
+        """
+        @param request: GetMedicineChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMedicineChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.factory):
             body['Factory'] = request.factory
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.service_code):
@@ -1524,14 +1955,19 @@
         )
 
     async def get_medicine_ch_medical_with_options_async(
         self,
         request: alinlp_20200629_models.GetMedicineChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetMedicineChMedicalResponse:
+        """
+        @param request: GetMedicineChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMedicineChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.factory):
             body['Factory'] = request.factory
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.service_code):
@@ -1559,29 +1995,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_medicine_ch_medical(
         self,
         request: alinlp_20200629_models.GetMedicineChMedicalRequest,
     ) -> alinlp_20200629_models.GetMedicineChMedicalResponse:
+        """
+        @param request: GetMedicineChMedicalRequest
+        @return: GetMedicineChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_medicine_ch_medical_with_options(request, runtime)
 
     async def get_medicine_ch_medical_async(
         self,
         request: alinlp_20200629_models.GetMedicineChMedicalRequest,
     ) -> alinlp_20200629_models.GetMedicineChMedicalResponse:
+        """
+        @param request: GetMedicineChMedicalRequest
+        @return: GetMedicineChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_medicine_ch_medical_with_options_async(request, runtime)
 
     def get_ner_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetNerChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetNerChEcomResponse:
+        """
+        @param request: GetNerChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNerChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.lexer_id):
             body['LexerId'] = request.lexer_id
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1606,14 +2055,19 @@
         )
 
     async def get_ner_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetNerChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetNerChEcomResponse:
+        """
+        @param request: GetNerChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNerChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.lexer_id):
             body['LexerId'] = request.lexer_id
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1637,29 +2091,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ner_ch_ecom(
         self,
         request: alinlp_20200629_models.GetNerChEcomRequest,
     ) -> alinlp_20200629_models.GetNerChEcomResponse:
+        """
+        @param request: GetNerChEcomRequest
+        @return: GetNerChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ner_ch_ecom_with_options(request, runtime)
 
     async def get_ner_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetNerChEcomRequest,
     ) -> alinlp_20200629_models.GetNerChEcomResponse:
+        """
+        @param request: GetNerChEcomRequest
+        @return: GetNerChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ner_ch_ecom_with_options_async(request, runtime)
 
     def get_ner_ch_medical_with_options(
         self,
         request: alinlp_20200629_models.GetNerChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetNerChMedicalResponse:
+        """
+        @param request: GetNerChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNerChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1682,14 +2149,19 @@
         )
 
     async def get_ner_ch_medical_with_options_async(
         self,
         request: alinlp_20200629_models.GetNerChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetNerChMedicalResponse:
+        """
+        @param request: GetNerChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNerChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -1711,29 +2183,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ner_ch_medical(
         self,
         request: alinlp_20200629_models.GetNerChMedicalRequest,
     ) -> alinlp_20200629_models.GetNerChMedicalResponse:
+        """
+        @param request: GetNerChMedicalRequest
+        @return: GetNerChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ner_ch_medical_with_options(request, runtime)
 
     async def get_ner_ch_medical_async(
         self,
         request: alinlp_20200629_models.GetNerChMedicalRequest,
     ) -> alinlp_20200629_models.GetNerChMedicalResponse:
+        """
+        @param request: GetNerChMedicalRequest
+        @return: GetNerChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ner_ch_medical_with_options_async(request, runtime)
 
     def get_ner_customized_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetNerCustomizedChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetNerCustomizedChEcomResponse:
+        """
+        @param request: GetNerCustomizedChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNerCustomizedChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.lexer_id):
             body['LexerId'] = request.lexer_id
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1758,14 +2243,19 @@
         )
 
     async def get_ner_customized_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetNerCustomizedChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetNerCustomizedChEcomResponse:
+        """
+        @param request: GetNerCustomizedChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNerCustomizedChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.lexer_id):
             body['LexerId'] = request.lexer_id
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1789,29 +2279,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ner_customized_ch_ecom(
         self,
         request: alinlp_20200629_models.GetNerCustomizedChEcomRequest,
     ) -> alinlp_20200629_models.GetNerCustomizedChEcomResponse:
+        """
+        @param request: GetNerCustomizedChEcomRequest
+        @return: GetNerCustomizedChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ner_customized_ch_ecom_with_options(request, runtime)
 
     async def get_ner_customized_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetNerCustomizedChEcomRequest,
     ) -> alinlp_20200629_models.GetNerCustomizedChEcomResponse:
+        """
+        @param request: GetNerCustomizedChEcomRequest
+        @return: GetNerCustomizedChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ner_customized_ch_ecom_with_options_async(request, runtime)
 
     def get_ner_customized_sea_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetNerCustomizedSeaEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetNerCustomizedSeaEcomResponse:
+        """
+        @param request: GetNerCustomizedSeaEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNerCustomizedSeaEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1836,14 +2339,19 @@
         )
 
     async def get_ner_customized_sea_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetNerCustomizedSeaEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetNerCustomizedSeaEcomResponse:
+        """
+        @param request: GetNerCustomizedSeaEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNerCustomizedSeaEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -1867,29 +2375,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ner_customized_sea_ecom(
         self,
         request: alinlp_20200629_models.GetNerCustomizedSeaEcomRequest,
     ) -> alinlp_20200629_models.GetNerCustomizedSeaEcomResponse:
+        """
+        @param request: GetNerCustomizedSeaEcomRequest
+        @return: GetNerCustomizedSeaEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ner_customized_sea_ecom_with_options(request, runtime)
 
     async def get_ner_customized_sea_ecom_async(
         self,
         request: alinlp_20200629_models.GetNerCustomizedSeaEcomRequest,
     ) -> alinlp_20200629_models.GetNerCustomizedSeaEcomResponse:
+        """
+        @param request: GetNerCustomizedSeaEcomRequest
+        @return: GetNerCustomizedSeaEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ner_customized_sea_ecom_with_options_async(request, runtime)
 
     def get_open_nluwith_options(
         self,
         request: alinlp_20200629_models.GetOpenNLURequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetOpenNLUResponse:
+        """
+        @summary openNLU
+        
+        @param request: GetOpenNLURequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOpenNLUResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.examples):
             body['Examples'] = request.examples
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.sentence):
@@ -1918,14 +2441,21 @@
         )
 
     async def get_open_nluwith_options_async(
         self,
         request: alinlp_20200629_models.GetOpenNLURequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetOpenNLUResponse:
+        """
+        @summary openNLU
+        
+        @param request: GetOpenNLURequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOpenNLUResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.examples):
             body['Examples'] = request.examples
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.sentence):
@@ -1953,29 +2483,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_open_nlu(
         self,
         request: alinlp_20200629_models.GetOpenNLURequest,
     ) -> alinlp_20200629_models.GetOpenNLUResponse:
+        """
+        @summary openNLU
+        
+        @param request: GetOpenNLURequest
+        @return: GetOpenNLUResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_open_nluwith_options(request, runtime)
 
     async def get_open_nlu_async(
         self,
         request: alinlp_20200629_models.GetOpenNLURequest,
     ) -> alinlp_20200629_models.GetOpenNLUResponse:
+        """
+        @summary openNLU
+        
+        @param request: GetOpenNLURequest
+        @return: GetOpenNLUResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_open_nluwith_options_async(request, runtime)
 
     def get_open_nluhigh_recall_with_options(
         self,
         request: alinlp_20200629_models.GetOpenNLUHighRecallRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetOpenNLUHighRecallResponse:
+        """
+        @summary openNLU高召回版
+        
+        @param request: GetOpenNLUHighRecallRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOpenNLUHighRecallResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.examples):
             body['Examples'] = request.examples
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.sentence):
@@ -2004,14 +2553,21 @@
         )
 
     async def get_open_nluhigh_recall_with_options_async(
         self,
         request: alinlp_20200629_models.GetOpenNLUHighRecallRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetOpenNLUHighRecallResponse:
+        """
+        @summary openNLU高召回版
+        
+        @param request: GetOpenNLUHighRecallRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOpenNLUHighRecallResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.examples):
             body['Examples'] = request.examples
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.sentence):
@@ -2039,29 +2595,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_open_nluhigh_recall(
         self,
         request: alinlp_20200629_models.GetOpenNLUHighRecallRequest,
     ) -> alinlp_20200629_models.GetOpenNLUHighRecallResponse:
+        """
+        @summary openNLU高召回版
+        
+        @param request: GetOpenNLUHighRecallRequest
+        @return: GetOpenNLUHighRecallResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_open_nluhigh_recall_with_options(request, runtime)
 
     async def get_open_nluhigh_recall_async(
         self,
         request: alinlp_20200629_models.GetOpenNLUHighRecallRequest,
     ) -> alinlp_20200629_models.GetOpenNLUHighRecallResponse:
+        """
+        @summary openNLU高召回版
+        
+        @param request: GetOpenNLUHighRecallRequest
+        @return: GetOpenNLUHighRecallResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_open_nluhigh_recall_with_options_async(request, runtime)
 
     def get_operation_ch_medical_with_options(
         self,
         request: alinlp_20200629_models.GetOperationChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetOperationChMedicalResponse:
+        """
+        @param request: GetOperationChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOperationChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -2084,14 +2657,19 @@
         )
 
     async def get_operation_ch_medical_with_options_async(
         self,
         request: alinlp_20200629_models.GetOperationChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetOperationChMedicalResponse:
+        """
+        @param request: GetOperationChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOperationChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -2113,29 +2691,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_operation_ch_medical(
         self,
         request: alinlp_20200629_models.GetOperationChMedicalRequest,
     ) -> alinlp_20200629_models.GetOperationChMedicalResponse:
+        """
+        @param request: GetOperationChMedicalRequest
+        @return: GetOperationChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_operation_ch_medical_with_options(request, runtime)
 
     async def get_operation_ch_medical_async(
         self,
         request: alinlp_20200629_models.GetOperationChMedicalRequest,
     ) -> alinlp_20200629_models.GetOperationChMedicalResponse:
+        """
+        @param request: GetOperationChMedicalRequest
+        @return: GetOperationChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_operation_ch_medical_with_options_async(request, runtime)
 
     def get_pos_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetPosChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetPosChEcomResponse:
+        """
+        @param request: GetPosChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPosChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -2162,14 +2753,19 @@
         )
 
     async def get_pos_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetPosChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetPosChEcomResponse:
+        """
+        @param request: GetPosChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPosChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -2195,29 +2791,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_pos_ch_ecom(
         self,
         request: alinlp_20200629_models.GetPosChEcomRequest,
     ) -> alinlp_20200629_models.GetPosChEcomResponse:
+        """
+        @param request: GetPosChEcomRequest
+        @return: GetPosChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_pos_ch_ecom_with_options(request, runtime)
 
     async def get_pos_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetPosChEcomRequest,
     ) -> alinlp_20200629_models.GetPosChEcomResponse:
+        """
+        @param request: GetPosChEcomRequest
+        @return: GetPosChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_pos_ch_ecom_with_options_async(request, runtime)
 
     def get_pos_ch_general_with_options(
         self,
         request: alinlp_20200629_models.GetPosChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetPosChGeneralResponse:
+        """
+        @param request: GetPosChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPosChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -2244,14 +2853,19 @@
         )
 
     async def get_pos_ch_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetPosChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetPosChGeneralResponse:
+        """
+        @param request: GetPosChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPosChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -2277,29 +2891,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_pos_ch_general(
         self,
         request: alinlp_20200629_models.GetPosChGeneralRequest,
     ) -> alinlp_20200629_models.GetPosChGeneralResponse:
+        """
+        @param request: GetPosChGeneralRequest
+        @return: GetPosChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_pos_ch_general_with_options(request, runtime)
 
     async def get_pos_ch_general_async(
         self,
         request: alinlp_20200629_models.GetPosChGeneralRequest,
     ) -> alinlp_20200629_models.GetPosChGeneralResponse:
+        """
+        @param request: GetPosChGeneralRequest
+        @return: GetPosChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_pos_ch_general_with_options_async(request, runtime)
 
     def get_price_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetPriceChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetPriceChEcomResponse:
+        """
+        @param request: GetPriceChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPriceChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -2322,14 +2949,19 @@
         )
 
     async def get_price_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetPriceChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetPriceChEcomResponse:
+        """
+        @param request: GetPriceChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPriceChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -2351,29 +2983,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_price_ch_ecom(
         self,
         request: alinlp_20200629_models.GetPriceChEcomRequest,
     ) -> alinlp_20200629_models.GetPriceChEcomResponse:
+        """
+        @param request: GetPriceChEcomRequest
+        @return: GetPriceChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_price_ch_ecom_with_options(request, runtime)
 
     async def get_price_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetPriceChEcomRequest,
     ) -> alinlp_20200629_models.GetPriceChEcomResponse:
+        """
+        @param request: GetPriceChEcomRequest
+        @return: GetPriceChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_price_ch_ecom_with_options_async(request, runtime)
 
     def get_ssetest_with_options(
         self,
         request: alinlp_20200629_models.GetSSETestRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSSETestResponse:
+        """
+        @summary 测试sse
+        
+        @param request: GetSSETestRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSSETestResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -2396,14 +3043,21 @@
         )
 
     async def get_ssetest_with_options_async(
         self,
         request: alinlp_20200629_models.GetSSETestRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSSETestResponse:
+        """
+        @summary 测试sse
+        
+        @param request: GetSSETestRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSSETestResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -2425,29 +3079,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ssetest(
         self,
         request: alinlp_20200629_models.GetSSETestRequest,
     ) -> alinlp_20200629_models.GetSSETestResponse:
+        """
+        @summary 测试sse
+        
+        @param request: GetSSETestRequest
+        @return: GetSSETestResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ssetest_with_options(request, runtime)
 
     async def get_ssetest_async(
         self,
         request: alinlp_20200629_models.GetSSETestRequest,
     ) -> alinlp_20200629_models.GetSSETestResponse:
+        """
+        @summary 测试sse
+        
+        @param request: GetSSETestRequest
+        @return: GetSSETestResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ssetest_with_options_async(request, runtime)
 
     def get_sa_ch_general_with_options(
         self,
         request: alinlp_20200629_models.GetSaChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSaChGeneralResponse:
+        """
+        @param request: GetSaChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSaChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -2470,14 +3141,19 @@
         )
 
     async def get_sa_ch_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetSaChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSaChGeneralResponse:
+        """
+        @param request: GetSaChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSaChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -2499,29 +3175,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_sa_ch_general(
         self,
         request: alinlp_20200629_models.GetSaChGeneralRequest,
     ) -> alinlp_20200629_models.GetSaChGeneralResponse:
+        """
+        @param request: GetSaChGeneralRequest
+        @return: GetSaChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_sa_ch_general_with_options(request, runtime)
 
     async def get_sa_ch_general_async(
         self,
         request: alinlp_20200629_models.GetSaChGeneralRequest,
     ) -> alinlp_20200629_models.GetSaChGeneralResponse:
+        """
+        @param request: GetSaChGeneralRequest
+        @return: GetSaChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_sa_ch_general_with_options_async(request, runtime)
 
     def get_sa_sea_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetSaSeaEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSaSeaEcomResponse:
+        """
+        @param request: GetSaSeaEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSaSeaEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -2546,14 +3235,19 @@
         )
 
     async def get_sa_sea_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetSaSeaEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSaSeaEcomResponse:
+        """
+        @param request: GetSaSeaEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSaSeaEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -2577,29 +3271,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_sa_sea_ecom(
         self,
         request: alinlp_20200629_models.GetSaSeaEcomRequest,
     ) -> alinlp_20200629_models.GetSaSeaEcomResponse:
+        """
+        @param request: GetSaSeaEcomRequest
+        @return: GetSaSeaEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_sa_sea_ecom_with_options(request, runtime)
 
     async def get_sa_sea_ecom_async(
         self,
         request: alinlp_20200629_models.GetSaSeaEcomRequest,
     ) -> alinlp_20200629_models.GetSaSeaEcomResponse:
+        """
+        @param request: GetSaSeaEcomRequest
+        @return: GetSaSeaEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_sa_sea_ecom_with_options_async(request, runtime)
 
     def get_service_data_import_status_with_options(
         self,
         tmp_req: alinlp_20200629_models.GetServiceDataImportStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetServiceDataImportStatusResponse:
+        """
+        @summary 获取服务数据导入状态
+        
+        @param tmp_req: GetServiceDataImportStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceDataImportStatusResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.GetServiceDataImportStatusShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.data_import_ids):
             request.data_import_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.data_import_ids, 'DataImportIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.data_import_ids_shrink):
@@ -2624,14 +3333,21 @@
         )
 
     async def get_service_data_import_status_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.GetServiceDataImportStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetServiceDataImportStatusResponse:
+        """
+        @summary 获取服务数据导入状态
+        
+        @param tmp_req: GetServiceDataImportStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceDataImportStatusResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.GetServiceDataImportStatusShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.data_import_ids):
             request.data_import_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.data_import_ids, 'DataImportIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.data_import_ids_shrink):
@@ -2655,29 +3371,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_service_data_import_status(
         self,
         request: alinlp_20200629_models.GetServiceDataImportStatusRequest,
     ) -> alinlp_20200629_models.GetServiceDataImportStatusResponse:
+        """
+        @summary 获取服务数据导入状态
+        
+        @param request: GetServiceDataImportStatusRequest
+        @return: GetServiceDataImportStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_service_data_import_status_with_options(request, runtime)
 
     async def get_service_data_import_status_async(
         self,
         request: alinlp_20200629_models.GetServiceDataImportStatusRequest,
     ) -> alinlp_20200629_models.GetServiceDataImportStatusResponse:
+        """
+        @summary 获取服务数据导入状态
+        
+        @param request: GetServiceDataImportStatusRequest
+        @return: GetServiceDataImportStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_service_data_import_status_with_options_async(request, runtime)
 
     def get_similarity_ch_medical_with_options(
         self,
         request: alinlp_20200629_models.GetSimilarityChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSimilarityChMedicalResponse:
+        """
+        @param request: GetSimilarityChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSimilarityChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.origin_q):
             body['OriginQ'] = request.origin_q
         if not UtilClient.is_unset(request.origin_t):
             body['OriginT'] = request.origin_t
         if not UtilClient.is_unset(request.service_code):
@@ -2702,14 +3435,19 @@
         )
 
     async def get_similarity_ch_medical_with_options_async(
         self,
         request: alinlp_20200629_models.GetSimilarityChMedicalRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSimilarityChMedicalResponse:
+        """
+        @param request: GetSimilarityChMedicalRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSimilarityChMedicalResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.origin_q):
             body['OriginQ'] = request.origin_q
         if not UtilClient.is_unset(request.origin_t):
             body['OriginT'] = request.origin_t
         if not UtilClient.is_unset(request.service_code):
@@ -2733,29 +3471,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_similarity_ch_medical(
         self,
         request: alinlp_20200629_models.GetSimilarityChMedicalRequest,
     ) -> alinlp_20200629_models.GetSimilarityChMedicalResponse:
+        """
+        @param request: GetSimilarityChMedicalRequest
+        @return: GetSimilarityChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_similarity_ch_medical_with_options(request, runtime)
 
     async def get_similarity_ch_medical_async(
         self,
         request: alinlp_20200629_models.GetSimilarityChMedicalRequest,
     ) -> alinlp_20200629_models.GetSimilarityChMedicalResponse:
+        """
+        @param request: GetSimilarityChMedicalRequest
+        @return: GetSimilarityChMedicalResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_similarity_ch_medical_with_options_async(request, runtime)
 
     def get_summary_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetSummaryChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSummaryChEcomResponse:
+        """
+        @param request: GetSummaryChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSummaryChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -2778,14 +3529,19 @@
         )
 
     async def get_summary_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetSummaryChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetSummaryChEcomResponse:
+        """
+        @param request: GetSummaryChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSummaryChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -2807,29 +3563,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_summary_ch_ecom(
         self,
         request: alinlp_20200629_models.GetSummaryChEcomRequest,
     ) -> alinlp_20200629_models.GetSummaryChEcomResponse:
+        """
+        @param request: GetSummaryChEcomRequest
+        @return: GetSummaryChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_summary_ch_ecom_with_options(request, runtime)
 
     async def get_summary_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetSummaryChEcomRequest,
     ) -> alinlp_20200629_models.GetSummaryChEcomResponse:
+        """
+        @param request: GetSummaryChEcomRequest
+        @return: GetSummaryChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_summary_ch_ecom_with_options_async(request, runtime)
 
     def get_table_qaservice_info_by_id_with_options(
         self,
         request: alinlp_20200629_models.GetTableQAServiceInfoByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetTableQAServiceInfoByIdResponse:
+        """
+        @summary 根据id查询tableqa服务基本信息
+        
+        @param request: GetTableQAServiceInfoByIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTableQAServiceInfoByIdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.service_id):
             body['ServiceId'] = request.service_id
         req = open_api_models.OpenApiRequest(
@@ -2852,14 +3623,21 @@
         )
 
     async def get_table_qaservice_info_by_id_with_options_async(
         self,
         request: alinlp_20200629_models.GetTableQAServiceInfoByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetTableQAServiceInfoByIdResponse:
+        """
+        @summary 根据id查询tableqa服务基本信息
+        
+        @param request: GetTableQAServiceInfoByIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTableQAServiceInfoByIdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.service_id):
             body['ServiceId'] = request.service_id
         req = open_api_models.OpenApiRequest(
@@ -2881,29 +3659,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_table_qaservice_info_by_id(
         self,
         request: alinlp_20200629_models.GetTableQAServiceInfoByIdRequest,
     ) -> alinlp_20200629_models.GetTableQAServiceInfoByIdResponse:
+        """
+        @summary 根据id查询tableqa服务基本信息
+        
+        @param request: GetTableQAServiceInfoByIdRequest
+        @return: GetTableQAServiceInfoByIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_table_qaservice_info_by_id_with_options(request, runtime)
 
     async def get_table_qaservice_info_by_id_async(
         self,
         request: alinlp_20200629_models.GetTableQAServiceInfoByIdRequest,
     ) -> alinlp_20200629_models.GetTableQAServiceInfoByIdResponse:
+        """
+        @summary 根据id查询tableqa服务基本信息
+        
+        @param request: GetTableQAServiceInfoByIdRequest
+        @return: GetTableQAServiceInfoByIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_table_qaservice_info_by_id_with_options_async(request, runtime)
 
     def get_tc_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetTcChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetTcChEcomResponse:
+        """
+        @param request: GetTcChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTcChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -2926,14 +3721,19 @@
         )
 
     async def get_tc_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetTcChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetTcChEcomResponse:
+        """
+        @param request: GetTcChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTcChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -2955,29 +3755,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_tc_ch_ecom(
         self,
         request: alinlp_20200629_models.GetTcChEcomRequest,
     ) -> alinlp_20200629_models.GetTcChEcomResponse:
+        """
+        @param request: GetTcChEcomRequest
+        @return: GetTcChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_tc_ch_ecom_with_options(request, runtime)
 
     async def get_tc_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetTcChEcomRequest,
     ) -> alinlp_20200629_models.GetTcChEcomResponse:
+        """
+        @param request: GetTcChEcomRequest
+        @return: GetTcChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_tc_ch_ecom_with_options_async(request, runtime)
 
     def get_tc_ch_general_with_options(
         self,
         request: alinlp_20200629_models.GetTcChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetTcChGeneralResponse:
+        """
+        @param request: GetTcChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTcChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -3000,14 +3813,19 @@
         )
 
     async def get_tc_ch_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetTcChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetTcChGeneralResponse:
+        """
+        @param request: GetTcChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTcChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
             body['Text'] = request.text
         req = open_api_models.OpenApiRequest(
@@ -3029,29 +3847,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_tc_ch_general(
         self,
         request: alinlp_20200629_models.GetTcChGeneralRequest,
     ) -> alinlp_20200629_models.GetTcChGeneralResponse:
+        """
+        @param request: GetTcChGeneralRequest
+        @return: GetTcChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_tc_ch_general_with_options(request, runtime)
 
     async def get_tc_ch_general_async(
         self,
         request: alinlp_20200629_models.GetTcChGeneralRequest,
     ) -> alinlp_20200629_models.GetTcChGeneralResponse:
+        """
+        @param request: GetTcChGeneralRequest
+        @return: GetTcChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_tc_ch_general_with_options_async(request, runtime)
 
     def get_ts_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetTsChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetTsChEcomResponse:
+        """
+        @param request: GetTsChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTsChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.origin_q):
             body['OriginQ'] = request.origin_q
         if not UtilClient.is_unset(request.origin_t):
             body['OriginT'] = request.origin_t
         if not UtilClient.is_unset(request.service_code):
@@ -3078,14 +3909,19 @@
         )
 
     async def get_ts_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetTsChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetTsChEcomResponse:
+        """
+        @param request: GetTsChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTsChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.origin_q):
             body['OriginQ'] = request.origin_q
         if not UtilClient.is_unset(request.origin_t):
             body['OriginT'] = request.origin_t
         if not UtilClient.is_unset(request.service_code):
@@ -3111,29 +3947,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ts_ch_ecom(
         self,
         request: alinlp_20200629_models.GetTsChEcomRequest,
     ) -> alinlp_20200629_models.GetTsChEcomResponse:
+        """
+        @param request: GetTsChEcomRequest
+        @return: GetTsChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ts_ch_ecom_with_options(request, runtime)
 
     async def get_ts_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetTsChEcomRequest,
     ) -> alinlp_20200629_models.GetTsChEcomResponse:
+        """
+        @param request: GetTsChEcomRequest
+        @return: GetTsChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ts_ch_ecom_with_options_async(request, runtime)
 
     def get_user_upload_sign_with_options(
         self,
         request: alinlp_20200629_models.GetUserUploadSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetUserUploadSignResponse:
+        """
+        @param request: GetUserUploadSignRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserUploadSignResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -3154,14 +4003,19 @@
         )
 
     async def get_user_upload_sign_with_options_async(
         self,
         request: alinlp_20200629_models.GetUserUploadSignRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetUserUploadSignResponse:
+        """
+        @param request: GetUserUploadSignRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserUploadSignResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -3181,29 +4035,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_upload_sign(
         self,
         request: alinlp_20200629_models.GetUserUploadSignRequest,
     ) -> alinlp_20200629_models.GetUserUploadSignResponse:
+        """
+        @param request: GetUserUploadSignRequest
+        @return: GetUserUploadSignResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_upload_sign_with_options(request, runtime)
 
     async def get_user_upload_sign_async(
         self,
         request: alinlp_20200629_models.GetUserUploadSignRequest,
     ) -> alinlp_20200629_models.GetUserUploadSignResponse:
+        """
+        @param request: GetUserUploadSignRequest
+        @return: GetUserUploadSignResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_upload_sign_with_options_async(request, runtime)
 
     def get_we_ch_comment_with_options(
         self,
         request: alinlp_20200629_models.GetWeChCommentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChCommentResponse:
+        """
+        @param request: GetWeChCommentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChCommentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3234,14 +4101,19 @@
         )
 
     async def get_we_ch_comment_with_options_async(
         self,
         request: alinlp_20200629_models.GetWeChCommentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChCommentResponse:
+        """
+        @param request: GetWeChCommentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChCommentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3271,29 +4143,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_we_ch_comment(
         self,
         request: alinlp_20200629_models.GetWeChCommentRequest,
     ) -> alinlp_20200629_models.GetWeChCommentResponse:
+        """
+        @param request: GetWeChCommentRequest
+        @return: GetWeChCommentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_we_ch_comment_with_options(request, runtime)
 
     async def get_we_ch_comment_async(
         self,
         request: alinlp_20200629_models.GetWeChCommentRequest,
     ) -> alinlp_20200629_models.GetWeChCommentResponse:
+        """
+        @param request: GetWeChCommentRequest
+        @return: GetWeChCommentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_we_ch_comment_with_options_async(request, runtime)
 
     def get_we_ch_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetWeChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChEcomResponse:
+        """
+        @param request: GetWeChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3324,14 +4209,19 @@
         )
 
     async def get_we_ch_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetWeChEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChEcomResponse:
+        """
+        @param request: GetWeChEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3361,29 +4251,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_we_ch_ecom(
         self,
         request: alinlp_20200629_models.GetWeChEcomRequest,
     ) -> alinlp_20200629_models.GetWeChEcomResponse:
+        """
+        @param request: GetWeChEcomRequest
+        @return: GetWeChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_we_ch_ecom_with_options(request, runtime)
 
     async def get_we_ch_ecom_async(
         self,
         request: alinlp_20200629_models.GetWeChEcomRequest,
     ) -> alinlp_20200629_models.GetWeChEcomResponse:
+        """
+        @param request: GetWeChEcomRequest
+        @return: GetWeChEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_we_ch_ecom_with_options_async(request, runtime)
 
     def get_we_ch_entertainment_with_options(
         self,
         request: alinlp_20200629_models.GetWeChEntertainmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChEntertainmentResponse:
+        """
+        @param request: GetWeChEntertainmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChEntertainmentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3414,14 +4317,19 @@
         )
 
     async def get_we_ch_entertainment_with_options_async(
         self,
         request: alinlp_20200629_models.GetWeChEntertainmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChEntertainmentResponse:
+        """
+        @param request: GetWeChEntertainmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChEntertainmentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3451,29 +4359,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_we_ch_entertainment(
         self,
         request: alinlp_20200629_models.GetWeChEntertainmentRequest,
     ) -> alinlp_20200629_models.GetWeChEntertainmentResponse:
+        """
+        @param request: GetWeChEntertainmentRequest
+        @return: GetWeChEntertainmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_we_ch_entertainment_with_options(request, runtime)
 
     async def get_we_ch_entertainment_async(
         self,
         request: alinlp_20200629_models.GetWeChEntertainmentRequest,
     ) -> alinlp_20200629_models.GetWeChEntertainmentResponse:
+        """
+        @param request: GetWeChEntertainmentRequest
+        @return: GetWeChEntertainmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_we_ch_entertainment_with_options_async(request, runtime)
 
     def get_we_ch_general_with_options(
         self,
         request: alinlp_20200629_models.GetWeChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChGeneralResponse:
+        """
+        @param request: GetWeChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3502,14 +4423,19 @@
         )
 
     async def get_we_ch_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetWeChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChGeneralResponse:
+        """
+        @param request: GetWeChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3537,29 +4463,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_we_ch_general(
         self,
         request: alinlp_20200629_models.GetWeChGeneralRequest,
     ) -> alinlp_20200629_models.GetWeChGeneralResponse:
+        """
+        @param request: GetWeChGeneralRequest
+        @return: GetWeChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_we_ch_general_with_options(request, runtime)
 
     async def get_we_ch_general_async(
         self,
         request: alinlp_20200629_models.GetWeChGeneralRequest,
     ) -> alinlp_20200629_models.GetWeChGeneralResponse:
+        """
+        @param request: GetWeChGeneralRequest
+        @return: GetWeChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_we_ch_general_with_options_async(request, runtime)
 
     def get_we_ch_search_with_options(
         self,
         request: alinlp_20200629_models.GetWeChSearchRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChSearchResponse:
+        """
+        @param request: GetWeChSearchRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChSearchResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3590,14 +4529,19 @@
         )
 
     async def get_we_ch_search_with_options_async(
         self,
         request: alinlp_20200629_models.GetWeChSearchRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWeChSearchResponse:
+        """
+        @param request: GetWeChSearchRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWeChSearchResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.operation):
             body['Operation'] = request.operation
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.size):
@@ -3627,29 +4571,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_we_ch_search(
         self,
         request: alinlp_20200629_models.GetWeChSearchRequest,
     ) -> alinlp_20200629_models.GetWeChSearchResponse:
+        """
+        @param request: GetWeChSearchRequest
+        @return: GetWeChSearchResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_we_ch_search_with_options(request, runtime)
 
     async def get_we_ch_search_async(
         self,
         request: alinlp_20200629_models.GetWeChSearchRequest,
     ) -> alinlp_20200629_models.GetWeChSearchResponse:
+        """
+        @param request: GetWeChSearchRequest
+        @return: GetWeChSearchResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_we_ch_search_with_options_async(request, runtime)
 
     def get_ws_ch_general_with_options(
         self,
         request: alinlp_20200629_models.GetWsChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsChGeneralResponse:
+        """
+        @param request: GetWsChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -3676,14 +4633,19 @@
         )
 
     async def get_ws_ch_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetWsChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsChGeneralResponse:
+        """
+        @param request: GetWsChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -3709,29 +4671,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_ch_general(
         self,
         request: alinlp_20200629_models.GetWsChGeneralRequest,
     ) -> alinlp_20200629_models.GetWsChGeneralResponse:
+        """
+        @param request: GetWsChGeneralRequest
+        @return: GetWsChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_ch_general_with_options(request, runtime)
 
     async def get_ws_ch_general_async(
         self,
         request: alinlp_20200629_models.GetWsChGeneralRequest,
     ) -> alinlp_20200629_models.GetWsChGeneralResponse:
+        """
+        @param request: GetWsChGeneralRequest
+        @return: GetWsChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_ch_general_with_options_async(request, runtime)
 
     def get_ws_customized_ch_ecom_comment_with_options(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomCommentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomCommentResponse:
+        """
+        @param request: GetWsCustomizedChEcomCommentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChEcomCommentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -3758,14 +4733,19 @@
         )
 
     async def get_ws_customized_ch_ecom_comment_with_options_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomCommentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomCommentResponse:
+        """
+        @param request: GetWsCustomizedChEcomCommentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChEcomCommentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -3791,29 +4771,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_customized_ch_ecom_comment(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomCommentRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomCommentResponse:
+        """
+        @param request: GetWsCustomizedChEcomCommentRequest
+        @return: GetWsCustomizedChEcomCommentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_customized_ch_ecom_comment_with_options(request, runtime)
 
     async def get_ws_customized_ch_ecom_comment_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomCommentRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomCommentResponse:
+        """
+        @param request: GetWsCustomizedChEcomCommentRequest
+        @return: GetWsCustomizedChEcomCommentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_customized_ch_ecom_comment_with_options_async(request, runtime)
 
     def get_ws_customized_ch_ecom_content_with_options(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomContentResponse:
+        """
+        @param request: GetWsCustomizedChEcomContentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChEcomContentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -3840,14 +4833,19 @@
         )
 
     async def get_ws_customized_ch_ecom_content_with_options_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomContentResponse:
+        """
+        @param request: GetWsCustomizedChEcomContentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChEcomContentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -3873,29 +4871,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_customized_ch_ecom_content(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomContentRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomContentResponse:
+        """
+        @param request: GetWsCustomizedChEcomContentRequest
+        @return: GetWsCustomizedChEcomContentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_customized_ch_ecom_content_with_options(request, runtime)
 
     async def get_ws_customized_ch_ecom_content_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomContentRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomContentResponse:
+        """
+        @param request: GetWsCustomizedChEcomContentRequest
+        @return: GetWsCustomizedChEcomContentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_customized_ch_ecom_content_with_options_async(request, runtime)
 
     def get_ws_customized_ch_ecom_title_with_options(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomTitleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomTitleResponse:
+        """
+        @param request: GetWsCustomizedChEcomTitleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChEcomTitleResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -3922,14 +4933,19 @@
         )
 
     async def get_ws_customized_ch_ecom_title_with_options_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomTitleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomTitleResponse:
+        """
+        @param request: GetWsCustomizedChEcomTitleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChEcomTitleResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -3955,29 +4971,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_customized_ch_ecom_title(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomTitleRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomTitleResponse:
+        """
+        @param request: GetWsCustomizedChEcomTitleRequest
+        @return: GetWsCustomizedChEcomTitleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_customized_ch_ecom_title_with_options(request, runtime)
 
     async def get_ws_customized_ch_ecom_title_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEcomTitleRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChEcomTitleResponse:
+        """
+        @param request: GetWsCustomizedChEcomTitleRequest
+        @return: GetWsCustomizedChEcomTitleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_customized_ch_ecom_title_with_options_async(request, runtime)
 
     def get_ws_customized_ch_entertainment_with_options(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEntertainmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChEntertainmentResponse:
+        """
+        @param request: GetWsCustomizedChEntertainmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChEntertainmentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4004,14 +5033,19 @@
         )
 
     async def get_ws_customized_ch_entertainment_with_options_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEntertainmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChEntertainmentResponse:
+        """
+        @param request: GetWsCustomizedChEntertainmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChEntertainmentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4037,29 +5071,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_customized_ch_entertainment(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEntertainmentRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChEntertainmentResponse:
+        """
+        @param request: GetWsCustomizedChEntertainmentRequest
+        @return: GetWsCustomizedChEntertainmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_customized_ch_entertainment_with_options(request, runtime)
 
     async def get_ws_customized_ch_entertainment_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChEntertainmentRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChEntertainmentResponse:
+        """
+        @param request: GetWsCustomizedChEntertainmentRequest
+        @return: GetWsCustomizedChEntertainmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_customized_ch_entertainment_with_options_async(request, runtime)
 
     def get_ws_customized_ch_general_with_options(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChGeneralResponse:
+        """
+        @summary a
+        
+        @param request: GetWsCustomizedChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4086,14 +5135,21 @@
         )
 
     async def get_ws_customized_ch_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChGeneralResponse:
+        """
+        @summary a
+        
+        @param request: GetWsCustomizedChGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4119,29 +5175,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_customized_ch_general(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChGeneralRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChGeneralResponse:
+        """
+        @summary a
+        
+        @param request: GetWsCustomizedChGeneralRequest
+        @return: GetWsCustomizedChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_customized_ch_general_with_options(request, runtime)
 
     async def get_ws_customized_ch_general_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChGeneralRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChGeneralResponse:
+        """
+        @summary a
+        
+        @param request: GetWsCustomizedChGeneralRequest
+        @return: GetWsCustomizedChGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_customized_ch_general_with_options_async(request, runtime)
 
     def get_ws_customized_ch_o2owith_options(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChO2ORequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChO2OResponse:
+        """
+        @param request: GetWsCustomizedChO2ORequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChO2OResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4168,14 +5241,19 @@
         )
 
     async def get_ws_customized_ch_o2owith_options_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChO2ORequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedChO2OResponse:
+        """
+        @param request: GetWsCustomizedChO2ORequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedChO2OResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.out_type):
             body['OutType'] = request.out_type
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4201,29 +5279,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_customized_ch_o2o(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChO2ORequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChO2OResponse:
+        """
+        @param request: GetWsCustomizedChO2ORequest
+        @return: GetWsCustomizedChO2OResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_customized_ch_o2owith_options(request, runtime)
 
     async def get_ws_customized_ch_o2o_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedChO2ORequest,
     ) -> alinlp_20200629_models.GetWsCustomizedChO2OResponse:
+        """
+        @param request: GetWsCustomizedChO2ORequest
+        @return: GetWsCustomizedChO2OResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_customized_ch_o2owith_options_async(request, runtime)
 
     def get_ws_customized_sea_ecom_with_options(
         self,
         request: alinlp_20200629_models.GetWsCustomizedSeaEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedSeaEcomResponse:
+        """
+        @param request: GetWsCustomizedSeaEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedSeaEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4248,14 +5339,19 @@
         )
 
     async def get_ws_customized_sea_ecom_with_options_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedSeaEcomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedSeaEcomResponse:
+        """
+        @param request: GetWsCustomizedSeaEcomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedSeaEcomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4279,29 +5375,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_customized_sea_ecom(
         self,
         request: alinlp_20200629_models.GetWsCustomizedSeaEcomRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedSeaEcomResponse:
+        """
+        @param request: GetWsCustomizedSeaEcomRequest
+        @return: GetWsCustomizedSeaEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_customized_sea_ecom_with_options(request, runtime)
 
     async def get_ws_customized_sea_ecom_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedSeaEcomRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedSeaEcomResponse:
+        """
+        @param request: GetWsCustomizedSeaEcomRequest
+        @return: GetWsCustomizedSeaEcomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_customized_sea_ecom_with_options_async(request, runtime)
 
     def get_ws_customized_sea_general_with_options(
         self,
         request: alinlp_20200629_models.GetWsCustomizedSeaGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedSeaGeneralResponse:
+        """
+        @param request: GetWsCustomizedSeaGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedSeaGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4326,14 +5435,19 @@
         )
 
     async def get_ws_customized_sea_general_with_options_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedSeaGeneralRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.GetWsCustomizedSeaGeneralResponse:
+        """
+        @param request: GetWsCustomizedSeaGeneralRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetWsCustomizedSeaGeneralResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.language):
             body['Language'] = request.language
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         if not UtilClient.is_unset(request.text):
@@ -4357,29 +5471,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_ws_customized_sea_general(
         self,
         request: alinlp_20200629_models.GetWsCustomizedSeaGeneralRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedSeaGeneralResponse:
+        """
+        @param request: GetWsCustomizedSeaGeneralRequest
+        @return: GetWsCustomizedSeaGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_ws_customized_sea_general_with_options(request, runtime)
 
     async def get_ws_customized_sea_general_async(
         self,
         request: alinlp_20200629_models.GetWsCustomizedSeaGeneralRequest,
     ) -> alinlp_20200629_models.GetWsCustomizedSeaGeneralResponse:
+        """
+        @param request: GetWsCustomizedSeaGeneralRequest
+        @return: GetWsCustomizedSeaGeneralResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_ws_customized_sea_general_with_options_async(request, runtime)
 
     def import_service_data_with_options(
         self,
         tmp_req: alinlp_20200629_models.ImportServiceDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ImportServiceDataResponse:
+        """
+        @summary 导入服务数据
+        
+        @param tmp_req: ImportServiceDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ImportServiceDataResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.ImportServiceDataShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.partition):
             request.partition_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.partition, 'Partition', 'json')
         body = {}
         if not UtilClient.is_unset(request.partition_shrink):
@@ -4410,14 +5539,21 @@
         )
 
     async def import_service_data_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.ImportServiceDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ImportServiceDataResponse:
+        """
+        @summary 导入服务数据
+        
+        @param tmp_req: ImportServiceDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ImportServiceDataResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.ImportServiceDataShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.partition):
             request.partition_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.partition, 'Partition', 'json')
         body = {}
         if not UtilClient.is_unset(request.partition_shrink):
@@ -4447,29 +5583,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def import_service_data(
         self,
         request: alinlp_20200629_models.ImportServiceDataRequest,
     ) -> alinlp_20200629_models.ImportServiceDataResponse:
+        """
+        @summary 导入服务数据
+        
+        @param request: ImportServiceDataRequest
+        @return: ImportServiceDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.import_service_data_with_options(request, runtime)
 
     async def import_service_data_async(
         self,
         request: alinlp_20200629_models.ImportServiceDataRequest,
     ) -> alinlp_20200629_models.ImportServiceDataResponse:
+        """
+        @summary 导入服务数据
+        
+        @param request: ImportServiceDataRequest
+        @return: ImportServiceDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.import_service_data_with_options_async(request, runtime)
 
     def import_service_data_v2with_options(
         self,
         tmp_req: alinlp_20200629_models.ImportServiceDataV2Request,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ImportServiceDataV2Response:
+        """
+        @summary 导入服务数据V2
+        
+        @param tmp_req: ImportServiceDataV2Request
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ImportServiceDataV2Response
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.ImportServiceDataV2ShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.documents):
             request.documents_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.documents, 'Documents', 'json')
         body = {}
         if not UtilClient.is_unset(request.data_type):
@@ -4498,14 +5653,21 @@
         )
 
     async def import_service_data_v2with_options_async(
         self,
         tmp_req: alinlp_20200629_models.ImportServiceDataV2Request,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.ImportServiceDataV2Response:
+        """
+        @summary 导入服务数据V2
+        
+        @param tmp_req: ImportServiceDataV2Request
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ImportServiceDataV2Response
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.ImportServiceDataV2ShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.documents):
             request.documents_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.documents, 'Documents', 'json')
         body = {}
         if not UtilClient.is_unset(request.data_type):
@@ -4533,29 +5695,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def import_service_data_v2(
         self,
         request: alinlp_20200629_models.ImportServiceDataV2Request,
     ) -> alinlp_20200629_models.ImportServiceDataV2Response:
+        """
+        @summary 导入服务数据V2
+        
+        @param request: ImportServiceDataV2Request
+        @return: ImportServiceDataV2Response
+        """
         runtime = util_models.RuntimeOptions()
         return self.import_service_data_v2with_options(request, runtime)
 
     async def import_service_data_v2_async(
         self,
         request: alinlp_20200629_models.ImportServiceDataV2Request,
     ) -> alinlp_20200629_models.ImportServiceDataV2Response:
+        """
+        @summary 导入服务数据V2
+        
+        @param request: ImportServiceDataV2Request
+        @return: ImportServiceDataV2Response
+        """
         runtime = util_models.RuntimeOptions()
         return await self.import_service_data_v2with_options_async(request, runtime)
 
     def insert_custom_with_options(
         self,
         request: alinlp_20200629_models.InsertCustomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.InsertCustomResponse:
+        """
+        @param request: InsertCustomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: InsertCustomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.api_id):
             body['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.custom_file_name):
             body['CustomFileName'] = request.custom_file_name
         if not UtilClient.is_unset(request.custom_url):
@@ -4586,14 +5765,19 @@
         )
 
     async def insert_custom_with_options_async(
         self,
         request: alinlp_20200629_models.InsertCustomRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.InsertCustomResponse:
+        """
+        @param request: InsertCustomRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: InsertCustomResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.api_id):
             body['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.custom_file_name):
             body['CustomFileName'] = request.custom_file_name
         if not UtilClient.is_unset(request.custom_url):
@@ -4623,28 +5807,41 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def insert_custom(
         self,
         request: alinlp_20200629_models.InsertCustomRequest,
     ) -> alinlp_20200629_models.InsertCustomResponse:
+        """
+        @param request: InsertCustomRequest
+        @return: InsertCustomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.insert_custom_with_options(request, runtime)
 
     async def insert_custom_async(
         self,
         request: alinlp_20200629_models.InsertCustomRequest,
     ) -> alinlp_20200629_models.InsertCustomResponse:
+        """
+        @param request: InsertCustomRequest
+        @return: InsertCustomResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.insert_custom_with_options_async(request, runtime)
 
     def open_alinlp_service_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.OpenAlinlpServiceResponse:
+        """
+        @param request: OpenAlinlpServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenAlinlpServiceResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='OpenAlinlpService',
             version='2020-06-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -4658,14 +5855,19 @@
             self.call_api(params, req, runtime)
         )
 
     async def open_alinlp_service_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.OpenAlinlpServiceResponse:
+        """
+        @param request: OpenAlinlpServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenAlinlpServiceResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='OpenAlinlpService',
             version='2020-06-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -4676,44 +5878,57 @@
         )
         return TeaCore.from_map(
             alinlp_20200629_models.OpenAlinlpServiceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def open_alinlp_service(self) -> alinlp_20200629_models.OpenAlinlpServiceResponse:
+        """
+        @return: OpenAlinlpServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_alinlp_service_with_options(runtime)
 
     async def open_alinlp_service_async(self) -> alinlp_20200629_models.OpenAlinlpServiceResponse:
+        """
+        @return: OpenAlinlpServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_alinlp_service_with_options_async(runtime)
 
     def post_isconv_rewriter_with_options(
         self,
         tmp_req: alinlp_20200629_models.PostISConvRewriterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostISConvRewriterResponse:
+        """
+        @summary 多轮改写
+        
+        @param tmp_req: PostISConvRewriterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostISConvRewriterResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostISConvRewriterShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input):
             request.input_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input, 'Input', 'json')
         if not UtilClient.is_unset(tmp_req.parameters):
             request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
         body = {}
         if not UtilClient.is_unset(request.algorithm):
             body['Algorithm'] = request.algorithm
         if not UtilClient.is_unset(request.debug):
             body['Debug'] = request.debug
         if not UtilClient.is_unset(request.input_shrink):
             body['Input'] = request.input_shrink
+        if not UtilClient.is_unset(request.model):
+            body['Model'] = request.model
         if not UtilClient.is_unset(request.parameters_shrink):
             body['Parameters'] = request.parameters_shrink
-        if not UtilClient.is_unset(request.version):
-            body['Version'] = request.version
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostISConvRewriter',
             version='2020-06-29',
             protocol='HTTPS',
@@ -4730,32 +5945,39 @@
         )
 
     async def post_isconv_rewriter_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.PostISConvRewriterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostISConvRewriterResponse:
+        """
+        @summary 多轮改写
+        
+        @param tmp_req: PostISConvRewriterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostISConvRewriterResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostISConvRewriterShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input):
             request.input_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input, 'Input', 'json')
         if not UtilClient.is_unset(tmp_req.parameters):
             request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
         body = {}
         if not UtilClient.is_unset(request.algorithm):
             body['Algorithm'] = request.algorithm
         if not UtilClient.is_unset(request.debug):
             body['Debug'] = request.debug
         if not UtilClient.is_unset(request.input_shrink):
             body['Input'] = request.input_shrink
+        if not UtilClient.is_unset(request.model):
+            body['Model'] = request.model
         if not UtilClient.is_unset(request.parameters_shrink):
             body['Parameters'] = request.parameters_shrink
-        if not UtilClient.is_unset(request.version):
-            body['Version'] = request.version
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostISConvRewriter',
             version='2020-06-29',
             protocol='HTTPS',
@@ -4771,29 +5993,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def post_isconv_rewriter(
         self,
         request: alinlp_20200629_models.PostISConvRewriterRequest,
     ) -> alinlp_20200629_models.PostISConvRewriterResponse:
+        """
+        @summary 多轮改写
+        
+        @param request: PostISConvRewriterRequest
+        @return: PostISConvRewriterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.post_isconv_rewriter_with_options(request, runtime)
 
     async def post_isconv_rewriter_async(
         self,
         request: alinlp_20200629_models.PostISConvRewriterRequest,
     ) -> alinlp_20200629_models.PostISConvRewriterResponse:
+        """
+        @summary 多轮改写
+        
+        @param request: PostISConvRewriterRequest
+        @return: PostISConvRewriterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.post_isconv_rewriter_with_options_async(request, runtime)
 
     def post_isretrieve_router_with_options(
         self,
         tmp_req: alinlp_20200629_models.PostISRetrieveRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostISRetrieveRouterResponse:
+        """
+        @summary 开放域搜索判定
+        
+        @param tmp_req: PostISRetrieveRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostISRetrieveRouterResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostISRetrieveRouterShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input):
             request.input_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input, 'Input', 'json')
         if not UtilClient.is_unset(tmp_req.parameters):
             request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
@@ -4803,16 +6044,16 @@
         if not UtilClient.is_unset(request.input_shrink):
             query['Input'] = request.input_shrink
         if not UtilClient.is_unset(request.parameters_shrink):
             query['Parameters'] = request.parameters_shrink
         body = {}
         if not UtilClient.is_unset(request.algorithm):
             body['Algorithm'] = request.algorithm
-        if not UtilClient.is_unset(request.version):
-            body['Version'] = request.version
+        if not UtilClient.is_unset(request.model):
+            body['Model'] = request.model
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostISRetrieveRouter',
             version='2020-06-29',
@@ -4830,14 +6071,21 @@
         )
 
     async def post_isretrieve_router_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.PostISRetrieveRouterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostISRetrieveRouterResponse:
+        """
+        @summary 开放域搜索判定
+        
+        @param tmp_req: PostISRetrieveRouterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostISRetrieveRouterResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostISRetrieveRouterShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.input):
             request.input_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.input, 'Input', 'json')
         if not UtilClient.is_unset(tmp_req.parameters):
             request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
@@ -4847,16 +6095,16 @@
         if not UtilClient.is_unset(request.input_shrink):
             query['Input'] = request.input_shrink
         if not UtilClient.is_unset(request.parameters_shrink):
             query['Parameters'] = request.parameters_shrink
         body = {}
         if not UtilClient.is_unset(request.algorithm):
             body['Algorithm'] = request.algorithm
-        if not UtilClient.is_unset(request.version):
-            body['Version'] = request.version
+        if not UtilClient.is_unset(request.model):
+            body['Model'] = request.model
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostISRetrieveRouter',
             version='2020-06-29',
@@ -4873,28 +6121,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def post_isretrieve_router(
         self,
         request: alinlp_20200629_models.PostISRetrieveRouterRequest,
     ) -> alinlp_20200629_models.PostISRetrieveRouterResponse:
+        """
+        @summary 开放域搜索判定
+        
+        @param request: PostISRetrieveRouterRequest
+        @return: PostISRetrieveRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.post_isretrieve_router_with_options(request, runtime)
 
     async def post_isretrieve_router_async(
         self,
         request: alinlp_20200629_models.PostISRetrieveRouterRequest,
     ) -> alinlp_20200629_models.PostISRetrieveRouterResponse:
+        """
+        @summary 开放域搜索判定
+        
+        @param request: PostISRetrieveRouterRequest
+        @return: PostISRetrieveRouterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.post_isretrieve_router_with_options_async(request, runtime)
 
     def post_msconv_search_token_generated_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostMSConvSearchTokenGeneratedResponse:
+        """
+        @summary 对话搜索身份凭证生成
+        
+        @param request: PostMSConvSearchTokenGeneratedRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostMSConvSearchTokenGeneratedResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='PostMSConvSearchTokenGenerated',
             version='2020-06-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -4908,14 +6175,21 @@
             self.call_api(params, req, runtime)
         )
 
     async def post_msconv_search_token_generated_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostMSConvSearchTokenGeneratedResponse:
+        """
+        @summary 对话搜索身份凭证生成
+        
+        @param request: PostMSConvSearchTokenGeneratedRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostMSConvSearchTokenGeneratedResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='PostMSConvSearchTokenGenerated',
             version='2020-06-29',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -4926,38 +6200,57 @@
         )
         return TeaCore.from_map(
             alinlp_20200629_models.PostMSConvSearchTokenGeneratedResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def post_msconv_search_token_generated(self) -> alinlp_20200629_models.PostMSConvSearchTokenGeneratedResponse:
+        """
+        @summary 对话搜索身份凭证生成
+        
+        @return: PostMSConvSearchTokenGeneratedResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.post_msconv_search_token_generated_with_options(runtime)
 
     async def post_msconv_search_token_generated_async(self) -> alinlp_20200629_models.PostMSConvSearchTokenGeneratedResponse:
+        """
+        @summary 对话搜索身份凭证生成
+        
+        @return: PostMSConvSearchTokenGeneratedResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.post_msconv_search_token_generated_with_options_async(runtime)
 
     def post_msdata_processing_count_with_options(
         self,
         tmp_req: alinlp_20200629_models.PostMSDataProcessingCountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostMSDataProcessingCountResponse:
+        """
+        @summary 数据处理进度查询
+        
+        @param tmp_req: PostMSDataProcessingCountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostMSDataProcessingCountResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostMSDataProcessingCountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.data_ids):
             request.data_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.data_ids, 'DataIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.data_ids_shrink):
             body['DataIds'] = request.data_ids_shrink
         if not UtilClient.is_unset(request.data_import_id):
             body['DataImportId'] = request.data_import_id
         if not UtilClient.is_unset(request.service_id):
             body['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.x_dash_scope_open_apisource):
+            body['X-DashScope-OpenAPISource'] = request.x_dash_scope_open_apisource
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostMSDataProcessingCount',
             version='2020-06-29',
             protocol='HTTPS',
@@ -4974,26 +6267,35 @@
         )
 
     async def post_msdata_processing_count_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.PostMSDataProcessingCountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostMSDataProcessingCountResponse:
+        """
+        @summary 数据处理进度查询
+        
+        @param tmp_req: PostMSDataProcessingCountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostMSDataProcessingCountResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostMSDataProcessingCountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.data_ids):
             request.data_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.data_ids, 'DataIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.data_ids_shrink):
             body['DataIds'] = request.data_ids_shrink
         if not UtilClient.is_unset(request.data_import_id):
             body['DataImportId'] = request.data_import_id
         if not UtilClient.is_unset(request.service_id):
             body['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.x_dash_scope_open_apisource):
+            body['X-DashScope-OpenAPISource'] = request.x_dash_scope_open_apisource
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostMSDataProcessingCount',
             version='2020-06-29',
             protocol='HTTPS',
@@ -5009,29 +6311,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def post_msdata_processing_count(
         self,
         request: alinlp_20200629_models.PostMSDataProcessingCountRequest,
     ) -> alinlp_20200629_models.PostMSDataProcessingCountResponse:
+        """
+        @summary 数据处理进度查询
+        
+        @param request: PostMSDataProcessingCountRequest
+        @return: PostMSDataProcessingCountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.post_msdata_processing_count_with_options(request, runtime)
 
     async def post_msdata_processing_count_async(
         self,
         request: alinlp_20200629_models.PostMSDataProcessingCountRequest,
     ) -> alinlp_20200629_models.PostMSDataProcessingCountResponse:
+        """
+        @summary 数据处理进度查询
+        
+        @param request: PostMSDataProcessingCountRequest
+        @return: PostMSDataProcessingCountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.post_msdata_processing_count_with_options_async(request, runtime)
 
     def post_mssearch_enhance_with_options(
         self,
         tmp_req: alinlp_20200629_models.PostMSSearchEnhanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostMSSearchEnhanceResponse:
+        """
+        @summary 搜索增强
+        
+        @param tmp_req: PostMSSearchEnhanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostMSSearchEnhanceResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostMSSearchEnhanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.custom_config_info):
             request.custom_config_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.custom_config_info, 'CustomConfigInfo', 'json')
         if not UtilClient.is_unset(tmp_req.fields):
             request.fields_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.fields, 'Fields', 'json')
@@ -5064,14 +6385,16 @@
             body['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.sort_shrink):
             body['Sort'] = request.sort_shrink
         if not UtilClient.is_unset(request.type):
             body['Type'] = request.type
         if not UtilClient.is_unset(request.uq):
             body['Uq'] = request.uq
+        if not UtilClient.is_unset(request.x_dash_scope_open_apisource):
+            body['X-DashScope-OpenAPISource'] = request.x_dash_scope_open_apisource
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostMSSearchEnhance',
             version='2020-06-29',
             protocol='HTTPS',
@@ -5088,14 +6411,21 @@
         )
 
     async def post_mssearch_enhance_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.PostMSSearchEnhanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostMSSearchEnhanceResponse:
+        """
+        @summary 搜索增强
+        
+        @param tmp_req: PostMSSearchEnhanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostMSSearchEnhanceResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostMSSearchEnhanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.custom_config_info):
             request.custom_config_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.custom_config_info, 'CustomConfigInfo', 'json')
         if not UtilClient.is_unset(tmp_req.fields):
             request.fields_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.fields, 'Fields', 'json')
@@ -5128,14 +6458,16 @@
             body['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.sort_shrink):
             body['Sort'] = request.sort_shrink
         if not UtilClient.is_unset(request.type):
             body['Type'] = request.type
         if not UtilClient.is_unset(request.uq):
             body['Uq'] = request.uq
+        if not UtilClient.is_unset(request.x_dash_scope_open_apisource):
+            body['X-DashScope-OpenAPISource'] = request.x_dash_scope_open_apisource
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='PostMSSearchEnhance',
             version='2020-06-29',
             protocol='HTTPS',
@@ -5151,29 +6483,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def post_mssearch_enhance(
         self,
         request: alinlp_20200629_models.PostMSSearchEnhanceRequest,
     ) -> alinlp_20200629_models.PostMSSearchEnhanceResponse:
+        """
+        @summary 搜索增强
+        
+        @param request: PostMSSearchEnhanceRequest
+        @return: PostMSSearchEnhanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.post_mssearch_enhance_with_options(request, runtime)
 
     async def post_mssearch_enhance_async(
         self,
         request: alinlp_20200629_models.PostMSSearchEnhanceRequest,
     ) -> alinlp_20200629_models.PostMSSearchEnhanceResponse:
+        """
+        @summary 搜索增强
+        
+        @param request: PostMSSearchEnhanceRequest
+        @return: PostMSSearchEnhanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.post_mssearch_enhance_with_options_async(request, runtime)
 
     def post_msservice_data_import_with_options(
         self,
         tmp_req: alinlp_20200629_models.PostMSServiceDataImportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostMSServiceDataImportResponse:
+        """
+        @summary 导入服务数据V2
+        
+        @param tmp_req: PostMSServiceDataImportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostMSServiceDataImportResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostMSServiceDataImportShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.documents):
             request.documents_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.documents, 'Documents', 'json')
         body = {}
         if not UtilClient.is_unset(request.data_type):
@@ -5202,14 +6553,21 @@
         )
 
     async def post_msservice_data_import_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.PostMSServiceDataImportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.PostMSServiceDataImportResponse:
+        """
+        @summary 导入服务数据V2
+        
+        @param tmp_req: PostMSServiceDataImportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PostMSServiceDataImportResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.PostMSServiceDataImportShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.documents):
             request.documents_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.documents, 'Documents', 'json')
         body = {}
         if not UtilClient.is_unset(request.data_type):
@@ -5237,29 +6595,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def post_msservice_data_import(
         self,
         request: alinlp_20200629_models.PostMSServiceDataImportRequest,
     ) -> alinlp_20200629_models.PostMSServiceDataImportResponse:
+        """
+        @summary 导入服务数据V2
+        
+        @param request: PostMSServiceDataImportRequest
+        @return: PostMSServiceDataImportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.post_msservice_data_import_with_options(request, runtime)
 
     async def post_msservice_data_import_async(
         self,
         request: alinlp_20200629_models.PostMSServiceDataImportRequest,
     ) -> alinlp_20200629_models.PostMSServiceDataImportResponse:
+        """
+        @summary 导入服务数据V2
+        
+        @param request: PostMSServiceDataImportRequest
+        @return: PostMSServiceDataImportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.post_msservice_data_import_with_options_async(request, runtime)
 
     def request_table_qawith_options(
         self,
         request: alinlp_20200629_models.RequestTableQARequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.RequestTableQAResponse:
+        """
+        @param request: RequestTableQARequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RequestTableQAResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -5282,14 +6657,19 @@
         )
 
     async def request_table_qawith_options_async(
         self,
         request: alinlp_20200629_models.RequestTableQARequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.RequestTableQAResponse:
+        """
+        @param request: RequestTableQARequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RequestTableQAResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.service_code):
             body['ServiceCode'] = request.service_code
         req = open_api_models.OpenApiRequest(
@@ -5311,29 +6691,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def request_table_qa(
         self,
         request: alinlp_20200629_models.RequestTableQARequest,
     ) -> alinlp_20200629_models.RequestTableQAResponse:
+        """
+        @param request: RequestTableQARequest
+        @return: RequestTableQAResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.request_table_qawith_options(request, runtime)
 
     async def request_table_qa_async(
         self,
         request: alinlp_20200629_models.RequestTableQARequest,
     ) -> alinlp_20200629_models.RequestTableQAResponse:
+        """
+        @param request: RequestTableQARequest
+        @return: RequestTableQAResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.request_table_qawith_options_async(request, runtime)
 
     def request_table_qaonline_with_options(
         self,
         request: alinlp_20200629_models.RequestTableQAOnlineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.RequestTableQAOnlineResponse:
+        """
+        @summary 表格问答在线接口
+        
+        @param request: RequestTableQAOnlineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RequestTableQAOnlineResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.bot_id):
             body['BotId'] = request.bot_id
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.question):
@@ -5360,14 +6755,21 @@
         )
 
     async def request_table_qaonline_with_options_async(
         self,
         request: alinlp_20200629_models.RequestTableQAOnlineRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.RequestTableQAOnlineResponse:
+        """
+        @summary 表格问答在线接口
+        
+        @param request: RequestTableQAOnlineRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RequestTableQAOnlineResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.bot_id):
             body['BotId'] = request.bot_id
         if not UtilClient.is_unset(request.params):
             body['Params'] = request.params
         if not UtilClient.is_unset(request.question):
@@ -5393,29 +6795,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def request_table_qaonline(
         self,
         request: alinlp_20200629_models.RequestTableQAOnlineRequest,
     ) -> alinlp_20200629_models.RequestTableQAOnlineResponse:
+        """
+        @summary 表格问答在线接口
+        
+        @param request: RequestTableQAOnlineRequest
+        @return: RequestTableQAOnlineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.request_table_qaonline_with_options(request, runtime)
 
     async def request_table_qaonline_async(
         self,
         request: alinlp_20200629_models.RequestTableQAOnlineRequest,
     ) -> alinlp_20200629_models.RequestTableQAOnlineResponse:
+        """
+        @summary 表格问答在线接口
+        
+        @param request: RequestTableQAOnlineRequest
+        @return: RequestTableQAOnlineResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.request_table_qaonline_with_options_async(request, runtime)
 
     def update_service_data_with_options(
         self,
         tmp_req: alinlp_20200629_models.UpdateServiceDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.UpdateServiceDataResponse:
+        """
+        @summary 更新服务数据
+        
+        @param tmp_req: UpdateServiceDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateServiceDataResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.UpdateServiceDataShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.conditions):
             request.conditions_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.conditions, 'Conditions', 'json')
         body = {}
         if not UtilClient.is_unset(request.conditions_shrink):
@@ -5442,14 +6863,21 @@
         )
 
     async def update_service_data_with_options_async(
         self,
         tmp_req: alinlp_20200629_models.UpdateServiceDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alinlp_20200629_models.UpdateServiceDataResponse:
+        """
+        @summary 更新服务数据
+        
+        @param tmp_req: UpdateServiceDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateServiceDataResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = alinlp_20200629_models.UpdateServiceDataShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.conditions):
             request.conditions_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.conditions, 'Conditions', 'json')
         body = {}
         if not UtilClient.is_unset(request.conditions_shrink):
@@ -5475,16 +6903,28 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_service_data(
         self,
         request: alinlp_20200629_models.UpdateServiceDataRequest,
     ) -> alinlp_20200629_models.UpdateServiceDataResponse:
+        """
+        @summary 更新服务数据
+        
+        @param request: UpdateServiceDataRequest
+        @return: UpdateServiceDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_service_data_with_options(request, runtime)
 
     async def update_service_data_async(
         self,
         request: alinlp_20200629_models.UpdateServiceDataRequest,
     ) -> alinlp_20200629_models.UpdateServiceDataResponse:
+        """
+        @summary 更新服务数据
+        
+        @param request: UpdateServiceDataRequest
+        @return: UpdateServiceDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_service_data_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629/models.py` & `alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -478,72 +478,88 @@
 
 
 class DeleteServiceDataByConditionsRequest(TeaModel):
     def __init__(
         self,
         conditions: Dict[str, Any] = None,
         service_id: int = None,
+        x_dash_scope_open_apisource: str = None,
     ):
+        # This parameter is required.
         self.conditions = conditions
+        # This parameter is required.
         self.service_id = service_id
+        self.x_dash_scope_open_apisource = x_dash_scope_open_apisource
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.conditions is not None:
             result['Conditions'] = self.conditions
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
+        if self.x_dash_scope_open_apisource is not None:
+            result['X-DashScope-OpenAPISource'] = self.x_dash_scope_open_apisource
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Conditions') is not None:
             self.conditions = m.get('Conditions')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
+        if m.get('X-DashScope-OpenAPISource') is not None:
+            self.x_dash_scope_open_apisource = m.get('X-DashScope-OpenAPISource')
         return self
 
 
 class DeleteServiceDataByConditionsShrinkRequest(TeaModel):
     def __init__(
         self,
         conditions_shrink: str = None,
         service_id: int = None,
+        x_dash_scope_open_apisource: str = None,
     ):
+        # This parameter is required.
         self.conditions_shrink = conditions_shrink
+        # This parameter is required.
         self.service_id = service_id
+        self.x_dash_scope_open_apisource = x_dash_scope_open_apisource
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.conditions_shrink is not None:
             result['Conditions'] = self.conditions_shrink
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
+        if self.x_dash_scope_open_apisource is not None:
+            result['X-DashScope-OpenAPISource'] = self.x_dash_scope_open_apisource
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Conditions') is not None:
             self.conditions_shrink = m.get('Conditions')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
+        if m.get('X-DashScope-OpenAPISource') is not None:
+            self.x_dash_scope_open_apisource = m.get('X-DashScope-OpenAPISource')
         return self
 
 
 class DeleteServiceDataByConditionsResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -637,15 +653,17 @@
 
 class DeleteServiceDataByIdsRequest(TeaModel):
     def __init__(
         self,
         ids: List[str] = None,
         service_id: int = None,
     ):
+        # This parameter is required.
         self.ids = ids
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -670,15 +688,17 @@
 
 class DeleteServiceDataByIdsShrinkRequest(TeaModel):
     def __init__(
         self,
         ids_shrink: str = None,
         service_id: int = None,
     ):
+        # This parameter is required.
         self.ids_shrink = ids_shrink
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -797,14 +817,15 @@
     def __init__(
         self,
         image_url: str = None,
         service_code: str = None,
         text: str = None,
     ):
         self.image_url = image_url
+        # This parameter is required.
         self.service_code = service_code
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -910,15 +931,17 @@
     def __init__(
         self,
         image_url: str = None,
         service_code: str = None,
         text: str = None,
     ):
         self.image_url = image_url
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1022,16 +1045,19 @@
 class GetCheckDuplicationChMedicalRequest(TeaModel):
     def __init__(
         self,
         origin_q: str = None,
         origin_t: str = None,
         service_code: str = None,
     ):
+        # This parameter is required.
         self.origin_q = origin_q
+        # This parameter is required.
         self.origin_t = origin_t
+        # This parameter is required.
         self.service_code = service_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1134,15 +1160,17 @@
 
 class GetDiagnosisChMedicalRequest(TeaModel):
     def __init__(
         self,
         name: str = None,
         service_code: str = None,
     ):
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.service_code = service_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1241,15 +1269,17 @@
 
 class GetDpChEcomRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1348,15 +1378,17 @@
 
 class GetDpChGeneralCTBRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1455,15 +1487,17 @@
 
 class GetDpChGeneralStanfordRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1562,15 +1596,17 @@
 
 class GetEcChGeneralRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1669,15 +1705,17 @@
 
 class GetEcEnGeneralRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1777,14 +1815,15 @@
 class GetEmbeddingRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
         text_type: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
         self.text = text
         self.text_type = text_type
 
     def validate(self):
         pass
 
@@ -1891,15 +1930,17 @@
     def __init__(
         self,
         image_url: str = None,
         service_code: str = None,
         text: str = None,
     ):
         self.image_url = image_url
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2004,15 +2045,17 @@
     def __init__(
         self,
         api_version: str = None,
         service_code: str = None,
         text: str = None,
     ):
         self.api_version = api_version
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2115,15 +2158,17 @@
 
 class GetKeywordEnEcomRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2226,15 +2271,17 @@
         factory: str = None,
         name: str = None,
         service_code: str = None,
         specification: str = None,
         unit: str = None,
     ):
         self.factory = factory
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.service_code = service_code
         self.specification = specification
         self.unit = unit
 
     def validate(self):
         pass
 
@@ -2349,15 +2396,17 @@
     def __init__(
         self,
         lexer_id: str = None,
         service_code: str = None,
         text: str = None,
     ):
         self.lexer_id = lexer_id
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2460,15 +2509,17 @@
 
 class GetNerChMedicalRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2569,15 +2620,17 @@
     def __init__(
         self,
         lexer_id: str = None,
         service_code: str = None,
         text: str = None,
     ):
         self.lexer_id = lexer_id
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2681,16 +2734,19 @@
 class GetNerCustomizedSeaEcomRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.language = language
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2799,14 +2855,15 @@
         sentence: str = None,
         service_code: str = None,
         task: str = None,
     ):
         self.examples = examples
         self.labels = labels
         self.sentence = sentence
+        # This parameter is required.
         self.service_code = service_code
         self.task = task
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2924,14 +2981,15 @@
         sentence: str = None,
         service_code: str = None,
         task: str = None,
     ):
         self.examples = examples
         self.labels = labels
         self.sentence = sentence
+        # This parameter is required.
         self.service_code = service_code
         self.task = task
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3043,15 +3101,17 @@
 
 class GetOperationChMedicalRequest(TeaModel):
     def __init__(
         self,
         name: str = None,
         service_code: str = None,
     ):
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.service_code = service_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3153,15 +3213,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3272,15 +3334,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3388,15 +3452,17 @@
 
 class GetPriceChEcomRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3602,15 +3668,17 @@
 
 class GetSaChGeneralRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3710,16 +3778,19 @@
 class GetSaSeaEcomRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.language = language
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3821,14 +3892,15 @@
 
 
 class GetServiceDataImportStatusRequest(TeaModel):
     def __init__(
         self,
         data_import_ids: List[int] = None,
     ):
+        # This parameter is required.
         self.data_import_ids = data_import_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3848,14 +3920,15 @@
 
 
 class GetServiceDataImportStatusShrinkRequest(TeaModel):
     def __init__(
         self,
         data_import_ids_shrink: str = None,
     ):
+        # This parameter is required.
         self.data_import_ids_shrink = data_import_ids_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3977,16 +4050,19 @@
 class GetSimilarityChMedicalRequest(TeaModel):
     def __init__(
         self,
         origin_q: str = None,
         origin_t: str = None,
         service_code: str = None,
     ):
+        # This parameter is required.
         self.origin_q = origin_q
+        # This parameter is required.
         self.origin_t = origin_t
+        # This parameter is required.
         self.service_code = service_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4089,15 +4165,17 @@
 
 class GetSummaryChEcomRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4303,15 +4381,17 @@
 
 class GetTcChEcomRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4410,15 +4490,17 @@
 
 class GetTcChGeneralRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4519,17 +4601,21 @@
     def __init__(
         self,
         origin_q: str = None,
         origin_t: str = None,
         service_code: str = None,
         type: str = None,
     ):
+        # This parameter is required.
         self.origin_q = origin_q
+        # This parameter is required.
         self.origin_t = origin_t
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4635,14 +4721,15 @@
 
 
 class GetUserUploadSignRequest(TeaModel):
     def __init__(
         self,
         service_code: str = None,
     ):
+        # This parameter is required.
         self.service_code = service_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4742,17 +4829,20 @@
         service_code: str = None,
         size: str = None,
         text: str = None,
         tokenizer_id: str = None,
         type: str = None,
     ):
         self.operation = operation
+        # This parameter is required.
         self.service_code = service_code
         self.size = size
+        # This parameter is required.
         self.text = text
+        # This parameter is required.
         self.tokenizer_id = tokenizer_id
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4873,17 +4963,20 @@
         service_code: str = None,
         size: str = None,
         text: str = None,
         tokenizer_id: str = None,
         type: str = None,
     ):
         self.operation = operation
+        # This parameter is required.
         self.service_code = service_code
         self.size = size
+        # This parameter is required.
         self.text = text
+        # This parameter is required.
         self.tokenizer_id = tokenizer_id
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5004,17 +5097,20 @@
         service_code: str = None,
         size: str = None,
         text: str = None,
         tokenizer_id: str = None,
         type: str = None,
     ):
         self.operation = operation
+        # This parameter is required.
         self.service_code = service_code
         self.size = size
+        # This parameter is required.
         self.text = text
+        # This parameter is required.
         self.tokenizer_id = tokenizer_id
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5134,16 +5230,18 @@
         operation: str = None,
         service_code: str = None,
         size: str = None,
         text: str = None,
         type: str = None,
     ):
         self.operation = operation
+        # This parameter is required.
         self.service_code = service_code
         self.size = size
+        # This parameter is required.
         self.text = text
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5260,17 +5358,20 @@
         service_code: str = None,
         size: str = None,
         text: str = None,
         tokenizer_id: str = None,
         type: str = None,
     ):
         self.operation = operation
+        # This parameter is required.
         self.service_code = service_code
         self.size = size
+        # This parameter is required.
         self.text = text
+        # This parameter is required.
         self.tokenizer_id = tokenizer_id
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5389,15 +5490,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5508,15 +5611,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5627,15 +5732,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5746,15 +5853,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5865,15 +5974,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5984,15 +6095,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6103,15 +6216,17 @@
         self,
         out_type: str = None,
         service_code: str = None,
         text: str = None,
         tokenizer_id: str = None,
     ):
         self.out_type = out_type
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
         self.tokenizer_id = tokenizer_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6220,16 +6335,19 @@
 class GetWsCustomizedSeaEcomRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.language = language
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6333,16 +6451,19 @@
 class GetWsCustomizedSeaGeneralRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         service_code: str = None,
         text: str = None,
     ):
+        # This parameter is required.
         self.language = language
+        # This parameter is required.
         self.service_code = service_code
+        # This parameter is required.
         self.text = text
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6448,14 +6569,15 @@
         self,
         partition: List[Dict[str, str]] = None,
         service_id: int = None,
         sub_path: str = None,
         url: str = None,
     ):
         self.partition = partition
+        # This parameter is required.
         self.service_id = service_id
         self.sub_path = sub_path
         self.url = url
 
     def validate(self):
         pass
 
@@ -6493,14 +6615,15 @@
         self,
         partition_shrink: str = None,
         service_id: int = None,
         sub_path: str = None,
         url: str = None,
     ):
         self.partition_shrink = partition_shrink
+        # This parameter is required.
         self.service_id = service_id
         self.sub_path = sub_path
         self.url = url
 
     def validate(self):
         pass
 
@@ -6687,14 +6810,15 @@
         self,
         data_type: str = None,
         documents: List[ImportServiceDataV2RequestDocuments] = None,
         service_id: int = None,
     ):
         self.data_type = data_type
         self.documents = documents
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         if self.documents:
             for k in self.documents:
                 if k:
                     k.validate()
@@ -6734,14 +6858,15 @@
         self,
         data_type: str = None,
         documents_shrink: str = None,
         service_id: int = None,
     ):
         self.data_type = data_type
         self.documents_shrink = documents_shrink
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6866,19 +6991,21 @@
         api_id: int = None,
         custom_file_name: str = None,
         custom_url: str = None,
         reg_file_name: str = None,
         reg_url: str = None,
         service_code: str = None,
     ):
+        # This parameter is required.
         self.api_id = api_id
         self.custom_file_name = custom_file_name
         self.custom_url = custom_url
         self.reg_file_name = reg_file_name
         self.reg_url = reg_url
+        # This parameter is required.
         self.service_code = service_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7067,22 +7194,22 @@
 
 class PostISConvRewriterRequest(TeaModel):
     def __init__(
         self,
         algorithm: str = None,
         debug: bool = None,
         input: Dict[str, Any] = None,
+        model: str = None,
         parameters: Dict[str, Any] = None,
-        version: str = None,
     ):
         self.algorithm = algorithm
         self.debug = debug
         self.input = input
+        self.model = model
         self.parameters = parameters
-        self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7091,49 +7218,49 @@
         result = dict()
         if self.algorithm is not None:
             result['Algorithm'] = self.algorithm
         if self.debug is not None:
             result['Debug'] = self.debug
         if self.input is not None:
             result['Input'] = self.input
+        if self.model is not None:
+            result['Model'] = self.model
         if self.parameters is not None:
             result['Parameters'] = self.parameters
-        if self.version is not None:
-            result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Algorithm') is not None:
             self.algorithm = m.get('Algorithm')
         if m.get('Debug') is not None:
             self.debug = m.get('Debug')
         if m.get('Input') is not None:
             self.input = m.get('Input')
+        if m.get('Model') is not None:
+            self.model = m.get('Model')
         if m.get('Parameters') is not None:
             self.parameters = m.get('Parameters')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
         return self
 
 
 class PostISConvRewriterShrinkRequest(TeaModel):
     def __init__(
         self,
         algorithm: str = None,
         debug: bool = None,
         input_shrink: str = None,
+        model: str = None,
         parameters_shrink: str = None,
-        version: str = None,
     ):
         self.algorithm = algorithm
         self.debug = debug
         self.input_shrink = input_shrink
+        self.model = model
         self.parameters_shrink = parameters_shrink
-        self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7142,32 +7269,32 @@
         result = dict()
         if self.algorithm is not None:
             result['Algorithm'] = self.algorithm
         if self.debug is not None:
             result['Debug'] = self.debug
         if self.input_shrink is not None:
             result['Input'] = self.input_shrink
+        if self.model is not None:
+            result['Model'] = self.model
         if self.parameters_shrink is not None:
             result['Parameters'] = self.parameters_shrink
-        if self.version is not None:
-            result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Algorithm') is not None:
             self.algorithm = m.get('Algorithm')
         if m.get('Debug') is not None:
             self.debug = m.get('Debug')
         if m.get('Input') is not None:
             self.input_shrink = m.get('Input')
+        if m.get('Model') is not None:
+            self.model = m.get('Model')
         if m.get('Parameters') is not None:
             self.parameters_shrink = m.get('Parameters')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
         return self
 
 
 class PostISConvRewriterResponseBody(TeaModel):
     def __init__(
         self,
         data: Dict[str, Any] = None,
@@ -7261,22 +7388,22 @@
 
 class PostISRetrieveRouterRequest(TeaModel):
     def __init__(
         self,
         algorithm: str = None,
         debug: bool = None,
         input: Dict[str, Any] = None,
+        model: str = None,
         parameters: Dict[str, Any] = None,
-        version: str = None,
     ):
         self.algorithm = algorithm
         self.debug = debug
         self.input = input
+        self.model = model
         self.parameters = parameters
-        self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7285,49 +7412,49 @@
         result = dict()
         if self.algorithm is not None:
             result['Algorithm'] = self.algorithm
         if self.debug is not None:
             result['Debug'] = self.debug
         if self.input is not None:
             result['Input'] = self.input
+        if self.model is not None:
+            result['Model'] = self.model
         if self.parameters is not None:
             result['Parameters'] = self.parameters
-        if self.version is not None:
-            result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Algorithm') is not None:
             self.algorithm = m.get('Algorithm')
         if m.get('Debug') is not None:
             self.debug = m.get('Debug')
         if m.get('Input') is not None:
             self.input = m.get('Input')
+        if m.get('Model') is not None:
+            self.model = m.get('Model')
         if m.get('Parameters') is not None:
             self.parameters = m.get('Parameters')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
         return self
 
 
 class PostISRetrieveRouterShrinkRequest(TeaModel):
     def __init__(
         self,
         algorithm: str = None,
         debug: bool = None,
         input_shrink: str = None,
+        model: str = None,
         parameters_shrink: str = None,
-        version: str = None,
     ):
         self.algorithm = algorithm
         self.debug = debug
         self.input_shrink = input_shrink
+        self.model = model
         self.parameters_shrink = parameters_shrink
-        self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7336,32 +7463,32 @@
         result = dict()
         if self.algorithm is not None:
             result['Algorithm'] = self.algorithm
         if self.debug is not None:
             result['Debug'] = self.debug
         if self.input_shrink is not None:
             result['Input'] = self.input_shrink
+        if self.model is not None:
+            result['Model'] = self.model
         if self.parameters_shrink is not None:
             result['Parameters'] = self.parameters_shrink
-        if self.version is not None:
-            result['Version'] = self.version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Algorithm') is not None:
             self.algorithm = m.get('Algorithm')
         if m.get('Debug') is not None:
             self.debug = m.get('Debug')
         if m.get('Input') is not None:
             self.input_shrink = m.get('Input')
+        if m.get('Model') is not None:
+            self.model = m.get('Model')
         if m.get('Parameters') is not None:
             self.parameters_shrink = m.get('Parameters')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
         return self
 
 
 class PostISRetrieveRouterResponseBody(TeaModel):
     def __init__(
         self,
         data: Dict[str, Any] = None,
@@ -7553,18 +7680,20 @@
 
 class PostMSDataProcessingCountRequest(TeaModel):
     def __init__(
         self,
         data_ids: List[str] = None,
         data_import_id: int = None,
         service_id: int = None,
+        x_dash_scope_open_apisource: str = None,
     ):
         self.data_ids = data_ids
         self.data_import_id = data_import_id
         self.service_id = service_id
+        self.x_dash_scope_open_apisource = x_dash_scope_open_apisource
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7573,37 +7702,43 @@
         result = dict()
         if self.data_ids is not None:
             result['DataIds'] = self.data_ids
         if self.data_import_id is not None:
             result['DataImportId'] = self.data_import_id
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
+        if self.x_dash_scope_open_apisource is not None:
+            result['X-DashScope-OpenAPISource'] = self.x_dash_scope_open_apisource
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DataIds') is not None:
             self.data_ids = m.get('DataIds')
         if m.get('DataImportId') is not None:
             self.data_import_id = m.get('DataImportId')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
+        if m.get('X-DashScope-OpenAPISource') is not None:
+            self.x_dash_scope_open_apisource = m.get('X-DashScope-OpenAPISource')
         return self
 
 
 class PostMSDataProcessingCountShrinkRequest(TeaModel):
     def __init__(
         self,
         data_ids_shrink: str = None,
         data_import_id: int = None,
         service_id: int = None,
+        x_dash_scope_open_apisource: str = None,
     ):
         self.data_ids_shrink = data_ids_shrink
         self.data_import_id = data_import_id
         self.service_id = service_id
+        self.x_dash_scope_open_apisource = x_dash_scope_open_apisource
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7612,24 +7747,28 @@
         result = dict()
         if self.data_ids_shrink is not None:
             result['DataIds'] = self.data_ids_shrink
         if self.data_import_id is not None:
             result['DataImportId'] = self.data_import_id
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
+        if self.x_dash_scope_open_apisource is not None:
+            result['X-DashScope-OpenAPISource'] = self.x_dash_scope_open_apisource
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DataIds') is not None:
             self.data_ids_shrink = m.get('DataIds')
         if m.get('DataImportId') is not None:
             self.data_import_id = m.get('DataImportId')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
+        if m.get('X-DashScope-OpenAPISource') is not None:
+            self.x_dash_scope_open_apisource = m.get('X-DashScope-OpenAPISource')
         return self
 
 
 class PostMSDataProcessingCountResponseBodyDataDataProcessedStatusesErrorDataList(TeaModel):
     def __init__(
         self,
         count: int = None,
@@ -7887,14 +8026,15 @@
         queries: str = None,
         rank_model_info: Dict[str, Any] = None,
         rows: int = None,
         service_id: int = None,
         sort: List[str] = None,
         type: str = None,
         uq: str = None,
+        x_dash_scope_open_apisource: str = None,
     ):
         self.body = body
         self.custom_config_info = custom_config_info
         self.debug = debug
         self.fields = fields
         self.filters = filters
         self.min_score = min_score
@@ -7902,14 +8042,15 @@
         self.queries = queries
         self.rank_model_info = rank_model_info
         self.rows = rows
         self.service_id = service_id
         self.sort = sort
         self.type = type
         self.uq = uq
+        self.x_dash_scope_open_apisource = x_dash_scope_open_apisource
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7940,14 +8081,16 @@
             result['ServiceId'] = self.service_id
         if self.sort is not None:
             result['Sort'] = self.sort
         if self.type is not None:
             result['Type'] = self.type
         if self.uq is not None:
             result['Uq'] = self.uq
+        if self.x_dash_scope_open_apisource is not None:
+            result['X-DashScope-OpenAPISource'] = self.x_dash_scope_open_apisource
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Body') is not None:
             self.body = m.get('Body')
         if m.get('CustomConfigInfo') is not None:
@@ -7972,14 +8115,16 @@
             self.service_id = m.get('ServiceId')
         if m.get('Sort') is not None:
             self.sort = m.get('Sort')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         if m.get('Uq') is not None:
             self.uq = m.get('Uq')
+        if m.get('X-DashScope-OpenAPISource') is not None:
+            self.x_dash_scope_open_apisource = m.get('X-DashScope-OpenAPISource')
         return self
 
 
 class PostMSSearchEnhanceShrinkRequest(TeaModel):
     def __init__(
         self,
         body: str = None,
@@ -7992,14 +8137,15 @@
         queries: str = None,
         rank_model_info_shrink: str = None,
         rows: int = None,
         service_id: int = None,
         sort_shrink: str = None,
         type: str = None,
         uq: str = None,
+        x_dash_scope_open_apisource: str = None,
     ):
         self.body = body
         self.custom_config_info_shrink = custom_config_info_shrink
         self.debug = debug
         self.fields_shrink = fields_shrink
         self.filters = filters
         self.min_score = min_score
@@ -8007,14 +8153,15 @@
         self.queries = queries
         self.rank_model_info_shrink = rank_model_info_shrink
         self.rows = rows
         self.service_id = service_id
         self.sort_shrink = sort_shrink
         self.type = type
         self.uq = uq
+        self.x_dash_scope_open_apisource = x_dash_scope_open_apisource
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -8045,14 +8192,16 @@
             result['ServiceId'] = self.service_id
         if self.sort_shrink is not None:
             result['Sort'] = self.sort_shrink
         if self.type is not None:
             result['Type'] = self.type
         if self.uq is not None:
             result['Uq'] = self.uq
+        if self.x_dash_scope_open_apisource is not None:
+            result['X-DashScope-OpenAPISource'] = self.x_dash_scope_open_apisource
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Body') is not None:
             self.body = m.get('Body')
         if m.get('CustomConfigInfo') is not None:
@@ -8077,14 +8226,16 @@
             self.service_id = m.get('ServiceId')
         if m.get('Sort') is not None:
             self.sort_shrink = m.get('Sort')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         if m.get('Uq') is not None:
             self.uq = m.get('Uq')
+        if m.get('X-DashScope-OpenAPISource') is not None:
+            self.x_dash_scope_open_apisource = m.get('X-DashScope-OpenAPISource')
         return self
 
 
 class PostMSSearchEnhanceResponseBody(TeaModel):
     def __init__(
         self,
         code: int = None,
@@ -8245,14 +8396,15 @@
         self,
         data_type: str = None,
         documents: List[PostMSServiceDataImportRequestDocuments] = None,
         service_id: int = None,
     ):
         self.data_type = data_type
         self.documents = documents
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         if self.documents:
             for k in self.documents:
                 if k:
                     k.validate()
@@ -8292,14 +8444,15 @@
         self,
         data_type: str = None,
         documents_shrink: str = None,
         service_id: int = None,
     ):
         self.data_type = data_type
         self.documents_shrink = documents_shrink
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8420,15 +8573,17 @@
 
 class RequestTableQARequest(TeaModel):
     def __init__(
         self,
         params: str = None,
         service_code: str = None,
     ):
+        # This parameter is required.
         self.params = params
+        # This parameter is required.
         self.service_code = service_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8646,15 +8801,17 @@
 
 class UpdateServiceDataRequest(TeaModel):
     def __init__(
         self,
         conditions: Dict[str, Any] = None,
         service_id: int = None,
     ):
+        # This parameter is required.
         self.conditions = conditions
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8679,15 +8836,17 @@
 
 class UpdateServiceDataShrinkRequest(TeaModel):
     def __init__(
         self,
         conditions_shrink: str = None,
         service_id: int = None,
     ):
+        # This parameter is required.
         self.conditions_shrink = conditions_shrink
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_alinlp20200629-2.8.2/alibabacloud_alinlp20200629.egg-info/PKG-INFO` & `alibabacloud_alinlp20200629-3.0.0/alibabacloud_alinlp20200629.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alinlp20200629
-Version: 2.8.2
+Version: 3.0.0
 Summary: Alibaba Cloud alinlp (20200629) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alinlp20200629-2.8.2/setup.py` & `alibabacloud_alinlp20200629-3.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alinlp20200629.
 
-Created on 10/04/2024
+Created on 20/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alinlp20200629"
 NAME = "alibabacloud_alinlp20200629" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud alinlp (20200629) SDK Library for Python"
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


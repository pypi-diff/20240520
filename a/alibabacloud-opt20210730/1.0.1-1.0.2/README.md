# Comparing `tmp/alibabacloud_opt20210730-1.0.1.tar.gz` & `tmp/alibabacloud_opt20210730-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_opt20210730-1.0.1.tar", last modified: Fri Apr 12 17:11:50 2024, max compression
+gzip compressed data, was "dist/alibabacloud_opt20210730-1.0.2.tar", last modified: Mon May 20 17:16:52 2024, max compression
```

## Comparing `alibabacloud_opt20210730-1.0.1.tar` & `alibabacloud_opt20210730-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9175 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/client.py
--rw-r--r--   0 root         (0) root         (0)    12810 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:16:52.000000 alibabacloud_opt20210730-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-20 17:16:52.000000 alibabacloud_opt20210730-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:16:52.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11039 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730/client.py
+-rw-r--r--   0 root         (0) root         (0)    13279 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:16:52.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 17:16:52.000000 alibabacloud_opt20210730-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-20 17:16:51.000000 alibabacloud_opt20210730-1.0.2/setup.py
```

### Comparing `alibabacloud_opt20210730-1.0.1/LICENSE` & `alibabacloud_opt20210730-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_opt20210730-1.0.1/PKG-INFO` & `alibabacloud_opt20210730-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_opt20210730
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud opt (20210730) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_opt20210730-1.0.1/README-CN.md` & `alibabacloud_opt20210730-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_opt20210730-1.0.1/README.md` & `alibabacloud_opt20210730-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/client.py` & `alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,14 +41,19 @@
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def get_open_status_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> opt_20210730_models.GetOpenStatusResponse:
+        """
+        @param request: GetOpenStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOpenStatusResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='GetOpenStatus',
             version='2021-07-30',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -62,14 +67,19 @@
             self.call_api(params, req, runtime)
         )
 
     async def get_open_status_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> opt_20210730_models.GetOpenStatusResponse:
+        """
+        @param request: GetOpenStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOpenStatusResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='GetOpenStatus',
             version='2021-07-30',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -80,28 +90,41 @@
         )
         return TeaCore.from_map(
             opt_20210730_models.GetOpenStatusResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def get_open_status(self) -> opt_20210730_models.GetOpenStatusResponse:
+        """
+        @return: GetOpenStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_open_status_with_options(runtime)
 
     async def get_open_status_async(self) -> opt_20210730_models.GetOpenStatusResponse:
+        """
+        @return: GetOpenStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_open_status_with_options_async(runtime)
 
     def get_order_info_with_options(
         self,
         request: opt_20210730_models.GetOrderInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> opt_20210730_models.GetOrderInfoResponse:
+        """
+        @param request: GetOrderInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOrderInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.list_released):
+            query['ListReleased'] = request.list_released
         if not UtilClient.is_unset(request.rel_service):
             query['RelService'] = request.rel_service
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -122,16 +145,23 @@
         )
 
     async def get_order_info_with_options_async(
         self,
         request: opt_20210730_models.GetOrderInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> opt_20210730_models.GetOrderInfoResponse:
+        """
+        @param request: GetOrderInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOrderInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.list_released):
+            query['ListReleased'] = request.list_released
         if not UtilClient.is_unset(request.rel_service):
             query['RelService'] = request.rel_service
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -151,29 +181,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_order_info(
         self,
         request: opt_20210730_models.GetOrderInfoRequest,
     ) -> opt_20210730_models.GetOrderInfoResponse:
+        """
+        @param request: GetOrderInfoRequest
+        @return: GetOrderInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_order_info_with_options(request, runtime)
 
     async def get_order_info_async(
         self,
         request: opt_20210730_models.GetOrderInfoRequest,
     ) -> opt_20210730_models.GetOrderInfoResponse:
+        """
+        @param request: GetOrderInfoRequest
+        @return: GetOrderInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_order_info_with_options_async(request, runtime)
 
     def get_order_usage_with_options(
         self,
         request: opt_20210730_models.GetOrderUsageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> opt_20210730_models.GetOrderUsageResponse:
+        """
+        @param request: GetOrderUsageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOrderUsageResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.license_key):
             query['LicenseKey'] = request.license_key
         if not UtilClient.is_unset(request.rel_service):
             query['RelService'] = request.rel_service
         if not UtilClient.is_unset(request.resource_type):
@@ -200,14 +243,19 @@
         )
 
     async def get_order_usage_with_options_async(
         self,
         request: opt_20210730_models.GetOrderUsageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> opt_20210730_models.GetOrderUsageResponse:
+        """
+        @param request: GetOrderUsageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetOrderUsageResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.license_key):
             query['LicenseKey'] = request.license_key
         if not UtilClient.is_unset(request.rel_service):
             query['RelService'] = request.rel_service
         if not UtilClient.is_unset(request.resource_type):
@@ -233,16 +281,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_order_usage(
         self,
         request: opt_20210730_models.GetOrderUsageRequest,
     ) -> opt_20210730_models.GetOrderUsageResponse:
+        """
+        @param request: GetOrderUsageRequest
+        @return: GetOrderUsageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_order_usage_with_options(request, runtime)
 
     async def get_order_usage_async(
         self,
         request: opt_20210730_models.GetOrderUsageRequest,
     ) -> opt_20210730_models.GetOrderUsageResponse:
+        """
+        @param request: GetOrderUsageRequest
+        @return: GetOrderUsageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_order_usage_with_options_async(request, runtime)
```

### Comparing `alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/models.py` & `alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,37 +95,45 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetOrderInfoRequest(TeaModel):
     def __init__(
         self,
+        list_released: bool = None,
         rel_service: str = None,
         resource_type: int = None,
     ):
+        self.list_released = list_released
+        # This parameter is required.
         self.rel_service = rel_service
+        # This parameter is required.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.list_released is not None:
+            result['ListReleased'] = self.list_released
         if self.rel_service is not None:
             result['RelService'] = self.rel_service
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('ListReleased') is not None:
+            self.list_released = m.get('ListReleased')
         if m.get('RelService') is not None:
             self.rel_service = m.get('RelService')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
@@ -296,16 +304,19 @@
     def __init__(
         self,
         license_key: str = None,
         rel_service: str = None,
         resource_type: int = None,
         time_range: int = None,
     ):
+        # This parameter is required.
         self.license_key = license_key
+        # This parameter is required.
         self.rel_service = rel_service
+        # This parameter is required.
         self.resource_type = resource_type
         self.time_range = time_range
 
     def validate(self):
         pass
 
     def to_map(self):
```

### Comparing `alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/PKG-INFO` & `alibabacloud_opt20210730-1.0.2/alibabacloud_opt20210730.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-opt20210730
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud opt (20210730) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_opt20210730-1.0.1/setup.py` & `alibabacloud_opt20210730-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_opt20210730.
 
-Created on 12/04/2024
+Created on 20/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_opt20210730"
 NAME = "alibabacloud_opt20210730" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud opt (20210730) SDK Library for Python"
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


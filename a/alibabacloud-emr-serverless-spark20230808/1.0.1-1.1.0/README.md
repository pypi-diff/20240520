# Comparing `tmp/alibabacloud_emr-serverless-spark20230808-1.0.1.tar.gz` & `tmp/alibabacloud_emr-serverless-spark20230808-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_emr-serverless-spark20230808-1.0.1.tar", last modified: Fri May 17 17:23:15 2024, max compression
+gzip compressed data, was "dist/alibabacloud_emr-serverless-spark20230808-1.1.0.tar", last modified: Mon May 20 17:14:59 2024, max compression
```

## Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1.tar` & `alibabacloud_emr-serverless-spark20230808-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1163 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1248 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23820 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808/client.py
--rw-r--r--   0 root         (0) root         (0)    85957 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 17:23:15.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2700 2024-05-17 17:23:14.000000 alibabacloud_emr-serverless-spark20230808-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37330 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/client.py
+-rw-r--r--   0 root         (0) root         (0)   116185 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2700 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/setup.py
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/LICENSE` & `alibabacloud_emr-serverless-spark20230808-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/PKG-INFO` & `alibabacloud_emr-serverless-spark20230808-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_emr-serverless-spark20230808
-Version: 1.0.1
+Version: 1.1.0
 Summary: Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/README-CN.md` & `alibabacloud_emr-serverless-spark20230808-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/README.md` & `alibabacloud_emr-serverless-spark20230808-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808/client.py` & `alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -429,14 +429,362 @@
         @param request: ListJobRunsRequest
         @return: ListJobRunsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_job_runs_with_options_async(workspace_id, request, headers, runtime)
 
+    def list_release_versions_with_options(
+        self,
+        request: emr_serverless_spark_20230808_models.ListReleaseVersionsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.ListReleaseVersionsResponse:
+        """
+        @summary 获取发布版本列表
+        
+        @param request: ListReleaseVersionsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListReleaseVersionsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        if not UtilClient.is_unset(request.release_type):
+            query['releaseType'] = request.release_type
+        if not UtilClient.is_unset(request.release_version):
+            query['releaseVersion'] = request.release_version
+        if not UtilClient.is_unset(request.release_version_status):
+            query['releaseVersionStatus'] = request.release_version_status
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListReleaseVersions',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/v1/releaseVersions',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.ListReleaseVersionsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_release_versions_with_options_async(
+        self,
+        request: emr_serverless_spark_20230808_models.ListReleaseVersionsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.ListReleaseVersionsResponse:
+        """
+        @summary 获取发布版本列表
+        
+        @param request: ListReleaseVersionsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListReleaseVersionsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        if not UtilClient.is_unset(request.release_type):
+            query['releaseType'] = request.release_type
+        if not UtilClient.is_unset(request.release_version):
+            query['releaseVersion'] = request.release_version
+        if not UtilClient.is_unset(request.release_version_status):
+            query['releaseVersionStatus'] = request.release_version_status
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListReleaseVersions',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/v1/releaseVersions',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.ListReleaseVersionsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_release_versions(
+        self,
+        request: emr_serverless_spark_20230808_models.ListReleaseVersionsRequest,
+    ) -> emr_serverless_spark_20230808_models.ListReleaseVersionsResponse:
+        """
+        @summary 获取发布版本列表
+        
+        @param request: ListReleaseVersionsRequest
+        @return: ListReleaseVersionsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_release_versions_with_options(request, headers, runtime)
+
+    async def list_release_versions_async(
+        self,
+        request: emr_serverless_spark_20230808_models.ListReleaseVersionsRequest,
+    ) -> emr_serverless_spark_20230808_models.ListReleaseVersionsResponse:
+        """
+        @summary 获取发布版本列表
+        
+        @param request: ListReleaseVersionsRequest
+        @return: ListReleaseVersionsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_release_versions_with_options_async(request, headers, runtime)
+
+    def list_workspace_queues_with_options(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.ListWorkspaceQueuesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.ListWorkspaceQueuesResponse:
+        """
+        @summary 查看工作空间队列列表
+        
+        @param request: ListWorkspaceQueuesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListWorkspaceQueuesResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.environment):
+            query['environment'] = request.environment
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListWorkspaceQueues',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/v1/workspaces/{OpenApiUtilClient.get_encode_param(workspace_id)}/queues',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.ListWorkspaceQueuesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_workspace_queues_with_options_async(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.ListWorkspaceQueuesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.ListWorkspaceQueuesResponse:
+        """
+        @summary 查看工作空间队列列表
+        
+        @param request: ListWorkspaceQueuesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListWorkspaceQueuesResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.environment):
+            query['environment'] = request.environment
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListWorkspaceQueues',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/v1/workspaces/{OpenApiUtilClient.get_encode_param(workspace_id)}/queues',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.ListWorkspaceQueuesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_workspace_queues(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.ListWorkspaceQueuesRequest,
+    ) -> emr_serverless_spark_20230808_models.ListWorkspaceQueuesResponse:
+        """
+        @summary 查看工作空间队列列表
+        
+        @param request: ListWorkspaceQueuesRequest
+        @return: ListWorkspaceQueuesResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_workspace_queues_with_options(workspace_id, request, headers, runtime)
+
+    async def list_workspace_queues_async(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.ListWorkspaceQueuesRequest,
+    ) -> emr_serverless_spark_20230808_models.ListWorkspaceQueuesResponse:
+        """
+        @summary 查看工作空间队列列表
+        
+        @param request: ListWorkspaceQueuesRequest
+        @return: ListWorkspaceQueuesResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_workspace_queues_with_options_async(workspace_id, request, headers, runtime)
+
+    def list_workspaces_with_options(
+        self,
+        request: emr_serverless_spark_20230808_models.ListWorkspacesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.ListWorkspacesResponse:
+        """
+        @summary 查看工作空间列表
+        
+        @param request: ListWorkspacesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListWorkspacesResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.name):
+            query['name'] = request.name
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        if not UtilClient.is_unset(request.state):
+            query['state'] = request.state
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListWorkspaces',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/v1/workspaces',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.ListWorkspacesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_workspaces_with_options_async(
+        self,
+        request: emr_serverless_spark_20230808_models.ListWorkspacesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.ListWorkspacesResponse:
+        """
+        @summary 查看工作空间列表
+        
+        @param request: ListWorkspacesRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListWorkspacesResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.name):
+            query['name'] = request.name
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        if not UtilClient.is_unset(request.state):
+            query['state'] = request.state
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListWorkspaces',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/v1/workspaces',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.ListWorkspacesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_workspaces(
+        self,
+        request: emr_serverless_spark_20230808_models.ListWorkspacesRequest,
+    ) -> emr_serverless_spark_20230808_models.ListWorkspacesResponse:
+        """
+        @summary 查看工作空间列表
+        
+        @param request: ListWorkspacesRequest
+        @return: ListWorkspacesResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_workspaces_with_options(request, headers, runtime)
+
+    async def list_workspaces_async(
+        self,
+        request: emr_serverless_spark_20230808_models.ListWorkspacesRequest,
+    ) -> emr_serverless_spark_20230808_models.ListWorkspacesResponse:
+        """
+        @summary 查看工作空间列表
+        
+        @param request: ListWorkspacesRequest
+        @return: ListWorkspacesResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_workspaces_with_options_async(request, headers, runtime)
+
     def start_job_run_with_options(
         self,
         workspace_id: str,
         request: emr_serverless_spark_20230808_models.StartJobRunRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> emr_serverless_spark_20230808_models.StartJobRunResponse:
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808/models.py` & `alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -2323,14 +2323,883 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListJobRunsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListReleaseVersionsRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+        release_type: str = None,
+        release_version: str = None,
+        release_version_status: str = None,
+    ):
+        self.region_id = region_id
+        self.release_type = release_type
+        self.release_version = release_version
+        self.release_version_status = release_version_status
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
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.release_type is not None:
+            result['releaseType'] = self.release_type
+        if self.release_version is not None:
+            result['releaseVersion'] = self.release_version
+        if self.release_version_status is not None:
+            result['releaseVersionStatus'] = self.release_version_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('releaseType') is not None:
+            self.release_type = m.get('releaseType')
+        if m.get('releaseVersion') is not None:
+            self.release_version = m.get('releaseVersion')
+        if m.get('releaseVersionStatus') is not None:
+            self.release_version_status = m.get('releaseVersionStatus')
+        return self
+
+
+class ListReleaseVersionsResponseBodyReleaseVersions(TeaModel):
+    def __init__(
+        self,
+        community_version: str = None,
+        cpu_architectures: List[str] = None,
+        gmt_create: int = None,
+        iaas_type: str = None,
+        release_version: str = None,
+        scala_version: str = None,
+        state: str = None,
+        type: str = None,
+    ):
+        self.community_version = community_version
+        self.cpu_architectures = cpu_architectures
+        self.gmt_create = gmt_create
+        self.iaas_type = iaas_type
+        self.release_version = release_version
+        self.scala_version = scala_version
+        self.state = state
+        self.type = type
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
+        if self.community_version is not None:
+            result['communityVersion'] = self.community_version
+        if self.cpu_architectures is not None:
+            result['cpuArchitectures'] = self.cpu_architectures
+        if self.gmt_create is not None:
+            result['gmtCreate'] = self.gmt_create
+        if self.iaas_type is not None:
+            result['iaasType'] = self.iaas_type
+        if self.release_version is not None:
+            result['releaseVersion'] = self.release_version
+        if self.scala_version is not None:
+            result['scalaVersion'] = self.scala_version
+        if self.state is not None:
+            result['state'] = self.state
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('communityVersion') is not None:
+            self.community_version = m.get('communityVersion')
+        if m.get('cpuArchitectures') is not None:
+            self.cpu_architectures = m.get('cpuArchitectures')
+        if m.get('gmtCreate') is not None:
+            self.gmt_create = m.get('gmtCreate')
+        if m.get('iaasType') is not None:
+            self.iaas_type = m.get('iaasType')
+        if m.get('releaseVersion') is not None:
+            self.release_version = m.get('releaseVersion')
+        if m.get('scalaVersion') is not None:
+            self.scala_version = m.get('scalaVersion')
+        if m.get('state') is not None:
+            self.state = m.get('state')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class ListReleaseVersionsResponseBody(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        release_versions: List[ListReleaseVersionsResponseBodyReleaseVersions] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # 一次获取的最大记录数。
+        self.max_results = max_results
+        # 下一页TOKEN。
+        self.next_token = next_token
+        self.release_versions = release_versions
+        # 请求ID。
+        self.request_id = request_id
+        # 记录总数。
+        self.total_count = total_count
+
+    def validate(self):
+        if self.release_versions:
+            for k in self.release_versions:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        result['releaseVersions'] = []
+        if self.release_versions is not None:
+            for k in self.release_versions:
+                result['releaseVersions'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        self.release_versions = []
+        if m.get('releaseVersions') is not None:
+            for k in m.get('releaseVersions'):
+                temp_model = ListReleaseVersionsResponseBodyReleaseVersions()
+                self.release_versions.append(temp_model.from_map(k))
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class ListReleaseVersionsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListReleaseVersionsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListReleaseVersionsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListWorkspaceQueuesRequest(TeaModel):
+    def __init__(
+        self,
+        environment: str = None,
+        region_id: str = None,
+    ):
+        self.environment = environment
+        self.region_id = region_id
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
+        if self.environment is not None:
+            result['environment'] = self.environment
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('environment') is not None:
+            self.environment = m.get('environment')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        return self
+
+
+class ListWorkspaceQueuesResponseBodyQueuesAllowActions(TeaModel):
+    def __init__(
+        self,
+        action_arn: str = None,
+        action_name: str = None,
+        dependencies: List[str] = None,
+        description: str = None,
+        display_name: str = None,
+    ):
+        # 行为 arn。
+        self.action_arn = action_arn
+        # 权限名称。
+        self.action_name = action_name
+        # action 依赖列表。
+        self.dependencies = dependencies
+        # action 描述。
+        self.description = description
+        # 权限展示名称。
+        self.display_name = display_name
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
+        if self.action_arn is not None:
+            result['actionArn'] = self.action_arn
+        if self.action_name is not None:
+            result['actionName'] = self.action_name
+        if self.dependencies is not None:
+            result['dependencies'] = self.dependencies
+        if self.description is not None:
+            result['description'] = self.description
+        if self.display_name is not None:
+            result['displayName'] = self.display_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('actionArn') is not None:
+            self.action_arn = m.get('actionArn')
+        if m.get('actionName') is not None:
+            self.action_name = m.get('actionName')
+        if m.get('dependencies') is not None:
+            self.dependencies = m.get('dependencies')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('displayName') is not None:
+            self.display_name = m.get('displayName')
+        return self
+
+
+class ListWorkspaceQueuesResponseBodyQueues(TeaModel):
+    def __init__(
+        self,
+        allow_actions: List[ListWorkspaceQueuesResponseBodyQueuesAllowActions] = None,
+        creator: str = None,
+        environments: List[str] = None,
+        max_resource: str = None,
+        min_resource: str = None,
+        properties: str = None,
+        queue_name: str = None,
+        queue_scope: str = None,
+        queue_status: str = None,
+        queue_type: str = None,
+        region_id: str = None,
+        used_resource: str = None,
+        workspace_id: str = None,
+    ):
+        # 队列允许的操作
+        self.allow_actions = allow_actions
+        self.creator = creator
+        self.environments = environments
+        # 队列资源最大容量
+        self.max_resource = max_resource
+        # 队列资源最小容量
+        self.min_resource = min_resource
+        # 队列Label
+        self.properties = properties
+        # 队列名称。
+        self.queue_name = queue_name
+        # 队列架构
+        self.queue_scope = queue_scope
+        self.queue_status = queue_status
+        # 队列类型
+        self.queue_type = queue_type
+        # regionId。
+        self.region_id = region_id
+        # 队列资源使用容量
+        self.used_resource = used_resource
+        # 工作空间id。
+        self.workspace_id = workspace_id
+
+    def validate(self):
+        if self.allow_actions:
+            for k in self.allow_actions:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['allowActions'] = []
+        if self.allow_actions is not None:
+            for k in self.allow_actions:
+                result['allowActions'].append(k.to_map() if k else None)
+        if self.creator is not None:
+            result['creator'] = self.creator
+        if self.environments is not None:
+            result['environments'] = self.environments
+        if self.max_resource is not None:
+            result['maxResource'] = self.max_resource
+        if self.min_resource is not None:
+            result['minResource'] = self.min_resource
+        if self.properties is not None:
+            result['properties'] = self.properties
+        if self.queue_name is not None:
+            result['queueName'] = self.queue_name
+        if self.queue_scope is not None:
+            result['queueScope'] = self.queue_scope
+        if self.queue_status is not None:
+            result['queueStatus'] = self.queue_status
+        if self.queue_type is not None:
+            result['queueType'] = self.queue_type
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.used_resource is not None:
+            result['usedResource'] = self.used_resource
+        if self.workspace_id is not None:
+            result['workspaceId'] = self.workspace_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.allow_actions = []
+        if m.get('allowActions') is not None:
+            for k in m.get('allowActions'):
+                temp_model = ListWorkspaceQueuesResponseBodyQueuesAllowActions()
+                self.allow_actions.append(temp_model.from_map(k))
+        if m.get('creator') is not None:
+            self.creator = m.get('creator')
+        if m.get('environments') is not None:
+            self.environments = m.get('environments')
+        if m.get('maxResource') is not None:
+            self.max_resource = m.get('maxResource')
+        if m.get('minResource') is not None:
+            self.min_resource = m.get('minResource')
+        if m.get('properties') is not None:
+            self.properties = m.get('properties')
+        if m.get('queueName') is not None:
+            self.queue_name = m.get('queueName')
+        if m.get('queueScope') is not None:
+            self.queue_scope = m.get('queueScope')
+        if m.get('queueStatus') is not None:
+            self.queue_status = m.get('queueStatus')
+        if m.get('queueType') is not None:
+            self.queue_type = m.get('queueType')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('usedResource') is not None:
+            self.used_resource = m.get('usedResource')
+        if m.get('workspaceId') is not None:
+            self.workspace_id = m.get('workspaceId')
+        return self
+
+
+class ListWorkspaceQueuesResponseBody(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        queues: List[ListWorkspaceQueuesResponseBodyQueues] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # 一次获取的最大记录数。
+        self.max_results = max_results
+        # 下一页TOKEN。
+        self.next_token = next_token
+        self.queues = queues
+        # 请求ID。
+        self.request_id = request_id
+        # 记录总数。
+        self.total_count = total_count
+
+    def validate(self):
+        if self.queues:
+            for k in self.queues:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        result['queues'] = []
+        if self.queues is not None:
+            for k in self.queues:
+                result['queues'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        self.queues = []
+        if m.get('queues') is not None:
+            for k in m.get('queues'):
+                temp_model = ListWorkspaceQueuesResponseBodyQueues()
+                self.queues.append(temp_model.from_map(k))
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class ListWorkspaceQueuesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListWorkspaceQueuesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListWorkspaceQueuesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListWorkspacesRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        name: str = None,
+        next_token: str = None,
+        region_id: str = None,
+        state: str = None,
+    ):
+        # 一次获取的最大记录数。
+        self.max_results = max_results
+        self.name = name
+        # 标记当前开始读取的位置，置空表示从头开始。
+        self.next_token = next_token
+        self.region_id = region_id
+        self.state = state
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
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.name is not None:
+            result['name'] = self.name
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.state is not None:
+            result['state'] = self.state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('state') is not None:
+            self.state = m.get('state')
+        return self
+
+
+class ListWorkspacesResponseBodyWorkspacesStateChangeReason(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.message = message
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
+        if self.code is not None:
+            result['code'] = self.code
+        if self.message is not None:
+            result['message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        return self
+
+
+class ListWorkspacesResponseBodyWorkspaces(TeaModel):
+    def __init__(
+        self,
+        auto_renew: bool = None,
+        auto_renew_period: int = None,
+        auto_renew_period_unit: str = None,
+        create_time: int = None,
+        dlf_catalog_id: str = None,
+        duration: int = None,
+        end_time: int = None,
+        fail_reason: str = None,
+        payment_duration_unit: str = None,
+        payment_status: str = None,
+        payment_type: str = None,
+        region_id: str = None,
+        release_type: str = None,
+        resource_spec: str = None,
+        state_change_reason: ListWorkspacesResponseBodyWorkspacesStateChangeReason = None,
+        storage: str = None,
+        workspace_id: str = None,
+        workspace_name: str = None,
+        workspace_status: str = None,
+    ):
+        # 是否自动续费(pre付费类型必须)。
+        self.auto_renew = auto_renew
+        # 自动续费时长(pre付费类型必须)。
+        self.auto_renew_period = auto_renew_period
+        # 自动续费周期(pre付费类型必须)。
+        self.auto_renew_period_unit = auto_renew_period_unit
+        self.create_time = create_time
+        # dlf catalog 信息。
+        self.dlf_catalog_id = dlf_catalog_id
+        # 订购周期数量(pre付费类型必须)。
+        self.duration = duration
+        self.end_time = end_time
+        # 失败原因。
+        self.fail_reason = fail_reason
+        # 订购周期(pre付费类型必须)。
+        self.payment_duration_unit = payment_duration_unit
+        # 支付状态。
+        self.payment_status = payment_status
+        # 付费类型。
+        self.payment_type = payment_type
+        self.region_id = region_id
+        self.release_type = release_type
+        # 资源规格。
+        self.resource_spec = resource_spec
+        self.state_change_reason = state_change_reason
+        # oss 路径。
+        self.storage = storage
+        # Workspace Id。
+        self.workspace_id = workspace_id
+        # 工作空间名称。
+        self.workspace_name = workspace_name
+        # 工作空间状态。
+        self.workspace_status = workspace_status
+
+    def validate(self):
+        if self.state_change_reason:
+            self.state_change_reason.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto_renew is not None:
+            result['autoRenew'] = self.auto_renew
+        if self.auto_renew_period is not None:
+            result['autoRenewPeriod'] = self.auto_renew_period
+        if self.auto_renew_period_unit is not None:
+            result['autoRenewPeriodUnit'] = self.auto_renew_period_unit
+        if self.create_time is not None:
+            result['createTime'] = self.create_time
+        if self.dlf_catalog_id is not None:
+            result['dlfCatalogId'] = self.dlf_catalog_id
+        if self.duration is not None:
+            result['duration'] = self.duration
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.fail_reason is not None:
+            result['failReason'] = self.fail_reason
+        if self.payment_duration_unit is not None:
+            result['paymentDurationUnit'] = self.payment_duration_unit
+        if self.payment_status is not None:
+            result['paymentStatus'] = self.payment_status
+        if self.payment_type is not None:
+            result['paymentType'] = self.payment_type
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.release_type is not None:
+            result['releaseType'] = self.release_type
+        if self.resource_spec is not None:
+            result['resourceSpec'] = self.resource_spec
+        if self.state_change_reason is not None:
+            result['stateChangeReason'] = self.state_change_reason.to_map()
+        if self.storage is not None:
+            result['storage'] = self.storage
+        if self.workspace_id is not None:
+            result['workspaceId'] = self.workspace_id
+        if self.workspace_name is not None:
+            result['workspaceName'] = self.workspace_name
+        if self.workspace_status is not None:
+            result['workspaceStatus'] = self.workspace_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('autoRenew') is not None:
+            self.auto_renew = m.get('autoRenew')
+        if m.get('autoRenewPeriod') is not None:
+            self.auto_renew_period = m.get('autoRenewPeriod')
+        if m.get('autoRenewPeriodUnit') is not None:
+            self.auto_renew_period_unit = m.get('autoRenewPeriodUnit')
+        if m.get('createTime') is not None:
+            self.create_time = m.get('createTime')
+        if m.get('dlfCatalogId') is not None:
+            self.dlf_catalog_id = m.get('dlfCatalogId')
+        if m.get('duration') is not None:
+            self.duration = m.get('duration')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('failReason') is not None:
+            self.fail_reason = m.get('failReason')
+        if m.get('paymentDurationUnit') is not None:
+            self.payment_duration_unit = m.get('paymentDurationUnit')
+        if m.get('paymentStatus') is not None:
+            self.payment_status = m.get('paymentStatus')
+        if m.get('paymentType') is not None:
+            self.payment_type = m.get('paymentType')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('releaseType') is not None:
+            self.release_type = m.get('releaseType')
+        if m.get('resourceSpec') is not None:
+            self.resource_spec = m.get('resourceSpec')
+        if m.get('stateChangeReason') is not None:
+            temp_model = ListWorkspacesResponseBodyWorkspacesStateChangeReason()
+            self.state_change_reason = temp_model.from_map(m['stateChangeReason'])
+        if m.get('storage') is not None:
+            self.storage = m.get('storage')
+        if m.get('workspaceId') is not None:
+            self.workspace_id = m.get('workspaceId')
+        if m.get('workspaceName') is not None:
+            self.workspace_name = m.get('workspaceName')
+        if m.get('workspaceStatus') is not None:
+            self.workspace_status = m.get('workspaceStatus')
+        return self
+
+
+class ListWorkspacesResponseBody(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        request_id: str = None,
+        total_count: int = None,
+        workspaces: List[ListWorkspacesResponseBodyWorkspaces] = None,
+    ):
+        # 一次获取的最大记录数。
+        self.max_results = max_results
+        # 下一页TOKEN。
+        self.next_token = next_token
+        # 请求ID。
+        self.request_id = request_id
+        # 记录总数。
+        self.total_count = total_count
+        self.workspaces = workspaces
+
+    def validate(self):
+        if self.workspaces:
+            for k in self.workspaces:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        result['workspaces'] = []
+        if self.workspaces is not None:
+            for k in self.workspaces:
+                result['workspaces'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        self.workspaces = []
+        if m.get('workspaces') is not None:
+            for k in m.get('workspaces'):
+                temp_model = ListWorkspacesResponseBodyWorkspaces()
+                self.workspaces.append(temp_model.from_map(k))
+        return self
+
+
+class ListWorkspacesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListWorkspacesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListWorkspacesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class StartJobRunRequestConfigurationOverridesConfigurations(TeaModel):
     def __init__(
         self,
         config_file_name: str = None,
         config_item_key: str = None,
         config_item_value: str = None,
     ):
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO` & `alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-emr-serverless-spark20230808
-Version: 1.0.1
+Version: 1.1.0
 Summary: Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt` & `alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.0.1/setup.py` & `alibabacloud_emr-serverless-spark20230808-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_emr-serverless-spark20230808.
 
-Created on 17/05/2024
+Created on 20/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_emr_serverless_spark20230808"
 NAME = "alibabacloud_emr-serverless-spark20230808" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python"
```


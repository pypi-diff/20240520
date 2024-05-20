# Comparing `tmp/alibabacloud_dbs20210101-2.0.1.tar.gz` & `tmp/alibabacloud_dbs20210101-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dbs20210101-2.0.1.tar", last modified: Fri May 17 17:23:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dbs20210101-2.1.0.tar", last modified: Mon May 20 17:18:54 2024, max compression
```

## Comparing `alibabacloud_dbs20210101-2.0.1.tar` & `alibabacloud_dbs20210101-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91515 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/client.py
--rw-r--r--   0 root         (0) root         (0)   138060 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)      535 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99429 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101/client.py
+-rw-r--r--   0 root         (0) root         (0)   156849 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-20 17:18:54.000000 alibabacloud_dbs20210101-2.1.0/setup.py
```

### Comparing `alibabacloud_dbs20210101-2.0.1/LICENSE` & `alibabacloud_dbs20210101-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-2.0.1/PKG-INFO` & `alibabacloud_dbs20210101-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dbs20210101
-Version: 2.0.1
+Version: 2.1.0
 Summary: Alibaba Cloud Dbs (20210101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dbs20210101-2.0.1/README-CN.md` & `alibabacloud_dbs20210101-2.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-2.0.1/README.md` & `alibabacloud_dbs20210101-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/client.py` & `alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,114 @@
         
         @param request: ChangeResourceGroupRequest
         @return: ChangeResourceGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.change_resource_group_with_options_async(request, runtime)
 
+    def create_advanced_policy_with_options(
+        self,
+        request: dbs_20210101_models.CreateAdvancedPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dbs_20210101_models.CreateAdvancedPolicyResponse:
+        """
+        @summary 开启高级备份策略
+        
+        @param request: CreateAdvancedPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAdvancedPolicyResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateAdvancedPolicy',
+            version='2021-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dbs_20210101_models.CreateAdvancedPolicyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_advanced_policy_with_options_async(
+        self,
+        request: dbs_20210101_models.CreateAdvancedPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dbs_20210101_models.CreateAdvancedPolicyResponse:
+        """
+        @summary 开启高级备份策略
+        
+        @param request: CreateAdvancedPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAdvancedPolicyResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateAdvancedPolicy',
+            version='2021-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dbs_20210101_models.CreateAdvancedPolicyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_advanced_policy(
+        self,
+        request: dbs_20210101_models.CreateAdvancedPolicyRequest,
+    ) -> dbs_20210101_models.CreateAdvancedPolicyResponse:
+        """
+        @summary 开启高级备份策略
+        
+        @param request: CreateAdvancedPolicyRequest
+        @return: CreateAdvancedPolicyResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.create_advanced_policy_with_options(request, runtime)
+
+    async def create_advanced_policy_async(
+        self,
+        request: dbs_20210101_models.CreateAdvancedPolicyRequest,
+    ) -> dbs_20210101_models.CreateAdvancedPolicyResponse:
+        """
+        @summary 开启高级备份策略
+        
+        @param request: CreateAdvancedPolicyRequest
+        @return: CreateAdvancedPolicyResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.create_advanced_policy_with_options_async(request, runtime)
+
     def create_download_with_options(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
         @summary Creates an advanced download task for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
@@ -1794,14 +1894,122 @@
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @return: DescribeSandboxRecoveryTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sandbox_recovery_time_with_options_async(request, runtime)
 
+    def modify_backup_policy_with_options(
+        self,
+        request: dbs_20210101_models.ModifyBackupPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dbs_20210101_models.ModifyBackupPolicyResponse:
+        """
+        @summary 修改备份策略
+        
+        @param request: ModifyBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyBackupPolicyResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.advance_data_policies):
+            query['AdvanceDataPolicies'] = request.advance_data_policies
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.preferred_backup_window_begin):
+            query['PreferredBackupWindowBegin'] = request.preferred_backup_window_begin
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyBackupPolicy',
+            version='2021-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dbs_20210101_models.ModifyBackupPolicyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_backup_policy_with_options_async(
+        self,
+        request: dbs_20210101_models.ModifyBackupPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dbs_20210101_models.ModifyBackupPolicyResponse:
+        """
+        @summary 修改备份策略
+        
+        @param request: ModifyBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyBackupPolicyResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.advance_data_policies):
+            query['AdvanceDataPolicies'] = request.advance_data_policies
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.preferred_backup_window_begin):
+            query['PreferredBackupWindowBegin'] = request.preferred_backup_window_begin
+        if not UtilClient.is_unset(request.region_code):
+            query['RegionCode'] = request.region_code
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyBackupPolicy',
+            version='2021-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dbs_20210101_models.ModifyBackupPolicyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_backup_policy(
+        self,
+        request: dbs_20210101_models.ModifyBackupPolicyRequest,
+    ) -> dbs_20210101_models.ModifyBackupPolicyResponse:
+        """
+        @summary 修改备份策略
+        
+        @param request: ModifyBackupPolicyRequest
+        @return: ModifyBackupPolicyResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.modify_backup_policy_with_options(request, runtime)
+
+    async def modify_backup_policy_async(
+        self,
+        request: dbs_20210101_models.ModifyBackupPolicyRequest,
+    ) -> dbs_20210101_models.ModifyBackupPolicyResponse:
+        """
+        @summary 修改备份策略
+        
+        @param request: ModifyBackupPolicyRequest
+        @return: ModifyBackupPolicyResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_backup_policy_with_options_async(request, runtime)
+
     def modify_dbtables_recovery_state_with_options(
         self,
         request: dbs_20210101_models.ModifyDBTablesRecoveryStateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.ModifyDBTablesRecoveryStateResponse:
         """
         @param request: ModifyDBTablesRecoveryStateRequest
```

### Comparing `alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/models.py` & `alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,151 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ChangeResourceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateAdvancedPolicyRequest(TeaModel):
+    def __init__(
+        self,
+        instance_name: str = None,
+        region_code: str = None,
+    ):
+        self.instance_name = instance_name
+        self.region_code = region_code
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
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.region_code is not None:
+            result['RegionCode'] = self.region_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('RegionCode') is not None:
+            self.region_code = m.get('RegionCode')
+        return self
+
+
+class CreateAdvancedPolicyResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: bool = None,
+        err_code: str = None,
+        err_message: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.err_code = err_code
+        self.err_message = err_message
+        self.message = message
+        self.request_id = request_id
+        self.success = success
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
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.err_code is not None:
+            result['ErrCode'] = self.err_code
+        if self.err_message is not None:
+            result['ErrMessage'] = self.err_message
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('ErrCode') is not None:
+            self.err_code = m.get('ErrCode')
+        if m.get('ErrMessage') is not None:
+            self.err_message = m.get('ErrMessage')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateAdvancedPolicyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateAdvancedPolicyResponseBody = None,
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
+            temp_model = CreateAdvancedPolicyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateDownloadRequest(TeaModel):
     def __init__(
         self,
         bak_set_id: str = None,
         bak_set_size: str = None,
         bak_set_type: str = None,
         download_point_in_time: str = None,
@@ -3468,14 +3605,412 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSandboxRecoveryTimeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyBackupPolicyRequestAdvanceDataPolicies(TeaModel):
+    def __init__(
+        self,
+        action_type: str = None,
+        dest_region: str = None,
+        dest_type: str = None,
+        filter_key: str = None,
+        filter_type: str = None,
+        filter_type_copy: str = None,
+        filter_value: str = None,
+        policy_id: str = None,
+        retention_type: str = None,
+        retention_value: str = None,
+        src_region: str = None,
+        src_type: str = None,
+    ):
+        self.action_type = action_type
+        self.dest_region = dest_region
+        self.dest_type = dest_type
+        self.filter_key = filter_key
+        self.filter_type = filter_type
+        self.filter_type_copy = filter_type_copy
+        self.filter_value = filter_value
+        self.policy_id = policy_id
+        self.retention_type = retention_type
+        self.retention_value = retention_value
+        self.src_region = src_region
+        self.src_type = src_type
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
+        if self.action_type is not None:
+            result['ActionType'] = self.action_type
+        if self.dest_region is not None:
+            result['DestRegion'] = self.dest_region
+        if self.dest_type is not None:
+            result['DestType'] = self.dest_type
+        if self.filter_key is not None:
+            result['FilterKey'] = self.filter_key
+        if self.filter_type is not None:
+            result['FilterType'] = self.filter_type
+        if self.filter_type_copy is not None:
+            result['FilterType-copy'] = self.filter_type_copy
+        if self.filter_value is not None:
+            result['FilterValue'] = self.filter_value
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.retention_type is not None:
+            result['RetentionType'] = self.retention_type
+        if self.retention_value is not None:
+            result['RetentionValue'] = self.retention_value
+        if self.src_region is not None:
+            result['SrcRegion'] = self.src_region
+        if self.src_type is not None:
+            result['SrcType'] = self.src_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActionType') is not None:
+            self.action_type = m.get('ActionType')
+        if m.get('DestRegion') is not None:
+            self.dest_region = m.get('DestRegion')
+        if m.get('DestType') is not None:
+            self.dest_type = m.get('DestType')
+        if m.get('FilterKey') is not None:
+            self.filter_key = m.get('FilterKey')
+        if m.get('FilterType') is not None:
+            self.filter_type = m.get('FilterType')
+        if m.get('FilterType-copy') is not None:
+            self.filter_type_copy = m.get('FilterType-copy')
+        if m.get('FilterValue') is not None:
+            self.filter_value = m.get('FilterValue')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RetentionType') is not None:
+            self.retention_type = m.get('RetentionType')
+        if m.get('RetentionValue') is not None:
+            self.retention_value = m.get('RetentionValue')
+        if m.get('SrcRegion') is not None:
+            self.src_region = m.get('SrcRegion')
+        if m.get('SrcType') is not None:
+            self.src_type = m.get('SrcType')
+        return self
+
+
+class ModifyBackupPolicyRequest(TeaModel):
+    def __init__(
+        self,
+        advance_data_policies: List[ModifyBackupPolicyRequestAdvanceDataPolicies] = None,
+        instance_name: str = None,
+        preferred_backup_window_begin: str = None,
+        region_code: str = None,
+    ):
+        self.advance_data_policies = advance_data_policies
+        self.instance_name = instance_name
+        self.preferred_backup_window_begin = preferred_backup_window_begin
+        self.region_code = region_code
+
+    def validate(self):
+        if self.advance_data_policies:
+            for k in self.advance_data_policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['AdvanceDataPolicies'] = []
+        if self.advance_data_policies is not None:
+            for k in self.advance_data_policies:
+                result['AdvanceDataPolicies'].append(k.to_map() if k else None)
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.preferred_backup_window_begin is not None:
+            result['PreferredBackupWindowBegin'] = self.preferred_backup_window_begin
+        if self.region_code is not None:
+            result['RegionCode'] = self.region_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.advance_data_policies = []
+        if m.get('AdvanceDataPolicies') is not None:
+            for k in m.get('AdvanceDataPolicies'):
+                temp_model = ModifyBackupPolicyRequestAdvanceDataPolicies()
+                self.advance_data_policies.append(temp_model.from_map(k))
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('PreferredBackupWindowBegin') is not None:
+            self.preferred_backup_window_begin = m.get('PreferredBackupWindowBegin')
+        if m.get('RegionCode') is not None:
+            self.region_code = m.get('RegionCode')
+        return self
+
+
+class ModifyBackupPolicyResponseBodyDataAdvanceDataPolicies(TeaModel):
+    def __init__(
+        self,
+        auto_created: bool = None,
+        bak_type: str = None,
+        dest_region: str = None,
+        dest_type: str = None,
+        dump_action: str = None,
+        filter_key: str = None,
+        filter_type: str = None,
+        filter_value: str = None,
+        policy_id: str = None,
+        retention_type: str = None,
+        retention_value: str = None,
+        src_region: str = None,
+        src_type: str = None,
+    ):
+        self.auto_created = auto_created
+        self.bak_type = bak_type
+        self.dest_region = dest_region
+        self.dest_type = dest_type
+        self.dump_action = dump_action
+        self.filter_key = filter_key
+        self.filter_type = filter_type
+        self.filter_value = filter_value
+        self.policy_id = policy_id
+        self.retention_type = retention_type
+        self.retention_value = retention_value
+        self.src_region = src_region
+        self.src_type = src_type
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
+        if self.auto_created is not None:
+            result['AutoCreated'] = self.auto_created
+        if self.bak_type is not None:
+            result['BakType'] = self.bak_type
+        if self.dest_region is not None:
+            result['DestRegion'] = self.dest_region
+        if self.dest_type is not None:
+            result['DestType'] = self.dest_type
+        if self.dump_action is not None:
+            result['DumpAction'] = self.dump_action
+        if self.filter_key is not None:
+            result['FilterKey'] = self.filter_key
+        if self.filter_type is not None:
+            result['FilterType'] = self.filter_type
+        if self.filter_value is not None:
+            result['FilterValue'] = self.filter_value
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.retention_type is not None:
+            result['RetentionType'] = self.retention_type
+        if self.retention_value is not None:
+            result['RetentionValue'] = self.retention_value
+        if self.src_region is not None:
+            result['SrcRegion'] = self.src_region
+        if self.src_type is not None:
+            result['SrcType'] = self.src_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AutoCreated') is not None:
+            self.auto_created = m.get('AutoCreated')
+        if m.get('BakType') is not None:
+            self.bak_type = m.get('BakType')
+        if m.get('DestRegion') is not None:
+            self.dest_region = m.get('DestRegion')
+        if m.get('DestType') is not None:
+            self.dest_type = m.get('DestType')
+        if m.get('DumpAction') is not None:
+            self.dump_action = m.get('DumpAction')
+        if m.get('FilterKey') is not None:
+            self.filter_key = m.get('FilterKey')
+        if m.get('FilterType') is not None:
+            self.filter_type = m.get('FilterType')
+        if m.get('FilterValue') is not None:
+            self.filter_value = m.get('FilterValue')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RetentionType') is not None:
+            self.retention_type = m.get('RetentionType')
+        if m.get('RetentionValue') is not None:
+            self.retention_value = m.get('RetentionValue')
+        if m.get('SrcRegion') is not None:
+            self.src_region = m.get('SrcRegion')
+        if m.get('SrcType') is not None:
+            self.src_type = m.get('SrcType')
+        return self
+
+
+class ModifyBackupPolicyResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        advance_data_policies: List[ModifyBackupPolicyResponseBodyDataAdvanceDataPolicies] = None,
+        preferred_backup_window: str = None,
+        preferred_backup_window_begin: str = None,
+    ):
+        self.advance_data_policies = advance_data_policies
+        self.preferred_backup_window = preferred_backup_window
+        self.preferred_backup_window_begin = preferred_backup_window_begin
+
+    def validate(self):
+        if self.advance_data_policies:
+            for k in self.advance_data_policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['AdvanceDataPolicies'] = []
+        if self.advance_data_policies is not None:
+            for k in self.advance_data_policies:
+                result['AdvanceDataPolicies'].append(k.to_map() if k else None)
+        if self.preferred_backup_window is not None:
+            result['PreferredBackupWindow'] = self.preferred_backup_window
+        if self.preferred_backup_window_begin is not None:
+            result['PreferredBackupWindowBegin'] = self.preferred_backup_window_begin
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.advance_data_policies = []
+        if m.get('AdvanceDataPolicies') is not None:
+            for k in m.get('AdvanceDataPolicies'):
+                temp_model = ModifyBackupPolicyResponseBodyDataAdvanceDataPolicies()
+                self.advance_data_policies.append(temp_model.from_map(k))
+        if m.get('PreferredBackupWindow') is not None:
+            self.preferred_backup_window = m.get('PreferredBackupWindow')
+        if m.get('PreferredBackupWindowBegin') is not None:
+            self.preferred_backup_window_begin = m.get('PreferredBackupWindowBegin')
+        return self
+
+
+class ModifyBackupPolicyResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: ModifyBackupPolicyResponseBodyData = None,
+        err_code: str = None,
+        err_message: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.err_code = err_code
+        self.err_message = err_message
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.err_code is not None:
+            result['ErrCode'] = self.err_code
+        if self.err_message is not None:
+            result['ErrMessage'] = self.err_message
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = ModifyBackupPolicyResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('ErrCode') is not None:
+            self.err_code = m.get('ErrCode')
+        if m.get('ErrMessage') is not None:
+            self.err_message = m.get('ErrMessage')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class ModifyBackupPolicyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyBackupPolicyResponseBody = None,
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
+            temp_model = ModifyBackupPolicyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyDBTablesRecoveryStateRequest(TeaModel):
     def __init__(
         self,
         category: str = None,
         instance_id: str = None,
         region_code: str = None,
         retention: str = None,
```

### Comparing `alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/PKG-INFO` & `alibabacloud_dbs20210101-2.1.0/alibabacloud_dbs20210101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dbs20210101
-Version: 2.0.1
+Version: 2.1.0
 Summary: Alibaba Cloud Dbs (20210101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dbs20210101-2.0.1/setup.py` & `alibabacloud_dbs20210101-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dbs20210101.
 
-Created on 17/05/2024
+Created on 20/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dbs20210101"
 NAME = "alibabacloud_dbs20210101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dbs (20210101) SDK Library for Python"
```


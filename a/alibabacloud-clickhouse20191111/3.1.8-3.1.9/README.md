# Comparing `tmp/alibabacloud_clickhouse20191111-3.1.8.tar.gz` & `tmp/alibabacloud_clickhouse20191111-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_clickhouse20191111-3.1.8.tar", last modified: Sun Feb  4 06:37:18 2024, max compression
+gzip compressed data, was "dist/alibabacloud_clickhouse20191111-3.1.9.tar", last modified: Wed Feb 21 17:12:12 2024, max compression
```

## Comparing `alibabacloud_clickhouse20191111-3.1.8.tar` & `alibabacloud_clickhouse20191111-3.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/
--rw-r--r--   0 root         (0) root         (0)      631 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302133 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111/client.py
--rw-r--r--   0 root         (0) root         (0)   463672 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-02-04 06:37:18.000000 alibabacloud_clickhouse20191111-3.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/
+-rw-r--r--   0 root         (0) root         (0)      822 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302349 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111/client.py
+-rw-r--r--   0 root         (0) root         (0)   464143 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-02-21 17:12:12.000000 alibabacloud_clickhouse20191111-3.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-02-21 17:12:11.000000 alibabacloud_clickhouse20191111-3.1.9/setup.py
```

### Comparing `alibabacloud_clickhouse20191111-3.1.8/LICENSE` & `alibabacloud_clickhouse20191111-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_clickhouse20191111-3.1.8/PKG-INFO` & `alibabacloud_clickhouse20191111-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_clickhouse20191111
-Version: 3.1.8
+Version: 3.1.9
 Summary: Alibaba Cloud ClickHouse (20191111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_clickhouse20191111-3.1.8/README-CN.md` & `alibabacloud_clickhouse20191111-3.1.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_clickhouse20191111-3.1.8/README.md` & `alibabacloud_clickhouse20191111-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111/client.py` & `alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1024,14 +1024,16 @@
     def create_dbinstance_with_options(
         self,
         request: clickhouse_20191111_models.CreateDBInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> clickhouse_20191111_models.CreateDBInstanceResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.auto_renew):
+            query['AutoRenew'] = request.auto_renew
         if not UtilClient.is_unset(request.backup_set_id):
             query['BackupSetID'] = request.backup_set_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_category):
             query['DBClusterCategory'] = request.dbcluster_category
         if not UtilClient.is_unset(request.dbcluster_class):
@@ -1108,14 +1110,16 @@
     async def create_dbinstance_with_options_async(
         self,
         request: clickhouse_20191111_models.CreateDBInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> clickhouse_20191111_models.CreateDBInstanceResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.auto_renew):
+            query['AutoRenew'] = request.auto_renew
         if not UtilClient.is_unset(request.backup_set_id):
             query['BackupSetID'] = request.backup_set_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_category):
             query['DBClusterCategory'] = request.dbcluster_category
         if not UtilClient.is_unset(request.dbcluster_class):
```

### Comparing `alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111/models.py` & `alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1498,14 +1498,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateDBInstanceRequest(TeaModel):
     def __init__(
         self,
+        auto_renew: bool = None,
         backup_set_id: str = None,
         client_token: str = None,
         dbcluster_category: str = None,
         dbcluster_class: str = None,
         dbcluster_description: str = None,
         dbcluster_network_type: str = None,
         dbcluster_version: str = None,
@@ -1528,14 +1529,15 @@
         v_switch_bak: str = None,
         v_switch_bak_2: str = None,
         v_switch_id: str = None,
         zond_id_bak_2: str = None,
         zone_id: str = None,
         zone_id_bak: str = None,
     ):
+        self.auto_renew = auto_renew
         # The ID of the backup set. You can call the [DescribeBackups](~~360339~~) operation to query the backup sets.
         # 
         # >  If you want to restore the data of an ApsaraDB for ClickHouse cluster, this parameter is required.
         self.backup_set_id = backup_set_id
         # The client token that is used to ensure the idempotence of the request. The value is a string and can be up to 64 ASCII characters in length.
         self.client_token = client_token
         # The edition of the cluster. Valid values:
@@ -1637,14 +1639,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.auto_renew is not None:
+            result['AutoRenew'] = self.auto_renew
         if self.backup_set_id is not None:
             result['BackupSetID'] = self.backup_set_id
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
         if self.dbcluster_category is not None:
             result['DBClusterCategory'] = self.dbcluster_category
         if self.dbcluster_class is not None:
@@ -1699,14 +1703,16 @@
             result['ZoneId'] = self.zone_id
         if self.zone_id_bak is not None:
             result['ZoneIdBak'] = self.zone_id_bak
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AutoRenew') is not None:
+            self.auto_renew = m.get('AutoRenew')
         if m.get('BackupSetID') is not None:
             self.backup_set_id = m.get('BackupSetID')
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
         if m.get('DBClusterCategory') is not None:
             self.dbcluster_category = m.get('DBClusterCategory')
         if m.get('DBClusterClass') is not None:
@@ -6000,18 +6006,18 @@
         # *   **CloudEfficiency**: The cluster uses an ultra disk.
         self.storage_type = storage_type
         # Indicates whether data backup is supported. Valid values:
         # 
         # *   **1**: Data backup is supported.
         # *   **2**: Data backup is not supported.
         self.support_backup = support_backup
-        # Indicates whether the cluster supports an HTTP port. Valid values:
+        # Indicates whether HTTPS ports are supported. Valid values:
         # 
-        # *   **true**: An HTTP port is supported.
-        # *   **false**: An HTTP port is not supported.
+        # *   **true**\
+        # *   **false**\
         self.support_https_port = support_https_port
         # Indicates whether the cluster supports a MySQL port. Valid values:
         # 
         # *   **true**: A MySQL port is supported.
         # *   **false**: A MySQL port is not supported.
         self.support_mysql_port = support_mysql_port
         # Indicates whether tiered storage of hot data and cold data is supported. Valid values:
@@ -6027,14 +6033,15 @@
         self.vpc_cloud_instance_id = vpc_cloud_instance_id
         # The virtual private cloud (VPC) ID.
         self.vpc_id = vpc_id
         # The IP address that is used to connect to the cluster over the VPC.
         self.vpc_ip_addr = vpc_ip_addr
         # The zone ID.
         self.zone_id = zone_id
+        # The list of vSwitch IDs in multi-zone clusters.
         self.zone_id_vswitch_map = zone_id_vswitch_map
         # The ZooKeeper specifications.
         self.zookeeper_class = zookeeper_class
 
     def validate(self):
         if self.scale_out_status:
             self.scale_out_status.validate()
@@ -8224,15 +8231,20 @@
         self.dbcluster_id = dbcluster_id
         # The ID of the query statement.
         self.initial_query_id = initial_query_id
         # The account that is used to log on to the database.
         self.initial_user = initial_user
         # The keyword that is used to query.
         self.keyword = keyword
-        # The column by which the query results are sorted.
+        # Sorting by the specified column name. Valid values:
+        # 
+        # *   elapsed: the cumulative execution time
+        # *   written_rows: the number of written rows
+        # *   read_rows: the number of read rows
+        # *   memory_usage: the memory usage
         self.order = order
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The page number. Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries returned per page. Valid values:
         # 
@@ -9832,16 +9844,16 @@
         error_msg: str = None,
         rds_id: str = None,
         rds_user_name: str = None,
         rds_vpc_url: str = None,
         syn_db: str = None,
         syn_status: bool = None,
     ):
-        # *   If the value **true** is returned for the **SynStatus** parameter, this parameter is not returned.
-        # *   If the value **false** is returned for the **SynStatus** parameter, the system returns the ErrorMsg parameter that provides the cause why the data synchronization failed.
+        # *   When the value **true** is returned for the **SynStatus** parameter, the system does not return the ErrorMsg parameter.
+        # *   When the value **false** is returned for the **SynStatus** parameter, the system returns for the ErrorMsg parameter the cause why the data synchronization failed.
         self.error_msg = error_msg
         # The ID of the ApsaraDB RDS for MySQL instance.
         self.rds_id = rds_id
         # The database account that is used to log on to the ApsaraDB RDS for MySQL instance.
         self.rds_user_name = rds_user_name
         # The internal endpoint of the ApsaraDB RDS for MySQL instance.
         self.rds_vpc_url = rds_vpc_url
@@ -11549,15 +11561,15 @@
         config: str = None,
         dbcluster_id: str = None,
         reason: str = None,
         region_id: str = None,
     ):
         # The configuration parameters whose settings you want to modify. You can call the [DescribeDBClusterConfigInXML](~~452210~~) operation to query configuration parameters, and modify the settings of the returned configuration parameters.
         # 
-        # >  You must specify all configuration parameters even when you want to modify the setting of a single parameter. If a configuration parameter is not specified, the original value of this parameter is retained or the modification fails.
+        # > You must specify all configuration parameters even when you want to modify the setting of a single parameter. If a configuration parameter is not specified, the original value of this parameter is retained or the modification fails.
         self.config = config
         # The cluster ID. You can call the [DescribeDBClusters](~~170879~~) operation to query information about all the clusters that are deployed in a specific region. The information includes the cluster IDs.
         self.dbcluster_id = dbcluster_id
         # The reason for the modification.
         self.reason = reason
         # The region ID of the cluster. You can call the [DescribeRegions](~~170875~~) operation to query the most recent region list.
         self.region_id = region_id
```

### Comparing `alibabacloud_clickhouse20191111-3.1.8/alibabacloud_clickhouse20191111.egg-info/PKG-INFO` & `alibabacloud_clickhouse20191111-3.1.9/alibabacloud_clickhouse20191111.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-clickhouse20191111
-Version: 3.1.8
+Version: 3.1.9
 Summary: Alibaba Cloud ClickHouse (20191111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_clickhouse20191111-3.1.8/setup.py` & `alibabacloud_clickhouse20191111-3.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_clickhouse20191111.
 
-Created on 04/02/2024
+Created on 21/02/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_clickhouse20191111"
 NAME = "alibabacloud_clickhouse20191111" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ClickHouse (20191111) SDK Library for Python"
```


# Comparing `tmp/prophecy-libs-1.8.9.tar.gz` & `tmp/prophecy-libs-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.8.9.tar", last modified: Wed Mar  6 13:11:26 2024, max compression
+gzip compressed data, was "prophecy-libs-1.9.0.tar", last modified: Mon May 20 10:20:21 2024, max compression
```

## Comparing `prophecy-libs-1.8.9.tar` & `prophecy-libs-1.9.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.273145 prophecy-libs-1.8.9/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.273145 prophecy-libs-1.8.9/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5645 2024-03-06 12:39:38.000000 prophecy-libs-1.8.9/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.8.9/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.277145 prophecy-libs-1.8.9/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1630 2023-08-26 18:29:07.000000 prophecy-libs-1.8.9/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.277145 prophecy-libs-1.8.9/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4678 2023-10-10 05:11:33.000000 prophecy-libs-1.8.9/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.277145 prophecy-libs-1.8.9/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.277145 prophecy-libs-1.8.9/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1944 2023-09-29 15:23:20.000000 prophecy-libs-1.8.9/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9645 2023-12-26 06:16:49.000000 prophecy-libs-1.8.9/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.281145 prophecy-libs-1.8.9/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2306 2024-02-23 07:14:39.000000 prophecy-libs-1.8.9/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.8.9/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.8.9/prophecy/udfs/scala_udf_wrapper.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.281145 prophecy-libs-1.8.9/prophecy/utils/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       75 2024-01-25 15:47:15.000000 prophecy-libs-1.8.9/prophecy/utils/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      303 2024-01-25 15:47:15.000000 prophecy-libs-1.8.9/prophecy/utils/gems_utils.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2824 2024-01-25 15:47:15.000000 prophecy-libs-1.8.9/prophecy/utils/metagem_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/prophecy/utils/transpiler/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      143 2023-08-26 18:29:07.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-08-26 18:29:07.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    22842 2023-08-30 12:14:40.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_core_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4406 2024-01-25 15:47:15.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_fcn_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     8387 2023-12-05 10:49:13.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/dataframe_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      692 2023-10-10 05:11:33.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/dml_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-08-26 18:29:07.000000 prophecy-libs-1.8.9/prophecy/utils/transpiler/fixed_file_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    29141 2024-02-11 09:01:20.000000 prophecy-libs-1.8.9/prophecy/utils/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1162 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2024-03-06 13:11:26.000000 prophecy-libs-1.8.9/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2024-03-06 13:11:26.285146 prophecy-libs-1.8.9/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      497 2024-03-06 13:11:25.000000 prophecy-libs-1.8.9/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.884415 prophecy-libs-1.9.0/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-05-20 10:20:21.884415 prophecy-libs-1.9.0/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     8391 2024-05-14 13:52:47.000000 prophecy-libs-1.9.0/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.9.0/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1777 2024-05-20 10:14:39.000000 prophecy-libs-1.9.0/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5483 2024-05-07 19:46:40.000000 prophecy-libs-1.9.0/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1944 2023-09-29 15:23:20.000000 prophecy-libs-1.9.0/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9645 2023-12-26 06:16:49.000000 prophecy-libs-1.9.0/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2306 2024-02-23 07:14:39.000000 prophecy-libs-1.9.0/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.9.0/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.9.0/prophecy/udfs/scala_udf_wrapper.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/utils/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      101 2024-05-20 10:20:20.000000 prophecy-libs-1.9.0/prophecy/utils/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      163 2024-05-20 10:14:39.000000 prophecy-libs-1.9.0/prophecy/utils/functions.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      303 2024-01-25 15:47:15.000000 prophecy-libs-1.9.0/prophecy/utils/gems_utils.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2824 2024-01-25 15:47:15.000000 prophecy-libs-1.9.0/prophecy/utils/metagem_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.880415 prophecy-libs-1.9.0/prophecy/utils/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      143 2023-08-26 18:29:07.000000 prophecy-libs-1.9.0/prophecy/utils/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-08-26 18:29:07.000000 prophecy-libs-1.9.0/prophecy/utils/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22842 2023-08-30 12:14:40.000000 prophecy-libs-1.9.0/prophecy/utils/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4406 2024-01-25 15:47:15.000000 prophecy-libs-1.9.0/prophecy/utils/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     8600 2024-04-28 17:37:46.000000 prophecy-libs-1.9.0/prophecy/utils/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      692 2023-10-10 05:11:33.000000 prophecy-libs-1.9.0/prophecy/utils/transpiler/dml_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-08-26 18:29:07.000000 prophecy-libs-1.9.0/prophecy/utils/transpiler/fixed_file_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    38816 2024-05-20 10:20:20.000000 prophecy-libs-1.9.0/prophecy/utils/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2024-05-20 10:20:21.884415 prophecy-libs-1.9.0/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2024-05-20 10:20:21.000000 prophecy-libs-1.9.0/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1190 2024-05-20 10:20:21.000000 prophecy-libs-1.9.0/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2024-05-20 10:20:21.000000 prophecy-libs-1.9.0/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.9.0/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2024-05-20 10:20:21.000000 prophecy-libs-1.9.0/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2024-05-20 10:20:21.000000 prophecy-libs-1.9.0/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2024-05-20 10:20:21.884415 prophecy-libs-1.9.0/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      497 2024-05-20 10:20:20.000000 prophecy-libs-1.9.0/setup.py
```

### Comparing `prophecy-libs-1.8.9/prophecy/config/config_base.py` & `prophecy-libs-1.9.0/prophecy/config/config_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 # WARNING - Do not add import * in this module
 from pyspark import Row
+from pyspark.sql import SparkSession
 from functools import lru_cache
 
 class ConfigBase:
 
     class SecretValue:
         def __init__(self, prophecy_spark=None, secretScope: str="", secretKey: str="", providerType: str="Databricks", **kwargs):
             self.prophecy_spark = prophecy_spark
             self.secretScope = secretScope
             self.secretKey = secretKey
             self.providerType = providerType
 
+        def __deepcopy__(self, memo):
+            import copy
+            from pyspark.sql import SparkSession
+            cls = self.__class__
+            result = cls.__new__(cls)
+            memo[id(self)] = result
+            for k, v in self.__dict__.items():
+                if isinstance(v, SparkSession):
+                    setattr(result, k, v)
+                else:
+                    setattr(result, k, copy.deepcopy(v, memo))
+            return result
+
         @lru_cache()
         def __str__(self):
+            if (self.prophecy_spark is not None and self.prophecy_spark.sparkContext.getConf().get("prophecy.schema.analysis") == "True"):
+                return f"{self.secretScope}:{self.secretKey}"
             self.jvm = self.prophecy_spark.sparkContext._jvm
             self.secret_manager = self.jvm.io.prophecy.libs.secrets.ProphecySecrets
             return self.secret_manager.get(self.secretScope, self.secretKey, self.providerType)
 
     def updateSpark(self, spark):
         self.spark = spark
 
@@ -93,47 +109,99 @@
         if override == None:
             return default
         else:
             return self.generate_config_object(spark, override, cls)
 
     def to_dict(self):
         def to_dict_recursive(obj):
-            def should_include(key):
-                ## these are in config objects but we need to remove them.
-                return key not in ["spark", "prophecy_spark"]
+            def should_include(key, value):
+                # remove any unwanted objects from the config:
+                return key not in ["spark", "prophecy_spark"] and not isinstance(value, SparkSession)
             if isinstance(obj, (list, tuple)):
                 return [to_dict_recursive(item) for item in obj]
             elif isinstance(obj, dict):
-                return {key: to_dict_recursive(value) for key, value in obj.items() if should_include(key)}
+                return {key: to_dict_recursive(value) for key, value in obj.items() if should_include(key, value)}
             elif hasattr(obj, "__dict__"):
-                return to_dict_recursive({key: value for key, value in obj.__dict__.items() if should_include(key)})
+                return to_dict_recursive({key: value for key, value in obj.__dict__.items() if should_include(key, value)})
             elif hasattr(obj, "__slots__"):
-                return to_dict_recursive({slot: getattr(obj, slot) for slot in obj.__slots__ if should_include(slot)})
+                return to_dict_recursive({slot: getattr(obj, slot) for slot in obj.__slots__ if should_include(slot, getattr(obj, slot))})
             else:
                 return obj
         return to_dict_recursive(self)
 
+    def update_all(self, name, new_value):
+        def process_attr_value(attr_val):
+            if isinstance(attr_val, ConfigBase):
+                attr_val.update_all(name, new_value)
+            elif isinstance(attr_val, list) or isinstance(attr_val, tuple):
+                for element in attr_val:
+                    if isinstance(element, ConfigBase):
+                        element.update_all(name, new_value)
+            elif isinstance(attr_val, dict):
+                for k, v in attr_val.items():
+                    if isinstance(v, ConfigBase):
+                        v.update_all(name, new_value)
+            else:
+                pass
+
+        if hasattr(self, "__dict__"):
+            for attr_name, attr_val in self.__dict__.items():
+                if attr_name == name:
+                    setattr(self, attr_name, new_value)
+                else:
+                    process_attr_value(attr_val)
+        if hasattr(self, "__slots__"):
+            for attr_name in self.__slots__:
+                if attr_name == name:
+                    setattr(self, attr_name, new_value)
+                else:
+                    process_attr_value(getattr(self, attr_name))
+        else:
+            pass
+
+    def find_spark(self, instance):
+        if isinstance(instance, list):
+            for element in instance:
+                spark = self.find_spark(element)
+                if spark is not None:
+                    return spark
+        if isinstance(instance, ConfigBase) or isinstance(instance, ConfigBase.SecretValue):
+            if hasattr(instance, "spark") and isinstance(instance.spark, SparkSession):
+                    return instance.spark
+            elif hasattr(instance, "prophecy_spark") and isinstance(instance.prophecy_spark, SparkSession):
+                    return instance.prophecy_spark
+            for key, value in instance.__dict__.items():
+                    spark = self.find_spark(value)
+                    if spark is not None:
+                        return spark
+        return None
+
     def update_from_row(self, row: Row):
         import copy
         new_config = copy.deepcopy(self)
-        spark_variable = None
+        spark_variable = self.find_spark(self)
         updated_config_json = {**new_config.to_dict(), **row.asDict(recursive=True)}
-        if hasattr(new_config, "spark") and new_config.spark is not None:
-            spark_variable = new_config.spark
-        elif hasattr(new_config, "prophecy_spark") and new_config.prophecy_spark is not None:
-            spark_variable = new_config.spark
         return self.get_config_object(spark_variable, new_config, updated_config_json, new_config.__class__)
 
     def update_from_row_map(self, row: Row, config_to_column: dict):
         import copy
         new_config = copy.deepcopy(self)
-        spark_variable = None
+        spark_variable = self.find_spark(self)
         row_as_dict = row.asDict(recursive=True)
         overridden_values = {}
         for config_name, column_name in config_to_column.items():
             overridden_values[config_name] = row_as_dict[column_name]
         updated_config_json = {**new_config.to_dict(), **overridden_values}
-        if hasattr(new_config, "spark") and new_config.spark is not None:
-            spark_variable = new_config.spark
-        elif hasattr(new_config, "prophecy_spark") and new_config.prophecy_spark is not None:
-            spark_variable = new_config.spark
         return self.get_config_object(spark_variable, new_config, updated_config_json, new_config.__class__)
+
+    def __deepcopy__(self, memo):
+        import copy
+        from pyspark.sql import SparkSession
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            if isinstance(v, SparkSession):
+                setattr(result, k, v)
+            else:
+                setattr(result, k, copy.deepcopy(v, memo))
+        return result
```

### Comparing `prophecy-libs-1.8.9/prophecy/config/utils.py` & `prophecy-libs-1.9.0/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/libs/utils.py` & `prophecy-libs-1.9.0/prophecy/libs/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from pyspark.sql import Column
 from pyspark.sql.functions import array, lit, struct
-
+from prophecy.config import ConfigBase
 
 def typed_lit(obj):
     if isinstance(obj, list):
         return array([typed_lit(x) for x in obj])
     elif isinstance(obj, dict):
         elementsList = []
         for key, value in obj.items():
             elementsList.append(typed_lit(value).alias(key))
         return struct(elementsList)
+    elif isinstance(obj, ConfigBase.SecretValue):
+        return lit(str(obj))
     else:
         try:
             # int, float, string
             return lit(obj)
         except:
             # class type
             return typed_lit(obj.__dict__)
@@ -56,8 +59,8 @@
     else:
         return spark.sparkContext._jvm.scala.Some(value)
 
 
 def isBlank(myString):
     if isinstance(myString, str) and myString and myString.strip():
         return False
-    return True
+    return True
```

### Comparing `prophecy-libs-1.8.9/prophecy/random_data_creator.py` & `prophecy-libs-1.9.0/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.9.0/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/test/base_test_case.py` & `prophecy-libs-1.9.0/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/test/utils.py` & `prophecy-libs-1.9.0/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.9.0/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.9.0/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/utils/metagem_utils.py` & `prophecy-libs-1.9.0/prophecy/utils/metagem_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_base.py` & `prophecy-libs-1.9.0/prophecy/utils/transpiler/abi_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_core_fcns.py` & `prophecy-libs-1.9.0/prophecy/utils/transpiler/abi_core_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/utils/transpiler/abi_fcn_wrapper.py` & `prophecy-libs-1.9.0/prophecy/utils/transpiler/abi_fcn_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/utils/transpiler/dataframe_fcns.py` & `prophecy-libs-1.9.0/prophecy/utils/transpiler/dataframe_fcns.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,18 @@
         pivotColumns,
         nameField,
         valueField,
         sparkSession
     )
 
 
+def evaluate_expression(df, userExpression, selectedColumnNames, sparkSession) -> DataFrame:
+    return ProphecyDataFrame(df, sparkSession).evaluate_expression(userExpression, selectedColumnNames, sparkSession)
+
+
 def compareRecords(df, otherDataFrame, componentName, limit, sparkSession) -> DataFrame:
     return ProphecyDataFrame(df, sparkSession).compareRecords(otherDataFrame, componentName, limit, sparkSession)
 
 
 def generateSurrogateKeys(
         df,
         keyDF,
```

### Comparing `prophecy-libs-1.8.9/prophecy/utils/transpiler/dml_schema.py` & `prophecy-libs-1.9.0/prophecy/utils/transpiler/dml_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/utils/transpiler/fixed_file_schema.py` & `prophecy-libs-1.9.0/prophecy/utils/transpiler/fixed_file_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.8.9/prophecy/utils/utils.py` & `prophecy-libs-1.9.0/prophecy/utils/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,28 @@
+import inspect
+import io
 import json
-from typing import Optional
+import sys
+import time
+from typing import Optional, Any
 import traceback
-from py4j.protocol import Py4JJavaError
+from py4j.protocol import Py4JError, Py4JJavaError
 from pyspark.sql import *
+from pyspark.sql.utils import CapturedException
 
 from prophecy.libs.utils import *
 
 
+class TaskState:
+    LAUNCHING = "LAUNCHING"
+    RUNNING = "RUNNING"
+    FAILED = "FAILED"
+    FINISHED = "FINISHED"
+
+
 class ProphecyDataFrame:
     def __init__(self, df: DataFrame, spark: SparkSession):
         self.jvm = spark.sparkContext._jvm
         self.spark = spark
         self.sqlContext = SQLContext(spark.sparkContext, sparkSession=spark)
 
         if type(df) == DataFrame:
@@ -136,14 +148,20 @@
 
     def metaPivot(self, pivotColumns, nameField, valueField, sparkSession) -> DataFrame:
         result = self.extended_dataframe.metaPivot(
             createScalaList(self.spark, pivotColumns), nameField, valueField, sparkSession._jsparkSession
         )
         return DataFrame(result, self.sqlContext)
 
+    def evaluate_expression(self, userExpression, selectedColumnNames, sparkSession) -> DataFrame:
+        result = self.extended_dataframe.evaluate_expression(
+            userExpression, createScalaList(self.spark, selectedColumnNames), sparkSession._jsparkSession
+        )
+        return DataFrame(result, self.sqlContext)
+
     def compareRecords(
             self, otherDataFrame, componentName, limit, sparkSession
     ) -> DataFrame:
         result = self.extended_dataframe.compareRecords(
             otherDataFrame._jdf, componentName, limit, sparkSession._jsparkSession
         )
         return DataFrame(result, self.sqlContext)
@@ -548,41 +566,41 @@
             config=None,
             **kwargs,
     ):
         global interimConfig
         interimConfig.maybeInitialize(spark, sessionForInteractive)
 
         # Define a function to convert object to a dictionary
-        def should_include(key):
-            ## these are in config objects but we need to remove them.
-            return key not in ["spark", "prophecy_spark"]
+        def should_include(key, value):
+            # remove any unwanted objects from the config:
+            return key not in ["spark", "prophecy_spark"] and not isinstance(value, SparkSession)
 
         def to_dict_recursive(obj):
             if isinstance(obj, (list, tuple)):
                 return [to_dict_recursive(item) for item in obj]
             elif isinstance(obj, dict):
                 return {
                     key: to_dict_recursive(value)
                     for key, value in obj.items()
-                    if should_include(key)
+                    if should_include(key, value)
                 }
             elif hasattr(obj, "__dict__"):
                 return to_dict_recursive(
                     {
                         key: value
                         for key, value in obj.__dict__.items()
-                        if should_include(key)
+                        if should_include(key, value)
                     }
                 )
             elif hasattr(obj, "__slots__"):
                 return to_dict_recursive(
                     {
                         slot: getattr(obj, slot)
                         for slot in obj.__slots__
-                        if should_include(slot)
+                        if should_include(slot, getattr(obj, slot))
                     }
                 )
             else:
                 return obj
 
         for key, value in kwargs.items():
             ProphecyDebugger.log(
@@ -628,43 +646,80 @@
         global interimConfig
         interimConfig.clear()
 
     # Use this like MetricsCollector.instrument(args)(pipeline_func_which_takes_spark)
     # Another variation could be annotation based, but going with this right now.
     @classmethod
     def instrument(
-        cls,
-        spark: SparkSession,
-        sessionForInteractive: str = "",
-        pipelineId: str = "",
-        config=None,
-        **kwargs,
+            cls,
+            spark: SparkSession,
+            sessionForInteractive: str = "",
+            pipelineId: str = "",
+            config=None,
+            **kwargs,
     ):
         def wrapper(f):
+
+            state = TaskState.LAUNCHING
+            startTime = currentTimeString()
             try:
                 MetricsCollector.start(
                     spark, sessionForInteractive, pipelineId, config, **kwargs
                 )
+                state = TaskState.RUNNING
+                sendPipelineProgressEvent(spark, sessionForInteractive, pipelineId, state,
+                                          startTime)
                 try:
-                    return f(spark)
+                    ret = f(spark)
+
+                    # if there are active streams, wait for them to finish
+                    if len(spark.streams.active) > 0:
+                        spark.streams.resetTerminated()
+                        spark.streams.awaitAnyTermination()
+
+                    return ret
                 except Exception as e:
+                    state = TaskState.FAILED
+                    endTime = currentTimeString()
                     etype = type(e).__name__
                     emsg = str(e)
                     etrace = traceback.format_exc()
-                    if isinstance(e, Py4JJavaError):
+
+                    if isinstance(e, CapturedException):
+                        py4j_error = None
+                        if e.getErrorClass():
+                            py4j_error = e._origin
+                        elif e.cause and e.cause.getErrorClass():
+                            py4j_error = e.cause._origin
+                        sendPipelineProgressEvent(spark, sessionForInteractive, pipelineId, state,
+                                                  startTime, endTime, py4j_error)
+                        spark.sparkContext._jvm.org.apache.spark.sql.MetricsCollector.setPythonFailedStatus(
+                            spark._jsparkSession, etype, emsg, etrace, py4j_error
+                        )
+                    elif isinstance(e, Py4JJavaError):
+                        sendPipelineProgressEvent(spark, sessionForInteractive, pipelineId, state,
+                                                  startTime, endTime, e)
                         spark.sparkContext._jvm.org.apache.spark.sql.MetricsCollector.setPythonFailedStatus(
                             spark._jsparkSession, etype, emsg, etrace, e.java_exception
                         )
                     else:
+                        # Python exception. Need not be transferred to JVM
+                        sendPipelineProgressEvent(spark, sessionForInteractive, pipelineId, state,
+                                                  startTime, endTime)
                         spark.sparkContext._jvm.org.apache.spark.sql.MetricsCollector.setPythonFailedStatus(
                             spark._jsparkSession, etype, emsg, etrace
                         )
                     raise
             finally:
                 try:
+                    if state != TaskState.FAILED:
+                        state = TaskState.FINISHED
+                        endTime = currentTimeString()
+                        sendPipelineProgressEvent(spark, sessionForInteractive, pipelineId, state,
+                                                  startTime, endTime)
                     MetricsCollector.end(spark)
                 except:
                     pass
 
         return wrapper
 
     @classmethod
@@ -784,14 +839,191 @@
                 postDataToSplunk(props, payload)
 
         batchDF.toJSON().foreachPartition(f)
 
     return wrapper
 
 
+def find_first_index(sequence, condition):
+    return next((i for i, x in enumerate(sequence) if condition(x)), -1)
+
+
+def find_last_index(sequence, condition):
+    return next((i for i, x in reversed(list(enumerate(sequence))) if condition(x)), -1)
+
+
+def currentTimeString() -> str:
+    return str(int(time.time() * 1000))
+
+
+def extractHierarchicalGemName(stack, function) -> str:
+    stack_function_names = [f.function for f in stack]
+    start_index = find_first_index(stack_function_names, lambda x: x == "inner_wrapper")
+    end_index = find_last_index(stack_function_names, lambda x: x == "pipeline")
+    sliced_stack = stack_function_names[start_index + 1:end_index]
+    stack_without_wrapper_nesting = [s for s in sliced_stack if s != "inner_wrapper"]
+    return ".".join(stack_without_wrapper_nesting + [function.__name__])
+
+
+# Add support for stdout in pipeline progress
+def sendPipelineProgressEvent(spark: SparkSession, userSession: str, pipelineId: str, state: str,
+                              startTime: str, endTime: str = "", stdout: str = "", stderr: str = "",
+                              exception: Optional[Any] = None):
+    if exception:
+        spark.sparkContext._jvm.org.apache.spark.sql.ProphecySparkSession.sendPipelineProgressEvent(
+            spark._jsparkSession, userSession, pipelineId, state, startTime, endTime, exception
+        )
+    else:
+        spark.sparkContext._jvm.org.apache.spark.sql.ProphecySparkSession.sendPipelineProgressEvent(
+            spark._jsparkSession, userSession, pipelineId, state, startTime, endTime
+        )
+
+
+def sendGemProgressEvent(spark: SparkSession, userSession: str, process_id: str, state: str,
+                         startTime: str, endTime: str = "", stdout: str = "[]", stderr: str = "[]",
+                         exception: Optional[Any] = None):
+    if exception:
+        spark.sparkContext._jvm.org.apache.spark.sql.ProphecySparkSession.sendGemProgressEvent(
+            spark._jsparkSession, userSession, process_id, state, startTime, endTime, stdout,
+            stderr, exception
+        )
+    else:
+        spark.sparkContext._jvm.org.apache.spark.sql.ProphecySparkSession.sendGemProgressEvent(
+            spark._jsparkSession, userSession, process_id, state, startTime, endTime, stdout,
+            stderr,
+        )
+
+
+def getProcessFromGem(spark: SparkSession, gemName: str, userSession: str) -> str:
+    return spark.sparkContext._jvm.org.apache.spark.sql.ProphecySparkSession.getProcessFromGem(
+        spark._jsparkSession, gemName, userSession)
+
+
+def instrument(function):
+    def inner_wrapper(spark, *args, **kwargs):
+        global interimConfig
+        if interimConfig.interimOutput:
+            user_session = interimConfig.interimOutput.session()
+        else:
+            user_session = ""
+        start_time = currentTimeString()
+        state = TaskState.LAUNCHING
+        gem_name = extractHierarchicalGemName(inspect.stack(), function)
+        process_id = getProcessFromGem(spark, gem_name, user_session)
+        sendGemProgressEvent(spark, user_session, process_id, state, start_time)
+
+        stdout_capture = TimestampedStringIO()
+        stderr_capture = TimestampedStringIO()
+
+        original_stdout = sys.stdout
+        original_stderr = sys.stderr
+
+        sys.stdout = MultiStream(original_stdout, stdout_capture)
+        sys.stderr = MultiStream(original_stderr, stderr_capture)
+
+        try:
+            state = TaskState.RUNNING
+            sendGemProgressEvent(spark, user_session, process_id, state,
+                                 start_time)
+            result = function(spark, *args, **kwargs)
+            return result
+        # Handle PythonException separately, probably similar to normal exception below?
+        except CapturedException as e:
+            state = TaskState.FAILED
+            captured_stdout = stdout_capture.getvalue()
+            captured_stderr = stderr_capture.getvalue()
+            py4j_error = None
+            if e.getErrorClass():
+                py4j_error = e._origin
+            elif e.cause and e.cause.getErrorClass():
+                py4j_error = e.cause._origin
+            sendGemProgressEvent(spark, user_session, process_id, state,
+                                 start_time, currentTimeString(), captured_stdout,
+                                 captured_stderr, py4j_error)
+            raise e
+        except Py4JError as e:
+            state = TaskState.FAILED
+            captured_stdout = stdout_capture.getvalue()
+            captured_stderr = stderr_capture.getvalue()
+            py4j_error = None
+            if (isinstance(e, Py4JJavaError)):
+                py4j_error = e
+            sendGemProgressEvent(spark, user_session, process_id, state,
+                                 start_time, currentTimeString(), captured_stdout,
+                                 captured_stderr, py4j_error)
+            raise e
+        except Exception as e:
+            state = TaskState.FAILED
+            captured_stdout = stdout_capture.getvalue()
+            captured_stderr = stderr_capture.getvalue()
+            sendGemProgressEvent(spark, user_session, process_id, state,
+                                 start_time, currentTimeString(), captured_stdout,
+                                 captured_stderr)
+            raise e
+        finally:
+            if state != TaskState.FAILED:
+                state = TaskState.FINISHED
+                captured_stdout = stdout_capture.getvalue()
+                captured_stderr = stderr_capture.getvalue()
+                sendGemProgressEvent(spark, user_session, process_id, state,
+                                     start_time,
+                                     currentTimeString(), captured_stdout, captured_stderr)
+
+            sys.stdout = original_stdout
+            sys.stderr = original_stderr
+            stdout_capture.close()
+            stderr_capture.close()
+
+    return inner_wrapper
+
+
+class TimestampedContent:
+
+    def __init__(self, content: str):
+        self.content = content
+        self.time = int(time.time() * 1000)
+
+    def to_dict(self) -> dict:
+        return {"content": self.content, "time": self.time}
+
+
+class TimestampedStringIO(io.StringIO):
+    def __init__(self):
+        super().__init__()
+        self.outputs = []
+
+    def write(self, s):
+        if s.strip():
+            self.outputs.append(TimestampedContent(s))
+        super().write(s)
+
+    def to_json(self):
+        return json.dumps([o.to_dict() for o in self.outputs])
+
+    def getvalue(self):
+        return self.to_json()
+
+
+class MultiStream:
+    def __init__(self, original, capture):
+        self.original = original
+        self.capture = capture
+
+    def write(self, data):
+        self.original.write(data)
+        self.capture.write(data)
+
+    def flush(self):
+        self.original.flush()
+        self.capture.flush()
+
+    def __getattr__(self, attr):
+        return getattr(self.original, attr)
+
+
 class SecretManager:
 
     def __init__(self, spark: SparkSession):
         self.jvm = spark.sparkContext._jvm
         self.spark = spark
         self.secret_manager = self.jvm.io.prophecy.libs.secrets.ProphecySecrets
```

### Comparing `prophecy-libs-1.8.9/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.9.0/prophecy_libs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 prophecy/test/base_test_case.py
 prophecy/test/utils.py
 prophecy/udfs/__init__.py
 prophecy/udfs/rest_api_udf.py
 prophecy/udfs/sample_udf.py
 prophecy/udfs/scala_udf_wrapper.py
 prophecy/utils/__init__.py
+prophecy/utils/functions.py
 prophecy/utils/gems_utils.py
 prophecy/utils/metagem_utils.py
 prophecy/utils/utils.py
 prophecy/utils/transpiler/__init__.py
 prophecy/utils/transpiler/abi_base.py
 prophecy/utils/transpiler/abi_core_fcns.py
 prophecy/utils/transpiler/abi_fcn_wrapper.py
```


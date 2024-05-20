# Comparing `tmp/rov_db_access-1.0.0.tar.gz` & `tmp/rov_db_access-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-1.0.0.tar", max compression
+gzip compressed data, was "rov_db_access-1.0.1.tar", max compression
```

## Comparing `rov_db_access-1.0.0.tar` & `rov_db_access-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      587 2024-05-17 19:53:02.768503 rov_db_access-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-1.0.0/README.md
--rw-r--r--   0        0        0      359 2024-05-07 17:08:16.858586 rov_db_access-1.0.0/rov_db_access/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-1.0.0/rov_db_access/authentication/__init__.py
--rw-r--r--   0        0        0     2324 2024-05-07 15:18:49.279026 rov_db_access-1.0.0/rov_db_access/authentication/models.py
--rw-r--r--   0        0        0     1233 2024-05-17 19:52:58.172569 rov_db_access-1.0.0/rov_db_access/authentication/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 19:52:58.172569 rov_db_access-1.0.0/rov_db_access/config/__init__.py
--rw-r--r--   0        0        0     2133 2024-05-14 15:53:52.686829 rov_db_access-1.0.0/rov_db_access/config/db_utils.py
--rw-r--r--   0        0        0      939 2024-05-17 19:52:58.173574 rov_db_access-1.0.0/rov_db_access/config/settings.py
--rw-r--r--   0        0        0        0 2024-05-17 19:52:58.174567 rov_db_access-1.0.0/rov_db_access/geodata/__init__.py
--rw-r--r--   0        0        0     2032 2024-05-17 19:52:58.176075 rov_db_access-1.0.0/rov_db_access/geodata/models.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-1.0.0/rov_db_access/gis/__init__.py
--rw-r--r--   0        0        0     7617 2024-05-15 19:14:44.177669 rov_db_access-1.0.0/rov_db_access/gis/models.py
--rw-r--r--   0        0        0       81 2024-05-17 19:52:58.176594 rov_db_access-1.0.0/rov_db_access/gis/test.py
--rw-r--r--   0        0        0    35434 2024-05-17 19:52:58.177603 rov_db_access-1.0.0/rov_db_access/gis/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 19:52:58.178602 rov_db_access-1.0.0/rov_db_access/ine/__init__.py
--rw-r--r--   0        0        0      875 2024-05-17 19:52:58.178602 rov_db_access-1.0.0/rov_db_access/ine/models.py
--rw-r--r--   0        0        0     2368 2024-05-17 19:52:58.179605 rov_db_access-1.0.0/rov_db_access/ine/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 19:52:58.179605 rov_db_access-1.0.0/rov_db_access/label_studio/__init__.py
--rw-r--r--   0        0        0     9336 2024-05-17 19:52:58.180604 rov_db_access-1.0.0/rov_db_access/label_studio/models.py
--rw-r--r--   0        0        0     7363 2024-05-17 19:52:58.181603 rov_db_access-1.0.0/rov_db_access/label_studio/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 19:52:58.181603 rov_db_access-1.0.0/rov_db_access/landing/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-17 19:52:58.182603 rov_db_access-1.0.0/rov_db_access/landing/models.py
--rw-r--r--   0        0        0     6062 2024-05-17 19:52:58.183605 rov_db_access-1.0.0/rov_db_access/landing/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 19:52:58.184605 rov_db_access-1.0.0/rov_db_access/risks/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-17 19:52:58.184605 rov_db_access-1.0.0/rov_db_access/risks/models.py
--rw-r--r--   0        0        0     6703 2024-05-17 19:52:58.184605 rov_db_access-1.0.0/rov_db_access/risks/worker.py
--rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-1.0.0/rov_db_access/sentinel/__init__.py
--rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-1.0.0/rov_db_access/sentinel/models.py
--rw-r--r--   0        0        0     6053 2024-05-17 19:52:58.186636 rov_db_access-1.0.0/rov_db_access/sentinel/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 19:52:58.186636 rov_db_access-1.0.0/rov_db_access/utils/__init__.py
--rw-r--r--   0        0        0     2022 2024-05-17 19:52:58.186636 rov_db_access-1.0.0/rov_db_access/utils/s3_utils.py
--rw-r--r--   0        0        0     1157 2024-05-17 19:52:58.187649 rov_db_access-1.0.0/rov_db_access/utils/utils.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      587 2024-05-20 15:42:57.563641 rov_db_access-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 17:20:32.047625 rov_db_access-1.0.1/README.md
+-rw-r--r--   0        0        0      359 2024-05-07 17:20:32.051852 rov_db_access-1.0.1/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:20:32.052868 rov_db_access-1.0.1/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2324 2024-05-16 19:12:21.968534 rov_db_access-1.0.1/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     1233 2024-05-17 19:53:13.581924 rov_db_access-1.0.1/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:53:13.581924 rov_db_access-1.0.1/rov_db_access/config/__init__.py
+-rw-r--r--   0        0        0     2133 2024-05-14 19:49:24.218901 rov_db_access-1.0.1/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0      939 2024-05-17 19:53:13.582923 rov_db_access-1.0.1/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:53:13.582923 rov_db_access-1.0.1/rov_db_access/geodata/__init__.py
+-rw-r--r--   0        0        0     2032 2024-05-17 19:53:13.584023 rov_db_access-1.0.1/rov_db_access/geodata/models.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:20:32.058935 rov_db_access-1.0.1/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     7617 2024-05-16 19:27:51.940053 rov_db_access-1.0.1/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0       81 2024-05-17 19:53:13.584023 rov_db_access-1.0.1/rov_db_access/gis/test.py
+-rw-r--r--   0        0        0    35563 2024-05-20 15:42:57.565005 rov_db_access-1.0.1/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:53:13.585408 rov_db_access-1.0.1/rov_db_access/ine/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-17 19:53:13.585408 rov_db_access-1.0.1/rov_db_access/ine/models.py
+-rw-r--r--   0        0        0     2368 2024-05-17 19:53:13.586765 rov_db_access-1.0.1/rov_db_access/ine/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:53:13.586765 rov_db_access-1.0.1/rov_db_access/label_studio/__init__.py
+-rw-r--r--   0        0        0     9336 2024-05-17 19:53:13.588172 rov_db_access-1.0.1/rov_db_access/label_studio/models.py
+-rw-r--r--   0        0        0     7363 2024-05-17 19:53:13.588172 rov_db_access-1.0.1/rov_db_access/label_studio/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:53:13.588172 rov_db_access-1.0.1/rov_db_access/landing/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-17 19:53:13.589179 rov_db_access-1.0.1/rov_db_access/landing/models.py
+-rw-r--r--   0        0        0     6062 2024-05-17 19:53:13.590180 rov_db_access-1.0.1/rov_db_access/landing/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:53:13.590180 rov_db_access-1.0.1/rov_db_access/risks/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-17 19:53:13.591254 rov_db_access-1.0.1/rov_db_access/risks/models.py
+-rw-r--r--   0        0        0     6703 2024-05-17 19:53:13.591254 rov_db_access-1.0.1/rov_db_access/risks/worker.py
+-rw-r--r--   0        0        0        0 2024-05-07 17:20:32.063358 rov_db_access-1.0.1/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-16 19:20:38.867932 rov_db_access-1.0.1/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     6053 2024-05-17 19:53:13.591254 rov_db_access-1.0.1/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:53:13.592761 rov_db_access-1.0.1/rov_db_access/utils/__init__.py
+-rw-r--r--   0        0        0     2022 2024-05-17 19:53:13.593768 rov_db_access-1.0.1/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1157 2024-05-17 19:53:13.593768 rov_db_access-1.0.1/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.1/PKG-INFO
```

### Comparing `rov_db_access-1.0.0/pyproject.toml` & `rov_db_access-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rov-db-access"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Pablo Cano <pablo.cano@rovisen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 geoalchemy2 = "^0.14.2"
```

### Comparing `rov_db_access-1.0.0/rov_db_access/authentication/models.py` & `rov_db_access-1.0.1/rov_db_access/authentication/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/authentication/worker.py` & `rov_db_access-1.0.1/rov_db_access/authentication/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/config/db_utils.py` & `rov_db_access-1.0.1/rov_db_access/config/db_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/config/settings.py` & `rov_db_access-1.0.1/rov_db_access/config/settings.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/geodata/models.py` & `rov_db_access-1.0.1/rov_db_access/geodata/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/gis/models.py` & `rov_db_access-1.0.1/rov_db_access/gis/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/gis/worker.py` & `rov_db_access-1.0.1/rov_db_access/gis/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -889,13 +889,16 @@
                         "runtime": run.runtime,
                         "cost": run.cost,
                         "data": run.data,
                         "process_id": run.process_id,
                         "process_name": run.process.name,
                         "mask": wkbelement_to_wkt(run.process.mask),
                         "inference_model_id": run.inference_model_id,
-                        "input_id": run.input_id,
-                        "input_data": run.input.data,
                         "organization_id": run.process.organization_id,
-                        "organization_name": run.process.organization.name
+                        "organization_name": run.process.organization.name,
+                        "input":{
+                            "input_id": run.input_id,
+                            "input_type": run.input.type,
+                            "input_data": run.input.data
+                        }
                     })
                 return results
```

### Comparing `rov_db_access-1.0.0/rov_db_access/ine/models.py` & `rov_db_access-1.0.1/rov_db_access/ine/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/ine/worker.py` & `rov_db_access-1.0.1/rov_db_access/ine/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/label_studio/models.py` & `rov_db_access-1.0.1/rov_db_access/label_studio/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/label_studio/worker.py` & `rov_db_access-1.0.1/rov_db_access/label_studio/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/landing/models.py` & `rov_db_access-1.0.1/rov_db_access/landing/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/landing/worker.py` & `rov_db_access-1.0.1/rov_db_access/landing/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/risks/models.py` & `rov_db_access-1.0.1/rov_db_access/risks/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/risks/worker.py` & `rov_db_access-1.0.1/rov_db_access/risks/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/sentinel/worker.py` & `rov_db_access-1.0.1/rov_db_access/sentinel/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/utils/s3_utils.py` & `rov_db_access-1.0.1/rov_db_access/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/rov_db_access/utils/utils.py` & `rov_db_access-1.0.1/rov_db_access/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.0/PKG-INFO` & `rov_db_access-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


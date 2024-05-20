# Comparing `tmp/increff_runner-4.1-py3-none-any.whl.zip` & `tmp/increff_runner-4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 12997 bytes, number of entries: 16
+Zip file size: 13055 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-05 05:14 increff_runner/__init__.py
 -rw-r--r--  2.0 unx     9847 b- defN 24-May-08 08:15 increff_runner/function.py
 -rw-r--r--  2.0 unx     4143 b- defN 24-Feb-22 04:41 increff_runner/commons/algo_block_downloader.py
--rw-r--r--  2.0 unx     2757 b- defN 24-May-08 08:15 increff_runner/commons/callback_helper.py
+-rw-r--r--  2.0 unx     2982 b- defN 24-May-15 06:12 increff_runner/commons/callback_helper.py
 -rw-r--r--  2.0 unx      351 b- defN 24-Feb-15 07:21 increff_runner/commons/constants.py
 -rw-r--r--  2.0 unx     3559 b- defN 24-May-08 08:15 increff_runner/commons/db_helper.py
 -rw-r--r--  2.0 unx      905 b- defN 24-Feb-22 04:41 increff_runner/commons/db_service.py
 -rw-r--r--  2.0 unx      481 b- defN 24-May-08 08:15 increff_runner/commons/event_helper.py
 -rw-r--r--  2.0 unx     8405 b- defN 24-May-07 09:07 increff_runner/commons/graphdb_helper.py
 -rw-r--r--  2.0 unx     3075 b- defN 24-May-08 09:05 increff_runner/commons/mse_helper.py
 -rw-r--r--  2.0 unx      687 b- defN 24-Feb-22 04:41 increff_runner/commons/setup.py
 -rw-r--r--  2.0 unx     2104 b- defN 24-Feb-22 04:41 increff_runner/commons/utils.py
--rw-r--r--  2.0 unx      610 b- defN 24-May-08 09:06 increff_runner-4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 09:06 increff_runner-4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-May-08 09:06 increff_runner-4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1416 b- defN 24-May-08 09:06 increff_runner-4.1.dist-info/RECORD
-16 files, 38447 bytes uncompressed, 10619 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx      610 b- defN 24-May-15 06:13 increff_runner-4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 06:13 increff_runner-4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-15 06:13 increff_runner-4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1416 b- defN 24-May-15 06:13 increff_runner-4.2.dist-info/RECORD
+16 files, 38672 bytes uncompressed, 10677 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: increff_runner/commons/setup.py
 Comment: 
 
 Filename: increff_runner/commons/utils.py
 Comment: 
 
-Filename: increff_runner-4.1.dist-info/METADATA
+Filename: increff_runner-4.2.dist-info/METADATA
 Comment: 
 
-Filename: increff_runner-4.1.dist-info/WHEEL
+Filename: increff_runner-4.2.dist-info/WHEEL
 Comment: 
 
-Filename: increff_runner-4.1.dist-info/top_level.txt
+Filename: increff_runner-4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: increff_runner-4.1.dist-info/RECORD
+Filename: increff_runner-4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## increff_runner/commons/callback_helper.py

```diff
@@ -47,15 +47,19 @@
     update_job(job)
     response = requests.post(url, data=json.dumps(body))
 
 
 def send_failure_webhook(url, task_id, error, job):
     node = get_task_node(job["data"]["algo_name"],task_id,job["data"]["level"])
     add_error_logs(job["id"], "Hitting Failure WebHook Callback with error -> "+str(error))
-    data = {"status": "FAILED", "taskId": task_id, "subtaskName":  node['parent_task'],"reason":str(error)}
+    err_dict = json.loads(error)
+    if 'is_warning' in err_dict and err_dict['is_warning'] == 1:
+        data = {"status": "WARNING", "taskId": task_id, "subtaskName":  node['parent_task'],"reason":str(error)}
+    else:
+        data = {"status": "FAILED", "taskId": task_id, "subtaskName":  node['parent_task'],"reason":str(error)}
 
     headers = {
         "Content-Type": "application/json",
         "authUsername":"caas-user@increff.com",
         "authPassword":"caasuser@123",
         "authdomainname": job["data"]["client"],
         "Conection":"keep-alive"
```

## Comparing `increff_runner-4.1.dist-info/METADATA` & `increff_runner-4.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increff-runner
-Version: 4.1
+Version: 4.2
 Summary: Algo Runner For Increff CaaS
 Author: Jaynit Patel
 Author-email: jaynitpatel11062001@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pytz ==2023.3.post1
 Requires-Dist: requests ==2.31.0
 Requires-Dist: azure-functions ==1.12.0
```

## Comparing `increff_runner-4.1.dist-info/RECORD` & `increff_runner-4.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 increff_runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 increff_runner/function.py,sha256=blXpb4Rx0WY9B4_iZnqbyzhn0yTDeV_i9eOiNGv8KOU,9847
 increff_runner/commons/algo_block_downloader.py,sha256=JSZLYpIuWhybRD13sHPu_05X4KoeMApa5qELLkqA9R4,4143
-increff_runner/commons/callback_helper.py,sha256=eLlRYyjLqsq6_GvNn78FhwvQd6Qq0nybS1TSJWihfDU,2757
+increff_runner/commons/callback_helper.py,sha256=-NfXzU_wOL9-fQF2lf9Kk14eEU1qpHUfvgvAhTZOIEI,2982
 increff_runner/commons/constants.py,sha256=dJRawPQQduTe1BqN6SrLYYpzI5bVqS6AbuYwj6Qa6is,351
 increff_runner/commons/db_helper.py,sha256=APr9mTd2RkEL1caxysuUgmCVQBH-izskLbVjpAf_Alo,3559
 increff_runner/commons/db_service.py,sha256=5PtU_AQCwm5FVmRXjJprysNoIy_vKt06vN1IlnxuH-c,905
 increff_runner/commons/event_helper.py,sha256=5aILmAJwk3TxiUYGKkmjh7rGwIJdu3ybTAcLbg8ApRI,481
 increff_runner/commons/graphdb_helper.py,sha256=c6cnD2He-xMer4dejiFKvAvM1qsbPlDoNqNKkz1mtZE,8405
 increff_runner/commons/mse_helper.py,sha256=aYHf3KLk5iqIXP1MgVR2HD8q7-pTA2cVrWJeL6g9YWo,3075
 increff_runner/commons/setup.py,sha256=iwg58X1DKaSP8hKlXLvH5OXSEW8N_UuRMDb2CocaAfY,687
 increff_runner/commons/utils.py,sha256=PUKWRMYzTTWK7pTK2S5DM0szru4zGmmVKfPpXhnmPUM,2104
-increff_runner-4.1.dist-info/METADATA,sha256=h1zPwKAZ67Lx5dAj3r3p5jIRCVegiR1m3ukVmxAL-DM,610
-increff_runner-4.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-increff_runner-4.1.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
-increff_runner-4.1.dist-info/RECORD,,
+increff_runner-4.2.dist-info/METADATA,sha256=Kt3zf5_JOQzq8DmtjIHO8-OA6njRoxUN4tOqoXDKo6Y,610
+increff_runner-4.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+increff_runner-4.2.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
+increff_runner-4.2.dist-info/RECORD,,
```


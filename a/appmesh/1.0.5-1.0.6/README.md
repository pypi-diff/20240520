# Comparing `tmp/appmesh-1.0.5-py3-none-any.whl.zip` & `tmp/appmesh-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16156 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-16 13:35 appmesh/__init__.py
--rw-r--r--  2.0 unx    58981 b- defN 24-May-16 13:35 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-May-16 13:35 appmesh-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 13:35 appmesh-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-16 13:35 appmesh-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-16 13:35 appmesh-1.0.5.dist-info/RECORD
-6 files, 70333 bytes uncompressed, 15334 bytes compressed:  78.2%
+Zip file size: 16174 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-19 23:30 appmesh/__init__.py
+-rw-r--r--  2.0 unx    59018 b- defN 24-May-19 23:30 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-May-19 23:31 appmesh-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-19 23:31 appmesh-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-19 23:31 appmesh-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-19 23:31 appmesh-1.0.6.dist-info/RECORD
+6 files, 70370 bytes uncompressed, 15352 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-1.0.5.dist-info/METADATA
+Filename: appmesh-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-1.0.5.dist-info/WHEEL
+Filename: appmesh-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-1.0.5.dist-info/top_level.txt
+Filename: appmesh-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-1.0.5.dist-info/RECORD
+Filename: appmesh-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -12,15 +12,15 @@
 
 from enum import Enum, unique
 from http import HTTPStatus
 from urllib import parse
 from datetime import datetime
 import requests
 
-# pylint: disable=broad-exception-raised,line-too-long
+# pylint: disable=broad-exception-raised,line-too-long,broad-exception-caught
 
 DEFAULT_TOKEN_EXPIRE_SECONDS = "P1W"  # default 7 day(s)
 DEFAULT_RUN_APP_TIMEOUT_SECONDS = "PT1H"  # 1 hour
 DEFAULT_RUN_APP_LIFECYCLE_SECONDS = "PT10H"  # 10 hours
 REST_TEXT_MESSAGE_JSON_KEY = "message"
 MESSAGE_ENCODING_UTF8 = "utf-8"
 TCP_MESSAGE_HEADER_LENGTH = 4
@@ -447,15 +447,15 @@
             totp_code (str): TOTP code
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
-            path=f"/appmesh/totp/setup",
+            path="/appmesh/totp/setup",
             header={"Totp": base64.b64encode(totp_code.encode())},
         )
         if resp.status_code != HTTPStatus.OK:
             raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
     def totp_disable(self, user="self") -> bool:
@@ -789,18 +789,18 @@
 
         Args:
             level (str, optional): log level.
 
         Returns:
             str: the updated log level.
         """
-        resp = self._request_http(AppMeshClient.Method.POST, path="/appmesh/config", body={"LogLevel": level})
+        resp = self._request_http(AppMeshClient.Method.POST, path="/appmesh/config", body={"BaseConfig": {"LogLevel": level}})
         if resp.status_code != HTTPStatus.OK:
             raise Exception(resp.text)
-        return resp.json()["LogLevel"]
+        return resp.json()["BaseConfig"]["LogLevel"]
 
     ########################################
     # User Management
     ########################################
     def user_passwd_update(self, new_password: str, user_name: str = "self") -> bool:
         """Change user password
 
@@ -1414,15 +1414,15 @@
         resp_data = self.__recvall(int.from_bytes(self.__recvall(TCP_MESSAGE_HEADER_LENGTH), "big", signed=False))
         if resp_data is None or len(resp_data) == 0:
             self.__close_socket()
             raise Exception("socket connection broken")
         appmesh_resp = ResponseMsg().desirialize(resp_data)
         http_resp = requests.Response()
         http_resp.status_code = appmesh_resp.http_status
-        http_resp._content = appmesh_resp.body if "application/octet-stream" in appmesh_resp.body_msg_type.lower() else appmesh_resp.body.encode("utf8")
+        http_resp._content = appmesh_resp.body if "application/octet-stream" in appmesh_resp.body_msg_type.lower() else appmesh_resp.body
         http_resp.headers = appmesh_resp.headers
         http_resp.encoding = MESSAGE_ENCODING_UTF8
         if appmesh_resp.body_msg_type:
             http_resp.headers["Content-Type"] = appmesh_resp.body_msg_type
         assert req_id == appmesh_resp.uuid
         return http_resp
```

## Comparing `appmesh-1.0.5.dist-info/METADATA` & `appmesh-1.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 1.0.5
+Version: 1.0.6
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 1.0.5 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 1.0.6 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```


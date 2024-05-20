# Comparing `tmp/api-nichotined-0.1.7.tar.gz` & `tmp/api-nichotined-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-nichotined-0.1.7.tar", last modified: Thu May  2 18:15:55 2024, max compression
+gzip compressed data, was "api-nichotined-0.1.9.tar", last modified: Fri May  3 08:28:57 2024, max compression
```

## Comparing `api-nichotined-0.1.7.tar` & `api-nichotined-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.432044 api-nichotined-0.1.7/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-02 18:15:55.431794 api-nichotined-0.1.7/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      877 2024-05-01 15:39:36.000000 api-nichotined-0.1.7/README.md
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.428541 api-nichotined-0.1.7/api_nichotined/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      130 2024-05-01 16:18:29.000000 api-nichotined-0.1.7/api_nichotined/__init__.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.429954 api-nichotined-0.1.7/api_nichotined/core/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.7/api_nichotined/core/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     2198 2024-05-01 16:14:45.000000 api-nichotined-0.1.7/api_nichotined/core/core.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      995 2024-05-01 16:27:20.000000 api-nichotined-0.1.7/api_nichotined/core/response.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.430795 api-nichotined-0.1.7/api_nichotined/utillity/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-27 13:10:31.000000 api-nichotined-0.1.7/api_nichotined/utillity/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1375 2024-05-01 12:24:28.000000 api-nichotined-0.1.7/api_nichotined/utillity/bq.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       53 2024-04-27 13:11:27.000000 api-nichotined-0.1.7/api_nichotined/utillity/pq.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.431549 api-nichotined-0.1.7/api_nichotined.egg-info/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      452 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       39 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/requires.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/top_level.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-05-02 18:15:55.432098 api-nichotined-0.1.7/setup.cfg
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      750 2024-05-02 17:28:35.000000 api-nichotined-0.1.7/setup.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.431191 api-nichotined-0.1.7/test/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.7/test/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      768 2024-05-01 16:31:04.000000 api-nichotined-0.1.7/test/main.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-03 08:28:57.694806 api-nichotined-0.1.9/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-03 08:28:57.694609 api-nichotined-0.1.9/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      877 2024-05-01 15:39:36.000000 api-nichotined-0.1.9/README.md
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-03 08:28:57.692309 api-nichotined-0.1.9/api_nichotined/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      130 2024-05-01 16:18:29.000000 api-nichotined-0.1.9/api_nichotined/__init__.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-03 08:28:57.693386 api-nichotined-0.1.9/api_nichotined/core/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.9/api_nichotined/core/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     2351 2024-05-03 08:27:44.000000 api-nichotined-0.1.9/api_nichotined/core/core.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1174 2024-05-02 18:25:41.000000 api-nichotined-0.1.9/api_nichotined/core/response.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-03 08:28:57.693861 api-nichotined-0.1.9/api_nichotined/utillity/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-27 13:10:31.000000 api-nichotined-0.1.9/api_nichotined/utillity/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1375 2024-05-01 12:24:28.000000 api-nichotined-0.1.9/api_nichotined/utillity/bq.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       53 2024-04-27 13:11:27.000000 api-nichotined-0.1.9/api_nichotined/utillity/pq.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-03 08:28:57.694398 api-nichotined-0.1.9/api_nichotined.egg-info/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-03 08:28:57.000000 api-nichotined-0.1.9/api_nichotined.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      452 2024-05-03 08:28:57.000000 api-nichotined-0.1.9/api_nichotined.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-05-03 08:28:57.000000 api-nichotined-0.1.9/api_nichotined.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       39 2024-05-03 08:28:57.000000 api-nichotined-0.1.9/api_nichotined.egg-info/requires.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-05-03 08:28:57.000000 api-nichotined-0.1.9/api_nichotined.egg-info/top_level.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-05-03 08:28:57.694852 api-nichotined-0.1.9/setup.cfg
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      750 2024-05-03 08:28:00.000000 api-nichotined-0.1.9/setup.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-03 08:28:57.694227 api-nichotined-0.1.9/test/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.9/test/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      768 2024-05-01 16:31:04.000000 api-nichotined-0.1.9/test/main.py
```

### Comparing `api-nichotined-0.1.7/PKG-INFO` & `api-nichotined-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-nichotined
-Version: 0.1.7
+Version: 0.1.9
 Summary: Simple lib for testing rest API
 Home-page: https://github.com/nichotined/simple-api
 Author: Nicholas Frederich
 Author-email: nicholas.frederich.lagaunne@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-nichotined-0.1.7/README.md` & `api-nichotined-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `api-nichotined-0.1.7/api_nichotined/core/core.py` & `api-nichotined-0.1.9/api_nichotined/core/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import logging
 
 import curlify
 from requests import Response, Session
 
-from api_nichotined.core.response import ResponseWrapper
+from api_nichotined.core.response import ResponseHandler
 
 
 class Api:
     def __init__(self, base_url):
         self.base_url = base_url
         self.session = Session()
         self.logger = logging.getLogger(__name__)
 
     def close_session(self):
         if self.session:
             self.session.close()
 
     def _make_request(self, method, path, params=None, data=None, json_data=None, headers=None,
-                      auth=None) -> ResponseWrapper:
+                      auth=None, files=None) -> ResponseHandler:
         url = self.base_url + path
         self.logger.info(f"Making {method} request to {url}")
 
         response = self.session.request(method, url, params=params, data=data, json=json_data, headers=headers,
-                                        auth=auth)
+                                        auth=auth, files=files)
 
         self.log_response(response)
-        return ResponseWrapper(response)
+        return ResponseHandler(response)
 
     def log_response(self, response: Response):
         curl = curlify.to_curl(response.request)
         self.logger.info(curl)
         self.logger.info(f"Response received with status code {response.status_code}")
         self.logger.info(response.json())
 
-    def get(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> ResponseWrapper:
+    def get(self, path, params=None, data=None, json_data=None, headers=None, auth=None, files=None) -> ResponseHandler:
         return self._make_request("GET", path, params=params, data=data, headers=headers, json_data=json_data,
-                                  auth=auth)
+                                  auth=auth, files=files)
 
-    def post(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> ResponseWrapper:
+    def post(self, path, params=None, data=None, json_data=None, headers=None, auth=None,
+             files=None) -> ResponseHandler:
         return self._make_request("POST", path, params=params, data=data, headers=headers, json_data=json_data,
-                                  auth=auth)
+                                  auth=auth, files=files)
 
-    def put(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> ResponseWrapper:
+    def put(self, path, params=None, data=None, json_data=None, headers=None, auth=None, files=None) -> ResponseHandler:
         return self._make_request("PUT", path, params=params, data=data, headers=headers, json_data=json_data,
-                                  auth=auth)
+                                  auth=auth, files=files)
 
-    def delete(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> ResponseWrapper:
+    def delete(self, path, params=None, data=None, json_data=None, headers=None, auth=None,
+               files=None) -> ResponseHandler:
         return self._make_request("DELETE", path, params=params, data=data, headers=headers, json_data=json_data,
-                                  auth=auth)
+                                  auth=auth, files=files)
```

### Comparing `api-nichotined-0.1.7/api_nichotined/core/response.py` & `api-nichotined-0.1.9/api_nichotined/core/response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-from requests import Response
+from requests import Response, PreparedRequest
 from requests.status_codes import codes
 
 
 class JsonToPythonHook:
     def __init__(self, json_data):
         self.__dict__ = json_data
 
 
-class ResponseWrapper:
+class ResponseHandler:
     def __init__(self, response: Response):
-        self._response = response
+        self._resp = response
 
     @property
-    def response(self):
-        return self._response
+    def resp(self) -> Response:
+        return self._resp
+
+    @property
+    def req(self) -> PreparedRequest:
+        return self._resp.request
 
     @property
     def body(self):
-        return self._response.json(object_hook=JsonToPythonHook)
+        return self._resp.json(object_hook=JsonToPythonHook)
+
+    @property
+    def status_code(self) -> int:
+        return self._resp.status_code
 
     def is_array(self) -> bool:
         """
         Check if response body is in array instead of object
         :return: bool
         """
         return type(self.body) == list
 
     def is_success(self):
         """
         Check if status code is equal to 200
         :return: bool
         """
-        return self._response.status_code == codes.okay
+        return self._resp.status_code == codes.okay
 
     def is_internal_server_error(self):
         """
         Check if status code is equal to 500
         :return: bool
         """
-        return self._response.status_code == codes.internal_server_error
+        return self._resp.status_code == codes.internal_server_error
```

### Comparing `api-nichotined-0.1.7/api_nichotined/utillity/bq.py` & `api-nichotined-0.1.9/api_nichotined/utillity/bq.py`

 * *Files identical despite different names*

### Comparing `api-nichotined-0.1.7/api_nichotined.egg-info/PKG-INFO` & `api-nichotined-0.1.9/api_nichotined.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-nichotined
-Version: 0.1.7
+Version: 0.1.9
 Summary: Simple lib for testing rest API
 Home-page: https://github.com/nichotined/simple-api
 Author: Nicholas Frederich
 Author-email: nicholas.frederich.lagaunne@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-nichotined-0.1.7/setup.py` & `api-nichotined-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="api-nichotined",
-    version="0.1.7",
+    version="0.1.9",
     author="Nicholas Frederich",
     author_email="nicholas.frederich.lagaunne@gmail.com",
     description="Simple lib for testing rest API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nichotined/simple-api",
     packages=setuptools.find_packages(),
```

### Comparing `api-nichotined-0.1.7/test/main.py` & `api-nichotined-0.1.9/test/main.py`

 * *Files identical despite different names*


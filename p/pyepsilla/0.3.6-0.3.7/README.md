# Comparing `tmp/pyepsilla-0.3.6.tar.gz` & `tmp/pyepsilla-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.3.6.tar", last modified: Fri Apr 26 16:01:43 2024, max compression
+gzip compressed data, was "pyepsilla-0.3.7.tar", last modified: Mon May 20 15:37:05 2024, max compression
```

## Comparing `pyepsilla-0.3.6.tar` & `pyepsilla-0.3.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.688896 pyepsilla-0.3.6/pyepsilla/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.688896 pyepsilla-0.3.6/pyepsilla/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/cloud/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.688896 pyepsilla-0.3.6/pyepsilla/enterprise/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/enterprise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/enterprise/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/enterprise/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.688896 pyepsilla-0.3.6/pyepsilla/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10361 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/utils/search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/pyepsilla/vectordb/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/pyepsilla/vectordb/machineid/
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/machineid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/machineid/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/pyepsilla/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/utils/embedding_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/pyepsilla/vectordb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/pyepsilla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 16:01:43.000000 pyepsilla-0.3.6/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:01:43.692896 pyepsilla-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-26 16:01:32.000000 pyepsilla-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.664674 pyepsilla-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 15:37:05.664674 pyepsilla-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.656674 pyepsilla-0.3.7/pyepsilla/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.660674 pyepsilla-0.3.7/pyepsilla/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12004 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/cloud/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.660674 pyepsilla-0.3.7/pyepsilla/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/enterprise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/enterprise/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/enterprise/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.660674 pyepsilla-0.3.7/pyepsilla/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10361 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/utils/search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.660674 pyepsilla-0.3.7/pyepsilla/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.660674 pyepsilla-0.3.7/pyepsilla/vectordb/machineid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/machineid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/machineid/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.660674 pyepsilla-0.3.7/pyepsilla/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/utils/embedding_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/pyepsilla/vectordb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:37:05.660674 pyepsilla-0.3.7/pyepsilla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 15:37:05.000000 pyepsilla-0.3.7/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-20 15:37:05.000000 pyepsilla-0.3.7/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:37:05.000000 pyepsilla-0.3.7/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 15:37:05.000000 pyepsilla-0.3.7/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 15:37:05.000000 pyepsilla-0.3.7/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:37:05.664674 pyepsilla-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-20 15:36:55.000000 pyepsilla-0.3.7/setup.py
```

### Comparing `pyepsilla-0.3.6/LICENSE.txt` & `pyepsilla-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.6/README.md` & `pyepsilla-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.6/pyepsilla/cloud/client.py` & `pyepsilla-0.3.7/pyepsilla/cloud/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from __future__ import annotations
 
 import datetime
 import json
 import pprint
 import socket
 from typing import Optional, Union
-from ..utils.search_engine import SearchEngine
 
 import requests
 import sentry_sdk
 from pydantic import BaseModel, Field, constr
 
+from ..utils.search_engine import SearchEngine
+
 requests.packages.urllib3.disable_warnings()
 
 
 class Client(object):
     def __init__(self, project_id: str, api_key: str, headers: dict = None):
         self._project_id = project_id
         self._apikey = api_key
@@ -29,61 +30,65 @@
             "Connection": "close",
             "X-API-Key": api_key,
         }
         if headers is not None:
             self._header.update(headers)
 
     def validate(self):
-        res = requests.get(
+        resp = requests.get(
             url=self._baseurl + "/vectordb/list",
             data=None,
             headers=self._header,
             verify=False,
         )
-        data = res.json()
-        res.close()
+        data = resp.json()
+        resp.close()
+        del resp
         return data
 
     def get_db_list(self):
         db_list = []
         req_url = "{}/vectordb/list".format(self._baseurl)
-        res = requests.get(url=req_url, data=None, headers=self._header, verify=False)
-        status_code = res.status_code
-        body = res.json()
+        resp = requests.get(url=req_url, data=None, headers=self._header, verify=False)
+        status_code = resp.status_code
+        body = resp.json()
         if status_code == 200 and body["statusCode"] == 200:
-            db_list = [db_id for db_id in res.json()["result"]]
-        res.close()
+            db_list = [db_id for db_id in body["result"]]
+        resp.close()
+        del resp
         return db_list
 
     def get_db_info(self, db_id: str):
         req_url = "{}/vectordb/{}".format(self._baseurl, db_id)
-        res = requests.get(url=req_url, data=None, headers=self._header, verify=False)
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        resp = requests.get(url=req_url, data=None, headers=self._header, verify=False)
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def get_db_statistics(self, db_id: str):
         req_url = "{}/vectordb/{}/statistics".format(self._baseurl, db_id)
         req_data = None
-        res = requests.get(
+        resp = requests.get(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def vectordb(self, db_id: str):
         # validate project_id and api_key
-        res = self.validate()
-        if res["statusCode"] != 200:
-            if res["statusCode"] == 404:
+        resp = self.validate()
+        if resp["statusCode"] != 200:
+            if resp["statusCode"] == 404:
                 raise Exception("Invalid project_id")
-            if res["statusCode"] == 401:
+            if resp["statusCode"] == 401:
                 raise Exception("Invalid api_key")
 
         # validate db_id
         db_list = self.get_db_list()
         if db_id not in db_list:
             raise Exception("Invalid db_id")
 
@@ -91,14 +96,15 @@
         status_code, resp = self.get_db_info(db_id=db_id)
         if resp["statusCode"] == 200:
             return Vectordb(
                 self._project_id, db_id, self._apikey, resp["result"]["public_endpoint"]
             )
         else:
             print(resp)
+            del resp
             raise Exception("Failed to get db info")
 
 
 class Vectordb(Client):
     def __init__(
         self,
         project_id: str,
@@ -119,18 +125,19 @@
             self._header.update(headers)
 
     # List table
     def list_tables(self):
         if self._db_id is None:
             raise Exception("[ERROR] db_id is None!")
         req_url = "{}/table/list".format(self._baseurl)
-        res = requests.get(url=req_url, headers=self._header, verify=False)
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        resp = requests.get(url=req_url, headers=self._header, verify=False)
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Create table
     def create_table(
         self,
         table_name: str,
         table_fields: list[dict] = None,
@@ -140,97 +147,115 @@
             raise Exception("[ERROR] db_id is None!")
         if table_fields is None:
             table_fields = []
         req_url = "{}/table/create".format(self._baseurl)
         req_data = {"name": table_name, "fields": table_fields}
         if indices is not None:
             req_data["indices"] = indices
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Drop table
     def drop_table(self, table_name: str):
         if self._db_id is None:
             raise Exception("[ERROR] db_id is None!")
         req_url = "{}/table/delete?table_name={}".format(self._baseurl, table_name)
         req_data = {}
-        res = requests.delete(
+        resp = requests.delete(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Insert data into table
     def insert(self, table_name: str, records: list[dict]):
         req_url = "{}/data/insert".format(self._baseurl)
         req_data = {"table": table_name, "data": records}
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def upsert(self, table_name: str, records: list[dict]):
         req_url = "{}/data/insert".format(self._baseurl)
         req_data = {"table": table_name, "data": records, "upsert": True}
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Query data from table
     def query(
         self,
         table_name: str,
         query_text: str = None,
         query_index: str = None,
         query_field: str = None,
         query_vector: Union[list, dict] = None,
         response_fields: Optional[list] = None,
         limit: int = 2,
         filter: Optional[str] = None,
         with_distance: Optional[bool] = False,
+        facets: Optional[list[dict]] = None,
     ):
         req_url = "{}/data/query".format(self._baseurl)
-        req_data = {"table": table_name}
+        req_data = {"table": table_name, "limit": limit}
+
+        if response_fields is None:
+            response_fields = []
+
         if query_text is not None:
             req_data["query"] = query_text
         if query_index is not None:
             req_data["queryIndex"] = query_index
-        if query_field != None:
+        if query_field is not None:
             req_data["queryField"] = query_field
-        if query_vector != None:
+        if query_vector is not None:
             req_data["queryVector"] = query_vector
-        if response_fields != None:
+        if response_fields is not None:
             req_data["response"] = response_fields
-        if limit != None:
-            req_data["limit"] = limit
-        if filter != None:
+        if filter is not None:
             req_data["filter"] = filter
-        if with_distance != None:
+        if with_distance is not False:
             req_data["withDistance"] = with_distance
 
-        res = requests.post(
+        if facets is not None and len(facets) > 0:
+            aggregate_not_existing = 0
+            for facet in facets:
+                if "aggregate" not in facet:
+                    aggregate_not_existing += 1
+            if aggregate_not_existing > 0:
+                raise Exception("[ERROR] key aggregate is a must in facets!")
+            else:
+                req_data["facets"] = facets
+
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Delete data from table
     def delete(
         self,
         table_name: str,
         primary_keys: Optional[list[Union[str, int]]] = None,
@@ -257,61 +282,75 @@
         req_url = "{}/data/delete".format(self._baseurl)
         req_data = {"table": table_name}
         if primary_keys is not None:
             req_data["primaryKeys"] = primary_keys
         if filter is not None:
             req_data["filter"] = filter
 
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Get data from table
     def get(
         self,
         table_name: str,
         response_fields: Optional[list] = None,
         primary_keys: Optional[list[Union[str, int]]] = None,
         ids: Optional[list[Union[str, int]]] = None,
         filter: Optional[str] = None,
         skip: Optional[int] = None,
         limit: Optional[int] = None,
+        facets: Optional[list[dict]] = None,
     ):
         """Epsilla supports get records by primary keys as default for now."""
         if primary_keys is not None and ids is not None:
             try:
                 sentry_sdk.sdk("Duplicate Keys with both primary_keys and ids", "info")
             except Exception as e:
                 pass
             print(
                 "[WARN]Both primary_keys and ids are prvoided, will use primary keys by default!"
             )
         if primary_keys is None and ids is not None:
             primary_keys = ids
 
         req_data = {"table": table_name}
+
         if response_fields is not None:
             req_data["response"] = response_fields
         if primary_keys is not None:
             req_data["primaryKeys"] = primary_keys
         if filter is not None:
             req_data["filter"] = filter
         if skip is not None:
             req_data["skip"] = skip
         if limit is not None:
             req_data["limit"] = limit
 
+        if facets is not None and len(facets) > 0:
+            aggregate_not_existing = 0
+            for facet in facets:
+                if "aggregate" not in facet:
+                    aggregate_not_existing += 1
+            if aggregate_not_existing > 0:
+                raise Exception("[ERROR] key aggregate is a must in facets!")
+            else:
+                req_data["facets"] = facets
+
         req_url = "{}/data/get".format(self._baseurl)
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def as_search_engine(self):
         return SearchEngine(self)
```

### Comparing `pyepsilla-0.3.6/pyepsilla/cloud/sentry.py` & `pyepsilla-0.3.7/pyepsilla/vectordb/sentry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,75 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 # Sentry collects crash reports and performance numbers
 # It is possible to turn off data collection using an environment variable named "SENTRY_DISABLE"
 
-import os, sys, platform, uuid, hashlib, socket, requests
+import hashlib
+import os
+import platform
+import socket
+import sys
+import uuid
+
+import requests
 import sentry_sdk
 from sentry_sdk.integrations.atexit import AtexitIntegration
-from pyepsilla.vectordb.version import __version__
 
+from .version import __version__
 
 CONFIG_URL = "https://config.epsilla.com/candidate.json"
-SENTRY_DSN = "https://c705adb9ba9a5750ab5719c69021e3b0@o4505952171917312.ingest.sentry.io/4506031458746368"
+SENTRY_DSN = "https://3f89b94a4a2e7620c8ecce81cb302d43@o4507288359862272.ingest.us.sentry.io/4507288364908545"
 
 try:
-    r = requests.get(CONFIG_URL, headers={"Agent": "PyEpsilla Cloud Client"}, timeout=2)
+    r = requests.get(CONFIG_URL, headers={"Agent": "PyEpsilla"}, timeout=2)
     if r.status_code == 200:
         SENTRY_DSN = r.json()["pyepsilla"][0]
 except Exception:
     pass
 
+
 def callback(pending, timeout):
     sys.stderr.flush()
-        
+
+
 def get_external_ip() -> str:
     try:
         return requests.get("https://api.ipify.org", timeout=2).text
     except Exception:
         return "NA"
 
+
 def init_sentry():
-    if "SENTRY_DISABLE" not in os.environ:
+    if os.getenv("SENTRY_DISABLE", None) is not None:
         try:
             uid = hashlib.sha256(str(uuid.getnode()).encode()).hexdigest()
             internal_ip = socket.gethostbyname(socket.gethostname())
             external_ip = get_external_ip()
             sentry_sdk.set_tag("uid", uid)
             sentry_sdk.set_tag("internal_ip", internal_ip)
             sentry_sdk.set_tag("external_ip", external_ip)
-            sentry_sdk.set_user({'ip_address': '{{auto}}'})
-            sentry_sdk.set_user({"username": "{}-{}-{}".format(socket.gethostname(), internal_ip, external_ip)})
+            sentry_sdk.set_user({"ip_address": "{{auto}}"})
+            sentry_sdk.set_user(
+                {
+                    "username": "{}-{}-{}".format(
+                        socket.gethostname(), internal_ip, external_ip
+                    )
+                }
+            )
             sentry_sdk.set_tag("version", platform.version())
-            sentry_sdk.set_tag("platform", "{}-{}".format(sys.platform, platform.machine()))
+            sentry_sdk.set_tag(
+                "platform", "{}-{}".format(sys.platform, platform.machine())
+            )
             sentry_sdk.init(
                 dsn=SENTRY_DSN,
                 release=__version__,
                 traces_sample_rate=1.0,
                 integrations=[AtexitIntegration(callback=callback)],
             )
 
-            sentry_sdk.capture_message("PyEpsilla Cloud Client Init", "info")
+            sentry_sdk.capture_message("PyEpsilla Init", "info")
         except Exception:
             sentry_sdk.flush()
             pass
+    else:
+        return None
```

### Comparing `pyepsilla-0.3.6/pyepsilla/enterprise/client.py` & `pyepsilla-0.3.7/pyepsilla/enterprise/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,29 +45,31 @@
     def hello(self):
         print("Hello Epsilla Enterprise!")
 
     # Get DB List
     def get_db_list(self):
         db_list = []
         req_url = "{}/vectordb/list".format(self._baseurl)
-        res = requests.get(url=req_url, data=None, headers=self._header, verify=False)
-        status_code = res.status_code
-        body = res.json()
+        resp = requests.get(url=req_url, data=None, headers=self._header, verify=False)
+        status_code = resp.status_code
+        body = resp.json()
         if status_code == 200 and body["statusCode"] == 200:
-            db_list = res.json()["result"]["uuids"]
-        res.close()
+            db_list = resp.json()["result"]["uuids"]
+        resp.close()
+        del resp
         return db_list
 
     # Get DB Information by db_id
     def get_db_info(self, db_id: str):
         req_url = "{}/vectordb/{}".format(self._baseurl, db_id)
-        res = requests.get(url=req_url, data=None, headers=self._header, verify=False)
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        resp = requests.get(url=req_url, data=None, headers=self._header, verify=False)
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Connect to DB
     def vectordb(self, db_id: str):
         # validate db_id
         if db_id not in self.get_db_list():
             raise Exception("Invalid db_id")
@@ -109,14 +111,15 @@
             data=json.dumps(req_data),
             headers=self._header,
             verify=False,
         )
         status_code = resp.status_code
         body = resp.json()
         resp.close()
+        del resp
         return status_code, body
 
     # Load DB
     def load_db(self, db_id: str):
         req_url = "{}/vectordb/{}/load".format(self._baseurl, db_id)
         req_data = {}
         resp = requests.post(
@@ -124,14 +127,15 @@
             data=json.dumps(req_data),
             headers=self._header,
             verify=False,
         )
         status_code = resp.status_code
         body = resp.json()
         resp.close()
+        del resp
         return status_code, body
 
     # Unload DB
     def unload_db(self, db_id: str):
         req_url = "{}/vectordb/{}/unload".format(self._baseurl, db_id)
         req_data = {}
         resp = requests.post(
@@ -139,14 +143,15 @@
             data=json.dumps(req_data),
             headers=self._header,
             verify=False,
         )
         status_code = resp.status_code
         body = resp.json()
         resp.close()
+        del resp
         return status_code, body
 
     # Delete DB
     def drop_db(self, db_id: str):
         req_url = "{}/vectordb/{}".format(self._baseurl, db_id)
         req_data = {}
         resp = requests.delete(
@@ -168,18 +173,18 @@
         self._header = header
 
     # List table
     def list_tables(self):
         if self._db_id is None:
             raise Exception("[ERROR] db_id is None!")
         req_url = "{}/table/list".format(self._baseurl)
-        res = requests.get(url=req_url, headers=self._header, verify=False)
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        resp = requests.get(url=req_url, headers=self._header, verify=False)
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
         return status_code, body
 
     # Create table
     def create_table(
         self,
         table_name: str,
         table_fields: list[dict] = None,
@@ -189,65 +194,69 @@
             raise Exception("[ERROR] db_id is None!")
         if table_fields is None:
             table_fields = []
         req_url = "{}/table/create".format(self._baseurl)
         req_data = {"name": table_name, "fields": table_fields}
         if indices is not None:
             req_data["indices"] = indices
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Drop table
     def drop_table(self, table_name: str):
         if self._db_id is None:
             raise Exception("[ERROR] db_id is None!")
         req_url = "{}/table/delete?table_name={}".format(self._baseurl, table_name)
         req_data = {}
-        res = requests.delete(
+        resp = requests.delete(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Insert data into table
     def insert(self, table_name: str, records: list[dict]):
         if self._db_id is None:
             raise Exception("[ERROR] db_id is None!")
         if records is None:
             records = []
         req_url = "{}/data/insert".format(self._baseurl)
         req_data = {"table": table_name, "data": records}
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def upsert(self, table_name: str, records: list[dict]):
         if self._db_id is None:
             raise Exception("[ERROR] db_id is None!")
         if records is None:
             records = []
         req_url = "{}/data/insert".format(self._baseurl)
         req_data = {"table": table_name, "data": records, "upsert": True}
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Query data from table
     def query(
         self,
         table_name: str,
         query_text: str = None,
@@ -257,129 +266,146 @@
         response_fields: Optional[list] = None,
         limit: int = 2,
         filter: Optional[str] = None,
         with_distance: Optional[bool] = False,
         facets: Optional[list[dict]] = None,
     ):
         req_url = "{}/data/query".format(self._baseurl)
-        req_data = {"table": table_name}
+        req_data = {"table": table_name, "limit": limit}
+
+        if response_fields is None:
+            response_fields = []
+
         if query_text is not None:
             req_data["query"] = query_text
         if query_index is not None:
             req_data["queryIndex"] = query_index
         if query_field is not None:
             req_data["queryField"] = query_field
         if query_vector is not None:
             req_data["queryVector"] = query_vector
         if response_fields is not None:
             req_data["response"] = response_fields
-        if limit is not None:
-            req_data["limit"] = limit
         if filter is not None:
             req_data["filter"] = filter
         if with_distance is not False:
             req_data["withDistance"] = with_distance
+
         if facets is not None and len(facets) > 0:
             aggregate_not_existing = 0
             for facet in facets:
                 if "aggregate" not in facet:
                     aggregate_not_existing += 1
             if aggregate_not_existing > 0:
                 raise Exception("[ERROR] key aggregate is a must in facets!")
             else:
                 req_data["facets"] = facets
 
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
-        del res
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     # Delete data from table
     def delete(
         self,
         table_name: str,
         primary_keys: Optional[list[Union[str, int]]] = None,
         ids: Optional[list[Union[str, int]]] = None,
         filter: Optional[str] = None,
     ):
         """Epsilla supports delete records by primary keys as default for now."""
-        if filter == None:
-            if primary_keys == None and ids == None:
+        if filter is None:
+            if primary_keys is None and ids is None:
                 raise Exception(
                     "[ERROR] Please provide at least one of primary keys(ids) and filter to delete record(s)."
                 )
-        if primary_keys == None and ids != None:
+        if primary_keys is None and ids is not None:
             primary_keys = ids
-        if primary_keys != None and ids != None:
+        if primary_keys is not None and ids is not None:
             try:
                 sentry_sdk.sdk("Duplicate Keys with both primary keys and ids", "info")
             except Exception as e:
                 pass
             print(
                 "[WARN] Both primary_keys and ids are prvoided, will use primary keys by default!"
             )
 
         req_url = "{}/data/delete".format(self._baseurl)
         req_data = {"table": table_name}
-        if primary_keys != None:
+        if primary_keys is not None:
             req_data["primaryKeys"] = primary_keys
-        if filter != None:
+        if filter is not None:
             req_data["filter"] = filter
 
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     ## get data from table
     def get(
         self,
         table_name: str,
         response_fields: Optional[list] = None,
         primary_keys: Optional[list[Union[str, int]]] = None,
         ids: Optional[list[Union[str, int]]] = None,
         filter: Optional[str] = None,
         skip: Optional[int] = None,
         limit: Optional[int] = None,
+        facets: Optional[list[dict]] = None,
     ):
         """Epsilla supports get records by primary keys as default for now."""
-        if primary_keys != None and ids != None:
+        if primary_keys is not None and ids is not None:
             try:
                 sentry_sdk.sdk("Duplicate Keys with both primary_keys and ids", "info")
             except Exception as e:
                 pass
             print(
                 "[WARN]Both primary_keys and ids are prvoided, will use primary keys by default!"
             )
-        if primary_keys == None and ids != None:
+        if primary_keys is None and ids is not None:
             primary_keys = ids
 
         req_data = {"table": table_name}
-        if response_fields != None:
+
+        if response_fields is not None:
             req_data["response"] = response_fields
-        if primary_keys != None:
+        if primary_keys is not None:
             req_data["primaryKeys"] = primary_keys
-        if filter != None:
+        if filter is not None:
             req_data["filter"] = filter
-        if skip != None:
+        if skip is not None:
             req_data["skip"] = skip
-        if limit != None:
+        if limit is not None:
             req_data["limit"] = limit
 
+        if facets is not None and len(facets) > 0:
+            aggregate_not_existing = 0
+            for facet in facets:
+                if "aggregate" not in facet:
+                    aggregate_not_existing += 1
+            if aggregate_not_existing > 0:
+                raise Exception("[ERROR] key aggregate is a must in facets!")
+            else:
+                req_data["facets"] = facets
+
         req_url = "{}/data/get".format(self._baseurl)
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def as_search_engine(self):
         return SearchEngine(self)
```

### Comparing `pyepsilla-0.3.6/pyepsilla/enterprise/sentry.py` & `pyepsilla-0.3.7/pyepsilla/cloud/sentry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,74 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 # Sentry collects crash reports and performance numbers
 # It is possible to turn off data collection using an environment variable named "SENTRY_DISABLE"
 
-import os, sys, platform, uuid, hashlib, socket, requests
+import hashlib
+import os
+import platform
+import socket
+import sys
+import uuid
+
+import requests
 import sentry_sdk
-from sentry_sdk.integrations.atexit import AtexitIntegration
 from pyepsilla.vectordb.version import __version__
-
+from sentry_sdk.integrations.atexit import AtexitIntegration
 
 CONFIG_URL = "https://config.epsilla.com/candidate.json"
-SENTRY_DSN = "https://c705adb9ba9a5750ab5719c69021e3b0@o4505952171917312.ingest.sentry.io/4506031458746368"
+SENTRY_DSN = "https://3f89b94a4a2e7620c8ecce81cb302d43@o4507288359862272.ingest.us.sentry.io/4507288364908545"
 
 try:
     r = requests.get(CONFIG_URL, headers={"Agent": "PyEpsilla Cloud Client"}, timeout=2)
     if r.status_code == 200:
         SENTRY_DSN = r.json()["pyepsilla"][0]
 except Exception:
     pass
 
+
 def callback(pending, timeout):
     sys.stderr.flush()
-        
+
+
 def get_external_ip() -> str:
     try:
         return requests.get("https://api.ipify.org", timeout=2).text
     except Exception:
         return "NA"
 
+
 def init_sentry():
-    if "SENTRY_DISABLE" not in os.environ:
+    if os.getenv("SENTRY_DISABLE", None) is not None:
         try:
             uid = hashlib.sha256(str(uuid.getnode()).encode()).hexdigest()
             internal_ip = socket.gethostbyname(socket.gethostname())
             external_ip = get_external_ip()
             sentry_sdk.set_tag("uid", uid)
             sentry_sdk.set_tag("internal_ip", internal_ip)
             sentry_sdk.set_tag("external_ip", external_ip)
-            sentry_sdk.set_user({'ip_address': '{{auto}}'})
-            sentry_sdk.set_user({"username": "{}-{}-{}".format(socket.gethostname(), internal_ip, external_ip)})
+            sentry_sdk.set_user({"ip_address": "{{auto}}"})
+            sentry_sdk.set_user(
+                {
+                    "username": "{}-{}-{}".format(
+                        socket.gethostname(), internal_ip, external_ip
+                    )
+                }
+            )
             sentry_sdk.set_tag("version", platform.version())
-            sentry_sdk.set_tag("platform", "{}-{}".format(sys.platform, platform.machine()))
+            sentry_sdk.set_tag(
+                "platform", "{}-{}".format(sys.platform, platform.machine())
+            )
             sentry_sdk.init(
                 dsn=SENTRY_DSN,
                 release=__version__,
                 traces_sample_rate=1.0,
                 integrations=[AtexitIntegration(callback=callback)],
             )
 
             sentry_sdk.capture_message("PyEpsilla Cloud Client Init", "info")
         except Exception:
             sentry_sdk.flush()
             pass
+    else:
+        return None
```

### Comparing `pyepsilla-0.3.6/pyepsilla/utils/search_engine.py` & `pyepsilla-0.3.7/pyepsilla/utils/search_engine.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.6/pyepsilla/vectordb/client.py` & `pyepsilla-0.3.7/pyepsilla/vectordb/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,36 +48,38 @@
         else:
             raise Exception(
                 "[ERROR] Failed to connect to {}:{}".format(self._host, self._port)
             )
 
     def welcome(self):
         req_url = "{}/".format(self._baseurl)
-        req_data = None
-        res = requests.get(
+        req_data = {}
+        resp = requests.get(
             url=req_url,
             data=json.dumps(req_data),
             headers=self._header,
             timeout=self._timeout,
             verify=False,
         )
-        status_code = res.status_code
-        body = res.text
-        res.close()
+        status_code = resp.status_code
+        body = resp.text
+        resp.close()
+        del resp
         return status_code, body
 
     def state(self):
         req_url = "{}/state".format(self._baseurl)
-        req_data = None
-        res = requests.get(
+        req_data = {}
+        resp = requests.get(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def use_db(self, db_name: str):
         self._db = db_name
 
     def load_db(
         self,
@@ -88,41 +90,47 @@
     ):
         req_url = "{}/api/load".format(self._baseurl)
         req_data = {"name": db_name, "path": db_path}
         if vector_scale is not None:
             req_data["vectorScale"] = vector_scale
         if wal_enabled is not None:
             req_data["walEnabled"] = wal_enabled
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def unload_db(self, db_name: str):
         req_url = "{}/api/{}/unload".format(self._baseurl, db_name)
-        res = requests.post(url=req_url, data=None, headers=self._header, verify=False)
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        req_data = {}
+        resp = requests.post(
+            url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
+        )
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def statistics(self):
         if self._db is None:
             raise Exception("[ERROR] Please use_db() first!")
         req_url = "{}/api/{}/statistics".format(self._baseurl, self._db)
-        req_data = None
-        res = requests.get(
+        req_data = {}
+        resp = requests.get(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def create_table(
         self,
         table_name: str,
         table_fields: list[dict] = None,
         indices: list[dict] = None,
@@ -131,60 +139,64 @@
             raise Exception("[ERROR] Please use_db() first!")
         if table_fields is None:
             table_fields = []
         req_url = "{}/api/{}/schema/tables".format(self._baseurl, self._db)
         req_data = {"name": table_name, "fields": table_fields}
         if indices is not None:
             req_data["indices"] = indices
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def list_tables(self):
         if self._db is None:
             raise Exception("[ERROR] Please use_db() first!")
         req_url = "{}/api/{}/schema/tables/show".format(self._baseurl, self._db)
-        res = requests.get(url=req_url, headers=self._header, verify=False)
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        resp = requests.get(url=req_url, headers=self._header, verify=False)
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def insert(self, table_name: str, records: list = None):
         if self._db is None:
             raise Exception("[ERROR] Please use_db() first!")
         if records is None:
             records = []
         req_url = "{}/api/{}/data/insert".format(self._baseurl, self._db)
         req_data = {"table": table_name, "data": records}
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def upsert(self, table_name: str, records: list = None):
         if self._db is None:
             raise Exception("[ERROR] Please use_db() first!")
         if records is None:
             records = []
         req_url = "{}/api/{}/data/insert".format(self._baseurl, self._db)
         req_data = {"table": table_name, "data": records, "upsert": True}
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def delete(
         self,
         table_name: str,
         primary_keys: list[Union[str, int]] = None,
         ids: list[Union[str, int]] = None,
@@ -212,39 +224,41 @@
 
         req_url = "{}/api/{}/data/delete".format(self._baseurl, self._db)
         req_data = {"table": table_name}
         if primary_keys != None:
             req_data["primaryKeys"] = primary_keys
         if filter != None:
             req_data["filter"] = filter
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def rebuild(self, timeout: int = 7200):
         req_url = "{}/api/rebuild".format(self._baseurl)
-        req_data = None
+        req_data = {}
         print("[INFO] waiting until rebuild is finished ...")
         start_time = datetime.datetime.now().strftime("%Y-%m-%dT%H:%M:%S")
-        res = requests.post(
+        resp = requests.post(
             url=req_url,
             data=json.dumps(req_data),
             headers=self._header,
             timeout=timeout,
             verify=False,
         )
         end_time = datetime.datetime.now().strftime("%Y-%m-%dT%H:%M:%S")
         print("[INFO] Start Time:{}\n       End   Time:{}".format(start_time, end_time))
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def query(
         self,
         table_name: str,
         query_text: str = None,
         query_index: str = None,
@@ -254,48 +268,52 @@
         limit: int = 2,
         filter: Optional[str] = None,
         with_distance: Optional[bool] = False,
         facets: Optional[list[dict]] = None,
     ):
         if self._db is None:
             raise Exception("[ERROR] Please use_db() first!")
+        req_url = "{}/api/{}/data/query".format(self._baseurl, self._db)
+        req_data = {"table": table_name, "limit": limit}
+
         if response_fields is None:
             response_fields = []
-        req_url = "{}/api/{}/data/query".format(self._baseurl, self._db)
-        req_data = {
-            "table": table_name,
-            "response": response_fields,
-            "limit": limit,
-            "filter": filter,
-            "withDistance": with_distance,
-        }
+
+        if query_text is not None:
+            req_data["query"] = query_text
+        if query_index is not None:
+            req_data["queryIndex"] = query_index
+        if query_field is not None:
+            req_data["queryField"] = query_field
+        if query_vector is not None:
+            req_data["queryVector"] = query_vector
+        if response_fields is not None:
+            req_data["response"] = response_fields
+        if filter is not None:
+            req_data["filter"] = filter
+        if with_distance is not False:
+            req_data["withDistance"] = with_distance
+
         if facets is not None and len(facets) > 0:
             aggregate_not_existing = 0
             for facet in facets:
                 if "aggregate" not in facet:
                     aggregate_not_existing += 1
             if aggregate_not_existing > 0:
                 raise Exception("[ERROR] key aggregate is a must in facets!")
             else:
                 req_data["facets"] = facets
-        if query_text is not None:
-            req_data["query"] = query_text
-        if query_index is not None:
-            req_data["queryIndex"] = query_index
-        if query_field is not None:
-            req_data["queryField"] = query_field
-        if query_vector is not None:
-            req_data["queryVector"] = query_vector
-        res = requests.post(
+
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
-        del res
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def get(
         self,
         table_name: str,
         response_fields: Optional[list] = None,
         primary_keys: Optional[list[Union[str, int]]] = None,
@@ -303,81 +321,82 @@
         filter: Optional[str] = None,
         skip: Optional[int] = None,
         limit: Optional[int] = None,
         facets: Optional[list[dict]] = None,
     ):
         if self._db is None:
             raise Exception("[ERROR] Please use_db() first!")
-        if primary_keys != None and ids != None:
+        if primary_keys is not None and ids is not None:
             try:
                 sentry_sdk.sdk("Duplicate Keys with both primary keys and ids", "info")
             except Exception as e:
                 pass
             print(
                 "[WARN] Both primary_keys and ids are prvoided, will use primary keys by default!"
             )
+
         if primary_keys is None and ids is not None:
             primary_keys = ids
 
         req_data = {"table": table_name}
 
         if response_fields is not None:
             req_data["response"] = response_fields
-
         if primary_keys is not None:
             req_data["primaryKeys"] = primary_keys
-
         if filter is not None:
             req_data["filter"] = filter
-
         if skip is not None:
-            req_data["skip"] = filter
-
+            req_data["skip"] = skip
         if limit is not None:
             req_data["limit"] = limit
 
         if facets is not None and len(facets) > 0:
             aggregate_not_existing = 0
             for facet in facets:
                 if "aggregate" not in facet:
                     aggregate_not_existing += 1
             if aggregate_not_existing > 0:
                 raise Exception("[ERROR] key aggregate is a must in facets!")
             else:
                 req_data["facets"] = facets
 
         req_url = "{}/api/{}/data/get".format(self._baseurl, self._db)
-        res = requests.post(
+        resp = requests.post(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def drop_table(self, table_name: str = None):
         if self._db is None:
             raise Exception("[ERROR] Please use_db() first!")
         req_url = "{}/api/{}/schema/tables/{}".format(
             self._baseurl, self._db, table_name
         )
-        req_data = None
-        res = requests.delete(
+        req_data = {}
+        resp = requests.delete(
             url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def drop_db(self, db_name: str):
         req_url = "{}/api/{}/drop".format(self._baseurl, db_name)
-        res = requests.delete(
-            url=req_url, data=None, headers=self._header, verify=False
+        req_data = {}
+        resp = requests.delete(
+            url=req_url, data=json.dumps(req_data), headers=self._header, verify=False
         )
-        status_code = res.status_code
-        body = res.json()
-        res.close()
+        status_code = resp.status_code
+        body = resp.json()
+        resp.close()
+        del resp
         return status_code, body
 
     def as_search_engine(self):
         return SearchEngine(self)
```

### Comparing `pyepsilla-0.3.6/pyepsilla/vectordb/field.py` & `pyepsilla-0.3.7/pyepsilla/vectordb/field.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.6/pyepsilla/vectordb/machineid/__init__.py` & `pyepsilla-0.3.7/pyepsilla/vectordb/machineid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.6/pyepsilla/vectordb/sentry.py` & `pyepsilla-0.3.7/pyepsilla/enterprise/sentry.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 import platform
 import socket
 import sys
 import uuid
 
 import requests
 import sentry_sdk
+from pyepsilla.vectordb.version import __version__
 from sentry_sdk.integrations.atexit import AtexitIntegration
 
-from .version import __version__
-
 CONFIG_URL = "https://config.epsilla.com/candidate.json"
-SENTRY_DSN = "https://7b7043e213409f7125c511127697d668@o4506949201428480.ingest.us.sentry.io/4506949333680128"
+SENTRY_DSN = "https://3f89b94a4a2e7620c8ecce81cb302d43@o4507288359862272.ingest.us.sentry.io/4507288364908545"
 
 try:
-    r = requests.get(CONFIG_URL, headers={"Agent": "PyEpsilla"}, timeout=2)
+    r = requests.get(
+        CONFIG_URL, headers={"Agent": "PyEpsilla Enterprise Client"}, timeout=2
+    )
     if r.status_code == 200:
         SENTRY_DSN = r.json()["pyepsilla"][0]
 except Exception:
     pass
 
 
 def callback(pending, timeout):
@@ -36,15 +37,15 @@
     try:
         return requests.get("https://api.ipify.org", timeout=2).text
     except Exception:
         return "NA"
 
 
 def init_sentry():
-    if "SENTRY_DISABLE" not in os.environ:
+    if os.getenv("SENTRY_DISABLE", None) is not None:
         try:
             uid = hashlib.sha256(str(uuid.getnode()).encode()).hexdigest()
             internal_ip = socket.gethostbyname(socket.gethostname())
             external_ip = get_external_ip()
             sentry_sdk.set_tag("uid", uid)
             sentry_sdk.set_tag("internal_ip", internal_ip)
             sentry_sdk.set_tag("external_ip", external_ip)
@@ -63,11 +64,13 @@
             sentry_sdk.init(
                 dsn=SENTRY_DSN,
                 release=__version__,
                 traces_sample_rate=1.0,
                 integrations=[AtexitIntegration(callback=callback)],
             )
 
-            sentry_sdk.capture_message("PyEpsilla Init", "info")
+            sentry_sdk.capture_message("PyEpsilla Enterprise Client Init", "info")
         except Exception:
             sentry_sdk.flush()
             pass
+    else:
+        return None
```

### Comparing `pyepsilla-0.3.6/pyepsilla/vectordb/telemetry.py` & `pyepsilla-0.3.7/pyepsilla/vectordb/telemetry.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.6/pyepsilla/vectordb/utils/embedding_functions.py` & `pyepsilla-0.3.7/pyepsilla/vectordb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.6/pyepsilla.egg-info/SOURCES.txt` & `pyepsilla-0.3.7/pyepsilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.3.6/setup.py` & `pyepsilla-0.3.7/setup.py`

 * *Files identical despite different names*


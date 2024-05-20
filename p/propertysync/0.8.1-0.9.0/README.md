# Comparing `tmp/propertysync-0.8.1.tar.gz` & `tmp/propertysync-0.9.0.tar.gz`

## Comparing `propertysync-0.8.1.tar` & `propertysync-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 propertysync-0.8.1/CHANGELOG.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.8.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/__about__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/__init__.py
--rw-r--r--   0        0        0    18746 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/api.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/batch.py
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/search.py
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.8.1/propertysync/titlesearch_batch.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.8.1/tests/test_batch.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.8.1/tests/test_document.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.8.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.8.1/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.8.1/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 propertysync-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.9.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.9.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.9.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.9.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.9.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.9.0/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.9.0/propertysync/__init__.py
+-rw-r--r--   0        0        0    19057 2020-02-02 00:00:00.000000 propertysync-0.9.0/propertysync/api.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.9.0/propertysync/batch.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.9.0/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.9.0/propertysync/search.py
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.9.0/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.9.0/tests/test_batch.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.9.0/tests/test_document.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.9.0/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.9.0/PKG-INFO
```

### Comparing `propertysync-0.8.1/CHANGELOG.md` & `propertysync-0.9.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Generated by [`auto-changelog`](https://github.com/CookPete/auto-changelog).
 
+## [v0.9.0](https://gitlab.com/propertysync/tools/python-api-client/compare/v0.8.1...v0.9.0) - 2023-08-16
+
+### Commits
+
+- allow doc action to be run on array of documentids [`def7906`](https://gitlab.com/propertysync/tools/python-api-client/commit/def7906869c5a2ba85ff50c16f2fb9fcf66fd15e)
+- Patch new version [`0cfd178`](https://gitlab.com/propertysync/tools/python-api-client/commit/0cfd178643945768c275d097c0674e0c318fc826)
+
 ## [v0.8.1](https://gitlab.com/propertysync/tools/python-api-client/compare/v0.8.0...v0.8.1) - 2023-08-02
 
 ### Commits
 
 - new version [`4d85d5f`](https://gitlab.com/propertysync/tools/python-api-client/commit/4d85d5f429180dee32845c322bf9f4d3abd37d7d)
 - doc updates [`c9ea065`](https://gitlab.com/propertysync/tools/python-api-client/commit/c9ea065bd5e8fa5646536c221e8c19dbd214edd7)
 - fix to validation return [`4b0b4b7`](https://gitlab.com/propertysync/tools/python-api-client/commit/4b0b4b725f594be70c2a4bd11d1323a877b1ac82)
```

### Comparing `propertysync-0.8.1/propertysync/api.py` & `propertysync-0.9.0/propertysync/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,19 @@
         elif request.status_code == 401:
             # if the token is invalid, try to login again, if we receive a failure again, raise an exception
             if (tries < 2):
                 tries += 1
                 self.login()
                 return self.api_call(method=method, url=url, params=params, tries=tries)
             else:
-                raise Exception("Unauthorized   : "+request.text)
+                raise Exception("Unauthorized : "+request.text)
         elif request.status_code == 403:
             raise Exception("Forbidden: You do not have access to this resource")
+        elif request.status_code == 404:
+            raise Exception("Not Found: "+request.text)
         elif request.status_code == 500:
             raise Exception("Server Error: "+request.text)
         else:
             raise Exception("Unknown Error: "+request.text)
 
     # get info about the document group
     def get_info(self):
@@ -388,20 +390,24 @@
     
     # run a search
     def run_search(self, search_query):
         url = f"{self.search_url}/document-groups/{self.document_group_id}/searches"
         return self.api_call("POST", url, body=search_query)
     
     # run a document action on a batch
-    def run_document_action(self, batch_id, action_id):
+    def run_document_action(self, batch_id, action_id, document_ids=None):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/document-actions/{action_id}/execute"
+        # if document_ids is set and has a count of more than 0, add it to the params
         params = {
             "batchId":batch_id
         }
-        return self.api_call("POST", url, params=params)
+        if document_ids is not None and len(document_ids) > 0:
+            params["documentIds"] = document_ids
+
+        return self.api_call("POST", url, body=params)
     
     # validate a document
     def validate_document(self, document_json):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/documents/validate"
 
         # if document_json contains an "id" key and no "json" key, it will validate the stored copy of the document
         # if document_json contains a "json" key and no "id" key, it will validate the json
```

### Comparing `propertysync-0.8.1/propertysync/batch.py` & `propertysync-0.9.0/propertysync/batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/propertysync/document.py` & `propertysync-0.9.0/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/propertysync/search.py` & `propertysync-0.9.0/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/propertysync/titlesearch_batch.py` & `propertysync-0.9.0/propertysync/titlesearch_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/tests/test_batch.py` & `propertysync-0.9.0/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/tests/test_document.py` & `propertysync-0.9.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/LICENSE` & `propertysync-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/README.md` & `propertysync-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/pyproject.toml` & `propertysync-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.8.1/PKG-INFO` & `propertysync-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.8.1
+Version: 0.9.0
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```


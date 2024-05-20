# Comparing `tmp/s3func-0.1.4.tar.gz` & `tmp/s3func-0.1.5.tar.gz`

## Comparing `s3func-0.1.4.tar` & `s3func-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 s3func-0.1.4/s3func/__init__.py
--rw-r--r--   0        0        0    18957 2020-02-02 00:00:00.000000 s3func-0.1.4/s3func/main.py
--rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 s3func-0.1.4/s3func/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.4/s3func/tests/__init__.py
--rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.4/s3func/tests/stns_data.blt
--rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 s3func-0.1.4/s3func/tests/test_s3func.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.4/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.4/LICENSE
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.4/README.md
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/__init__.py
+-rw-r--r--   0        0        0    21923 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/main.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/tests/__init__.py
+-rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/tests/stns_data.blt
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 s3func-0.1.5/s3func/tests/test_s3func.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.5/.gitignore
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.5/README.md
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.5/PKG-INFO
```

### Comparing `s3func-0.1.4/s3func/main.py` & `s3func-0.1.5/s3func/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # -*- coding: utf-8 -*-
 """
 Created on May 13 08:04:38 2024
 
 @author: mike
 """
 import io
-import os
+# import os
 from pydantic import HttpUrl
 from typing import List, Union
 import boto3
 import botocore
 import copy
 # import requests
 import urllib.parse
 from urllib3.util import Retry, Timeout
-import datetime
+# import datetime
 import hashlib
 # from requests import Session
 # from requests.adapters import HTTPAdapter
 import urllib3
 
 from . import utils
 # import utils
@@ -30,14 +30,17 @@
 # key_patterns = {
 #     'b2': '{base_url}/{bucket}/{obj_key}',
 #     'contabo': '{base_url}:{bucket}/{obj_key}',
 #     }
 
 # multipart_size = 2**28
 
+b2_auth_url = 'https://api.backblazeb2.com/b2api/v3/b2_authorize_account'
+
+available_capabilities = [ "listKeys", "writeKeys", "deleteKeys", "listAllBucketNames", "listBuckets", "readBuckets", "writeBuckets", "deleteBuckets", "readBucketRetentions", "writeBucketRetentions", "readBucketEncryption", "writeBucketEncryption", "writeBucketNotifications", "listFiles", "readFiles", "shareFiles", "writeFiles", "deleteFiles", "readBucketNotifications", "readFileLegalHolds", "writeFileLegalHolds", "readFileRetentions", "writeFileRetentions", "bypassGovernance" ]
 
 ##################################################
 ### S3 Client and url session
 
 
 def s3_client(connection_config: utils.ConnectionConfig, max_pool_connections: int = 10, max_attempts: int = 3, retry_mode: str='adaptive', read_timeout: int=120):
     """
@@ -161,30 +164,29 @@
     """
     if session is None:
         session = url_session(**url_session_kwargs)
 
     headers = utils.build_url_headers(range_start=range_start, range_end=range_end)
 
     response = session.request('get', url, headers=headers, preload_content=False)
-    metadata = utils.add_metadata_from_urllib3(response)
-    response.metadata = metadata
+    resp = utils.HttpResponse(response)
 
-    return response
+    return resp
 
 
 def base_url_to_stream(obj_key: str, base_url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **url_session_kwargs):
     """
 
     """
     if not base_url.endswith('/'):
         base_url += '/'
     url = urllib.parse.urljoin(base_url, obj_key)
-    stream = url_to_stream(url, session, range_start, range_end, chunk_size, **url_session_kwargs)
+    response = url_to_stream(url, session, range_start, range_end, chunk_size, **url_session_kwargs)
 
-    return stream
+    return response
 
 
 def get_object(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **s3_client_kwargs):
     """
     Function to get an object from an S3 bucket. Either s3 or connection_config must be used. This function will return a file object of the object in the S3 location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
     Parameters
@@ -212,25 +214,17 @@
     """
     ## Get the object
     if s3 is None:
         s3 = s3_client(**s3_client_kwargs)
 
     params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id, range_start=range_start, range_end=range_end)
 
-    try:
-        response = s3.get_object(**params)
-        stream = response['Body']
-        metadata = utils.add_metadata_from_s3(response)
-    except s3.exceptions.NoSuchKey:
-        stream = utils.S3ErrorResponse()
-        metadata = {'status': 404}
-
-    stream.metadata = metadata
+    s3resp = utils.S3Response(s3, 'get_object', **params)
 
-    return stream
+    return s3resp
 
 
 def get_object_combo(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, session: urllib3.poolmanager.PoolManager=None, base_url: HttpUrl=None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **kwargs):
     """
     Combo function to get an object from an S3 bucket either using the S3 get_object function or the base_url_to_stream function. One of s3, connection_config, or base_url must be used. This function will return a file object of the object in the S3 (or url) location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
     Parameters
@@ -275,19 +269,17 @@
     """
 
     """
     if session is None:
         session = url_session(**url_session_kwargs)
 
     response = session.request('head', url)
+    resp = utils.HttpResponse(response)
 
-    metadata = utils.add_metadata_from_urllib3(response)
-    response.metadata = metadata
-
-    return response
+    return resp
 
 
 def base_url_to_headers(obj_key: str, base_url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, **url_session_kwargs):
     """
 
     """
     if not base_url.endswith('/'):
@@ -321,26 +313,17 @@
     """
     ## Get the object
     if s3 is None:
         s3 = s3_client(**s3_client_kwargs)
 
     params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id)
 
-    try:
-        response = utils.S3Response()
-        response.headers = s3.head_object(**params)
-        metadata = utils.add_metadata_from_s3(response.headers)
-
-    except s3.exceptions.NoSuchKey:
-        response = utils.S3ErrorResponse()
-        metadata = {'status': 404}
+    s3resp = utils.S3Response(s3, 'head_object', **params)
 
-    response.metadata = metadata
-
-    return response
+    return s3resp
 
 
 def put_object(s3: botocore.client.BaseClient, bucket: str, obj_key: str, obj: Union[bytes, io.BufferedIOBase], metadata: dict={}, content_type: str=None, object_legal_hold: bool=False):
     """
     Function to upload data to an S3 bucket. This function will iteratively write the input file_obj in chunks ensuring that little memory is needed writing the object.
 
     Parameters
@@ -364,26 +347,20 @@
     -------
     None
     """
     # TODO : In python version 3.11, the file_digest function can input a file object
     if isinstance(obj, (bytes, bytearray)) and ('content-md5' not in metadata):
         metadata['content-md5'] = hashlib.md5(obj).hexdigest()
     params = utils.build_s3_params(bucket, obj_key=obj_key, metadata=metadata, content_type=content_type, object_legal_hold=object_legal_hold)
+    params['Body'] = obj
 
-    try:
-        response = utils.S3Response()
-        response.headers = s3.put_object(Body=obj, **params)
-        metadata = utils.add_metadata_from_s3(response.headers)
-    except s3.exceptions.ClientError:
-        response = utils.S3ErrorResponse()
-        metadata = {'status': 404}
-
-    response.metadata = metadata
+    s3resp = utils.S3Response(s3, 'put_object', **params)
+    s3resp.metadata.update(metadata)
 
-    return response
+    return s3resp
 
 
 #####################################
 ### Other S3 operations
 
 
 def list_objects(s3: botocore.client.BaseClient, bucket: str, prefix: str=None, start_after: str=None, delimiter: str=None, max_keys: int=None, continuation_token: str=None):
@@ -495,17 +472,43 @@
     -------
     None
     """
     for keys in utils.chunks(obj_keys, 1000):
         _ = s3.delete_objects(Bucket=bucket, Delete={'Objects': keys, 'Quiet': True})
 
 
+########################################################
+### S3 Locks and holds
+
+
+def get_object_legal_hold(s3: botocore.client.BaseClient, bucket: str, obj_key: str):
+    """
+    Function to get the staus of a legal hold of an object. The user must have s3:GetObjectLegalHold or b2:readFileLegalHolds permissions for this request.
+
+    Parameters
+    ----------
+    s3 : boto3.client
+        A boto3 client object
+    bucket : str
+        The S3 bucket.
+    obj_key : str
+        The key name for the uploaded object.
+
+    Returns
+    -------
+    S3Response
+    """
+    s3resp = utils.S3Response(s3, 'get_object_legal_hold', Bucket=bucket, Key=obj_key)
+
+    return s3resp
+
+
 def put_object_legal_hold(s3: botocore.client.BaseClient, bucket: str, obj_key: str, lock: bool=False):
     """
-    Function to put or remove a legal hold on an object.
+    Function to put or remove a legal hold on an object. The user must have s3:PutObjectLegalHold or b2:writeFileLegalHolds permissions for this request.
 
     Parameters
     ----------
     s3 : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
@@ -519,24 +522,46 @@
     None
     """
     if lock:
         hold = {'Status': 'ON'}
     else:
         hold = {'Status': 'OFF'}
 
-    resp = s3.put_object_legal_hold(Bucket=bucket, Key=obj_key, LegalHold=hold)
-    if resp['ResponseMetadata']['HTTPStatusCode'] != 200:
-        raise urllib.error.HTTPError(resp['ResponseMetadata']['HTTPStatusCode'])
+    # resp = s3.put_object_legal_hold(Bucket=bucket, Key=obj_key, LegalHold=hold)
+    # if resp['ResponseMetadata']['HTTPStatusCode'] != 200:
+    #     raise urllib.error.HTTPError(resp['ResponseMetadata']['HTTPStatusCode'])
+
+    s3resp = utils.S3Response(s3, 'put_object_legal_hold', Bucket=bucket, Key=obj_key, LegalHold=hold)
+
+    return s3resp
+
+
+def get_object_lock_configuration(s3: botocore.client.BaseClient, bucket: str):
+    """
+    Function to whther a bucket is configured to have object locks. The user must have s3:GetBucketObjectLockConfiguration or b2:readBucketRetentions permissions for this request.
+
+    Parameters
+    ----------
+    s3 : boto3.client
+        A boto3 client object
+    bucket : str
+        The S3 bucket.
 
-    # return resp
+    Returns
+    -------
+    S3Reponse
+    """
+    s3resp = utils.S3Response(s3, 'get_object_lock_configuration', Bucket=bucket)
+
+    return s3resp
 
 
 def put_object_lock_configuration(s3: botocore.client.BaseClient, bucket: str, lock: bool=False):
     """
-    Function to enable or disable object locks for a bucket.
+    Function to enable or disable object locks for a bucket. The user must have s3:PutBucketObjectLockConfiguration or b2:writeBucketRetentions permissions for this request.
 
     Parameters
     ----------
     s3 : boto3.client
         A boto3 client object
     bucket : str
         The S3 bucket.
@@ -548,47 +573,108 @@
     boto3 response
     """
     if lock:
         hold = {'ObjectLockEnabled': 'Enable'}
     else:
         hold = {'ObjectLockEnabled': 'Disable'}
 
-    resp = s3.put_object_lock_configuration(Bucket=bucket, ObjectLockConfiguration=hold)
+    # resp = s3.put_object_lock_configuration(Bucket=bucket, ObjectLockConfiguration=hold)
+    s3resp = utils.S3Response(s3, 'put_object_lock_configuration', Bucket=bucket, ObjectLockConfiguration=hold)
+
+    return s3resp
+
+
+class S3Lock:
+    """
+
+    """
+    def __init__(self, s3: botocore.client.BaseClient, bucket: str, obj_key: str):
+        """
+
+        """
+
+
+
+#########################################################
+### Backblaze
+
+
+def get_authorization_b2(username, password, session=None, **url_session_kwargs):
+    """
+
+    """
+    if session is None:
+        session = url_session(**url_session_kwargs)
+
+    headers = urllib3.make_headers(basic_auth=f'{username}:{password}')
+
+    response = session.request('get', b2_auth_url, headers=headers)
+    resp = utils.HttpResponse(response)
 
     return resp
 
 
-def get_object_legal_hold(s3: botocore.client.BaseClient, bucket: str, obj_key: str):
+def create_app_key_b2(auth_dict: dict, capabilities: List[str], key_name: str, duration: int=None, bucket_id: str=None, prefix: str=None, session=None, **url_session_kwargs):
     """
-    Function to get the staus of a legal hold of an object.
 
-    Parameters
-    ----------
-    s3 : boto3.client
-        A boto3 client object
-    bucket : str
-        The S3 bucket.
-    obj_key : str
-        The key name for the uploaded object.
+    """
+    account_id = auth_dict['accountId']
+    api_url = auth_dict['apiInfo']['storageApi']['apiUrl']
+    auth_token = auth_dict['authorizationToken']
 
-    Returns
-    -------
-    bool
+    fields = {
+        'accountId': account_id,
+        'capabilities': capabilities,
+        'keyName': key_name}
+
+    if isinstance(duration, int):
+        fields['validDurationInSeconds'] = duration
+
+    if isinstance(bucket_id, str):
+        fields['bucketId'] = bucket_id
+
+    if isinstance(prefix, str):
+        fields['namePrefix'] = prefix
+
+    url = urllib.parse.urljoin(api_url, '/b2api/v3/b2_create_key')
+
+    if session is None:
+        session = url_session(**url_session_kwargs)
+
+    response = session.request('post', url, json=fields, headers={'Authorization': auth_token})
+    resp = utils.HttpResponse(response)
+
+    return resp
+
+
+def list_buckets_b2(auth_dict: dict, session=None, **url_session_kwargs):
     """
-    try:
-        resp = s3.get_object_legal_hold(Bucket=bucket, Key=obj_key)
-    except botocore.exceptions.ClientError:
-        return False
 
-    status = resp['LegalHold']['Status']
+    """
+    account_id = auth_dict['accountId']
+    api_url = auth_dict['apiInfo']['storageApi']['apiUrl']
+    auth_token = auth_dict['authorizationToken']
+
+    fields = {
+        'accountId': account_id,
+        }
+
+    url = urllib.parse.urljoin(api_url, '/b2api/v3/b2_list_buckets')
+
+    if session is None:
+        session = url_session(**url_session_kwargs)
+
+    response = session.request('post', url, json=fields, headers={'Authorization': auth_token})
+    resp = utils.HttpResponse(response)
+
+    return resp
+
+
+
 
-    if status == 'ON':
-        return True
-    else:
-        return False
```

### Comparing `s3func-0.1.4/s3func/utils.py` & `s3func-0.1.5/s3func/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Created on Sat Oct  8 11:02:46 2022
 
 @author: mike
 """
 # import io
 # import os
 # import pandas as pd
+import urllib3
+import botocore
 from pydantic import BaseModel, HttpUrl
 import datetime
 
 #######################################################
 ### Parameters
 
 # key_patterns = {
@@ -155,22 +157,33 @@
     """
     # headers = response.headers
     if 'Metadata' in response:
         metadata = response.pop('Metadata')
     else:
         metadata = {}
 
-    metadata['etag'] = response['ETag'].strip('"')
-    metadata['version_id'] = response['VersionId']
-    metadata['last_modified'] = datetime.datetime.fromtimestamp(int(metadata['version_id'].split('_u')[1]) * 0.001, datetime.timezone.utc)
+    if 'ETag' in response:
+        metadata['etag'] = response['ETag'].strip('"')
+    if 'VersionId' in response:
+        metadata['version_id'] = response['VersionId']
+        metadata['last_modified'] = datetime.datetime.fromtimestamp(int(metadata['version_id'].split('_u')[1]) * 0.001, datetime.timezone.utc)
     if 'ContentLength' in response:
         metadata['content_length'] = response['ContentLength']
     if 'HTTPStatusCode' in response['ResponseMetadata']:
         metadata['status'] = response['ResponseMetadata']['HTTPStatusCode']
 
+    if 'LegalHold' in response:
+        if 'Status' in response['LegalHold']:
+            status = response['LegalHold']['Status']
+
+            if status == 'ON':
+                metadata['legal_hold'] = True
+            else:
+                metadata['legal_hold'] = False
+
     return metadata
 
 
 # class ResponseStream(object):
 #     """
 #     In many applications, you'd like to access a requests response as a file-like object, simply having .read(), .seek(), and .tell() as normal. Especially when you only want to partially download a file, it'd be extra convenient if you could use a normal file interface for it, loading as needed.
 
@@ -230,18 +243,77 @@
 #     def send(self, request, **kwargs):
 #         timeout = kwargs.get("timeout")
 #         if timeout is None and hasattr(self, 'timeout'):
 #             kwargs["timeout"] = self.timeout
 #         return super().send(request, **kwargs)
 
 class S3Response:
-    pass
+    """
+
+    """
+    def __init__(self, s3, method, **kwargs):
+        """
+
+        """
+        stream = None
+        error = {}
+        headers = {}
+
+        func = getattr(s3, method)
+        try:
+            resp = func(**kwargs)
+            metadata = add_metadata_from_s3(resp)
+            status = 200
+            metadata['status'] = 200
+
+            if 'Body' in resp:
+                if isinstance(resp['Body'], botocore.response.StreamingBody):
+                    stream = resp.pop('Body')
+                else:
+                    del resp['Body']
+
+            headers = resp
+        except s3.exceptions.NoSuchKey as err:
+            status = 404
+            metadata = {'status': status}
+            error = {'status': status, 'message': str(err)}
+        except s3.exceptions.ClientError as err:
+            status = 403
+            metadata = {'status': status}
+            error = {'status': status, 'message': str(err)}
+
+        self.headers = headers
+        self.metadata = metadata
+        self.stream = stream
+        self.error = error
+        self.status = status
+
+
+class HttpResponse:
+    """
+
+    """
+    def __init__(self, response: urllib3.HTTPResponse):
+        """
+
+        """
+        stream = None
+        error = {}
+        metadata = add_metadata_from_urllib3(response)
+
+        if response.status != 200:
+            error = response.json()
+        else:
+            stream = response
 
-class S3ErrorResponse:
-    pass
+        self.headers = dict(response.headers)
+        self.metadata = metadata
+        self.stream = stream
+        self.error = error
+        self.status = response.status
```

### Comparing `s3func-0.1.4/s3func/tests/stns_data.blt` & `s3func-0.1.5/s3func/tests/stns_data.blt`

 * *Files identical despite different names*

### Comparing `s3func-0.1.4/s3func/tests/test_s3func.py` & `s3func-0.1.5/s3func/tests/test_s3func.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,31 +149,31 @@
 
 
 def test_get_object():
     """
 
     """
     stream1 = get_object(obj_key, bucket, s3)
-    data1 = stream1.read()
+    data1 = stream1.stream.read()
 
     stream2 = get_object(obj_key, bucket, connection_config=conn_config)
-    data2 = stream2.read()
+    data2 = stream2.stream.read()
 
     assert data1 == data2
 
 
 def test_url_to_stream():
     """
 
     """
     stream1 = url_to_stream(url)
-    data1 = stream1.read()
+    data1 = stream1.stream.read()
 
     stream2 = base_url_to_stream(obj_key, base_url)
-    data2 = stream2.read()
+    data2 = stream2.stream.read()
 
     assert data1 == data2
 
 
 def test_head_object():
     """
 
@@ -193,39 +193,45 @@
 
 
 def test_legal_hold():
     """
 
     """
     hold = get_object_legal_hold(s3, bucket, obj_key)
-    if hold:
+    if hold.status != 403:
         raise ValueError("There's a hold, but there shouldn't be.")
 
-    put_object_legal_hold(s3, bucket, obj_key, True)
+    put_hold = put_object_legal_hold(s3, bucket, obj_key, True)
+    if put_hold.status != 200:
+        raise ValueError("Creating a hold failed.")
 
     hold = get_object_legal_hold(s3, bucket, obj_key)
-    if not hold:
+    if not hold.metadata['legal_hold']:
         raise ValueError("There isn't a hold, but there should be.")
 
-    put_object_legal_hold(s3, bucket, obj_key, False)
+    put_hold = put_object_legal_hold(s3, bucket, obj_key, False)
+    if put_hold.status != 200:
+        raise ValueError("Removing a hold failed.")
 
     hold = get_object_legal_hold(s3, bucket, obj_key)
-    if hold:
+    if hold.metadata['legal_hold']:
         raise ValueError("There's a hold, but there shouldn't be.")
 
     resp2 = put_object(s3, bucket, obj_key, open(script_path.joinpath(file_name), 'rb'), object_legal_hold=True)
 
     hold = get_object_legal_hold(s3, bucket, obj_key)
-    if not hold:
+    if not hold.metadata['legal_hold']:
         raise ValueError("There isn't a hold, but there should be.")
 
-    put_object_legal_hold(s3, bucket, obj_key, False)
+    put_hold = put_object_legal_hold(s3, bucket, obj_key, False)
+    if put_hold.status != 200:
+        raise ValueError("Removing a hold failed.")
 
     hold = get_object_legal_hold(s3, bucket, obj_key)
-    if hold:
+    if hold.metadata['legal_hold']:
         raise ValueError("There's a hold, but there shouldn't be.")
 
     assert True
 
 
 def test_delete_objects():
     """
```

### Comparing `s3func-0.1.4/.gitignore` & `s3func-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `s3func-0.1.4/LICENSE` & `s3func-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `s3func-0.1.4/README.md` & `s3func-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `s3func-0.1.4/pyproject.toml` & `s3func-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s3func-0.1.4/PKG-INFO` & `s3func-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: s3func
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple functions for working with S3
 Project-URL: Documentation, https://mullenkamp.github.io/s3func/
 Project-URL: Source, https://github.com/mullenkamp/s3func
 Author-email: s3func <mullenkamp1@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: s3func Version: 0.1.4 Summary: Simple functions for
+Metadata-Version: 2.3 Name: s3func Version: 0.1.5 Summary: Simple functions for
 working with S3 Project-URL: Documentation, https://mullenkamp.github.io/
 s3func/ Project-URL: Source, https://github.com/mullenkamp/s3func Author-email:
 s3func
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.9 Requires-Dist: boto3 Requires-Dist: pydantic
 Requires-Dist: urllib3 Description-Content-Type: text/markdown # s3func
                      SSiimmppllee ffuunnccttiioonnss ffoorr wwoorrkkiinngg wwiitthh SS33
```


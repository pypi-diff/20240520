# Comparing `tmp/adri_storage-0.0.1.tar.gz` & `tmp/adri_storage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adri_storage-0.0.1.tar", last modified: Mon May 20 12:24:50 2024, max compression
+gzip compressed data, was "adri_storage-0.0.2.tar", last modified: Mon May 20 12:39:38 2024, max compression
```

## Comparing `adri_storage-0.0.1.tar` & `adri_storage-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 12:24:50.806585 adri_storage-0.0.1/
--rw-rw-rw-   0        0        0      450 2024-05-20 12:24:50.801111 adri_storage-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 12:24:50.751208 adri_storage-0.0.1/adri_storage/
--rw-rw-rw-   0        0        0        0 2024-05-20 11:27:28.000000 adri_storage-0.0.1/adri_storage/__init__.py
--rw-rw-rw-   0        0        0     1098 2024-05-20 11:18:27.000000 adri_storage-0.0.1/adri_storage/client.py
--rw-rw-rw-   0        0        0       88 2024-05-19 11:03:38.000000 adri_storage-0.0.1/adri_storage/client_enums.py
--rw-rw-rw-   0        0        0     7691 2024-05-20 12:22:03.000000 adri_storage-0.0.1/adri_storage/local_client.py
--rw-rw-rw-   0        0        0     1996 2024-05-20 11:32:52.000000 adri_storage-0.0.1/adri_storage/main.py
--rw-rw-rw-   0        0        0     4774 2024-05-20 11:18:04.000000 adri_storage-0.0.1/adri_storage/s3_client.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:24:50.798525 adri_storage-0.0.1/adri_storage.egg-info/
--rw-rw-rw-   0        0        0      450 2024-05-20 12:24:50.000000 adri_storage-0.0.1/adri_storage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-05-20 12:24:50.000000 adri_storage-0.0.1/adri_storage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 12:24:50.000000 adri_storage-0.0.1/adri_storage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-20 12:24:50.000000 adri_storage-0.0.1/adri_storage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-20 12:24:50.000000 adri_storage-0.0.1/adri_storage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      592 2024-05-20 12:24:14.000000 adri_storage-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 12:24:50.808257 adri_storage-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 12:39:38.750277 adri_storage-0.0.2/
+-rw-rw-rw-   0        0        0      450 2024-05-20 12:39:38.744495 adri_storage-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 12:39:38.684464 adri_storage-0.0.2/adri_storage/
+-rw-rw-rw-   0        0        0        0 2024-05-20 11:27:28.000000 adri_storage-0.0.2/adri_storage/__init__.py
+-rw-rw-rw-   0        0        0     1098 2024-05-20 11:18:27.000000 adri_storage-0.0.2/adri_storage/client.py
+-rw-rw-rw-   0        0        0       88 2024-05-19 11:03:38.000000 adri_storage-0.0.2/adri_storage/client_enums.py
+-rw-rw-rw-   0        0        0     7686 2024-05-20 12:36:15.000000 adri_storage-0.0.2/adri_storage/local_client.py
+-rw-rw-rw-   0        0        0     1994 2024-05-20 12:38:32.000000 adri_storage-0.0.2/adri_storage/main.py
+-rw-rw-rw-   0        0        0     4769 2024-05-20 12:35:47.000000 adri_storage-0.0.2/adri_storage/s3_client.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:39:38.741480 adri_storage-0.0.2/adri_storage.egg-info/
+-rw-rw-rw-   0        0        0      450 2024-05-20 12:39:38.000000 adri_storage-0.0.2/adri_storage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-05-20 12:39:38.000000 adri_storage-0.0.2/adri_storage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:39:38.000000 adri_storage-0.0.2/adri_storage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-20 12:39:38.000000 adri_storage-0.0.2/adri_storage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 12:39:38.000000 adri_storage-0.0.2/adri_storage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      592 2024-05-20 12:39:03.000000 adri_storage-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:39:38.751272 adri_storage-0.0.2/setup.cfg
```

### Comparing `adri_storage-0.0.1/adri_storage/client.py` & `adri_storage-0.0.2/adri_storage/client.py`

 * *Files identical despite different names*

### Comparing `adri_storage-0.0.1/adri_storage/local_client.py` & `adri_storage-0.0.2/adri_storage/local_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import hashlib
 import hmac
 import os
 import tempfile
 from typing import Dict, Optional
-from client import Client
+import client
 import requests
 import json
 import base64
 import uuid
 from pathlib import Path
 from shutil import copyfileobj
 
 
 class InvalidParamException(Exception):
     pass
 
 class InvalidPolicyException(Exception):
     pass
 
-class LocalFileSystem(Client):
+class LocalFileSystem(client.Client):
 
     def __init__(self, bucket_name: str, local_fs_secret_key: str, local_fs_secured_url: str):
         self.bucket_name = bucket_name
         self.secret_key = local_fs_secret_key
         self.secured_url = local_fs_secured_url
 
     def put_object_from_url(self, bucket: str, key: str, url: str, temp_directory: str) -> str:
```

### Comparing `adri_storage-0.0.1/adri_storage/main.py` & `adri_storage-0.0.2/adri_storage/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from local_client import LocalFileSystem
-from s3_client import S3FileSystem
-from client import Client
-from client_enums import FileSystemType
+import client
+import client_enums
+import s3_client
+import local_client
 
-def get_filesystem(fs_type:FileSystemType, **kwargs) -> Client:
+def get_filesystem(fs_type:client_enums.FileSystemType, **kwargs) -> client.Client:
     """
     Get an instance of a file system client based on the specified file system type.
 
     Parameters:
         fs_type (FileSystemType): The type of file system client to instantiate.
             Supported types are FileSystemType.LOCAL and FileSystemType.S3.
 
@@ -26,22 +26,22 @@
 
     Returns:
         Client: An instance of the file system client.
 
     Raises:
         ValueError: If an unsupported file system type is specified.
     """
-    if fs_type == FileSystemType.LOCAL:
-        return LocalFileSystem(
+    if fs_type == client_enums.FileSystemType.LOCAL:
+        return local_client.LocalFileSystem(
             bucket_name=kwargs.get("bucket_name"),
             local_fs_secret_key=kwargs.get('secret_key'),
             local_fs_secured_url=kwargs.get('secured_url')
         )
-    elif fs_type == FileSystemType.S3:
-        return S3FileSystem(
+    elif fs_type == client_enums.FileSystemType.S3:
+        return s3_client.S3FileSystem(
             bucket_name=kwargs.get('bucket_name'),
             aws_access_key_id=kwargs.get('access_key'),
             aws_secret_access_key=kwargs.get('secret_key'),
             region_name=kwargs.get('region_name')
         )
     else:
         raise ValueError(f"Unsupported file system type: {fs_type}")
```

### Comparing `adri_storage-0.0.1/adri_storage/s3_client.py` & `adri_storage-0.0.2/adri_storage/s3_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import os
 import boto3
 from typing import Optional, IO
 from pathlib import Path
 import tempfile
 import uuid
 import requests
-from client import Client
+import client
 import tempfile
 from pathlib import Path
 from botocore.exceptions import ClientError
 
-class S3FileSystem(Client):
+class S3FileSystem(client.Client):
 
     def __init__(self, bucket_name: str, aws_access_key_id: Optional[str] = None, aws_secret_access_key: Optional[str] = None, region_name: Optional[str] = None):
         self.bucket_name = bucket_name
         self.s3 = boto3.client(
             's3',
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
```

### Comparing `adri_storage-0.0.1/pyproject.toml` & `adri_storage-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adri_storage"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Khalid Rasool", email="khalid.rasool@adri.nz" },
   { name="Eslam Allam", email="eslam.allam@adri.nz" }
 ]
 description = "ADRI Storage Python SDK"
 requires-python = ">=3.8"
 classifiers = [
```


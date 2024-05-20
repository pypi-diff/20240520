# Comparing `tmp/pyfunvice-0.1.5.tar.gz` & `tmp/pyfunvice-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfunvice-0.1.5.tar", max compression
+gzip compressed data, was "pyfunvice-0.1.6.tar", max compression
```

## Comparing `pyfunvice-0.1.5.tar` & `pyfunvice-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.5/README.md
--rw-r--r--   0        0        0     5628 2024-04-12 09:27:28.208125 pyfunvice-0.1.5/pyfunvice/__init__.py
--rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.5/pyfunvice/cli.py
--rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.5/pyfunvice/common_func.py
--rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.5/pyfunvice/docker_cli.py
--rw-r--r--   0        0        0      577 2024-03-26 09:15:00.081774 pyfunvice-0.1.5/pyfunvice/struct.py
--rw-r--r--   0        0        0      454 2024-04-18 02:22:16.165161 pyfunvice-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.6/README.md
+-rw-r--r--   0        0        0     5506 2024-05-20 06:11:22.735172 pyfunvice-0.1.6/pyfunvice/__init__.py
+-rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.6/pyfunvice/cli.py
+-rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.6/pyfunvice/common_func.py
+-rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.6/pyfunvice/docker_cli.py
+-rw-r--r--   0        0        0      709 2024-05-20 06:11:16.293160 pyfunvice-0.1.6/pyfunvice/struct.py
+-rw-r--r--   0        0        0      454 2024-05-20 06:35:06.675675 pyfunvice-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.6/PKG-INFO
```

### Comparing `pyfunvice-0.1.5/README.md` & `pyfunvice-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.5/pyfunvice/__init__.py` & `pyfunvice-0.1.6/pyfunvice/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from gunicorn.workers.base import Worker
 from fastapi import APIRouter, FastAPI, File, Request, UploadFile
 from fastapi.params import Form
 from functools import wraps
 import inspect
 import aiofiles
 
-from pyfunvice.common_func import delete_file, get_uuid
+from pyfunvice.common_func import delete_file
 from pyfunvice.struct import ResponseModel
 
 app = FastAPI()
 faas_router = APIRouter()
 
 
 def app_service(path="/", body_type="raw", inparam_type="dict"):
@@ -94,16 +94,14 @@
             async def process_function(
                 file: UploadFile = File(...),
                 requestId: str = Form(None),
             ):
                 try:
                     if not file:
                         raise Exception("file is empty")
-                    if requestId is None or len(requestId) == 0:
-                        requestId = get_uuid()
                     file_name: str = requestId
                     result = await wrapper(file_name, file)
                     return ResponseModel(
                         requestId=requestId,
                         code="200",
                         message="success",
                         data=result,
```

### Comparing `pyfunvice-0.1.5/pyfunvice/cli.py` & `pyfunvice-0.1.6/pyfunvice/cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.5/pyfunvice/docker_cli.py` & `pyfunvice-0.1.6/pyfunvice/docker_cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.5/PKG-INFO` & `pyfunvice-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfunvice
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: 遥奕
 Author-email: jibing.yjb@alibaba-inc.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


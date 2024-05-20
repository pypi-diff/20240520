# Comparing `tmp/hopeit_aws_s3-0.1.1.tar.gz` & `tmp/hopeit_aws_s3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopeit_aws_s3-0.1.1.tar", last modified: Fri May 17 14:04:19 2024, max compression
+gzip compressed data, was "hopeit_aws_s3-0.1.2.tar", last modified: Mon May 20 14:13:36 2024, max compression
```

## Comparing `hopeit_aws_s3-0.1.1.tar` & `hopeit_aws_s3-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:04:19.882246 hopeit_aws_s3-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-17 14:04:19.882246 hopeit_aws_s3-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-17 14:02:35.000000 hopeit_aws_s3-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 14:02:35.000000 hopeit_aws_s3-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-17 14:04:19.882246 hopeit_aws_s3-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-17 14:02:35.000000 hopeit_aws_s3-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:04:19.878246 hopeit_aws_s3-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:04:19.878246 hopeit_aws_s3-0.1.1/src/hopeit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:04:19.878246 hopeit_aws_s3-0.1.1/src/hopeit/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:04:19.882246 hopeit_aws_s3-0.1.1/src/hopeit/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 14:03:37.000000 hopeit_aws_s3-0.1.1/src/hopeit/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17246 2024-05-17 14:03:37.000000 hopeit_aws_s3-0.1.1/src/hopeit/aws/s3/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-17 14:02:35.000000 hopeit_aws_s3-0.1.1/src/hopeit/aws/s3/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 14:02:35.000000 hopeit_aws_s3-0.1.1/src/hopeit/aws/s3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:04:19.882246 hopeit_aws_s3-0.1.1/src/hopeit.aws.s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-17 14:04:19.000000 hopeit_aws_s3-0.1.1/src/hopeit.aws.s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-17 14:04:19.000000 hopeit_aws_s3-0.1.1/src/hopeit.aws.s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:04:19.000000 hopeit_aws_s3-0.1.1/src/hopeit.aws.s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 14:04:19.000000 hopeit_aws_s3-0.1.1/src/hopeit.aws.s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 14:04:19.000000 hopeit_aws_s3-0.1.1/src/hopeit.aws.s3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:13:36.236107 hopeit_aws_s3-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-20 14:13:36.236107 hopeit_aws_s3-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-20 14:11:44.000000 hopeit_aws_s3-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 14:11:44.000000 hopeit_aws_s3-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 14:13:36.236107 hopeit_aws_s3-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-20 14:11:44.000000 hopeit_aws_s3-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:13:36.232107 hopeit_aws_s3-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:13:36.232107 hopeit_aws_s3-0.1.2/src/hopeit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:13:36.232107 hopeit_aws_s3-0.1.2/src/hopeit/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:13:36.236107 hopeit_aws_s3-0.1.2/src/hopeit/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-20 14:12:55.000000 hopeit_aws_s3-0.1.2/src/hopeit/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-05-20 14:12:55.000000 hopeit_aws_s3-0.1.2/src/hopeit/aws/s3/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-20 14:11:44.000000 hopeit_aws_s3-0.1.2/src/hopeit/aws/s3/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 14:11:44.000000 hopeit_aws_s3-0.1.2/src/hopeit/aws/s3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:13:36.236107 hopeit_aws_s3-0.1.2/src/hopeit.aws.s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-20 14:13:36.000000 hopeit_aws_s3-0.1.2/src/hopeit.aws.s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 14:13:36.000000 hopeit_aws_s3-0.1.2/src/hopeit.aws.s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:13:36.000000 hopeit_aws_s3-0.1.2/src/hopeit.aws.s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 14:13:36.000000 hopeit_aws_s3-0.1.2/src/hopeit.aws.s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 14:13:36.000000 hopeit_aws_s3-0.1.2/src/hopeit.aws.s3.egg-info/top_level.txt
```

### Comparing `hopeit_aws_s3-0.1.1/PKG-INFO` & `hopeit_aws_s3-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.aws.s3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Hopeit Engine S3 Storage Toolkit
 Home-page: https://github.com/hopeit-git/hopeit.aws
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.aws/actions?query=workflow
 Project-URL: GitHub: issues, https://github.com/hopeit-git/hopeit.aws/issues
```

### Comparing `hopeit_aws_s3-0.1.1/README.md` & `hopeit_aws_s3-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hopeit_aws_s3-0.1.1/setup.py` & `hopeit_aws_s3-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-version = "0.1.1"
+version = "0.1.2"
 
 setuptools.setup(
     name="hopeit.aws.s3",
     version=version,
     description="Hopeit Engine S3 Storage Toolkit",
     license="Apache 2",
     long_description=open("README.md").read(),
```

### Comparing `hopeit_aws_s3-0.1.1/src/hopeit/aws/s3/object_storage.py` & `hopeit_aws_s3-0.1.2/src/hopeit/aws/s3/object_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import fnmatch
 import os
 from dataclasses import dataclass
 from io import BytesIO
 from typing import (
     IO,
     Any,
+    AsyncGenerator,
     AsyncIterator,
     Dict,
     Generic,
     List,
     Optional,
     Tuple,
     Type,
@@ -195,15 +196,18 @@
                 if self._conn_config.get("region_name", None) is not None
                 else {}
             )
             async with self._session.client(S3, **self._conn_config) as object_storage:
                 try:
                     await object_storage.create_bucket(Bucket=self.bucket, **kwargs)
                 except ClientError as e:
-                    if e.response["Error"]["Code"] == "BucketAlreadyOwnedByYou":
+                    if e.response["Error"]["Code"] in [
+                        "BucketAlreadyOwnedByYou",
+                        "BucketAlreadyExists",
+                    ]:
                         pass
                     else:
                         raise e
         return self
 
     async def get(
         self,
@@ -218,29 +222,29 @@
         :param key, str
         :param datatype: dataclass implementing @dataobject (@see DataObject)
         :param partition_key, Optional[str]: Optional partition key
         :return: instance
         """
 
         async with self._session.client(S3, **self._conn_config) as object_storage:
+            key = f"{partition_key}/{key}" if partition_key else key
+            key = f"{self.prefix or ''}{key}"
             try:
-                key = f"{partition_key}/{key}" if partition_key else key
-                key = f"{'' if not self.prefix else self.prefix}{key}"
                 file_obj = BytesIO()
                 await object_storage.download_fileobj(
                     self.bucket, key + SUFFIX, file_obj
                 )
                 obj = file_obj.getvalue()
                 if len(obj):
                     return Payload.from_json(obj, datatype)
                 return None
-            except ClientError as ex:
-                if ex.response["Error"]["Code"] == "404":
+            except ClientError as e:
+                if e.response["Error"]["Code"] == "404":
                     return None
-                raise ex
+                raise e
 
     async def get_file(
         self,
         file_name: str,
         *,
         partition_key: Optional[str] = None,
     ) -> Optional[bytes]:
@@ -249,16 +253,16 @@
 
         :param file_name, str: The name of the file to download
         :param partition_key, Optional[str]: Optional partition key
         :return: The contents of the requested file as bytes, or None if the file does not exist
         """
 
         async with self._session.client(S3, **self._conn_config) as object_storage:
-            if self.partition_dateformat:
-                file_name = f"{self.prefix or ''}{partition_key + '/' if partition_key else ''}{file_name}"
+            file_name = f"{partition_key}/{file_name}" if partition_key else file_name
+            file_name = f"{self.prefix or ''}{file_name}"
             try:
                 obj = await object_storage.get_object(Bucket=self.bucket, Key=file_name)
                 ret = BytesIO()
                 async for chunk in obj["Body"]:
                     ret.write(chunk)
                 return ret.getvalue()
             except ClientError as e:
@@ -312,15 +316,15 @@
                 file_path = f"{partition_key}{file_path}"
             file_path = f"{'' if not self.prefix else self.prefix}{file_path}"
             await object_storage.upload_fileobj(
                 BytesIO(Payload.to_json(value).encode()),
                 Bucket=self.bucket,
                 Key=file_path,
             )
-            return file_path
+            return self._prune_prefix(file_path)
 
     async def store_file(
         self, *, file_name: str, value: Union[bytes, IO[bytes], Any]
     ) -> str:
         """
         Stores bytes or a file-like object.
 
@@ -344,28 +348,31 @@
                 )
             else:
                 await object_storage.upload_fileobj(
                     value,
                     Bucket=self.bucket,
                     Key=file_path,
                 )
-        return file_path
+        return self._prune_prefix(file_path)
 
-    async def list_objects(self, wildcard: str = "*") -> List[ItemLocator]:
+    async def list_objects(
+        self, wildcard: str = "*", recursive: bool = False
+    ) -> List[ItemLocator]:
         """
         Retrieves list of objects keys from the object storage
 
         :param wildcard: allow filter the listing of objects
         :return: List of `ItemLocator` with objects location info
         """
         wildcard = wildcard + SUFFIX
         n_part_comps = len(self.partition_dateformat.split("/"))
-
+        if self.partition_dateformat:
+            recursive = True
         item_list = []
-        async for key in self._aioglob(True, wildcard=wildcard):
+        async for key in self._aioglob(wildcard, recursive):
             item_list.append(key)
         return [
             self._get_item_locator(item_path, n_part_comps, SUFFIX)
             for item_path in item_list
         ]
 
     async def delete(self, *keys: str, partition_key: Optional[str] = None):
@@ -394,64 +401,91 @@
             for key in file_names:
                 key = f"{partition_key}/{key}" if partition_key else key
                 await object_storage.delete_object(
                     Bucket=self.bucket,
                     Key=f"{'' if not self.prefix else self.prefix}{key}",
                 )
 
-    async def list_files(self, wildcard: str = "*") -> List[ItemLocator]:
+    async def list_files(
+        self, wildcard: str = "*", recursive: bool = False
+    ) -> List[ItemLocator]:
         """
         Retrieves list of files_names from the object storage
 
         :param wildcard, str: allow filter the listing of objects
         :return: List of `ItemLocator` with file location info
         """
         n_part_comps = len(self.partition_dateformat.split("/"))
         item_list = []
-        async for key in self._aioglob(True, wildcard=wildcard):
+        if self.partition_dateformat:
+            recursive = True
+        async for key in self._aioglob(wildcard, recursive):
             item_list.append(key)
         return [
             self._get_item_locator(item_path, n_part_comps) for item_path in item_list
         ]
 
-    async def _aioglob(self, recursive: bool = False, wildcard: Optional[str] = None):
+    def partition_key(self, path: str) -> str:
+        """
+        Get the partition key for a given path.
+
+        :param path, str
+        :return str: the extracted partition key.
+        """
+        partition_key = ""
+        if self.partition_dateformat:
+            partition_key = path.rsplit("/", 1)[0]
+        return partition_key
+
+    async def _aioglob(
+        self,
+        wildcard: Optional[str] = None,
+        recursive: bool = False,
+    ) -> AsyncGenerator[str, None]:
         """
         A generator function similar to `glob` that lists files in an S3 bucket
+
+        :param wildcard, Optional[str]: Pattern to match file keys against.
+        :param recursive, bool: If True, lists files recursively.
+
+        :yields: str: The keys of the files that match the criteria.
         """
         async with self._session.client(S3, **self._conn_config) as object_storage:
+
+            prefix = self.prefix or ""
+
+            if wildcard:
+                dir_path = os.path.dirname(wildcard)
+                if dir_path:
+                    prefix = os.path.join(prefix, dir_path) + "/"
+
             paginator = object_storage.get_paginator("list_objects_v2")
             async for result in paginator.paginate(
                 Bucket=self.bucket,
-                Prefix="" if not self.prefix else self.prefix,
-                Delimiter="/" if not recursive else "",
+                Prefix=prefix,
+                Delimiter="" if recursive else "/",
             ):
                 for content in result.get("Contents", []):
                     key = content["Key"]
-                    if wildcard and not fnmatch.fnmatch(key, wildcard):
+                    if wildcard and not fnmatch.fnmatch(
+                        key, (self.prefix or "") + wildcard
+                    ):
                         continue
-                    yield key
-
-    def partition_key(self, path: str) -> str:
-        """
-        Get the partition key for a given path.
-
-        :param path, str
-        :return str: the extracted partition key.
-        """
-        partition_key = ""
-        if self.partition_dateformat:
-            partition_key = path.rsplit("/", 1)[0]
-        ret = partition_key if not self.prefix else partition_key[len(self.prefix) :]
-        return ret
+                    yield self._prune_prefix(key)
 
     def _get_item_locator(
         self, item_path: str, n_part_comps: int, suffix: Optional[str] = None
     ) -> ItemLocator:
         """This method generates an `ItemLocator` object from a given `item_path`"""
         comps = item_path.split("/")
         partition_key = (
             "/".join(comps[(-n_part_comps - 1) : -1])
-            if self.partition_dateformat
+            if self.partition_dateformat or len(comps) > 1
             else None
         )
         item_id = comps[-1][: -len(suffix)] if suffix else comps[-1]
         return ItemLocator(item_id=item_id, partition_key=partition_key)
+
+    def _prune_prefix(self, file_path: str) -> str:
+        if self.prefix and file_path.startswith(self.prefix):
+            return file_path.replace(self.prefix, "", 1)
+        return file_path
```

### Comparing `hopeit_aws_s3-0.1.1/src/hopeit/aws/s3/partition.py` & `hopeit_aws_s3-0.1.2/src/hopeit/aws/s3/partition.py`

 * *Files identical despite different names*

### Comparing `hopeit_aws_s3-0.1.1/src/hopeit.aws.s3.egg-info/PKG-INFO` & `hopeit_aws_s3-0.1.2/src/hopeit.aws.s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.aws.s3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Hopeit Engine S3 Storage Toolkit
 Home-page: https://github.com/hopeit-git/hopeit.aws
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.aws/actions?query=workflow
 Project-URL: GitHub: issues, https://github.com/hopeit-git/hopeit.aws/issues
```


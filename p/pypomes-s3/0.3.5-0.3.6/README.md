# Comparing `tmp/pypomes_s3-0.3.5.tar.gz` & `tmp/pypomes_s3-0.3.6.tar.gz`

## Comparing `pypomes_s3-0.3.5.tar` & `pypomes_s3-0.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/__init__.py
--rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/aws_pomes.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/minio_client.py
--rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/minio_pomes.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/s3_common.py
--rw-r--r--   0        0        0    29382 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/s3_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/src/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/src/pypomes_s3/__init__.py
+-rw-r--r--   0        0        0    21995 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/src/pypomes_s3/aws_pomes.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/src/pypomes_s3/minio_client.py
+-rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/src/pypomes_s3/minio_pomes.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/src/pypomes_s3/s3_common.py
+-rw-r--r--   0        0        0    29336 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/src/pypomes_s3/s3_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pypomes_s3-0.3.6/PKG-INFO
```

### Comparing `pypomes_s3-0.3.5/src/pypomes_s3/__init__.py` & `pypomes_s3-0.3.6/src/pypomes_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.5/src/pypomes_s3/aws_pomes.py` & `pypomes_s3-0.3.6/src/pypomes_s3/aws_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                            engine="aws",
                            logger=logger)
     return result
 
 
 def file_store(errors: list[str],
                bucket: str,
-               basepath: Path | str,
+               basepath: str,
                identifier: str,
                filepath: Path | str,
                mimetype: str,
                tags: dict = None,
                client: BaseClient = None,
                logger: Logger = None) -> bool:
     """
@@ -140,15 +140,15 @@
                            engine="aws",
                            logger=logger)
     return result
 
 
 def file_retrieve(errors: list[str],
                   bucket: str,
-                  basepath: Path | str,
+                  basepath: str,
                   identifier: str,
                   filepath: Path | str,
                   client: BaseClient = None,
                   logger: Logger = None) -> Any:
     """
     Retrieve a file from the *AWS* store.
 
@@ -184,24 +184,24 @@
                                engine="aws",
                                logger=logger)
     return result
 
 
 def object_exists(errors: list[str],
                   bucket: str,
-                  basepath: Path | str,
+                  basepath: str,
                   identifier: str | None,
                   client: BaseClient = None,
                   logger: Logger = None) -> bool:
     """
     Determine if a given object exists in the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
-    :param basepath: the path specifying the location to locate the object at
+    :param basepath: the path specifying where to locate the object
     :param identifier: optional object identifier
     :param client: optional AWS client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: True if the object was found, false otherwise
     """
     # initialize the return variable
     result: bool = False
@@ -236,15 +236,15 @@
                 stmt=f"Object {remotepath}, bucket {bucket}, {existence}")
 
     return result
 
 
 def object_stat(errors: list[str],
                 bucket: str,
-                basepath: Path | str,
+                basepath: str,
                 identifier: str,
                 client: BaseClient = None,
                 logger: Logger = None) -> dict:
     """
     Retrieve and return the information about an object in the *AWS* store.
 
     :param errors: incidental error messages
@@ -277,15 +277,15 @@
                                engine="aws",
                                logger=logger)
     return result
 
 
 def object_store(errors: list[str],
                  bucket: str,
-                 basepath: Path | str,
+                 basepath: str,
                  identifier: str,
                  obj: Any,
                  tags: dict = None,
                  client: BaseClient = None,
                  logger: Logger = None) -> bool:
     """
     Store an object at the *AWS* store.
@@ -342,15 +342,15 @@
                 stmt=f"{storage} {remotepath}, bucket {bucket}")
 
     return result
 
 
 def object_retrieve(errors: list[str],
                     bucket: str,
-                    basepath: Path,
+                    basepath: str,
                     identifier: str,
                     client: BaseClient = None,
                     logger: Logger = None) -> Any:
     """
     Retrieve an object from the *AWS* store.
 
     :param errors: incidental error messages
```

### Comparing `pypomes_s3-0.3.5/src/pypomes_s3/minio_client.py` & `pypomes_s3-0.3.6/src/pypomes_s3/minio_client.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.5/src/pypomes_s3/minio_pomes.py` & `pypomes_s3-0.3.6/src/pypomes_s3/minio_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                            engine="minio",
                            logger=logger)
     return result
 
 
 def file_store(errors: list[str],
                bucket: str,
-               basepath: Path | str,
+               basepath: str,
                identifier: str,
                filepath: Path | str,
                mimetype: str,
                tags: dict = None,
                client: Minio = None,
                logger: Logger = None) -> bool:
     """
@@ -144,15 +144,15 @@
                            engine="minio",
                            logger=logger)
     return result
 
 
 def file_retrieve(errors: list[str],
                   bucket: str,
-                  basepath: Path | str,
+                  basepath: str,
                   identifier: str,
                   filepath: Path | str,
                   client: Minio = None,
                   logger: Logger = None) -> Any:
     """
     Retrieve a file from the *MinIO* store.
 
@@ -188,24 +188,24 @@
                                engine="minio",
                                logger=logger)
     return result
 
 
 def object_exists(errors: list[str],
                   bucket: str,
-                  basepath: Path | str,
+                  basepath: str,
                   identifier: str | None,
                   client: Minio = None,
                   logger: Logger = None) -> bool:
     """
     Determine if a given object exists in the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
-    :param basepath: the path specifying the location to locate the object at
+    :param basepath: the path specifying where to locate the object
     :param identifier: optional object identifier
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: True if the object was found, false otherwise
     """
     # initialize the return variable
     result: bool = False
@@ -240,15 +240,15 @@
                 stmt=f"Object {remotepath}, bucket {bucket}, {existence}")
 
     return result
 
 
 def object_stat(errors: list[str],
                 bucket: str,
-                basepath: Path | str,
+                basepath: str,
                 identifier: str,
                 client: Minio = None,
                 logger: Logger = None) -> MinioObject:
     """
     Retrieve and return the information about an object in the *MinIO* store.
 
     :param errors: incidental error messages
@@ -281,15 +281,15 @@
                                engine="minio",
                                logger=logger)
     return result
 
 
 def object_store(errors: list[str],
                  bucket: str,
-                 basepath: Path | str,
+                 basepath: str,
                  identifier: str,
                  obj: Any,
                  tags: dict = None,
                  client: Minio = None,
                  logger: Logger = None) -> bool:
     """
     Store an object at the *MinIO* store.
@@ -346,15 +346,15 @@
                 stmt=f"{storage} {remotepath}, bucket {bucket}")
 
     return result
 
 
 def object_retrieve(errors: list[str],
                     bucket: str,
-                    basepath: Path,
+                    basepath: str,
                     identifier: str,
                     client: Minio = None,
                     logger: Logger = None) -> Any:
     """
     Retrieve an object from the *MinIO* store.
 
     :param errors: incidental error messages
```

### Comparing `pypomes_s3-0.3.5/src/pypomes_s3/s3_common.py` & `pypomes_s3-0.3.6/src/pypomes_s3/s3_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.5/src/pypomes_s3/s3_pomes.py` & `pypomes_s3-0.3.6/src/pypomes_s3/s3_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_file_store(errors: list[str],
-                  basepath: Path | str,
+                  basepath: str,
                   identifier: str,
                   filepath: Path | str,
                   mimetype: str,
                   tags: dict = None,
                   bucket: str = None,
                   engine: Any = None,
                   client: Any = None,
@@ -271,15 +271,15 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_file_retrieve(errors: list[str],
-                     basepath: Path | str,
+                     basepath: str,
                      identifier: str,
                      filepath: Path | str,
                      bucket: str = None,
                      engine: str = None,
                      client: Any = None,
                      logger: Logger = None) -> Any:
     """
@@ -330,25 +330,25 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_exists(errors: list[str],
-                     basepath: Path | str,
+                     basepath: str,
                      identifier: str | None,
                      bucket: str = None,
                      engine: str = None,
                      client: Any = None,
                      logger: Logger = None) -> bool:
     """
     Determine if a given object exists in the S3 store.
 
     :param errors: incidental error messages
-    :param basepath: the path specifying the location to locate the object at
+    :param basepath: the path specifying where to locate the object
     :param identifier: optional object identifier
     :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: True if the object was found, false otherwise
     """
@@ -385,15 +385,15 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_stat(errors: list[str],
-                   basepath: Path | str,
+                   basepath: str,
                    identifier: str,
                    bucket: str = None,
                    engine: str = None,
                    client: Any = None,
                    logger: Logger = None) -> Any:
     """
     Retrieve and return the information about an object in the S3 store.
@@ -440,15 +440,15 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_store(errors: list[str],
-                    basepath: Path | str,
+                    basepath: str,
                     identifier: str,
                     obj: Any,
                     tags: dict = None,
                     bucket: str = None,
                     engine: str = None,
                     client: Any = None,
                     logger: Logger = None) -> bool:
@@ -503,15 +503,15 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_retrieve(errors: list[str],
-                       basepath: Path,
+                       basepath: str,
                        identifier: str,
                        bucket: str = None,
                        engine: str = None,
                        client: Any = None,
                        logger: Logger = None) -> Any:
     """
     Retrieve an object from the S3 store.
```

### Comparing `pypomes_s3-0.3.5/LICENSE` & `pypomes_s3-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.5/pyproject.toml` & `pypomes_s3-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_s3"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (S3 storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_s3-0.3.5/PKG-INFO` & `pypomes_s3-0.3.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_s3
-Version: 0.3.5
+Version: 0.3.6
 Summary: A collection of Python pomes, pennyeach (S3 storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-S3
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-S3/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/pypomes_s3-0.3.7.tar.gz` & `tmp/pypomes_s3-0.3.8.tar.gz`

## Comparing `pypomes_s3-0.3.7.tar` & `pypomes_s3-0.3.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/src/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/src/pypomes_s3/__init__.py
--rw-r--r--   0        0        0    21995 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/src/pypomes_s3/aws_pomes.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/src/pypomes_s3/minio_client.py
--rw-r--r--   0        0        0    22025 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/src/pypomes_s3/minio_pomes.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/src/pypomes_s3/s3_common.py
--rw-r--r--   0        0        0    29336 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/src/pypomes_s3/s3_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pypomes_s3-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/src/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/src/pypomes_s3/__init__.py
+-rw-r--r--   0        0        0    21995 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/src/pypomes_s3/aws_pomes.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/src/pypomes_s3/minio_client.py
+-rw-r--r--   0        0        0    22025 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/src/pypomes_s3/minio_pomes.py
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/src/pypomes_s3/s3_common.py
+-rw-r--r--   0        0        0    29336 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/src/pypomes_s3/s3_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pypomes_s3-0.3.8/PKG-INFO
```

### Comparing `pypomes_s3-0.3.7/src/pypomes_s3/__init__.py` & `pypomes_s3-0.3.8/src/pypomes_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.7/src/pypomes_s3/aws_pomes.py` & `pypomes_s3-0.3.8/src/pypomes_s3/aws_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.7/src/pypomes_s3/minio_client.py` & `pypomes_s3-0.3.8/src/pypomes_s3/minio_client.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.7/src/pypomes_s3/minio_pomes.py` & `pypomes_s3-0.3.8/src/pypomes_s3/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.7/src/pypomes_s3/s3_common.py` & `pypomes_s3-0.3.8/src/pypomes_s3/s3_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         _tag = "S3"
         _default_setup = False
     else:
         _tag: str = str_get_positional(source=engine,
                                        list_origin=["aws", "minio"],
                                        list_dest=["AWS", "MINIO"])
     _s3_data = {
-        "access-key":  env_get_str(f"{APP_PREFIX}_{_tag}_ACESS_KEY"),
+        "access-key":  env_get_str(f"{APP_PREFIX}_{_tag}_ACCESS_KEY"),
         "secret-key": env_get_str(f"{APP_PREFIX}_{_tag}_SECRET_KEY"),
         "bucket-name": env_get_str(f"{APP_PREFIX}_{_tag}_BUCKET_NAME"),
         "temp-folder": Path(env_get_str(f"{APP_PREFIX}_{_tag}_TEMP_FOLDER"))
     }
     if engine == "aws":
         _s3_data["client"] = env_get_str(f"{APP_PREFIX}_{_tag}_REGION_NAME")
     elif engine == "minio":
```

### Comparing `pypomes_s3-0.3.7/src/pypomes_s3/s3_pomes.py` & `pypomes_s3-0.3.8/src/pypomes_s3/s3_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.7/LICENSE` & `pypomes_s3-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.7/pyproject.toml` & `pypomes_s3-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_s3"
-version = "0.3.7"
+version = "0.3.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (S3 storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_s3-0.3.7/PKG-INFO` & `pypomes_s3-0.3.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_s3
-Version: 0.3.7
+Version: 0.3.8
 Summary: A collection of Python pomes, pennyeach (S3 storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-S3
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-S3/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


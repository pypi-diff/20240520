# Comparing `tmp/unibox-0.4.0.tar.gz` & `tmp/unibox-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.4.0.tar", max compression
+gzip compressed data, was "unibox-0.4.1.tar", max compression
```

## Comparing `unibox-0.4.0.tar` & `unibox-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2024-05-08 17:50:46.629745 unibox-0.4.0/LICENSE
--rw-r--r--   0        0        0     4088 2024-05-08 17:50:46.629745 unibox-0.4.0/README.md
--rw-r--r--   0        0        0      629 2024-05-08 17:50:46.629745 unibox-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4353 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/__init__.py
--rw-r--r--   0        0        0     5428 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/cli.py
--rw-r--r--   0        0        0        0 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/processing/__init__.py
--rw-r--r--   0        0        0     3051 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/processing/file_mover.py
--rw-r--r--   0        0        0     2149 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/processing/file_renamer.py
--rw-r--r--   0        0        0     7196 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/__init__.py
--rw-r--r--   0        0        0      244 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/constants.py
--rw-r--r--   0        0        0     6249 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/s3_client.py
--rw-r--r--   0        0        0     6751 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_loader.py
--rw-r--r--   0        0        0     4279 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_logger.py
--rw-r--r--   0        0        0     3139 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_merger.py
--rw-r--r--   0        0        0     4377 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_peeker.py
--rw-r--r--   0        0        0     8327 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_resizer.py
--rw-r--r--   0        0        0     5387 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_saver.py
--rw-r--r--   0        0        0     5885 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/uni_traverser.py
--rw-r--r--   0        0        0      580 2024-05-08 17:50:46.629745 unibox-0.4.0/unibox/utils/utils.py
--rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 unibox-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-20 01:53:31.357326 unibox-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4329 2024-05-20 01:53:31.361326 unibox-0.4.1/README.md
+-rw-r--r--   0        0        0      629 2024-05-20 01:53:31.361326 unibox-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4353 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/__init__.py
+-rw-r--r--   0        0        0     5428 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/cli.py
+-rw-r--r--   0        0        0        0 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     3051 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/processing/file_mover.py
+-rw-r--r--   0        0        0     2149 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/processing/file_renamer.py
+-rw-r--r--   0        0        0     7196 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/constants.py
+-rw-r--r--   0        0        0     6415 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/s3_client.py
+-rw-r--r--   0        0        0     6788 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_loader.py
+-rw-r--r--   0        0        0     4279 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_logger.py
+-rw-r--r--   0        0        0     3139 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_merger.py
+-rw-r--r--   0        0        0     4377 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_peeker.py
+-rw-r--r--   0        0        0     8327 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_resizer.py
+-rw-r--r--   0        0        0     5387 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_saver.py
+-rw-r--r--   0        0        0     5885 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/uni_traverser.py
+-rw-r--r--   0        0        0      580 2024-05-20 01:53:31.361326 unibox-0.4.1/unibox/utils/utils.py
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 unibox-0.4.1/PKG-INFO
```

### Comparing `unibox-0.4.0/LICENSE` & `unibox-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/README.md` & `unibox-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 - uses appropriate best practices (such as `orjson` package for json) for speed ups
 
 ```python
 some_dict = ub.loads("some_file.json")    # json → dict
 some_list = ub.loads("some_file.txt")     # txt  → list[str]
 some_img  = ub.loads("some_image.jpg")    # webp/jpg/png/..etc → PIL.Image
 some_df   = ub.loads("some_data.parquet") # parquet/csv/feather → pd.Dataframe
+
 # .... for more: see uni_loader.py#L40
 ```
 
 <br>
 
 **saving various python data structure in the same way**:
 
 - similar as `ub.loads` but also for saving files
 
 ```python
-# mostly similar as above
-ub.saves(some_dict, "some_file.json")
+ub.saves(some_dict, "some_file.json") # similar as above
 ub.saves(some_df, "some_df.parquet")
 ```
 
 <br>
 
 **list s3 or local directories in the same way:**
 
@@ -64,35 +64,43 @@
 
 **simplified logger class for easier debug**:
 
 - a logger with functionalities pre-configured
 - includes caller frame info, emoji warnings, datetime, and more
 
 ```python
+import unibox as ub
+
 logger = ub.UniLogger()
-logger.info("....") 
-logger.warn("....")
-logger.error("....")
+
+def some_function(): 
+    logger.info("some info") 
+    # logger.warning("....")
+    # logger.error("....")
+
+some_function()
+# 2024-05-08 17:57:23,149 [INFO] UniLogger: some_function: some info
 ```
 
 <br>
 
-**resizing millions of images efficiently**:
+**resize millions of images efficiently**:
 
-- (pre-configured omitted here for simplicity)
+- (pre-configured omitted here for simplicity; saves to 98% quality WEBP by default)
 - also able to resize by minimum or maximum of side lengths,
 
 ```python
-# Initialize resizer
-resizer = ub.UniResizer(root_dir, dst_dir,
-    target_pixels=int(1024 * 1024 * 1.5),
-)
+# root_dir: where the images to be resized are
+target_pixels = int(1024 * 1024 * 1.5)
+resizer = ub.UniResizer(root_dir, dst_dir, target_pixels)
 
-# Resize the images
+# get resize jobs
 images_to_resize = resizer.get_resize_jobs()
+
+# execute resize jobs
 resizer.execute_resize_jobs(images_to_resize)
 ```
 
 
 
 ## Install
```

### Comparing `unibox-0.4.0/pyproject.toml` & `unibox-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unibox"
-version = "0.4.0"
+version = "0.4.1"
 description = "Unibox provides unified interface for common file operations."
 authors = ["yada <trojblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/trojblue/unibox"
 
 [tool.poetry.dependencies]
```

### Comparing `unibox-0.4.0/unibox/__init__.py` & `unibox-0.4.1/unibox/__init__.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/cli.py` & `unibox-0.4.1/unibox/cli.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/processing/file_mover.py` & `unibox-0.4.1/unibox/processing/file_mover.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/processing/file_renamer.py` & `unibox-0.4.1/unibox/processing/file_renamer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/processing/image_resizer.py` & `unibox-0.4.1/unibox/processing/image_resizer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/utils/s3_client.py` & `unibox-0.4.1/unibox/utils/s3_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,28 +142,31 @@
                 dir_key = d['Prefix']
                 dir_entry = dir_key if relative_unix else f"s3://{bucket}/{dir_key}"
                 all_entries.append(dir_entry)
 
             # Add files to the list, applying filters if specified
             for obj in page.get('Contents', []):
                 file_key = obj["Key"]
+                if file_key == prefix:  # Skip the input directory itself
+                    continue
                 _, ext = os.path.splitext(file_key)
                 if include_extensions and ext not in include_extensions:
                     continue
                 if exclude_extensions and ext in exclude_extensions:
                     continue
 
                 file_entry = file_key[len(prefix):] if relative_unix else f"s3://{bucket}/{file_key}"
                 all_entries.append(file_entry)
 
+
         return all_entries
 
 
 if __name__ == '__main__':
     client = S3Client()
-    s3_uri = "s3://dataset-artstation-uw2/artists/_angelaramos_/"
+    # s3_uri = "s3://dataset-artstation-uw2/artists/_angelaramos_/"
+    s3_uri = "s3://dataset-ingested/gallery-dl/_todo_lists/"
     res = client.traverse(s3_uri)
 
     print(res)
-
     print("D")
```

### Comparing `unibox-0.4.0/unibox/utils/uni_loader.py` & `unibox-0.4.1/unibox/utils/uni_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             '.jpg': self._load_image,
             '.webp': self._load_image,
             '.jpeg': self._load_image,
             '.toml': self._load_toml,
             '.yaml': self._load_yaml,
             '.parquet': self._load_parquet,
             '.feather': self._load_feather,
+            ".har": self._load_json,
         }
 
     def _load_from_s3(self, s3_uri: str):
         """Download a file from an S3 URI and load its content."""
         s3_client = S3Client()
         try:
             with tempfile.TemporaryDirectory() as tmp_dir:
```

### Comparing `unibox-0.4.0/unibox/utils/uni_logger.py` & `unibox-0.4.1/unibox/utils/uni_logger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/utils/uni_merger.py` & `unibox-0.4.1/unibox/utils/uni_merger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/utils/uni_peeker.py` & `unibox-0.4.1/unibox/utils/uni_peeker.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/utils/uni_resizer.py` & `unibox-0.4.1/unibox/utils/uni_resizer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/utils/uni_saver.py` & `unibox-0.4.1/unibox/utils/uni_saver.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/utils/uni_traverser.py` & `unibox-0.4.1/unibox/utils/uni_traverser.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/unibox/utils/utils.py` & `unibox-0.4.1/unibox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `unibox-0.4.0/PKG-INFO` & `unibox-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unibox
-Version: 0.4.0
+Version: 0.4.1
 Summary: Unibox provides unified interface for common file operations.
 Home-page: https://github.com/trojblue/unibox
 License: MIT
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -57,26 +57,26 @@
 - uses appropriate best practices (such as `orjson` package for json) for speed ups
 
 ```python
 some_dict = ub.loads("some_file.json")    # json → dict
 some_list = ub.loads("some_file.txt")     # txt  → list[str]
 some_img  = ub.loads("some_image.jpg")    # webp/jpg/png/..etc → PIL.Image
 some_df   = ub.loads("some_data.parquet") # parquet/csv/feather → pd.Dataframe
+
 # .... for more: see uni_loader.py#L40
 ```
 
 <br>
 
 **saving various python data structure in the same way**:
 
 - similar as `ub.loads` but also for saving files
 
 ```python
-# mostly similar as above
-ub.saves(some_dict, "some_file.json")
+ub.saves(some_dict, "some_file.json") # similar as above
 ub.saves(some_df, "some_df.parquet")
 ```
 
 <br>
 
 **list s3 or local directories in the same way:**
 
@@ -94,35 +94,43 @@
 
 **simplified logger class for easier debug**:
 
 - a logger with functionalities pre-configured
 - includes caller frame info, emoji warnings, datetime, and more
 
 ```python
+import unibox as ub
+
 logger = ub.UniLogger()
-logger.info("....") 
-logger.warn("....")
-logger.error("....")
+
+def some_function(): 
+    logger.info("some info") 
+    # logger.warning("....")
+    # logger.error("....")
+
+some_function()
+# 2024-05-08 17:57:23,149 [INFO] UniLogger: some_function: some info
 ```
 
 <br>
 
-**resizing millions of images efficiently**:
+**resize millions of images efficiently**:
 
-- (pre-configured omitted here for simplicity)
+- (pre-configured omitted here for simplicity; saves to 98% quality WEBP by default)
 - also able to resize by minimum or maximum of side lengths,
 
 ```python
-# Initialize resizer
-resizer = ub.UniResizer(root_dir, dst_dir,
-    target_pixels=int(1024 * 1024 * 1.5),
-)
+# root_dir: where the images to be resized are
+target_pixels = int(1024 * 1024 * 1.5)
+resizer = ub.UniResizer(root_dir, dst_dir, target_pixels)
 
-# Resize the images
+# get resize jobs
 images_to_resize = resizer.get_resize_jobs()
+
+# execute resize jobs
 resizer.execute_resize_jobs(images_to_resize)
 ```
 
 
 
 ## Install
```


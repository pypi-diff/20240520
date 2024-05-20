# Comparing `tmp/burial_mounds-0.1.2.tar.gz` & `tmp/burial_mounds-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burial_mounds-0.1.2.tar", max compression
+gzip compressed data, was "burial_mounds-0.1.3.tar", max compression
```

## Comparing `burial_mounds-0.1.2.tar` & `burial_mounds-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-04-22 07:49:21.859560 burial_mounds-0.1.2/LICENSE
--rw-r--r--   0        0        0      100 2024-04-22 07:49:21.859560 burial_mounds-0.1.2/README.md
--rw-r--r--   0        0        0       53 2024-05-07 09:39:10.646657 burial_mounds-0.1.2/burial_mounds/__init__.py
--rw-r--r--   0        0        0      124 2024-05-07 10:06:17.874263 burial_mounds-0.1.2/burial_mounds/__main__.py
--rw-r--r--   0        0        0       45 2024-05-07 09:18:28.665769 burial_mounds-0.1.2/burial_mounds/cli.py
--rw-r--r--   0        0        0     1593 2024-05-20 08:26:21.357222 burial_mounds-0.1.2/burial_mounds/finetune.py
--rw-r--r--   0        0        0     2157 2024-05-07 10:05:45.822170 burial_mounds-0.1.2/burial_mounds/hub.py
--rw-r--r--   0        0        0     7019 2024-05-20 09:21:03.038104 burial_mounds-0.1.2/burial_mounds/preprocess_mounds.py
--rw-r--r--   0        0        0     5890 2024-05-19 13:46:15.939729 burial_mounds-0.1.2/burial_mounds/preprocess_xview.py
--rw-r--r--   0        0        0     2566 2024-05-20 08:46:21.207877 burial_mounds-0.1.2/burial_mounds/utils.py
--rw-r--r--   0        0        0      514 2024-05-20 10:52:42.164472 burial_mounds-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 burial_mounds-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-22 07:49:21.859560 burial_mounds-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5808 2024-05-20 11:54:58.570945 burial_mounds-0.1.3/README.md
+-rw-r--r--   0        0        0       53 2024-05-07 09:39:10.646657 burial_mounds-0.1.3/burial_mounds/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-07 10:06:17.874263 burial_mounds-0.1.3/burial_mounds/__main__.py
+-rw-r--r--   0        0        0       45 2024-05-07 09:18:28.665769 burial_mounds-0.1.3/burial_mounds/cli.py
+-rw-r--r--   0        0        0     1579 2024-05-20 11:47:17.337595 burial_mounds-0.1.3/burial_mounds/finetune.py
+-rw-r--r--   0        0        0     2157 2024-05-07 10:05:45.822170 burial_mounds-0.1.3/burial_mounds/hub.py
+-rw-r--r--   0        0        0     7019 2024-05-20 09:21:03.038104 burial_mounds-0.1.3/burial_mounds/preprocess_mounds.py
+-rw-r--r--   0        0        0     5890 2024-05-19 13:46:15.939729 burial_mounds-0.1.3/burial_mounds/preprocess_xview.py
+-rw-r--r--   0        0        0     2566 2024-05-20 08:46:21.207877 burial_mounds-0.1.3/burial_mounds/utils.py
+-rw-r--r--   0        0        0      514 2024-05-20 11:56:12.391157 burial_mounds-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6736 1970-01-01 00:00:00.000000 burial_mounds-0.1.3/PKG-INFO
```

### Comparing `burial_mounds-0.1.2/LICENSE` & `burial_mounds-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.2/burial_mounds/finetune.py` & `burial_mounds-0.1.3/burial_mounds/finetune.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,18 @@
         flipud=0.3,
         optimizer="Adam",
         lr0=0.01,
     )
 
     print("Validating model:")
     model.val()
-    success = model.export(format="onnx")
+    success = model.export()
     success = Path(success)
 
     extension = success.suffix
     base_model_name = Path(base_model).stem
     out_path = models_dir.joinpath(
-        f"{config_path.stem}_base-{base_model_name}_best.{extension}"
+        f"{config_path.stem}_base-{base_model_name}_best{extension}"
     )
     # Moving model to output path
     success.rename(out_path)
     print(f"Saved best model to {out_path}")
```

### Comparing `burial_mounds-0.1.2/burial_mounds/hub.py` & `burial_mounds-0.1.3/burial_mounds/hub.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.2/burial_mounds/preprocess_mounds.py` & `burial_mounds-0.1.3/burial_mounds/preprocess_mounds.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.2/burial_mounds/preprocess_xview.py` & `burial_mounds-0.1.3/burial_mounds/preprocess_xview.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.2/burial_mounds/utils.py` & `burial_mounds-0.1.3/burial_mounds/utils.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.2/pyproject.toml` & `burial_mounds-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burial-mounds"
-version = "0.1.2"
+version = "0.1.3"
 description = "Recognizing burial mounds with YOLO"
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```


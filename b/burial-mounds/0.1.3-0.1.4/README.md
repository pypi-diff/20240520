# Comparing `tmp/burial_mounds-0.1.3.tar.gz` & `tmp/burial_mounds-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burial_mounds-0.1.3.tar", max compression
+gzip compressed data, was "burial_mounds-0.1.4.tar", max compression
```

## Comparing `burial_mounds-0.1.3.tar` & `burial_mounds-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-04-22 07:49:21.859560 burial_mounds-0.1.3/LICENSE
--rw-r--r--   0        0        0     5808 2024-05-20 11:54:58.570945 burial_mounds-0.1.3/README.md
--rw-r--r--   0        0        0       53 2024-05-07 09:39:10.646657 burial_mounds-0.1.3/burial_mounds/__init__.py
--rw-r--r--   0        0        0      124 2024-05-07 10:06:17.874263 burial_mounds-0.1.3/burial_mounds/__main__.py
--rw-r--r--   0        0        0       45 2024-05-07 09:18:28.665769 burial_mounds-0.1.3/burial_mounds/cli.py
--rw-r--r--   0        0        0     1579 2024-05-20 11:47:17.337595 burial_mounds-0.1.3/burial_mounds/finetune.py
--rw-r--r--   0        0        0     2157 2024-05-07 10:05:45.822170 burial_mounds-0.1.3/burial_mounds/hub.py
--rw-r--r--   0        0        0     7019 2024-05-20 09:21:03.038104 burial_mounds-0.1.3/burial_mounds/preprocess_mounds.py
--rw-r--r--   0        0        0     5890 2024-05-19 13:46:15.939729 burial_mounds-0.1.3/burial_mounds/preprocess_xview.py
--rw-r--r--   0        0        0     2566 2024-05-20 08:46:21.207877 burial_mounds-0.1.3/burial_mounds/utils.py
--rw-r--r--   0        0        0      514 2024-05-20 11:56:12.391157 burial_mounds-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6736 1970-01-01 00:00:00.000000 burial_mounds-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-22 07:49:21.859560 burial_mounds-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6779 2024-05-20 12:05:23.784727 burial_mounds-0.1.4/README.md
+-rw-r--r--   0        0        0       53 2024-05-07 09:39:10.646657 burial_mounds-0.1.4/burial_mounds/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-07 10:06:17.874263 burial_mounds-0.1.4/burial_mounds/__main__.py
+-rw-r--r--   0        0        0       45 2024-05-07 09:18:28.665769 burial_mounds-0.1.4/burial_mounds/cli.py
+-rw-r--r--   0        0        0     1752 2024-05-20 12:23:06.423889 burial_mounds-0.1.4/burial_mounds/finetune.py
+-rw-r--r--   0        0        0     2157 2024-05-07 10:05:45.822170 burial_mounds-0.1.4/burial_mounds/hub.py
+-rw-r--r--   0        0        0     7019 2024-05-20 09:21:03.038104 burial_mounds-0.1.4/burial_mounds/preprocess_mounds.py
+-rw-r--r--   0        0        0     5890 2024-05-19 13:46:15.939729 burial_mounds-0.1.4/burial_mounds/preprocess_xview.py
+-rw-r--r--   0        0        0     2566 2024-05-20 08:46:21.207877 burial_mounds-0.1.4/burial_mounds/utils.py
+-rw-r--r--   0        0        0      514 2024-05-20 12:23:49.812017 burial_mounds-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7707 1970-01-01 00:00:00.000000 burial_mounds-0.1.4/PKG-INFO
```

### Comparing `burial_mounds-0.1.3/LICENSE` & `burial_mounds-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.3/README.md` & `burial_mounds-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -124,9 +124,34 @@
 ```
 
 ### Publishing
 
 If you intend to publish a trained model to the HuggingFace Hub you can use the `push_to_hub` command.
 
 ```bash
-python3 -m burial_mounds push_to_hub --model_path "models/mounds_base-yolov8n_best.pt" --repo_id "chcaa/burial-mounds_yolo8n_obb"
+python3 -m burial_mounds push_to_hub --model_path "models/mounds_base-yolov8n_best.pt" --repo_id "chcaa/burial-mounds_yolov8n"
 ```
+
+### Inference
+
+You can use the models trained with this package like any other YOLO model.
+The package also comes with a convenience function for loading models from HuggingFace repositories.
+
+```python
+from burial_mounds.hub import load_from_hub
+
+model = load_from_hub("chcaa/burial_mounds_yolov8n")
+
+mounds = model(["data/mounds/images/east_30.png"])
+
+# Process results list
+for result in results:
+    boxes = result.boxes  # Boxes object for bounding box outputs
+    masks = result.masks  # Masks object for segmentation masks outputs
+    keypoints = result.keypoints  # Keypoints object for pose outputs
+    probs = result.probs  # Probs object for classification outputs
+    obb = result.obb  # Oriented boxes object for OBB outputs
+    result.show()  # display to screen
+    result.save(filename="result.jpg")  # save to disk
+```
+
+For a more detailed guide consult the [YOLOv8 documentation](https://docs.ultralytics.com/modes/predict/#key-features-of-predict-mode).
```

### Comparing `burial_mounds-0.1.3/burial_mounds/finetune.py` & `burial_mounds-0.1.4/burial_mounds/finetune.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 
 @cli.command(
     "finetune",
     base_model=Arg(help="Base Model to finetune."),
     config=Arg(help="Name of the config to finetune the model on or path to config."),
     epochs=Arg("--epochs", "-e", help="Number of epochs for training."),
     image_size=Arg("--image_size", "-s", help="Size of the images to use in training."),
+    scale_images=Arg(
+        "--scale_images", help="Factor to scale the images by when augmenting data."
+    ),
 )
 def finetune(
     base_model: str,
     config: str,
     epochs: int = 100,
     image_size: int = 640,
+    scale_images: float = 2.0,
 ):
     # User may either specify a path to a config file, or just a name like "mounds", "xview"
     if config.endswith(".yaml") or config.endswith(".yml"):
         config_path = Path(config)
     else:
         config_path = Path("configs").joinpath(f"{config}.yaml")
 
@@ -36,14 +40,15 @@
         data=config_path,
         epochs=epochs,
         imgsz=image_size,
         degrees=180,
         flipud=0.3,
         optimizer="Adam",
         lr0=0.01,
+        scale=scale_images,
     )
 
     print("Validating model:")
     model.val()
     success = model.export()
     success = Path(success)
```

### Comparing `burial_mounds-0.1.3/burial_mounds/hub.py` & `burial_mounds-0.1.4/burial_mounds/hub.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.3/burial_mounds/preprocess_mounds.py` & `burial_mounds-0.1.4/burial_mounds/preprocess_mounds.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.3/burial_mounds/preprocess_xview.py` & `burial_mounds-0.1.4/burial_mounds/preprocess_xview.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.3/burial_mounds/utils.py` & `burial_mounds-0.1.4/burial_mounds/utils.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.3/pyproject.toml` & `burial_mounds-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burial-mounds"
-version = "0.1.3"
+version = "0.1.4"
 description = "Recognizing burial mounds with YOLO"
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `burial_mounds-0.1.3/PKG-INFO` & `burial_mounds-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burial-mounds
-Version: 0.1.3
+Version: 0.1.4
 Summary: Recognizing burial mounds with YOLO
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -149,10 +149,35 @@
 ```
 
 ### Publishing
 
 If you intend to publish a trained model to the HuggingFace Hub you can use the `push_to_hub` command.
 
 ```bash
-python3 -m burial_mounds push_to_hub --model_path "models/mounds_base-yolov8n_best.pt" --repo_id "chcaa/burial-mounds_yolo8n_obb"
+python3 -m burial_mounds push_to_hub --model_path "models/mounds_base-yolov8n_best.pt" --repo_id "chcaa/burial-mounds_yolov8n"
 ```
 
+### Inference
+
+You can use the models trained with this package like any other YOLO model.
+The package also comes with a convenience function for loading models from HuggingFace repositories.
+
+```python
+from burial_mounds.hub import load_from_hub
+
+model = load_from_hub("chcaa/burial_mounds_yolov8n")
+
+mounds = model(["data/mounds/images/east_30.png"])
+
+# Process results list
+for result in results:
+    boxes = result.boxes  # Boxes object for bounding box outputs
+    masks = result.masks  # Masks object for segmentation masks outputs
+    keypoints = result.keypoints  # Keypoints object for pose outputs
+    probs = result.probs  # Probs object for classification outputs
+    obb = result.obb  # Oriented boxes object for OBB outputs
+    result.show()  # display to screen
+    result.save(filename="result.jpg")  # save to disk
+```
+
+For a more detailed guide consult the [YOLOv8 documentation](https://docs.ultralytics.com/modes/predict/#key-features-of-predict-mode).
+
```


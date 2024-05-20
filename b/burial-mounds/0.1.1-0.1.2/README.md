# Comparing `tmp/burial_mounds-0.1.1.tar.gz` & `tmp/burial_mounds-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burial_mounds-0.1.1.tar", max compression
+gzip compressed data, was "burial_mounds-0.1.2.tar", max compression
```

## Comparing `burial_mounds-0.1.1.tar` & `burial_mounds-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-04-22 07:49:21.859560 burial_mounds-0.1.1/LICENSE
--rw-r--r--   0        0        0      100 2024-04-22 07:49:21.859560 burial_mounds-0.1.1/README.md
--rw-r--r--   0        0        0       53 2024-05-07 09:39:10.646657 burial_mounds-0.1.1/burial_mounds/__init__.py
--rw-r--r--   0        0        0      124 2024-05-07 10:06:17.874263 burial_mounds-0.1.1/burial_mounds/__main__.py
--rw-r--r--   0        0        0       45 2024-05-07 09:18:28.665769 burial_mounds-0.1.1/burial_mounds/cli.py
--rw-r--r--   0        0        0     1299 2024-05-07 09:42:47.376593 burial_mounds-0.1.1/burial_mounds/finetune.py
--rw-r--r--   0        0        0     2157 2024-05-07 10:05:45.822170 burial_mounds-0.1.1/burial_mounds/hub.py
--rw-r--r--   0        0        0     6057 2024-05-07 09:42:57.272683 burial_mounds-0.1.1/burial_mounds/preprocess_mounds.py
--rw-r--r--   0        0        0     4114 2024-05-17 09:37:15.144768 burial_mounds-0.1.1/burial_mounds/preprocess_xview.py
--rw-r--r--   0        0        0      514 2024-05-17 09:39:49.083785 burial_mounds-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 burial_mounds-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-22 07:49:21.859560 burial_mounds-0.1.2/LICENSE
+-rw-r--r--   0        0        0      100 2024-04-22 07:49:21.859560 burial_mounds-0.1.2/README.md
+-rw-r--r--   0        0        0       53 2024-05-07 09:39:10.646657 burial_mounds-0.1.2/burial_mounds/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-07 10:06:17.874263 burial_mounds-0.1.2/burial_mounds/__main__.py
+-rw-r--r--   0        0        0       45 2024-05-07 09:18:28.665769 burial_mounds-0.1.2/burial_mounds/cli.py
+-rw-r--r--   0        0        0     1593 2024-05-20 08:26:21.357222 burial_mounds-0.1.2/burial_mounds/finetune.py
+-rw-r--r--   0        0        0     2157 2024-05-07 10:05:45.822170 burial_mounds-0.1.2/burial_mounds/hub.py
+-rw-r--r--   0        0        0     7019 2024-05-20 09:21:03.038104 burial_mounds-0.1.2/burial_mounds/preprocess_mounds.py
+-rw-r--r--   0        0        0     5890 2024-05-19 13:46:15.939729 burial_mounds-0.1.2/burial_mounds/preprocess_xview.py
+-rw-r--r--   0        0        0     2566 2024-05-20 08:46:21.207877 burial_mounds-0.1.2/burial_mounds/utils.py
+-rw-r--r--   0        0        0      514 2024-05-20 10:52:42.164472 burial_mounds-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 burial_mounds-0.1.2/PKG-INFO
```

### Comparing `burial_mounds-0.1.1/LICENSE` & `burial_mounds-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.1/burial_mounds/finetune.py` & `burial_mounds-0.1.2/burial_mounds/finetune.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,42 +4,54 @@
 from ultralytics import YOLO
 
 from burial_mounds.cli import cli
 
 
 @cli.command(
     "finetune",
+    base_model=Arg(help="Base Model to finetune."),
     config=Arg(help="Name of the config to finetune the model on or path to config."),
-    base_model=Arg("--base_model", "-b", help="Base Model to finetune."),
     epochs=Arg("--epochs", "-e", help="Number of epochs for training."),
+    image_size=Arg("--image_size", "-s", help="Size of the images to use in training."),
 )
 def finetune(
+    base_model: str,
     config: str,
-    base_model: str = "yolov8n.pt",
     epochs: int = 100,
+    image_size: int = 640,
 ):
     # User may either specify a path to a config file, or just a name like "mounds", "xview"
     if config.endswith(".yaml") or config.endswith(".yml"):
         config_path = Path(config)
     else:
         config_path = Path("configs").joinpath(f"{config}.yaml")
 
     models_dir = Path("models/")
     models_dir.mkdir(exist_ok=True)
 
     print("Training model")
     # Load a model
-    model = YOLO("yolov8n.pt")
+    model = YOLO(base_model)
     # Train the model
-    results = model.train(data=config_path, epochs=epochs, imgsz=640)
+    results = model.train(
+        data=config_path,
+        epochs=epochs,
+        imgsz=image_size,
+        degrees=180,
+        flipud=0.3,
+        optimizer="Adam",
+        lr0=0.01,
+    )
 
     print("Validating model:")
     model.val()
     success = model.export(format="onnx")
     success = Path(success)
 
     extension = success.suffix
+    base_model_name = Path(base_model).stem
     out_path = models_dir.joinpath(
-        f"{config_path.stem}_base-{base_model}_best.{extension}"
+        f"{config_path.stem}_base-{base_model_name}_best.{extension}"
     )
     # Moving model to output path
     success.rename(out_path)
+    print(f"Saved best model to {out_path}")
```

### Comparing `burial_mounds-0.1.1/burial_mounds/hub.py` & `burial_mounds-0.1.2/burial_mounds/hub.py`

 * *Files identical despite different names*

### Comparing `burial_mounds-0.1.1/burial_mounds/preprocess_mounds.py` & `burial_mounds-0.1.2/burial_mounds/preprocess_mounds.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from pathlib import Path
-from typing import Iterable
+from typing import Iterable, Literal
 
 import geopandas as gpd
 import numpy as np
 import rasterio
 import shapely
 from PIL import Image, ImageEnhance
 from radicli import Arg
 from rasterio.features import geometry_window
-from rasterio.windows import Window
+from rasterio.windows import Window, WindowError
 from tqdm import tqdm
 from ultralytics.data.utils import autosplit
-from ultralytics.utils.ops import xywhn2xyxy, xyxy2xywhn
-from ultralytics.utils.plotting import Annotator
 
 from burial_mounds.cli import cli
+from burial_mounds.utils import convert_bbox, image_with_annotations
 
 MOUNDS_CONFIG = """
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-path: ../data/TRAP_Data
+path: ../{out_dir}
 train: autosplit_train.txt
 val: autosplit_val.txt
 
 # Classes
 names:
   0: Mound
 """
@@ -32,106 +31,138 @@
 def minmax(channel: np.ndarray) -> np.ndarray:
     """Minmax normalizes a whole array and keeps it the same shape."""
     return (channel - np.min(channel)) / (np.max(channel) - np.min(channel))
 
 
 def iterate_windows(dataset, size: int = 1024) -> Iterable[tuple[int, int, Window]]:
     """Iterates through windows in a rasterio dataset."""
-    w, h = dataset.shape
+    h, w = dataset.shape
     for i_horizontal in range(w // size):
         for i_vertical in range(h // size):
-            yield i_horizontal, i_vertical, Window(
-                i_vertical * size, i_horizontal * size, size, size
-            )
-
-
-def to_yolo_entry(bbox, width, height) -> list[str]:
-    """Turns bounding boxes to YOLO annotation entries."""
-    yolo_bbox = xyxy2xywhn(
-        x=np.array(bbox, dtype=np.float64), w=width, h=height, clip=True
-    )
-    yolo_bbox_str = [f"{coord:.6f}" for coord in yolo_bbox]
-    return ["0", *yolo_bbox_str]
+            window = Window(i_vertical * size, i_horizontal * size, size, size)
+            yield i_horizontal, i_vertical, window
 
 
-def image_with_annotations(
-    image: np.ndarray, annotations: list[list[str]]
-) -> np.ndarray:
-    """Produces image with annotations on them."""
-    annotator = Annotator(image)
-    w, h, *_ = image.shape
-    for label, *xywhn in annotations:
-        xywhn = np.array([float(coord) for coord in xywhn])
-        xyxy = xywhn2xyxy(xywhn, w=w, h=h)
-        annotator.box_label(box=xyxy, label=label)
-    return annotator.result()
+def get_bounding_box(
+    polygon: shapely.Polygon, window: Window, dataset
+) -> tuple[int, int, int, int]:
+    """Returns bounding box of of feature in a rasterio dataset in a window."""
+    enclosing_window = geometry_window(dataset, [polygon])
+    x_min = enclosing_window.col_off - window.col_off
+    y_min = enclosing_window.row_off - window.row_off
+    x_max = enclosing_window.col_off + enclosing_window.width - window.col_off
+    y_max = enclosing_window.row_off + enclosing_window.height - window.row_off
+    return x_min, y_min, x_max, y_max
+
+
+def get_labels_in_window(
+    polygons: Iterable[shapely.Polygon],
+    window: Window,
+    dataset,
+    image_size: int,
+    format: Literal["detect", "obb"] = "obb",
+) -> Iterable[list[str]]:
+    """Yields YOLO label entries in a window in a dataset
+    for each bounding polygons."""
+    window_bounds = shapely.box(*dataset.window_bounds(window))
+    # YOLO entries for window
+    for polygon in polygons:
+        if not polygon.intersects(window_bounds):
+            continue
+        polygon = polygon.intersection(window_bounds)
+        try:
+            bbox = get_bounding_box(polygon=polygon, window=window, dataset=dataset)
+            bbox = convert_bbox(
+                bbox,
+                width=image_size,
+                height=image_size,
+                format=format,
+            )
+            yield ["0"] + [f"{coord:.6f}" for coord in bbox]
+        except WindowError as e:
+            print(f"WARNING: Couldn't add feature on window, {e}")
 
 
 @cli.command(
     "preprocess_mounds",
     data_dir=Arg("--data_dir", "-d", help="Data where mounds data is located."),
+    out_dir=Arg(
+        "--out_dir", "-o", help="Data where mounds YOLO dataset should be saved."
+    ),
     image_size=Arg(
         "--image_size", "-s", help="Size of the square shaped images to produce."
     ),
+    format=Arg("--format", "-f", help="Format of the dataset {'detect' or 'obb'}"),
 )
-def preprocess_mounds(data_dir: str = "data/TRAP_Data", image_size: int = 640):
+def preprocess_mounds(
+    data_dir: str = "data/TRAP_Data",
+    out_dir: str = "data/mounds",
+    image_size: int = 1024,
+    format: Literal["obb", "detect"] = "obb",
+):
     """Preprocesses the mounds dataset.
     Creates square images with annotations, corrects satellite color
     channels and produces train and test splits."""
+    print(
+        f"""
+    Preprocessing burial mounds dataset with following parameters:
+      - directory: {data_dir}
+      - window size: {image_size} x {image_size}
+      - format: {format}
+    """
+    )
     data_path = Path(data_dir)
     print("Loading bounding boxes")
     boxes = gpd.read_file(data_path.joinpath("Kaz_mndbbox.geojson"))
     boxes = boxes.set_crs(epsg=32635, allow_override=True)
+    out_path = Path(out_dir)
+    out_path.mkdir(exist_ok=True, parents=True)
 
     files = {
         "east": data_path.joinpath("East/kaz_e_fuse.img"),
-        "west": data_path.joinpath("East/kaz_w_fuse.img"),
-        "joint": data_path.joinpath("East/kaz_fuse.img"),
+        "west": data_path.joinpath("West/kaz_w_fuse.img"),
+        # "joint": data_path.joinpath("kaz_fuse.img"),
     }
-    images_path = data_path.joinpath("images")
+    images_path = out_path.joinpath("images")
     images_path.mkdir(exist_ok=True)
-    labels_path = data_path.joinpath("labels")
+    labels_path = out_path.joinpath("labels")
     labels_path.mkdir(exist_ok=True)
-    annotated_path = data_path.joinpath("annotated")
+    annotated_path = out_path.joinpath("annotated")
     annotated_path.mkdir(exist_ok=True)
+    print("Deleting previous images.")
+    for file in images_path.glob("*.png"):
+        file.unlink()
+    for file in annotated_path.glob("*.png"):
+        file.unlink()
     bands = []
     # YOLO entries for each image
     entries: list[list[list[str]]] = []
     for name, file in files.items():
         print(f"Processing {name}")
         with rasterio.open(file) as dataset:
-            windows = list(iterate_windows(dataset))
+            windows = list(iterate_windows(dataset, size=image_size))
             for i, j, window in tqdm(windows, desc="Going through windows."):
-                window_bounds = shapely.box(*dataset.window_bounds(window))
                 # YOLO entries for window
-                window_entries: list[list[str]] = []
-                for certainty, polygon in zip(boxes.Certainty, boxes.geometry):
-                    if not polygon.intersects(window_bounds):
-                        continue
-                    polygon = polygon.intersection(window_bounds)
-                    enclosing_window = geometry_window(dataset, [polygon])
-                    bbox = [
-                        enclosing_window.col_off - window.col_off,
-                        enclosing_window.row_off - window.row_off,
-                        enclosing_window.col_off
-                        + enclosing_window.width
-                        - window.col_off,
-                        enclosing_window.row_off
-                        + enclosing_window.height
-                        - window.row_off,
-                    ]
-                    window_entries.append(
-                        to_yolo_entry(bbox, width=image_size, height=image_size)
+                window_entries: list[list[str]] = list(
+                    get_labels_in_window(
+                        boxes.geometry,
+                        window=window,
+                        dataset=dataset,
+                        image_size=image_size,
+                        format=format,
                     )
+                )
                 # Go to next window if there are no mounds in it
                 if not window_entries:
                     continue
                 image = np.stack([dataset.read(ch, window=window) for ch in (1, 2, 3)])
-                bands.append(image)
-                entries.append(window_entries)
+                # Only appending image if it is large enough
+                if (image.shape[1], image.shape[2]) == (image_size, image_size):
+                    bands.append(image)
+                    entries.append(window_entries)
 
         images = np.stack(bands)
         images = minmax(images) * 256
         idx = tqdm(np.arange(len(images)), desc="Saving images")
         for i, image, window_entries in zip(idx, images, entries):
             image = Image.merge(
                 "RGB", [Image.fromarray(ch.astype(np.uint8)) for ch in image]
@@ -150,8 +181,8 @@
     print("Producing training and validation splits.")
     autosplit(images_path)
 
     print("Saving config")
     configs_dir = Path("configs")
     configs_dir.mkdir(exist_ok=True)
     with configs_dir.joinpath("mounds.yaml").open("w") as config_file:
-        config_file.write(MOUNDS_CONFIG)
+        config_file.write(MOUNDS_CONFIG.format(out_dir=out_dir))
```

### Comparing `burial_mounds-0.1.1/pyproject.toml` & `burial_mounds-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burial-mounds"
-version = "0.1.1"
+version = "0.1.2"
 description = "Recognizing burial mounds with YOLO"
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `burial_mounds-0.1.1/PKG-INFO` & `burial_mounds-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burial-mounds
-Version: 0.1.1
+Version: 0.1.2
 Summary: Recognizing burial mounds with YOLO
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/seg_tgce-0.1.1.tar.gz` & `tmp/seg_tgce-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seg_tgce-0.1.1.tar", max compression
+gzip compressed data, was "seg_tgce-0.1.2.tar", max compression
```

## Comparing `seg_tgce-0.1.1.tar` & `seg_tgce-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0      322 2024-05-14 04:12:07.157195 seg_tgce-0.1.1/README.md
--rw-r--r--   0        0        0     1580 2024-05-14 05:03:56.356442 seg_tgce-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 14:27:20.493094 seg_tgce-0.1.1/seg_tgce/data/crowd_seg/__init__.py
--rw-r--r--   0        0        0     4937 2024-05-07 10:46:36.549085 seg_tgce-0.1.1/seg_tgce/data/crowd_seg/generator.py
--rw-r--r--   0        0        0      475 2024-04-30 04:42:11.177868 seg_tgce-0.1.1/seg_tgce/data/crowd_seg/map.py
--rw-r--r--   0        0        0     2231 2024-05-06 04:51:09.581252 seg_tgce-0.1.1/seg_tgce/data/crowd_seg/visualizer.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/data/oxford_pet/__init__.py
--rw-r--r--   0        0        0     2465 2024-05-06 05:34:13.661853 seg_tgce-0.1.1/seg_tgce/data/oxford_pet/disturbance/model.py
--rw-r--r--   0        0        0     2711 2024-05-14 03:29:38.912294 seg_tgce-0.1.1/seg_tgce/data/oxford_pet/oxford_iiit_pet.py
--rw-r--r--   0        0        0      876 2024-05-14 03:55:28.061819 seg_tgce-0.1.1/seg_tgce/data/oxford_pet/oxford_pet.py
--rw-r--r--   0        0        0     2228 2024-05-14 03:55:28.058486 seg_tgce-0.1.1/seg_tgce/data/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/experiments/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/experiments/apr_14_2024/__init__.py
--rw-r--r--   0        0        0      856 2024-05-06 05:22:24.575116 seg_tgce-0.1.1/seg_tgce/experiments/apr_14_2024/experiment.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/loss/__init__.py
--rw-r--r--   0        0        0     3290 2024-05-06 04:49:42.271689 seg_tgce-0.1.1/seg_tgce/loss/tgce.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/metrics/__init__.py
--rw-r--r--   0        0        0     1225 2024-05-06 05:24:38.627838 seg_tgce-0.1.1/seg_tgce/metrics/dice_coefficient.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/models/__init__.py
--rw-r--r--   0        0        0      746 2024-05-06 05:22:57.754965 seg_tgce-0.1.1/seg_tgce/models/ma_model.py
--rw-r--r--   0        0        0     4618 2024-05-06 05:10:53.688560 seg_tgce-0.1.1/seg_tgce/models/unet.py
--rw-r--r--   0        0        0        0 2024-04-30 04:42:11.177868 seg_tgce-0.1.1/seg_tgce/py.typed
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/run/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 04:39:26.044844 seg_tgce-0.1.1/seg_tgce/run/oxford_ma_runner/__init__.py
--rw-r--r--   0        0        0      414 2024-05-06 05:13:40.777698 seg_tgce-0.1.1/seg_tgce/run/oxford_ma_runner/model_result.py
--rw-r--r--   0        0        0     2468 2024-05-06 05:24:38.624505 seg_tgce-0.1.1/seg_tgce/run/oxford_ma_runner/plotting.py
--rw-r--r--   0        0        0     7072 2024-05-07 11:10:44.874873 seg_tgce-0.1.1/seg_tgce/run/oxford_ma_runner/runner.py
--rw-r--r--   0        0        0      800 2024-04-16 19:11:40.745930 seg_tgce-0.1.1/seg_tgce/run/runner.py
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 seg_tgce-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      322 2024-05-14 04:12:07.157195 seg_tgce-0.1.2/README.md
+-rw-r--r--   0        0        0     1580 2024-05-20 13:15:37.004961 seg_tgce-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/data/__init__.py
+-rw-r--r--   0        0        0     1238 2024-05-20 13:03:41.594701 seg_tgce-0.1.2/seg_tgce/data/crowd_seg/__init__.py
+-rw-r--r--   0        0        0      274 2024-05-20 12:50:59.994994 seg_tgce-0.1.2/seg_tgce/data/crowd_seg/__main__.py
+-rw-r--r--   0        0        0     4829 2024-05-20 12:41:31.854328 seg_tgce-0.1.2/seg_tgce/data/crowd_seg/generator.py
+-rw-r--r--   0        0        0      475 2024-04-30 04:42:11.177868 seg_tgce-0.1.2/seg_tgce/data/crowd_seg/map.py
+-rw-r--r--   0        0        0     1001 2024-05-20 12:31:40.420402 seg_tgce-0.1.2/seg_tgce/data/crowd_seg/retrieve.py
+-rw-r--r--   0        0        0      166 2024-05-20 11:50:15.678622 seg_tgce-0.1.2/seg_tgce/data/crowd_seg/stage.py
+-rw-r--r--   0        0        0     2231 2024-05-06 04:51:09.581252 seg_tgce-0.1.2/seg_tgce/data/crowd_seg/visualizer.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/data/oxford_pet/__init__.py
+-rw-r--r--   0        0        0     2465 2024-05-06 05:34:13.661853 seg_tgce-0.1.2/seg_tgce/data/oxford_pet/disturbance/model.py
+-rw-r--r--   0        0        0     2711 2024-05-14 03:29:38.912294 seg_tgce-0.1.2/seg_tgce/data/oxford_pet/oxford_iiit_pet.py
+-rw-r--r--   0        0        0      876 2024-05-14 03:55:28.061819 seg_tgce-0.1.2/seg_tgce/data/oxford_pet/oxford_pet.py
+-rw-r--r--   0        0        0     2228 2024-05-14 03:55:28.058486 seg_tgce-0.1.2/seg_tgce/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/experiments/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/experiments/apr_14_2024/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-06 05:22:24.575116 seg_tgce-0.1.2/seg_tgce/experiments/apr_14_2024/experiment.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/loss/__init__.py
+-rw-r--r--   0        0        0     3290 2024-05-06 04:49:42.271689 seg_tgce-0.1.2/seg_tgce/loss/tgce.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/metrics/__init__.py
+-rw-r--r--   0        0        0     1225 2024-05-06 05:24:38.627838 seg_tgce-0.1.2/seg_tgce/metrics/dice_coefficient.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/models/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-06 05:22:57.754965 seg_tgce-0.1.2/seg_tgce/models/ma_model.py
+-rw-r--r--   0        0        0     4618 2024-05-06 05:10:53.688560 seg_tgce-0.1.2/seg_tgce/models/unet.py
+-rw-r--r--   0        0        0        0 2024-04-30 04:42:11.177868 seg_tgce-0.1.2/seg_tgce/py.typed
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/run/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 04:39:26.044844 seg_tgce-0.1.2/seg_tgce/run/oxford_ma_runner/__init__.py
+-rw-r--r--   0        0        0      414 2024-05-06 05:13:40.777698 seg_tgce-0.1.2/seg_tgce/run/oxford_ma_runner/model_result.py
+-rw-r--r--   0        0        0     2468 2024-05-06 05:24:38.624505 seg_tgce-0.1.2/seg_tgce/run/oxford_ma_runner/plotting.py
+-rw-r--r--   0        0        0     7072 2024-05-07 11:10:44.874873 seg_tgce-0.1.2/seg_tgce/run/oxford_ma_runner/runner.py
+-rw-r--r--   0        0        0      800 2024-04-16 19:11:40.745930 seg_tgce-0.1.2/seg_tgce/run/runner.py
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 seg_tgce-0.1.2/PKG-INFO
```

### Comparing `seg_tgce-0.1.1/pyproject.toml` & `seg_tgce-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 description = "Framework for handling image segmentation in the context of multiple annotators"
 name = "seg_tgce"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 authors = [{ name = "Brandon Lotero", email = "blotero@gmail.com" }]
 maintainers = [{ name = "Brandon Lotero", email = "blotero@gmail.com" }]
 license = { file = "../LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/blotero/seg_tgce"
 Documentation = "https://seg-tgce.readthedocs.io/en/latest/"
 Repository = "https://github.com/blotero/seg_tgce"
 Issues = "https://github.com/blotero/seg_tgce/issues"
 
 [tool.poetry]
 name = "seg_tgce"
-version = "0.1.1"
+version = "0.1.2"
 authors = ["Brandon Lotero <blotero@gmail.com>"]
 description = "A package for the SEG TGCE project"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
```

### Comparing `seg_tgce-0.1.1/seg_tgce/data/crowd_seg/generator.py` & `seg_tgce-0.1.2/seg_tgce/data/crowd_seg/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 import logging
 import os
-from typing import List, Tuple
+from typing import List, Optional, Tuple, TypedDict
 
 import numpy as np
 from keras.preprocessing.image import img_to_array, load_img
 from keras.utils import Sequence
 from matplotlib import pyplot as plt
 
+from .retrieve import fetch_data, get_masks_dir, get_patches_dir
+from .stage import Stage
+
 LOGGER = logging.getLogger(__name__)
 logging.basicConfig(level=logging.WARNING)
 
 
+class CustomPath(TypedDict):
+    image_dir: str
+    mask_dir: str
+
+
 class ImageDataGenerator(Sequence):  # pylint: disable=too-many-instance-attributes
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        image_dir: str,
-        mask_dir: str,
         n_classes: int,
         image_size: Tuple[int, int] = (256, 256),
         batch_size: int = 32,
         shuffle: bool = True,
+        stage: Stage = Stage.TRAIN,
+        paths: Optional[CustomPath] = None,
     ):
+        if paths is not None:
+            image_dir = paths["image_dir"]
+            mask_dir = paths["mask_dir"]
+        else:
+            fetch_data()
+            image_dir = get_patches_dir(stage)
+            mask_dir = get_masks_dir(stage)
         self.image_dir = image_dir
         self.mask_dir = mask_dir
         self.image_size = image_size
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.image_filenames = sorted(
             [
                 filename
                 for filename in os.listdir(image_dir)
                 if filename.endswith(".png")
             ]
         )
         self.n_scorers = len(os.listdir(mask_dir))
         self.scorers_tags = sorted(os.listdir(mask_dir))
-        print(f"Scorer tags: {self.scorers_tags}")
+        LOGGER.info("Scorer tags: %s", self.scorers_tags)
         self.n_classes = n_classes
         self.on_epoch_end()
 
     def __len__(self):
         return int(np.ceil(len(self.image_filenames) / self.batch_size))
 
     def __getitem__(self, index):
@@ -117,24 +132,7 @@
 
             image = load_img(img_path, target_size=self.image_size)
             image = img_to_array(image)
 
             images[batch] = image
 
         return images, masks
-
-
-if __name__ == "__main__":
-    val_gen = ImageDataGenerator(
-        image_dir="/home/brandon/unal/maestria/datasets/Histology Data/patches/Val",
-        mask_dir="/home/brandon/unal/maestria/datasets/Histology Data/masks/Val",
-        batch_size=16,
-        n_classes=6,
-    )
-    print(f"Train len: {len(val_gen)}")
-    print(f"Train masks scorers: {val_gen.n_scorers}")
-    print(f"Train masks scorers tags: {val_gen.scorers_tags}")
-    val_gen.visualize_sample(
-        batch_index=8,
-        sample_index=8,
-        scorers=["NP8", "NP16", "NP21", "expert"],
-    )
```

### Comparing `seg_tgce-0.1.1/seg_tgce/data/crowd_seg/visualizer.py` & `seg_tgce-0.1.2/seg_tgce/data/crowd_seg/visualizer.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/data/oxford_pet/disturbance/model.py` & `seg_tgce-0.1.2/seg_tgce/data/oxford_pet/disturbance/model.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/data/oxford_pet/oxford_iiit_pet.py` & `seg_tgce-0.1.2/seg_tgce/data/oxford_pet/oxford_iiit_pet.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/data/oxford_pet/oxford_pet.py` & `seg_tgce-0.1.2/seg_tgce/data/oxford_pet/oxford_pet.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/data/utils.py` & `seg_tgce-0.1.2/seg_tgce/data/utils.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/experiments/apr_14_2024/experiment.py` & `seg_tgce-0.1.2/seg_tgce/experiments/apr_14_2024/experiment.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/loss/tgce.py` & `seg_tgce-0.1.2/seg_tgce/loss/tgce.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/metrics/dice_coefficient.py` & `seg_tgce-0.1.2/seg_tgce/metrics/dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/models/ma_model.py` & `seg_tgce-0.1.2/seg_tgce/models/ma_model.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/models/unet.py` & `seg_tgce-0.1.2/seg_tgce/models/unet.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/run/oxford_ma_runner/plotting.py` & `seg_tgce-0.1.2/seg_tgce/run/oxford_ma_runner/plotting.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/run/oxford_ma_runner/runner.py` & `seg_tgce-0.1.2/seg_tgce/run/oxford_ma_runner/runner.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/seg_tgce/run/runner.py` & `seg_tgce-0.1.2/seg_tgce/run/runner.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.1/PKG-INFO` & `seg_tgce-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seg_tgce
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for the SEG TGCE project
 Home-page: https://github.com/blotero/seg_tgce
 Author: Brandon Lotero
 Author-email: blotero@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


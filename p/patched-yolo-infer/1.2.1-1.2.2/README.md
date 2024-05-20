# Comparing `tmp/patched_yolo_infer-1.2.1.tar.gz` & `tmp/patched_yolo_infer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patched_yolo_infer-1.2.1.tar", last modified: Sun May 19 20:57:40 2024, max compression
+gzip compressed data, was "patched_yolo_infer-1.2.2.tar", last modified: Mon May 20 21:10:58 2024, max compression
```

## Comparing `patched_yolo_infer-1.2.1.tar` & `patched_yolo_infer-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 20:57:40.475005 patched_yolo_infer-1.2.1/
--rw-rw-rw-   0        0        0    35184 2024-03-29 07:50:02.000000 patched_yolo_infer-1.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0    12850 2024-05-19 20:57:40.475005 patched_yolo_infer-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    17797 2024-05-19 20:12:36.000000 patched_yolo_infer-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 20:57:40.450206 patched_yolo_infer-1.2.1/patched_yolo_infer/
--rw-rw-rw-   0        0        0      262 2024-03-14 20:52:00.000000 patched_yolo_infer-1.2.1/patched_yolo_infer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 20:57:40.475005 patched_yolo_infer-1.2.1/patched_yolo_infer/elements/
--rw-rw-rw-   0        0        0     6841 2024-05-19 16:18:07.000000 patched_yolo_infer-1.2.1/patched_yolo_infer/elements/CropElement.py
--rw-rw-rw-   0        0        0        0 2024-03-14 21:13:30.000000 patched_yolo_infer-1.2.1/patched_yolo_infer/elements/__init__.py
--rw-rw-rw-   0        0        0    16850 2024-05-19 14:49:58.000000 patched_yolo_infer-1.2.1/patched_yolo_infer/functions_extra.py
-drwxrwxrwx   0        0        0        0 2024-05-19 20:57:40.475005 patched_yolo_infer-1.2.1/patched_yolo_infer/nodes/
--rw-rw-rw-   0        0        0    13547 2024-05-19 17:57:19.000000 patched_yolo_infer-1.2.1/patched_yolo_infer/nodes/CombineDetections.py
--rw-rw-rw-   0        0        0     8716 2024-05-19 17:59:53.000000 patched_yolo_infer-1.2.1/patched_yolo_infer/nodes/MakeCropsDetectThem.py
--rw-rw-rw-   0        0        0        0 2024-03-14 21:13:13.000000 patched_yolo_infer-1.2.1/patched_yolo_infer/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 20:57:40.473175 patched_yolo_infer-1.2.1/patched_yolo_infer.egg-info/
--rw-rw-rw-   0        0        0    12850 2024-05-19 20:57:40.000000 patched_yolo_infer-1.2.1/patched_yolo_infer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-05-19 20:57:40.000000 patched_yolo_infer-1.2.1/patched_yolo_infer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 20:57:40.000000 patched_yolo_infer-1.2.1/patched_yolo_infer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-19 20:57:40.000000 patched_yolo_infer-1.2.1/patched_yolo_infer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-19 20:57:40.000000 patched_yolo_infer-1.2.1/patched_yolo_infer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 20:57:40.480365 patched_yolo_infer-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1695 2024-05-19 20:54:32.000000 patched_yolo_infer-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:10:58.915745 patched_yolo_infer-1.2.2/
+-rw-rw-rw-   0        0        0    35184 2024-03-29 07:50:02.000000 patched_yolo_infer-1.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    12850 2024-05-20 21:10:58.914740 patched_yolo_infer-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17797 2024-05-19 21:30:31.000000 patched_yolo_infer-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 21:10:58.887990 patched_yolo_infer-1.2.2/patched_yolo_infer/
+-rw-rw-rw-   0        0        0      262 2024-03-14 20:52:00.000000 patched_yolo_infer-1.2.2/patched_yolo_infer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:10:58.912515 patched_yolo_infer-1.2.2/patched_yolo_infer/elements/
+-rw-rw-rw-   0        0        0     6841 2024-05-19 21:30:31.000000 patched_yolo_infer-1.2.2/patched_yolo_infer/elements/CropElement.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 21:13:30.000000 patched_yolo_infer-1.2.2/patched_yolo_infer/elements/__init__.py
+-rw-rw-rw-   0        0        0    16848 2024-05-20 21:08:43.000000 patched_yolo_infer-1.2.2/patched_yolo_infer/functions_extra.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:10:58.914740 patched_yolo_infer-1.2.2/patched_yolo_infer/nodes/
+-rw-rw-rw-   0        0        0    13547 2024-05-19 21:30:31.000000 patched_yolo_infer-1.2.2/patched_yolo_infer/nodes/CombineDetections.py
+-rw-rw-rw-   0        0        0     8716 2024-05-19 21:30:31.000000 patched_yolo_infer-1.2.2/patched_yolo_infer/nodes/MakeCropsDetectThem.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 21:13:13.000000 patched_yolo_infer-1.2.2/patched_yolo_infer/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 21:10:58.910514 patched_yolo_infer-1.2.2/patched_yolo_infer.egg-info/
+-rw-rw-rw-   0        0        0    12850 2024-05-20 21:10:58.000000 patched_yolo_infer-1.2.2/patched_yolo_infer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-05-20 21:10:58.000000 patched_yolo_infer-1.2.2/patched_yolo_infer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 21:10:58.000000 patched_yolo_infer-1.2.2/patched_yolo_infer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-20 21:10:58.000000 patched_yolo_infer-1.2.2/patched_yolo_infer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-20 21:10:58.000000 patched_yolo_infer-1.2.2/patched_yolo_infer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 21:10:58.916457 patched_yolo_infer-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1695 2024-05-20 21:09:06.000000 patched_yolo_infer-1.2.2/setup.py
```

### Comparing `patched_yolo_infer-1.2.1/LICENSE.txt` & `patched_yolo_infer-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.2.1/PKG-INFO` & `patched_yolo_infer-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patched_yolo_infer
-Version: 1.2.1
+Version: 1.2.2
 Summary: YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.
 Home-page: https://github.com/Koldim2001/YOLO-Patch-Based-Inference
 Author: Koldim2001
 License: AGPL-3.0 license
 Keywords: python,yolov8,yolov9,rtdetr,sam,object detection,instance segmentation,patch-based inference,small object detection,yolov8-seg,image patching,yolo visualization,slice-based inference,slicing inference,inference visualization,patchify,ultralytics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `patched_yolo_infer-1.2.1/README.md` & `patched_yolo_infer-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.2.1/patched_yolo_infer/elements/CropElement.py` & `patched_yolo_infer-1.2.2/patched_yolo_infer/elements/CropElement.py`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.2.1/patched_yolo_infer/functions_extra.py` & `patched_yolo_infer-1.2.2/patched_yolo_infer/functions_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,28 +357,27 @@
             if fill_mask:
                 if alpha == 1:
                     cv2.fillPoly(labeled_image, pts=mask_contours, color=color)
                 else:
                     color_mask = np.zeros_like(img)
                     color_mask[mask_resized > 0] = color
                     labeled_image = cv2.addWeighted(labeled_image, 1, color_mask, alpha, 0)
-
             cv2.drawContours(labeled_image, mask_contours, -1, color, thickness)
         
         elif segment and len(polygons) > 0:
             if len(polygons[i]) > 0:
                 points = np.array(polygons[i].reshape((-1, 1, 2)), dtype=np.int32)
-                cv2.drawContours(labeled_image, [points], -1, color, thickness)
                 if fill_mask:
                     if alpha == 1:
                         cv2.fillPoly(labeled_image, pts=[points], color=color)
                     else:
                         mask_from_poly = np.zeros_like(img)
                         color_mask_from_poly = cv2.fillPoly(mask_from_poly, pts=[points], color=color)
                         labeled_image = cv2.addWeighted(labeled_image, 1, color_mask_from_poly, alpha, 0)
+                cv2.drawContours(labeled_image, [points], -1, color, thickness)
 
         # Write class label
         if show_boxes:
             cv2.rectangle(labeled_image, (x_min, y_min), (x_max, y_max), color, thickness)
 
         if show_class:
             if show_confidences:
```

### Comparing `patched_yolo_infer-1.2.1/patched_yolo_infer/nodes/CombineDetections.py` & `patched_yolo_infer-1.2.2/patched_yolo_infer/nodes/CombineDetections.py`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.2.1/patched_yolo_infer/nodes/MakeCropsDetectThem.py` & `patched_yolo_infer-1.2.2/patched_yolo_infer/nodes/MakeCropsDetectThem.py`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.2.1/patched_yolo_infer.egg-info/PKG-INFO` & `patched_yolo_infer-1.2.2/patched_yolo_infer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patched-yolo-infer
-Version: 1.2.1
+Version: 1.2.2
 Summary: YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.
 Home-page: https://github.com/Koldim2001/YOLO-Patch-Based-Inference
 Author: Koldim2001
 License: AGPL-3.0 license
 Keywords: python,yolov8,yolov9,rtdetr,sam,object detection,instance segmentation,patch-based inference,small object detection,yolov8-seg,image patching,yolo visualization,slice-based inference,slicing inference,inference visualization,patchify,ultralytics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `patched_yolo_infer-1.2.1/patched_yolo_infer.egg-info/SOURCES.txt` & `patched_yolo_infer-1.2.2/patched_yolo_infer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.2.1/setup.py` & `patched_yolo_infer-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 pwd = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(pwd, "patched_yolo_infer/README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.2.1'
+VERSION = '1.2.2'
 DESCRIPTION = '''YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.'''
 
 setup(
     name="patched_yolo_infer",
     version=VERSION,
     license="AGPL-3.0 license",
     url="https://github.com/Koldim2001/YOLO-Patch-Based-Inference",
```


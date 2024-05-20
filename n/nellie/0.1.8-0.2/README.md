# Comparing `tmp/nellie-0.1.8.tar.gz` & `tmp/nellie-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nellie-0.1.8.tar", last modified: Fri Apr 26 16:18:29 2024, max compression
+gzip compressed data, was "nellie-0.2.tar", last modified: Mon May 20 18:20:04 2024, max compression
```

## Comparing `nellie-0.1.8.tar` & `nellie-0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.351884 nellie-0.1.8/
--rw-r--r--   0 austin     (501) staff       (20)    18826 2024-03-19 19:14:37.000000 nellie-0.1.8/LICENSE
--rw-r--r--   0 austin     (501) staff       (20)    11217 2024-04-26 16:18:29.351703 nellie-0.1.8/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)    10555 2024-03-23 00:41:03.000000 nellie-0.1.8/README.md
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.340877 nellie-0.1.8/nellie/
--rw-r--r--   0 austin     (501) staff       (20)     1421 2024-03-15 22:18:53.000000 nellie-0.1.8/nellie/__init__.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.341939 nellie-0.1.8/nellie/feature_extraction/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/feature_extraction/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    54414 2024-04-01 21:48:11.000000 nellie-0.1.8/nellie/feature_extraction/hierarchical.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.342222 nellie-0.1.8/nellie/im_info/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/im_info/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    16203 2024-04-01 22:05:10.000000 nellie-0.1.8/nellie/im_info/im_info.py
--rw-r--r--   0 austin     (501) staff       (20)     1774 2024-04-26 16:15:57.000000 nellie-0.1.8/nellie/run.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.343223 nellie-0.1.8/nellie/segmentation/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/segmentation/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    11578 2024-04-26 16:12:16.000000 nellie-0.1.8/nellie/segmentation/filtering.py
--rw-r--r--   0 austin     (501) staff       (20)     6525 2024-04-26 16:17:35.000000 nellie-0.1.8/nellie/segmentation/labelling.py
--rw-r--r--   0 austin     (501) staff       (20)     9769 2024-04-01 17:29:51.000000 nellie-0.1.8/nellie/segmentation/mocap_marking.py
--rw-r--r--   0 austin     (501) staff       (20)    16823 2024-03-15 22:18:53.000000 nellie-0.1.8/nellie/segmentation/networking.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.344311 nellie-0.1.8/nellie/tracking/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/tracking/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     4743 2024-04-12 20:45:28.000000 nellie-0.1.8/nellie/tracking/all_tracks_for_label.py
--rw-r--r--   0 austin     (501) staff       (20)    11441 2024-04-26 16:12:16.000000 nellie-0.1.8/nellie/tracking/flow_interpolation.py
--rw-r--r--   0 austin     (501) staff       (20)    17974 2024-04-26 16:12:16.000000 nellie-0.1.8/nellie/tracking/hu_tracking.py
--rw-r--r--   0 austin     (501) staff       (20)    19639 2024-04-26 16:12:16.000000 nellie-0.1.8/nellie/tracking/voxel_reassignment.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.345369 nellie-0.1.8/nellie/utils/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/utils/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)      275 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/utils/base_logger.py
--rw-r--r--   0 austin     (501) staff       (20)     1572 2024-04-01 21:26:56.000000 nellie-0.1.8/nellie/utils/general.py
--rw-r--r--   0 austin     (501) staff       (20)     2594 2024-03-15 22:18:53.000000 nellie-0.1.8/nellie/utils/gpu_functions.py
--rw-r--r--   0 austin     (501) staff       (20)     5892 2024-03-15 22:13:16.000000 nellie-0.1.8/nellie/utils/torch_xp.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.351389 nellie-0.1.8/nellie.egg-info/
--rw-r--r--   0 austin     (501) staff       (20)    11217 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)     1253 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/SOURCES.txt
--rw-r--r--   0 austin     (501) staff       (20)        1 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/dependency_links.txt
--rw-r--r--   0 austin     (501) staff       (20)       53 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/entry_points.txt
--rw-r--r--   0 austin     (501) staff       (20)      127 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/requires.txt
--rw-r--r--   0 austin     (501) staff       (20)       27 2024-04-26 16:18:29.000000 nellie-0.1.8/nellie.egg-info/top_level.txt
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.348394 nellie-0.1.8/nellie_napari/
--rw-r--r--   0 austin     (501) staff       (20)      112 2024-03-18 21:13:24.000000 nellie-0.1.8/nellie_napari/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     8386 2024-03-19 15:37:36.000000 nellie-0.1.8/nellie_napari/batch_mode.py
--rw-r--r--   0 austin     (501) staff       (20)     3595 2024-03-23 00:44:38.000000 nellie-0.1.8/nellie_napari/home.py
--rw-r--r--   0 austin     (501) staff       (20)    89016 2024-03-19 16:27:20.000000 nellie-0.1.8/nellie_napari/logo.png
--rw-r--r--   0 austin     (501) staff       (20)      218 2024-03-15 22:32:30.000000 nellie-0.1.8/nellie_napari/napari.yaml
--rw-r--r--   0 austin     (501) staff       (20)    20913 2024-03-19 21:11:06.000000 nellie-0.1.8/nellie_napari/nellie_analysis.py
--rw-r--r--   0 austin     (501) staff       (20)    16190 2024-03-19 18:53:00.000000 nellie-0.1.8/nellie_napari/nellie_fileselect.py
--rw-r--r--   0 austin     (501) staff       (20)     2719 2024-03-19 01:57:46.000000 nellie-0.1.8/nellie_napari/nellie_loader.py
--rw-r--r--   0 austin     (501) staff       (20)    15621 2024-04-01 16:16:45.000000 nellie-0.1.8/nellie_napari/nellie_processor.py
--rw-r--r--   0 austin     (501) staff       (20)    12833 2024-03-19 16:50:50.000000 nellie-0.1.8/nellie_napari/visualizer.py
--rw-r--r--   0 austin     (501) staff       (20)       90 2024-01-23 18:46:05.000000 nellie-0.1.8/pyproject.toml
--rw-r--r--   0 austin     (501) staff       (20)      822 2024-04-26 16:18:29.352696 nellie-0.1.8/setup.cfg
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.348703 nellie-0.1.8/tests/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/tests/__init__.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-26 16:18:29.349336 nellie-0.1.8/tests/unit/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.8/tests/unit/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)        6 2024-03-15 22:13:16.000000 nellie-0.1.8/tests/unit/test_frangi_filter.py
--rw-r--r--   0 austin     (501) staff       (20)     3310 2024-03-15 22:18:53.000000 nellie-0.1.8/tests/unit/test_im_info.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.849929 nellie-0.2/
+-rw-r--r--   0 austin     (501) staff       (20)    18826 2024-03-19 19:14:37.000000 nellie-0.2/LICENSE
+-rw-r--r--   0 austin     (501) staff       (20)    11215 2024-05-20 18:20:04.849802 nellie-0.2/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)    10555 2024-03-23 00:41:03.000000 nellie-0.2/README.md
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.839257 nellie-0.2/nellie/
+-rw-r--r--   0 austin     (501) staff       (20)     1421 2024-03-15 22:18:53.000000 nellie-0.2/nellie/__init__.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.840349 nellie-0.2/nellie/feature_extraction/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.2/nellie/feature_extraction/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    54414 2024-04-01 21:48:11.000000 nellie-0.2/nellie/feature_extraction/hierarchical.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.841182 nellie-0.2/nellie/im_info/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.2/nellie/im_info/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    16203 2024-04-01 22:05:10.000000 nellie-0.2/nellie/im_info/im_info.py
+-rw-r--r--   0 austin     (501) staff       (20)     2470 2024-05-20 18:18:26.000000 nellie-0.2/nellie/run.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.842316 nellie-0.2/nellie/segmentation/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.2/nellie/segmentation/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    11589 2024-05-20 18:18:26.000000 nellie-0.2/nellie/segmentation/filtering.py
+-rw-r--r--   0 austin     (501) staff       (20)     6791 2024-05-20 18:18:26.000000 nellie-0.2/nellie/segmentation/labelling.py
+-rw-r--r--   0 austin     (501) staff       (20)     9769 2024-04-01 17:29:51.000000 nellie-0.2/nellie/segmentation/mocap_marking.py
+-rw-r--r--   0 austin     (501) staff       (20)    16842 2024-05-20 18:18:26.000000 nellie-0.2/nellie/segmentation/networking.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.843345 nellie-0.2/nellie/tracking/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.2/nellie/tracking/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     4743 2024-04-12 20:45:28.000000 nellie-0.2/nellie/tracking/all_tracks_for_label.py
+-rw-r--r--   0 austin     (501) staff       (20)    11534 2024-05-20 18:18:26.000000 nellie-0.2/nellie/tracking/flow_interpolation.py
+-rw-r--r--   0 austin     (501) staff       (20)    18071 2024-05-20 18:18:26.000000 nellie-0.2/nellie/tracking/hu_tracking.py
+-rw-r--r--   0 austin     (501) staff       (20)    19712 2024-05-20 18:18:26.000000 nellie-0.2/nellie/tracking/voxel_reassignment.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.844529 nellie-0.2/nellie/utils/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.2/nellie/utils/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)      275 2024-03-15 22:13:16.000000 nellie-0.2/nellie/utils/base_logger.py
+-rw-r--r--   0 austin     (501) staff       (20)     1572 2024-04-01 21:26:56.000000 nellie-0.2/nellie/utils/general.py
+-rw-r--r--   0 austin     (501) staff       (20)     2594 2024-03-15 22:18:53.000000 nellie-0.2/nellie/utils/gpu_functions.py
+-rw-r--r--   0 austin     (501) staff       (20)     5892 2024-03-15 22:13:16.000000 nellie-0.2/nellie/utils/torch_xp.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.849507 nellie-0.2/nellie.egg-info/
+-rw-r--r--   0 austin     (501) staff       (20)    11215 2024-05-20 18:20:04.000000 nellie-0.2/nellie.egg-info/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)     1253 2024-05-20 18:20:04.000000 nellie-0.2/nellie.egg-info/SOURCES.txt
+-rw-r--r--   0 austin     (501) staff       (20)        1 2024-05-20 18:20:04.000000 nellie-0.2/nellie.egg-info/dependency_links.txt
+-rw-r--r--   0 austin     (501) staff       (20)       53 2024-05-20 18:20:04.000000 nellie-0.2/nellie.egg-info/entry_points.txt
+-rw-r--r--   0 austin     (501) staff       (20)      127 2024-05-20 18:20:04.000000 nellie-0.2/nellie.egg-info/requires.txt
+-rw-r--r--   0 austin     (501) staff       (20)       27 2024-05-20 18:20:04.000000 nellie-0.2/nellie.egg-info/top_level.txt
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.847890 nellie-0.2/nellie_napari/
+-rw-r--r--   0 austin     (501) staff       (20)      112 2024-03-18 21:13:24.000000 nellie-0.2/nellie_napari/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     8386 2024-03-19 15:37:36.000000 nellie-0.2/nellie_napari/batch_mode.py
+-rw-r--r--   0 austin     (501) staff       (20)     3595 2024-03-23 00:44:38.000000 nellie-0.2/nellie_napari/home.py
+-rw-r--r--   0 austin     (501) staff       (20)    89016 2024-03-19 16:27:20.000000 nellie-0.2/nellie_napari/logo.png
+-rw-r--r--   0 austin     (501) staff       (20)      218 2024-03-15 22:32:30.000000 nellie-0.2/nellie_napari/napari.yaml
+-rw-r--r--   0 austin     (501) staff       (20)    20913 2024-03-19 21:11:06.000000 nellie-0.2/nellie_napari/nellie_analysis.py
+-rw-r--r--   0 austin     (501) staff       (20)    16190 2024-03-19 18:53:00.000000 nellie-0.2/nellie_napari/nellie_fileselect.py
+-rw-r--r--   0 austin     (501) staff       (20)     2719 2024-03-19 01:57:46.000000 nellie-0.2/nellie_napari/nellie_loader.py
+-rw-r--r--   0 austin     (501) staff       (20)    15621 2024-04-01 16:16:45.000000 nellie-0.2/nellie_napari/nellie_processor.py
+-rw-r--r--   0 austin     (501) staff       (20)    12833 2024-03-19 16:50:50.000000 nellie-0.2/nellie_napari/visualizer.py
+-rw-r--r--   0 austin     (501) staff       (20)       90 2024-01-23 18:46:05.000000 nellie-0.2/pyproject.toml
+-rw-r--r--   0 austin     (501) staff       (20)      820 2024-05-20 18:20:04.850218 nellie-0.2/setup.cfg
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.848209 nellie-0.2/tests/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.2/tests/__init__.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-05-20 18:20:04.848774 nellie-0.2/tests/unit/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.2/tests/unit/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)        6 2024-03-15 22:13:16.000000 nellie-0.2/tests/unit/test_frangi_filter.py
+-rw-r--r--   0 austin     (501) staff       (20)     3310 2024-03-15 22:18:53.000000 nellie-0.2/tests/unit/test_im_info.py
```

### Comparing `nellie-0.1.8/LICENSE` & `nellie-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/PKG-INFO` & `nellie-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nellie
-Version: 0.1.8
+Version: 0.2
 Summary: Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 Home-page: https://github.com/aelefebv/nellie
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre+nellie@gmail.com
 Classifier: Framework :: napari
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `nellie-0.1.8/README.md` & `nellie-0.2/README.md`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie/__init__.py` & `nellie-0.2/nellie/__init__.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie/feature_extraction/hierarchical.py` & `nellie-0.2/nellie/feature_extraction/hierarchical.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie/im_info/im_info.py` & `nellie-0.2/nellie/im_info/im_info.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie/run.py` & `nellie-0.2/nellie/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,22 +33,33 @@
     hierarchy.run()
 
     return im_info
 
 
 if __name__ == "__main__":
     # Single file run
-    im_path = r"/Users/austin/Downloads/test.tif"
-    im_info = run(im_path, remove_edges=False, ch=0)
+    # im_path = r"/Users/austin/Downloads/test.tif"
+    # im_path = r"/Users/austin/GitHub/nellie-simulations/motion/fission_fusion/outputs/fusion-std_fusion-std_512-t_0p5.ome.tif"
+    # im_info = run(im_path, remove_edges=False, ch=0)
 
-    # # Directory bactch run
-    # import os
-    # top_dir = r"D:\test_files\nellie_longer_smorgasbord"
-    # ch = 0
-    # num_t = None
-    # # get all non-folder files
-    # all_files = os.listdir(top_dir)
-    # all_files = [os.path.join(top_dir, file) for file in all_files if not os.path.isdir(os.path.join(top_dir, file))]
-    # for file_num, tif_file in enumerate(all_files):
-    #     # for ch in range(1):
-    #     print(f'Processing file {file_num + 1} of {len(all_files)}, channel {ch + 1} of 1')
-    #     im_info = run(tif_file, remove_edges=True, ch=ch, num_t=num_t)
+    # Directory bactch run
+    import os
+    top_dirs = [
+        r"C:\Users\austin\GitHub\nellie-supplemental\comparisons\simulations\multi_grid\outputs",
+        r"C:\Users\austin\GitHub\nellie-supplemental\comparisons\simulations\separation\outputs",
+        r"C:\Users\austin\GitHub\nellie-supplemental\comparisons\simulations\px_sizes\outputs",
+        ]
+    ch = 0
+    num_t = 1
+    # get all non-folder files
+    for top_dir in top_dirs:
+        all_files = os.listdir(top_dir)
+        all_files = [os.path.join(top_dir, file) for file in all_files if not os.path.isdir(os.path.join(top_dir, file))]
+        all_files = [file for file in all_files if file.endswith('.tif')]
+        for file_num, tif_file in enumerate(all_files):
+            # for ch in range(1):
+            print(f'Processing file {file_num + 1} of {len(all_files)}, channel {ch + 1} of 1')
+            im_info = ImInfo(tif_file, ch=ch)
+            if os.path.exists(im_info.pipeline_paths['im_skel_relabelled']):
+                print(f'Already exists, skipping.')
+                continue
+            im_info = run(tif_file, remove_edges=False, ch=ch, num_t=num_t)
```

### Comparing `nellie-0.1.8/nellie/segmentation/filtering.py` & `nellie-0.2/nellie/segmentation/filtering.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,21 +122,24 @@
                 np.concatenate([hxy, hyy, hyz], axis=-1),
                 np.concatenate([hxz, hyz, hzz], axis=-1)
             ], axis=-2)
 
         return h_mask, hessian_matrices
 
     def _get_frob_mask(self, hessian_matrices):
-        # todo, can we avoid rescaling? slowing down..
         rescaled_hessian = hessian_matrices / xp.max(xp.abs(hessian_matrices))
         frobenius_norm = xp.linalg.norm(rescaled_hessian, axis=0)
-        frobenius_norm[xp.isinf(frobenius_norm)] = 0
-        frob_triangle_thresh = triangle_threshold(frobenius_norm[frobenius_norm > 0])
-        frob_otsu_thresh, _ = otsu_threshold(frobenius_norm[frobenius_norm > 0])
-        frobenius_threshold = min(frob_triangle_thresh, frob_otsu_thresh)
+        frobenius_norm[xp.isinf(frobenius_norm)] = xp.max(frobenius_norm[~xp.isinf(frobenius_norm)])
+        non_zero_frobenius = frobenius_norm[frobenius_norm > 0]
+        if len(non_zero_frobenius) == 0:
+            frobenius_threshold = 0
+        else:
+            frob_triangle_thresh = triangle_threshold(non_zero_frobenius)
+            frob_otsu_thresh, _ = otsu_threshold(non_zero_frobenius)
+            frobenius_threshold = min(frob_triangle_thresh, frob_otsu_thresh)
         mask = frobenius_norm > frobenius_threshold
         return mask
 
     def _compute_chunkwise_eigenvalues(self, hessian_matrices, chunk_size=1E6):
         chunk_size = int(chunk_size)
         total_voxels = len(hessian_matrices)
 
@@ -197,14 +200,16 @@
         for sigma_num, sigma in enumerate(self.sigmas):
             gauss_volume = self._gauss_filter(sigma, t)  # * xp.mean(sigma) ** 2
 
             gamma = self._calculate_gamma(gauss_volume)
             gamma_sq = 2 * gamma ** 2
 
             h_mask, hessian_matrices = self._compute_hessian(gauss_volume, mask=mask)
+            if len(hessian_matrices) == 0:
+                continue
             eigenvalues = self._compute_chunkwise_eigenvalues(hessian_matrices.astype('float'))
 
             temp[h_mask] = self._filter_hessian(eigenvalues, gamma_sq=gamma_sq)
 
             max_indices = temp > vesselness
             vesselness[max_indices] = temp[max_indices]
             masks = xp.where(~h_mask, 0, masks)
@@ -232,26 +237,22 @@
             frangi_frame[z_idx, rmin:rmin + 15, ...] = 0
             frangi_frame[z_idx, rmax - 15:rmax + 1, ...] = 0
         return frangi_frame
 
     def _run_filter(self, mask=True):
         for t in range(self.num_t):
             frangi_frame = self._run_frame(t, mask=mask)
-            frangi_frame = self._mask_volume(frangi_frame)
-            if not self.im_info.no_z:  # helps with z anisotropy
-                log_frame = self._filter_log(frangi_frame, frangi_frame > 0)
-                log_frame[log_frame < 0] = 0
-                filtered_im = log_frame
-            else:
-                filtered_im = frangi_frame
+            if not xp.sum(frangi_frame):
+                frangi_frame = self._mask_volume(frangi_frame)
+            filtered_im = frangi_frame
 
             if device_type == 'cuda':
                 filtered_im = filtered_im.get()
 
-            if self.im_info.no_t:
+            if self.im_info.no_t or self.num_t == 1:
                 self.frangi_memmap[:] = filtered_im[:]
             else:
                 self.frangi_memmap[t, ...] = filtered_im
             self.frangi_memmap.flush()
 
     def run(self, mask=True):
         logger.info('Running frangi filter.')
```

### Comparing `nellie-0.1.8/nellie/segmentation/labelling.py` & `nellie-0.2/nellie/segmentation/labelling.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 
         if not self.im_info.no_z and self.im_info.dim_sizes['Z'] < self.min_z_radius_um:
             mask = ndi.binary_opening(mask, structure=xp.ones((2, 2, 2)))
         elif self.im_info.no_z:
             mask = ndi.binary_opening(mask, structure=xp.ones((2, 2)))
 
         labels, _ = ndi.label(mask, structure=footprint)
+        # remove anything 4 pixels or under using bincounts
+        areas = xp.bincount(labels.ravel())[1:]
+        mask = xp.where(xp.isin(labels, xp.where(areas > 4)[0]+1), labels, 0) > 0
+        labels, _ = ndi.label(mask, structure=footprint)
         return mask, labels
 
     def _get_subtraction_mask(self, original_frame, labels_frame):
         subtraction_mask = original_frame.copy()
         subtraction_mask[labels_frame > 0] = 0
         return subtraction_mask
 
@@ -129,15 +133,15 @@
         return labels
 
     def _run_segmentation(self):
         for t in range(self.num_t):
             labels = self._run_frame(t)
             if device_type == 'cuda':
                 labels = labels.get()
-            if self.im_info.no_t:
+            if self.im_info.no_t or self.num_t == 1:
                 self.instance_label_memmap[:] = labels[:]
             else:
                 self.instance_label_memmap[t, ...] = labels
 
             self.instance_label_memmap.flush()
 
     def run(self):
```

### Comparing `nellie-0.1.8/nellie/segmentation/mocap_marking.py` & `nellie-0.2/nellie/segmentation/mocap_marking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie/segmentation/networking.py` & `nellie-0.2/nellie/segmentation/networking.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
             junction_coords.pop(nearest_junction_indices)
             pixel_class[tuple(np.array(junction_coords).T)] = 3
         return pixel_class
 
     def _run_networking(self):
         for t in range(self.num_t):
             skel, pixel_class, skel_relabelled_memmap = self._run_frame(t)
-            if self.im_info.no_t:
+            if self.im_info.no_t or self.num_t == 1:
                 if device_type == 'cuda':
                     self.skel_memmap[:] = skel[:].get()
                     self.pixel_class_memmap[:] = pixel_class[:].get()
                     self.skel_relabelled_memmap[:] = skel_relabelled_memmap[:].get()
                 else:
                     self.skel_memmap[:] = skel[:]
                     self.pixel_class_memmap[:] = pixel_class[:]
```

### Comparing `nellie-0.1.8/nellie/tracking/all_tracks_for_label.py` & `nellie-0.2/nellie/tracking/all_tracks_for_label.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie/tracking/flow_interpolation.py` & `nellie-0.2/nellie/tracking/flow_interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,17 @@
             self.num_t = im_info.shape[im_info.axes.index('T')]
 
         if self.im_info.no_z:
             self.scaling = (im_info.dim_sizes['Y'], im_info.dim_sizes['X'])
         else:
             self.scaling = (im_info.dim_sizes['Z'], im_info.dim_sizes['Y'], im_info.dim_sizes['X'])
 
-        self.max_distance_um = max_distance_um
+        self.max_distance_um = max_distance_um * im_info.dim_sizes['T']
+        self.max_distance_um = np.max([self.max_distance_um, 0.5])
+
         self.forward = forward
 
         self.shape = ()
 
         self.im_memmap = None
         self.flow_vector_array = None
```

### Comparing `nellie-0.1.8/nellie/tracking/hu_tracking.py` & `nellie-0.2/nellie/tracking/hu_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
             self.num_t = im_info.shape[im_info.axes.index('T')]
 
         if self.im_info.no_z:
             self.scaling = (im_info.dim_sizes['Y'], im_info.dim_sizes['X'])
         else:
             self.scaling = (im_info.dim_sizes['Z'], im_info.dim_sizes['Y'], im_info.dim_sizes['X'])
 
-        self.max_distance_um = max_distance_um
+        self.max_distance_um = max_distance_um * self.im_info.dim_sizes['T']
+        self.max_distance_um = xp.max([self.max_distance_um, 0.5])
 
         self.vector_start_coords = []
         self.vectors = []
         self.vector_magnitudes = []
 
         self.shape = ()
```

### Comparing `nellie-0.1.8/nellie/tracking/voxel_reassignment.py` & `nellie-0.2/nellie/tracking/voxel_reassignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,19 @@
         vox_next_matches = np.concatenate([vox_next_matches_fw, vox_next_matches_bw])
         distances = np.concatenate([distances_fw, distances_bw])
 
         vox_prev_matches_unique, vox_next_matches_unique = self._assign_unique_matches(vox_prev_matches,
                                                                                        vox_next_matches, distances)
 
         vox_next_matches_unique = np.array(vox_next_matches_unique)
+        if len(vox_next_matches_unique) == 0:
+            return [], []
         vox_next_matched_tuples = set([tuple(coord) for coord in vox_next_matches_unique])
         vox_next_unmatched = np.array([coord for coord in vox_next if tuple(coord) not in vox_next_matched_tuples])
+
         unmatched_diff = np.inf
         while unmatched_diff:
             num_unmatched = len(vox_next_unmatched)
             if num_unmatched == 0:
                 break
             tree = cKDTree(vox_next_matches_unique * self.flow_interpolator_fw.scaling)
             dists, idxs = tree.query(vox_next_unmatched * self.flow_interpolator_fw.scaling, k=1, workers=-1)
```

### Comparing `nellie-0.1.8/nellie/utils/general.py` & `nellie-0.2/nellie/utils/general.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie/utils/gpu_functions.py` & `nellie-0.2/nellie/utils/gpu_functions.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie/utils/torch_xp.py` & `nellie-0.2/nellie/utils/torch_xp.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie.egg-info/PKG-INFO` & `nellie-0.2/nellie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nellie
-Version: 0.1.8
+Version: 0.2
 Summary: Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 Home-page: https://github.com/aelefebv/nellie
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre+nellie@gmail.com
 Classifier: Framework :: napari
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `nellie-0.1.8/nellie.egg-info/SOURCES.txt` & `nellie-0.2/nellie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie_napari/batch_mode.py` & `nellie-0.2/nellie_napari/batch_mode.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie_napari/home.py` & `nellie-0.2/nellie_napari/home.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie_napari/logo.png` & `nellie-0.2/nellie_napari/logo.png`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie_napari/nellie_analysis.py` & `nellie-0.2/nellie_napari/nellie_analysis.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie_napari/nellie_fileselect.py` & `nellie-0.2/nellie_napari/nellie_fileselect.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie_napari/nellie_loader.py` & `nellie-0.2/nellie_napari/nellie_loader.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie_napari/nellie_processor.py` & `nellie-0.2/nellie_napari/nellie_processor.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/nellie_napari/visualizer.py` & `nellie-0.2/nellie_napari/visualizer.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.8/setup.cfg` & `nellie-0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nellie
-version = 0.1.8
+version = 0.2
 description = Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Austin E. Y. T. Lefebvre
 author_email = austin.e.lefebvre+nellie@gmail.com
 url = https://github.com/aelefebv/nellie
 classifiers =
```

### Comparing `nellie-0.1.8/tests/unit/test_im_info.py` & `nellie-0.2/tests/unit/test_im_info.py`

 * *Files identical despite different names*


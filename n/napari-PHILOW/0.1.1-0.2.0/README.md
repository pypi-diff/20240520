# Comparing `tmp/napari-PHILOW-0.1.1.tar.gz` & `tmp/napari_philow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-PHILOW-0.1.1.tar", last modified: Sun Feb  4 08:11:23 2024, max compression
+gzip compressed data, was "napari_philow-0.2.0.tar", last modified: Mon May 20 07:08:22 2024, max compression
```

## Comparing `napari-PHILOW-0.1.1.tar` & `napari_philow-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-02-04 08:11:23.604128 napari-PHILOW-0.1.1/
--rw-r--r--   0 hiroki     (501) staff       (20)    35148 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.1/LICENSE
--rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/MANIFEST.in
--rw-r--r--   0 hiroki     (501) staff       (20)     9793 2024-02-04 08:11:23.604005 napari-PHILOW-0.1.1/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)     8022 2024-02-04 08:09:07.000000 napari-PHILOW-0.1.1/README.md
--rw-r--r--   0 hiroki     (501) staff       (20)      179 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/pyproject.toml
--rw-r--r--   0 hiroki     (501) staff       (20)      193 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.1/requirements.txt
--rw-r--r--   0 hiroki     (501) staff       (20)     1786 2024-02-04 08:11:23.604454 napari-PHILOW-0.1.1/setup.cfg
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-02-04 08:11:23.596661 napari-PHILOW-0.1.1/src/
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-02-04 08:11:23.603400 napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/
--rw-r--r--   0 hiroki     (501) staff       (20)     9793 2024-02-04 08:11:23.000000 napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)     1051 2024-02-04 08:11:23.000000 napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/SOURCES.txt
--rw-r--r--   0 hiroki     (501) staff       (20)        1 2024-02-04 08:11:23.000000 napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/dependency_links.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       60 2024-02-04 08:11:23.000000 napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/entry_points.txt
--rw-r--r--   0 hiroki     (501) staff       (20)      164 2024-02-04 08:11:23.000000 napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/requires.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       14 2024-02-04 08:11:23.000000 napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/top_level.txt
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-02-04 08:11:23.601480 napari-PHILOW-0.1.1/src/napari_philow/
--rw-r--r--   0 hiroki     (501) staff       (20)      279 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/__init__.py
--rw-r--r--   0 hiroki     (501) staff       (20)     7787 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/_annotation.py
--rw-r--r--   0 hiroki     (501) staff       (20)     4453 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.1/src/napari_philow/_data_manager.py
--rw-r--r--   0 hiroki     (501) staff       (20)     4226 2024-02-04 08:07:02.000000 napari-PHILOW-0.1.1/src/napari_philow/_predict.py
--rw-r--r--   0 hiroki     (501) staff       (20)     5909 2024-02-04 08:05:33.000000 napari-PHILOW-0.1.1/src/napari_philow/_prediction.py
--rw-r--r--   0 hiroki     (501) staff       (20)     7703 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/_selector.py
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-02-04 08:11:23.601847 napari-PHILOW-0.1.1/src/napari_philow/_tests/
--rw-r--r--   0 hiroki     (501) staff       (20)        0 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.1/src/napari_philow/_tests/__init__.py
--rw-r--r--   0 hiroki     (501) staff       (20)      696 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.1/src/napari_philow/_tests/test_dock_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)     7683 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/_train_tf.py
--rw-r--r--   0 hiroki     (501) staff       (20)    10977 2024-02-04 08:05:33.000000 napari-PHILOW-0.1.1/src/napari_philow/_trainer.py
--rw-r--r--   0 hiroki     (501) staff       (20)    27950 2024-02-04 08:05:33.000000 napari-PHILOW-0.1.1/src/napari_philow/_utils.py
--rw-r--r--   0 hiroki     (501) staff       (20)      799 2024-02-04 08:09:10.000000 napari-PHILOW-0.1.1/src/napari_philow/napari.yaml
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-02-04 08:11:23.603187 napari-PHILOW-0.1.1/src/napari_philow/segmentation/
--rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/segmentation/__init__.py
--rw-r--r--   0 hiroki     (501) staff       (20)     4526 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/segmentation/data_augmentation.py
--rw-r--r--   0 hiroki     (501) staff       (20)     2653 2024-02-04 08:05:33.000000 napari-PHILOW-0.1.1/src/napari_philow/segmentation/dataset.py
--rw-r--r--   0 hiroki     (501) staff       (20)     1031 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/segmentation/loss.py
--rw-r--r--   0 hiroki     (501) staff       (20)      252 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/segmentation/metric.py
--rw-r--r--   0 hiroki     (501) staff       (20)     2244 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/segmentation/predict.py
--rw-r--r--   0 hiroki     (501) staff       (20)     5011 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/segmentation/train.py
--rw-r--r--   0 hiroki     (501) staff       (20)      316 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.1/src/napari_philow/segmentation/utils.py
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-05-20 07:08:22.125891 napari_philow-0.2.0/
+-rw-r--r--   0 hiroki     (501) staff       (20)    35148 2022-04-25 01:47:53.000000 napari_philow-0.2.0/LICENSE
+-rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-18 02:41:23.000000 napari_philow-0.2.0/MANIFEST.in
+-rw-r--r--   0 hiroki     (501) staff       (20)    11484 2024-05-20 07:08:22.125564 napari_philow-0.2.0/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)     9713 2024-05-20 07:06:43.000000 napari_philow-0.2.0/README.md
+-rw-r--r--   0 hiroki     (501) staff       (20)      179 2023-04-18 02:41:23.000000 napari_philow-0.2.0/pyproject.toml
+-rw-r--r--   0 hiroki     (501) staff       (20)      193 2022-04-25 01:47:53.000000 napari_philow-0.2.0/requirements.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)     1786 2024-05-20 07:08:22.126379 napari_philow-0.2.0/setup.cfg
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-05-20 07:08:22.108626 napari_philow-0.2.0/src/
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-05-20 07:08:22.124391 napari_philow-0.2.0/src/napari_PHILOW.egg-info/
+-rw-r--r--   0 hiroki     (501) staff       (20)    11484 2024-05-20 07:08:22.000000 napari_philow-0.2.0/src/napari_PHILOW.egg-info/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)     1086 2024-05-20 07:08:22.000000 napari_philow-0.2.0/src/napari_PHILOW.egg-info/SOURCES.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)        1 2024-05-20 07:08:22.000000 napari_philow-0.2.0/src/napari_PHILOW.egg-info/dependency_links.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       60 2024-05-20 07:08:22.000000 napari_philow-0.2.0/src/napari_PHILOW.egg-info/entry_points.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)      164 2024-05-20 07:08:22.000000 napari_philow-0.2.0/src/napari_PHILOW.egg-info/requires.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       14 2024-05-20 07:08:22.000000 napari_philow-0.2.0/src/napari_PHILOW.egg-info/top_level.txt
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-05-20 07:08:22.119259 napari_philow-0.2.0/src/napari_philow/
+-rw-r--r--   0 hiroki     (501) staff       (20)      279 2023-04-18 02:41:23.000000 napari_philow-0.2.0/src/napari_philow/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     9540 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/_annotation.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     4453 2022-04-25 01:47:53.000000 napari_philow-0.2.0/src/napari_philow/_data_manager.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     6412 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/_predict.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     8737 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/_prediction.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     7703 2023-04-18 02:41:23.000000 napari_philow-0.2.0/src/napari_philow/_selector.py
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-05-20 07:08:22.120043 napari_philow-0.2.0/src/napari_philow/_tests/
+-rw-r--r--   0 hiroki     (501) staff       (20)        0 2022-04-25 01:47:53.000000 napari_philow-0.2.0/src/napari_philow/_tests/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      696 2022-04-25 01:47:53.000000 napari_philow-0.2.0/src/napari_philow/_tests/test_dock_widget.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     7683 2023-04-18 02:41:23.000000 napari_philow-0.2.0/src/napari_philow/_train_tf.py
+-rw-r--r--   0 hiroki     (501) staff       (20)    14518 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/_trainer.py
+-rw-r--r--   0 hiroki     (501) staff       (20)    27914 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/_utils.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     2401 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/_utils_legacy.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      800 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/napari.yaml
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2024-05-20 07:08:22.123881 napari_philow-0.2.0/src/napari_philow/segmentation/
+-rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-18 02:41:23.000000 napari_philow-0.2.0/src/napari_philow/segmentation/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     4846 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/segmentation/data_augmentation.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     4714 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/segmentation/dataset.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     1031 2023-04-18 02:41:23.000000 napari_philow-0.2.0/src/napari_philow/segmentation/loss.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      252 2023-04-18 02:41:23.000000 napari_philow-0.2.0/src/napari_philow/segmentation/metric.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     2722 2024-05-20 07:06:43.000000 napari_philow-0.2.0/src/napari_philow/segmentation/predict.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     5011 2023-04-18 02:41:23.000000 napari_philow-0.2.0/src/napari_philow/segmentation/train.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      316 2023-04-18 02:41:23.000000 napari_philow-0.2.0/src/napari_philow/segmentation/utils.py
```

### Comparing `napari-PHILOW-0.1.1/LICENSE` & `napari_philow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.1.1/PKG-INFO` & `napari_philow-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-PHILOW
-Version: 0.1.1
+Version: 0.2.0
 Summary: PHILOW is an interactive deep learning-based platform for 3D datasets
 Home-page: https://github.com/neurobiology-ut/PHILOW
 Author: Hiroki Kawai
 Author-email: h.kawai888@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/neurobiology-ut/PHILOW/issues
 Project-URL: Documentation, https://github.com/neurobiology-ut/PHILOW#README.md
@@ -151,14 +151,32 @@
 3) Select labels dir : all label images should be named same as original images and contains data management csv file   
    
 4) Select dir for save trained model   
    
 5) Click on the "start training" button   
 
 6) Dice score and dice loss are displayed. For more detail, check the command line for the progress of training. If you want to stop in the middle, click stop button.   
+
+##### IF YOU WANT TO SEGMENT CRISTAE AREA IN THE EM DATASET
+
+1) Plugins > napari-PHILOW > Trainer
+
+2) Click on the "Cristae segmentation mode" button   
+
+3) Select original dir : all slices must be in separate PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)  
+
+4) Select mito mask dir : all label images should be named same as original images
+
+5) Select dir for save trained model  
+
+6) Select cristae labels dir : all label images should be named same as original images and contains data management csv file  
+
+7) Click on the "start training" button   
+
+8) Dice score and dice loss are displayed. For more detail, check the command line for the progress of training. If you want to stop in the middle, click stop button.   
    
 #### Predict
 To predict labels on your machine,  
 
 1) Plugins > napari-PHILOW > Predicter
    
 2) Select original dir : all slices must be in separate 8bit PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)   
@@ -173,14 +191,38 @@
    
 7) Click on the "predict" button  
 
 8) Check the command line for the progress of prediction. If you want to stop in the middle, use ctrl+C.   
 
 9) You can start the next round of annotation by selecting the merged_prediction directory as the mask dir in Annotation mode.
 
+##### IF YOU WANT TO SEGMENT CRISTAE AREA IN THE EM DATASET
+
+1) Plugins > napari-PHILOW > Predicter
+
+2) Select original dir : all slices must be in separate PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)   
+
+3) (Optional) Select cristae labels dir if you want to keep labels witch were used on training, and data management csv file  
+
+4) Select model dir contains hdf5 file   
+
+5) Select output dir for predicted labels   
+
+6) Uncheck the box if you DO NOT want to use TAP (Three-Axis-Prediction)   
+
+7) Click on the "Use cristae inference mode" button   
+
+8) Select mitochondria mask dir : all label images should be named same as original images
+
+9) Click on the "predict" button  
+
+10) Check the command line for the progress of prediction. If you want to stop in the middle, use ctrl+C.   
+
+11) You can start the next round of annotation by selecting the merged_prediction directory as the mask dir in Annotation mode.
+
 ### Train and predict with Google Colab   
 If you don't have a GPU machine, you can use Google Colab to perform GPU-based training and prediction for free.    
 
 1) Open [train and predict notebook](https://github.com/neurobiology-ut/PHILOW/blob/develop/notebooks/train_and_pred_using_PHILOW.ipynb) and click "Open in Colab" button
 
 2) You can upload your own dataset to train and predict, or try it on demo data
```

### Comparing `napari-PHILOW-0.1.1/README.md` & `napari_philow-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -107,14 +107,32 @@
 3) Select labels dir : all label images should be named same as original images and contains data management csv file   
    
 4) Select dir for save trained model   
    
 5) Click on the "start training" button   
 
 6) Dice score and dice loss are displayed. For more detail, check the command line for the progress of training. If you want to stop in the middle, click stop button.   
+
+##### IF YOU WANT TO SEGMENT CRISTAE AREA IN THE EM DATASET
+
+1) Plugins > napari-PHILOW > Trainer
+
+2) Click on the "Cristae segmentation mode" button   
+
+3) Select original dir : all slices must be in separate PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)  
+
+4) Select mito mask dir : all label images should be named same as original images
+
+5) Select dir for save trained model  
+
+6) Select cristae labels dir : all label images should be named same as original images and contains data management csv file  
+
+7) Click on the "start training" button   
+
+8) Dice score and dice loss are displayed. For more detail, check the command line for the progress of training. If you want to stop in the middle, click stop button.   
    
 #### Predict
 To predict labels on your machine,  
 
 1) Plugins > napari-PHILOW > Predicter
    
 2) Select original dir : all slices must be in separate 8bit PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)   
@@ -129,14 +147,38 @@
    
 7) Click on the "predict" button  
 
 8) Check the command line for the progress of prediction. If you want to stop in the middle, use ctrl+C.   
 
 9) You can start the next round of annotation by selecting the merged_prediction directory as the mask dir in Annotation mode.
 
+##### IF YOU WANT TO SEGMENT CRISTAE AREA IN THE EM DATASET
+
+1) Plugins > napari-PHILOW > Predicter
+
+2) Select original dir : all slices must be in separate PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)   
+
+3) (Optional) Select cristae labels dir if you want to keep labels witch were used on training, and data management csv file  
+
+4) Select model dir contains hdf5 file   
+
+5) Select output dir for predicted labels   
+
+6) Uncheck the box if you DO NOT want to use TAP (Three-Axis-Prediction)   
+
+7) Click on the "Use cristae inference mode" button   
+
+8) Select mitochondria mask dir : all label images should be named same as original images
+
+9) Click on the "predict" button  
+
+10) Check the command line for the progress of prediction. If you want to stop in the middle, use ctrl+C.   
+
+11) You can start the next round of annotation by selecting the merged_prediction directory as the mask dir in Annotation mode.
+
 ### Train and predict with Google Colab   
 If you don't have a GPU machine, you can use Google Colab to perform GPU-based training and prediction for free.    
 
 1) Open [train and predict notebook](https://github.com/neurobiology-ut/PHILOW/blob/develop/notebooks/train_and_pred_using_PHILOW.ipynb) and click "Open in Colab" button
 
 2) You can upload your own dataset to train and predict, or try it on demo data
```

### Comparing `napari-PHILOW-0.1.1/setup.cfg` & `napari_philow-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-PHILOW
-version = 0.1.1
+version = 0.2.0
 author = Hiroki Kawai
 author_email = h.kawai888@gmail.com
 url = https://github.com/neurobiology-ut/PHILOW
 license = GPLv3
 license_files = LICENSE
 description = PHILOW is an interactive deep learning-based platform for 3D datasets
 long_description = file: README.md
```

### Comparing `napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/PKG-INFO` & `napari_philow-0.2.0/src/napari_PHILOW.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-PHILOW
-Version: 0.1.1
+Version: 0.2.0
 Summary: PHILOW is an interactive deep learning-based platform for 3D datasets
 Home-page: https://github.com/neurobiology-ut/PHILOW
 Author: Hiroki Kawai
 Author-email: h.kawai888@gmail.com
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/neurobiology-ut/PHILOW/issues
 Project-URL: Documentation, https://github.com/neurobiology-ut/PHILOW#README.md
@@ -151,14 +151,32 @@
 3) Select labels dir : all label images should be named same as original images and contains data management csv file   
    
 4) Select dir for save trained model   
    
 5) Click on the "start training" button   
 
 6) Dice score and dice loss are displayed. For more detail, check the command line for the progress of training. If you want to stop in the middle, click stop button.   
+
+##### IF YOU WANT TO SEGMENT CRISTAE AREA IN THE EM DATASET
+
+1) Plugins > napari-PHILOW > Trainer
+
+2) Click on the "Cristae segmentation mode" button   
+
+3) Select original dir : all slices must be in separate PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)  
+
+4) Select mito mask dir : all label images should be named same as original images
+
+5) Select dir for save trained model  
+
+6) Select cristae labels dir : all label images should be named same as original images and contains data management csv file  
+
+7) Click on the "start training" button   
+
+8) Dice score and dice loss are displayed. For more detail, check the command line for the progress of training. If you want to stop in the middle, click stop button.   
    
 #### Predict
 To predict labels on your machine,  
 
 1) Plugins > napari-PHILOW > Predicter
    
 2) Select original dir : all slices must be in separate 8bit PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)   
@@ -173,14 +191,38 @@
    
 7) Click on the "predict" button  
 
 8) Check the command line for the progress of prediction. If you want to stop in the middle, use ctrl+C.   
 
 9) You can start the next round of annotation by selecting the merged_prediction directory as the mask dir in Annotation mode.
 
+##### IF YOU WANT TO SEGMENT CRISTAE AREA IN THE EM DATASET
+
+1) Plugins > napari-PHILOW > Predicter
+
+2) Select original dir : all slices must be in separate PNG and must be sequentially numbered (e.g. 000.png, 001.png ...)   
+
+3) (Optional) Select cristae labels dir if you want to keep labels witch were used on training, and data management csv file  
+
+4) Select model dir contains hdf5 file   
+
+5) Select output dir for predicted labels   
+
+6) Uncheck the box if you DO NOT want to use TAP (Three-Axis-Prediction)   
+
+7) Click on the "Use cristae inference mode" button   
+
+8) Select mitochondria mask dir : all label images should be named same as original images
+
+9) Click on the "predict" button  
+
+10) Check the command line for the progress of prediction. If you want to stop in the middle, use ctrl+C.   
+
+11) You can start the next round of annotation by selecting the merged_prediction directory as the mask dir in Annotation mode.
+
 ### Train and predict with Google Colab   
 If you don't have a GPU machine, you can use Google Colab to perform GPU-based training and prediction for free.    
 
 1) Open [train and predict notebook](https://github.com/neurobiology-ut/PHILOW/blob/develop/notebooks/train_and_pred_using_PHILOW.ipynb) and click "Open in Colab" button
 
 2) You can upload your own dataset to train and predict, or try it on demo data
```

### Comparing `napari-PHILOW-0.1.1/src/napari_PHILOW.egg-info/SOURCES.txt` & `napari_philow-0.2.0/src/napari_PHILOW.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/napari_philow/_data_manager.py
 src/napari_philow/_predict.py
 src/napari_philow/_prediction.py
 src/napari_philow/_selector.py
 src/napari_philow/_train_tf.py
 src/napari_philow/_trainer.py
 src/napari_philow/_utils.py
+src/napari_philow/_utils_legacy.py
 src/napari_philow/napari.yaml
 src/napari_philow/_tests/__init__.py
 src/napari_philow/_tests/test_dock_widget.py
 src/napari_philow/segmentation/__init__.py
 src/napari_philow/segmentation/data_augmentation.py
 src/napari_philow/segmentation/dataset.py
 src/napari_philow/segmentation/loss.py
```

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/_annotation.py` & `napari_philow-0.2.0/src/napari_philow/_annotation.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,76 +3,115 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 from magicgui import magicgui
 from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.figure import Figure
 from napari._qt.qthreading import thread_worker
-from qtpy.QtWidgets import QWidget, QPushButton, QSizePolicy, QLineEdit, QCheckBox, QLabel, QVBoxLayout, QFileDialog
+from qtpy.QtWidgets import QWidget, QPushButton, QSizePolicy, QLineEdit, QCheckBox, QLabel, QVBoxLayout, QFileDialog, QFormLayout
+from qtpy.QtCore import Qt
 from scipy import ndimage
 from skimage import io
+from vispy.color import Colormap
 
 from napari_philow._data_manager import Datamanager
-from napari_philow._utils import combine_blocks, load_images, load_saved_masks, load_raw_masks, label_ct, \
-    label_and_sort, save_masks, crop_img, show_so_layer
+from napari_philow._utils import load_images, load_saved_masks, load_raw_masks, label_ct, \
+    label_and_sort, save_masks, crop_img, show_so_layer, load_mask_masks
 
 
 class AnnotationMode(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self._viewer = napari_viewer
         self.opath = ""
         self.modpath = ""
-        self.btn1 = QPushButton('open', self)
-        self.btn1.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.maskpath = ""
+        self.btn1 = QPushButton('Open', self)
         self.btn1.clicked.connect(self.show_dialog_o)
-        self.btn2 = QPushButton('open', self)
-        self.btn2.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.lbl1 = QLabel("Not selected")
+        self.btn2 = QPushButton('Open', self)
         self.btn2.clicked.connect(self.show_dialog_mod)
+        self.lbl2 = QLabel("Not selected")
 
         self.textbox = QLineEdit(self)
-        self.textbox.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
 
-        self.checkBox = QCheckBox("create new dataset?")
-        self.checkBox.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.checkBox = QCheckBox("Create new dataset?")
+
+        self.checkBox_mask = QCheckBox("Apply mask? (If you are labeling cristae, please apply a mitochondrial mask)")
+        self.checkBox_mask.stateChanged.connect(self.toggle_mask_button)
+
+        self.lbl_mask_dir = QLabel('Mask dir:')
+        self.btn_mask = QPushButton('Open', self)
+        self.btn_mask.clicked.connect(self.show_dialog_mask)
+        self.lbl_mask = QLabel("Not selected")
+        self.lbl_mask_dir.hide()
+        self.btn_mask.hide()
+        self.lbl_mask.hide()
+
+        self.checkBox_3d = QCheckBox("If you are labeling 3D data, please check this box")
 
         self.btn4 = QPushButton('Start tracing', self)
-        self.btn4.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn4.clicked.connect(self.launch)
-        self.lbl = QLabel('original dir', self)
-        self.lbl2 = QLabel('mask dir', self)
-        self.lbl4 = QLabel('model type (do not use word "train")', self)
+
         self.build()
 
         self.filenames = None
 
     def build(self):
-        vbox = QVBoxLayout()
-        vbox.addWidget(combine_blocks(self.btn1, self.lbl))
-        vbox.addWidget(combine_blocks(self.btn2, self.lbl2))
-        vbox.addWidget(combine_blocks(self.textbox, self.lbl4))
-        vbox.addWidget(self.checkBox)
-        vbox.addWidget(self.btn4)
+        layout = QVBoxLayout()
+
+        form_layout = QFormLayout()
+        form_layout.addRow('Original dir:', self.btn1)
+        form_layout.addRow(self.lbl1)
+        form_layout.addRow('Label dir:', self.btn2)
+        form_layout.addRow(self.lbl2)
+        form_layout.addRow(self.checkBox_mask)
+        form_layout.addRow(self.lbl_mask_dir, self.btn_mask)
+        form_layout.addRow(self.lbl_mask)
+        form_layout.addRow('Model type (do not use word "train"):', self.textbox)
+        form_layout.setLabelAlignment(Qt.AlignLeft)  # 左寄せに設定
+
+        layout.addLayout(form_layout)
+        layout.addWidget(self.checkBox)
+        layout.addWidget(self.checkBox_3d)
+        layout.addWidget(self.btn4)
 
-        self.setLayout(vbox)
+        self.setLayout(layout)
         self.show()
 
     def show_dialog_o(self):
         default_path = max(self.opath, self.modpath, os.path.expanduser('~'))
         f_name = QFileDialog.getExistingDirectory(self, 'Open Directory', default_path)
         if f_name:
             self.opath = f_name
-            self.lbl.setText(self.opath)
+            self.lbl1.setText(f_name)
 
     def show_dialog_mod(self):
         default_path = max(self.opath, self.modpath, os.path.expanduser('~'))
         f_name = QFileDialog.getExistingDirectory(self, 'Open Directory', default_path)
         if f_name:
             self.modpath = f_name
-            self.lbl2.setText(self.modpath)
+            self.lbl2.setText(f_name)
+
+    def show_dialog_mask(self):
+        default_path = max(self.opath, self.modpath, os.path.expanduser('~'))
+        f_name = QFileDialog.getExistingDirectory(self, 'Open Directory', default_path)
+        if f_name:
+            self.maskpath = f_name
+            self.lbl_mask.setText(f_name)
+
+    def toggle_mask_button(self, state):
+        if state == Qt.Checked:
+            self.lbl_mask_dir.show()
+            self.btn_mask.show()
+            self.lbl_mask.show()
+        else:
+            self.lbl_mask_dir.hide()
+            self.btn_mask.hide()
+            self.lbl_mask.hide()
 
     def launch(self):
         images = load_images(self.opath)
         if self.modpath == "":
             self.modpath = os.path.join(os.path.dirname(self.opath), self.textbox.text())
             os.makedirs(self.modpath, exist_ok=True)
         else:
@@ -84,18 +123,22 @@
                 io.imsave(os.path.join(self.modpath, filename), labels[i])
         else:
             labels, self.filenames = load_saved_masks(self.modpath)
         try:
             labels_raw = load_raw_masks(self.modpath + '_raw')
         except:
             labels_raw = None
+        if self.maskpath == "":
+            mask = None
+        else:
+            mask = load_mask_masks(self.maskpath)
         self._viewer.window.remove_dock_widget(self)
-        self.launch_anm(images, labels, labels_raw)
+        self.launch_anm(images, labels, labels_raw, mask)
 
-    def launch_anm(self, original, base, raw):
+    def launch_anm(self, original, base, raw, mask):
         global slicer
         global z_pos
         global layer
         global images_original
         global base_label
         r_path = self.modpath
         model_type = self.textbox.text()
@@ -105,18 +148,24 @@
         try:
             del layer
         except NameError:
             pass
         self._viewer.add_image(images_original, contrast_limits=[0, 255])
         self._viewer.add_labels(base_label, name='base')
         if raw is not None:
-            self._viewer.add_image(ndimage.gaussian_filter(raw, sigma=3), colormap='magenta', name='low_confident',
-                                   blending='additive')
+            if self.checkBox_3d.isChecked():
+                self._viewer.add_image(ndimage.gaussian_filter(raw, sigma=3), colormap='magenta', name='low_confident',
+                                       blending='additive')
+            else:
+                self._viewer.add_image(ndimage.gaussian_filter(raw, sigma=(0, 3, 3)), colormap='magenta', name='low_confident',
+                                       blending='additive')
         else:
             pass
+        if mask is not None:
+            self._viewer.add_image(mask, name='mask', blending='minimum')
 
         @thread_worker(connect={"returned": show_so_layer})
         def create_label(viewer):
             labeled_sorted, nums = label_and_sort(base_label)
             print(nums)
             labeled_c = label_ct(labeled_sorted, nums, 10)
             return labeled_c, labeled_sorted, nums, viewer
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/_data_manager.py` & `napari_philow-0.2.0/src/napari_philow/_data_manager.py`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/_selector.py` & `napari_philow-0.2.0/src/napari_philow/_selector.py`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/_tests/test_dock_widget.py` & `napari_philow-0.2.0/src/napari_philow/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/_train_tf.py` & `napari_philow-0.2.0/src/napari_philow/_train_tf.py`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/_trainer.py` & `napari_philow-0.2.0/src/napari_philow/_trainer.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,56 +8,67 @@
 from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.figure import Figure
 import numpy as np
 import pandas as pd
 from PIL import Image
 from napari.qt.threading import create_worker
 from qtpy.QtWidgets import QWidget, QPushButton, QSizePolicy, QLabel, QVBoxLayout, QFileDialog, QCheckBox, QSpinBox
+from qtpy.QtCore import Qt
 from segmentation_models_pytorch import UnetPlusPlus
 from torch import optim
 from torch.utils import data
 
-from napari_philow._utils import combine_blocks
-from napari_philow.segmentation.dataset import PHILOWDataset, ImageTransform
+from napari_philow._utils import combine_blocks, preprocess_cristae
+from napari_philow.segmentation.dataset import PHILOWDataset, ImageTransform, CristaeDataset, CristaeImageTransform
 from napari_philow.segmentation.loss import DiceBCELoss
 from napari_philow.segmentation.train import train_model
 
 
 class Trainer(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self._viewer = napari_viewer
         self.opath = ""
         self.labelpath = ""
+        self.cristaepath = ""
         self.modelpath = ""
         self.prev_modelpath = ""
+        self.checkBox_cristae = QCheckBox("Cristae segmentation mode")
+        self.checkBox_cristae.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.checkBox_cristae.stateChanged.connect(self.toggle_checkboxes)
+        self.lbl = QLabel('original dir', self)
         self.btn1 = QPushButton('open', self)
         self.btn1.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn1.clicked.connect(self.show_dialog_o)
+        self.lbl2 = QLabel('label dir', self)
         self.btn2 = QPushButton('open', self)
         self.btn2.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn2.clicked.connect(self.show_dialog_label)
+        self.lbl3 = QLabel('model output dir', self)
         self.btn3 = QPushButton('open', self)
         self.btn3.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn3.clicked.connect(self.show_dialog_model)
+        self.lbl4 = QLabel('(optional) previous model path (.pth)', self)
         self.btn4 = QPushButton('open', self)
         self.btn4.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn4.clicked.connect(self.show_dialog_prev_model)
         self.btn5 = QPushButton('start training', self)
         self.btn5.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn5.clicked.connect(self.trainer)
-        self.lbl = QLabel('original dir', self)
-        self.lbl2 = QLabel('label dir', self)
-        self.lbl3 = QLabel('model output dir', self)
-        self.lbl4 = QLabel('(optional) previous model path (.pth)', self)
         self.lbl5 = QLabel('epochs', self)
         self.epoch = QSpinBox(maximum=1000, value=400)
         self.checkBox = QCheckBox("Resize to 256x256?")
         self.checkBox_split = QCheckBox("Split and create validation data from training data?")
         self.checkBox.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.lbl_cristae = QLabel('cristae label dir', self)
+        self.btn_cristae = QPushButton('open', self)
+        self.btn_cristae.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        self.btn_cristae.clicked.connect(self.show_dialog_cristae)
+        self.lbl_cristae.setVisible(False)
+        self.btn_cristae.setVisible(False)
 
         with plt.style.context('dark_background'):
             self.canvas = FigureCanvas(Figure(figsize=(3, 5)))
             self.canvas.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Maximum)
             self.axes = self.canvas.figure.subplots()
 
         self.build()
@@ -70,21 +81,23 @@
         self.label_layer = None
         self.prediction_layer = None
 
         self.df = pd.DataFrame(columns=['epoch', 'train_loss', 'val_loss'])
 
     def build(self):
         vbox = QVBoxLayout()
+        vbox.addWidget(self.checkBox_cristae)
         vbox.addWidget(combine_blocks(self.btn1, self.lbl))
         vbox.addWidget(combine_blocks(self.btn2, self.lbl2))
         vbox.addWidget(combine_blocks(self.btn3, self.lbl3))
         vbox.addWidget(combine_blocks(self.btn4, self.lbl4))
         vbox.addWidget(combine_blocks(self.lbl5, self.epoch))
-        # vbox.addWidget(self.checkBox)
+        vbox.addWidget(self.checkBox)
         vbox.addWidget(self.checkBox_split)
+        vbox.addWidget(combine_blocks(self.btn_cristae, self.lbl_cristae))
         vbox.addWidget(self.btn5)
         vbox.addWidget(self.canvas)
 
         self.setLayout(vbox)
         self.show()
 
     def show_dialog_o(self):
@@ -111,19 +124,43 @@
     def show_dialog_prev_model(self):
         default_path = max(self.opath, self.labelpath, os.path.expanduser('~'))
         f_name, _ = QFileDialog.getOpenFileName(self, 'Select weight file', default_path)
         if f_name:
             self.prev_modelpath = f_name
             self.lbl4.setText(self.prev_modelpath)
 
+    def show_dialog_cristae(self):
+        default_path = max(self.opath, self.labelpath, os.path.expanduser('~'))
+        f_name = QFileDialog.getExistingDirectory(self, 'Open Directory', default_path)
+        if f_name:
+            self.cristaepath = f_name
+            self.lbl_cristae.setText(self.cristaepath)
+
     def get_newest_csv(self):
-        csvs = sorted(list(Path(self.labelpath).glob('./*csv')))
+        if self.cristaepath:
+            csvs = sorted(list(Path(self.cristaepath).glob('./*csv')))
+        else:
+            csvs = sorted(list(Path(self.labelpath).glob('./*csv')))
         csv = pd.read_csv(str(csvs[-1]), index_col=0)
         return csv
 
+    def toggle_checkboxes(self, state):
+        if state == Qt.Checked:
+            self.checkBox.setVisible(False)
+            self.checkBox_split.setVisible(False)
+            self.btn_cristae.setVisible(True)
+            self.lbl_cristae.setVisible(True)
+            self.lbl2.setText("mito mask dir")
+        else:
+            self.checkBox.setVisible(True)
+            self.checkBox_split.setVisible(True)
+            self.btn_cristae.setVisible(False)
+            self.lbl_cristae.setVisible(False)
+            self.lbl2.setText("label dir")
+
     def update_layer(self, value):
         self.axes.clear()
         self.df.loc[len(self.df)] = {'epoch': value[0], 'train_loss': value[1], 'val_loss': value[2]}
         self.df.to_csv(os.path.join(self.modelpath, "train_log.csv"))
         self.axes.plot(list(self.df['epoch']), list(self.df['train_loss']), label='train_loss')
         if self.checkBox_split.isChecked():
             self.axes.plot(list(self.df['epoch']), list(self.df['val_loss']), label='val_loss')
@@ -161,70 +198,88 @@
 
     def delete_worker(self):
         del self.worker
         self.worker = None
         self.btn5.setText('start training')
 
     def trainer(self):
+        train_cristae = self.checkBox_cristae.isChecked()
         if self.worker:
             if self.worker.is_running:
                 self.btn5.setText('stopping...')
                 self.stop_training = True
                 self.worker.send(self.stop_training)
             else:
                 self.delete_worker()
         else:
             self.df = pd.DataFrame(columns=['epoch', 'train_loss', 'val_loss'])
             csv = self.get_newest_csv()
             names = list(csv[csv['train'] == 'Checked']['filename'])
             test_names = [name for name in list(csv[csv['train'] != 'Checked']['filename']) if
                           os.path.isfile(os.path.join(self.opath, name))]
-            print(test_names)
-            if self.checkBox_split.isChecked():
-                np.random.shuffle(names)
-                split_index = 9 * len(names) // 10
-                train_names = names[0: split_index]
-                val_names = names[split_index:]
-            else:
-                train_names = names
-
-            w, h = Image.open(os.path.join(self.opath, names[0])).size
-
-            batch_size = min(math.ceil(len(train_names) / 10), 4)
-            print('batchsize = ', batch_size)
-
-            train_dataset = PHILOWDataset(self.opath, self.labelpath, train_names, 'train', ImageTransform(512),
-                                          multiplier=math.ceil(max(w, h) / 512))
-            train_dataloader = data.DataLoader(
-                train_dataset, batch_size=batch_size, shuffle=True, num_workers=max(1, os.cpu_count() - 2))
-            if len(test_names) != 0:
-                test_dataset = PHILOWDataset(self.opath, self.labelpath, test_names, 'val', ImageTransform(512))
-                test_dataloader = data.DataLoader(test_dataset, batch_size=1, shuffle=True, num_workers=1)
-            else:
-                test_dataloader = None
+            # GPUが使えるかを確認
+            device = torch.device("cuda:0" if torch.cuda.is_available() else "mps" if torch.backends.mps.is_available() else "cpu")
+            print("使用デバイス：", device)
 
-            if self.checkBox_split.isChecked():
-                val_dataset = PHILOWDataset(self.opath, self.labelpath, val_names, 'val', ImageTransform(512),
-                                            multiplier=math.ceil(max(w, h) / 512))
+            if train_cristae:
+                w, h = 1000, 1000
+                ori_imgs, label_imgs = preprocess_cristae(self.opath, self.labelpath, self.cristaepath, names)
+                assert ori_imgs.shape[0] == label_imgs.shape[0]
+                assert ori_imgs.shape[0] > 1, 'not enough data'
+                split_index = 9 * ori_imgs.shape[0] // 10
+                train_imgs, train_labels = ori_imgs[:split_index], label_imgs[:split_index]
+                val_imgs, val_labels = ori_imgs[split_index:], label_imgs[split_index:]
+                batch_size = min(math.ceil(train_imgs.shape[0] / 10), 4)
+                train_dataset = CristaeDataset(train_imgs, train_labels, 'train', CristaeImageTransform(512),
+                                               multiplier=math.ceil(max(w, h) / 512))
+                train_dataloader = data.DataLoader(
+                    train_dataset, batch_size=batch_size, shuffle=True, num_workers=max(1, os.cpu_count() - 2))
+                val_dataset = CristaeDataset(val_imgs, val_labels, 'val', CristaeImageTransform(512),
+                                             multiplier=math.ceil(max(w, h) / 512))
                 val_dataloader = data.DataLoader(
                     val_dataset, batch_size=batch_size, shuffle=True, num_workers=max(1, os.cpu_count() - 2))
-            else:
-                val_dataloader = None
+                test_dataloader = None
+                net = UnetPlusPlus(encoder_name="efficientnet-b0", encoder_weights="imagenet", in_channels=1, classes=3,
+                                   activation='sigmoid')
 
+            else:
+                if self.checkBox_split.isChecked():
+                    assert len(names) > 1, 'not enough data'
+                    np.random.shuffle(names)
+                    split_index = 9 * len(names) // 10
+                    train_names = names[0: split_index]
+                    val_names = names[split_index:]
+                else:
+                    train_names = names
+
+                batch_size = min(math.ceil(len(train_names) / 10), 4)
+                w, h = Image.open(os.path.join(self.opath, names[0])).size
+                train_dataset = PHILOWDataset(self.opath, self.labelpath, train_names, 'train', ImageTransform(512),
+                                              multiplier=math.ceil(max(w, h) / 512))
+                train_dataloader = data.DataLoader(
+                    train_dataset, batch_size=batch_size, shuffle=True, num_workers=max(1, os.cpu_count() - 2))
+                if len(test_names) != 0:
+                    test_dataset = PHILOWDataset(self.opath, self.labelpath, test_names, 'val', ImageTransform(512))
+                    test_dataloader = data.DataLoader(test_dataset, batch_size=1, shuffle=True, num_workers=1)
+                else:
+                    test_dataloader = None
+                if self.checkBox_split.isChecked():
+                    val_dataset = PHILOWDataset(self.opath, self.labelpath, val_names, 'val', ImageTransform(512),
+                                                multiplier=math.ceil(max(w, h) / 512))
+                    val_dataloader = data.DataLoader(
+                        val_dataset, batch_size=batch_size, shuffle=True, num_workers=max(1, os.cpu_count() - 2))
+                else:
+                    val_dataloader = None
+                net = UnetPlusPlus(encoder_name="efficientnet-b0", encoder_weights="imagenet", in_channels=1, classes=1,
+                                   activation='sigmoid')
             # 辞書オブジェクトにまとめる
             dataloaders_dict = {"train": train_dataloader, "val": val_dataloader, "test": test_dataloader}
 
             print(dataloaders_dict)
-
-            # GPUが使えるかを確認
-            device = torch.device("cuda:0" if torch.cuda.is_available() else "mps" if torch.backends.mps.is_available() else "cpu")
-            print("使用デバイス：", device)
-
-            net = UnetPlusPlus(encoder_name="efficientnet-b0", encoder_weights="imagenet", in_channels=1, classes=1,
-                               activation='sigmoid')
+            print('batchsize = ', batch_size)
 
             optimizer = optim.AdamW(net.parameters())
 
             try:
                 net.load_state_dict(torch.load(self.prev_modelpath, map_location=device))
                 print('loaded model from ' + self.prev_modelpath)
             except:
@@ -246,7 +301,10 @@
         if self.worker.is_running:
             self.btn5.setText('stopping...')
             self.stop_training = True
         else:
             self.worker.start()
             self.stop_training = False
             self.btn5.setText('stop')
+
+
+
```

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/_utils.py` & `napari_philow-0.2.0/src/napari_philow/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,41 @@
 import copy
 import os
+from datetime import datetime
 from pathlib import Path
 
-import cv2
 import dask
 import dask_image.imread
 from qtpy.QtWidgets import QWidget, QHBoxLayout, QSlider, QLabel
 from qtpy.QtCore import Qt
 import numpy as np
 from scipy import ndimage
-from skimage import io
-from skimage.filters import gaussian
+from skimage import io, morphology
 import pandas as pd
-from tqdm import tqdm
-
-
-def combine_blocks(block1, block2):
-    temp_widget = QWidget()
-    temp_layout = QHBoxLayout()
-    temp_layout.addWidget(block1)
-    temp_layout.addWidget(block2)
-    temp_widget.setLayout(temp_layout)
-    return temp_widget
-
-
-def normalize_x(image):
-    image = image / 127.5 - 1
-    return image
-
-
-def normalize_y(image):
-    image = image / 255
-    return image
-
-
-def denormalize_y(image):
-    return image * 255
 
 
 def renormalize_8bit(image):
     origin_min = image.min()
     origin_max = image.max()
     image -= origin_min
     image = image/(origin_max-origin_min)
     image *= 255
     return image.astype(np.uint8)
 
 
-def annotation_to_input(label_ermito):
-    mito = (label_ermito == 1) * 255
-    er = (label_ermito == 2) * 255
-    mito = normalize_y(mito)
-    er = normalize_y(er)
-    mito_anno = np.zeros_like(mito)
-    er_anno = np.zeros_like(er)
-    mito = gaussian(mito, sigma=2) * 255
-    er = gaussian(er, sigma=2) * 255
-    mito_anno[:, :] = mito
-    er_anno[:, :] = er
-    anno = np.concatenate([mito_anno[:, :, np.newaxis], er_anno[:, :, np.newaxis]], 2)
-    anno = normalize_x(anno[np.newaxis, :, :, :])
-    return anno
-
-
 def check_csv(project_path, ext):
     if not os.path.isfile(os.path.join(project_path, os.path.basename(project_path) + '.csv')):
         cols = ['project', 'type', 'ext', 'z', 'y', 'x', 'z_size', 'y_size', 'x_size', 'created_date', 'update_date',
                 'path', 'notes']
         df = pd.DataFrame(index=[], columns=cols)
         filename_pattern_original = os.path.join(project_path, f'dataset/Original_size/Original/*{ext}')
         images_original = dask_image.imread.imread(filename_pattern_original)
         z, y, x = images_original.shape
         record = pd.Series(
-            [os.path.basename(project_path), 'dataset', '.tif', 0, 0, 0, z, y, x, datetime.datetime.now(),
+            [os.path.basename(project_path), 'dataset', '.tif', 0, 0, 0, z, y, x, datetime.now(),
              '', os.path.join(project_path, 'dataset/Original_size/Original'), ''], index=df.columns)
         df = df.append(record, ignore_index=True)
         df.to_csv(os.path.join(project_path, os.path.basename(project_path) + '.csv'))
     else:
         pass
 
 
@@ -101,15 +60,15 @@
     check_zarr(project_path, ext)
     check_annotations_dir(project_path)
 
 
 def load_images(directory):
     filename_pattern_original = os.path.join(directory, '*png')
     images_original = dask_image.imread.imread(filename_pattern_original)
-    renormalized_images_original = dask.array.asarray([ renormalize_8bit(images_original[z]) for z in range(images_original.shape[0]) ])
+    renormalized_images_original = dask.array.asarray([ renormalize_8bit(images_original[z]) for z in range(images_original.shape[0])])
     return renormalized_images_original
 
 
 def load_predicted_masks(mito_mask_dir, er_mask_dir):
     filename_pattern_mito_label = os.path.join(mito_mask_dir, '*png')
     filename_pattern_er_label = os.path.join(er_mask_dir, '*png')
     images_mito_label = dask_image.imread.imread(filename_pattern_mito_label)
@@ -124,22 +83,30 @@
     filename_pattern_label = os.path.join(mod_mask_dir, '*png')
     images_label = dask_image.imread.imread(filename_pattern_label)
     images_label = images_label.compute()
     base_label = images_label
     return base_label, [x.name for x in sorted(list(Path(mod_mask_dir).glob('./*png')))]
 
 
+def load_mask_masks(mask_dir):
+    filename_pattern_label = os.path.join(mask_dir, '*png')
+    images_label = dask_image.imread.imread(filename_pattern_label)
+    if images_label.max() == 1:
+        pass
+    else:
+        images_label = 1 * (images_label > 0)
+    return images_label.compute()
+
 def load_raw_masks(raw_mask_dir):
     filename_pattern_raw = os.path.join(raw_mask_dir, '*png')
     images_raw = dask_image.imread.imread(filename_pattern_raw)
     images_raw = images_raw.compute()
     base_label = np.where((126 < images_raw) & (images_raw < 171), 255, 0)
     return base_label
 
-
 def combine_blocks(block1, block2):
     temp_widget = QWidget()
     temp_layout = QHBoxLayout()
     temp_layout.addWidget(block1)
     temp_layout.addWidget(block2)
     temp_widget.setLayout(temp_layout)
     return temp_widget
@@ -147,15 +114,14 @@
 
 def save_masks(labels, out_path, filenames):
     num = labels.shape[0]
     for i in range(num):
         label = labels[i]
         io.imsave(os.path.join(out_path, filenames[i]), label)
 
-
 def label_and_sort(base_label):
     labeled = ndimage.label(base_label, structure=np.ones((3, 3, 3)))[0]
 
     mks, nums = np.unique(labeled, return_counts=True)
 
     idx_list = list(np.argsort(nums[1:]))
     nums = np.sort(nums[1:])
@@ -214,66 +180,54 @@
     slider_widget = combine_blocks(lbl, object_slider)
     viewer.window.add_dock_widget(slider_widget, name='object_size_slider', area='left')
 
     def calc_object_callback(t_layer, value, labeled_array, nums):
         t_layer.data = label_ct(labeled_array, nums, value)
 
 
-def load_X_gray(folder_path):
-    image_files = []
-    for file in os.listdir(folder_path):
-        base, ext = os.path.splitext(file)
-        if ext == '.png':
-            image_files.append(file)
-        else:
-            pass
-
-    image_files.sort()
-
-    img = cv2.imread(folder_path + os.sep + image_files[0], cv2.IMREAD_GRAYSCALE)
-
-    images = np.zeros((len(image_files), img.shape[0], img.shape[1], 1), np.float32)
-    for i, image_file in tqdm(enumerate(image_files)):
-        image = cv2.imread(folder_path + os.sep + image_file, cv2.IMREAD_GRAYSCALE)
-        image = image[:, :, np.newaxis]
-        images[i] = normalize_x(image)
-
-    print(images.shape)
-
-    return images, image_files
-
-
-def load_Y_gray(folder_path, thresh=None, normalize=False):
-    image_files = []
-    for file in os.listdir(folder_path):
-        base, ext = os.path.splitext(file)
-        if ext == '.png':
-            image_files.append(file)
-        else:
-            pass
-
-    image_files.sort()
-
-    img = cv2.imread(folder_path + os.sep + image_files[0], cv2.IMREAD_GRAYSCALE)
-
-    images = np.zeros((len(image_files), img.shape[0], img.shape[1], 1), np.float32)
-
-    for i, image_file in tqdm(enumerate(image_files)):
-        image = cv2.imread(folder_path + os.sep + image_file, cv2.IMREAD_GRAYSCALE)
-        if thresh:
-            ret, image = cv2.threshold(image, thresh, 255, cv2.THRESH_BINARY)
-        image = image[:, :, np.newaxis]
-        if normalize:
-            images[i] = normalize_y(image)
-        else:
-            images[i] = image
-
-    print(images.shape)
+def preprocess_cristae(ori_path, mito_path, cristae_path, names, crop_size=1000):
+    ori_imgs = [renormalize_8bit(io.imread(os.path.join(ori_path, name), as_gray=True)) for name in names]
+    mito_imgs = [io.imread(os.path.join(mito_path, name), as_gray=True) for name in names]
+    cristae_imgs = [io.imread(os.path.join(cristae_path, name), as_gray=True) for name in names]
+
+    # make gap
+    preprocessed_imgs = []
+    for i in range(len(cristae_imgs)):
+        dilated_cristae_img = morphology.binary_dilation(cristae_imgs[i], morphology.disk(5))
+        dilated_cristae_img = dilated_cristae_img - cristae_imgs[i]
+        dilated_cristae_img = dilated_cristae_img * mito_imgs[i]
+        merged_img = np.concatenate([
+            cristae_imgs[i][..., np.newaxis],
+            dilated_cristae_img[..., np.newaxis],
+            np.zeros_like(cristae_imgs[i][..., np.newaxis])
+        ], axis=-1)
+        preprocessed_imgs.append(merged_img)
+    preprocessed_imgs = np.array(preprocessed_imgs)
+
+    # crop
+    cropped_ori_imgs = []
+    cropped_cristae_imgs = []
+    H = ori_imgs[0].shape[0] // crop_size + 1
+    W = ori_imgs[0].shape[1] // crop_size + 1
+    for z in range(len(ori_imgs)):
+        margin_ori_img = np.zeros((H * crop_size, W * crop_size), ori_imgs[0].dtype)
+        margin_ori_img[:ori_imgs[0].shape[0], :ori_imgs[0].shape[1]] = ori_imgs[z] * mito_imgs[z]
+        margin_label_img = np.zeros((H * crop_size, W * crop_size, preprocessed_imgs.shape[3]), preprocessed_imgs.dtype)
+        margin_label_img[:preprocessed_imgs.shape[1], :preprocessed_imgs.shape[2]] = preprocessed_imgs[z]
+        for h in range(H):
+            for w in range(W):
+                cropped_ori_img = margin_ori_img[h * crop_size:(h + 1) * crop_size, w * crop_size:(w + 1) * crop_size]
+                if np.max(cropped_ori_img) > 0:
+                    cropped_ori_imgs.append(cropped_ori_img)
+                    cropped_label_img = margin_label_img[h * crop_size:(h + 1) * crop_size,
+                                        w * crop_size:(w + 1) * crop_size]
+                    cropped_label_img *= 255
+                    cropped_cristae_imgs.append(cropped_label_img)
 
-    return images, image_files
+    return np.array(cropped_ori_imgs), np.array(cropped_cristae_imgs)
 
 
 def select_train_data(dataframe, ori_imgs, label_imgs, ori_filenames):
     train_img_names = list()
     for node in dataframe.itertuples():
         if node.train == "Checked":
             train_img_names.append(node.filename)
```

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/napari.yaml` & `napari_philow-0.2.0/src/napari_philow/napari.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 name: napari-PHILOW
-schema_version: 0.1.1
+schema_version: 0.2.0
 contributions:
   commands:
   - id: napari-PHILOW.AnnotationMode
     title: Create Annotation Mode
     python_name: napari_philow._annotation:AnnotationMode
   - id: napari-PHILOW.Trainer
     title: Create Trainer
     python_name: napari_philow._trainer:Trainer
   - id: napari-PHILOW.Predicter
     title: Create Predicter
     python_name: napari_philow._prediction:Predicter
   - id: napari-PHILOW.Selector
     title: Create Selector
     python_name: napari_philow._selector:Selector
+
   widgets:
   - command: napari-PHILOW.AnnotationMode
     display_name: Annotation Mode
   - command: napari-PHILOW.Trainer
     display_name: Trainer
   - command: napari-PHILOW.Predicter
     display_name: Predicter
```

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/segmentation/data_augmentation.py` & `napari_philow-0.2.0/src/napari_philow/segmentation/data_augmentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,26 @@
         img = img.rotate(rotate_angle, Image.BILINEAR)
         anno_class_img = anno_class_img.rotate(rotate_angle, Image.NEAREST)
 
         return img, anno_class_img
 
 
 class RandomBrightness(object):
-    def __call__(self, img, anno_class_img):
-        return transforms.ColorJitter(brightness=0.5)(img), anno_class_img
+    def __call__(self, img, mask):
+        """
+        Args:
+            img (PIL Image or Tensor):
+            mask (PIL Image or Tensor):
+        Returns:
+            Tuple of PIL Image or Tensor: Transformed image and mask
+        """
+        if np.random.randint(2):
+            brightness_factor = np.random.default_rng().uniform(0.5,1.5)
+            img = functional.adjust_brightness(img, brightness_factor)
+        return img, mask
 
 
 class RandomCrop(object):
     """randomにcropするクラス"""
 
     def __init__(self, size):
         self.size = size
```

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/segmentation/loss.py` & `napari_philow-0.2.0/src/napari_philow/segmentation/loss.py`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/segmentation/predict.py` & `napari_philow-0.2.0/src/napari_philow/segmentation/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from torchvision.transforms import functional
 from tqdm import tqdm
 
 from .utils import add_margin
 
 
-def pred_large_image(image, net, device, size):
+def pred_large_image(image, net, device, size, is_3class=False):
     """
     predict large image
     Args:
         image (PIL image): input image
         net (torch.nn.Module): model
         device (str): e.g. 'cpu', 'cuda:0'
         size (int):  patch size
@@ -32,31 +32,42 @@
         else:
             by = int(y % ps / 2) + ms
         if x < size:
             bx = int(x % ps / 2) + ms + size - x
         else:
             bx = int(x % ps / 2) + ms
         temp_image = add_margin(image, by, bx, by, bx, 'black')
-        temp_label = np.zeros((y + by * 2, x + bx * 2), np.float32)
+        if is_3class:
+            temp_label = np.zeros((y + by * 2, x + bx * 2, 3), np.float32)
+        else:
+            temp_label = np.zeros((y + by * 2, x + bx * 2), np.float32)
         row = (y + by * 2) // ds - 1
         col = (x + bx * 2) // ds - 1
         for r in range(row):
             for c in range(col):
                 temp = temp_image.crop((c * ds, r * ds, c * ds + ps, r * ds + ps))
                 temp = functional.to_tensor(temp).unsqueeze(0).to(device)
                 pred = net(temp).cpu().detach().numpy()
-                temp_label[r * ds + ms:r * ds + ps - ms, c * ds + ms:c * ds + ps - ms] = pred[0, 0, ms:ps - ms,
-                                                                                         ms:ps - ms]
+                if is_3class:
+                    temp_label[r * ds + ms : r * ds + ps - ms, c * ds + ms : c * ds + ps - ms] \
+                        = pred.transpose(0, 2, 3, 1)[0, ms:ps - ms, ms:ps - ms]
+                else:
+                    temp_label[r * ds + ms:r * ds + ps - ms, c * ds + ms:c * ds + ps - ms] \
+                        = pred[0, 0, ms:ps - ms, ms:ps - ms]
+
         return temp_label[by:y + by, bx:x + bx]
     else:
         if x < size:
             dx = size - x
         else:
             dx = 0
         if y < size:
             dy = size - y
         else:
             dy = 0
         image = add_margin(image, math.floor(dy / 2), math.floor(dx / 2), math.ceil(dy / 2), math.ceil(dx / 2), 'black')
         temp = functional.to_tensor(image).unsqueeze(0).to(device)
         pred = net(temp).cpu().detach().numpy()
-        return pred[0, 0, math.floor(dy / 2):math.floor(dy / 2) + y, math.floor(dx / 2):math.floor(dx / 2) + x]
+        if is_3class:
+            return pred.transpose(0, 2, 3, 1)[0, math.floor(dy / 2):math.floor(dy / 2) + y, math.floor(dx / 2):math.floor(dx / 2) + x]
+        else:
+            return pred[0, 0, math.floor(dy / 2):math.floor(dy / 2) + y, math.floor(dx / 2):math.floor(dx / 2) + x]
```

### Comparing `napari-PHILOW-0.1.1/src/napari_philow/segmentation/train.py` & `napari_philow-0.2.0/src/napari_philow/segmentation/train.py`

 * *Files identical despite different names*


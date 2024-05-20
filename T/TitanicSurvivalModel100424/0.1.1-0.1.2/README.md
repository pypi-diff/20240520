# Comparing `tmp/titanicsurvivalmodel100424-0.1.1.tar.gz` & `tmp/titanicsurvivalmodel100424-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanicsurvivalmodel100424-0.1.1.tar", last modified: Sat May 18 07:36:23 2024, max compression
+gzip compressed data, was "titanicsurvivalmodel100424-0.1.2.tar", last modified: Mon May 20 01:57:13 2024, max compression
```

## Comparing `titanicsurvivalmodel100424-0.1.1.tar` & `titanicsurvivalmodel100424-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.901917 titanicsurvivalmodel100424-0.1.1/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      482 2024-05-09 06:18:45.000000 titanicsurvivalmodel100424-0.1.1/MANIFEST.in
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-18 07:36:23.901518 titanicsurvivalmodel100424-0.1.1/PKG-INFO
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.901010 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/PKG-INFO
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1022 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/SOURCES.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)        1 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/dependency_links.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)      188 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/requires.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       21 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/top_level.txt
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.897710 titanicsurvivalmodel100424-0.1.1/classification_model/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        6 2024-05-18 07:34:56.000000 titanicsurvivalmodel100424-0.1.1/classification_model/VERSION
--rw-r--r--   0 ongzhicong   (501) staff       (20)      862 2024-05-04 09:04:59.000000 titanicsurvivalmodel100424-0.1.1/classification_model/__init__.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.898157 titanicsurvivalmodel100424-0.1.1/classification_model/config/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:23.000000 titanicsurvivalmodel100424-0.1.1/classification_model/config/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     2128 2024-05-17 09:35:46.000000 titanicsurvivalmodel100424-0.1.1/classification_model/config/core.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      899 2024-05-17 08:13:51.000000 titanicsurvivalmodel100424-0.1.1/classification_model/config.yml
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.898398 titanicsurvivalmodel100424-0.1.1/classification_model/datasets/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:51.000000 titanicsurvivalmodel100424-0.1.1/classification_model/datasets/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     2434 2024-05-17 06:12:30.000000 titanicsurvivalmodel100424-0.1.1/classification_model/pipeline.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1058 2024-05-18 07:00:50.000000 titanicsurvivalmodel100424-0.1.1/classification_model/predict.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.899236 titanicsurvivalmodel100424-0.1.1/classification_model/processing/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:58.000000 titanicsurvivalmodel100424-0.1.1/classification_model/processing/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1750 2024-05-18 06:45:19.000000 titanicsurvivalmodel100424-0.1.1/classification_model/processing/data_manager.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     3575 2024-05-17 06:26:00.000000 titanicsurvivalmodel100424-0.1.1/classification_model/processing/features.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1763 2024-05-18 07:29:10.000000 titanicsurvivalmodel100424-0.1.1/classification_model/processing/validation.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      831 2024-05-17 06:24:46.000000 titanicsurvivalmodel100424-0.1.1/classification_model/train_pipeline.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.899966 titanicsurvivalmodel100424-0.1.1/classification_model/trained_models/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:09:07.000000 titanicsurvivalmodel100424-0.1.1/classification_model/trained_models/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     4110 2024-05-18 06:53:30.000000 titanicsurvivalmodel100424-0.1.1/classification_model/trained_models/classification_model_output_v0.1.0.pkl
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1914 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.1/pyproject.toml
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.894538 titanicsurvivalmodel100424-0.1.1/requirements/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      225 2024-05-17 09:24:00.000000 titanicsurvivalmodel100424-0.1.1/requirements/requirements.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       65 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.1/requirements/test_requirements.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       38 2024-05-18 07:36:23.901998 titanicsurvivalmodel100424-0.1.1/setup.cfg
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1996 2024-05-10 07:40:06.000000 titanicsurvivalmodel100424-0.1.1/setup.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.900703 titanicsurvivalmodel100424-0.1.1/tests/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      680 2024-05-14 08:58:22.000000 titanicsurvivalmodel100424-0.1.1/tests/test_features.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      855 2024-05-14 08:58:29.000000 titanicsurvivalmodel100424-0.1.1/tests/test_prediction.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.138573 titanicsurvivalmodel100424-0.1.2/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      482 2024-05-09 06:18:45.000000 titanicsurvivalmodel100424-0.1.2/MANIFEST.in
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-20 01:57:13.138269 titanicsurvivalmodel100424-0.1.2/PKG-INFO
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.137906 titanicsurvivalmodel100424-0.1.2/TitanicSurvivalModel100424.egg-info/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-20 01:57:13.000000 titanicsurvivalmodel100424-0.1.2/TitanicSurvivalModel100424.egg-info/PKG-INFO
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1022 2024-05-20 01:57:13.000000 titanicsurvivalmodel100424-0.1.2/TitanicSurvivalModel100424.egg-info/SOURCES.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        1 2024-05-20 01:57:13.000000 titanicsurvivalmodel100424-0.1.2/TitanicSurvivalModel100424.egg-info/dependency_links.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      188 2024-05-20 01:57:13.000000 titanicsurvivalmodel100424-0.1.2/TitanicSurvivalModel100424.egg-info/requires.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       21 2024-05-20 01:57:13.000000 titanicsurvivalmodel100424-0.1.2/TitanicSurvivalModel100424.egg-info/top_level.txt
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.135074 titanicsurvivalmodel100424-0.1.2/classification_model/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        6 2024-05-20 01:54:44.000000 titanicsurvivalmodel100424-0.1.2/classification_model/VERSION
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      862 2024-05-04 09:04:59.000000 titanicsurvivalmodel100424-0.1.2/classification_model/__init__.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.135395 titanicsurvivalmodel100424-0.1.2/classification_model/config/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:23.000000 titanicsurvivalmodel100424-0.1.2/classification_model/config/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     2129 2024-05-20 00:42:53.000000 titanicsurvivalmodel100424-0.1.2/classification_model/config/core.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      899 2024-05-17 08:13:51.000000 titanicsurvivalmodel100424-0.1.2/classification_model/config.yml
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.135594 titanicsurvivalmodel100424-0.1.2/classification_model/datasets/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:51.000000 titanicsurvivalmodel100424-0.1.2/classification_model/datasets/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     2434 2024-05-17 06:12:30.000000 titanicsurvivalmodel100424-0.1.2/classification_model/pipeline.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1058 2024-05-18 07:00:50.000000 titanicsurvivalmodel100424-0.1.2/classification_model/predict.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.136603 titanicsurvivalmodel100424-0.1.2/classification_model/processing/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:58.000000 titanicsurvivalmodel100424-0.1.2/classification_model/processing/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1766 2024-05-20 01:48:26.000000 titanicsurvivalmodel100424-0.1.2/classification_model/processing/data_manager.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     3575 2024-05-17 06:26:00.000000 titanicsurvivalmodel100424-0.1.2/classification_model/processing/features.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1763 2024-05-18 07:29:10.000000 titanicsurvivalmodel100424-0.1.2/classification_model/processing/validation.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      831 2024-05-17 06:24:46.000000 titanicsurvivalmodel100424-0.1.2/classification_model/train_pipeline.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.136934 titanicsurvivalmodel100424-0.1.2/classification_model/trained_models/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:09:07.000000 titanicsurvivalmodel100424-0.1.2/classification_model/trained_models/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     4110 2024-05-20 01:54:58.000000 titanicsurvivalmodel100424-0.1.2/classification_model/trained_models/classification_model_output_v0.1.2.pkl
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1914 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.2/pyproject.toml
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.132474 titanicsurvivalmodel100424-0.1.2/requirements/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      225 2024-05-17 09:24:00.000000 titanicsurvivalmodel100424-0.1.2/requirements/requirements.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       65 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.2/requirements/test_requirements.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       38 2024-05-20 01:57:13.138627 titanicsurvivalmodel100424-0.1.2/setup.cfg
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1997 2024-05-20 01:46:16.000000 titanicsurvivalmodel100424-0.1.2/setup.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 01:57:13.137574 titanicsurvivalmodel100424-0.1.2/tests/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      680 2024-05-14 08:58:22.000000 titanicsurvivalmodel100424-0.1.2/tests/test_features.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      855 2024-05-14 08:58:29.000000 titanicsurvivalmodel100424-0.1.2/tests/test_prediction.py
```

### Comparing `titanicsurvivalmodel100424-0.1.1/PKG-INFO` & `titanicsurvivalmodel100424-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanicSurvivalModel100424
-Version: 0.1.1
+Version: 0.1.2
 Summary: sample Classification model package.
 Home-page: https://github.com/zong006/model_packaging
 Author: sample_author
 Author-email: sample_email@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/PKG-INFO` & `titanicsurvivalmodel100424-0.1.2/TitanicSurvivalModel100424.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanicSurvivalModel100424
-Version: 0.1.1
+Version: 0.1.2
 Summary: sample Classification model package.
 Home-page: https://github.com/zong006/model_packaging
 Author: sample_author
 Author-email: sample_email@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/SOURCES.txt` & `titanicsurvivalmodel100424-0.1.2/TitanicSurvivalModel100424.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 classification_model/config/core.py
 classification_model/datasets/__init__.py
 classification_model/processing/__init__.py
 classification_model/processing/data_manager.py
 classification_model/processing/features.py
 classification_model/processing/validation.py
 classification_model/trained_models/__init__.py
-classification_model/trained_models/classification_model_output_v0.1.0.pkl
+classification_model/trained_models/classification_model_output_v0.1.2.pkl
 tests/test_features.py
 tests/test_prediction.py
```

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/__init__.py` & `titanicsurvivalmodel100424-0.1.2/classification_model/__init__.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/config/core.py` & `titanicsurvivalmodel100424-0.1.2/classification_model/config/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import List, Optional
 
 from pydantic import BaseModel
 from strictyaml import YAML, load
 
-script_path = Path(__file__).resolve().parent
+script_path = Path(__file__).resolve().parent 
 
 PACKAGE_ROOT = script_path.parent
 ROOT = PACKAGE_ROOT.parent
 CONFIG_FILE_PATH = PACKAGE_ROOT / "config.yml"
 DATASET_DIR = PACKAGE_ROOT / "datasets"
 TRAINED_MODEL_DIR = PACKAGE_ROOT / "trained_models"
```

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/config.yml` & `titanicsurvivalmodel100424-0.1.2/classification_model/config.yml`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/pipeline.py` & `titanicsurvivalmodel100424-0.1.2/classification_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/predict.py` & `titanicsurvivalmodel100424-0.1.2/classification_model/predict.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/processing/data_manager.py` & `titanicsurvivalmodel100424-0.1.2/classification_model/processing/data_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,7 +49,9 @@
     mapping between the package version and the model
     version to be imported and used by other applications.
     """
     do_not_delete = files_to_keep + ["__init__.py"]
     for model_file in TRAINED_MODEL_DIR.iterdir():
         if model_file.name not in do_not_delete:
             model_file.unlink()
+
+print(_version)
```

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/processing/features.py` & `titanicsurvivalmodel100424-0.1.2/classification_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/processing/validation.py` & `titanicsurvivalmodel100424-0.1.2/classification_model/processing/validation.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/train_pipeline.py` & `titanicsurvivalmodel100424-0.1.2/classification_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/classification_model/trained_models/classification_model_output_v0.1.0.pkl` & `titanicsurvivalmodel100424-0.1.2/classification_model/trained_models/classification_model_output_v0.1.2.pkl`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/pyproject.toml` & `titanicsurvivalmodel100424-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/setup.py` & `titanicsurvivalmodel100424-0.1.2/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-)
+)
```

### Comparing `titanicsurvivalmodel100424-0.1.1/tests/test_features.py` & `titanicsurvivalmodel100424-0.1.2/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.1/tests/test_prediction.py` & `titanicsurvivalmodel100424-0.1.2/tests/test_prediction.py`

 * *Files identical despite different names*


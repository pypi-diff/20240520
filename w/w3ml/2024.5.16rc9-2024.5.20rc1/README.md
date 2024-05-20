# Comparing `tmp/w3ml-2024.5.16rc9.tar.gz` & `tmp/w3ml-2024.5.20rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/w3ml-2024.5.16rc9.tar", last modified: Thu May 16 05:27:01 2024, max compression
+gzip compressed data, was "w3ml-2024.5.20rc1.tar", last modified: Mon May 20 04:13:11 2024, max compression
```

## Comparing `w3ml-2024.5.16rc9.tar` & `w3ml-2024.5.20rc1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/automl_multilabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/automl_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/automl_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:13:11.013291 w3ml-2024.5.20rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 04:13:11.013291 w3ml-2024.5.20rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 04:13:11.013291 w3ml-2024.5.20rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:13:11.009291 w3ml-2024.5.20rc1/w3ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/w3ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:13:11.009291 w3ml-2024.5.20rc1/w3ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/w3ml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:13:11.009291 w3ml-2024.5.20rc1/w3ml/models/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/w3ml/models/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/w3ml/models/contrib/automl_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/w3ml/models/contrib/automl_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/w3ml/models/contrib/automl_multilabel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:13:11.009291 w3ml-2024.5.20rc1/w3ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/w3ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-20 04:13:02.000000 w3ml-2024.5.20rc1/w3ml/utils/automl_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:13:11.013291 w3ml-2024.5.20rc1/w3ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 04:13:10.000000 w3ml-2024.5.20rc1/w3ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 04:13:11.000000 w3ml-2024.5.20rc1/w3ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 04:13:10.000000 w3ml-2024.5.20rc1/w3ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 04:13:10.000000 w3ml-2024.5.20rc1/w3ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 04:13:10.000000 w3ml-2024.5.20rc1/w3ml.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `w3ml-2024.5.16rc9/setup.py` & `w3ml-2024.5.20rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     install_requires=[
-        "autogluon.tabular==0.5.0",
+        "autogluon==0.5.0",
         "numpy<1.23,>=1.21",
     ],
 )
```

### Comparing `w3ml-2024.5.16rc9/w3ml/models/contrib/automl_multilabel.py` & `w3ml-2024.5.20rc1/w3ml/models/contrib/automl_multilabel.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc9/w3ml/models/contrib/automl_binary.py` & `w3ml-2024.5.20rc1/w3ml/models/contrib/automl_binary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import shutil
 from pathlib import Path
 from typing import Dict, List
 
 import pandas as pd
 from autogluon.tabular import TabularPredictor
 
 MODEL_DIR = Path.home().joinpath("w3ml_models")
@@ -23,14 +24,15 @@
         excluded_model_types: List[str] = [
             "FASTTEXT",
             "AG_TEXT_NN",
             "TRANSF",
             "custom",
         ],
         keep_only_best =True,
+        overwrite=True,
     ):
         """
         2024.06.01 v1 개발
         Contact : 이규남(kyunam@sk.com), 김태형(th0804@sk.com), 강예진(yejin.k@sk.com), 정유철(jungyc@sk.com), 진기훈(kh.jin@sk.com), 송지영(jiyoung.song@sk.com)
 
         AutoML을 통해 모델을 학습합니다.
         Class의 개수는 Multi가 아니라 2개 까지 지원합니다. 3개 이상의 Class는 타 함수를 참조바랍니다.
@@ -92,32 +94,49 @@
         else:
             assert isinstance(path, str), "`path(는) str 타입이어야 합니다.`"
             self.path = path
 
         assert isinstance(presets, str), "`presets(는) str 타입이어야 합니다.`"
         assert presets in ['best_quality', 'high_quality', 'good_quality', 'medium_quality', 'optimize_for_deployment']
         
-        assert isinstance(keep_only_best, bool), "`presets(는) str 타입이어야 합니다.`"
+        assert isinstance(keep_only_best, bool), "`keep_only_best(는) bool 타입이어야 합니다.`"
+        assert isinstance(overwrite, bool), "`overwrite(는) bool 타입이어야 합니다.`"
         
         self.presets = presets
         self.train_data = train_data
         self.label = label
         self.non_training_features = non_training_features
         self.eval_metric = eval_metric
         self.time_limit = time_limit
         self.excluded_model_types = excluded_model_types
         self.keep_only_best = keep_only_best
+        self.overwrite = overwrite
 
     def fit(self):
-        try:
-            self.models = self._fit()
-            os.rmdir(self.path)
-        except Exception as e:
-            os.rmdir(self.path)
-            raise Exception(f"Error occured : {e}")
+        if self.overwrite == True:
+            if os.path.isdir(self.path):
+                shutil.rmtree(self.path)
+                try:
+                    self.models = self._fit()
+                except Exception as e:
+                    raise Exception(f"Error occured : {e}")
+            else:
+                try:
+                    self.models = self._fit()
+                except Exception as e:
+                    raise Exception(f"Error occured : {e}")
+        else:
+            if os.path.isdir(self.path):
+                raise Exception(f"Error occured : 이미 {self.path} 디렉토리가 존재합니다.")
+            else:
+                try:
+                    self.models = self._fit()
+                except Exception as e:
+                    raise Exception(f"Error occured : {e}")
+            
             
     def _fit(self):
         columns = [
             f for f in self.train_data.columns if f not in self.non_training_features
         ]
         predictor = TabularPredictor(
             label=self.label,
```

### Comparing `w3ml-2024.5.16rc9/w3ml/models/contrib/automl_multiclass.py` & `w3ml-2024.5.20rc1/w3ml/models/contrib/automl_multiclass.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc9/LICENSE` & `w3ml-2024.5.20rc1/LICENSE`

 * *Files identical despite different names*


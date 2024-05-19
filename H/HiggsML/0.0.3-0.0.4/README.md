# Comparing `tmp/higgsml-0.0.3.tar.gz` & `tmp/higgsml-0.0.4.tar.gz`

## Comparing `higgsml-0.0.3.tar` & `higgsml-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/__init__.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/datasets.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/ingestion.py
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/score.py
--rw-r--r--   0        0        0    20116 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/systematics.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.3/HiggsML/visualization.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.3/LICENSE
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 higgsml-0.0.3/README.md
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 higgsml-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 higgsml-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 higgsml-0.0.4/HiggsML/__init__.py
+-rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 higgsml-0.0.4/HiggsML/datasets.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 higgsml-0.0.4/HiggsML/ingestion.py
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 higgsml-0.0.4/HiggsML/score.py
+-rw-r--r--   0        0        0    20116 2020-02-02 00:00:00.000000 higgsml-0.0.4/HiggsML/systematics.py
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 higgsml-0.0.4/HiggsML/visualization.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 higgsml-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 higgsml-0.0.4/LICENSE
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 higgsml-0.0.4/README.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 higgsml-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 higgsml-0.0.4/PKG-INFO
```

### Comparing `higgsml-0.0.3/HiggsML/datasets.py` & `higgsml-0.0.4/HiggsML/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from frozendict import frozendict
 import numpy as np
 import pandas as pd
 import json
 import os
 import subprocess
+import wget
 
 
 test_set_settings = None
 
 
 class Data:
 
@@ -159,36 +160,30 @@
     ):
         from systematics import systematics
 
         if self.__train_set is None:
             self.load_train_set()
         return systematics(self.__train_set, tes, jes, soft_met, w_scale, bkg_scale)
 
-
-current_path = os.path.dirname(os.path.realpath(__file__))
-
+current_path = os.getcwd()
 
 def Neurips2024_public_dataset():
 
     file_read_loc = os.path.join(current_path, "public_data")
     if not os.path.isdir(file_read_loc):
         os.mkdir(file_read_loc)
-        
+
     file = "public_data.zip"
     if file not in os.listdir(file_read_loc):
-        subprocess.run(
-            [
-                "wget",
-                "-O",
-                os.path.join(file_read_loc, "public_data.zip"),
-                "https://www.codabench.org/datasets/download/c3b5c664-2f7e-4e81-8975-7926dae44703/",
-            ]
+        wget.download(
+            "https://www.codabench.org/datasets/download/c3b5c664-2f7e-4e81-8975-7926dae44703/",
+            out=os.path.join(file_read_loc, "public_data.zip"),
         )
 
-    if "public_data" not in os.listdir(file_read_loc):
+    if "input_data" not in os.listdir(file_read_loc):
         subprocess.run(
             ["unzip", os.path.join(file_read_loc, file), "-d", file_read_loc]
         )
 
     return Data(
         os.path.join(current_path, "public_data", "input_data"), data_format="parquet"
     )
```

### Comparing `higgsml-0.0.3/HiggsML/ingestion.py` & `higgsml-0.0.4/HiggsML/ingestion.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.3/HiggsML/score.py` & `higgsml-0.0.4/HiggsML/score.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.3/HiggsML/systematics.py` & `higgsml-0.0.4/HiggsML/systematics.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.3/HiggsML/visualization.py` & `higgsml-0.0.4/HiggsML/visualization.py`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.3/.gitignore` & `higgsml-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.3/LICENSE` & `higgsml-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `higgsml-0.0.3/pyproject.toml` & `higgsml-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HiggsML"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ragansu Chakkappai", email="ragansu.chakkappai@universite-paris-saclay.fr"},
   { name="David Rousseau", email="david.rousseau@uijclab.in2p3.fr" },
   { name="V. Estrade", email="v.estrade@centralesupelec.fr" },
   { name="Ihsan Ullah", email="ihsan.ullah@universite-paris-saclay.fr"}
 ]
 description = "A Black Swan test package"
@@ -19,28 +19,30 @@
     "numpy",
     "pandas",
     "scikit-learn",
     "matplotlib",
     "seaborn",
     "frozendict",
     "pyarrow",
+    "wget",
     "setuptools"
 ]
 install_requires=["numpy>=1.26.4",
                   "sklearn>=1.4.2",
                   "pandas>=2.2.2",
                   "matplotlib>=3.8.0",
                   "seaborn>=0.13.1",
                   "frozendict>=2.4.4",
                   "pyarrow>=15.0.0",
+                  "wget>=3.2",
                   "setuptools>=58.2.0"
                   ]
 
 
 
 [build-system]
-requires = ["hatchling", "numpy", "pandas", "scikit-learn", "matplotlib", "seaborn", "frozendict", "pyarrow", "setuptools"]
+requires = ["hatchling", "numpy", "pandas", "scikit-learn", "matplotlib", "seaborn", "frozendict", "pyarrow","wget", "setuptools"]
 build-backend = "hatchling.build"
 
 [project.urls]
 Homepage = "https://github.com/blackSwanCS/black_swan_pkg"
 Issues = "https://github.com/blackSwanCS/black_swan_pkg/issues"
```

### Comparing `higgsml-0.0.3/PKG-INFO` & `higgsml-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: HiggsML
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Black Swan test package
 Project-URL: Homepage, https://github.com/blackSwanCS/black_swan_pkg
 Project-URL: Issues, https://github.com/blackSwanCS/black_swan_pkg/issues
 Author-email: Ragansu Chakkappai <ragansu.chakkappai@universite-paris-saclay.fr>, David Rousseau <david.rousseau@uijclab.in2p3.fr>, "V. Estrade" <v.estrade@centralesupelec.fr>, Ihsan Ullah <ihsan.ullah@universite-paris-saclay.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: scikit-learn
 Requires-Dist: seaborn
 Requires-Dist: setuptools
+Requires-Dist: wget
 Description-Content-Type: text/markdown
 
 # HiggsML BlackSwan Package
 
 you can install this package by 
 ```shell
 pip install HiggsML
```


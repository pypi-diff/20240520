# Comparing `tmp/mimllearning-0.5.4.tar.gz` & `tmp/mimllearning-0.5.5.tar.gz`

## Comparing `mimllearning-0.5.4.tar` & `mimllearning-0.5.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.4/readme.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mimllearning-0.5.4/todo.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.4/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mi/mi_wrapper_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/data/bag.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/data/instance.py
--rw-r--r--   0        0        0    21354 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/datasets/dataset_utils.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/report/__init__.py
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/tutorial/classifiers_mimltomi.ipynb
--rw-r--r--   0        0        0    15720 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/tutorial/classifiers_mimltoml.ipynb
--rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/tutorial/data_miml.ipynb
--rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/tutorial/train_test_experiment_miml.ipynb
--rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 mimllearning-0.5.4/src/miml/tutorial/transformations_miml.ipynb
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.4/LICENSE.txt
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.4/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.5/readme.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mimllearning-0.5.5/todo.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.5/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mi/mi_wrapper_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/data/instance.py
+-rw-r--r--   0        0        0    21354 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     6642 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/tutorial/classifiers_mimltomi.ipynb
+-rw-r--r--   0        0        0    15720 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/tutorial/classifiers_mimltoml.ipynb
+-rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/tutorial/data_miml.ipynb
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/tutorial/train_test_experiment_miml.ipynb
+-rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 mimllearning-0.5.5/src/miml/tutorial/transformations_miml.ipynb
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.5/LICENSE.txt
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.5/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.5/PKG-INFO
```

### Comparing `mimllearning-0.5.4/readme.md` & `mimllearning-0.5.5/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.5.5/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/classifier/miml_classifier.py` & `mimllearning-0.5.5/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.5.5/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/classifier/mi/mi_wrapper_classifier.py` & `mimllearning-0.5.5/src/miml/classifier/mi/mi_wrapper_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.5.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.5.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-0.5.5/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.5.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/data/bag.py` & `mimllearning-0.5.5/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/data/instance.py` & `mimllearning-0.5.5/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/data/miml_dataset.py` & `mimllearning-0.5.5/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/datasets/dataset_utils.py` & `mimllearning-0.5.5/src/miml/datasets/dataset_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,29 @@
     """
     Function to load a dataset
 
     Parameters
     ----------
     file : str
         Path of the dataset file
+    from_library : bool, default = False
+        Boolean value to load datasets from library
 
     Returns
     ----------
     dataset : MIMLDataset
         Dataset loaded
     """
     if from_library:
         library_datasets = ["toy.arff", "miml_birds.arff", "miml_birds_random_20train.arff",
                             "miml_birds_random_20test.arff"]
         if file in library_datasets:
             return load_dataset(pkg_resources.resource_filename('miml', 'datasets/'+file))
         else:
-            raise Exception("Datasets availables from library are: "+str(library_datasets))
+            raise Exception("Datasets available from library are: "+str(library_datasets))
 
     if file[-4:] == ".csv":
         return load_dataset_csv(file)
     elif file[-5:] == ".arff":
         return load_dataset_arff(file)
     else:
         raise Exception("Filetype is not admitted. You should use an .arff or .csv file")
```

### Comparing `mimllearning-0.5.4/src/miml/datasets/miml_birds.arff` & `mimllearning-0.5.5/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/datasets/miml_birds.csv` & `mimllearning-0.5.5/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.5.5/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.5.5/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/report/report.py` & `mimllearning-0.5.5/src/miml/report/report.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/test/data_test.py` & `mimllearning-0.5.5/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.5.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-0.5.5/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.5.5/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.5.5/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.5.5/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/tutorial/classifiers_mimltomi.ipynb` & `mimllearning-0.5.5/src/miml/tutorial/classifiers_mimltomi.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/tutorial/classifiers_mimltoml.ipynb` & `mimllearning-0.5.5/src/miml/tutorial/classifiers_mimltoml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/tutorial/data_miml.ipynb` & `mimllearning-0.5.5/src/miml/tutorial/data_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/tutorial/train_test_experiment_miml.ipynb` & `mimllearning-0.5.5/src/miml/tutorial/train_test_experiment_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/src/miml/tutorial/transformations_miml.ipynb` & `mimllearning-0.5.5/src/miml/tutorial/transformations_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/LICENSE.txt` & `mimllearning-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/README.md` & `mimllearning-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.4/pyproject.toml` & `mimllearning-0.5.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.5.4"
+version = "0.5.5"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 license = "GPL-3.0"
 keywords = ["machine-learning", "python", "data-science", "miml", "multilabel", "multi-instance"]
 readme = "README.md"
```

### Comparing `mimllearning-0.5.4/PKG-INFO` & `mimllearning-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.5.4
+Version: 0.5.5
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE.txt
 Keywords: data-science,machine-learning,miml,multi-instance,multilabel,python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```


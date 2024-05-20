# Comparing `tmp/mimllearning-0.5.2.tar.gz` & `tmp/mimllearning-0.5.3.tar.gz`

## Comparing `mimllearning-0.5.2.tar` & `mimllearning-0.5.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.2/readme.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mimllearning-0.5.2/todo.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.2/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mi/mi_wrapper_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/data/bag.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/data/instance.py
--rw-r--r--   0        0        0    21354 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/dataset_utils.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/report/__init__.py
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/tutorial/classifiers_mimltoml.ipynb
--rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/tutorial/data_miml.ipynb
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/tutorial/transformations_miml.ipynb
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.2/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.3/readme.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mimllearning-0.5.3/todo.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.3/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mi/mi_wrapper_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/data/instance.py
+-rw-r--r--   0        0        0    21354 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/tutorial/classifiers_mimltomi.ipynb
+-rw-r--r--   0        0        0    15720 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/tutorial/classifiers_mimltoml.ipynb
+-rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/tutorial/data_miml.ipynb
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/tutorial/train_test_experiment_miml.ipynb
+-rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 mimllearning-0.5.3/src/miml/tutorial/transformations_miml.ipynb
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.3/LICENSE.txt
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.3/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.3/PKG-INFO
```

### Comparing `mimllearning-0.5.2/readme.md` & `mimllearning-0.5.3/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.5.3/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/classifier/miml_classifier.py` & `mimllearning-0.5.3/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.5.3/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/classifier/mi/mi_wrapper_classifier.py` & `mimllearning-0.5.3/src/miml/classifier/mi/mi_wrapper_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.5.3/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.5.3/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-0.5.3/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.5.3/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/data/bag.py` & `mimllearning-0.5.3/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/data/instance.py` & `mimllearning-0.5.3/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/data/miml_dataset.py` & `mimllearning-0.5.3/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/datasets/dataset_utils.py` & `mimllearning-0.5.3/src/miml/datasets/dataset_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,36 @@
 import pkg_resources
 
 from ..data.bag import Bag
 from ..data.instance import Instance
 from ..data.miml_dataset import MIMLDataset
 
 
-def load_dataset(file: str) -> MIMLDataset:
+def load_dataset(file: str, from_library: bool = False) -> MIMLDataset:
     """
     Function to load a dataset
 
     Parameters
     ----------
     file : str
         Path of the dataset file
 
     Returns
     ----------
     dataset : MIMLDataset
         Dataset loaded
     """
+    if from_library:
+        library_datasets = ["toy.arff", "miml_birds.arff", "miml_birds_random_20train.arff",
+                            "miml_birds_random_20test.arff"]
+        if file in library_datasets:
+            return load_dataset(pkg_resources.resource_filename('miml', 'datasets/'+file))
+        else:
+            raise Exception("Datasets availables from library are: "+str(library_datasets))
+
     if file[-4:] == ".csv":
         return load_dataset_csv(file)
     elif file[-5:] == ".arff":
         return load_dataset_arff(file)
     else:
         raise Exception("Filetype is not admitted. You should use an .arff or .csv file")
 
@@ -146,63 +154,14 @@
                     bag.add_instance(instance)
                     dataset.add_bag(bag)
                 else:
                     dataset.add_instance(key, instance)
 
     return dataset
 
-
-def load_toy():
-    """
-    Load toy dataset from package
-
-    Returns
-    ----------
-    dataset : MIMLDataset
-        Dataset loaded
-    """
-    return load_dataset(pkg_resources.resource_filename('miml', 'datasets/toy.arff'))
-
-
-def load_birds():
-    """
-    Load birds dataset from package
-
-    Returns
-    ----------
-    dataset : MIMLDataset
-        Dataset loaded
-    """
-    return load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds.arff'))
-
-
-def load_birds_train():
-    """
-    Load a train partition of birds dataset from package
-
-    Returns
-    ----------
-    dataset : MIMLDataset
-        Dataset loaded
-    """
-    return load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_80train.arff'))
-
-
-def load_birds_test():
-    """
-    Load a test partition of birds dataset from package
-
-    Returns
-    ----------
-    dataset : MIMLDataset
-        Dataset loaded
-    """
-    return load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_20test.arff'))
-
-
 def arff_to_csv(file: str) -> None:
     """
     Convert MIML Arff to CSV.
 
     Parameters
     ----------
     file : str
```

### Comparing `mimllearning-0.5.2/src/miml/datasets/miml_birds.arff` & `mimllearning-0.5.3/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/datasets/miml_birds.csv` & `mimllearning-0.5.3/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.5.3/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.5.3/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/report/report.py` & `mimllearning-0.5.3/src/miml/report/report.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/test/data_test.py` & `mimllearning-0.5.3/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.5.3/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-0.5.3/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.5.3/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.5.3/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.5.3/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/src/miml/tutorial/demo.ipynb` & `mimllearning-0.5.3/src/miml/tutorial/train_test_experiment_miml.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9410978835978836%*

 * *Differences: {"'cells'": "{0: {'source': ['<a "*

 * *            'href="https://colab.research.google.com/github/p82maavd/MIML/blob/main/src/miml/tutorial/train_test_experiment_miml.ipynb" '*

 * *            'target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" '*

 * *            'alt="Open In Colab"/></a>\']}, 2: {\'source\': [\'!pip install mimllearning\']}, 4: '*

 * *            '{\'source\': {insert: [(3, \'# dataset = load_dataset("miml_birds.csv"))\\n\'), (4, '*

 * *            "'# dataset = "*

 * *            ' […]*

```diff
@@ -3,15 +3,15 @@
         {
             "cell_type": "markdown",
             "metadata": {
                 "colab_type": "text",
                 "id": "view-in-github"
             },
             "source": [
-                "<a href=\"https://colab.research.google.com/github/p82maavd/MIML/blob/main/src/miml/tutorial/demo.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
+                "<a href=\"https://colab.research.google.com/github/p82maavd/MIML/blob/main/src/miml/tutorial/train_test_experiment_miml.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "UwOvUSvR-8Sm"
             },
@@ -23,18 +23,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "jZMmibMJcRf2"
             },
             "outputs": [],
             "source": [
-                "!pip install mimllearning\n",
-                "!pip install mil\n",
-                "!pip install tensorflow\n",
-                "!pip install keras==2.12.0"
+                "!pip install mimllearning"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "AYTbl78HBtuZ"
             },
@@ -49,192 +46,65 @@
                 "id": "L-_qkpnOxj_V"
             },
             "outputs": [],
             "source": [
                 "import pkg_resources\n",
                 "from miml.datasets import load_dataset, load_birds\n",
                 "\n",
+                "# dataset = load_dataset(\"miml_birds.csv\"))\n",
+                "# dataset = load_dataset(\"C:\\Users\\Dami\u00e1n\\Downloads\\miml_birds.arff\")\n",
                 "# dataset = load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds'))\n",
                 "dataset = load_birds()\n",
                 "\n",
                 "dataset_train, dataset_test = dataset.split_dataset(0.8)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "id": "Rf5EX0HXEtZA"
-            },
-            "source": [
-                "# MIMLtoML Classifier"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {
-                "id": "c1OvYWW9Eyhw"
-            },
-            "outputs": [],
-            "source": [
-                "from sklearn.neighbors import KNeighborsClassifier\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
-                "classifier_ml = MIMLtoMLClassifier(KNeighborsClassifier(), ArithmeticTransformation())\n",
-                "classifier_ml.fit(dataset_train)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
                 "id": "KCupyHfc9c0F"
             },
             "source": [
                 "# MIMLtoMI Classifier\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {
                 "id": "J7CxjYzK9jdX"
             },
             "outputs": [],
             "source": [
-                "from miml.classifier import MIMLtoMIBRClassifier, AllPositiveAPRClassifier\n",
-                "\n",
-                "classifier_mi = MIMLtoMIBRClassifier(AllPositiveAPRClassifier())\n",
-                "classifier_mi.fit(dataset_train)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "id": "6aovUjKBxVmw"
-            },
-            "source": [
-                "# Prediction of a bag"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {
-                "colab": {
-                    "base_uri": "https://localhost:8080/"
-                },
-                "id": "2oUifr2vxY8L",
-                "outputId": "d1d857de-8fa0-491c-ca55-f5f67c3defe2"
-            },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "MIMLtoML Classifier\n",
-                        "-------------------\n",
-                        "\n",
-                        "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0.]\n",
-                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 0. 0.]]\n",
-                        "\n",
-                        "MIMLtoMI Classifier\n",
-                        "-------------------\n",
-                        "\n",
-                        "True Labels:       [0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0.]\n",
-                        "Predicted Labels:  [0. 1. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0.]\n"
-                    ]
-                }
-            ],
-            "source": [
-                "print(\"MIMLtoML Classifier\")\n",
-                "print(\"-------------------\")\n",
-                "print(\"\")\n",
-                "print(\"True Labels:       \", dataset_test.get_bag(\"254\").get_labels()[0])\n",
-                "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"254\")))\n",
-                "print(\"\")\n",
-                "print(\"MIMLtoMI Classifier\")\n",
-                "print(\"-------------------\")\n",
-                "print(\"\")\n",
-                "print(\"True Labels:      \", dataset_test.get_bag(\"254\").get_labels()[0])\n",
-                "print(\"Predicted Labels: \", classifier_mi.predict_bag(dataset_test.get_bag(\"254\")))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "id": "3Ns-WjntvZEH"
-            },
-            "source": [
-                "#  Report ML\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {
-                "colab": {
-                    "base_uri": "https://localhost:8080/"
-                },
-                "id": "ysIgN-dkvc8r",
-                "outputId": "f53bc618-971a-4bf6-9cd7-5797dfb505b1"
-            },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "precision-score-macro :  0.11025641025641027\n",
-                        "precision-score-micro :  0.3548387096774194\n",
-                        "average-precision-score-macro :  0.18543572591101495\n",
-                        "average-precision-score-micro :  0.21535397464607572\n",
-                        "recall-score-macro :  0.044037232117727476\n",
-                        "recall-score-micro :  0.10185185185185185\n",
-                        "f1-score-macro :  0.054704944178628395\n",
-                        "f1-score-micro :  0.15827338129496402\n",
-                        "fbeta-score-macro :  0.06945975659091401\n",
-                        "fbeta-score-micro :  0.2370689655172414\n",
-                        "subset-accuracy-score :  0.058823529411764705\n",
-                        "hamming-loss :  0.12074303405572756\n",
-                        "jaccard-score-macro :  0.03210078625591091\n",
-                        "jaccard-score-micro :  0.0859375\n",
-                        "log-loss :  30.660915561748453\n",
-                        "\n",
-                        "precision-score-macro,precision-score-micro,average-precision-score-macro,average-precision-score-micro,recall-score-macro,recall-score-micro,f1-score-macro,f1-score-micro,fbeta-score-macro,fbeta-score-micro,subset-accuracy-score,hamming-loss,jaccard-score-macro,jaccard-score-micro,log-loss\n",
-                        "0.11025641025641027,0.3548387096774194,0.18543572591101495,0.21535397464607572,0.044037232117727476,0.10185185185185185,0.054704944178628395,0.15827338129496402,0.06945975659091401,0.2370689655172414,0.058823529411764705,0.12074303405572756,0.03210078625591091,0.0859375,30.660915561748453\n"
-                    ]
-                }
-            ],
-            "source": [
-                "from miml.report import Report\n",
+                "from miml.classifier import MIMLtoMIBRClassifier, APRClassifier\n",
                 "\n",
-                "report = Report(classifier_ml, dataset_test, per_label=False)\n",
-                "report.to_string()\n",
-                "print(\"\")\n",
-                "report.to_csv()"
+                "classifier_mi = MIMLtoMIBRClassifier(APRClassifier())\n",
+                "classifier_mi.fit(dataset_train)\n",
+                "results_mi = classifier_mi.evaluate(dataset_test)\n",
+                "probs_mi = classifier_mi.predict_proba(dataset_test)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "5VmZnFleZUMZ"
             },
             "source": [
                 "# Report MI"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 4,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "_blawc4pZWuH",
-                "outputId": "a7b9c0e5-6fcf-473f-94da-3623266addb0"
+                "outputId": "e02d579c-479d-4297-e76e-43a8dd9eeaf8"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "precision-score-macro :  0.16599026450285032\n",
@@ -350,24 +220,26 @@
                         "\n",
                         "precision-score-macro,precision-score-micro,average-precision-score-macro,average-precision-score-micro,recall-score-macro,recall-score-micro,f1-score-macro,f1-score-micro,fbeta-score-macro,fbeta-score-micro,subset-accuracy-score,hamming-loss,jaccard-score-macro,jaccard-score-micro,log-loss,precision-score-BRCR,precision-score-PAWR,precision-score-PSFL,precision-score-RBNU,precision-score-DEJU,precision-score-OSFL,precision-score-HETH,precision-score-CBCH,precision-score-VATH,precision-score-HEWA,precision-score-SWTH,precision-score-HAFL,precision-score-WETA,precision-score-BHGB,precision-score-GCKI,precision-score-WAVI,precision-score-MGWA,precision-score-STJA,precision-score-CONI,recall-score-BRCR,recall-score-PAWR,recall-score-PSFL,recall-score-RBNU,recall-score-DEJU,recall-score-OSFL,recall-score-HETH,recall-score-CBCH,recall-score-VATH,recall-score-HEWA,recall-score-SWTH,recall-score-HAFL,recall-score-WETA,recall-score-BHGB,recall-score-GCKI,recall-score-WAVI,recall-score-MGWA,recall-score-STJA,recall-score-CONI,f1-score-BRCR,f1-score-PAWR,f1-score-PSFL,f1-score-RBNU,f1-score-DEJU,f1-score-OSFL,f1-score-HETH,f1-score-CBCH,f1-score-VATH,f1-score-HEWA,f1-score-SWTH,f1-score-HAFL,f1-score-WETA,f1-score-BHGB,f1-score-GCKI,f1-score-WAVI,f1-score-MGWA,f1-score-STJA,f1-score-CONI,fbeta-score-BRCR,fbeta-score-PAWR,fbeta-score-PSFL,fbeta-score-RBNU,fbeta-score-DEJU,fbeta-score-OSFL,fbeta-score-HETH,fbeta-score-CBCH,fbeta-score-VATH,fbeta-score-HEWA,fbeta-score-SWTH,fbeta-score-HAFL,fbeta-score-WETA,fbeta-score-BHGB,fbeta-score-GCKI,fbeta-score-WAVI,fbeta-score-MGWA,fbeta-score-STJA,fbeta-score-CONI,jaccard-score-BRCR,jaccard-score-PAWR,jaccard-score-PSFL,jaccard-score-RBNU,jaccard-score-DEJU,jaccard-score-OSFL,jaccard-score-HETH,jaccard-score-CBCH,jaccard-score-VATH,jaccard-score-HEWA,jaccard-score-SWTH,jaccard-score-HAFL,jaccard-score-WETA,jaccard-score-BHGB,jaccard-score-GCKI,jaccard-score-WAVI,jaccard-score-MGWA,jaccard-score-STJA,jaccard-score-CONI\n",
                         "0.16599026450285032,0.208955223880597,0.13233912181953641,0.13673291608692004,0.15933416428772468,0.25925925925925924,0.14296150593201268,0.23140495867768596,0.14634518676605035,0.2173913043478261,0.0196078431372549,0.19195046439628483,0.08445809323477566,0.1308411214953271,23.432988277126885,0.0,0.3333333333333333,0.23076923076923078,0.0,0.0,1.0,0.2857142857142857,0.0,0.07692307692307693,0.3,0.30434782608695654,0.0,0.2727272727272727,0.0,0.1,0.0,0.0,0.0,0.25,0.0,0.5,0.42857142857142855,0.0,0.0,0.2,0.16666666666666666,0.0,0.14285714285714285,0.2727272727272727,0.4117647058823529,0.0,0.42857142857142855,0.0,0.14285714285714285,0.0,0.0,0.0,0.3333333333333333,0.0,0.4,0.3,0.0,0.0,0.33333333333333337,0.2105263157894737,0.0,0.1,0.28571428571428564,0.35,0.0,0.33333333333333326,0.0,0.11764705882352941,0.0,0.0,0.0,0.28571428571428575,0.0,0.3571428571428571,0.2542372881355932,0.0,0.0,0.5555555555555556,0.24999999999999997,0.0,0.08474576271186442,0.29411764705882354,0.3211009174311927,0.0,0.29411764705882354,0.0,0.10638297872340426,0.0,0.0,0.0,0.2631578947368421,0.0,0.25,0.17647058823529413,0.0,0.0,0.2,0.11764705882352941,0.0,0.05263157894736842,0.16666666666666666,0.21212121212121213,0.0,0.2,0.0,0.0625,0.0,0.0,0.0,0.16666666666666666\n"
                     ]
                 }
             ],
             "source": [
-                "report = Report(classifier_mi, dataset_test)\n",
+                "from miml.report import Report\n",
+                "\n",
+                "report = Report(results_mi, probs_mi, dataset_test)\n",
                 "report.to_string()\n",
                 "print(\"\")\n",
                 "report.to_csv()"
             ]
         }
     ],
     "metadata": {
         "colab": {
-            "authorship_tag": "ABX9TyNJBtr/9a4IqLc8Ax3qNAea",
+            "authorship_tag": "ABX9TyPHBLcx6x97ebPE6LXXGnFd",
             "include_colab_link": true,
             "provenance": []
         },
         "kernelspec": {
             "display_name": "Python 3",
             "name": "python3"
         },
```

### Comparing `mimllearning-0.5.2/LICENSE.txt` & `mimllearning-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/README.md` & `mimllearning-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.2/pyproject.toml` & `mimllearning-0.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.5.2"
+version = "0.5.3"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 license = "GPL-3.0"
 keywords = ["machine-learning", "python", "data-science", "miml", "multilabel", "multi-instance"]
 readme = "README.md"
```

### Comparing `mimllearning-0.5.2/PKG-INFO` & `mimllearning-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.5.2
+Version: 0.5.3
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE.txt
 Keywords: data-science,machine-learning,miml,multi-instance,multilabel,python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```


# Comparing `tmp/mimllearning-0.5.0.tar.gz` & `tmp/mimllearning-0.5.1.tar.gz`

## Comparing `mimllearning-0.5.0.tar` & `mimllearning-0.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 mimllearning-0.5.0/readme.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 mimllearning-0.5.0/todo.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.0/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mi/mi_wrapper_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/data/bag.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/data/instance.py
--rw-r--r--   0        0        0    21294 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/dataset_utils.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/report/__init__.py
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/tutorial/classifiers_mimltoml.ipynb
--rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/tutorial/data_miml.ipynb
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/tutorial/transformations_miml.ipynb
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 mimllearning-0.5.0/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 mimllearning-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.1/readme.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 mimllearning-0.5.1/todo.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.1/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mi/mi_wrapper_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/data/instance.py
+-rw-r--r--   0        0        0    21228 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/tutorial/classifiers_mimltoml.ipynb
+-rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/tutorial/data_miml.ipynb
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/tutorial/transformations_miml.ipynb
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.1/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.1/PKG-INFO
```

### Comparing `mimllearning-0.5.0/readme.md` & `mimllearning-0.5.1/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,20 @@
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
 $ pip install mimllearning
 ```
 #### Requirements
-The requirement packages for miml library are: numpy, scikit-learn, scipy, mil, tensorflow and keras.
+The requirement packages for miml library are: numpy and scikit-learn.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
     $ pip install scikit-learn
-    $ pip install scipy
-    $ pip install mil
-    $ pip install tensorflow
-    $ pip install keras==2.12.0
 
 ### Usage
 
 
 #### Datasets
 
 ``` python
```

### Comparing `mimllearning-0.5.0/todo.md` & `mimllearning-0.5.1/todo.md`

 * *Files 24% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 
 ### Report
 
 ### Tutorials
 - tutorial particionado datasets con varios clasificadores y sus reports
 - Ejecutarlos todos de nuevo
 - Que se entienda mejor, mas prints y tal.
+- ejemplo compact mode
 
 ### Otros
 - documentacion bonita del codigo a web. Usar sphinx
 - Train_test experiment
 - Pequeño experimento
```

### Comparing `mimllearning-0.5.0/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.5.1/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/classifier/miml_classifier.py` & `mimllearning-0.5.1/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.5.1/src/miml/classifier/mi/apr_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,48 +51,47 @@
         for bag_index in positive_bag_indices:
             for instance in x_train[bag_index]:
                 apr_min = np.minimum(apr_min, instance)
                 apr_max = np.maximum(apr_max, instance)
 
         self.apr = [apr_min, apr_max]
 
-    def predict(self, bag: np.array) -> int:
+    def predict(self, bag: np.ndarray) -> int:
         """
         Predict the label of the bag
 
         Parameters
         ----------
         bag: np.ndarray of shape(n_instances, n_features)
-            features values of a bag
+            Features values of a bag
 
         Returns
         -------
         label: int
             Predicted label of the bag
 
         """
-        # If all instances of the bag and all feature values inside of apr, it is a positive bag
+        # If all instances of the bag and all feature values in apr, it is a positive bag
         if np.all(bag >= self.apr[0]):
             if np.all(bag <= self.apr[1]):
                 return 1
         return 0
 
-    def predict_proba(self, x: np.ndarray) -> np.ndarray:
+    def predict_proba(self, x_test: np.ndarray) -> np.ndarray:
         """
         Predict probabilities of given data of having a positive label
 
         Parameters
         ----------
-        x : np.ndarray of shape (n_instances, n_features)
+        x_test : np.ndarray of shape (n_bags, n_instances, n_features)
             Data to predict probabilities
 
         Returns
         -------
         results: np.ndarray of shape (n_instances, n_features)
             Predicted probabilities for given data
         """
-        result = np.zeros(x.shape[0])
-        for i in range(x.shape[0]):
-            result[i] = self.predict(x[i])
+        result = np.zeros(x_test.shape[0])
+        for i in range(x_test.shape[0]):
+            result[i] = self.predict(x_test[i])
         return result
 
-
```

### Comparing `mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from copy import deepcopy
 
 from .miml_to_mi_classifier import MIMLtoMIClassifier
 from ...transformation import BinaryRelevanceTransformation
-from ...data import Bag
 from ...data import MIMLDataset
 
 
 class MIMLtoMIBRClassifier(MIMLtoMIClassifier):
     """
     Class to represent a multi-instance classifier using a binary relevance transformation
     """
```

### Comparing `mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
-from copy import deepcopy
 
 from .miml_to_mi_classifier import MIMLtoMIClassifier
 from ...transformation import LabelPowersetTransformation
-from ...data import Bag
 from ...data import MIMLDataset
 
 
 class MIMLtoMILPClassifier(MIMLtoMIClassifier):
     """
     Class to represent a multi-instance classifier using a label powerset transformation
     """
```

### Comparing `mimllearning-0.5.0/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.5.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/data/bag.py` & `mimllearning-0.5.1/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/data/instance.py` & `mimllearning-0.5.1/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/data/miml_dataset.py` & `mimllearning-0.5.1/src/miml/data/miml_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,15 +316,14 @@
         ----------
         bag : int/str
             Index or key of the bag where the instance will be added
 
         instance : Instance
             Instance of Instance class to be added
         """
-        # TODO: Test if it works
         new_bag = self.get_bag(bag)
         new_bag.add_instance(instance)
         self.data[new_bag.key] = new_bag
 
     def delete_instance(self, bag, index_instance: int) -> None:
         """
         Delete an instance of a bag of the dataset
@@ -506,22 +505,21 @@
             Percentage of bags in train dataset
 
         seed: int
             Seed to generate random numbers
 
         Returns
         ----------
-        dataset_trein : MIMLDataset
+        dataset_train : MIMLDataset
             Train dataset
 
-        dataset_test:MIMLDataset
+        dataset_test : MIMLDataset
             Test dataset
         """
         for count_label in np.sum(self.get_labels_by_bag(), 0):
-            # print(count_label)
             if count_label == 0:
                 raise Exception("Dataset contain a label with no positive instance")
 
         random.seed(seed)
         labels_train = list(range(self.get_number_labels()))
         bags_not_used = list(range(self.get_number_bags()))
```

### Comparing `mimllearning-0.5.0/src/miml/datasets/dataset_utils.py` & `mimllearning-0.5.1/src/miml/datasets/dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
     dataset = MIMLDataset()
     csv_file = open(file)
     dataset.set_name(file.split("/")[-1])
     file_name = os.path.basename(file)
     dataset.set_name(os.path.splitext(file_name)[0])
 
-    # TODO: Make it possible to pass by parameter
     num_labels = int(csv_file.readline().replace("\n", ""))
 
     header_line = csv_file.readline().replace("\n", "").split(",")
     features_name = header_line[1:-num_labels]
     dataset.set_features_name(features_name)
     labels_name = header_line[-num_labels:]
     dataset.set_labels_name(labels_name)
```

### Comparing `mimllearning-0.5.0/src/miml/datasets/miml_birds.arff` & `mimllearning-0.5.1/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/datasets/miml_birds.csv` & `mimllearning-0.5.1/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.5.1/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.5.1/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/report/report.py` & `mimllearning-0.5.1/src/miml/report/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import warnings
 import numpy as np
 from sklearn.metrics import hamming_loss, accuracy_score, fbeta_score, jaccard_score, log_loss, \
     roc_auc_score, f1_score, precision_score, recall_score, average_precision_score
-from ..classifier import MIMLClassifier
 from ..data import MIMLDataset
 
 
 class Report:
     """
     Class to generate a report
     """
 
-    def __init__(self, y_pred: np.ndarray, label_probs: np.ndarray, dataset_test: MIMLDataset, metrics: list[str] = None,
-                 header: bool = True, per_label: bool = True):
+    def __init__(self, y_pred: np.ndarray, label_probs: np.ndarray, dataset_test: MIMLDataset,
+                 metrics: list[str] = None, header: bool = True, per_label: bool = True):
 
         """
         Constructor of the class report
         """
         self.dataset = dataset_test
         self.y_true = dataset_test.get_labels_by_bag()
         self.y_pred = y_pred
```

### Comparing `mimllearning-0.5.0/src/miml/test/data_test.py` & `mimllearning-0.5.1/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.5.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-0.5.1/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 
     def __init__(self):
         self.dataset = None
         self.number_labels = 0
 
     def transform_dataset(self, dataset: MIMLDataset) -> MIMLDataset:
         """
-        Transform the dataset to multi-instance datasets dividing the original dataset into n datasets with a single
-        label, where n is the number of labels.
+        Transform the dataset to multi-instance dataset converting the labels to one label using binary to decimal
+        codification
 
         Returns
         -------
 
         datasets: MIMLDataset
             Multi instance dataset
 
         """
         self.dataset = deepcopy(dataset)
         self.number_labels = self.dataset.get_number_labels()
         labels = self.dataset.get_labels_by_bag()
         labels_transformed = []
 
         for label in labels:
-            labels_transformed.append(np.dot(label, np.flip(2 ** np.arange(len(label)))))
+            labels_transformed.append(self.ml_to_lp_label(label))
 
         for i in range(self.number_labels-1, 0, -1):
             self.dataset.delete_attribute(self.dataset.get_number_features()+i)
 
         for i in range(self.dataset.get_number_bags()):
             bag = self.dataset.get_bag(i)
             for j in range(bag.get_number_instances()):
@@ -52,27 +52,61 @@
         Parameters
         ----------
         bag :
             Bag to be transformed to multi-instance bag
 
         Returns
         -------
-        bags : list[Bag]
-            List of n_labels transformed bags
-
+        transformed_bag : Bag
+            Transformed bag
         """
         if bag.dataset is None:
             raise Exception("Can't transform a bag without an assigned dataset, because we wouldn't have info about "
                             "the features and labels")
 
         transformed_bag = deepcopy(bag)
-        for j in range(bag.get_number_labels(), 0, -1):
+
+        lp_label = self.ml_to_lp_label(bag.get_labels())
+
+        for i in range(bag.get_number_labels(), 0, -1):
             transformed_bag.dataset.attributes.pop(list(transformed_bag.dataset.attributes)[-1])
-            transformed_bag.data = np.delete(transformed_bag.data, bag.get_number_features()+j, axis=1)
+            transformed_bag.data = np.delete(transformed_bag.data, bag.get_number_features()+i, axis=1)
+
+        for j in range(bag.get_number_instances()):
+            transformed_bag.set_attribute(j, self.dataset.get_number_attributes() - 1, lp_label)
 
         transformed_bag.dataset.set_labels_name(["lp label"])
 
         return transformed_bag
 
-    def lp_to_ml_label(self, label):
+    def lp_to_ml_label(self, label) -> np.ndarray:
+        """
+        Transform lp label to multilabel
+
+        Parameters
+        ----------
+        label
+            Lp label to be transformed
+
+        Returns
+        -------
+        labels : np.ndarray
+            Multilabel labels
+        """
         binary_str = np.binary_repr(label.astype(int), width=self.number_labels)
         return np.array([int(bit) for bit in binary_str])
+
+    def ml_to_lp_label(self, labels: np.ndarray) -> float:
+        """
+        Transform multilabel to lp label
+
+        Parameters
+        ----------
+        labels : np.ndarray
+            Multilabel labels to be transformed
+
+        Returns
+        -------
+        label
+            Lp label to be transformed
+        """
+        return np.dot(labels, np.flip(2 ** np.arange(self.number_labels)))
```

### Comparing `mimllearning-0.5.0/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.5.1/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.5.1/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.5.1/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/tutorial/classifiers_mimltoml.ipynb` & `mimllearning-0.5.1/src/miml/tutorial/classifiers_mimltoml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/tutorial/data_miml.ipynb` & `mimllearning-0.5.1/src/miml/tutorial/data_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/tutorial/demo.ipynb` & `mimllearning-0.5.1/src/miml/tutorial/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/src/miml/tutorial/transformations_miml.ipynb` & `mimllearning-0.5.1/src/miml/tutorial/transformations_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/LICENSE.txt` & `mimllearning-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.0/README.md` & `mimllearning-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,20 @@
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
 $ pip install mimllearning
 ```
 #### Requirements
-The requirement packages for miml library are: numpy, scikit-learn, scipy, mil, tensorflow and keras.
+The requirement packages for miml library are: numpy and scikit-learn.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
     $ pip install scikit-learn
-    $ pip install scipy
-    $ pip install mil
-    $ pip install tensorflow
-    $ pip install keras==2.12.0
 
 ### Usage
 
 
 #### Datasets
 
 ``` python
```

### Comparing `mimllearning-0.5.0/pyproject.toml` & `mimllearning-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.5.0"
+version = "0.5.1"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 license = "GPL-3.0"
 keywords = ["machine-learning", "python", "data-science", "miml", "multilabel", "multi-instance"]
 readme = "README.md"
```

### Comparing `mimllearning-0.5.0/PKG-INFO` & `mimllearning-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.5.0
+Version: 0.5.1
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE.txt
 Keywords: data-science,machine-learning,miml,multi-instance,multilabel,python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -26,24 +26,20 @@
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install miml.
 
 ```bash
 $ pip install mimllearning
 ```
 #### Requirements
-The requirement packages for miml library are: numpy, scikit-learn, scipy, mil, tensorflow and keras.
+The requirement packages for miml library are: numpy and scikit-learn.
 Installing miml with the package manager does not install the package dependencies.
 So install them with the package manager manually if not already downloaded.
 
     $ pip install numpy
     $ pip install scikit-learn
-    $ pip install scipy
-    $ pip install mil
-    $ pip install tensorflow
-    $ pip install keras==2.12.0
 
 ### Usage
 
 
 #### Datasets
 
 ``` python
```


# Comparing `tmp/mimllearning-0.4.9.tar.gz` & `tmp/mimllearning-0.5.0.tar.gz`

## Comparing `mimllearning-0.4.9.tar` & `mimllearning-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.9/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.4.9/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/data/instance.py
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/datasets/dataset_utils.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/report/__init__.py
--rw-r--r--   0        0        0     8446 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/tutorial/miml_data.ipynb
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/tutorial/miml_transformations.ipynb
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.4.9/src/miml/tutorial/mimltoml_classifiers.ipynb
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.4.9/.gitignore
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.9/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 mimllearning-0.5.0/readme.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 mimllearning-0.5.0/todo.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.0/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mi/mi_wrapper_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/data/instance.py
+-rw-r--r--   0        0        0    21294 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/tutorial/classifiers_mimltoml.ipynb
+-rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/tutorial/data_miml.ipynb
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 mimllearning-0.5.0/src/miml/tutorial/transformations_miml.ipynb
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 mimllearning-0.5.0/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 mimllearning-0.5.0/PKG-INFO
```

### Comparing `mimllearning-0.4.9/readme.md` & `mimllearning-0.5.0/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -59,9 +59,8 @@
 report = Report()
 report.to_string(dataset_test.get_labels_by_bag(), results_ml)
 print("")
 report.to_csv(dataset_test.get_labels_by_bag(), results_ml)
 ```
 
 ### License
-[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
-- **[MIT license](http://opensource.org/licenses/mit-license.php)**
+MIML library is released under the GNU General Public License [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html).
```

### Comparing `mimllearning-0.4.9/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.5.0/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/classifier/miml_classifier.py` & `mimllearning-0.5.0/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.5.0/src/miml/classifier/mi/apr_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-class AllPositiveAPRClassifier:
+class APRClassifier:
 
     """
     Classifier for All-Positive Bags using Axis-Aligned Positive Region.
 
     This classifier assigns a positive label to bags that contain instances within a predefined
     axis-parallel rectangle (APR) defined by the minimum and maximum feature values of positive
     instances in the training set.
@@ -72,15 +72,15 @@
         """
         # If all instances of the bag and all feature values inside of apr, it is a positive bag
         if np.all(bag >= self.apr[0]):
             if np.all(bag <= self.apr[1]):
                 return 1
         return 0
 
-    def predict_proba(self, x: np.ndarray):
+    def predict_proba(self, x: np.ndarray) -> np.ndarray:
         """
         Predict probabilities of given data of having a positive label
 
         Parameters
         ----------
         x : np.ndarray of shape (n_instances, n_features)
             Data to predict probabilities
```

### Comparing `mimllearning-0.4.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         -------
         results : ndarray of shape (n_labels)
             Predicted labels of the bag
         """
         if not self.trained:
             raise Exception("The classifier is not trained. You need to call fit before predict anything")
 
-        return self.predict(bag.get_features())
+        return self.predict(bag.get_features()).astype(int)
 
     @abstractmethod
     def predict_proba(self, dataset_test: MIMLDataset) -> np.ndarray:
         """
         Predict probabilities of given dataset of having a positive label
 
         Parameters
```

### Comparing `mimllearning-0.4.9/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-0.5.0/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,18 +50,17 @@
         -------
         results : ndarray of shape (n_labels)
             Predicted labels
         """
         if not self.trained:
             raise Exception("The classifier is not trained. You need to call fit before predict anything")
 
-        # Prediction of each label
-        results = self.classifier.predict(x)
-        binary_str = np.binary_repr(results, width=self.transformation.dataset.get_number_labels())
-        return np.array([int(bit) for bit in binary_str])
+        lp_label = self.classifier.predict(x)
+
+        return self.transformation.lp_to_ml_label(lp_label)
 
     def predict_proba(self, dataset_test: MIMLDataset):
         """
         Predict probabilities of given dataset of having a positive label
 
         Parameters
         ----------
@@ -72,9 +71,19 @@
         -------
         results: np.ndarray of shape (n_instances, n_features)
             Predicted probabilities for given dataset
         """
         if not self.trained:
             raise Exception("The classifier is not trained. You need to call fit before predict anything")
 
-        return self.classifier.predict_proba(dataset_test.get_features_by_bag())
+        bags_prob = self.classifier.predict_proba(dataset_test.get_features_by_bag())
+        results = np.zeros((dataset_test.get_number_bags(), dataset_test.get_number_labels()))
+        for bag_prob_index, bag_prob in enumerate(bags_prob):
+            ml_probs = np.zeros(self.transformation.number_labels)
+            for lp_label_index, lp_label_prob in enumerate(bag_prob):
+                if lp_label_prob != 0:
+                    ml_labels = self.transformation.lp_to_ml_label(self.classifier.classes_[lp_label_index])
+                    ml_probs += ml_labels*lp_label_prob
+            results[bag_prob_index] = ml_probs
+
+        return results
```

### Comparing `mimllearning-0.4.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.5.0/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
          results : ndarray of shape (n_labels)
              Predicted labels of data
         """
         if not self.trained:
             raise Exception("The classifier is not trained. You need to call fit before predict anything")
         transformed_bag = self.transformation.transform_bag(bag)
 
-        return self.predict(transformed_bag.get_features())
+        return self.predict(transformed_bag.get_features()).astype(int)
 
     def predict_proba(self, dataset_test: MIMLDataset) -> np.ndarray:
         """
         Predict probabilities of given dataset of having a positive label
 
         Parameters
         ----------
```

### Comparing `mimllearning-0.4.9/src/miml/data/bag.py` & `mimllearning-0.5.0/src/miml/data/bag.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,14 @@
         attributes : list[str]
             List of attributes to display. If empty, all attributes will be displayed.
         """
         header = [self.key]
 
         if end is None:
             end = self.get_number_instances()
-
         if not attributes:
             header += [""] * self.get_number_attributes()
             if self.dataset is not None:
                 header = [self.key] + self.get_features_name() + self.get_labels_name()
         else:
             header = [self.key] + attributes
```

### Comparing `mimllearning-0.4.9/src/miml/data/instance.py` & `mimllearning-0.5.0/src/miml/data/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         """
         if isinstance(attribute, int):
             return self.data.item(attribute)
         elif isinstance(attribute, str):
             index = list(self.get_attributes()).index(attribute)
             return self.data.item(index)
 
-    def set_attribute(self, attribute, value) -> None:
+    def set_attribute(self, attribute, value: float) -> None:
         """
         Update value of an attribute of the instance
 
         Parameters
         ----------
         attribute : int/str
             Index/Name of the attribute
```

### Comparing `mimllearning-0.4.9/src/miml/data/miml_dataset.py` & `mimllearning-0.5.0/src/miml/data/miml_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         Get attributes name
 
         Returns
         ----------
         attributes : list[str]
             Attributes name of the dataset
         """
-        return list(self.attributes.keys())
+        return self.get_features_name()+self.get_labels_name()
 
     def get_attributes(self) -> np.ndarray:
         """
         Get attributes values of the dataset
 
         Returns
         -------
@@ -381,57 +381,72 @@
         value: float
             New value for the update
         """
         new_bag = self.get_bag(bag)
         new_bag.set_attribute(index_instance, attribute, value)
         self.data[new_bag.key] = new_bag
 
-    def add_attribute(self, position: int = None, values: np.ndarray = None) -> None:
+    def add_attribute(self, name: str, position: int = None, values: np.ndarray = None, feature: bool = True) -> None:
         """
         Add attribute to the dataset
 
         Parameters
         ----------
+        name : str
+            Name of the new attribute
+
         position : int, default = None
             Index for the new attribute
 
         values:  ndarray of shape(n_instances)
             Values for the new attribute
+
+        feature : bool
+            Boolean value to determine if the attribute added is a feature or a label
         """
-        # TODO: Test on tutorial
         count = 0
         if position is None:
-            position = self.get_number_attributes()
-        if values:
+            position = self.get_number_features()
+            if not feature:
+                position = self.get_number_attributes()
+        if values is not None:
             if values.shape[0] != self.get_number_instances():
                 raise Exception("Incorrect number of values for the new attribute. Should be the same as number of "
                                 "instances of the dataset")
         for bag_index in range(self.get_number_bags()):
             bag = self.get_bag(bag_index)
             add_values = np.zeros(self.data[bag.key].get_number_instances())
-            if values:
+            if values is not None:
                 add_values = values[count:bag.get_number_instances()+count]
-            self.data[bag.key] = np.insert(self.data[bag.key], position, add_values, axis=1)
+            self.data[bag.key].data = np.insert(self.data[bag.key].data, position, add_values, axis=1)
             count += bag.get_number_instances()
-        # TODO: Improve this. Maybe implement add_feature, add_label with name_attribute as parameter
-        self.attributes["new_attribute"] = 0
+        if feature:
+            self.attributes[name] = 0
+            features_name = self.get_features_name()
+            features_name.insert(position, name)
+            self.set_features_name(features_name)
+        if not feature:
+            self.attributes[name] = 1
+            labels_name = self.get_features_name()
+            labels_name.insert(position, name)
+            self.set_features_name(labels_name)
 
     def delete_attribute(self, position: int) -> None:
 
         """
         Delete attribute of the dataset
 
         Parameters
         ----------
         position : int
             Index of the attribute to be deleted
         """
         for bag in self.data.keys():
             self.data[bag].data = np.delete(self.data[bag].data, position, axis=1)
-        self.attributes.pop(list(self.attributes)[position])
+        self.attributes.pop(list(self.get_attributes_name())[position])
 
     def show_dataset(self, start: int = 0, end: int = None, attributes=None, mode: str = "table", info=False) -> None:
         """
         Function to show information about the dataset
 
         Parameters
         ----------
@@ -478,14 +493,33 @@
                                                if self.get_attributes_name()[i] in attributes]
                     print(",".join(list([bag.key] + instance_attributes)))
         else:
             raise Exception("Mode not available. Mode options are \"table\" and \"compact\"")
 
     def split_dataset(self, train_percentage: float = 0.8, seed=0):
 
+        """
+        Split dataset in two parts, one for training and the other for test
+
+        Parameters
+        ----------
+        train_percentage : float
+            Percentage of bags in train dataset
+
+        seed: int
+            Seed to generate random numbers
+
+        Returns
+        ----------
+        dataset_trein : MIMLDataset
+            Train dataset
+
+        dataset_test:MIMLDataset
+            Test dataset
+        """
         for count_label in np.sum(self.get_labels_by_bag(), 0):
             # print(count_label)
             if count_label == 0:
                 raise Exception("Dataset contain a label with no positive instance")
 
         random.seed(seed)
         labels_train = list(range(self.get_number_labels()))
```

### Comparing `mimllearning-0.4.9/src/miml/datasets/dataset_utils.py` & `mimllearning-0.5.0/src/miml/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/datasets/miml_birds.arff` & `mimllearning-0.5.0/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/datasets/miml_birds.csv` & `mimllearning-0.5.0/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.5.0/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.5.0/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/report/report.py` & `mimllearning-0.5.0/src/miml/report/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 
 class Report:
     """
     Class to generate a report
     """
 
-    def __init__(self, classifier: MIMLClassifier, dataset_test: MIMLDataset, metrics: list[str] = None,
+    def __init__(self, y_pred: np.ndarray, label_probs: np.ndarray, dataset_test: MIMLDataset, metrics: list[str] = None,
                  header: bool = True, per_label: bool = True):
 
         """
         Constructor of the class report
         """
         self.dataset = dataset_test
         self.y_true = dataset_test.get_labels_by_bag()
-        self.y_pred = classifier.evaluate(dataset_test)
-        self.probs = classifier.predict_proba(dataset_test)
+        self.y_pred = y_pred
+        self.probs = label_probs
 
         all_metrics = ["precision-score-macro", "precision-score-micro", "average-precision-score-macro",
                        "average-precision-score-micro", "recall-score-macro", "recall-score-micro", "f1-score-macro",
                        "f1-score-micro", "fbeta-score-macro", "fbeta-score-micro", "subset-accuracy-score",
                        "hamming-loss", "jaccard-score-macro", "jaccard-score-micro", "log-loss"]
         if per_label:
             per_label_metrics = ["precision-score", "recall-score", "f1-score", "fbeta-score", "jaccard-score"]
```

### Comparing `mimllearning-0.4.9/src/miml/test/data_test.py` & `mimllearning-0.5.0/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.5.0/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.9/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-0.5.0/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,36 +7,37 @@
 class LabelPowersetTransformation:
     """
     Class that performs a label powerset transformation.
     """
 
     def __init__(self):
         self.dataset = None
+        self.number_labels = 0
 
     def transform_dataset(self, dataset: MIMLDataset) -> MIMLDataset:
         """
         Transform the dataset to multi-instance datasets dividing the original dataset into n datasets with a single
         label, where n is the number of labels.
 
         Returns
         -------
 
         datasets: MIMLDataset
             Multi instance dataset
 
         """
         self.dataset = deepcopy(dataset)
-        number_labels = self.dataset.get_number_labels()
+        self.number_labels = self.dataset.get_number_labels()
         labels = self.dataset.get_labels_by_bag()
         labels_transformed = []
 
         for label in labels:
             labels_transformed.append(np.dot(label, np.flip(2 ** np.arange(len(label)))))
 
-        for i in range(number_labels-1, 0, -1):
+        for i in range(self.number_labels-1, 0, -1):
             self.dataset.delete_attribute(self.dataset.get_number_features()+i)
 
         for i in range(self.dataset.get_number_bags()):
             bag = self.dataset.get_bag(i)
             for j in range(bag.get_number_instances()):
                 self.dataset.set_attribute(i, j, self.dataset.get_number_attributes()-1, labels_transformed[i])
 
@@ -67,7 +68,11 @@
         for j in range(bag.get_number_labels(), 0, -1):
             transformed_bag.dataset.attributes.pop(list(transformed_bag.dataset.attributes)[-1])
             transformed_bag.data = np.delete(transformed_bag.data, bag.get_number_features()+j, axis=1)
 
         transformed_bag.dataset.set_labels_name(["lp label"])
 
         return transformed_bag
+
+    def lp_to_ml_label(self, label):
+        binary_str = np.binary_repr(label.astype(int), width=self.number_labels)
+        return np.array([int(bit) for bit in binary_str])
```

### Comparing `mimllearning-0.4.9/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.5.0/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
     def transform_dataset(self, dataset: MIMLDataset) -> MIMLDataset:
         """
         Transform the dataset to multilabel dataset converting each bag into a single instance being the value of each
         attribute the mean value of the instances in the bag.
 
         Parameters
+        -------
+        dataset : MIMLDataset
+            Dataset to transform
 
         Returns
         -------
         transformed_dataset : MIMLDataset
             Transformed dataset
 
         """
@@ -42,18 +45,21 @@
     def transform_bag(self, bag: Bag):
         """
         Transform a bag to a multilabel instance
 
         Parameters
         ----------
         bag : Bag
-            Bag to be transformed
+            Bag to transform
 
         Returns
         -------
+        transformed_bag : Bag
+            Transformed bag
+
         """
         if bag.dataset is None:
             raise Exception("Can't transform a bag without an assigned dataset, because we wouldn't have info about "
                             "the features and labels")
 
         features = bag.get_features()
         labels = bag.get_labels()[0]
```

### Comparing `mimllearning-0.4.9/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.5.0/src/miml/transformation/mimlTOml/geometric.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,23 @@
         super().__init__()
 
     def transform_dataset(self, dataset: MIMLDataset) -> MIMLDataset:
         """
         Transform the dataset to multilabel dataset converting each bag into a single instance being the value of each
         attribute the geometric center of the instances in the bag.
 
+        Parameters
+        -------
+        dataset : MIMLDataset
+            Dataset to transform
+
         Returns
         -------
+        transformed_dataset : MIMLDataset
+            Transformed dataset
         """
         self.dataset = dataset
         transformed_dataset = MIMLDataset()
         transformed_dataset.set_name(dataset.get_name())
         transformed_dataset.set_features_name(dataset.get_features_name())
         transformed_dataset.set_labels_name(dataset.get_labels_name())
         for bag_index, key in enumerate(self.dataset.data.keys()):
```

### Comparing `mimllearning-0.4.9/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.5.0/src/miml/transformation/mimlTOml/minmax.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,22 +16,23 @@
         super().__init__()
 
     def transform_dataset(self, dataset: MIMLDataset):
         """
         Transform the dataset to multilabel dataset converting each bag into a single instance with the min and max
         value of each attribute as two new attributes.
 
-        Returns
+        Parameters
         -------
+        dataset : MIMLDataset
+            Dataset to transform
 
-        X : ndarray of shape (n_bags, n_features*2)
-            Training vector
-
-        Y : ndarray of shape (n_bags, n_labels)
-            Target vector relative to X.
+        Returns
+        -------
+        transformed_dataset : MIMLDataset
+            Transformed dataset
 
         """
         self.dataset = dataset
         transformed_dataset = MIMLDataset()
         transformed_dataset.set_name(dataset.get_name())
         features_name = dataset.get_features_name()
         features_name_min = ["min_" + feature for feature in features_name]
```

### Comparing `mimllearning-0.4.9/src/miml/tutorial/mimltoml_classifiers.ipynb` & `mimllearning-0.5.0/src/miml/tutorial/classifiers_mimltoml.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9222537878787879%*

 * *Differences: {"'cells'": "{1: {'source': ['### Examples of ML Classifiers that can be used in the library from "*

 * *            "scikit-learn:']}, 5: {'source': {delete: [3, 2, 1]}, 'metadata': {'outputId': "*

 * *            "'d2a97714-7a53-4ab8-cd88-675a6f3df5c6'}, 'execution_count': 3, 'outputs': {0: "*

 * *            "{'text': {insert: [(0, 'Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 1. "*

 * *            "0. 0. 0. 0. 0. 1.]]\\n')], delete: [0]}}}}, 7: {'source': {insert: [(2, "*

 * *            "'classifier_ml = MIMLtoMLCl […]*

```diff
@@ -1,301 +1,416 @@
 {
     "cells": [
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "id": "QNmyu82hKcVB"
+            },
+            "outputs": [],
+            "source": [
+                "!pip install mimllearning\n",
+                "!pip install mil\n",
+                "!pip install tensorflow\n",
+                "!pip install keras==2.12.0\n",
+                "\n",
+                "from miml.transformation import ArithmeticTransformation, GeometricTransformation, MinMaxTransformation\n",
+                "from miml.classifier import MIMLtoMLClassifier\n",
+                "from miml.datasets import load_birds_train, load_birds_test\n",
+                "\n",
+                "dataset_train = load_birds_train()\n",
+                "dataset_test = load_birds_test()"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {
                 "id": "KwibNMJV9Gns"
             },
             "source": [
-                "Examples of ML Classifiers that can be used in the library from scikit-learn:"
+                "### Examples of ML Classifiers that can be used in the library from scikit-learn:"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "DMTHDNJ2Vz67"
+            },
+            "source": [
+                "#### One vs Rest Classifier (Binary Relevance Classifier) [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.multiclass.OneVsRestClassifier.html)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 2,
+            "metadata": {
+                "colab": {
+                    "base_uri": "https://localhost:8080/"
+                },
+                "id": "Z-8LL2vbWEBh",
+                "outputId": "cf4d5150-8c4f-40a2-97ae-59576771cd4e"
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Predicted Labels:  [[0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0]]\n",
+                        "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from sklearn.multiclass import OneVsRestClassifier\n",
+                "from sklearn.svm import SVC\n",
+                "\n",
+                "classifier_ml = MIMLtoMLClassifier(OneVsRestClassifier(SVC()), ArithmeticTransformation())\n",
+                "classifier_ml.fit(dataset_train)\n",
+                "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
+                "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "BfO7dgESMX9O"
+            },
+            "source": [
+                "#### Decision Tree Classifier [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "ZP8rdL8KKFO-",
-                "outputId": "a8d53d5b-87a0-4381-a8ba-0962c358b139"
+                "outputId": "d2a97714-7a53-4ab8-cd88-675a6f3df5c6"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Predicted Labels:  [[0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 1. 0. 1. 0. 0. 0. 0. 0. 0.]]\n",
+                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 1. 0. 0. 0. 0. 0. 1.]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.tree import DecisionTreeClassifier\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
                 "classifier_ml = MIMLtoMLClassifier(DecisionTreeClassifier(), ArithmeticTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "tci9srfrMgdb"
+            },
+            "source": [
+                "#### Extra Tree Classifier [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.tree.ExtraTreeClassifier.html)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 4,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "GSsomGovLXDu",
-                "outputId": "f0d6a52f-8177-435c-ce52-78151eecfca6"
+                "outputId": "b1ca675e-64f3-41d8-d10b-33cdff42311c"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 1. 0. 0. 0. 0. 0. 0. 0. 1.]]\n",
+                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 0. 0. 1. 1. 0. 0. 0. 0.]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.tree import ExtraTreeClassifier\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
-                "classifier_ml = MIMLtoMLClassifier(ExtraTreeClassifier(), ArithmeticTransformation())\n",
+                "classifier_ml = MIMLtoMLClassifier(ExtraTreeClassifier(), GeometricTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "tFiaHceqNhId"
+            },
+            "source": [
+                "#### Extra Trees Classifier [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.ExtraTreesClassifier.html)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 5,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "lqWQmt4GLXhQ",
-                "outputId": "8f7ea35e-45ca-4414-8b9a-dac81c388df4"
+                "outputId": "59ac66ec-da36-44ef-c61b-72ef95450455"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 0. 0. 0. 0.]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.ensemble import ExtraTreesClassifier\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
                 "classifier_ml = MIMLtoMLClassifier(ExtraTreesClassifier(), ArithmeticTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "ntyyKA6zN3VI"
+            },
+            "source": [
+                "#### K-Nearest Neighbors Classifier [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 6,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "0CRlS6loLX3Z",
-                "outputId": "03f1b296-9cfc-4450-b169-8f28363ea76d"
+                "outputId": "28febdc5-bfb3-4aec-f691-ba27f2c5c62d"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 0. 0. 0. 0.]]\n",
+                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0.]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.neighbors import KNeighborsClassifier\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
-                "classifier_ml = MIMLtoMLClassifier(KNeighborsClassifier(), ArithmeticTransformation())\n",
+                "classifier_ml = MIMLtoMLClassifier(KNeighborsClassifier(), MinMaxTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "SYuoXFFFOThR"
+            },
+            "source": [
+                "#### Multi-layer Perceptron Classifier [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 7,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "lrh21g0yLYDq",
-                "outputId": "2efbdde6-7e02-4d77-f038-a4db176ab957"
+                "outputId": "74bc62b6-e801-4065-bc0a-ddde3add6f89"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Predicted Labels:  [[0 1 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0 0]]\n",
+                        "Predicted Labels:  [[0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.neural_network import MLPClassifier\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
-                "classifier_ml = MIMLtoMLClassifier(MLPClassifier(), ArithmeticTransformation())\n",
+                "classifier_ml = MIMLtoMLClassifier(MLPClassifier(), GeometricTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "xQoVtETZOgKP"
+            },
+            "source": [
+                "Radius Neighbors Classifier [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.RadiusNeighborsClassifier.html)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 50,
+            "execution_count": 8,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "rrrjmBUULYTc",
-                "outputId": "43cb57b9-4e05-43c7-861a-0c90eb072e11"
+                "outputId": "aec2e900-7123-4aea-87a0-1cf9d66ac015"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 0. 0. 0. 0.]]\n",
+                        "Predicted Labels:  [[1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.neighbors import RadiusNeighborsClassifier\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
-                "classifier_ml = MIMLtoMLClassifier(RadiusNeighborsClassifier(radius=50, outlier_label=1), ArithmeticTransformation())\n",
+                "classifier_ml = MIMLtoMLClassifier(RadiusNeighborsClassifier(radius=50, outlier_label=1), MinMaxTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "lU1O_FOnO9Q0"
+            },
+            "source": [
+                "#### Random Forest Classifier [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 9,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "SUo12TmnLYiT",
-                "outputId": "8f3595f1-9ef2-44ab-aba0-d013cd50f0cf"
+                "outputId": "65b7eca0-038b-4df8-f5b0-796c1e04c882"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 0. 0. 0. 0.]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.ensemble import RandomForestClassifier\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
                 "classifier_ml = MIMLtoMLClassifier(RandomForestClassifier(), ArithmeticTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "-6oH8LQhPXte"
+            },
+            "source": [
+                "#### Ridge Classifier [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.RidgeClassifier.html)"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 10,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "yW0erV4eM_IS",
-                "outputId": "8c0a3620-3e98-4004-c4da-38e704e2940f"
+                "outputId": "fee8e30e-b589-427a-ac21-ba7e0815ed08"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Predicted Labels:  [[0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.linear_model import RidgeClassifier\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
-                "classifier_ml = MIMLtoMLClassifier(RidgeClassifier(), ArithmeticTransformation())\n",
+                "classifier_ml = MIMLtoMLClassifier(RidgeClassifier(), GeometricTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "J21jhGbAMQb8"
+            },
+            "source": [
+                "#### Ridge Classifier CV [Reference](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.RidgeClassifierCV.html)\n",
+                "\n"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 11,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "qUXu_fhNNBYL",
-                "outputId": "bea103ca-322e-4d97-81e2-30a84ab7ea40"
+                "outputId": "11dd4665-2c40-4a2c-984b-ce3f7b0d9926"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Predicted Labels:  [[0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0]]\n",
+                        "Predicted Labels:  [[0 0 0 0 0 0 0 0 0 0 1 0 0 0 0 0 0 0 0]]\n",
                         "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "from sklearn.linear_model import RidgeClassifierCV\n",
                 "\n",
-                "from miml.transformation import ArithmeticTransformation\n",
-                "from miml.classifier import MIMLtoMLClassifier\n",
-                "\n",
-                "classifier_ml = MIMLtoMLClassifier(RidgeClassifierCV(), ArithmeticTransformation())\n",
+                "classifier_ml = MIMLtoMLClassifier(RidgeClassifierCV(), MinMaxTransformation())\n",
                 "classifier_ml.fit(dataset_train)\n",
                 "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
                 "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])"
             ]
         }
     ],
     "metadata": {
```

### Comparing `mimllearning-0.4.9/README.md` & `mimllearning-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -59,9 +59,8 @@
 report = Report()
 report.to_string(dataset_test.get_labels_by_bag(), results_ml)
 print("")
 report.to_csv(dataset_test.get_labels_by_bag(), results_ml)
 ```
 
 ### License
-[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
-- **[MIT license](http://opensource.org/licenses/mit-license.php)**
+MIML library is released under the GNU General Public License [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html).
```

### Comparing `mimllearning-0.4.9/PKG-INFO` & `mimllearning-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.4.9
+Version: 0.5.0
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
-Classifier: License :: OSI Approved :: MIT License
+License-Expression: GPL-3.0
+License-File: LICENSE.txt
+Keywords: data-science,machine-learning,miml,multi-instance,multilabel,python
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # miml: Multi Instance Multi Label Learning Library for Python
 The aim of the library is to ease the development, testing and comparison of classification algorithms for multi-instance multi-label learning (MIML). 
@@ -71,9 +74,8 @@
 report = Report()
 report.to_string(dataset_test.get_labels_by_bag(), results_ml)
 print("")
 report.to_csv(dataset_test.get_labels_by_bag(), results_ml)
 ```
 
 ### License
-[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)
-- **[MIT license](http://opensource.org/licenses/mit-license.php)**
+MIML library is released under the GNU General Public License [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html).
```


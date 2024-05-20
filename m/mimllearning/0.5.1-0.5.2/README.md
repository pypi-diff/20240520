# Comparing `tmp/mimllearning-0.5.1.tar.gz` & `tmp/mimllearning-0.5.2.tar.gz`

## Comparing `mimllearning-0.5.1.tar` & `mimllearning-0.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.1/readme.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 mimllearning-0.5.1/todo.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.1/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mi/mi_wrapper_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/data/bag.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/data/instance.py
--rw-r--r--   0        0        0    21228 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/dataset_utils.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/report/__init__.py
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/tutorial/classifiers_mimltoml.ipynb
--rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/tutorial/data_miml.ipynb
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 mimllearning-0.5.1/src/miml/tutorial/transformations_miml.ipynb
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.1/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.2/readme.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mimllearning-0.5.2/todo.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.2/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mi/mi_wrapper_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/data/instance.py
+-rw-r--r--   0        0        0    21354 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/tutorial/classifiers_mimltoml.ipynb
+-rw-r--r--   0        0        0    13675 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/tutorial/data_miml.ipynb
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 mimllearning-0.5.2/src/miml/tutorial/transformations_miml.ipynb
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.2/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.2/PKG-INFO
```

### Comparing `mimllearning-0.5.1/readme.md` & `mimllearning-0.5.2/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/todo.md` & `mimllearning-0.5.2/todo.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 
 ## Preguntas
 
-- Llamar evaluate fuera report pasandoselo al init, si hago esto tengo que pasar dataset.get_features_by_bag(), 
-  resultado_evaluate y nombre_etiquetas. Tampoco podria pasarle detalles como el clasificador, algoritmo y transformacion usada
-
 ### Documentacion
 - Revisar todos los nombres
 
 ### Data
+- En show dataset y bag, ver si cambiar mode compact to mode csv
 
 ### Datasets
 - Tener todos dataset en arff y csv
 - Load from libray
 
 ### Classifiers
-- Que el predict_bag de ml devuelva un array solo, y ver el tipo con el que devuelve las labels
 
 ### Report
 
 ### Tutorials
 - tutorial particionado datasets con varios clasificadores y sus reports
+- Train_test experiment
 - Ejecutarlos todos de nuevo
 - Que se entienda mejor, mas prints y tal.
-- ejemplo compact mode
 
 ### Otros
 - documentacion bonita del codigo a web. Usar sphinx
-- Train_test experiment
 - Pequeño experimento
```

### Comparing `mimllearning-0.5.1/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.5.2/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/classifier/miml_classifier.py` & `mimllearning-0.5.2/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.5.2/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/classifier/mi/mi_wrapper_classifier.py` & `mimllearning-0.5.2/src/miml/classifier/mi/mi_wrapper_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-0.5.2/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.5.2/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/data/bag.py` & `mimllearning-0.5.2/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/data/instance.py` & `mimllearning-0.5.2/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/data/miml_dataset.py` & `mimllearning-0.5.2/src/miml/data/miml_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -651,11 +651,13 @@
         n_instances, min_instances, max_instances, distribution = self.get_statistics()
         print("-----MULTIINSTANCE-----")
         print("Nº of bags: ", self.get_number_bags())
         print("Total instances: ", n_instances)
         print("Average Instances per bag: ", n_instances / self.get_number_bags())
         print("Min Instances per bag: ", min_instances)
         print("Max Instances per bag: ", max_instances)
+        print("Features per bag: ", self.get_number_features())
+        print("Labels per bag: ", self.get_number_labels())
         print("Attributes per bag: ", self.get_number_attributes())
         print("\nDistribution of bags:")
         for number_instances_in_bag, occurrences in sorted(distribution.items()):
             print("\tBags with ", number_instances_in_bag, " instances: ", occurrences)
```

### Comparing `mimllearning-0.5.1/src/miml/datasets/dataset_utils.py` & `mimllearning-0.5.2/src/miml/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/datasets/miml_birds.arff` & `mimllearning-0.5.2/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/datasets/miml_birds.csv` & `mimllearning-0.5.2/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.5.2/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.5.2/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/report/report.py` & `mimllearning-0.5.2/src/miml/report/report.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/test/data_test.py` & `mimllearning-0.5.2/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.5.2/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-0.5.2/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.5.2/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.5.2/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.5.2/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/tutorial/classifiers_mimltoml.ipynb` & `mimllearning-0.5.2/src/miml/tutorial/classifiers_mimltoml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/tutorial/data_miml.ipynb` & `mimllearning-0.5.2/src/miml/tutorial/data_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/tutorial/demo.ipynb` & `mimllearning-0.5.2/src/miml/tutorial/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/src/miml/tutorial/transformations_miml.ipynb` & `mimllearning-0.5.2/src/miml/tutorial/transformations_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/LICENSE.txt` & `mimllearning-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/README.md` & `mimllearning-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.1/pyproject.toml` & `mimllearning-0.5.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.5.1"
+version = "0.5.2"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 license = "GPL-3.0"
 keywords = ["machine-learning", "python", "data-science", "miml", "multilabel", "multi-instance"]
 readme = "README.md"
```

### Comparing `mimllearning-0.5.1/PKG-INFO` & `mimllearning-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.5.1
+Version: 0.5.2
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE.txt
 Keywords: data-science,machine-learning,miml,multi-instance,multilabel,python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```


# Comparing `tmp/Package_G2-1.0.0.tar.gz` & `tmp/Package_G2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Package_G2-1.0.0.tar", last modified: Sat May 18 14:44:55 2024, max compression
+gzip compressed data, was "Package_G2-1.0.1.tar", last modified: Sun May 19 21:56:51 2024, max compression
```

## Comparing `Package_G2-1.0.0.tar` & `Package_G2-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:44:55.929939 Package_G2-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-18 14:44:55.896940 Package_G2-1.0.0/KMeans_G2/
--rw-rw-rw-   0        0        0      943 2024-05-18 12:16:48.000000 Package_G2-1.0.0/KMeans_G2/KMeans_G2.py
--rw-rw-rw-   0        0        0        0 2024-05-18 12:13:15.000000 Package_G2-1.0.0/KMeans_G2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:44:55.909940 Package_G2-1.0.0/KNN_G2/
--rw-rw-rw-   0        0        0     1076 2024-05-18 12:19:27.000000 Package_G2-1.0.0/KNN_G2/KNN_G2.py
--rw-rw-rw-   0        0        0        0 2024-05-18 12:13:24.000000 Package_G2-1.0.0/KNN_G2/__init__.py
--rw-rw-rw-   0        0        0      181 2024-05-18 14:44:55.927939 Package_G2-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 14:44:55.924943 Package_G2-1.0.0/Package_G2.egg-info/
--rw-rw-rw-   0        0        0      181 2024-05-18 14:44:55.000000 Package_G2-1.0.0/Package_G2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-18 14:44:55.000000 Package_G2-1.0.0/Package_G2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:44:55.000000 Package_G2-1.0.0/Package_G2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-18 14:44:55.000000 Package_G2-1.0.0/Package_G2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-18 14:44:55.000000 Package_G2-1.0.0/Package_G2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 14:44:55.929939 Package_G2-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      347 2024-05-18 14:42:18.000000 Package_G2-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:56:51.408842 Package_G2-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-19 21:56:51.359604 Package_G2-1.0.1/KMeans_G2/
+-rw-rw-rw-   0        0        0      991 2024-05-19 20:24:48.000000 Package_G2-1.0.1/KMeans_G2/KMeans_G2.py
+-rw-rw-rw-   0        0        0        0 2024-05-18 12:13:15.000000 Package_G2-1.0.1/KMeans_G2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:56:51.371718 Package_G2-1.0.1/KNN_G2/
+-rw-rw-rw-   0        0        0     1222 2024-05-19 21:55:46.000000 Package_G2-1.0.1/KNN_G2/KNN_G2.py
+-rw-rw-rw-   0        0        0        0 2024-05-18 12:13:24.000000 Package_G2-1.0.1/KNN_G2/__init__.py
+-rw-rw-rw-   0        0        0      181 2024-05-19 21:56:51.407843 Package_G2-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 21:56:51.403842 Package_G2-1.0.1/Package_G2.egg-info/
+-rw-rw-rw-   0        0        0      181 2024-05-19 21:56:50.000000 Package_G2-1.0.1/Package_G2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8340 2024-05-19 21:55:58.000000 Package_G2-1.0.1/Package_G2.egg-info/Readme.md
+-rw-rw-rw-   0        0        0      288 2024-05-19 21:56:51.000000 Package_G2-1.0.1/Package_G2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 21:56:50.000000 Package_G2-1.0.1/Package_G2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-19 21:56:50.000000 Package_G2-1.0.1/Package_G2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 21:56:50.000000 Package_G2-1.0.1/Package_G2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 21:56:51.409844 Package_G2-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      366 2024-05-19 21:48:08.000000 Package_G2-1.0.1/setup.py
```

### Comparing `Package_G2-1.0.0/KMeans_G2/KMeans_G2.py` & `Package_G2-1.0.1/KMeans_G2/KMeans_G2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import numpy as np
 def kmeans_G2(X, k, num_iterations=10000000):
     
     # Convertir la liste en un tableau numpy
     X = np.array(X)
-    
+    iteration = 0
     # Initialisation : choisissez k points aléatoires comme centroïdes
     np.random.seed(45)  # Fixer l'aléa
     centroids = X[np.random.choice(X.shape[0], k, replace=False)]
 
     for _ in range(num_iterations):
     
         # Assignation des points aux clusters
@@ -17,13 +17,14 @@
         labels = np.argmin(distances, axis=1)
 
         # Mise à jour des centroïdes
         #for i in range(k):
             #centroids[i] = np.mean(X[labels == i], axis=0)
         new_centers = np.array([X[labels == i].mean(axis=0) for i in range(k)])
         
+        iteration += 1
         if np.allclose(new_centers, centroids):
             break 
         
         centroids = new_centers
     
-    return labels, centroids
+    return labels, centroids, iteration
```

### Comparing `Package_G2-1.0.0/KNN_G2/KNN_G2.py` & `Package_G2-1.0.1/KNN_G2/KNN_G2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import pandas as pd
-import numpy as np 
+import numpy as np
 
-## Initialisation des parametres
-def __init__(self, k=3):
-    self.k = k
+### Algorithme de KNN sans bibliotèque externe
 
-## Entrainement du modele
-def fit(self, X_train, y_train):
-    self.X_train = X_train
-    self.y_train = y_train
+class KNN_G2 :
+    ## Initialisation des parametres
+    def __init__(self, k=3):
+        self.k = k
 
-        
+    ## Entrainement du modele
+    def fit(self, X_train, y_train):
+        self.X_train = X_train
+        self.y_train = y_train
 
-## Application à nos données de tests
+    ## Application à nos données de tests
 
-def predict(self, X_test): 
-    predictions = []
-    for x in X_test:
-        # Calcul des distances euclidiennes entre x et tous les points de X_train
-        distances = np.sqrt(np.sum((self.X_train - x)**2, axis=1))
+    def predict(self, X_test): 
+        predictions = []
+        for x in X_test:
+            # Calcul des distances euclidiennes entre x et tous les points de X_train
+            distances = np.sqrt(np.sum((self.X_train - x)**2, axis=1))
 
-        # Tri des indices des distances croissantes
-        sorted_indices = np.argsort(distances)
+            # Tri des indices des distances croissantes
+            sorted_indices = np.argsort(distances)
 
-        # Sélection des k plus proches voisins
-        k_nearest_indices = sorted_indices[:self.k]
+            # Sélection des k plus proches voisins
+            k_nearest_indices = sorted_indices[:self.k]
 
-        # Obtention des étiquettes des k plus proches voisins
-        k_nearest_labels = self.y_train[k_nearest_indices]
+            # Obtention des étiquettes des k plus proches voisins
+            k_nearest_labels = self.y_train[k_nearest_indices]
 
-        # Prédiction de l'étiquette majoritaire parmi les k plus proches voisins
-        prediction = np.bincount(k_nearest_labels).argmax()
+            # Prédiction de l'étiquette majoritaire parmi les k plus proches voisins
+            prediction = np.bincount(k_nearest_labels).argmax()
 
-        predictions.append(prediction)
+            predictions.append(prediction)
 
-    return np.array(predictions)
+        return np.array(predictions)
```


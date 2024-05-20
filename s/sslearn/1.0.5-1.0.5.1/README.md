# Comparing `tmp/sslearn-1.0.5.tar.gz` & `tmp/sslearn-1.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sslearn-1.0.5.tar", last modified: Wed May  8 15:30:09 2024, max compression
+gzip compressed data, was "sslearn-1.0.5.1.tar", last modified: Mon May 20 11:13:44 2024, max compression
```

## Comparing `sslearn-1.0.5.tar` & `sslearn-1.0.5.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.569039 sslearn-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-08 15:30:02.000000 sslearn-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 15:30:09.569039 sslearn-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-08 15:30:02.000000 sslearn-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 15:30:09.569039 sslearn-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 15:30:02.000000 sslearn-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.565039 sslearn-1.0.5/sslearn/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.565039 sslearn-1.0.5/sslearn/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/datasets/_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/datasets/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/datasets/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.565039 sslearn-1.0.5/sslearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/model_selection/_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/restricted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.565039 sslearn-1.0.5/sslearn/subview/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/subview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/subview/_subview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.569039 sslearn-1.0.5/sslearn/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60686 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/wrapper/_co.py
--rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/wrapper/_self.py
--rw-r--r--   0 runner    (1001) docker     (127)    32663 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/wrapper/_tritraining.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.569039 sslearn-1.0.5/sslearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.569039 sslearn-1.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_subview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.833571 sslearn-1.0.5.1/sslearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.833571 sslearn-1.0.5.1/sslearn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/datasets/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/datasets/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/datasets/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/sslearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/model_selection/_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/restricted (Copia en conflicto de CROSS-PC 2024-05-14).py
+-rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/restricted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/sslearn/subview/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/subview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/subview/_subview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/sslearn/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60641 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/wrapper/_co.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15721 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/wrapper/_self.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32663 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/wrapper/_tritraining.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/sslearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_subview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_wrapper.py
```

### Comparing `sslearn-1.0.5/LICENSE` & `sslearn-1.0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/PKG-INFO` & `sslearn-1.0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sslearn
-Version: 1.0.5
+Version: 1.0.5.1
 Summary: A Python package for semi-supervised learning with scikit-learn
 Home-page: https://github.com/jlgarridol/sslearn
-Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.tar.gz
+Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.1.tar.gz
 Author: José Luis Garrido-Labrador
 Author-email: jlgarrido@ubu.es
 License: new BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `sslearn-1.0.5/README.md` & `sslearn-1.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/setup.py` & `sslearn-1.0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/__init__.py` & `sslearn-1.0.5.1/sslearn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 elif os.path.exists("README.md"):
     with open("README.md", "r") as f:
         __doc__ = f.read()
 else:
     __doc__ = "Semi-Supervised Learning (SSL) is a Python package that provides tools to train and evaluate semi-supervised learning models."
 
 
-__version__='1.0.5'
+__version__='1.0.5.1'
 __AUTHOR__="José Luis Garrido-Labrador"  # Author of the package
 __AUTHOR_EMAIL__="jlgarrido@ubu.es"  # Author's email
 __URL__="https://pypi.org/project/sslearn/"
```

### Comparing `sslearn-1.0.5/sslearn/base.py` & `sslearn-1.0.5.1/sslearn/base.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/datasets/__init__.py` & `sslearn-1.0.5.1/sslearn/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/datasets/_loader.py` & `sslearn-1.0.5.1/sslearn/datasets/_loader.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/datasets/_preprocess.py` & `sslearn-1.0.5.1/sslearn/datasets/_preprocess.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/datasets/_writer.py` & `sslearn-1.0.5.1/sslearn/datasets/_writer.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/model_selection/_split.py` & `sslearn-1.0.5.1/sslearn/model_selection/_split.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sklearn.model_selection as ms
 from sklearn.utils import check_random_state
 import numpy as np
+import pandas as pd
 
 
 class StratifiedKFoldSS():
     """
     Stratified K-Folds cross-validator for semi-supervised learning.
     
     Provides label and unlabel indices for each split. Using the `StratifiedKFold` method from `sklearn`.
@@ -104,14 +105,24 @@
     unlabel: ndarray (optional)
         The training set indexes for split mark as unlabeled.
     """
     assert (label_rate > 0) and (label_rate < 1),\
         "Label rate must be in (0, 1)."
     assert "test_size" not in kwards and "train_size" not in kwards,\
         "Test size and train size are illegal parameters in this method."
+    
+    columns = None
+    is_df = False
+    if hasattr(X, "iloc"):
+        is_df = True
+        columns = X.columns
+        X = X.values
+    if hasattr(y, "iloc"):
+        is_df = True
+        y = y.values
 
     indices = np.arange(len(y))
 
     if force_minimum is not None:
         try:
             selected = __random_select_n_instances(y, force_minimum, random_state)
         except ValueError:
@@ -123,26 +134,32 @@
     # Train test split with indexes
     label, unlabel = ms.train_test_split(indices, train_size=label_rate,
                                          random_state=random_state, **kwards)
 
     if force_minimum is not None:
         label = np.concatenate((selected, label))
     
+    y_unlabel_original = y[unlabel]
+
     # Create the label and unlabel sets
     X_label, y_label, X_unlabel, y_unlabel = X[label], y[label],\
         X[unlabel], np.array([-1] * len(unlabel))
 
     # Create the artificial dataset
     X = np.concatenate((X_label, X_unlabel), axis=0)
     y = np.concatenate((y_label, y_unlabel), axis=0)
 
+    if is_df:
+        X = pd.DataFrame(X, columns=columns)
+        y = pd.Series(y)
+
     if indexes:
-        return X, y, X_unlabel, y_unlabel, label, unlabel
+        return X, y, X_unlabel, y_unlabel_original, label, unlabel
 
-    return X, y, X_unlabel, y_unlabel
+    return X, y, X_unlabel, y_unlabel_original
 
 
     """    
     if force_minimum is not None:
         try:
             selected = __random_select_n_instances(y, force_minimum, random_state)
         except ValueError:
```

### Comparing `sslearn-1.0.5/sslearn/restricted.py` & `sslearn-1.0.5.1/sslearn/restricted.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/subview/_subview.py` & `sslearn-1.0.5.1/sslearn/subview/_subview.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/utils.py` & `sslearn-1.0.5.1/sslearn/utils.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/wrapper/__init__.py` & `sslearn-1.0.5.1/sslearn/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn/wrapper/_co.py` & `sslearn-1.0.5.1/sslearn/wrapper/_co.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,16 +105,14 @@
             Sample weights.
 
         Returns
         -------
         score : float
             Mean accuracy of ``self.predict(X)`` w.r.t. `y`.
         """
-        from .metrics import accuracy_score
-
         return accuracy_score(y, self.predict(X), sample_weight=sample_weight)
 
 
 class DemocraticCoLearning(BaseCoTraining):
     """
     **Democratic Co-learning. Ensemble of classifiers of different types.**
     --------------------------------------------
```

### Comparing `sslearn-1.0.5/sslearn/wrapper/_self.py` & `sslearn-1.0.5.1/sslearn/wrapper/_self.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 import pandas as pd
 from scipy.stats import norm
-from sklearn.base import BaseEstimator, ClassifierMixin
+from sklearn.base import BaseEstimator, MetaEstimatorMixin
 from sklearn.base import clone as skclone
 from sklearn.neighbors import KNeighborsClassifier, kneighbors_graph
 from sklearn.semi_supervised import SelfTrainingClassifier
 from sklearn.utils import check_random_state, resample
+from sklearn.metrics import accuracy_score
 
 from sslearn.utils import calculate_prior_probability, check_classifier
 
 from ..base import get_dataset
 
 
 class SelfTraining(SelfTrainingClassifier):
@@ -120,15 +121,15 @@
         y_adapted = y.copy()
         if y_adapted.dtype.type is str or y_adapted.dtype.type is np.str_:
             y_adapted = y_adapted.astype(object)
             y_adapted[y_adapted == '-1'] = -1
         return super().fit(X, y_adapted)
 
 
-class Setred(ClassifierMixin, BaseEstimator):
+class Setred(BaseEstimator, MetaEstimatorMixin):
     """
     **Self-training with Editing.**
     ----------------------------
 
     Create a SETRED classifier. It is a self-training algorithm that uses a rejection mechanism to avoid adding noisy samples to the training set.
     The main process are:
     1. Train a classifier with the labeled data.
@@ -361,7 +362,33 @@
             The input samples.
         Returns
         -------
         y : ndarray of shape (n_samples, n_classes) or list of n_outputs such arrays if n_outputs > 1
             The predicted classes
         """
         return self._base_estimator.predict_proba(X, **kwards)
+    
+    def score(self, X, y, sample_weight=None):
+        """
+        Return the mean accuracy on the given test data and labels.
+
+        In multi-label classification, this is the subset accuracy
+        which is a harsh metric since you require for each sample that
+        each label set be correctly predicted.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Test samples.
+
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True labels for `X`.
+
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights.
+
+        Returns
+        -------
+        score : float
+            Mean accuracy of ``self.predict(X)`` w.r.t. `y`.
+        """
+        return accuracy_score(y, self.predict(X), sample_weight=sample_weight)
```

### Comparing `sslearn-1.0.5/sslearn/wrapper/_tritraining.py` & `sslearn-1.0.5.1/sslearn/wrapper/_tritraining.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/sslearn.egg-info/PKG-INFO` & `sslearn-1.0.5.1/sslearn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sslearn
-Version: 1.0.5
+Version: 1.0.5.1
 Summary: A Python package for semi-supervised learning with scikit-learn
 Home-page: https://github.com/jlgarridol/sslearn
-Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.tar.gz
+Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.1.tar.gz
 Author: José Luis Garrido-Labrador
 Author-email: jlgarrido@ubu.es
 License: new BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `sslearn-1.0.5/sslearn.egg-info/SOURCES.txt` & `sslearn-1.0.5.1/sslearn.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 sslearn/__init__.py
 sslearn/base.py
+sslearn/restricted (Copia en conflicto de CROSS-PC 2024-05-14).py
 sslearn/restricted.py
 sslearn/utils.py
 sslearn.egg-info/PKG-INFO
 sslearn.egg-info/SOURCES.txt
 sslearn.egg-info/dependency_links.txt
 sslearn.egg-info/requires.txt
 sslearn.egg-info/top_level.txt
```

### Comparing `sslearn-1.0.5/test/test_datasets.py` & `sslearn-1.0.5.1/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/test/test_general.py` & `sslearn-1.0.5.1/test/test_general.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/test/test_model_selection.py` & `sslearn-1.0.5.1/test/test_model_selection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import os
 import sys
 import numpy as np
+import pandas as pd
 import pytest
 
 sys.path.append(os.path.join(os.path.dirname(os.path.abspath(__file__)), ".."))
 
 from sslearn.model_selection import (artificial_ssl_dataset, StratifiedKFoldSS)
 from sklearn.datasets import load_iris
 
+def test_artificial_ssl_dataset_with_pandas():
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, true_label = artificial_ssl_dataset(pd.DataFrame(X), pd.Series(y), label_rate=0.1)
+    assert X_unlabel.shape[0] == true_label.shape[0]
+    assert X_unlabel.shape[0]/X.shape[0] == pytest.approx(0.9)
+
 def test_artificial_ssl_dataset():
     X, y = load_iris(return_X_y=True)
     X, y, X_unlabel, true_label = artificial_ssl_dataset(X, y, label_rate=0.1)
     assert X_unlabel.shape[0] == true_label.shape[0]
     assert X_unlabel.shape[0]/X.shape[0] == pytest.approx(0.9)
 
 def test_artificial_ssl_dataset_with_force_minimum():
```

### Comparing `sslearn-1.0.5/test/test_subview.py` & `sslearn-1.0.5.1/test/test_subview.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5/test/test_wrapper.py` & `sslearn-1.0.5.1/test/test_wrapper.py`

 * *Files identical despite different names*


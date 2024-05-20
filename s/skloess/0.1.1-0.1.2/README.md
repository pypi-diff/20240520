# Comparing `tmp/skloess-0.1.1.tar.gz` & `tmp/skloess-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skloess-0.1.1.tar", max compression
+gzip compressed data, was "skloess-0.1.2.tar", max compression
```

## Comparing `skloess-0.1.1.tar` & `skloess-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1520 2024-05-16 18:00:45.333493 skloess-0.1.1/LICENSE
--rw-r--r--   0        0        0     3124 2024-05-17 13:22:34.212023 skloess-0.1.1/README.md
--rw-r--r--   0        0        0      451 2024-05-17 13:24:17.790668 skloess-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      163 2024-05-17 11:30:19.769673 skloess-0.1.1/skloess/__init__.py
--rw-r--r--   0        0        0       22 2024-05-17 13:24:32.842905 skloess-0.1.1/skloess/_version.py
--rw-r--r--   0        0        0    11949 2024-05-17 13:21:26.926285 skloess-0.1.1/skloess/skloess.py
--rw-r--r--   0        0        0       67 2024-05-16 18:00:45.341493 skloess-0.1.1/skloess/tests/__init__.py
--rw-r--r--   0        0        0     5949 2024-05-17 11:38:15.059046 skloess-0.1.1/skloess/tests/test_LOESS.py
--rw-r--r--   0        0        0     1164 2024-05-17 11:39:01.068330 skloess-0.1.1/skloess/tests/test_common.py
--rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 skloess-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1520 2024-05-16 18:00:45.333493 skloess-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3124 2024-05-17 13:22:34.212023 skloess-0.1.2/README.md
+-rw-r--r--   0        0        0      451 2024-05-20 08:26:44.605283 skloess-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      163 2024-05-17 11:30:19.769673 skloess-0.1.2/skloess/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-17 13:24:32.842905 skloess-0.1.2/skloess/_version.py
+-rw-r--r--   0        0        0    12394 2024-05-20 08:18:11.193795 skloess-0.1.2/skloess/skloess.py
+-rw-r--r--   0        0        0       67 2024-05-16 18:00:45.341493 skloess-0.1.2/skloess/tests/__init__.py
+-rw-r--r--   0        0        0     5949 2024-05-17 11:38:15.059046 skloess-0.1.2/skloess/tests/test_LOESS.py
+-rw-r--r--   0        0        0     1164 2024-05-17 11:39:01.068330 skloess-0.1.2/skloess/tests/test_common.py
+-rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 skloess-0.1.2/PKG-INFO
```

### Comparing `skloess-0.1.1/LICENSE` & `skloess-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skloess-0.1.1/README.md` & `skloess-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `skloess-0.1.1/skloess/skloess.py` & `skloess-0.1.2/skloess/skloess.py`

 * *Files 10% similar despite different names*

```diff
@@ -268,24 +268,50 @@
 
     Raises
     ------
     ValueError
         If smoothing is not between (degree + 1) / n_obs and 1
     """
     smoothing_min = (degree + 1) / n_obs
-    if smoothing_min <= smoothing < 1:
+    if smoothing_min <= smoothing <= 1:
         return smoothing
     raise ValueError(
-        "Smoothing for a polynomial with {degree} degrees "
-        "must be between {smoothing_min} and 1".format(
+        f"Smoothing for a polynomial with {degree} degrees \
+        must be between {smoothing_min} and 1".format(
             degree=degree, smoothing_min=smoothing_min
         )
     )
 
 
+def to_numpy_array(data):
+    """
+    Converts input data into a NumPy array.
+
+    Parameters:
+    data (array-like): Input data, which can be a list, NumPy array, pandas Series, etc.
+
+    Returns:
+    np.ndarray: Converted NumPy array.
+    """
+    if isinstance(data, np.ndarray):
+        if data.ndim == 1:
+            return data.reshape(-1, 1)
+        elif data.ndim >= 1:
+            if data.shape[0] > 1:
+                raise ValueError("Input numpy arrays must be 1 x n shaped")
+            else:
+                return data
+    elif isinstance(data, (list, tuple)):
+        return np.array(data).reshape(-1, 1)
+    elif isinstance(data, pd.Series):
+        return data.values.reshape(-1, 1)
+    else:
+        raise TypeError(f"Unsupported input type: {type(data)}")
+
+
 class LOESS(RegressorMixin, BaseEstimator):
     """
 
     Parameters
     ----------
     degree : int, default=1
         Degree of the polynomial used to estimate the data.
@@ -332,28 +358,27 @@
             The y coordinates of the input. Must be 1-dimensional (list/array/pandas series)
 
         Returns
         -------
         self : object
             Returns self.
         """
-        validate_smoothing(self.smoothing, self.degree, X.shape[0])
-        if X.ndim == 1:
-            if len(y) != len(X):
-                raise ValueError("X and y must have the same length")
-            # if input is list or array reshape it for sklearn compatibility
-            X = X.reshape(-1, 1)
+        X = to_numpy_array(X)
+        validate_smoothing(self.smoothing, self.degree, len(X))
+        self.n_neighbors_ = round(self.smoothing * X.shape[0])
+
         X, y = self._validate_data(X, y, accept_sparse=True, reset=True)
         self.norm_X_global_, self.min_X_global, self.max_X_global = normalize_array(X)
         self.norm_y_global_, self.min_y_global, self.max_y_global = normalize_array(y)
-        self.n_neighbors_ = round(self.smoothing * X.shape[0])
         self.is_fitted_ = True
         return self
 
     def estimate(self, X):
+        if X == np.nan:
+            return np.nan
         norm_X_local = normalize_value(X, self.min_X_global, self.max_X_global)
         distances = np.abs(self.norm_X_global_ - norm_X_local)
         min_range = get_min_range(distances, self.n_neighbors_)
         weights = get_weights(distances, min_range)
         if self.degree == 1:
             y = estimate_linear(
                 min_range,
@@ -387,17 +412,12 @@
         Returns
         -------
         y : ndarray, shape (n, 1)
             Returns an array containing the estimated values.
         """
         # Check if fit had been called
         check_is_fitted(self)
-        if type(X) in [int, float]:
-            X = np.array([[X]])
-        if X.ndim == 1:
-            # if input is list or array reshape it for sklearn compatibility
-            X = X.reshape(-1, 1)
-
+        X = to_numpy_array(X)
         X = self._validate_data(X, accept_sparse=True, reset=False)
         predicted = np.vectorize(self.estimate)(X)
         predicted = predicted.flatten()
         return predicted
```

### Comparing `skloess-0.1.1/skloess/tests/test_LOESS.py` & `skloess-0.1.2/skloess/tests/test_LOESS.py`

 * *Files identical despite different names*

### Comparing `skloess-0.1.1/skloess/tests/test_common.py` & `skloess-0.1.2/skloess/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `skloess-0.1.1/PKG-INFO` & `skloess-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skloess
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sklearn compatible implementation of the Locally Estimated Scatterplot Smoothing (LOESS) algorithm
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


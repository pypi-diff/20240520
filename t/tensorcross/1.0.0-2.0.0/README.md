# Comparing `tmp/tensorcross-1.0.0.tar.gz` & `tmp/tensorcross-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcross-1.0.0.tar", last modified: Sun Oct 29 10:46:18 2023, max compression
+gzip compressed data, was "tensorcross-2.0.0.tar", last modified: Mon May 20 19:06:06 2024, max compression
```

## Comparing `tensorcross-1.0.0.tar` & `tensorcross-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-10-29 10:46:18.532560 tensorcross-1.0.0/
--rw-rw-rw-   0        0        0     1110 2021-06-24 10:48:25.000000 tensorcross-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      864 2023-10-29 10:46:18.532560 tensorcross-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5636 2023-10-29 10:38:59.000000 tensorcross-1.0.0/README.md
--rw-rw-rw-   0        0        0     3942 2023-10-29 10:36:09.000000 tensorcross-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1016 2023-10-29 10:46:18.537561 tensorcross-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1475 2023-10-29 10:39:36.000000 tensorcross-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-29 10:46:18.507561 tensorcross-1.0.0/tensorcross/
--rw-rw-rw-   0        0        0       65 2023-10-29 10:39:36.000000 tensorcross-1.0.0/tensorcross/__init__.py
--rw-rw-rw-   0        0        0      270 2023-10-29 10:39:36.000000 tensorcross-1.0.0/tensorcross/_types.py
-drwxrwxrwx   0        0        0        0 2023-10-29 10:46:18.524562 tensorcross-1.0.0/tensorcross/model_selection/
--rw-rw-rw-   0        0        0      355 2023-10-29 10:39:36.000000 tensorcross-1.0.0/tensorcross/model_selection/__init__.py
--rw-rw-rw-   0        0        0    11028 2023-10-29 10:39:36.000000 tensorcross-1.0.0/tensorcross/model_selection/search.py
--rw-rw-rw-   0        0        0    11625 2023-10-29 10:39:36.000000 tensorcross-1.0.0/tensorcross/model_selection/search_cv.py
-drwxrwxrwx   0        0        0        0 2023-10-29 10:46:18.526562 tensorcross-1.0.0/tensorcross/utils/
--rw-rw-rw-   0        0        0      120 2023-10-29 10:39:36.000000 tensorcross-1.0.0/tensorcross/utils/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-10-29 10:39:36.000000 tensorcross-1.0.0/tensorcross/utils/dataset.py
--rw-rw-rw-   0        0        0       22 2023-10-29 10:39:36.000000 tensorcross-1.0.0/tensorcross/version.py
-drwxrwxrwx   0        0        0        0 2023-10-29 10:46:18.521563 tensorcross-1.0.0/tensorcross.egg-info/
--rw-rw-rw-   0        0        0      864 2023-10-29 10:46:18.000000 tensorcross-1.0.0/tensorcross.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-10-29 10:46:18.000000 tensorcross-1.0.0/tensorcross.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-29 10:46:18.000000 tensorcross-1.0.0/tensorcross.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-10-29 10:46:18.000000 tensorcross-1.0.0/tensorcross.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-29 10:46:18.000000 tensorcross-1.0.0/tensorcross.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-29 10:46:18.531561 tensorcross-1.0.0/tests/
--rw-rw-rw-   0        0        0     2359 2023-10-29 10:31:12.000000 tensorcross-1.0.0/tests/test_grid_search.py
--rw-rw-rw-   0        0        0     1926 2023-10-29 10:31:12.000000 tensorcross-1.0.0/tests/test_grid_search_cv.py
--rw-rw-rw-   0        0        0     2492 2023-10-29 10:31:12.000000 tensorcross-1.0.0/tests/test_random_search.py
--rw-rw-rw-   0        0        0     2021 2023-10-29 10:31:12.000000 tensorcross-1.0.0/tests/test_random_search_cv.py
--rw-rw-rw-   0        0        0     2798 2023-10-29 10:31:12.000000 tensorcross-1.0.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:06:06.543215 tensorcross-2.0.0/
+-rw-rw-rw-   0        0        0     1110 2021-06-24 10:48:25.000000 tensorcross-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      897 2024-05-20 19:06:06.542213 tensorcross-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5636 2023-10-29 10:38:59.000000 tensorcross-2.0.0/README.md
+-rw-rw-rw-   0        0        0     4218 2024-03-10 09:22:58.000000 tensorcross-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 19:06:06.543215 tensorcross-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2024-05-20 18:43:03.000000 tensorcross-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:06:06.467099 tensorcross-2.0.0/tensorcross/
+-rw-rw-rw-   0        0        0       65 2023-10-29 10:39:36.000000 tensorcross-2.0.0/tensorcross/__init__.py
+-rw-rw-rw-   0        0        0      270 2024-05-20 18:42:36.000000 tensorcross-2.0.0/tensorcross/_types.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:06:06.497649 tensorcross-2.0.0/tensorcross/model_selection/
+-rw-rw-rw-   0        0        0      355 2024-02-11 10:32:48.000000 tensorcross-2.0.0/tensorcross/model_selection/__init__.py
+-rw-rw-rw-   0        0        0    11010 2024-02-11 10:34:19.000000 tensorcross-2.0.0/tensorcross/model_selection/search.py
+-rw-rw-rw-   0        0        0    11879 2024-05-20 18:50:06.000000 tensorcross-2.0.0/tensorcross/model_selection/search_cv.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:06:06.508163 tensorcross-2.0.0/tensorcross/utils/
+-rw-rw-rw-   0        0        0      120 2024-02-11 10:32:48.000000 tensorcross-2.0.0/tensorcross/utils/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-10-29 10:39:36.000000 tensorcross-2.0.0/tensorcross/utils/dataset.py
+-rw-rw-rw-   0        0        0       22 2024-05-20 18:43:03.000000 tensorcross-2.0.0/tensorcross/version.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:06:06.541211 tensorcross-2.0.0/tensorcross.egg-info/
+-rw-rw-rw-   0        0        0      897 2024-05-20 19:06:06.000000 tensorcross-2.0.0/tensorcross.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2024-05-20 19:06:06.000000 tensorcross-2.0.0/tensorcross.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 19:06:06.000000 tensorcross-2.0.0/tensorcross.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-20 19:06:06.000000 tensorcross-2.0.0/tensorcross.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 19:06:06.000000 tensorcross-2.0.0/tensorcross.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 19:06:06.540212 tensorcross-2.0.0/tests/
+-rw-rw-rw-   0        0        0     2362 2024-05-20 18:43:03.000000 tensorcross-2.0.0/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0     1929 2024-05-20 18:43:03.000000 tensorcross-2.0.0/tests/test_grid_search_cv.py
+-rw-rw-rw-   0        0        0     2495 2024-05-20 18:43:03.000000 tensorcross-2.0.0/tests/test_random_search.py
+-rw-rw-rw-   0        0        0     2024 2024-05-20 18:43:03.000000 tensorcross-2.0.0/tests/test_random_search_cv.py
+-rw-rw-rw-   0        0        0     2798 2023-10-29 10:31:12.000000 tensorcross-2.0.0/tests/test_utils.py
```

### Comparing `tensorcross-1.0.0/LICENSE` & `tensorcross-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcross-1.0.0/PKG-INFO` & `tensorcross-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcross
-Version: 1.0.0
+Version: 2.0.0
 Summary: Cross Validation, Grid Search and Random Search for TensorFlow Datasets.
 Author: Jan Schaffranek, Saif Al-Dilaimi
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
 Programming Language :: Python :: 3.11
@@ -13,13 +13,14 @@
 Operating System :: Microsoft :: Windows
 Operating System :: POSIX
 Operating System :: Unix
 Operating System :: MacOS
 
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: keras>=2.8
+Requires-Dist: tensorflow>=2.13
+Requires-Dist: keras>=3.0
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn>=1.0
 
 Cross Validation, Grid Search and Random Search for TensorFlow Datasets. For more information see here: https://github.com/franneck94/TensorCross
```

### Comparing `tensorcross-1.0.0/README.md` & `tensorcross-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tensorcross-1.0.0/setup.py` & `tensorcross-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,21 @@
     "https://github.com/franneck94/TensorCross"
 )
 
 VERSION = __version__
 ISRELEASED = False
 
 MIN_PYTHON_VERSION = "3.9"
-INSTALL_REQUIRES = ["keras>=2.8", "numpy", "scipy", "scikit-learn>=1.0"]
+INSTALL_REQUIRES = [
+    "tensorflow>=2.13",
+    "keras>=3.0",
+    "numpy",
+    "scipy",
+    "scikit-learn>=1.0",
+]
 
 
 PACKAGES = find_packages(include=["tensorcross", "tensorcross.*"])
 
 metadata = dict(  # noqa: C408
     name=DISTNAME,
     version=VERSION,
```

### Comparing `tensorcross-1.0.0/tensorcross/model_selection/search.py` & `tensorcross-2.0.0/tensorcross/model_selection/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 import os
-from abc import ABCMeta
+from abc import ABC
 from abc import abstractmethod
 from collections.abc import Iterable
 from collections.abc import Mapping
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
@@ -21,15 +21,15 @@
 
 from tensorcross._types import ResultsDict
 
 
 logger = tf.get_logger()
 
 
-class BaseSearch(metaclass=ABCMeta):
+class BaseSearch(ABC):
     """Abstract BaseSearch class for the grid or random search.
 
     Args:
         model_fn (Callable[..., Model]): Function that
             builds and compiles a Model object.
         verbose (int): Whether to show information in terminal.
             Defaults to 0.
```

### Comparing `tensorcross-1.0.0/tensorcross/model_selection/search_cv.py` & `tensorcross-2.0.0/tensorcross/model_selection/search_cv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 import os
-from abc import ABCMeta
+from abc import ABC
 from abc import abstractmethod
 from collections.abc import Iterable
 from collections.abc import Mapping
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
@@ -22,15 +22,15 @@
 from tensorcross._types import ResultsDict
 from tensorcross.utils import dataset_split
 
 
 logger = tf.get_logger()
 
 
-class BaseSearchCV(metaclass=ABCMeta):
+class BaseSearchCV(ABC):
     """Abstract BaseSearchCV class for the grid or random search
     with cross validation.
 
     Args:
         model_fn (Callable[..., Model]): Function that
             builds and compiles a Model object.
         n_folds (int): How many folds. Defaults to 3.
@@ -50,16 +50,18 @@
         self.model_fn = model_fn
         self.verbose = verbose
         self.n_folds = n_folds
         self.model_fn_kwargs = kwargs
         self.results_: ResultsDict = {
             "best_score": -np.inf,
             "best_params": {},
+            "best_model" : [],
             "val_scores": [],
             "params": [],
+            "models" : []
         }
 
     def _run_search(  # noqa: PLR0912
         self,
         dataset: tf.data.Dataset,
         parameter_obj: Union[ParameterGrid, ParameterSampler],
         **kwargs: Any,
@@ -70,15 +72,16 @@
             dataset (tf.data.Dataset): tf.data.Dataset object for the training.
             parameter_obj (ParameterGrid | ParameterSampler): Object to iterate
                 over, to generate hyperparameter combinations.
             kwargs (Any): Keyword arguments for the fit method of the
                 Model or tf.keras.models.Sequential model.
         """
         if len(dataset) == 0:
-            raise ValueError("Data Set is empty!")
+            error_msg = "Validation Set is empty!"
+            raise ValueError(error_msg)
 
         maximize = True
         tensorboard_callback: Optional[TensorBoard] = None
         tensorboard_log_dir = ""
 
         for param, value in kwargs.items():
             if param == "callbacks":
@@ -108,15 +111,16 @@
                     **grid_combination, **self.model_fn_kwargs
                 )
 
                 train_dataset, val_dataset = dataset_split(
                     dataset=dataset, split_fraction=split_fraction, fold=fold
                 )
                 if len(val_dataset) == 0:
-                    raise ValueError("Val Set is empty!")
+                    error_msg = "Validation Set is empty!"
+                    raise ValueError(error_msg)
 
                 if tensorboard_callback:
                     if not os.path.exists(tensorboard_log_dir):
                         os.mkdir(tensorboard_log_dir)
                     new_log_dir = os.path.join(
                         tensorboard_log_dir, f"model_{idx}_fold_{fold}"
                     )
@@ -130,24 +134,26 @@
                 else:
                     maximize = False
                     val_score = model.evaluate(val_dataset, verbose=0)
                 val_scores[fold] = val_score
 
             self.results_["val_scores"].append(val_scores)
             self.results_["params"].append(grid_combination)
+            self.results_["models"].append(model)
 
         logger.setLevel(tf_log_level)  # Issue 30
 
         mean_val_scores = np.mean(self.results_["val_scores"], axis=1)
         if maximize:
             best_run_idx = np.argmax(mean_val_scores)
         else:
             best_run_idx = np.argmin(mean_val_scores)
         self.results_["best_score"] = self.results_["val_scores"][best_run_idx]
         self.results_["best_params"] = self.results_["params"][best_run_idx]
+        self.results_["best_model"] = self.results_["models"][best_run_idx]
 
     def summary(self) -> str:
         """Prints the summary of the search to the console.
 
         Assuming the *RandomSearch* had n iterations or the
         *GridSearch* had n combinations in total, the output
         would have the following structure:
```

### Comparing `tensorcross-1.0.0/tensorcross/utils/dataset.py` & `tensorcross-2.0.0/tensorcross/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcross-1.0.0/tensorcross.egg-info/PKG-INFO` & `tensorcross-2.0.0/tensorcross.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcross
-Version: 1.0.0
+Version: 2.0.0
 Summary: Cross Validation, Grid Search and Random Search for TensorFlow Datasets.
 Author: Jan Schaffranek, Saif Al-Dilaimi
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
 Programming Language :: Python :: 3.11
@@ -13,13 +13,14 @@
 Operating System :: Microsoft :: Windows
 Operating System :: POSIX
 Operating System :: Unix
 Operating System :: MacOS
 
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: keras>=2.8
+Requires-Dist: tensorflow>=2.13
+Requires-Dist: keras>=3.0
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn>=1.0
 
 Cross Validation, Grid Search and Random Search for TensorFlow Datasets. For more information see here: https://github.com/franneck94/TensorCross
```

### Comparing `tensorcross-1.0.0/tensorcross.egg-info/SOURCES.txt` & `tensorcross-2.0.0/tensorcross.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 tensorcross/__init__.py
 tensorcross/_types.py
 tensorcross/version.py
 tensorcross.egg-info/PKG-INFO
 tensorcross.egg-info/SOURCES.txt
 tensorcross.egg-info/dependency_links.txt
```

### Comparing `tensorcross-1.0.0/tests/test_grid_search.py` & `tensorcross-2.0.0/tests/test_grid_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 def build_model(
     num_features: int,
     num_targets: int,
     optimizer: Optimizer,
     learning_rate: float,
 ) -> Model:
     """Build the test model."""
-    x_input = Input(shape=num_features)
+    x_input = Input(shape=(num_features,))
     y_pred = Dense(units=num_targets)(x_input)
     model = Model(inputs=[x_input], outputs=[y_pred])
 
     opt = optimizer(learning_rate=learning_rate)
 
     model.compile(loss="mse", optimizer=opt, metrics=["mse"])
```

### Comparing `tensorcross-1.0.0/tests/test_grid_search_cv.py` & `tensorcross-2.0.0/tests/test_grid_search_cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 def build_model(
     num_features: int,
     num_targets: int,
     optimizer: Optimizer,
     learning_rate: float,
 ) -> Model:
     """Build the test model."""
-    x_input = Input(shape=num_features)
+    x_input = Input(shape=(num_features,))
     y_pred = Dense(units=num_targets)(x_input)
     model = Model(inputs=[x_input], outputs=[y_pred])
 
     opt = optimizer(learning_rate=learning_rate)
 
     model.compile(loss="mse", optimizer=opt, metrics=["mse"])
```

### Comparing `tensorcross-1.0.0/tests/test_random_search.py` & `tensorcross-2.0.0/tests/test_random_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 def build_model(
     num_features: int,
     num_targets: int,
     optimizer: Optimizer,
     learning_rate: float,
 ) -> Model:
     """Build the test model."""
-    x_input = Input(shape=num_features)
+    x_input = Input(shape=(num_features,))
     y_pred = Dense(units=num_targets)(x_input)
     model = Model(inputs=[x_input], outputs=[y_pred])
 
     opt = optimizer(learning_rate=learning_rate)
 
     model.compile(loss="mse", optimizer=opt, metrics=["mse"])
```

### Comparing `tensorcross-1.0.0/tests/test_random_search_cv.py` & `tensorcross-2.0.0/tests/test_random_search_cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def build_model(
     num_features: int,
     num_targets: int,
     optimizer: Optimizer,
     learning_rate: float,
 ) -> Model:
     """Build the test model."""
-    x_input = Input(shape=num_features)
+    x_input = Input(shape=(num_features,))
     y_pred = Dense(units=num_targets)(x_input)
     model = Model(inputs=[x_input], outputs=[y_pred])
 
     opt = optimizer(learning_rate=learning_rate)
 
     model.compile(loss="mse", optimizer=opt, metrics=["mse"])
```

### Comparing `tensorcross-1.0.0/tests/test_utils.py` & `tensorcross-2.0.0/tests/test_utils.py`

 * *Files identical despite different names*


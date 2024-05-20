# Comparing `tmp/EQL-NN-2.0.2.tar.gz` & `tmp/eql_nn-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EQL-NN-2.0.2.tar", last modified: Wed Nov 15 22:21:04 2023, max compression
+gzip compressed data, was "eql_nn-2.1.0.tar", last modified: Mon May 20 21:12:02 2024, max compression
```

## Comparing `EQL-NN-2.0.2.tar` & `eql_nn-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:21:04.589472 EQL-NN-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:21:04.589472 EQL-NN-2.0.2/EQL/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 22:20:55.000000 EQL-NN-2.0.2/EQL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2023-11-15 22:20:55.000000 EQL-NN-2.0.2/EQL/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26217 2023-11-15 22:20:55.000000 EQL-NN-2.0.2/EQL/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 22:21:04.589472 EQL-NN-2.0.2/EQL_NN.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-11-15 22:21:04.000000 EQL-NN-2.0.2/EQL_NN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-15 22:21:04.000000 EQL-NN-2.0.2/EQL_NN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 22:21:04.000000 EQL-NN-2.0.2/EQL_NN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-15 22:21:04.000000 EQL-NN-2.0.2/EQL_NN.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-15 22:21:04.000000 EQL-NN-2.0.2/EQL_NN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-11-15 22:20:55.000000 EQL-NN-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-11-15 22:20:55.000000 EQL-NN-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-11-15 22:21:04.589472 EQL-NN-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2023-11-15 22:20:55.000000 EQL-NN-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 22:21:04.589472 EQL-NN-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-11-15 22:20:55.000000 EQL-NN-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:12:02.781601 eql_nn-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:12:02.781601 eql_nn-2.1.0/EQL/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:11:58.000000 eql_nn-2.1.0/EQL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-20 21:11:58.000000 eql_nn-2.1.0/EQL/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29618 2024-05-20 21:11:58.000000 eql_nn-2.1.0/EQL/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:12:02.781601 eql_nn-2.1.0/EQL_NN.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-20 21:12:02.000000 eql_nn-2.1.0/EQL_NN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-20 21:12:02.000000 eql_nn-2.1.0/EQL_NN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:12:02.000000 eql_nn-2.1.0/EQL_NN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 21:12:02.000000 eql_nn-2.1.0/EQL_NN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 21:12:02.000000 eql_nn-2.1.0/EQL_NN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 21:11:58.000000 eql_nn-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-20 21:11:58.000000 eql_nn-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-20 21:12:02.781601 eql_nn-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-20 21:11:58.000000 eql_nn-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:12:02.781601 eql_nn-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-20 21:11:58.000000 eql_nn-2.1.0/setup.py
```

### Comparing `EQL-NN-2.0.2/EQL/layer.py` & `eql_nn-2.1.0/EQL/layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 def sigmoid(out, index):
     return tf.sigmoid(tf.gather(out, [index], axis=1), name='sig_output')
 
 
 def mult(out, index):
     sum1 = tf.gather(out, [index], axis=1)
     sum2 = tf.gather(out, [index + 1], axis=1)
-    sum_input = tf.add(sum1, sum2)
-    return tf.multiply(sum_input, sum_input, name='mult_output')
+    return tf.multiply(sum1, sum2, name='mult_output')
 
 
 class EqlLayer(keras.layers.Layer):
     def __init__(self, w_initializer, b_initializer, v, lmbda=0, mask=None, exclude=None):
         super(EqlLayer, self).__init__()
         if exclude is None:
             exclude = []
@@ -51,14 +50,21 @@
         if 'sig' in exclude:
             self.exclusion += 1
             self.activations.remove(sigmoid)
         if 'mult' in exclude:
             self.exclusion += 2
             self.activations.remove(mult)
 
+    def _mask(self):
+        for i in range(self.w.shape[0]):
+            w_mask = tf.matmul([self.w[i]], self.mask[0][i])[0]
+            self.w[i].assign(w_mask)
+        b_mask = tf.matmul([self.b], self.mask[1])[0]
+        self.b.assign(b_mask)
+
     def build(self, input_shape):
         self.w = self.add_weight(
             shape=(input_shape[-1], 6 * self.v - self.v * self.exclusion),
             initializer=self.w_initializer,
             trainable=True, regularizer=self.regularizer
         )
         self.b = self.add_weight(
@@ -89,17 +95,25 @@
     def __init__(self, w_initializer, b_initializer, lmbda=0, mask=None):
         super(DenseLayer, self).__init__()
         self.regularizer = regularizers.L1(l1=lmbda)
         self.w_initializer = initializers.get(w_initializer)
         self.b_initializer = initializers.get(b_initializer)
         self.mask = mask
 
+
+    def _mask(self):
+        for i in range(self.w.shape[0]):
+            w_mask = tf.matmul([self.w[i]], self.mask[0][i])[0]
+            self.w[i].assign(w_mask)
+        b_mask = tf.matmul([self.b], self.mask[1])[0]
+        self.b.assign(b_mask)
+
     def build(self, input_shape):
         self.w = self.add_weight(
-            shape=(input_shape[-1], 1),
+            shape=(input_shape[-1], 1), #TODO: Output of dense layer is 1, maybe change this for multi-dimensionality
             initializer=self.w_initializer,
             trainable=True, regularizer=self.regularizer
         )
         self.b = self.add_weight(
             shape=(1,), initializer=self.b_initializer, trainable=True, regularizer=self.regularizer
         )
```

### Comparing `EQL-NN-2.0.2/EQL/model.py` & `eql_nn-2.1.0/EQL/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import tensorflow as tf
 
 from tensorflow import keras
 import numpy as np
+from sympy import *
+from math import floor
 from EQL.layer import EqlLayer, DenseLayer
 
 
 class EQL:
     """
     EQL model class, here we build our model and specify training processes and architecture
     """
@@ -309,14 +311,16 @@
             if verbose != 0:
                 print('Beginning L0 Training, T2_epochs = ' + str(t2))
             self.model.fit(x, y, batch_size, t2, verbose, callbacks,
                            validation_split, validation_data, shuffle, class_weight,
                            sample_weight, initial_epoch, steps_per_epoch,
                            validation_steps, validation_batch_size, validation_freq,
                            max_queue_size, workers, use_multiprocessing)
+            for layer in self.model.layers[1:]:
+                layer._mask()
 
     def predict(self, x, batch_size=None, verbose=0, steps=None, callbacks=None, max_queue_size=10,
                 workers=1, use_multiprocessing=False):
         """
         Generates output predictions for the input samples.
 
         Computation is done in batches. This method is designed for performance in large scale inputs. For small amount
@@ -377,14 +381,83 @@
         :param layer: Specified layer number to get weights from
         :type layer: int
         :return: Array of weights and biases in certain layer
         :rtype: np.ndarray
         """
         return self.model.layers[layer].get_weights()
 
+    def formula(self, raw_latex=False, reduce=True):
+        init_printing()
+
+        num_layers = self.num_layers + 1 # EQL + Dense
+        input_dim = len(self.get_weights(1)[0])
+
+        output = {}
+        # Looping through EQL layers
+        for layer in range(1, num_layers):
+            previous_output = output
+            output = {}
+            input_dim = len(self.get_weights(layer)[0])
+            prev_keys = list(previous_output.keys())
+            # Looping through input dimension of layer
+            for dim in range(input_dim):
+                layer_weights = self.get_weights(layer)[0][dim]
+                layer_biases = self.get_weights(layer)[1]
+                weight_index = 0
+                # Handling first layer defining sympy symbols
+                if layer == 1:
+                    symbol = symbols(f'x_{dim+1}')
+                else:
+                    symbol = previous_output[prev_keys[dim]]
+                # Looping through number of nodes in next layer, v * activations
+                for num_repetition in range(self.v[layer-1]):
+                    for activation in self.model.layers[layer].activations:
+                        if activation.__name__ == 'mult':
+                            if dim == 0:
+                                output[f'{activation.__name__}{num_repetition}'] = [layer_biases[weight_index], layer_biases[weight_index+1]]
+                            output[f'{activation.__name__}{num_repetition}'][0] += layer_weights[weight_index] * symbol
+                            output[f'{activation.__name__}{num_repetition}'][1] += layer_weights[weight_index+1] * symbol
+                            weight_index += 1 # Skip over second mult node
+                        else:
+                            if dim == 0:
+                                output[f'{activation.__name__}{num_repetition}'] = layer_biases[weight_index]
+                            output[f'{activation.__name__}{num_repetition}'] +=  layer_weights[weight_index] * symbol
+                        weight_index += 1
+                    
+            for activation in output.keys():
+                if 'sin' in activation:
+                    output[activation] = sin(output[activation])
+                elif 'cos' in activation:
+                    output[activation] = cos(output[activation])
+                elif 'identity' in activation:
+                    continue
+                elif 'sigmoid' in activation:
+                    output[activation] = Function('\sigma')(output[activation])
+                elif 'mult' in activation:
+                    output[activation] = output[activation][0] * output[activation][1]
+                else:
+                    raise Exception(activation, 'Not a valid activation')
+
+        # DenseLayer
+        f = 0
+        layer = self.get_weights(len(self.model.layers)-1)
+         # Looping through weights for each input dimension
+        for dim in range(len(layer[0])):
+            if dim == 0:
+                f += layer[1][0]
+            # Looping through activation functions of previous layer
+            f += layer[0][dim][0] * output[list(output.keys())[dim]]
+
+        if reduce:
+            f = simplify(f)
+        if raw_latex:
+            return latex(f)
+        else:
+            return f
+
     def set_weights(self, layer, weights):
         """
         :param layer: Specified layer number to set weights in
         :type layer: int
         :param weights: Array of weights, must match dimensionality of specified model layer
         :type weights: np.ndarray
         """
```

### Comparing `EQL-NN-2.0.2/EQL_NN.egg-info/PKG-INFO` & `eql_nn-2.1.0/EQL_NN.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: EQL-NN
-Version: 2.0.2
+Version: 2.1.0
 Summary: A Tensorflow implementation of the Equation Learning Based Neural Network Model
 Home-page: https://github.com/KristofPusztai/EQL
 Author: Kristof Pusztai
 Author-email: kpusztai@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tensorflow>=2.11
 Requires-Dist: numpy
+Requires-Dist: sympy
 
 [![GitHub Action Badge](https://github.com/KristofPusztai/EQL/actions/workflows/pytest.yml/badge.svg)](https://github.com/KristofPusztai/EQL/actions)
-
 [![codecov](https://codecov.io/gh/KristofPusztai/EQL/graph/badge.svg?token=5BLB6GHC7S)](https://codecov.io/gh/KristofPusztai/EQL)
-
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/KristofPusztai/EQL?style=plastic)](https://pypi.org/project/EQL-NN/)
-
 [![PyPI - License](https://img.shields.io/pypi/l/EQL-NN)](https://opensource.org/license/mit/)
-
 [![Downloads](https://static.pepy.tech/badge/eql-nn)](https://pepy.tech/project/eql-nn)
-
 [![GitHub issues](https://img.shields.io/github/issues/KristofPusztai/EQL)](https://github.com/KristofPusztai/EQL/issues)
 
 # Introduction:
 
 A tensorflow implementation of the Equation Learner Neural Network based model:
 ![Imgur](https://i.imgur.com/L77pz3d.png)
 - https://arxiv.org/pdf/1610.02995.pdf
@@ -73,14 +69,15 @@
 There are a variety of methods for understanding what is going on
 in your model.
 
     EQLmodel.summary() # Provides tensorflow summary
     EQLmodel.count_params() # Provides # trainable params
     EQLmodel.get_weights(layer) #returns array of layer values
     EQLmodel.set_weights(layer, weights) #sets weights of specified layer
+    EQLmodel.formula(raw_latex=False, reduce=True) # Returns interpretable equations via sympy
     
     EQLmodel.evaluate(x=None, y=None, batch_size=None, verbose=1,
                       sample_weight=None, steps=None,
                       callbacks=None, max_queue_size=10, 
                       workers=1, use_multiprocessing=False,
                       return_dict=False)
     # Returns the loss value & metrics values for the model
```

### Comparing `EQL-NN-2.0.2/LICENSE` & `eql_nn-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EQL-NN-2.0.2/PKG-INFO` & `eql_nn-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: EQL-NN
-Version: 2.0.2
+Version: 2.1.0
 Summary: A Tensorflow implementation of the Equation Learning Based Neural Network Model
 Home-page: https://github.com/KristofPusztai/EQL
 Author: Kristof Pusztai
 Author-email: kpusztai@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tensorflow>=2.11
 Requires-Dist: numpy
+Requires-Dist: sympy
 
 [![GitHub Action Badge](https://github.com/KristofPusztai/EQL/actions/workflows/pytest.yml/badge.svg)](https://github.com/KristofPusztai/EQL/actions)
-
 [![codecov](https://codecov.io/gh/KristofPusztai/EQL/graph/badge.svg?token=5BLB6GHC7S)](https://codecov.io/gh/KristofPusztai/EQL)
-
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/KristofPusztai/EQL?style=plastic)](https://pypi.org/project/EQL-NN/)
-
 [![PyPI - License](https://img.shields.io/pypi/l/EQL-NN)](https://opensource.org/license/mit/)
-
 [![Downloads](https://static.pepy.tech/badge/eql-nn)](https://pepy.tech/project/eql-nn)
-
 [![GitHub issues](https://img.shields.io/github/issues/KristofPusztai/EQL)](https://github.com/KristofPusztai/EQL/issues)
 
 # Introduction:
 
 A tensorflow implementation of the Equation Learner Neural Network based model:
 ![Imgur](https://i.imgur.com/L77pz3d.png)
 - https://arxiv.org/pdf/1610.02995.pdf
@@ -73,14 +69,15 @@
 There are a variety of methods for understanding what is going on
 in your model.
 
     EQLmodel.summary() # Provides tensorflow summary
     EQLmodel.count_params() # Provides # trainable params
     EQLmodel.get_weights(layer) #returns array of layer values
     EQLmodel.set_weights(layer, weights) #sets weights of specified layer
+    EQLmodel.formula(raw_latex=False, reduce=True) # Returns interpretable equations via sympy
     
     EQLmodel.evaluate(x=None, y=None, batch_size=None, verbose=1,
                       sample_weight=None, steps=None,
                       callbacks=None, max_queue_size=10, 
                       workers=1, use_multiprocessing=False,
                       return_dict=False)
     # Returns the loss value & metrics values for the model
```

### Comparing `EQL-NN-2.0.2/README.md` & `eql_nn-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 [![GitHub Action Badge](https://github.com/KristofPusztai/EQL/actions/workflows/pytest.yml/badge.svg)](https://github.com/KristofPusztai/EQL/actions)
-
 [![codecov](https://codecov.io/gh/KristofPusztai/EQL/graph/badge.svg?token=5BLB6GHC7S)](https://codecov.io/gh/KristofPusztai/EQL)
-
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/KristofPusztai/EQL?style=plastic)](https://pypi.org/project/EQL-NN/)
-
 [![PyPI - License](https://img.shields.io/pypi/l/EQL-NN)](https://opensource.org/license/mit/)
-
 [![Downloads](https://static.pepy.tech/badge/eql-nn)](https://pepy.tech/project/eql-nn)
-
 [![GitHub issues](https://img.shields.io/github/issues/KristofPusztai/EQL)](https://github.com/KristofPusztai/EQL/issues)
 
 # Introduction:
 
 A tensorflow implementation of the Equation Learner Neural Network based model:
 ![Imgur](https://i.imgur.com/L77pz3d.png)
 - https://arxiv.org/pdf/1610.02995.pdf
@@ -57,14 +52,15 @@
 There are a variety of methods for understanding what is going on
 in your model.
 
     EQLmodel.summary() # Provides tensorflow summary
     EQLmodel.count_params() # Provides # trainable params
     EQLmodel.get_weights(layer) #returns array of layer values
     EQLmodel.set_weights(layer, weights) #sets weights of specified layer
+    EQLmodel.formula(raw_latex=False, reduce=True) # Returns interpretable equations via sympy
     
     EQLmodel.evaluate(x=None, y=None, batch_size=None, verbose=1,
                       sample_weight=None, steps=None,
                       callbacks=None, max_queue_size=10, 
                       workers=1, use_multiprocessing=False,
                       return_dict=False)
     # Returns the loss value & metrics values for the model
```

### Comparing `EQL-NN-2.0.2/setup.py` & `eql_nn-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EQL-NN",
-    version="2.0.2", # MAJOR.MINOR.MAINTENANCE
+    version="2.1.0", # MAJOR.MINOR.MAINTENANCE
     author="Kristof Pusztai",
     author_email="kpusztai@berkeley.edu",
     description="A Tensorflow implementation of the Equation Learning Based Neural Network Model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KristofPusztai/EQL",
     packages=setuptools.find_packages(),
     install_requires=[
         'tensorflow>=2.11',
-        'numpy'
+        'numpy',
+        'sympy'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
```


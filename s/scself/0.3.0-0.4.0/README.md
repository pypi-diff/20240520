# Comparing `tmp/scself-0.3.0.tar.gz` & `tmp/scself-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scself-0.3.0.tar", last modified: Thu May 16 15:57:27 2024, max compression
+gzip compressed data, was "scself-0.4.0.tar", last modified: Mon May 20 17:14:09 2024, max compression
```

## Comparing `scself-0.3.0.tar` & `scself-0.4.0.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.290478 scself-0.3.0/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1122 2024-05-06 19:22:25.000000 scself-0.3.0/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     1393 2024-05-16 15:57:27.290478 scself-0.3.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      848 2024-05-15 16:20:07.000000 scself-0.3.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.286477 scself-0.3.0/scself/
--rw-rw-r--   0 chris     (1000) chris     (1000)      282 2024-05-15 17:00:18.000000 scself-0.3.0/scself/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.286477 scself-0.3.0/scself/_mcv/
--rw-rw-r--   0 chris     (1000) chris     (1000)       85 2024-05-10 13:43:03.000000 scself-0.3.0/scself/_mcv/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3386 2024-05-14 16:32:20.000000 scself-0.3.0/scself/_mcv/common.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2696 2024-05-10 15:45:08.000000 scself-0.3.0/scself/_mcv/mcv_per_cell.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3148 2024-05-14 16:22:17.000000 scself-0.3.0/scself/_mcv/molecular_crossvalidation.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.290478 scself-0.3.0/scself/_noise2self/
--rw-rw-r--   0 chris     (1000) chris     (1000)      112 2024-05-15 17:18:49.000000 scself-0.3.0/scself/_noise2self/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5798 2024-05-16 15:17:41.000000 scself-0.3.0/scself/_noise2self/common.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6634 2024-05-15 16:07:07.000000 scself-0.3.0/scself/_noise2self/graph.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6670 2024-05-16 15:17:48.000000 scself-0.3.0/scself/_noise2self/multimodal_n2s.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5637 2024-05-15 19:48:10.000000 scself-0.3.0/scself/_noise2self/n2s.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.290478 scself-0.3.0/scself/scaling/
--rw-rw-r--   0 chris     (1000) chris     (1000)       76 2024-05-06 19:59:56.000000 scself-0.3.0/scself/scaling/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1363 2024-05-06 19:59:29.000000 scself-0.3.0/scself/scaling/truncscaler.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.290478 scself-0.3.0/scself/sparse/
--rw-rw-r--   0 chris     (1000) chris     (1000)      191 2024-05-06 20:01:16.000000 scself-0.3.0/scself/sparse/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1847 2024-05-06 20:17:13.000000 scself-0.3.0/scself/sparse/graph.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7413 2024-05-14 16:56:55.000000 scself-0.3.0/scself/sparse/math.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10626 2024-05-06 20:56:50.000000 scself-0.3.0/scself/sparse/truncated_svd.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.290478 scself-0.3.0/scself/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-05-06 21:01:57.000000 scself-0.3.0/scself/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1509 2024-02-29 17:23:43.000000 scself-0.3.0/scself/tests/_stubs.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7413 2024-05-14 16:57:15.000000 scself-0.3.0/scself/tests/test_math.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3993 2024-05-14 16:33:35.000000 scself-0.3.0/scself/tests/test_mcv.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      946 2024-05-07 18:20:28.000000 scself-0.3.0/scself/tests/test_mkl_hacks.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7209 2024-05-15 16:17:23.000000 scself-0.3.0/scself/tests/test_noise2self.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.290478 scself-0.3.0/scself/utils/
--rw-rw-r--   0 chris     (1000) chris     (1000)      303 2024-05-15 17:00:15.000000 scself-0.3.0/scself/utils/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1083 2024-05-09 21:07:13.000000 scself-0.3.0/scself/utils/_pca.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      762 2024-05-15 18:15:59.000000 scself-0.3.0/scself/utils/dot_product.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      557 2024-05-06 19:45:49.000000 scself-0.3.0/scself/utils/logging.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4622 2024-05-14 16:43:56.000000 scself-0.3.0/scself/utils/pairwise_loss.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2067 2024-05-10 15:11:33.000000 scself-0.3.0/scself/utils/standardization.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      984 2024-05-15 15:38:57.000000 scself-0.3.0/scself/utils/sum.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-16 15:57:27.290478 scself-0.3.0/scself.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     1393 2024-05-16 15:57:27.000000 scself-0.3.0/scself.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      990 2024-05-16 15:57:27.000000 scself-0.3.0/scself.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-16 15:57:27.000000 scself-0.3.0/scself.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-06 21:04:55.000000 scself-0.3.0/scself.egg-info/not-zip-safe
--rw-rw-r--   0 chris     (1000) chris     (1000)       78 2024-05-16 15:57:27.000000 scself-0.3.0/scself.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2024-05-16 15:57:27.000000 scself-0.3.0/scself.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-16 15:57:27.290478 scself-0.3.0/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     1092 2024-05-15 16:59:44.000000 scself-0.3.0/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.508574 scself-0.4.0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1122 2024-05-06 19:22:25.000000 scself-0.4.0/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     1393 2024-05-20 17:14:09.508574 scself-0.4.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      848 2024-05-15 16:20:07.000000 scself-0.4.0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.504574 scself-0.4.0/scself/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      317 2024-05-20 16:26:44.000000 scself-0.4.0/scself/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.504574 scself-0.4.0/scself/_denoise/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-20 16:27:01.000000 scself-0.4.0/scself/_denoise/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4294 2024-05-20 17:12:01.000000 scself-0.4.0/scself/_denoise/n2s_denoise.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.504574 scself-0.4.0/scself/_mcv/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       85 2024-05-10 13:43:03.000000 scself-0.4.0/scself/_mcv/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3386 2024-05-14 16:32:20.000000 scself-0.4.0/scself/_mcv/common.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2696 2024-05-10 15:45:08.000000 scself-0.4.0/scself/_mcv/mcv_per_cell.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3155 2024-05-18 18:46:27.000000 scself-0.4.0/scself/_mcv/molecular_crossvalidation.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.508574 scself-0.4.0/scself/_noise2self/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      112 2024-05-20 16:20:40.000000 scself-0.4.0/scself/_noise2self/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6435 2024-05-18 18:48:28.000000 scself-0.4.0/scself/_noise2self/common.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6485 2024-05-20 16:34:38.000000 scself-0.4.0/scself/_noise2self/graph.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7171 2024-05-17 19:42:49.000000 scself-0.4.0/scself/_noise2self/multimodal_n2s.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6130 2024-05-17 19:42:51.000000 scself-0.4.0/scself/_noise2self/n2s.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.508574 scself-0.4.0/scself/scaling/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       76 2024-05-06 19:59:56.000000 scself-0.4.0/scself/scaling/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1363 2024-05-06 19:59:29.000000 scself-0.4.0/scself/scaling/truncscaler.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.508574 scself-0.4.0/scself/sparse/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      191 2024-05-06 20:01:16.000000 scself-0.4.0/scself/sparse/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1960 2024-05-17 18:22:47.000000 scself-0.4.0/scself/sparse/graph.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7413 2024-05-14 16:56:55.000000 scself-0.4.0/scself/sparse/math.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10626 2024-05-06 20:56:50.000000 scself-0.4.0/scself/sparse/truncated_svd.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.508574 scself-0.4.0/scself/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-05-06 21:01:57.000000 scself-0.4.0/scself/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1509 2024-02-29 17:23:43.000000 scself-0.4.0/scself/tests/_stubs.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3679 2024-05-20 17:13:05.000000 scself-0.4.0/scself/tests/test_denoise.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7411 2024-05-17 18:22:38.000000 scself-0.4.0/scself/tests/test_math.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3993 2024-05-14 16:33:35.000000 scself-0.4.0/scself/tests/test_mcv.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      946 2024-05-07 18:20:28.000000 scself-0.4.0/scself/tests/test_mkl_hacks.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10619 2024-05-20 16:23:14.000000 scself-0.4.0/scself/tests/test_noise2self.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.508574 scself-0.4.0/scself/utils/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      303 2024-05-15 17:00:15.000000 scself-0.4.0/scself/utils/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1083 2024-05-09 21:07:13.000000 scself-0.4.0/scself/utils/_pca.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      762 2024-05-15 18:15:59.000000 scself-0.4.0/scself/utils/dot_product.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      557 2024-05-06 19:45:49.000000 scself-0.4.0/scself/utils/logging.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4622 2024-05-14 16:43:56.000000 scself-0.4.0/scself/utils/pairwise_loss.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2067 2024-05-10 15:11:33.000000 scself-0.4.0/scself/utils/standardization.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      984 2024-05-15 15:38:57.000000 scself-0.4.0/scself/utils/sum.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-20 17:14:09.508574 scself-0.4.0/scself.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1393 2024-05-20 17:14:09.000000 scself-0.4.0/scself.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1078 2024-05-20 17:14:09.000000 scself-0.4.0/scself.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-20 17:14:09.000000 scself-0.4.0/scself.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-06 21:04:55.000000 scself-0.4.0/scself.egg-info/not-zip-safe
+-rw-rw-r--   0 chris     (1000) chris     (1000)       78 2024-05-20 17:14:09.000000 scself-0.4.0/scself.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2024-05-20 17:14:09.000000 scself-0.4.0/scself.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-20 17:14:09.508574 scself-0.4.0/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1092 2024-05-20 16:21:31.000000 scself-0.4.0/setup.py
```

### Comparing `scself-0.3.0/LICENSE` & `scself-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/PKG-INFO` & `scself-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scself
-Version: 0.3.0
+Version: 0.4.0
 Summary: Self Supervised Tools for Single Cell Data
 Home-page: https://github.com/GreshamLab/sc_self_supervised
 Author: Chris Jackson
 Author-email: cj59@nyu.edu
 Maintainer: Chris Jackson
 Maintainer-email: cj59@nyu.edu
 Description-Content-Type: text/markdown
```

### Comparing `scself-0.3.0/README.md` & `scself-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/_mcv/common.py` & `scself-0.4.0/scself/_mcv/common.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/_mcv/mcv_per_cell.py` & `scself-0.4.0/scself/_mcv/mcv_per_cell.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/_mcv/molecular_crossvalidation.py` & `scself-0.4.0/scself/_mcv/molecular_crossvalidation.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 
         if sps.issparse(B.X):
             metric_arr[i, 0] = np.sum(B.X.data ** 2) / size
         else:
             metric_arr[i, 0] = np.sum(B.X ** 2) / size
 
         # Calculate metric for 1-n_pcs number of PCs
-        for j in tqdm.trange(1, n_pcs + 1):
-            log(f"Iter #{i}: {j} PCs", level=10)
+        for j in (pbar := tqdm.trange(1, n_pcs + 1)):
+            pbar.set_description(f"{j} PCs")
+
             metric_arr[i, j] = mcv_comp(
                 B.X,
                 A.obsm['X_pca'][:, 0:j],
                 A.varm['PCs'][:, 0:j].T,
                 metric=metric,
                 axis=None,
                 tss=metric_arr[i, 0],
```

### Comparing `scself-0.3.0/scself/_noise2self/common.py` & `scself-0.4.0/scself/_noise2self/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import scipy.sparse as sps
 import anndata as ad
+import tqdm
 
 from scself.utils import (
     dot,
     standardize_data,
     pairwise_metric,
     sparse_dot_patch
 )
@@ -44,23 +45,24 @@
     X,
     graphs,
     k,
     by_row=False,
     loss='mse',
     loss_kwargs={},
     connectivity=False,
-    chunk_size=10000
+    chunk_size=10000,
+    pbar=False
 ):
     """
     Find optimal number of neighbors for a given graph
 
     :param X: Data [M x N]
     :type X: np.ndarray, sp.spmatrix
-    :param graph: Graph
-    :type graph: np.ndarray, sp.spmatrix
+    :param graph: List or tuple of graphs [M x M]
+    :type graph: tuple(np.ndarray, sp.spmatrix)
     :param k: k values to search
     :type k: np.ndarray [K]
     :param by_row: Get optimal k for each observation,
         defaults to False
     :type by_row: bool, optional
     :param pbar: Show a progress bar, defaults to False
     :type pbar: bool
@@ -68,17 +70,29 @@
         for each k and each observation [K x M]
     :rtype: np.ndarray
     """
 
     n, _ = X.shape
     n_k = len(k)
 
+    if not isinstance(graphs, (list, tuple)):
+        raise ValueError(
+            f"graphs must be a list or tuple; "
+            f"{type(graphs)} provided"
+        )
+
+    n_modes = len(graphs)
     mses = np.zeros(n_k) if not by_row else np.zeros((n_k, n))
 
-    for i in range(n_k):
+    if pbar:
+        rfunc = tqdm.trange
+    else:
+        rfunc = range
+
+    for i in rfunc(n_k):
 
         k_graph = [
             # Convert to a row stochastic graph
             row_normalize(
                 # Extract k non-zero neighbors from the graph
                 local_optimal_knn(
                     graph.copy(),
@@ -86,15 +100,15 @@
                     keep='smallest'
                 ),
                 connectivity=connectivity
             )
             for graph in graphs
         ]
 
-        if len(k_graph) == 1:
+        if n_modes == 1:
             k_graph = k_graph[0]
         else:
             k_graph = combine_row_stochastic_graphs(k_graph)
 
         # Calculate mean squared error
         mses[i] = _noise_to_self_error(
             X,
@@ -113,32 +127,48 @@
     k_graph,
     by_row=False,
     metric='mse',
     chunk_size=10000,
     **loss_kwargs
 ):
 
-    if (metric == 'mse' and is_csr(X) and chunk_size is not None):
+    if (metric == 'mse' and is_csr(X)):
 
-        from ..sparse.graph import _chunk_graph_mse
+        from ..sparse.graph import chunk_graph_mse
 
         _n_row = X.shape[0]
-        _row_mse = np.zeros(X.shape[0], dtype=float)
 
-        for i in range(int(np.ceil(_n_row / chunk_size))):
-            _start = i * chunk_size
-            _end = min(_start + chunk_size, _n_row)
+        if chunk_size is None:
+            _n_chunks = 1
+        else:
+            _n_chunks = int(_n_row / chunk_size) + 1
 
-            _row_mse[_start:_end] = _chunk_graph_mse(
+        if _n_chunks == 1:
+            _row_mse = chunk_graph_mse(
                 X,
-                k_graph,
-                _start,
-                _end
+                k_graph
             )
 
+        else:
+            _row_mse = np.zeros(_n_row, dtype=float)
+
+            for i in range(_n_chunks):
+                _start = i * chunk_size
+                _end = min((i + 1) * chunk_size, _n_row)
+
+                if _end <= _start:
+                    break
+
+                _row_mse[_start:_end] = chunk_graph_mse(
+                    X,
+                    k_graph,
+                    _start,
+                    _end
+                )
+
     else:
         _row_mse = pairwise_metric(
             X,
             dot(k_graph, X, dense=not sps.issparse(X)),
             metric=metric,
             **loss_kwargs
         )
```

### Comparing `scself-0.3.0/scself/_noise2self/graph.py` & `scself-0.4.0/scself/_noise2self/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     return neighbor_graph
 
 
 def combine_row_stochastic_graphs(graphs):
     graph = functools.reduce(lambda x, y: x + y, graphs)
 
     rowsum = array_sum(graph, axis=1).astype(float)
+    rowsum[rowsum == 0] = 1.
 
     if np.all(rowsum == len(graphs)):
         if sps.issparse(graph):
             graph.data /= len(graphs)
         else:
             graph /= len(graphs)
 
@@ -142,34 +143,36 @@
 
     else:
         np.fill_diagonal(X, diag)
 
     return X
 
 
-def neighbor_graph(adata, pc, k, metric='euclidean'):
+def neighbor_graph(adata, pc, k, metric='euclidean', random_state=None):
     """
     Build neighbor graph in an AnnData object
     """
 
     if adata.n_obs < 25000:
 
         adata.obsp['distances'] = NearestNeighbors(
             n_neighbors=k,
             metric=metric,
-            n_jobs=-1
+            n_jobs=-1,
+            algorithm='brute'
         ).fit(adata.obsm['X_pca'][:, :pc]).kneighbors_graph()
 
     else:
         adata.obsp['distances'] = PyNNDescentTransformer(
             n_neighbors=k,
             n_jobs=None,
             metric=metric,
             n_trees=min(64, 5 + int(round((adata.n_obs) ** 0.5 / 20.0))),
             n_iters=max(5, int(round(np.log2(adata.n_obs)))),
+            random_state=random_state
         ).fit_transform(adata.obsm['X_pca'][:, :pc])
 
     # Enforce diagonal zeros on graph
     # Single precision floats
     set_diag(adata.obsp['distances'], 0)
     adata.obsp['distances'].data = adata.obsp['distances'].data.astype(
         np.float32
@@ -178,31 +181,22 @@
     return adata
 
 
 def _invert_distance_graph(graph):
 
     if sps.issparse(graph):
 
-        rowmean = array_sum(graph, axis=1).astype(float) / graph.shape[1]
-        rowmean[rowmean == 0] = 1.
-
-        _row_divide(graph, rowmean)
-        graph.data *= -1
-        np.exp(graph.data, out=graph.data, where=graph.data != 0)
+        _nonzero = graph.data != 0.
+        graph.data[_nonzero] = 1 / graph.data[_nonzero]
 
         return graph
 
     else:
 
-        rowmean = graph.mean(axis=1)
-        rowmean[rowmean == 0] = 1.
-
-        graph /= rowmean[:, None]
-        graph *= -1
-        np.exp(graph, out=graph, where=graph != 0)
+        np.divide(1, graph, out=graph, where=graph != 0)
 
         return graph
 
 
 def _dist_to_row_stochastic(graph):
 
     if sps.issparse(graph):
```

### Comparing `scself-0.3.0/scself/_noise2self/multimodal_n2s.py` & `scself-0.4.0/scself/_noise2self/multimodal_n2s.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     metric='euclidean',
     loss='mse',
     loss_kwargs={},
     return_errors=False,
     connectivity=False,
     pc_data=None,
     chunk_size=10000,
+    random_state=None,
     verbose=None
 ):
     """
     Select an optimal set of graph parameters based on noise2self
 
     :param count_data: Count data
     :type count_data: np.ndarray, sp.spmatrix
@@ -74,14 +75,15 @@
     :rtype: sp.sparse.csr_matrix, int, int, np.ndarray [int]
     """
 
     neighbors, npcs = _check_args(
         neighbors,
         npcs
     )
+    _max_neighbors = np.max(neighbors)
 
     if not isinstance(count_data, (list, tuple)):
         raise ValueError(
             f"count_data must be a list of count matrices; "
             f"{type(count_data)} provided"
         )
 
@@ -104,15 +106,18 @@
     for i in range(_n_modes):
 
         data_obj[i], expr_data[i] = _standardize(
             count_data[i],
             standardization_method
         )
 
-    log(f"Searching {len(npcs)} PC x {len(neighbors)} Neighbors space")
+    log(
+        f"Searching {len(npcs)} PCs [{np.min(npcs)}-{np.max(npcs)}] by "
+        f"{len(neighbors)} Neighbors [{np.min(neighbors)}-{_max_neighbors}]"
+    )
 
     for i in range(_n_modes):
         if pc_data[i] is not None:
             log(f"Using existing PCs {pc_data[i].shape}")
             data_obj[i].obsm['X_pca'] = pc_data[i]
 
         else:
@@ -121,25 +126,28 @@
     mses = np.zeros((len(npcs), len(neighbors)))
 
     if len(npcs) > 1:
 
         # Search for the smallest MSE for each n_pcs / k combination
         # Outer loop does PCs, because the distance graph has to be
         # recalculated when PCs changes
-        for i, pc in tqdm.tqdm(enumerate(npcs), total=len(npcs)):
+        for i, pc in (pbar := tqdm.tqdm(enumerate(npcs), total=len(npcs))):
+
+            pbar.set_description(f"{pc} PCs")
 
             # Calculate neighbor graph with the max number of neighbors
             # Faster to select only a subset of edges than to recalculate
             # (obviously)
             for i in range(_n_modes):
                 neighbor_graph(
                     data_obj[i],
                     pc,
-                    np.max(neighbors),
-                    metric=metric
+                    _max_neighbors,
+                    metric=metric,
+                    random_state=random_state
                 )
 
             # Search through the neighbors space
             mses[i, :] = _search_k(
                 expr_data[target_data_index],
                 [data_obj[i].obsp['distances'] for i in range(_n_modes)],
                 neighbors,
@@ -167,39 +175,47 @@
         op_k = None
 
     # Recalculate a k-NN graph from the optimal # of PCs
     for i in range(_n_modes):
         neighbor_graph(
             data_obj[i],
             npcs[op_pc],
-            np.max(neighbors),
-            metric=metric
+            _max_neighbors,
+            metric=metric,
+            random_state=random_state
         )
 
     # Search space for k-neighbors
     local_neighbors = np.arange(
         np.min(neighbors) if len(neighbors) > 1 else 1,
-        np.max(neighbors)
+        _max_neighbors + 1
     )
 
+    log(f"Searching local k ({local_neighbors[0]}-{local_neighbors[-1]})")
+
     # Search for the optimal number of k for each obs
     # For the global optimal n_pc
-    local_k = local_neighbors[np.argmin(
-        _search_k(
-            expr_data[target_data_index],
-            [data_obj[i].obsp['distances'] for i in range(_n_modes)],
-            local_neighbors,
-            by_row=True,
-            connectivity=connectivity,
-            loss=loss,
-            loss_kwargs=loss_kwargs,
-            chunk_size=chunk_size
-        ),
-        axis=0
-    )]
+    local_error = _search_k(
+        expr_data[target_data_index],
+        [data_obj[i].obsp['distances'] for i in range(_n_modes)],
+        local_neighbors,
+        by_row=True,
+        connectivity=connectivity,
+        loss=loss,
+        loss_kwargs=loss_kwargs,
+        chunk_size=chunk_size,
+        pbar=True
+    )
+
+    local_k = local_neighbors[np.argmin(local_error, axis=0)]
+
+    log(
+        f"Optimal local k complete ({local_k.min()}-{local_k.max()}, "
+        f"mean={local_k.mean():.2f})"
+    )
 
     # Pack return object:
     # Optimal (variable-k) graphs
     # Optimal # of PCs
     # Optimal # of neighbors (global)
     # Optimal # of neighbors (local)
     optimals = (
@@ -212,11 +228,11 @@
         ],
         npcs[op_pc],
         neighbors[op_k] if op_k is not None else None,
         local_k
     )
 
     if return_errors:
-        return optimals, mses
+        return optimals, (mses, local_error)
 
     else:
         return optimals
```

### Comparing `scself-0.3.0/scself/_noise2self/n2s.py` & `scself-0.4.0/scself/_noise2self/n2s.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     loss='mse',
     loss_kwargs={},
     return_errors=False,
     connectivity=False,
     standardization_method='log',
     pc_data=None,
     chunk_size=10000,
+    random_state=None,
     verbose=None
 ):
     """
     Select an optimal set of graph parameters based on noise2self
 
     :param count_data: Count data
     :type count_data: np.ndarray, sp.spmatrix
@@ -73,21 +74,25 @@
 
     neighbors, npcs = _check_args(
         neighbors,
         npcs,
         count_data,
         pc_data
     )
+    _max_neighbors = np.max(neighbors)
 
     data_obj, expr_data = _standardize(
         count_data,
         standardization_method
     )
 
-    log(f"Searching {len(npcs)} PC x {len(neighbors)} Neighbors space")
+    log(
+        f"Searching {len(npcs)} PCs [{np.min(npcs)}-{np.max(npcs)}] by "
+        f"{len(neighbors)} Neighbors [{np.min(neighbors)}-{_max_neighbors}]"
+    )
 
     if pc_data is not None:
         log(f"Using existing PCs {pc_data.shape}")
         data_obj.obsm['X_pca'] = pc_data
 
     else:
         data_obj.obsm['X_pca'] = pca(expr_data, np.max(npcs))
@@ -95,24 +100,27 @@
     mses = np.zeros((len(npcs), len(neighbors)))
 
     if len(npcs) > 1:
 
         # Search for the smallest MSE for each n_pcs / k combination
         # Outer loop does PCs, because the distance graph has to be
         # recalculated when PCs changes
-        for i, pc in tqdm.tqdm(enumerate(npcs), total=len(npcs)):
+        for i, pc in (pbar := tqdm.tqdm(enumerate(npcs), total=len(npcs))):
+
+            pbar.set_description(f"{pc} PCs")
 
             # Calculate neighbor graph with the max number of neighbors
             # Faster to select only a subset of edges than to recalculate
             # (obviously)
             neighbor_graph(
                 data_obj,
                 pc,
-                np.max(neighbors),
-                metric=metric
+                _max_neighbors,
+                metric=metric,
+                random_state=random_state
             )
 
             # Search through the neighbors space
             mses[i, :] = _search_k(
                 expr_data,
                 (data_obj.obsp['distances'], ),
                 neighbors,
@@ -139,39 +147,47 @@
         op_pc = 0
         op_k = None
 
     # Recalculate a k-NN graph from the optimal # of PCs
     neighbor_graph(
         data_obj,
         npcs[op_pc],
-        np.max(neighbors),
-        metric=metric
+        _max_neighbors,
+        metric=metric,
+        random_state=random_state
     )
 
     # Search space for k-neighbors
     local_neighbors = np.arange(
         np.min(neighbors) if len(neighbors) > 1 else 1,
-        np.max(neighbors)
+        _max_neighbors + 1
     )
 
+    log(f"Searching local k ({local_neighbors[0]}-{local_neighbors[-1]})")
+
     # Search for the optimal number of k for each obs
     # For the global optimal n_pc
-    local_k = local_neighbors[np.argmin(
-        _search_k(
-            expr_data,
-            (data_obj.obsp['distances'], ),
-            local_neighbors,
-            by_row=True,
-            connectivity=connectivity,
-            loss=loss,
-            loss_kwargs=loss_kwargs,
-            chunk_size=chunk_size
-        ),
-        axis=0
-    )]
+    local_error = _search_k(
+        expr_data,
+        (data_obj.obsp['distances'], ),
+        local_neighbors,
+        by_row=True,
+        connectivity=connectivity,
+        loss=loss,
+        loss_kwargs=loss_kwargs,
+        chunk_size=chunk_size,
+        pbar=True
+    )
+
+    local_k = local_neighbors[np.argmin(local_error, axis=0)]
+
+    log(
+        f"Optimal local k complete ({local_k.min()}-{local_k.max()}, "
+        f"mean={local_k.mean():.2f})"
+    )
 
     # Pack return object:
     # Optimal (variable-k) graph
     # Optimal # of PCs
     # Optimal # of neighbors (global)
     # Optimal # of neighbors (local)
     optimals = (
@@ -181,11 +197,11 @@
         ),
         npcs[op_pc],
         neighbors[op_k] if op_k is not None else None,
         local_k
     )
 
     if return_errors:
-        return optimals, mses
+        return optimals, (mses, local_error)
 
     else:
         return optimals
```

### Comparing `scself-0.3.0/scself/scaling/truncscaler.py` & `scself-0.4.0/scself/scaling/truncscaler.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/sparse/graph.py` & `scself-0.4.0/scself/sparse/graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -48,44 +48,53 @@
 
             if smallest:
                 _data[np.argsort(_data)[k - _n:]] = 0
             else:
                 _data[np.argsort(_data)[:_n - k]] = 0
 
 
-def _chunk_graph_mse(
+def chunk_graph_mse(
     X,
     k_graph,
-    row_start=0,
-    row_end=None
+    start=None,
+    end=None
 ):
-    if row_end is None:
-        row_end = k_graph.shape[0]
+
+    if start is not None:
+        if end is None:
+            end = X.shape[0]
+
+        if end <= start:
+            return
+
+        indptr = X.indptr[start:end + 1]
+        k_graph = k_graph[start:end, :]
     else:
-        row_end = min(k_graph.shape[0], row_end)
+        indptr = X.indptr
 
     return _mse_rowwise(
         X.data,
         X.indices,
-        X.indptr,
+        indptr,
         dot(
-            k_graph[row_start:row_end, :],
+            k_graph,
             X,
             dense=True
         )
     )
 
 
 @numba.njit(parallel=True)
 def _mse_rowwise(
     a_data,
     a_indices,
     a_indptr,
     b
 ):
+    # B WILL BE OVERWRITTEN #
 
     n_row = b.shape[0]
     output = np.zeros(n_row, dtype=float)
 
     for i in numba.prange(n_row):
 
         _idx_a = a_indices[a_indptr[i]:a_indptr[i + 1]]
@@ -93,13 +102,13 @@
 
         row = b[i, :]
 
         if _nnz_a == 0:
             pass
 
         else:
-            row = row.copy()
             row[_idx_a] -= a_data[a_indptr[i]:a_indptr[i + 1]]
+            row **= 2
 
-        output[i] = np.mean(row ** 2)
+        output[i] = np.mean(row)
 
     return output
```

### Comparing `scself-0.3.0/scself/sparse/math.py` & `scself-0.4.0/scself/sparse/math.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/sparse/truncated_svd.py` & `scself-0.4.0/scself/sparse/truncated_svd.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/tests/_stubs.py` & `scself-0.4.0/scself/tests/_stubs.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/tests/test_math.py` & `scself-0.4.0/scself/tests/test_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         cls.Z = np.mean((cls.X - cls.Y) ** 2)
         cls.MAE = np.mean(np.abs(cls.X - cls.Y))
         cls.Z_row = np.mean((cls.X - cls.Y) ** 2, axis=1)
         cls.MAE_row = np.mean(np.abs(cls.X - cls.Y), axis=1)
         cls.Z_noY = np.mean(cls.X ** 2)
         cls.Z_noY_row = np.mean(cls.X ** 2, axis=1)
 
-    def test_mse_rowwise(self):
+    def test_mcv_error(self):
 
         npt.assert_array_almost_equal(
             mcv_mean_error(
                 self.X,
                 self.PC,
                 self.ROTATION,
                 axis=None,
```

### Comparing `scself-0.3.0/scself/tests/test_mcv.py` & `scself-0.4.0/scself/tests/test_mcv.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/tests/test_mkl_hacks.py` & `scself-0.4.0/scself/tests/test_mkl_hacks.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/tests/test_noise2self.py` & `scself-0.4.0/scself/tests/test_noise2self.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 from scself._noise2self.graph import local_optimal_knn
 from scself._noise2self.common import (
     _dist_to_row_stochastic,
     _connect_to_row_stochastic,
     _invert_distance_graph,
     _search_k,
-    standardize_data
+    _noise_to_self_error,
+    standardize_data,
+    row_normalize
 )
 from scself._noise2self import noise2self
 
 M, N = 100, 10
 
 RNG = np.random.default_rng(100)
 
@@ -34,25 +36,122 @@
 
 EXPR = BASE + NOISE
 PEAKS = RNG.choice([0, 1], (M, N), p=(0.9, 0.1))
 
 DIST = sklearn.metrics.pairwise_distances(EXPR, metric='cosine')
 PDIST = sklearn.metrics.pairwise_distances(PEAKS, metric='cosine')
 
-ADATA = ad.AnnData(EXPR.astype(int))
-
 
 def _knn(k, dist=sps.csr_matrix(DIST)):
     return local_optimal_knn(
         dist.copy(),
         np.array([k] * 100),
         keep='smallest'
     )
 
 
+class TestKnnSelect(unittest.TestCase):
+
+    def test_nnz(self):
+
+        knn_1 = _knn(1)
+        npt.assert_equal(knn_1.indptr, np.arange(101))
+
+        knn_2 = _knn(2)
+        npt.assert_equal(knn_2.indptr, np.arange(101) * 2)
+
+        for i in range(100):
+            npt.assert_equal(
+                sorted(knn_2[i].indices),
+                sorted(np.argsort(DIST[i, :])[1:3])
+            )
+
+        knn_7 = _knn(7)
+        npt.assert_equal(knn_7.indptr, np.arange(101) * 7)
+
+
+class TestError(unittest.TestCase):
+
+    def test_error_max_dense(self):
+
+        err = _noise_to_self_error(
+            EXPR.astype(np.float64),
+            np.zeros_like(DIST),
+            by_row=True
+        )
+
+        expect = np.mean(EXPR ** 2, axis=1)
+
+        npt.assert_almost_equal(err, expect)
+
+    def test_error_max_sparse(self):
+
+        err = _noise_to_self_error(
+            sps.csr_array(EXPR.astype(np.float64)),
+            sps.csr_array(np.zeros_like(DIST)),
+            chunk_size=5,
+            by_row=True
+        )
+
+        expect = np.mean(EXPR ** 2, axis=1)
+
+        npt.assert_almost_equal(err, expect)
+
+    def test_error_max_sparse_nochunk(self):
+
+        err = _noise_to_self_error(
+            sps.csr_array(EXPR.astype(np.float64)),
+            sps.csr_array(np.zeros_like(DIST)),
+            chunk_size=None,
+            by_row=True
+        )
+
+        expect = np.mean(EXPR ** 2, axis=1)
+
+        npt.assert_almost_equal(err, expect)
+
+    def test_error_min_dense(self):
+
+        err = _noise_to_self_error(
+            EXPR.astype(np.float64),
+            np.eye(DIST.shape[0]),
+            by_row=True
+        )
+
+        expect = np.zeros_like(err)
+
+        npt.assert_almost_equal(err, expect)
+
+    def test_error_min_sparse(self):
+
+        err = _noise_to_self_error(
+            sps.csr_array(EXPR.astype(np.float64)),
+            sps.csr_array(np.eye(DIST.shape[0])),
+            chunk_size=5,
+            by_row=True
+        )
+
+        expect = np.zeros_like(err)
+
+        npt.assert_almost_equal(err, expect)
+
+    def test_error_min_sparse_nochunk(self):
+
+        err = _noise_to_self_error(
+            sps.csr_array(EXPR.astype(np.float64)),
+            sps.csr_array(np.eye(DIST.shape[0])),
+            chunk_size=None,
+            by_row=True
+        )
+
+        expect = np.zeros_like(err)
+
+        npt.assert_almost_equal(err, expect)
+
+
 class TestDistInvert(unittest.TestCase):
 
     def test_invert_sparse(self):
         graph = sps.csr_matrix(DIST)
         graph = _invert_distance_graph(graph).A
 
         invert_order = np.zeros_like(DIST)
@@ -72,14 +171,45 @@
 
         for i in range(graph.shape[0]):
             npt.assert_equal(
                 np.argsort(invert_order[i]),
                 np.argsort(graph[i])
             )
 
+    def test_row_normalize(self):
+        graph = sps.csr_matrix(DIST)
+        graph = row_normalize(graph).A
+
+        invert_order = np.zeros_like(DIST)
+        np.divide(1, DIST, out=invert_order, where=DIST != 0)
+
+        for i in range(graph.shape[0]):
+            npt.assert_equal(
+                np.argsort(invert_order[i]),
+                np.argsort(graph[i])
+            )
+
+        _rowsum = graph.sum(axis=1)
+        npt.assert_almost_equal(_rowsum, np.ones_like(_rowsum))
+
+    def test_row_normalize_dense(self):
+        graph = row_normalize(DIST.copy())
+
+        invert_order = np.zeros_like(DIST)
+        np.divide(1, DIST, out=invert_order, where=DIST != 0)
+
+        for i in range(graph.shape[0]):
+            npt.assert_equal(
+                np.argsort(invert_order[i]),
+                np.argsort(graph[i])
+            )
+
+        _rowsum = graph.sum(axis=1)
+        npt.assert_almost_equal(_rowsum, np.ones_like(_rowsum))
+
 
 class TestRowStochastic(unittest.TestCase):
 
     loss = 'mse'
 
     def test_full_k(self):
         graph = sps.csr_matrix(DIST)
@@ -158,21 +288,21 @@
 
     data = EXPR.astype(float)
     dist = (DIST.copy(), )
     normalize = 'log'
     loss = 'mse'
     correct_loss = np.array([
         234.314,
-        223.1832274,
-        212.9209424,
-        203.5771366,
-        194.4068273,
-        185.2830849
+        160.764803,
+        142.8430503,
+        135.422603,
+        130.4516997,
+        130.762186
     ])
-    correct_mse_argmin = 5
+    correct_mse_argmin = 4
     correct_opt_pc = 7
     correct_opt_k = 4
 
 
 class TestKNNSearch(_N2SSetup, unittest.TestCase):
 
     def test_ksearch_regression(self):
@@ -208,43 +338,45 @@
         )
 
 
 class TestNoise2Self(_N2SSetup, unittest.TestCase):
 
     def test_knn_select_stack_regression(self):
 
-        _, opt_pc, opt_k, local_ks = noise2self(
+        (_, opt_pc, opt_k, local_ks), errs = noise2self(
             self.data,
-            np.arange(1, 11),
+            np.arange(4, 11),
             np.array([3, 5, 7]),
             loss=self.loss,
-            standardization_method=self.normalize
+            standardization_method=self.normalize,
+            return_errors=True,
+            random_state=50
         )
 
         self.assertEqual(opt_pc, self.correct_opt_pc)
         self.assertEqual(opt_k, self.correct_opt_k)
 
     def test_knn_select_stack_regression_sparse(self):
 
         obsp, opt_pc, opt_k, local_ks = noise2self(
             sps.csr_matrix(self.data),
-            np.arange(1, 11),
+            np.arange(4, 11),
             np.array([3, 5, 7]),
             loss=self.loss,
             standardization_method=self.normalize
         )
 
         self.assertEqual(opt_pc, self.correct_opt_pc)
         self.assertEqual(opt_k, self.correct_opt_k)
 
     def test_knn_select_stack_regression_nopcsearch(self):
 
         _, opt_pc, opt_k, local_ks = noise2self(
             self.data,
-            np.arange(1, 11),
+            np.arange(4, 11),
             5,
             loss=self.loss,
             standardization_method=self.normalize
         )
 
         self.assertEqual(opt_pc, 5)
         self.assertIsNone(opt_k)
@@ -262,22 +394,23 @@
 
     normalize = None
     data = PEAKS.astype(float)
     dist = (PDIST.copy(), )
     loss = 'log_loss'
     correct_loss = np.array([
         0.999322,
-        0.5909092,
-        0.3082457,
-        0.2716103,
-        0.2355531,
-        0.1897085
+        0.4702795,
+        0.2203677,
+        0.1766228,
+        0.1764214,
+        0.1564008
     ])
     correct_opt_pc = 7
     correct_opt_k = 8
+    correct_mse_argmin = 5
 
 
 class TestKNNSearchMultimodal(TestKNNSearch):
 
     dist = (DIST.copy(), DIST.copy())
```

### Comparing `scself-0.3.0/scself/utils/_pca.py` & `scself-0.4.0/scself/utils/_pca.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/utils/dot_product.py` & `scself-0.4.0/scself/utils/dot_product.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/utils/logging.py` & `scself-0.4.0/scself/utils/logging.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/utils/pairwise_loss.py` & `scself-0.4.0/scself/utils/pairwise_loss.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/utils/standardization.py` & `scself-0.4.0/scself/utils/standardization.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself/utils/sum.py` & `scself-0.4.0/scself/utils/sum.py`

 * *Files identical despite different names*

### Comparing `scself-0.3.0/scself.egg-info/PKG-INFO` & `scself-0.4.0/scself.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scself
-Version: 0.3.0
+Version: 0.4.0
 Summary: Self Supervised Tools for Single Cell Data
 Home-page: https://github.com/GreshamLab/sc_self_supervised
 Author: Chris Jackson
 Author-email: cj59@nyu.edu
 Maintainer: Chris Jackson
 Maintainer-email: cj59@nyu.edu
 Description-Content-Type: text/markdown
```

### Comparing `scself-0.3.0/scself.egg-info/SOURCES.txt` & `scself-0.4.0/scself.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 scself/__init__.py
 scself.egg-info/PKG-INFO
 scself.egg-info/SOURCES.txt
 scself.egg-info/dependency_links.txt
 scself.egg-info/not-zip-safe
 scself.egg-info/requires.txt
 scself.egg-info/top_level.txt
+scself/_denoise/__init__.py
+scself/_denoise/n2s_denoise.py
 scself/_mcv/__init__.py
 scself/_mcv/common.py
 scself/_mcv/mcv_per_cell.py
 scself/_mcv/molecular_crossvalidation.py
 scself/_noise2self/__init__.py
 scself/_noise2self/common.py
 scself/_noise2self/graph.py
@@ -21,14 +23,15 @@
 scself/scaling/truncscaler.py
 scself/sparse/__init__.py
 scself/sparse/graph.py
 scself/sparse/math.py
 scself/sparse/truncated_svd.py
 scself/tests/__init__.py
 scself/tests/_stubs.py
+scself/tests/test_denoise.py
 scself/tests/test_math.py
 scself/tests/test_mcv.py
 scself/tests/test_mkl_hacks.py
 scself/tests/test_noise2self.py
 scself/utils/__init__.py
 scself/utils/_pca.py
 scself/utils/dot_product.py
```

### Comparing `scself-0.3.0/setup.py` & `scself-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 
 tests_require = [
     "coverage",
     "pytest"
 ]
 
-version = "0.3.0"
+version = "0.4.0"
 
 # Description from README.md
 long_description = "\n\n".join(
     [open(
         os.path.join(
             os.path.dirname(os.path.abspath(__file__)),
             "README.md"
```


# Comparing `tmp/torchseal-0.1.2.tar.gz` & `tmp/torchseal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchseal-0.1.2.tar", last modified: Fri Apr  5 06:53:58 2024, max compression
+gzip compressed data, was "torchseal-0.2.0.tar", last modified: Mon May 20 16:02:04 2024, max compression
```

## Comparing `torchseal-0.1.2.tar` & `torchseal-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,57 @@
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.362795 torchseal-0.1.2/
--rw-r--r--   0 rayhankinan   (501) staff       (20)     1112 2024-02-27 12:01:08.000000 torchseal-0.1.2/LICENSE
--rw-r--r--   0 rayhankinan   (501) staff       (20)      758 2024-04-05 06:53:58.362575 torchseal-0.1.2/PKG-INFO
--rw-r--r--   0 rayhankinan   (501) staff       (20)      100 2024-02-27 12:01:08.000000 torchseal-0.1.2/README.md
--rw-r--r--   0 rayhankinan   (501) staff       (20)      717 2024-04-05 06:53:54.000000 torchseal-0.1.2/pyproject.toml
--rw-r--r--   0 rayhankinan   (501) staff       (20)       38 2024-04-05 06:53:58.362845 torchseal-0.1.2/setup.cfg
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.356893 torchseal-0.1.2/src/
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.358044 torchseal-0.1.2/src/torchseal/
--rw-r--r--   0 rayhankinan   (501) staff       (20)       86 2024-03-04 07:35:25.000000 torchseal-0.1.2/src/torchseal/__init__.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.360126 torchseal-0.1.2/src/torchseal/function/
--rw-r--r--   0 rayhankinan   (501) staff       (20)      183 2024-04-04 20:12:15.000000 torchseal-0.1.2/src/torchseal/function/__init__.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     2579 2024-04-04 19:13:37.000000 torchseal-0.1.2/src/torchseal/function/average2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     3272 2024-04-04 19:13:40.000000 torchseal-0.1.2/src/torchseal/function/conv2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     1767 2024-04-04 16:28:22.000000 torchseal-0.1.2/src/torchseal/function/linear.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-04-04 16:47:44.000000 torchseal-0.1.2/src/torchseal/function/max2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-25 17:29:39.000000 torchseal-0.1.2/src/torchseal/function/relu.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      851 2024-04-04 16:28:35.000000 torchseal-0.1.2/src/torchseal/function/sigmoid.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      843 2024-04-04 16:28:47.000000 torchseal-0.1.2/src/torchseal/function/square.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-25 18:45:58.000000 torchseal-0.1.2/src/torchseal/function/tanh.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.361499 torchseal-0.1.2/src/torchseal/nn/
--rw-r--r--   0 rayhankinan   (501) staff       (20)      143 2024-04-04 16:52:01.000000 torchseal-0.1.2/src/torchseal/nn/__init__.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     1293 2024-04-04 20:12:26.000000 torchseal-0.1.2/src/torchseal/nn/average2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     1247 2024-04-04 20:12:29.000000 torchseal-0.1.2/src/torchseal/nn/conv2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      790 2024-04-04 20:12:33.000000 torchseal-0.1.2/src/torchseal/nn/linear.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-04-04 16:47:50.000000 torchseal-0.1.2/src/torchseal/nn/max2d.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-25 17:29:34.000000 torchseal-0.1.2/src/torchseal/nn/relu.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      391 2024-04-04 16:12:14.000000 torchseal-0.1.2/src/torchseal/nn/sigmoid.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-26 15:51:49.000000 torchseal-0.1.2/src/torchseal/nn/softmax.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      387 2024-04-04 16:12:37.000000 torchseal-0.1.2/src/torchseal/nn/square.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-25 18:46:04.000000 torchseal-0.1.2/src/torchseal/nn/tanh.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.361751 torchseal-0.1.2/src/torchseal/utils/
--rw-r--r--   0 rayhankinan   (501) staff       (20)       49 2024-04-04 05:05:15.000000 torchseal-0.1.2/src/torchseal/utils/__init__.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     4028 2024-04-04 18:46:35.000000 torchseal-0.1.2/src/torchseal/utils/toeplitz.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.362155 torchseal-0.1.2/src/torchseal/wrapper/
--rw-r--r--   0 rayhankinan   (501) staff       (20)        0 2024-03-04 07:34:56.000000 torchseal-0.1.2/src/torchseal/wrapper/__init__.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)     5015 2024-04-04 18:32:05.000000 torchseal-0.1.2/src/torchseal/wrapper/ckks.py
--rw-r--r--   0 rayhankinan   (501) staff       (20)      319 2024-04-04 12:28:23.000000 torchseal-0.1.2/src/torchseal/wrapper/function.py
-drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-04-05 06:53:58.362341 torchseal-0.1.2/src/torchseal.egg-info/
--rw-r--r--   0 rayhankinan   (501) staff       (20)      758 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/PKG-INFO
--rw-r--r--   0 rayhankinan   (501) staff       (20)      974 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/SOURCES.txt
--rw-r--r--   0 rayhankinan   (501) staff       (20)        1 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/dependency_links.txt
--rw-r--r--   0 rayhankinan   (501) staff       (20)       20 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/requires.txt
--rw-r--r--   0 rayhankinan   (501) staff       (20)       10 2024-04-05 06:53:58.000000 torchseal-0.1.2/src/torchseal.egg-info/top_level.txt
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.093249 torchseal-0.2.0/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1112 2024-02-27 12:01:08.000000 torchseal-0.2.0/LICENSE
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      758 2024-05-20 16:02:04.092966 torchseal-0.2.0/PKG-INFO
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      100 2024-02-27 12:01:08.000000 torchseal-0.2.0/README.md
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      717 2024-05-20 16:01:43.000000 torchseal-0.2.0/pyproject.toml
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       38 2024-05-20 16:02:04.093301 torchseal-0.2.0/setup.cfg
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.078364 torchseal-0.2.0/src/
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.079727 torchseal-0.2.0/src/torchseal/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1330 2024-05-14 12:45:12.000000 torchseal-0.2.0/src/torchseal/__init__.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.084225 torchseal-0.2.0/src/torchseal/function/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      330 2024-05-20 12:54:28.000000 torchseal-0.2.0/src/torchseal/function/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     2144 2024-05-14 11:46:25.000000 torchseal-0.2.0/src/torchseal/function/average2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     5223 2024-05-14 09:07:34.000000 torchseal-0.2.0/src/torchseal/function/conv2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     2172 2024-05-20 13:28:14.000000 torchseal-0.2.0/src/torchseal/function/cross_entropy.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     2143 2024-05-14 06:47:05.000000 torchseal-0.2.0/src/torchseal/function/linear.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     2207 2024-05-20 13:23:25.000000 torchseal-0.2.0/src/torchseal/function/mse.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1477 2024-05-14 20:53:57.000000 torchseal-0.2.0/src/torchseal/function/relu.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1439 2024-05-14 20:39:15.000000 torchseal-0.2.0/src/torchseal/function/sigmoid.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1205 2024-05-14 04:41:56.000000 torchseal-0.2.0/src/torchseal/function/square.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1390 2024-05-14 12:59:33.000000 torchseal-0.2.0/src/torchseal/function/tanh.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.087118 torchseal-0.2.0/src/torchseal/nn/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      258 2024-05-20 12:56:59.000000 torchseal-0.2.0/src/torchseal/nn/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1882 2024-05-14 20:37:31.000000 torchseal-0.2.0/src/torchseal/nn/average2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     4205 2024-05-14 20:36:56.000000 torchseal-0.2.0/src/torchseal/nn/conv2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     3267 2024-05-20 12:55:46.000000 torchseal-0.2.0/src/torchseal/nn/cross_entropy.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1710 2024-05-14 20:38:38.000000 torchseal-0.2.0/src/torchseal/nn/linear.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      445 2024-05-20 12:56:02.000000 torchseal-0.2.0/src/torchseal/nn/mse.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     2005 2024-05-14 22:28:46.000000 torchseal-0.2.0/src/torchseal/nn/relu.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1112 2024-05-14 21:59:14.000000 torchseal-0.2.0/src/torchseal/nn/sigmoid.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      445 2024-05-14 22:45:48.000000 torchseal-0.2.0/src/torchseal/nn/square.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1089 2024-05-14 21:59:30.000000 torchseal-0.2.0/src/torchseal/nn/tanh.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.087645 torchseal-0.2.0/src/torchseal/optim/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       21 2024-05-12 06:35:27.000000 torchseal-0.2.0/src/torchseal/optim/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1344 2024-05-14 10:43:19.000000 torchseal-0.2.0/src/torchseal/optim/sgd.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.088219 torchseal-0.2.0/src/torchseal/state/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       31 2024-05-13 16:18:39.000000 torchseal-0.2.0/src/torchseal/state/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1808 2024-05-20 15:41:22.000000 torchseal-0.2.0/src/torchseal/state/context.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.091230 torchseal-0.2.0/src/torchseal/utils/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      509 2024-05-20 13:19:32.000000 torchseal-0.2.0/src/torchseal/utils/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      554 2024-05-11 16:24:03.000000 torchseal-0.2.0/src/torchseal/utils/average2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      657 2024-05-14 06:12:00.000000 torchseal-0.2.0/src/torchseal/utils/block.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1897 2024-05-14 09:21:29.000000 torchseal-0.2.0/src/torchseal/utils/conv2d.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      281 2024-05-20 15:37:15.000000 torchseal-0.2.0/src/torchseal/utils/handle_batch_size.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      410 2024-05-06 03:43:10.000000 torchseal-0.2.0/src/torchseal/utils/near_zeros.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     2741 2024-05-14 11:38:19.000000 torchseal-0.2.0/src/torchseal/utils/padding.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      354 2024-05-11 16:35:05.000000 torchseal-0.2.0/src/torchseal/utils/sparse.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     8455 2024-05-06 05:28:01.000000 torchseal-0.2.0/src/torchseal/utils/toeplitz.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.092283 torchseal-0.2.0/src/torchseal/wrapper/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      237 2024-05-20 12:32:55.000000 torchseal-0.2.0/src/torchseal/wrapper/__init__.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)    19355 2024-05-20 15:36:38.000000 torchseal-0.2.0/src/torchseal/wrapper/ckks.py
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     3402 2024-05-20 12:32:38.000000 torchseal-0.2.0/src/torchseal/wrapper/function.py
+drwxr-xr-x   0 rayhankinan   (501) staff       (20)        0 2024-05-20 16:02:04.092663 torchseal-0.2.0/src/torchseal.egg-info/
+-rw-r--r--   0 rayhankinan   (501) staff       (20)      758 2024-05-20 16:02:04.000000 torchseal-0.2.0/src/torchseal.egg-info/PKG-INFO
+-rw-r--r--   0 rayhankinan   (501) staff       (20)     1366 2024-05-20 16:02:04.000000 torchseal-0.2.0/src/torchseal.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhankinan   (501) staff       (20)        1 2024-05-20 16:02:04.000000 torchseal-0.2.0/src/torchseal.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       20 2024-05-20 16:02:04.000000 torchseal-0.2.0/src/torchseal.egg-info/requires.txt
+-rw-r--r--   0 rayhankinan   (501) staff       (20)       10 2024-05-20 16:02:04.000000 torchseal-0.2.0/src/torchseal.egg-info/top_level.txt
```

### Comparing `torchseal-0.1.2/LICENSE` & `torchseal-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchseal-0.1.2/PKG-INFO` & `torchseal-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchseal
-Version: 0.1.2
+Version: 0.2.0
 Summary: PyTorch extension to enable training and testing using homomorphic encryption
 Author-email: Rayhan Kinan Muhannad <rayhankinan@gmail.com>
 Project-URL: Homepage, https://github.com/cnn-for-ckks/pytorch-for-tenseal
 Project-URL: Issues, https://github.com/cnn-for-ckks/pytorch-for-tenseal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `torchseal-0.1.2/pyproject.toml` & `torchseal-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torchseal"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Rayhan Kinan Muhannad", email="rayhankinan@gmail.com" },
 ]
 description = "PyTorch extension to enable training and testing using homomorphic encryption"
 readme = "README.md"
 requires-python = ">=3.6, <3.10"
 dependencies = [
```

### Comparing `torchseal-0.1.2/src/torchseal/function/linear.py` & `torchseal-0.2.0/src/torchseal/function/average2d.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,55 @@
-from typing import Optional, Tuple
-from torchseal.wrapper.ckks import CKKSWrapper
-from torchseal.wrapper.function import CKKSFunctionWrapper
+from typing import Tuple, Optional
+from torchseal.wrapper import CKKSWrapper, CKKSPoolingFunctionWrapper
 
+import typing
 import torch
 
 
-class LinearFunction(torch.autograd.Function):
+class AvgPool2dFunction(torch.autograd.Function):
     @staticmethod
-    def forward(ctx: CKKSFunctionWrapper, enc_x: CKKSWrapper, weight: torch.Tensor, bias: torch.Tensor) -> CKKSWrapper:
+    def forward(ctx: CKKSPoolingFunctionWrapper, enc_input: CKKSWrapper, weight: torch.Tensor, conv2d_padding_transformation: torch.Tensor, conv2d_inverse_padding_transformation: torch.Tensor) -> CKKSWrapper:
+        # Apply the padding transformation to the encrypted input
+        # NOTE: This is useless if padding is 0 (we can skip this step if that's the case)
+        enc_padding_input = enc_input.ckks_matrix_multiplication(
+            conv2d_padding_transformation
+        )
+
         # Save the ctx for the backward method
-        ctx.save_for_backward(weight)
-        ctx.enc_x = enc_x.clone()
+        ctx.save_for_backward(weight, conv2d_inverse_padding_transformation)
 
-        # Apply the linear transformation to the encrypted input
-        out_x = enc_x.do_linear(weight, bias)
+        # Apply the convolution to the encrypted input
+        enc_output = enc_padding_input.ckks_matrix_multiplication(weight.t())
 
-        return out_x
+        return enc_output
 
     @staticmethod
-    def backward(ctx: CKKSFunctionWrapper, grad_output: torch.Tensor) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]:
+    def backward(ctx: CKKSPoolingFunctionWrapper, enc_grad_output: CKKSWrapper) -> Tuple[Optional[CKKSWrapper], None, None, None]:
         # Get the saved tensors
-        saved_tensors: Tuple[torch.Tensor] = ctx.saved_tensors  # type: ignore
-        x = ctx.enc_x.do_decryption()
-
-        # Unpack the saved tensors
-        weight, = saved_tensors
+        weight, conv2d_inverse_padding_transformation = typing.cast(
+            Tuple[torch.Tensor, torch.Tensor],
+            ctx.saved_tensors
+        )
 
         # Get the needs_input_grad
-        result: Tuple[bool, bool, bool] = ctx.needs_input_grad  # type: ignore
+        result = typing.cast(
+            Tuple[bool, bool, bool, bool],
+            ctx.needs_input_grad
+        )
 
         # Initialize the gradients
-        grad_input = grad_weight = grad_bias = None
+        enc_grad_input = None
 
-        # Compute the gradients
+        # Calculate the gradient for the input
         if result[0]:
-            grad_input = grad_output.matmul(weight)
-        if result[1]:
-            grad_weight = grad_output.unsqueeze(0).t().matmul(x.unsqueeze(0))
-        if result[2]:
-            grad_bias = grad_output
-
-        return grad_input, grad_weight, grad_bias
-
-    @staticmethod
-    def apply(enc_x: CKKSWrapper, weight: torch.Tensor, bias: torch.Tensor) -> CKKSWrapper:
-        out_x: CKKSWrapper = super(LinearFunction, LinearFunction).apply(
-            enc_x, weight, bias
-        )  # type: ignore
+            # Calculate the gradients for the input tensor
+            enc_padded_grad_input = enc_grad_output.ckks_matrix_multiplication(
+                weight
+            )
+
+            # Apply the inverse padding transformation to the gradient input
+            # NOTE: This is useless if padding is 0 (we can skip this step if that's the case)
+            enc_grad_input = enc_padded_grad_input.ckks_matrix_multiplication(
+                conv2d_inverse_padding_transformation
+            )
 
-        return out_x
+        return enc_grad_input, None, None, None
```

### Comparing `torchseal-0.1.2/src/torchseal/nn/conv2d.py` & `torchseal-0.2.0/src/torchseal/nn/linear.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,60 @@
-from typing import Tuple, Optional
-from torchseal.wrapper.ckks import CKKSWrapper
-from torchseal.function import Conv2dFunction
+from typing import Optional
+from torchseal.wrapper import CKKSWrapper
+from torchseal.function import LinearFunction
 
+import typing
 import torch
+import torchseal
 
 
-class Conv2d(torch.nn.Module):
-    def __init__(self, in_channel: int, out_channel: int, kernel_size: Tuple[int, int], output_size: torch.Size, stride: int = 1, padding: int = 0, weight: Optional[torch.Tensor] = None, bias: Optional[torch.Tensor] = None) -> None:
-        super(Conv2d, self).__init__()
-
-        # Save the parameters
-        self.output_size = output_size
-        self.stride = stride
-        self.padding = padding
-
-        # Unpack the kernel size
-        kernel_n_rows, kernel_n_cols = kernel_size
-
-        # Create the weight and bias
-        self.weight = torch.nn.Parameter(
-            torch.rand(
-                out_channel, in_channel, kernel_n_rows, kernel_n_cols
-            ) if weight is None else weight
+class Linear(torch.nn.Module):
+    weight: CKKSWrapper
+    bias: CKKSWrapper
+
+    def __init__(self, in_features: int, out_features: int, weight: Optional[CKKSWrapper] = None, bias: Optional[CKKSWrapper] = None):
+        super(Linear, self).__init__()
+
+        self.weight = typing.cast(
+            CKKSWrapper,
+            torch.nn.Parameter(
+                torchseal.ckks_wrapper(
+                    torch.rand(out_features, in_features),
+                    do_encryption=True
+                ) if weight is None else weight
+            )
         )
-        self.bias = torch.nn.Parameter(
-            torch.rand(out_channel) if bias is None else bias
+
+        self.bias = typing.cast(
+            CKKSWrapper,
+            torch.nn.Parameter(
+                torchseal.ckks_wrapper(
+                    torch.rand(out_features),
+                    do_encryption=True
+                ) if bias is None else bias
+            )
         )
 
     def forward(self, enc_x: CKKSWrapper) -> CKKSWrapper:
-        out_x: CKKSWrapper = Conv2dFunction.apply(
-            enc_x, self.weight, self.bias, self.output_size, self.stride, self.padding
-        )  # type: ignore
+        enc_output = typing.cast(
+            CKKSWrapper,
+            LinearFunction.apply(
+                enc_x, self.weight, self.bias, self.training
+            )
+        )
+
+        return enc_output
+
+    def train(self, mode=True) -> "Linear":
+        if mode:
+            # Inplace encrypt the parameters
+            self.weight.inplace_encrypt()
+            self.bias.inplace_encrypt()
+        else:
+            # Inplace decrypt the parameters
+            self.weight.inplace_decrypt()
+            self.bias.inplace_decrypt()
+
+        return super(Linear, self).train(mode)
 
-        return out_x
+    def eval(self) -> "Linear":
+        return self.train(False)
```

### Comparing `torchseal-0.1.2/src/torchseal/utils/toeplitz.py` & `torchseal-0.2.0/src/torchseal/nn/conv2d.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,113 @@
+from typing import Tuple, Optional
+
+from torchseal.wrapper import CKKSWrapper
+from torchseal.function import Conv2dFunction
+from torchseal.utils import approximate_toeplitz_multiple_channels, create_conv2d_weight_mask, create_conv2d_bias_transformation, create_padding_transformation_matrix, create_inverse_padding_transformation_matrix
+
+import typing
 import torch
+import torchseal
+
 
+class Conv2d(torch.nn.Module):
+    weight: CKKSWrapper
+    bias: CKKSWrapper
+    conv2d_padding_transformation: torch.Tensor
+    conv2d_inverse_padding_transformation: torch.Tensor
+    conv2d_weight_mask: torch.Tensor
+    conv2d_bias_transformation: torch.Tensor
+
+    def __init__(self, in_channels: int, out_channels: int, kernel_size: Tuple[int, int], input_size: Tuple[int, int], stride: int = 1, padding: int = 0, weight: Optional[CKKSWrapper] = None, bias: Optional[CKKSWrapper] = None) -> None:
+        super(Conv2d, self).__init__()
+
+        # Unpack the kernel size
+        kernel_height, kernel_width = kernel_size
+
+        # Unpack the input size
+        input_height, input_width = input_size
+
+        # Adjust for padding
+        padded_input_height = input_height + 2 * padding
+        padded_input_width = input_width + 2 * padding
+
+        # Count the output dimensions
+        output_height = (padded_input_height - kernel_height) // stride + 1
+        output_width = (padded_input_width - kernel_width) // stride + 1
+
+        # Create the weight and bias
+        self.weight = typing.cast(
+            CKKSWrapper,
+            torch.nn.Parameter(
+                torchseal.ckks_wrapper(
+                    approximate_toeplitz_multiple_channels(
+                        torch.randn(
+                            out_channels, in_channels, kernel_height, kernel_width
+                        ),
+                        (in_channels, input_height, input_width),
+                        stride=stride,
+                        padding=padding
+                    ),
+                    do_encryption=True
+                ) if weight is None else weight
+            )
+        )
 
-# Source: https://stackoverflow.com/questions/68896578/pytorchs-torch-as-strided-with-negative-strides-for-making-a-toeplitz-matrix/68899386#68899386
-def toeplitz(c: torch.Tensor, r: torch.Tensor) -> torch.Tensor:
-    vals = torch.cat((r, c[1:].flip(0)))
-    shape = len(c), len(r)
-    i, j = torch.ones(*shape).nonzero().T
-
-    return vals[j - i].view(*shape)
-
-
-# Source: https://stackoverflow.com/questions/56702873/is-there-an-function-in-pytorch-for-converting-convolutions-to-fully-connected-n
-def toeplitz_one_channel(kernel: torch.Tensor, input_size: torch.Size, stride: int = 1, padding: int = 0) -> torch.Tensor:
-    kernel_height, kernel_width = kernel.shape
-    input_height, input_width = input_size
-
-    # Adjust the input dimensions based on padding
-    padded_input_height = input_height + 2 * padding
-    padded_input_width = input_width + 2 * padding
-
-    # Calculate the output dimensions considering stride and padding
-    output_height = ((padded_input_height - kernel_height) // stride) + 1
-
-    # Stack and reshape the matrices to form the final weight matrix
-    toeplitz_matrices = torch.stack([
-        # Construct 1D convolution toeplitz matrices for each row of the kernel considering stride
-        toeplitz(
-            torch.cat(
-                [
-                    kernel[r, 0:1],
-                    torch.zeros(
-                        padded_input_height - kernel_height
-                    )
-                ]
-            ),
-            torch.cat(
-                [kernel[r, :], torch.zeros(padded_input_width - kernel_width)]
+        self.bias = typing.cast(
+            CKKSWrapper,
+            torch.nn.Parameter(
+                torchseal.ckks_wrapper(
+                    torch.repeat_interleave(
+                        torch.randn(out_channels),
+                        output_height * output_width
+                    ),
+                    do_encryption=True
+                ) if bias is None else bias
             )
-        )[::stride, :][:output_height]
-        for r in range(kernel_height)
-    ])
-
-    # Calculate the number of blocks and their sizes for constructing the final matrix
-    num_blocks_height = output_height
-    block_height, block_width = toeplitz_matrices[0].shape
-
-    # Initialize the final weight matrix with zeros
-    weight_matrix = torch.zeros(
-        (num_blocks_height * block_height, padded_input_width * padded_input_height)
-    )
-
-    # Fill in the blocks for the final weight matrix
-    for i in range(kernel_height):
-        for j in range(output_height):
-            start_row = j * block_height
-            end_row = start_row + block_height
-            start_col = (i + j * stride) * padded_input_width
-            end_col = start_col + block_width
-            weight_matrix[
-                start_row:end_row, start_col:end_col
-            ] = toeplitz_matrices[i]
-
-    return weight_matrix
-
-
-# Source: https://stackoverflow.com/questions/56702873/is-there-an-function-in-pytorch-for-converting-convolutions-to-fully-connected-n
-def toeplitz_multiple_channels(kernel: torch.Tensor, input_size: torch.Size, stride: int = 1, padding: int = 0) -> torch.Tensor:
-    # Get the shapes
-    kernel_out_channel, _, kernel_height, kernel_width = kernel.shape
-    input_in_channel, input_height, input_width = input_size
-
-    # Adjust for padding
-    padded_input_height = input_height + 2 * padding
-    padded_input_width = input_width + 2 * padding
-
-    # Calculate the output size (with padding and stride)
-    output_height = (padded_input_height - kernel_height) // stride + 1
-    output_width = (padded_input_width - kernel_width) // stride + 1
-
-    # Initialize the output tensor
-    weight_convolutions = torch.zeros(
-        (
-            kernel_out_channel,
-            output_height * output_width,
-            input_in_channel,
-            input_height * input_width
-        )
-    )
-
-    # Fill the output tensor
-    for i, kernel_output in enumerate(kernel):
-        for j, kernel_input in enumerate(kernel_output):
-            weight_convolutions[i, :, j, :] = toeplitz_one_channel(
-                kernel_input, input_size[1:], padding=padding, stride=stride
+        )
+
+        # Create the binary masking for inference
+        self.conv2d_padding_transformation = create_padding_transformation_matrix(
+            in_channels, input_height, input_width, padding
+        )
+
+        self.conv2d_inverse_padding_transformation = create_inverse_padding_transformation_matrix(
+            out_channels, input_height, input_width, padding
+        )
+
+        # Create the binary masking for training
+        self.conv2d_weight_mask = create_conv2d_weight_mask(
+            (in_channels, input_height, input_width),
+            (out_channels, in_channels, kernel_height, kernel_width),
+            stride=stride,
+            padding=padding
+        )
+
+        self.conv2d_bias_transformation = create_conv2d_bias_transformation(
+            repeat=output_height * output_width,
+            length=out_channels * output_height * output_width
+        )
+
+    def forward(self, enc_x: CKKSWrapper) -> CKKSWrapper:
+        enc_output = typing.cast(
+            CKKSWrapper,
+            Conv2dFunction.apply(
+                enc_x, self.weight, self.bias, self.conv2d_padding_transformation, self.conv2d_inverse_padding_transformation, self.conv2d_weight_mask, self.conv2d_bias_transformation, self.training
             )
+        )
+
+        return enc_output
+
+    def train(self, mode=True) -> "Conv2d":
+        if mode:
+            # Inplace encrypt the parameters
+            self.weight.inplace_encrypt()
+            self.bias.inplace_encrypt()
+        else:
+            # Inplace decrypt the parameters
+            self.weight.inplace_decrypt()
+            self.bias.inplace_decrypt()
 
-    # Reshape the output tensor
-    weight_convolutions = weight_convolutions.view(
-        kernel_out_channel * output_height * output_width,
-        input_in_channel * input_height * input_width
-    )
+        return super(Conv2d, self).train(mode)
 
-    return weight_convolutions
+    def eval(self) -> "Conv2d":
+        return self.train(False)
```

### Comparing `torchseal-0.1.2/src/torchseal.egg-info/PKG-INFO` & `torchseal-0.2.0/src/torchseal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchseal
-Version: 0.1.2
+Version: 0.2.0
 Summary: PyTorch extension to enable training and testing using homomorphic encryption
 Author-email: Rayhan Kinan Muhannad <rayhankinan@gmail.com>
 Project-URL: Homepage, https://github.com/cnn-for-ckks/pytorch-for-tenseal
 Project-URL: Issues, https://github.com/cnn-for-ckks/pytorch-for-tenseal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `torchseal-0.1.2/src/torchseal.egg-info/SOURCES.txt` & `torchseal-0.2.0/src/torchseal.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,40 @@
 src/torchseal.egg-info/SOURCES.txt
 src/torchseal.egg-info/dependency_links.txt
 src/torchseal.egg-info/requires.txt
 src/torchseal.egg-info/top_level.txt
 src/torchseal/function/__init__.py
 src/torchseal/function/average2d.py
 src/torchseal/function/conv2d.py
+src/torchseal/function/cross_entropy.py
 src/torchseal/function/linear.py
-src/torchseal/function/max2d.py
+src/torchseal/function/mse.py
 src/torchseal/function/relu.py
 src/torchseal/function/sigmoid.py
 src/torchseal/function/square.py
 src/torchseal/function/tanh.py
 src/torchseal/nn/__init__.py
 src/torchseal/nn/average2d.py
 src/torchseal/nn/conv2d.py
+src/torchseal/nn/cross_entropy.py
 src/torchseal/nn/linear.py
-src/torchseal/nn/max2d.py
+src/torchseal/nn/mse.py
 src/torchseal/nn/relu.py
 src/torchseal/nn/sigmoid.py
-src/torchseal/nn/softmax.py
 src/torchseal/nn/square.py
 src/torchseal/nn/tanh.py
+src/torchseal/optim/__init__.py
+src/torchseal/optim/sgd.py
+src/torchseal/state/__init__.py
+src/torchseal/state/context.py
 src/torchseal/utils/__init__.py
+src/torchseal/utils/average2d.py
+src/torchseal/utils/block.py
+src/torchseal/utils/conv2d.py
+src/torchseal/utils/handle_batch_size.py
+src/torchseal/utils/near_zeros.py
+src/torchseal/utils/padding.py
+src/torchseal/utils/sparse.py
 src/torchseal/utils/toeplitz.py
 src/torchseal/wrapper/__init__.py
 src/torchseal/wrapper/ckks.py
 src/torchseal/wrapper/function.py
```


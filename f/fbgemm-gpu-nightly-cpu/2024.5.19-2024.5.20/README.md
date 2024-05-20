# Comparing `tmp/fbgemm_gpu_nightly_cpu-2024.5.19-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2024.5.20-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,60 +1,60 @@
-Zip file size: 3164700 bytes, number of entries: 58
--rw-r--r--  2.0 unx     1342 b- defN 24-May-19 13:00 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx     3079 b- defN 24-May-19 13:00 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      789 b- defN 24-May-19 13:00 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10924536 b- defN 24-May-19 13:00 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5663 b- defN 24-May-19 13:00 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2362 b- defN 24-May-19 13:00 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2752 b- defN 24-May-19 13:00 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7885 b- defN 24-May-19 13:00 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4020 b- defN 24-May-19 13:00 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     6947 b- defN 24-May-19 13:00 fbgemm_gpu/runtime_monitor.py
--rw-r--r--  2.0 unx    30886 b- defN 24-May-19 13:00 fbgemm_gpu/sparse_ops.py
--rw-r--r--  2.0 unx     5774 b- defN 24-May-19 13:00 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     7058 b- defN 24-May-19 13:00 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      540 b- defN 24-May-19 13:00 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    26853 b- defN 24-May-19 13:00 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2339 b- defN 24-May-19 13:00 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     4035 b- defN 24-May-19 13:00 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    67230 b- defN 24-May-19 13:00 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx   101933 b- defN 24-May-19 13:00 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    40800 b- defN 24-May-19 13:00 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      925 b- defN 24-May-19 13:00 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx      419 b- defN 24-May-19 13:00 fbgemm_gpu/docs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 24-May-19 13:00 fbgemm_gpu/docs/common.py
--rw-r--r--  2.0 unx     2377 b- defN 24-May-19 13:00 fbgemm_gpu/docs/examples.py
--rw-r--r--  2.0 unx     7381 b- defN 24-May-19 13:00 fbgemm_gpu/docs/jagged_tensor_ops.py
--rw-r--r--  2.0 unx     7708 b- defN 24-May-19 13:00 fbgemm_gpu/docs/table_batched_embedding_ops.py
--rw-r--r--  2.0 unx      264 b- defN 24-May-19 13:00 fbgemm_gpu/docs/version.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4180 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4180 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
--rw-r--r--  2.0 unx     2147 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3395 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
--rw-r--r--  2.0 unx     3144 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     3144 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
--rw-r--r--  2.0 unx     2420 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2420 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     3100 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
--rw-r--r--  2.0 unx     4512 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     4512 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
--rw-r--r--  2.0 unx     3964 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3964 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
--rw-r--r--  2.0 unx     3762 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     3762 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
--rw-r--r--  2.0 unx      649 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6162 b- defN 24-May-19 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx      231 b- defN 24-May-19 13:00 fbgemm_gpu/tbe/__init__.py
--rw-r--r--  2.0 unx      308 b- defN 24-May-19 13:00 fbgemm_gpu/tbe/cache/__init__.py
--rw-r--r--  2.0 unx     1660 b- defN 24-May-19 13:00 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
--rw-r--r--  2.0 unx     2602 b- defN 24-May-19 13:00 fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-May-19 13:00 fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-19 13:00 fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6301 b- defN 24-May-19 13:00 fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/RECORD
-58 files, 11357756 bytes uncompressed, 3154168 bytes compressed:  72.2%
+Zip file size: 3164697 bytes, number of entries: 58
+-rw-r--r--  2.0 unx     1342 b- defN 24-May-20 12:59 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx     3079 b- defN 24-May-20 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      789 b- defN 24-May-20 12:59 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10924536 b- defN 24-May-20 12:59 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5663 b- defN 24-May-20 12:59 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-May-20 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-May-20 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-May-20 12:59 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4020 b- defN 24-May-20 12:59 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     6947 b- defN 24-May-20 12:59 fbgemm_gpu/runtime_monitor.py
+-rw-r--r--  2.0 unx    30886 b- defN 24-May-20 12:59 fbgemm_gpu/sparse_ops.py
+-rw-r--r--  2.0 unx     5774 b- defN 24-May-20 12:59 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     7058 b- defN 24-May-20 12:59 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      540 b- defN 24-May-20 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    26853 b- defN 24-May-20 12:59 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-May-20 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     4035 b- defN 24-May-20 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    67230 b- defN 24-May-20 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx   101933 b- defN 24-May-20 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    40800 b- defN 24-May-20 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      925 b- defN 24-May-20 12:59 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx      419 b- defN 24-May-20 12:59 fbgemm_gpu/docs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 24-May-20 12:59 fbgemm_gpu/docs/common.py
+-rw-r--r--  2.0 unx     2377 b- defN 24-May-20 12:59 fbgemm_gpu/docs/examples.py
+-rw-r--r--  2.0 unx     7381 b- defN 24-May-20 12:59 fbgemm_gpu/docs/jagged_tensor_ops.py
+-rw-r--r--  2.0 unx     7708 b- defN 24-May-20 12:59 fbgemm_gpu/docs/table_batched_embedding_ops.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-20 12:59 fbgemm_gpu/docs/version.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
+-rw-r--r--  2.0 unx     2147 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
+-rw-r--r--  2.0 unx      649 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6162 b- defN 24-May-20 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx      231 b- defN 24-May-20 12:59 fbgemm_gpu/tbe/__init__.py
+-rw-r--r--  2.0 unx      308 b- defN 24-May-20 12:59 fbgemm_gpu/tbe/cache/__init__.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-20 12:59 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
+-rw-r--r--  2.0 unx     2602 b- defN 24-May-20 12:59 fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 24-May-20 12:59 fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-20 12:59 fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6301 b- defN 24-May-20 12:59 fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/RECORD
+58 files, 11357756 bytes uncompressed, 3154165 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -156,20 +156,20 @@
 
 Filename: fbgemm_gpu/tbe/cache/__init__.py
 Comment: 
 
 Filename: fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/docs/version.py

```diff
@@ -2,8 +2,8 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-__version__: str = "2024.5.19"
+__version__: str = "2024.5.20"
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm_gpu_nightly-cpu
-Version: 2024.5.19
+Version: 2024.5.20
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=cm1TiXU9SDDv7t9AEOjw2KntViShpOp8TZSVf8jBm48,40800
 fbgemm_gpu/uvm.py,sha256=-cZunsuvnAKUEQptIwdYVar_3hUE99FbQUsyfBVeXPE,925
 fbgemm_gpu/docs/__init__.py,sha256=Rh8Kn4L7LJRqCFWILZD7wReoBy8ZD2R_TfEzWHVCoA0,419
 fbgemm_gpu/docs/common.py,sha256=8ipXTwVb222X-aZ71O6n8fhxHCHPNhJEHMFiO7epcIs,273
 fbgemm_gpu/docs/examples.py,sha256=ZMN_6sL74LH_hrp2bF_hmg8gi29GhcgvwV3kCMjxkoE,2377
 fbgemm_gpu/docs/jagged_tensor_ops.py,sha256=Bsx-ZxvvdMv5CaldSvuw9GPR-HRcLbRR2IEXCOCm9r0,7381
 fbgemm_gpu/docs/table_batched_embedding_ops.py,sha256=h_EQOIMsdVlr-Pygul-fDGxx7JqLRjaBMI_z0PFrGAE,7708
-fbgemm_gpu/docs/version.py,sha256=sag7mZ-qQrbm22_f_ITNEkShPrmNi5t8rLlM00g4klA,264
+fbgemm_gpu/docs/version.py,sha256=ZwuOuwcyod3L2fLZhtbHFuYfi5IPObS_7uRLrby4BAE,264
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=lfob_IDNeAs2FjS2WCldKlw0gm_qUZdp043fngI8sGE,1466
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py,sha256=ibfUa6H9BY85_e9VgbKujKi4nuR7Mgyw77VbFMkLKCs,2147
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py,sha256=xhDnYR0vVDSK96nbcNSs5NbGXqFF3FGIs3DPDBJYt08,3395
@@ -48,11 +48,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=yiD3_bG5yT5VXLoGw4eeRKQ2Nj087DRq0qKCVPb52SY,649
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=OFw5PM2YDiKvr6T9ZW7BKiq58gB7txcKfuJkBUROxdI,6162
 fbgemm_gpu/tbe/__init__.py,sha256=fE0IHi1JJpxsNVBNzWNee2thrNXFFRhY94c80RxNSIE,231
 fbgemm_gpu/tbe/cache/__init__.py,sha256=kueJp-xYnDflz4DYf7dh5_xtx5ItzrbQc_1neoe5XQc,308
 fbgemm_gpu/tbe/cache/split_embeddings_cache_ops.py,sha256=F2XIec8Kgcihy1vXJRp0tQErqIQSQIDZRuzLfkasE70,1660
-fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/METADATA,sha256=M8p7EVK1lwBMWFMlvH-X2KGlAdZKL2wcmw8vX77CEKw,2602
-fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
-fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2024.5.19.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/METADATA,sha256=ck9AplucbYLPBEQl6iePrtkyzVJZEAzDzxhEpZo6c3s,2602
+fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
+fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2024.5.20.dist-info/RECORD,,
```


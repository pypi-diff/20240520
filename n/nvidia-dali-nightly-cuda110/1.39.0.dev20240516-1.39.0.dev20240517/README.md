# Comparing `tmp/nvidia_dali_nightly_cuda110-1.39.0.dev20240516.tar.gz` & `tmp/nvidia_dali_nightly_cuda110-1.39.0.dev20240517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_nightly_cuda110-1.39.0.dev20240516.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_nightly_cuda110-1.39.0.dev20240517.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_nightly_cuda110-1.39.0.dev20240516.tar` & `nvidia_dali_nightly_cuda110-1.39.0.dev20240517.tar`

### PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.39.0.dev20240516
-Summary: NVIDIA DALI nightly  for CUDA 11.0. Git SHA: 17458b7b47e22d7cd76d18e2624e3c7431278386
+Version: 1.39.0.dev20240517
+Summary: NVIDIA DALI nightly  for CUDA 11.0. Git SHA: 306221661a585ed7791857141e15b69e28952905
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

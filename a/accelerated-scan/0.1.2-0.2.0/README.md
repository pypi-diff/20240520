# Comparing `tmp/accelerated_scan-0.1.2.tar.gz` & `tmp/accelerated_scan-0.2.0.tar.gz`

## Comparing `accelerated_scan-0.1.2.tar` & `accelerated_scan-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0    43724 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/bench.png
--rw-r--r--   0        0        0    24798 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/max-abs-error.png
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/accelerated_scan/__init__.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/accelerated_scan/ref.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/accelerated_scan/triton.py
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/accelerated_scan/warp.cuh
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/accelerated_scan/warp.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/tests/test_eq.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/LICENSE
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/README.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 accelerated_scan-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/CITATION.cff
+-rw-r--r--   0        0        0    43724 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/bench.png
+-rw-r--r--   0        0        0    24798 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/max-abs-error.png
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/accelerated_scan/__init__.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/accelerated_scan/ref.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/accelerated_scan/triton.py
+-rw-r--r--   0        0        0    18149 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/accelerated_scan/warp.cuh
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/accelerated_scan/warp.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/tests/bench.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/tests/test_eq.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 accelerated_scan-0.2.0/PKG-INFO
```

### Comparing `accelerated_scan-0.1.2/bench.png` & `accelerated_scan-0.2.0/bench.png`

 * *Files identical despite different names*

### Comparing `accelerated_scan-0.1.2/max-abs-error.png` & `accelerated_scan-0.2.0/max-abs-error.png`

 * *Files identical despite different names*

### Comparing `accelerated_scan-0.1.2/.github/workflows/release.yml` & `accelerated_scan-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `accelerated_scan-0.1.2/accelerated_scan/ref.py` & `accelerated_scan-0.2.0/accelerated_scan/ref.py`

 * *Files identical despite different names*

### Comparing `accelerated_scan-0.1.2/accelerated_scan/triton.py` & `accelerated_scan-0.2.0/accelerated_scan/triton.py`

 * *Files identical despite different names*

### Comparing `accelerated_scan-0.1.2/tests/test_eq.py` & `accelerated_scan-0.2.0/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `accelerated_scan-0.1.2/LICENSE` & `accelerated_scan-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `accelerated_scan-0.1.2/README.md` & `accelerated_scan-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Accelerated Scan
 
-[![PyPI Version](https://img.shields.io/pypi/v/accelerated-scan.svg)](https://pypi.python.org/pypi/accelerated-scan)
+[![PyPI Version](https://img.shields.io/pypi/v/accelerated-scan.svg)](https://pypi.python.org/pypi/accelerated-scan) [![DOI](https://zenodo.org/badge/741400326.svg)](https://zenodo.org/doi/10.5281/zenodo.10600962)
+
 
 This package implements the fastest [first-order parallel associative scan](https://www.cs.cmu.edu/~guyb/papers/Ble93.pdf) on the GPU for forward and [backward](https://arxiv.org/abs/1709.04057).
 
 The scan efficiently solves first-order recurrences of the form `x[t] = gate[t] * x[t-1] + token[t]`, common in state space models and linear RNNs.
 
 The `accelerated_scan.warp` C++ CUDA kernel uses a chunked processing algorithm that leverages the fastest GPU communication primitives available
 on each level of hierarchy: [warp shuffles](https://developer.nvidia.com/blog/using-cuda-warp-level-primitives/) within warps of 32 threads and shared memory (SRAM) between warps within a thread block. One sequence per channel dimension is confined to one thread block.
```

### Comparing `accelerated_scan-0.1.2/pyproject.toml` & `accelerated_scan-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accelerated_scan-0.1.2/PKG-INFO` & `accelerated_scan-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: accelerated-scan
-Version: 0.1.2
+Version: 0.2.0
 Author-email: Volodymyr Kyrylov <vol@wilab.org.ua>
 License: MIT License
         
         Copyright (c) 2024 Volodymyr Kyrylov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -29,15 +29,16 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: torch>=2.1.0
 Description-Content-Type: text/markdown
 
 # Accelerated Scan
 
-[![PyPI Version](https://img.shields.io/pypi/v/accelerated-scan.svg)](https://pypi.python.org/pypi/accelerated-scan)
+[![PyPI Version](https://img.shields.io/pypi/v/accelerated-scan.svg)](https://pypi.python.org/pypi/accelerated-scan) [![DOI](https://zenodo.org/badge/741400326.svg)](https://zenodo.org/doi/10.5281/zenodo.10600962)
+
 
 This package implements the fastest [first-order parallel associative scan](https://www.cs.cmu.edu/~guyb/papers/Ble93.pdf) on the GPU for forward and [backward](https://arxiv.org/abs/1709.04057).
 
 The scan efficiently solves first-order recurrences of the form `x[t] = gate[t] * x[t-1] + token[t]`, common in state space models and linear RNNs.
 
 The `accelerated_scan.warp` C++ CUDA kernel uses a chunked processing algorithm that leverages the fastest GPU communication primitives available
 on each level of hierarchy: [warp shuffles](https://developer.nvidia.com/blog/using-cuda-warp-level-primitives/) within warps of 32 threads and shared memory (SRAM) between warps within a thread block. One sequence per channel dimension is confined to one thread block.
```


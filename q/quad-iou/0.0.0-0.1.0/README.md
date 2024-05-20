# Comparing `tmp/quad_iou-0.0.0.tar.gz` & `tmp/quad_iou-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quad_iou-0.0.0.tar", last modified: Sat May 18 21:35:46 2024, max compression
+gzip compressed data, was "quad_iou-0.1.0.tar", last modified: Mon May 20 11:45:38 2024, max compression
```

## Comparing `quad_iou-0.0.0.tar` & `quad_iou-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.649158 quad_iou-0.0.0/
--rw-r--r--   0 isalia    (1000) isalia    (1000)      544 2024-05-18 20:51:33.000000 quad_iou-0.0.0/LICENSE
--rw-r--r--   0 isalia    (1000) isalia    (1000)       91 2024-05-18 19:47:42.000000 quad_iou-0.0.0/MANIFEST.in
--rw-r--r--   0 isalia    (1000) isalia    (1000)     1763 2024-05-18 21:35:46.649158 quad_iou-0.0.0/PKG-INFO
--rw-r--r--   0 isalia    (1000) isalia    (1000)     1354 2024-05-18 21:29:00.000000 quad_iou-0.0.0/README.md
--rw-r--r--   0 isalia    (1000) isalia    (1000)       38 2024-05-18 21:35:46.649158 quad_iou-0.0.0/setup.cfg
--rw-rw-r--   0 isalia    (1000) isalia    (1000)     1000 2024-05-18 21:27:58.000000 quad_iou-0.0.0/setup.py
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.645158 quad_iou-0.0.0/src/
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.649158 quad_iou-0.0.0/src/cuda/
--rw-r--r--   0 isalia    (1000) isalia    (1000)      579 2024-05-18 16:19:02.000000 quad_iou-0.0.0/src/cuda/allPoints.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)      799 2024-05-15 17:20:33.000000 quad_iou-0.0.0/src/cuda/checks.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)     3285 2024-05-18 17:29:58.000000 quad_iou-0.0.0/src/cuda/insidePoints.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)     3794 2024-05-18 17:29:59.000000 quad_iou-0.0.0/src/cuda/intersectionPoints.cuh
--rw-rw-r--   0 isalia    (1000) isalia    (1000)     2007 2024-05-18 17:30:01.000000 quad_iou-0.0.0/src/cuda/polygonArea.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)     8187 2024-05-18 20:22:00.000000 quad_iou-0.0.0/src/cuda/quad_iou_tensors.cu
--rw-r--r--   0 isalia    (1000) isalia    (1000)      289 2024-05-18 19:44:34.000000 quad_iou-0.0.0/src/cuda/quad_iou_tensors_cuda.cpp
--rw-rw-r--   0 isalia    (1000) isalia    (1000)     1925 2024-05-16 07:28:12.000000 quad_iou-0.0.0/src/cuda/simpleIntersectCheck.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)     5028 2024-05-18 17:30:12.000000 quad_iou-0.0.0/src/cuda/sortPoints.cuh
--rw-r--r--   0 isalia    (1000) isalia    (1000)      147 2024-05-18 17:30:14.000000 quad_iou-0.0.0/src/cuda/utils.cuh
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.649158 quad_iou-0.0.0/src/quad_iou/
--rw-r--r--   0 isalia    (1000) isalia    (1000)       73 2024-05-18 20:36:15.000000 quad_iou-0.0.0/src/quad_iou/__init__.py
--rw-r--r--   0 isalia    (1000) isalia    (1000)     1237 2024-05-18 20:27:56.000000 quad_iou-0.0.0/src/quad_iou/wrap.py
-drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-18 21:35:46.649158 quad_iou-0.0.0/src/quad_iou.egg-info/
--rw-r--r--   0 isalia    (1000) isalia    (1000)     1763 2024-05-18 21:35:46.000000 quad_iou-0.0.0/src/quad_iou.egg-info/PKG-INFO
--rw-r--r--   0 isalia    (1000) isalia    (1000)      495 2024-05-18 21:35:46.000000 quad_iou-0.0.0/src/quad_iou.egg-info/SOURCES.txt
--rw-r--r--   0 isalia    (1000) isalia    (1000)        1 2024-05-18 21:35:46.000000 quad_iou-0.0.0/src/quad_iou.egg-info/dependency_links.txt
--rw-r--r--   0 isalia    (1000) isalia    (1000)       25 2024-05-18 21:35:46.000000 quad_iou-0.0.0/src/quad_iou.egg-info/top_level.txt
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-20 11:45:38.906291 quad_iou-0.1.0/
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      544 2024-05-18 21:45:47.000000 quad_iou-0.1.0/LICENSE
+-rw-r--r--   0 isalia    (1000) isalia    (1000)       88 2024-05-20 11:20:34.000000 quad_iou-0.1.0/MANIFEST.in
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     1422 2024-05-20 11:45:38.906291 quad_iou-0.1.0/PKG-INFO
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     1075 2024-05-20 11:11:19.000000 quad_iou-0.1.0/README.md
+-rw-r--r--   0 isalia    (1000) isalia    (1000)       38 2024-05-20 11:45:38.906291 quad_iou-0.1.0/setup.cfg
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     1151 2024-05-20 11:41:03.000000 quad_iou-0.1.0/setup.py
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-20 11:45:38.906291 quad_iou-0.1.0/src/
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-20 11:45:38.906291 quad_iou-0.1.0/src/core/
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      700 2024-05-20 10:20:25.000000 quad_iou-0.1.0/src/core/allPoints.h
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      657 2024-05-20 10:34:06.000000 quad_iou-0.1.0/src/core/checks.h
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     3404 2024-05-20 10:20:33.000000 quad_iou-0.1.0/src/core/insidePoints.h
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     3914 2024-05-20 10:20:39.000000 quad_iou-0.1.0/src/core/intersectionPoints.h
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     2125 2024-05-20 10:21:33.000000 quad_iou-0.1.0/src/core/polygonArea.h
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     6097 2024-05-20 11:00:04.000000 quad_iou-0.1.0/src/core/quad_iou_tensors.cpp
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     8305 2024-05-20 10:28:04.000000 quad_iou-0.1.0/src/core/quad_iou_tensors.cu
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      449 2024-05-20 10:03:00.000000 quad_iou-0.1.0/src/core/quad_iou_tensors_bind_torch.cpp
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     2045 2024-05-20 10:20:54.000000 quad_iou-0.1.0/src/core/simpleIntersectCheck.h
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     5151 2024-05-20 10:21:01.000000 quad_iou-0.1.0/src/core/sortPoints.h
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      148 2024-05-20 10:21:03.000000 quad_iou-0.1.0/src/core/utils.h
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-20 11:45:38.906291 quad_iou-0.1.0/src/quad_iou/
+-rw-r--r--   0 isalia    (1000) isalia    (1000)       73 2024-05-20 10:37:59.000000 quad_iou-0.1.0/src/quad_iou/__init__.py
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     1662 2024-05-20 11:26:55.000000 quad_iou-0.1.0/src/quad_iou/wrap.py
+drwxr-xr-x   0 isalia    (1000) isalia    (1000)        0 2024-05-20 11:45:38.906291 quad_iou-0.1.0/src/quad_iou.egg-info/
+-rw-r--r--   0 isalia    (1000) isalia    (1000)     1422 2024-05-20 11:45:38.000000 quad_iou-0.1.0/src/quad_iou.egg-info/PKG-INFO
+-rw-r--r--   0 isalia    (1000) isalia    (1000)      515 2024-05-20 11:45:38.000000 quad_iou-0.1.0/src/quad_iou.egg-info/SOURCES.txt
+-rw-r--r--   0 isalia    (1000) isalia    (1000)        1 2024-05-20 11:45:38.000000 quad_iou-0.1.0/src/quad_iou.egg-info/dependency_links.txt
+-rw-r--r--   0 isalia    (1000) isalia    (1000)       36 2024-05-20 11:45:38.000000 quad_iou-0.1.0/src/quad_iou.egg-info/top_level.txt
```

### Comparing `quad_iou-0.0.0/LICENSE` & `quad_iou-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quad_iou-0.0.0/README.md` & `quad_iou-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-# IoU(Intersection over Union) Calculation for Quadrilaterals(CUDA Kernel)
+# IoU(Intersection over Union) Calculation for Quadrilaterals(Torch extension)
 
-Cuda kernel for calculating IoU(intersection over union) for quadrilaterals. It can calculate IoU either for 1->1 match or N->M match, returning an iou matrix with N rows and M columns. Torch CUDA extensions are used for running the compiled kernels. 
+Torch extension for calculating IoU (Intersection over Union) for quadrilaterals. It can calculate IoU either for a 1-to-1 match or an M-to-N match, returning an IoU matrix with M rows and N columns. Torch CUDA/CPP extensions are used for binding the code to Torch.
 
 ## Example usage:
 ```
 import torch
 import quad_iou
 
 # NxM quadrilaterals
-a = torch.rand((200, 4, 2)).cuda()
+a = torch.rand((200, 4, 2)).cuda() # Can also be without cuda
 b = torch.rand((300, 4, 2)).cuda()
 
 # sort_input_quads indicate whether kernel should sort the quadrilateral corners
 # clockwise before calculating iou
 iou_matrix = quad_iou.calculate_iou(a, b, sort_input_quads=True) # returns tensor of shape [200, 300]
 
 # 1x1 case
-a = torch.tensor([0.0, 0, 300, 0, 300, 300, 0, 300]).cuda()
+a = torch.tensor([0.0, 0, 300, 0, 300, 300, 0, 300]).cuda() # Can also be without cuda
 b = torch.tensor([0.0, 0, 150, 0, 150, 150, 0, 150]).cuda()
 # Module expects tensor of shape [N, 4, 2], so we reshape the tensors
 a = a.reshape(-1, 4, 2)
 b = b.reshape(-1, 4, 2)
 iou = quad_iou.calculate_iou(a, b, sort_input_quads=True)
 ```
-
-## Comparison with Shapely library
-
-While CPUs and GPUs are not to be compared for speed, we provide a script to demonstrate the potential speedup when using a GPU. To compare the execution time of calculating the IoU for quadrilaterals using the `Shapely` library versus our GPU-accelerated implementation, run `python tryout_scripts/comparison.py`
```

### Comparing `quad_iou-0.0.0/setup.py` & `quad_iou-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 from setuptools import setup, find_packages
-from torch.utils.cpp_extension import BuildExtension, CUDAExtension
+from torch.utils.cpp_extension import BuildExtension, CUDAExtension, CppExtension
+import torch
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
+ext_modules = [
+    CppExtension("quad_iou_cpu", [
+        "src/core/quad_iou_tensors_bind_torch.cpp",
+        "src/core/quad_iou_tensors.cpp",
+    ])
+]
+
+if torch.cuda.is_available():
+    ext_modules.append(
+        CUDAExtension('quad_iou_cuda', [
+            'src/core/quad_iou_tensors_bind_torch.cpp',
+            'src/core/quad_iou_tensors.cu',
+        ])
+    )
+
 setup(
     name="quad_iou",
-    version="0.0.0",
+    version="0.1.0",
     author="Irakli Salia",
     author_email="irakli.salia854@gmail.com",
-    description="A CUDA extension for calculating IoU(Intersection over Union) for quadrilaterals(MxN) bound to PyTorch(usable with torch tensors).",
+    description="Torch extension for calculating IoU(Intersection over Union) for quadrilaterals(MxN)",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="https://github.com/Isalia20/quadrilaterals_iou_cuda_kernel",  # Update with your repository URL
+    url="https://github.com/Isalia20/quad-iou-torch",
     package_dir={'': 'src'},
     packages=find_packages(where="src"),
-    ext_modules=[
-        CUDAExtension('quad_iou_kernel', [
-            'src/cuda/quad_iou_tensors_cuda.cpp',
-            'src/cuda/quad_iou_tensors.cu',
-        ]),
-    ],
+    ext_modules=ext_modules,
     cmdclass={
         'build_ext': BuildExtension
     },
     python_requires='>=3.9',
-)
+)
```

### Comparing `quad_iou-0.0.0/src/cuda/allPoints.cuh` & `quad_iou-0.1.0/src/core/allPoints.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 #define MAX_INTERSECTION_POINTS 8
 #define MAX_INSIDE_POINTS 8
 #define MAX_ALL_POINTS 16
 #include <torch/extension.h>
+#ifdef __CUDACC__
+#include <cuda_runtime.h>
+#define HOST_DEVICE __host__ __device__
+#else
+#define HOST_DEVICE
+#endif
+
 
 template <typename scalar_t>
-__device__ inline void fillArrayWithInfinity(scalar_t points[][2], int num_points){
+HOST_DEVICE inline void fillArrayWithInfinity(scalar_t points[][2], int num_points){
     #pragma unroll
     for (int i = 0; i < num_points; i++){
         points[i][0] = INFINITY;
         points[i][1] = INFINITY;
     }
 }
 
 namespace allPoints {
     template <typename scalar_t>
-    __device__ inline void fillPointsWithInfinity(scalar_t all_points[MAX_ALL_POINTS][2]){
+    HOST_DEVICE inline void fillPointsWithInfinity(scalar_t all_points[MAX_ALL_POINTS][2]){
         fillArrayWithInfinity(all_points, MAX_ALL_POINTS);
     }
-}
+}
```

### Comparing `quad_iou-0.0.0/src/cuda/checks.cuh` & `quad_iou-0.1.0/src/core/checks.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 #include <torch/extension.h>
-#define CHECK_CUDA(x) TORCH_CHECK(x.device().is_cuda(), #x " must be a CUDA tensor");
 
 namespace checks {
     void check_tensor_validity(torch::Tensor& quad_0, torch::Tensor& quad_1){
-        CHECK_CUDA(quad_0);
-        CHECK_CUDA(quad_1);
         TORCH_CHECK(quad_0.is_contiguous() && quad_1.is_contiguous(), "Input tensors must be contiguous");
         TORCH_CHECK(quad_0.numel() > 0 && quad_1.numel() > 0, "Input tensors must not empty");
         TORCH_CHECK(quad_0.dim() == 3, "Input tensor must contain 3 dimensions");
         TORCH_CHECK(quad_0.size(1) == 4 && quad_1.size(1) == 4, "Input tensors must have 4 values on 2nd dim(dim=1)");
         TORCH_CHECK(quad_0.size(2) == 2 && quad_1.size(2) == 2, "Input tensors must have 2 values on last dim(dim=2)");
     }
 }
```

### Comparing `quad_iou-0.0.0/src/cuda/insidePoints.cuh` & `quad_iou-0.1.0/src/core/insidePoints.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 #define MAX_ALL_POINTS 16
 #include <torch/extension.h>
-#include "utils.cuh"
+#include "utils.h"
+#ifdef __CUDACC__
+#include <cuda_runtime.h>
+#define HOST_DEVICE __host__ __device__
+#else
+#define HOST_DEVICE
+#endif
 
 template <typename scalar_t>
-__device__ inline scalar_t findMaxQuadCoordinate(const scalar_t *box, Coordinate coord){
+HOST_DEVICE inline scalar_t findMaxQuadCoordinate(const scalar_t *box, Coordinate coord){
     // Find the maximum x-coordinate or y-coordinate of the quadrilateral based on the coord value
     scalar_t max_value = box[static_cast<int>(coord)];
     #pragma unroll
     for (int i = 1; i < 4; ++i) {
         if (box[i * 2 + static_cast<int>(coord)] > max_value) {
             max_value = box[i * 2 + static_cast<int>(coord)];
         }
     }
     return max_value;
 }
 
 template <typename scalar_t>
-__device__ inline int isPointInsideQuadrilateral(const Point<scalar_t>& point_to_check, const scalar_t *box) {
+HOST_DEVICE inline int isPointInsideQuadrilateral(const Point<scalar_t>& point_to_check, const scalar_t *box) {
     scalar_t max_x = findMaxQuadCoordinate(box, Coordinate::X);
     scalar_t max_y = findMaxQuadCoordinate(box, Coordinate::Y);
     // If the point's x-coordinate is greater than the max x-coordinate, it's outside
     if (point_to_check.x > max_x) return -1;
     if (point_to_check.y > max_y) return -1;
 
     #pragma unroll
@@ -40,15 +46,15 @@
         }
     }
     return 1; // Point is inside the quadrilateral
 }
 
 namespace insidePoints{
     template <typename scalar_t>
-    __device__ inline void findPointsInside(const scalar_t *quad_0, 
+    HOST_DEVICE inline void findPointsInside(const scalar_t *quad_0, 
                                             const scalar_t *quad_1, 
                                             scalar_t inside_points[MAX_ALL_POINTS][2],
                                             int numIntersections) {
         int numInsidePoints = numIntersections;
         #pragma unroll
         for (int i = 0; i < 4; i++) {
             Point<scalar_t> quad_0_point = {quad_0[i * 2], quad_0[i * 2 + 1]};
@@ -65,8 +71,8 @@
                     inside_points[numInsidePoints][0] = quad_1[i * 2];
                     inside_points[numInsidePoints][1] = quad_1[i * 2 + 1];
                     numInsidePoints++;
                 }
             }
         }
     }
-}
+}
```

### Comparing `quad_iou-0.0.0/src/cuda/intersectionPoints.cuh` & `quad_iou-0.1.0/src/core/intersectionPoints.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 #define MAX_INTERSECTION_POINTS 8
 #define MAX_ALL_POINTS 16
 #define EPSILON 1e-6
 #include <torch/extension.h>
-#include "utils.cuh"
+#include "utils.h"
+#ifdef __CUDACC__
+#include <cuda_runtime.h>
+#define HOST_DEVICE __host__ __device__
+#else
+#define HOST_DEVICE
+#endif
 
 template <typename scalar_t>
-__device__ inline bool arePointsEqual(const Point<scalar_t>& p1, const Point<scalar_t>& p2) {
+HOST_DEVICE inline bool arePointsEqual(const Point<scalar_t>& p1, const Point<scalar_t>& p2) {
     return fabsf(p1.x - p2.x) < EPSILON && fabsf(p1.y - p2.y) < EPSILON;
 }
 
 template <typename scalar_t>
-__device__ inline int orientation(const Point<scalar_t>& p, const Point<scalar_t>& q, const Point<scalar_t>& r) {
+HOST_DEVICE inline int orientation(const Point<scalar_t>& p, const Point<scalar_t>& q, const Point<scalar_t>& r) {
     scalar_t val = (q.y - p.y) * (r.x - q.x) - (q.x - p.x) * (r.y - q.y);
     if (fabsf(val) < EPSILON) return 0;  // colinear
     return (val > 0) ? 1 : 2;  // clockwise
 }
 
 template <typename scalar_t>
-__device__ inline bool doIntersect(const Point<scalar_t>& p1, const Point<scalar_t>& q1, const Point<scalar_t>& p2, const Point<scalar_t>& q2, Point<scalar_t>& intersection) {
+HOST_DEVICE inline bool doIntersect(const Point<scalar_t>& p1, const Point<scalar_t>& q1, const Point<scalar_t>& p2, const Point<scalar_t>& q2, Point<scalar_t>& intersection) {
     // Find the four orientations needed for general and
     // special cases
     int o1 = orientation(p1, q1, p2);
     int o2 = orientation(p1, q1, q2);
     int o3 = orientation(p2, q2, p1);
     int o4 = orientation(p2, q2, q1);
 
@@ -48,15 +54,15 @@
     }
     
     return false; // Doesn't fall in any of the above cases
 }
 
 namespace intersectionPoints{    
     template <typename scalar_t>
-    __device__ inline int findIntersectionPoints(const scalar_t *quad_0, 
+    HOST_DEVICE inline int findIntersectionPoints(const scalar_t *quad_0, 
                                                   const scalar_t *quad_1, 
                                                   scalar_t intersections[MAX_ALL_POINTS][2]) {
         int numIntersections = 0;
         #pragma unroll
         for (int i = 0; i < 4; ++i) {
             for (int j = 0; j < 4; ++j) {
                 Point<scalar_t> intersection;
@@ -80,8 +86,8 @@
                         numIntersections++;
                     }
                 }
             }
         }
         return numIntersections;
     }
-}
+}
```

### Comparing `quad_iou-0.0.0/src/cuda/polygonArea.cuh` & `quad_iou-0.1.0/src/core/polygonArea.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 #define MAX_ALL_POINTS 16
 #include <torch/extension.h>
-#include "utils.cuh"
+#include "utils.h"
+#ifdef __CUDACC__
+#include <cuda_runtime.h>
+#define HOST_DEVICE __host__ __device__
+#else
+#define HOST_DEVICE
+#endif
 
 namespace polygonArea{
     template <typename scalar_t>
-    __device__ inline scalar_t calcQuadrilateralArea(const scalar_t *quadrilateral) {
+    HOST_DEVICE inline scalar_t calcQuadrilateralArea(const scalar_t *quadrilateral) {
         scalar_t area = 0.0;
         const int vertices = 4;
 
         // Calculate the sum for the Gaussian formula
         #pragma unroll
         for (int i = 1, j = 0; i < vertices; ++i) {
             area += quadrilateral[j * 2] * quadrilateral[i * 2 + 1] - 
@@ -20,15 +26,15 @@
         area += quadrilateral[6] * quadrilateral[1] - 
                 quadrilateral[0] * quadrilateral[7];
 
         return fabs(area) / 2.0;
     }
 
     template <typename scalar_t>
-    __device__ inline scalar_t calcPolygonArea(scalar_t polygon[MAX_ALL_POINTS][2]) {
+    HOST_DEVICE inline scalar_t calcPolygonArea(scalar_t polygon[MAX_ALL_POINTS][2]) {
         scalar_t area = 0;
         int n = MAX_ALL_POINTS;
         int j = 0; // Index of the previous valid vertex
 
         // Initialize the previous valid vertex
         #pragma unroll
         for (int i = 0; i < n; ++i) {
@@ -49,8 +55,8 @@
         // Close the polygon loop if the last vertex is valid
         if (!isinf(polygon[j][0]) && !isinf(polygon[j][1]) && (!isinf(polygon[0][0]) && !isinf(polygon[0][1]))) {
             area += (polygon[j][0] * polygon[0][1] - polygon[0][0] * polygon[j][1]);
         }
 
         return fabs(area) / 2.0;
     }
-}
+}
```

### Comparing `quad_iou-0.0.0/src/cuda/quad_iou_tensors.cu` & `quad_iou-0.1.0/src/core/quad_iou_tensors.cu`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 
 #define QUAD_ELEMENTS 8
 #define MAX_ALL_POINTS 16
 #define THREAD_COUNT_X 16
 #define THREAD_COUNT_Y 16
 #include <torch/extension.h>
 #include <cmath>
-#include "polygonArea.cuh"
-#include "insidePoints.cuh"
-#include "intersectionPoints.cuh"
-#include "sortPoints.cuh"
-#include "allPoints.cuh"
-#include "simpleIntersectCheck.cuh"
-#include "checks.cuh"
+#include "polygonArea.h"
+#include "insidePoints.h"
+#include "intersectionPoints.h"
+#include "sortPoints.h"
+#include "allPoints.h"
+#include "simpleIntersectCheck.h"
+#include "checks.h"
 
 
 template <typename scalar_t>
 __device__ inline scalar_t intersectionArea(
-    const scalar_t *quad_0,
-    const scalar_t *quad_1
+    const scalar_t quad_0[QUAD_ELEMENTS],
+    const scalar_t quad_1[QUAD_ELEMENTS]
 ) {
     // If we know that quad_0 and quad_1 are not
     // intersecting even a tiny bit(minimum enclosing box check)
     // we can skip below calculation altogether
     if (!simpleIntersectCheck::checkSimpleIntersection(quad_0, quad_1)) return 0.0;
 
     scalar_t all_points[MAX_ALL_POINTS][2];
@@ -207,7 +207,9 @@
 
         // Synchronize and free device memory
         cudaDeviceSynchronize();
         cudaFree(polygonAreas_d);
     }));
     return iou_matrix;
 }
+
+torch::Tensor calculateIoUCPUTorch(torch::Tensor quad_0, torch::Tensor quad_1, bool sort_input_quads){}
```

### Comparing `quad_iou-0.0.0/src/cuda/simpleIntersectCheck.cuh` & `quad_iou-0.1.0/src/core/simpleIntersectCheck.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 #include <torch/extension.h>
+#ifdef __CUDACC__
+#include <cuda_runtime.h>
+#define HOST_DEVICE __host__ __device__
+#else
+#define HOST_DEVICE
+#endif
 
 template <typename scalar_t>
-__device__ inline void findMinMaxQuadCoordinate(const scalar_t *box, 
+HOST_DEVICE inline void findMinMaxQuadCoordinate(const scalar_t *box, 
                                                 Coordinate coord, 
                                                 scalar_t& min_val, 
                                                 scalar_t& max_val) {
     // Initialize min and max with the first point's coordinate
     int coord_index = static_cast<int>(coord);
     min_val = box[coord_index];
     max_val = box[coord_index];
@@ -21,15 +27,15 @@
             max_val = val;
         }
     }
 }
 
 namespace simpleIntersectCheck {
     template <typename scalar_t>
-    __device__ inline bool checkSimpleIntersection(const scalar_t *quad_0,
+    HOST_DEVICE inline bool checkSimpleIntersection(const scalar_t *quad_0,
                                                    const scalar_t *quad_1) {
         // Function to check a very simple intersection. If one quad's x's and y's are not overlapping with another's x and y's 
         // we know that intersection area will be 0 and we avoid other calculations in kernel
         scalar_t min_x_0, max_x_0, min_y_0, max_y_0;
         scalar_t min_x_1, max_x_1, min_y_1, max_y_1;
 
         // Find min/max for both quads
@@ -40,8 +46,8 @@
 
         // Check for overlap in the x and y dimensions
         bool overlap_x = (min_x_0 <= max_x_1) && (max_x_0 >= min_x_1);
         bool overlap_y = (min_y_0 <= max_y_1) && (max_y_0 >= min_y_1);
 
         return overlap_x && overlap_y;
     }
-}
+}
```

### Comparing `quad_iou-0.0.0/src/cuda/sortPoints.cuh` & `quad_iou-0.1.0/src/core/sortPoints.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 #define MAX_ALL_POINTS 16
 #define EPSILON 1e-6
 #include <torch/extension.h>
-#include "utils.cuh"
-
+#include "utils.h"
+#ifdef __CUDACC__
+#include <cuda_runtime.h>
+#define HOST_DEVICE __host__ __device__
+#else
+#define HOST_DEVICE
+#endif
 
 template <typename scalar_t>
-__device__ inline scalar_t computeAngle(const Point<scalar_t>& centroid, const Point<scalar_t>& p) {
+HOST_DEVICE inline scalar_t computeAngle(const Point<scalar_t>& centroid, const Point<scalar_t>& p) {
     // Use atan2f for float and atan2 for double
     return (sizeof(scalar_t) == sizeof(double)) ? atan2(p.y - centroid.y, p.x - centroid.x) : atan2f(p.y - centroid.y, p.x - centroid.x);
 }
 
 template <typename scalar_t>
-__device__ inline Point<scalar_t> findCentroid(scalar_t *points) {
+HOST_DEVICE inline Point<scalar_t> findCentroid(scalar_t *points) {
     Point<scalar_t> centroid = {0.0, 0.0};
     #pragma unroll
     for (int i = 0; i < 4; i++) {
         centroid.x += points[i * 2];
         centroid.y += points[i * 2 + 1];
     }
     centroid.x /= 4.0;
     centroid.y /= 4.0;
     return centroid;
 }
 
 template <typename scalar_t>
-__device__ inline Point<scalar_t> findCentroid(scalar_t points[MAX_ALL_POINTS][2]) {
+HOST_DEVICE inline Point<scalar_t> findCentroid(scalar_t points[MAX_ALL_POINTS][2]) {
     Point<scalar_t> centroid = {0.0, 0.0};
     int valid_point_counter = 0;
     #pragma unroll
     for (int i = 0; i < MAX_ALL_POINTS; i++) {
         if (!isinf(points[i][0]) && !isinf(points[i][1])){
             centroid.x += points[i][0];
             centroid.y += points[i][1];
@@ -37,35 +42,35 @@
     }
     centroid.x /= valid_point_counter;
     centroid.y /= valid_point_counter;
     return centroid;
 }
 
 template<typename scalar_t>
-__device__ inline void swapPoints(scalar_t *points, int i){
+HOST_DEVICE inline void swapPoints(scalar_t *points, int i){
     scalar_t tempX = points[i * 2];
     scalar_t tempY = points[i * 2 + 1];
     points[i * 2] = points[(i + 1) * 2];
     points[i * 2 + 1] = points[(i + 1) * 2 + 1];
     points[(i + 1) * 2] = tempX;
     points[(i + 1) * 2 + 1] = tempY;
 }
 
 template<typename scalar_t>
-__device__ inline void swapPoints(scalar_t points[MAX_ALL_POINTS][2], int i){
+HOST_DEVICE inline void swapPoints(scalar_t points[MAX_ALL_POINTS][2], int i){
     scalar_t tempX = points[i][0];
     scalar_t tempY = points[i][1];
     points[i][0] = points[i + 1][0];
     points[i][1] = points[i + 1][1];
     points[i + 1][0] = tempX;
     points[i + 1][1] = tempY;
 }
 
 template <typename scalar_t>
-__device__ inline bool comparePoints(const Point<scalar_t>& p1, const Point<scalar_t>& p2, const Point<scalar_t>& centroid) {
+HOST_DEVICE inline bool comparePoints(const Point<scalar_t>& p1, const Point<scalar_t>& p2, const Point<scalar_t>& centroid) {
     scalar_t angle1 = computeAngle(centroid, p1);
     scalar_t angle2 = computeAngle(centroid, p2);
 
     if (fabs(angle1 - angle2) < EPSILON) {
         scalar_t dist1 = (p1.x - centroid.x) * (p1.x - centroid.x) +
                          (p1.y - centroid.y) * (p1.y - centroid.y);
         scalar_t dist2 = (p2.x - centroid.x) * (p2.x - centroid.x) +
@@ -73,15 +78,15 @@
         return dist1 < dist2;
     }
     return angle1 < angle2;
 }
 
 namespace sortPoints{
     template <typename scalar_t>
-    __device__ inline void sortQuadPointsClockwise(scalar_t *points) {
+    HOST_DEVICE inline void sortQuadPointsClockwise(scalar_t *points) {
         // Calculate the centroid of the points
         Point<scalar_t> centroid = findCentroid(points);
         
         bool swapped = true; // Initialize swapped to true to enter the loop
         int n = 4;
         while (swapped) {
             swapped = false; // Set swapped to false at the beginning of the loop
@@ -98,15 +103,15 @@
             }
             // Decrement n because the last element is now guaranteed to be in place
             --n;
         }
     }
 
     template <typename scalar_t>
-    __device__ inline void sortPointsClockwise(scalar_t points[MAX_ALL_POINTS][2]) {
+    HOST_DEVICE inline void sortPointsClockwise(scalar_t points[MAX_ALL_POINTS][2]) {
         // Calculate the centroid of the points
         Point<scalar_t> centroid = findCentroid(points);
         
         bool swapped = true; // Initialize swapped to true to enter the loop
         int n = MAX_ALL_POINTS;
         while (swapped) {
             swapped = false; // Set swapped to false at the beginning of the loop
@@ -124,8 +129,8 @@
                     swapped = true; // Indicate a swap occurred
                 }
             }
             // Decrement n because the last element is now guaranteed to be in place
             --n;
         }
     }
-}
+}
```

### Comparing `quad_iou-0.0.0/src/quad_iou/wrap.py` & `quad_iou-0.1.0/src/quad_iou/wrap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import torch
 from torch import Tensor
-from quad_iou_kernel import calculateIoU
+if torch.cuda.is_available():
+    from quad_iou_cuda import calculateIoUCuda
+from quad_iou_cpu import calculateIoUCPU
+
 
 def calculate_iou(quad_0: Tensor, quad_1: Tensor, sort_input_quads: bool = True) -> Tensor:
     """
     Calculates the Intersection over Union (IoU) between two sets of quadrilaterals.
 
     Parameters:
     - quad_0 (Tensor): A tensor of shape (M, 4, 2) representing the coordinates of M quadrilaterals. Each quadrilateral
@@ -17,8 +20,13 @@
     Returns:
     - Tensor: An (N, M) tensor where each element [i, j] is the IoU between the i-th quadrilateral from quad_1 and the
       j-th quadrilateral from quad_0.
 
     This function computes the IoU for each pair of quadrilaterals from the two input tensors and returns a matrix
     of these IoU values.
     """
-    return calculateIoU(quad_0, quad_1, sort_input_quads)
+    if quad_0.device == quad_1.device:
+        if quad_0.device.type == "cpu":
+            return calculateIoUCPU(quad_0, quad_1, sort_input_quads)
+        elif quad_0.device.type == "cuda":
+            return calculateIoUCuda(quad_0, quad_1, sort_input_quads)
+    raise ValueError(f"Expected all tensors to be on the same device but got device {quad_0.device} for quad_0 and {quad_1.device} for quad_1")
```


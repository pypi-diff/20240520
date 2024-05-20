# Comparing `tmp/delaunay_triangulation_and_its_dual_2d-0.1.5.tar.gz` & `tmp/delaunay_triangulation_and_its_dual_2d-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delaunay_triangulation_and_its_dual_2d-0.1.5.tar", last modified: Thu May 16 11:26:35 2024, max compression
+gzip compressed data, was "delaunay_triangulation_and_its_dual_2d-0.1.6.tar", last modified: Mon May 20 01:47:58 2024, max compression
```

## Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5.tar` & `delaunay_triangulation_and_its_dual_2d-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.464269 delaunay_triangulation_and_its_dual_2d-0.1.5/
--rw-rw-rw-   0        0        0     3318 2024-05-05 03:33:40.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/.gitignore
--rw-rw-rw-   0        0        0     1086 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     6089 2024-05-16 11:26:35.464269 delaunay_triangulation_and_its_dual_2d-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4084 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.437375 delaunay_triangulation_and_its_dual_2d-0.1.5/assets/
--rw-rw-rw-   0        0        0    66443 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/assets/time_to_compute_voronoi_tessellation.png
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.446690 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/
--rw-rw-rw-   0        0        0       32 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/__init__.py
--rw-rw-rw-   0        0        0      427 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/_version.py
--rw-rw-rw-   0        0        0    22218 2024-05-16 11:01:21.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/delaunay.py
--rw-rw-rw-   0        0        0       58 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.457695 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/
--rw-rw-rw-   0        0        0      142 2024-05-09 13:57:34.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
--rw-rw-rw-   0        0        0     3912 2024-05-16 11:23:28.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
--rw-rw-rw-   0        0        0      220 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
--rw-rw-rw-   0        0        0     2758 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.458263 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/util/
--rw-rw-rw-   0        0        0       65 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/util/__init__.py
--rw-rw-rw-   0        0        0      865 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.463267 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/
--rw-rw-rw-   0        0        0     6089 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       39 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1319 2024-05-05 04:11:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 11:26:35.465267 delaunay_triangulation_and_its_dual_2d-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.434376 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.462268 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/
--rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/__init__.py
--rw-rw-rw-   0        0        0     2484 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/performance.py
--rw-rw-rw-   0        0        0      481 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/profiling.py
--rw-rw-rw-   0        0        0     6180 2024-05-05 03:48:22.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/test_all.py
--rw-rw-rw-   0        0        0     3478 2024-05-16 11:22:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/try.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.462268 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/geometry/
--rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/geometry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.759478 delaunay_triangulation_and_its_dual_2d-0.1.6/
+-rw-rw-rw-   0        0        0     3318 2024-05-05 03:33:40.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/.gitignore
+-rw-rw-rw-   0        0        0     1086 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     6089 2024-05-20 01:47:58.758474 delaunay_triangulation_and_its_dual_2d-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4084 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.694251 delaunay_triangulation_and_its_dual_2d-0.1.6/assets/
+-rw-rw-rw-   0        0        0    66443 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/assets/time_to_compute_voronoi_tessellation.png
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.706914 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/
+-rw-rw-rw-   0        0        0       32 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-05-20 01:47:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/_version.py
+-rw-rw-rw-   0        0        0    22253 2024-05-20 01:43:37.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/delaunay.py
+-rw-rw-rw-   0        0        0       58 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.733965 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/geometry/
+-rw-rw-rw-   0        0        0      142 2024-05-09 13:57:34.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
+-rw-rw-rw-   0        0        0     4319 2024-05-20 01:46:02.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
+-rw-rw-rw-   0        0        0      220 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
+-rw-rw-rw-   0        0        0     2758 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.743969 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/util/
+-rw-rw-rw-   0        0        0       65 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/util/__init__.py
+-rw-rw-rw-   0        0        0      865 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.756970 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d.egg-info/
+-rw-rw-rw-   0        0        0     6089 2024-05-20 01:47:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2024-05-20 01:47:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 01:47:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-20 01:47:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2024-05-20 01:47:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1319 2024-05-05 04:11:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 01:47:58.759478 delaunay_triangulation_and_its_dual_2d-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.691252 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.755971 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/delaunay/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/delaunay/__init__.py
+-rw-rw-rw-   0        0        0     2484 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/delaunay/performance.py
+-rw-rw-rw-   0        0        0      481 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/delaunay/profiling.py
+-rw-rw-rw-   0        0        0     6180 2024-05-05 03:48:22.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/delaunay/test_all.py
+-rw-rw-rw-   0        0        0     5227 2024-05-20 01:46:11.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/delaunay/try.py
+drwxrwxrwx   0        0        0        0 2024-05-20 01:47:58.756970 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/geometry/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.6/tests/geometry/__init__.py
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/.gitignore` & `delaunay_triangulation_and_its_dual_2d-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/LICENSE` & `delaunay_triangulation_and_its_dual_2d-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/PKG-INFO` & `delaunay_triangulation_and_its_dual_2d-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-triangulation-and-its-dual-2d
-Version: 0.1.5
+Version: 0.1.6
 License: MIT License
         
         Copyright (c) 2024 M.H. Luk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/README.md` & `delaunay_triangulation_and_its_dual_2d-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/assets/time_to_compute_voronoi_tessellation.png` & `delaunay_triangulation_and_its_dual_2d-0.1.6/assets/time_to_compute_voronoi_tessellation.png`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/delaunay.py` & `delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/delaunay.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,18 @@
             new_points, a_min=bounding_box.min_, a_max=bounding_box.max_
         )
         return new_points
 
 
 class Delaunay(Base):
     def __init__(
-        self, *, points: NDArray[np.float_], bounding_box: BoundingBox2d | None
+        self,
+        *,
+        points: NDArray[np.float_],
+        bounding_box: BoundingBox2d | None = None,
     ) -> None:
         super().__init__(points=points, bounding_box=bounding_box)
 
         self.compute_delaunay_triangulation()
 
     def _compute_ridges_and_regions(self) -> None:
         if self._ridges_and_regions_computed:
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py` & `delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,19 @@
         return BoundingBox2d(
             min_=self.min_ - dilation, max_=self.max_ + dilation
         )
 
     def liang_barsky_line_clipping(
         self, line_segments: NDArray[np.float_]
     ) -> NDArray[np.float_]:
+        """
+
+        References:
+            - Liang-Barsky Algorithm. [link](https://www.geeksforgeeks.org/liang-barsky-algorithm/)
+        """
         x1, y1 = line_segments[:, 0].T
         x2, y2 = line_segments[:, 1].T
         dx = x2 - x1
         dy = y2 - y1
         p = np.stack([-dx, dx, -dy, dy], dtype=np.float_)
         q = np.stack(
             [
@@ -93,18 +98,29 @@
         for i in range(4):
             is_parallel = np.isclose(p[i], 0)
             outside_parallel = np.logical_and(is_parallel, q[i] < 0)
             t_enter[outside_parallel] = np.nan
             t_exit[outside_parallel] = np.nan
             # To avoid RuntimeWarning: divide by zero encountered in divide
             t = np.divide(
-                q[i], p[i], out=np.full_like(q[i], np.inf), where=~is_parallel
+                q[i],
+                p[i],
+                out=np.full_like(q[i], fill_value=np.inf),
+                where=~is_parallel,
+            )
+            t_enter = np.where(
+                np.logical_and(~is_parallel, p[i] < 0),
+                np.maximum(t_enter, t),
+                t_enter,
+            )
+            t_exit = np.where(
+                np.logical_and(~is_parallel, p[i] > 0),
+                np.minimum(t_exit, t),
+                t_exit,
             )
-            t_enter = np.where(p[i] < 0, np.maximum(t_enter, t), t_enter)
-            t_exit = np.where(p[i] > 0, np.minimum(t_exit, t), t_exit)
 
         outside = np.logical_or(np.isnan(t_enter), t_enter > t_exit)
         x1_clip = np.where(~outside, x1 + t_enter * dx, np.nan)
         y1_clip = np.where(~outside, y1 + t_enter * dy, np.nan)
         x2_clip = np.where(~outside, x1 + t_exit * dx, np.nan)
         y2_clip = np.where(~outside, y1 + t_exit * dy, np.nan)
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py` & `delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py` & `delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO` & `delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-triangulation-and-its-dual-2d
-Version: 0.1.5
+Version: 0.1.6
 License: MIT License
         
         Copyright (c) 2024 M.H. Luk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt` & `delaunay_triangulation_and_its_dual_2d-0.1.6/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/pyproject.toml` & `delaunay_triangulation_and_its_dual_2d-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/performance.py` & `delaunay_triangulation_and_its_dual_2d-0.1.6/tests/delaunay/performance.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/test_all.py` & `delaunay_triangulation_and_its_dual_2d-0.1.6/tests/delaunay/test_all.py`

 * *Files identical despite different names*


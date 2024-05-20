# Comparing `tmp/skytek_generic_map_api-0.9.1.tar.gz` & `tmp/skytek_generic_map_api-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytek_generic_map_api-0.9.1.tar", last modified: Tue Apr 23 18:43:16 2024, max compression
+gzip compressed data, was "skytek_generic_map_api-0.9.2.tar", last modified: Mon May 20 18:18:18 2024, max compression
```

## Comparing `skytek_generic_map_api-0.9.1.tar` & `skytek_generic_map_api-0.9.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.628788 skytek_generic_map_api-0.9.1/generic_map_api/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:43:14.000000 skytek_generic_map_api-0.9.1/generic_map_api/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/date_line_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/geometry_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/generic_map_api/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/resources/empty_tile.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default-features.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default-tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default.png
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/values.py
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:18.573464 skytek_generic_map_api-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-20 18:18:18.573464 skytek_generic_map_api-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:18.569464 skytek_generic_map_api-0.9.2/generic_map_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 18:18:16.000000 skytek_generic_map_api-0.9.2/generic_map_api/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/date_line_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/geometry_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:18.569464 skytek_generic_map_api-0.9.2/generic_map_api/multi_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/multi_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/multi_meta/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/multi_meta/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:18.569464 skytek_generic_map_api-0.9.2/generic_map_api/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/resources/empty_tile.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:18.569464 skytek_generic_map_api-0.9.2/generic_map_api/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/resources/icons/default-features.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/resources/icons/default-tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/resources/icons/default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/generic_map_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:18.569464 skytek_generic_map_api-0.9.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:18:18.573464 skytek_generic_map_api-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:18.573464 skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-20 18:18:18.000000 skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-20 18:18:18.000000 skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:18:18.000000 skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:18:18.000000 skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 18:18:18.000000 skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 18:18:18.000000 skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:18:18.573464 skytek_generic_map_api-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/tests/test_date_line_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-20 18:18:15.000000 skytek_generic_map_api-0.9.2/tests/test_values.py
```

### Comparing `skytek_generic_map_api-0.9.1/LICENSE` & `skytek_generic_map_api-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/PKG-INFO` & `skytek_generic_map_api-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-generic-map-api
-Version: 0.9.1
+Version: 0.9.2
 Summary: skytek-generic-map-api - expose geographical data for Skytek's frontends
 Home-page: http://github.com/Skytek/generic-map-api
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/bounding_box.py` & `skytek_generic_map_api-0.9.2/generic_map_api/bounding_box.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/clustering.py` & `skytek_generic_map_api-0.9.2/generic_map_api/clustering.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/date_line_normalization.py` & `skytek_generic_map_api-0.9.2/generic_map_api/date_line_normalization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from itertools import pairwise
-from typing import Generator, Iterable, Tuple
+from typing import Generator, Iterable, Tuple, Union
 
-from shapely.geometry import Polygon, box
+from shapely.geometry import MultiPolygon, Polygon, box
 
 
 def normalize_line(
     line: Iterable[Tuple[float, float]]
 ) -> Generator[Tuple[float, float], None, None]:
     """Fixes date line crossing problem for a line
 
@@ -50,14 +50,43 @@
         # line
         return tuple(normalize_line(geometry))
 
     # higher dimension object (polygon, multipolygon, etc.)
     return tuple(normalize_geometry(subgeom) for subgeom in geometry)
 
 
+def _normalize_longitudes(longitudes: Tuple[float, float]) -> Tuple[float, float]:
+    left_x, right_x = longitudes
+
+    while left_x < -180:
+        left_x += 360
+        right_x += 360
+
+    while left_x > 180:
+        left_x -= 360
+        right_x -= 360
+
+    return left_x, right_x
+
+
 def normalized_viewport(
     upper_left_x: float,
     upper_left_y: float,
     lower_right_x: float,
     lower_right_y: float,
-) -> Polygon:
-    return box(upper_left_x, upper_left_y, lower_right_x, lower_right_y)
+) -> Union[Polygon, MultiPolygon]:
+    longitude_span = lower_right_x - upper_left_x
+
+    if longitude_span >= 360:
+        return box(-180, upper_left_y, 180, lower_right_y)
+
+    upper_left_x, lower_right_x = _normalize_longitudes((upper_left_x, lower_right_x))
+
+    if upper_left_x <= lower_right_x:
+        return box(upper_left_x, upper_left_y, lower_right_x, lower_right_y)
+
+    return MultiPolygon(
+        [
+            box(lower_right_x, lower_right_y, -180, upper_left_y),
+            box(180, lower_right_y, upper_left_x, upper_left_y),
+        ]
+    )
```

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/geometry_serializers.py` & `skytek_generic_map_api-0.9.2/generic_map_api/geometry_serializers.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/views.py` & `skytek_generic_map_api-0.9.2/generic_map_api/multi_meta/views.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/params.py` & `skytek_generic_map_api-0.9.2/generic_map_api/params.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/resources/empty_tile.png` & `skytek_generic_map_api-0.9.2/generic_map_api/resources/empty_tile.png`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default-features.png` & `skytek_generic_map_api-0.9.2/generic_map_api/resources/icons/default-features.png`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default-tiles.png` & `skytek_generic_map_api-0.9.2/generic_map_api/resources/icons/default-tiles.png`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default.png` & `skytek_generic_map_api-0.9.2/generic_map_api/resources/icons/default.png`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/routers.py` & `skytek_generic_map_api-0.9.2/generic_map_api/routers.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/serializers.py` & `skytek_generic_map_api-0.9.2/generic_map_api/serializers.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/values.py` & `skytek_generic_map_api-0.9.2/generic_map_api/values.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass
-from typing import Any
+from typing import Any, Union
 
 import geohash2
 from shapely import set_srid
-from shapely.geometry import Point, Polygon
+from shapely.geometry import MultiPolygon, Point, Polygon
 from skytek_utils.spatial import tiles
 
 from .constants import WGS84
 from .date_line_normalization import normalized_viewport
 
 
 class BaseViewPort:
@@ -40,15 +40,15 @@
 
 class ViewPort(BaseViewPort):
     def __init__(self, upper_left, lower_right) -> None:
         super().__init__()
         self.upper_left = upper_left
         self.lower_right = lower_right
 
-    def to_polygon(self) -> Polygon:
+    def to_polygon(self) -> Union[Polygon | MultiPolygon]:
         return set_srid(
             normalized_viewport(
                 self.upper_left.x,
                 self.upper_left.y,
                 self.lower_right.x,
                 self.lower_right.y,
             ),
@@ -87,15 +87,15 @@
 class Tile(BaseViewPort):
     def __init__(self, x: int, y: int, z: int) -> None:
         super().__init__()
         self.x = x
         self.y = y
         self.z = z
 
-    def to_polygon(self) -> Polygon:
+    def to_polygon(self) -> Union[Polygon, MultiPolygon]:
         upper_left_x, upper_left_y = tiles.tile2deg(
             self.x,
             self.y,
             self.z,
         )
         lower_right_x, lower_right_y = tiles.tile2deg(
             self.x + 1,
```

### Comparing `skytek_generic_map_api-0.9.1/generic_map_api/views.py` & `skytek_generic_map_api-0.9.2/generic_map_api/views.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/setup.py` & `skytek_generic_map_api-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/PKG-INFO` & `skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-generic-map-api
-Version: 0.9.1
+Version: 0.9.2
 Summary: skytek-generic-map-api - expose geographical data for Skytek's frontends
 Home-page: http://github.com/Skytek/generic-map-api
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/SOURCES.txt` & `skytek_generic_map_api-0.9.2/skytek_generic_map_api.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 requirements/tests.txt
 skytek_generic_map_api.egg-info/PKG-INFO
 skytek_generic_map_api.egg-info/SOURCES.txt
 skytek_generic_map_api.egg-info/dependency_links.txt
 skytek_generic_map_api.egg-info/not-zip-safe
 skytek_generic_map_api.egg-info/requires.txt
 skytek_generic_map_api.egg-info/top_level.txt
+tests/test_date_line_normalization.py
 tests/test_values.py
```


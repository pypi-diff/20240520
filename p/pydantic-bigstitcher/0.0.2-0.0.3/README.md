# Comparing `tmp/pydantic_bigstitcher-0.0.2.tar.gz` & `tmp/pydantic_bigstitcher-0.0.3.tar.gz`

## Comparing `pydantic_bigstitcher-0.0.2.tar` & `pydantic_bigstitcher-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/src/pydantic_bigstitcher/__about__.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/src/pydantic_bigstitcher/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0    30091 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/tests/test_models.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/README.md
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/src/pydantic_bigstitcher/__about__.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/src/pydantic_bigstitcher/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    30091 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/tests/test_models.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/README.md
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 pydantic_bigstitcher-0.0.3/PKG-INFO
```

### Comparing `pydantic_bigstitcher-0.0.2/src/pydantic_bigstitcher/__init__.py` & `pydantic_bigstitcher-0.0.3/src/pydantic_bigstitcher/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 class BasePath(BaseXmlModel):
     typ: Literal["relative", "absolute"] = attr(name="type")
 
 
 class ZGroup(BaseXmlModel, tag="zgroup"):
     setup: str = attr()
     timepoint: str = attr()
-    path: str = element()
+    path: str | None = element(default=None)
 
 
 class ZGroups(BaseXmlModel, tag="zgroups"):
     zgroups: list[ZGroup] = element(tag="zgroup")
 
 
 class Zarr(BaseXmlModel, tag="zarr"):
     typ: str = attr(name="type")
 
 
 class ZarrImageLoader(BaseXmlModel, tag="ImageLoader"):
     fmt: str = attr(name="format")
     version: str = attr()
+    s3bucket: str | None = element(default=None)
     zarr: Zarr = element(tag="zarr")
-    zgroups: ZGroups
+    zgroups: ZGroups = element(tag="zgroups")
 
 
 class VoxelSize(BaseXmlModel):
     unit: str = element()
     size: str = element()
 
 
@@ -134,11 +135,11 @@
 class SpimData2(SpimData, tag="SpimData"):
     """
     https://github.com/PreibischLab/multiview-reconstruction/blob/master/src/main/java/net/preibisch/mvrecon/fiji/spimdata/SpimData2.java#L64
     """
 
     view_interest_points: ViewInterestPoints = element(tag='ViewInterestPoints')
     bounding_boxes: BoundingBoxes = element(tag='BoundingBoxes')
-#    point_spread_functions: PointSpreadFunctions
-#    stitching_results: StitchingResults
-#    intensity_adjustments: IntensityAdjustments 
+    # point_spread_functions: PointSpreadFunctions
+    # stitching_results: StitchingResults
+    # intensity_adjustments: IntensityAdjustments
```

### Comparing `pydantic_bigstitcher-0.0.2/tests/conftest.py` & `pydantic_bigstitcher-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic_bigstitcher-0.0.2/LICENSE.txt` & `pydantic_bigstitcher-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydantic_bigstitcher-0.0.2/README.md` & `pydantic_bigstitcher-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_bigstitcher-0.0.2/pyproject.toml` & `pydantic_bigstitcher-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic_bigstitcher-0.0.2/PKG-INFO` & `pydantic_bigstitcher-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydantic-bigstitcher
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/unknown/pydantic-bigstitcher#readme
 Project-URL: Issues, https://github.com/unknown/pydantic-bigstitcher/issues
 Project-URL: Source, https://github.com/unknown/pydantic-bigstitcher
 Author-email: Davis Vann Bennett <davis.v.bennett@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```


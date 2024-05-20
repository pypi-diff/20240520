# Comparing `tmp/pygmtsar-2024.4.17.post6.tar.gz` & `tmp/pygmtsar-2024.4.17.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.4.17.post6.tar", last modified: Sat May 18 17:40:53 2024, max compression
+gzip compressed data, was "pygmtsar-2024.4.17.post8.tar", last modified: Mon May 20 14:18:12 2024, max compression
```

## Comparing `pygmtsar-2024.4.17.post6.tar` & `pygmtsar-2024.4.17.post8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-18 17:40:53.692665 pygmtsar-2024.4.17.post6/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post6/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-18 17:40:53.692345 pygmtsar-2024.4.17.post6/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post6/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-18 17:40:53.690543 pygmtsar-2024.4.17.post6/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post6/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post6/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post6/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post6/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post6/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post6/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post6/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post6/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44539 2024-05-08 11:23:30.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    47608 2024-05-07 07:53:29.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    46915 2024-05-13 12:07:20.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     9599 2024-05-15 06:53:05.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post6/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post6/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)    10511 2024-05-18 08:33:45.000000 pygmtsar-2024.4.17.post6/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post6/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-05-18 17:40:10.000000 pygmtsar-2024.4.17.post6/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post6/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post6/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post6/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post6/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-18 17:40:53.691951 pygmtsar-2024.4.17.post6/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-18 17:40:53.000000 pygmtsar-2024.4.17.post6/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-05-18 17:40:53.000000 pygmtsar-2024.4.17.post6/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-05-18 17:40:53.000000 pygmtsar-2024.4.17.post6/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-05-18 17:40:53.000000 pygmtsar-2024.4.17.post6/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-05-18 17:40:53.000000 pygmtsar-2024.4.17.post6/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-05-18 17:40:53.692724 pygmtsar-2024.4.17.post6/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17.post6/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-20 14:18:12.627515 pygmtsar-2024.4.17.post8/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post8/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-20 14:18:12.624869 pygmtsar-2024.4.17.post8/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post8/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-20 14:18:12.618288 pygmtsar-2024.4.17.post8/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post8/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post8/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post8/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post8/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post8/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post8/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post8/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post8/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5706 2024-05-19 15:27:12.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44539 2024-05-08 11:23:30.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47608 2024-05-07 07:53:29.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    48188 2024-05-20 08:24:15.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9599 2024-05-15 06:53:05.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post8/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10511 2024-05-18 08:33:45.000000 pygmtsar-2024.4.17.post8/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post8/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-05-20 08:15:48.000000 pygmtsar-2024.4.17.post8/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post8/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post8/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post8/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post8/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-20 14:18:12.624554 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-05-20 14:18:12.627570 pygmtsar-2024.4.17.post8/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-05-20 06:11:34.000000 pygmtsar-2024.4.17.post8/setup.py
```

### Comparing `pygmtsar-2024.4.17.post6/LICENSE.txt` & `pygmtsar-2024.4.17.post8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/PKG-INFO` & `pygmtsar-2024.4.17.post8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post6
+Version: 2024.4.17.post8
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,15 +21,15 @@
 Requires-Dist: xarray>=2024.1.0
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: numba
 Requires-Dist: pandas>=2.2
 Requires-Dist: geopandas
 Requires-Dist: distributed>=2024.1.0
 Requires-Dist: dask[complete]>=2024.4.1
-Requires-Dist: dask_image
+Requires-Dist: dask-image
 Requires-Dist: joblib
 Requires-Dist: tqdm
 Requires-Dist: scipy==1.11.4
 Requires-Dist: cffi
 Requires-Dist: shapely>=2.0.2
 Requires-Dist: scikit-learn
 Requires-Dist: xmltodict
```

### Comparing `pygmtsar-2024.4.17.post6/README.md` & `pygmtsar-2024.4.17.post8/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/ASF.py` & `pygmtsar-2024.4.17.post8/pygmtsar/ASF.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/AWS.py` & `pygmtsar-2024.4.17.post8/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/GMT.py` & `pygmtsar-2024.4.17.post8/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/IO.py` & `pygmtsar-2024.4.17.post8/pygmtsar/IO.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.4.17.post8/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/PRM.py` & `pygmtsar-2024.4.17.post8/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.4.17.post8/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/S1.py` & `pygmtsar-2024.4.17.post8/pygmtsar/S1.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack.py`

 * *Files 10% similar despite different names*

```diff
@@ -111,31 +111,33 @@
             marker_size = kwargs['marker_size']
         if 'marker_color' not in kwargs:
             marker_color = 'red'
         else:
             marker_color = kwargs['marker_color']
         geometry.plot(ax=plt.gca(), marker=marker, markersize=marker_size, color=marker_color)
 
-    def plot_scenes(self, dem='auto', caption='Estimated Scene Locations', cmap='turbo', aspect=None, **kwargs):
+    def plot_scenes(self, dem='auto', image=None, alpha=None, caption='Estimated Scene Locations', cmap='turbo', aspect=None, **kwargs):
         import matplotlib.pyplot as plt
         import matplotlib
 
         plt.figure()
+        if image is not None:
+            image.plot.imshow(cmap='gray', alpha=alpha, add_colorbar=False)
         if isinstance(dem, str) and dem == 'auto':
             if self.dem_filename is not None:
                 dem = self.get_dem()
                 # TODO: check shape and decimate large grids
                 dem.plot.imshow(cmap='gray', add_colorbar=False)
         elif dem is not None:
             dem.plot.imshow(cmap='gray', add_colorbar=False)
         gdf = self.to_dataframe()
         cmap = matplotlib.colormaps[cmap]
         colors = dict([(v, cmap(k)) for k, v in enumerate(gdf.index.unique())])
         # too small an alpha becomes invisible
-        alpha = 0.5/len(gdf)
-        alpha = alpha if alpha>=0.002 else 0.002
-        gdf.reset_index().plot(color=[colors[k] for k in gdf.index], alpha=alpha, edgecolor='black', ax=plt.gca())
+        gdf_alpha = 0.5/len(gdf)
+        gdf_alpha = gdf_alpha if gdf_alpha>=0.002 else 0.002
+        gdf.reset_index().plot(color=[colors[k] for k in gdf.index], alpha=gdf_alpha, edgecolor='black', ax=plt.gca())
         self.plot_AOI(**kwargs)
         self.plot_POI(**kwargs)
         if aspect is not None:
             plt.gca().set_aspect(aspect)
         plt.title(caption)
```

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_align.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_base.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_dem.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_export.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_phasediff.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_prm.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_ps.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_ps.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_sbas.py`

 * *Files 2% similar despite different names*

```diff
@@ -666,26 +666,26 @@
             counts, edges = np.histogram(baseline_pairs.duration, bins=bins)
             sums, _ = np.histogram(baseline_pairs.duration, bins=bins, weights=baseline_pairs[column])
             averages = sums / counts
 
             # Normalize the average values for coloring
             norm = mcolors.Normalize(vmin=vmin if vmin is not None else np.nanmin(averages),
                                      vmax=vmax if vmax is not None else np.nanmax(averages))
-            cmap = plt.cm.get_cmap(cmap)
+            cmap = plt.colormaps[cmap]
 
             for i in range(len(bin_midpoints)):
                 bin_color = 'white' if np.isnan(averages[i]) else cmap(norm(averages[i]))
                 ax.bar(bin_midpoints[i], counts[i], width=bins[i+1] - bins[i], color=bin_color,
                        edgecolor='black', align='center', zorder=3)
 
             plt.colorbar(plt.cm.ScalarMappable(norm=norm, cmap=cmap), ax=ax, label=f'Average {column}')
         elif column is not None:
             norm = mcolors.Normalize(vmin=vmin if vmin is not None else baseline_pairs[column].min(),
                                      vmax=vmax if vmax is not None else baseline_pairs[column].max())
-            cmap = plt.cm.get_cmap(cmap)
+            cmap = plt.colormaps[cmap]
 
             for i in range(len(bins) - 1):
                 bin_data = baseline_pairs[(baseline_pairs.duration >= bins[i]) & (baseline_pairs.duration < bins[i + 1])]
                 bin_data = bin_data.sort_values(by=column, ascending=ascending)
                 #print (i, bin_data[column].mean())
 
                 bottom = 0
@@ -748,15 +748,15 @@
         #print ('NOTE: this function is deprecated, use instead Stack.plot_baseline_attribute()')
         self.plot_baseline_attribute(baseline_pairs, pairs_best, column=column, caption='Baseline Correlation')
 
     def plot_baseline_deviation(self, baseline_pairs, pairs_best=None, column='stddev'):
         #print ('NOTE: this function is deprecated, use instead Stack.plot_baseline_attribute()')
         self.plot_baseline_attribute(baseline_pairs, pairs_best, column=column, caption='Baseline Deviation')
 
-    def plot_baseline_displacement(self, phase, corr=None, caption=None, cmap='turbo',
+    def plot_baseline_displacement(self, phase, corr=None, caption='LSQ and STL Displacement Models, [rad]', cmap='turbo',
                                    displacement=True, unwrap=True,
                                    stl=False, stl_freq='W', stl_periods=52, stl_robust=True,
                                    los=False, tolerance=np.pi/2, xlabel_rotation=45,
                                    legend=True, legend_alpha=None, linewidth=0.5):
         """
         Performs 1D unwrapping, linear regression, and STL on a given set of phase values.
     
@@ -783,15 +783,15 @@
         from matplotlib.cm import ScalarMappable
     
         if not displacement and stl:
             print ("NOTE: Displacement is automatically set to 'True' because it is required for 'stl=True'.")
         assert isinstance(phase, xr.DataArray) and phase.dims == ('pair',), \
             'ERROR: Argument phase should be 1D Xarray with "pair" dimension'
         plt.figure()
-        colors = matplotlib.cm.get_cmap(cmap)
+        colors = plt.colormaps[cmap]
     
         df = phase.to_dataframe()
         df['corr'] = corr.values if corr is not None else 1
         pairs, dates = self.get_pairs(phase, dates=True)
         dates = pd.DatetimeIndex(dates)
         matrix = self.lstsq_matrix(pairs)
     
@@ -896,23 +896,21 @@
             sm.set_array([])
             cbar = plt.colorbar(sm, ax=plt.gca(), orientation='vertical')
             cbar.set_label('Correlation')
     
         plt.xticks(rotation=xlabel_rotation)
         plt.xlabel('Timeline')
         plt.ylabel(f'{name}, [{unit}]')
-        plt.title('Displacement' \
-                  + (f' RMSE={rmse:0.3f} [{unit}]' if displacement or stl else '') \
-                  + (f'\n{caption}' if caption is not None else ''))
+        plt.title(f'{caption}\n' + (f'RMSE={rmse:0.3f} [{unit}]' if displacement or stl else ''))
         plt.xlim([dates[0], dates[-1]])
         if (displacement or stl) and legend:
             plt.legend(framealpha=legend_alpha)
 
-    def plot_baseline_displacement_los_mm(self, phase, corr=None, caption=None, cmap='turbo',
-                                   displacement=True, unwrap=True,
+    def plot_baseline_displacement_los_mm(self, phase, corr=None, caption='LSQ and STL Displacement Models, [mm]',
+                                   cmap='turbo', displacement=True, unwrap=True,
                                    stl=False, stl_freq='W', stl_periods=52, stl_robust=True,
                                    tolerance=np.pi/2, xlabel_rotation=45,
                                    legend=True, legend_alpha=None, linewidth=0.5):
         self.plot_baseline_displacement(phase=phase, corr=corr, caption=caption, cmap=cmap,
                                    displacement=displacement, unwrap=unwrap,
                                    stl=stl, stl_freq=stl_freq, stl_periods=stl_periods, stl_robust=stl_robust,
                                    los=True, tolerance=tolerance, xlabel_rotation=xlabel_rotation,
@@ -991,15 +989,21 @@
             col_wrap=cols, size=size, aspect=aspect,
             vmin=vmin, vmax=vmax, cmap='turbo'
         )
         fg.set_axis_labels('Range', 'Azimuth')
         fg.set_ticks(max_xticks=nbins, max_yticks=nbins)
         fg.fig.suptitle(caption, y=y)
 
-    def plot_velocity(self, data, caption='Velocity, mm/year',
+    def plot_displacements_los_mm(self, data, caption='Cumulative LOS Displacement, [mm]', cols=4, size=4, nbins=5, aspect=1.2, y=1.05,
+                           quantile=None, vmin=None, vmax=None, symmetrical=False):
+        self.plot_displacements(self.los_displacement_mm(data),
+                                caption=caption, cols=cols, size=size, nbins=nbins, aspect=aspect, y=y,
+                                quantile=quantile, vmin=vmin, vmax=vmax, symmetrical=symmetrical)
+
+    def plot_velocity(self, data, caption='Velocity, [rad/year]',
                       quantile=None, vmin=None, vmax=None, symmetrical=False, aspect=None, alpha=1, **kwargs):
         import numpy as np
         import matplotlib.pyplot as plt
     
         if quantile is not None:
             assert vmin is None and vmax is None, "ERROR: arguments 'quantile' and 'vmin', 'vmax' cannot be used together"
     
@@ -1016,15 +1020,21 @@
         data.plot.imshow(vmin=vmin, vmax=vmax, alpha=alpha, cmap='turbo')
         self.plot_AOI(**kwargs)
         self.plot_POI(**kwargs)
         if aspect is not None:
             plt.gca().set_aspect(aspect)
         plt.title(caption)
 
-    def plot_rmse(self, rmse, caption='RMSE', cmap='turbo',
+    def plot_velocity_los_mm(self, data, caption='Velocity, [mm/year]',
+                      quantile=None, vmin=None, vmax=None, symmetrical=False, aspect=None, alpha=1, **kwargs):
+        self.plot_velocity(self.los_displacement_mm(data),
+                           caption=caption, aspect=aspect, alpha=alpha,
+                           quantile=quantile, vmin=vmin, vmax=vmax, symmetrical=symmetrical, **kwargs)
+                      
+    def plot_rmse(self, rmse, caption='RMSE, [rad]', cmap='turbo',
                   quantile=None, vmin=None, vmax=None, symmetrical=False, **kwargs):
         import numpy as np
         import matplotlib.pyplot as plt
         import warnings
         # suppress Dask warning "RuntimeWarning: invalid value encountered in divide"
         warnings.filterwarnings('ignore')
         warnings.filterwarnings('ignore', module='dask')
@@ -1043,7 +1053,13 @@
             vmax =  minmax
 
         plt.figure()
         rmse.plot.imshow(cmap=cmap, vmin=vmin, vmax=vmax)
         self.plot_AOI(**kwargs)
         self.plot_POI(**kwargs)
         plt.title(caption)
+
+    def plot_rmse_los_mm(self, rmse, caption='RMSE, [mm]', cmap='turbo',
+                  quantile=None, vmin=None, vmax=None, symmetrical=False, **kwargs):
+        self.plot_rmse(abs(self.los_displacement_mm(rmse)),
+                       caption=caption, cmap=cmap,
+                       quantile=quantile, vmin=vmin, vmax=vmax, symmetrical=symmetrical, **kwargs)
```

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_stl.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_stl.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_topo.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_trans.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_unwrap.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/Tiles.py` & `pygmtsar-2024.4.17.post8/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/XYZTiles.py` & `pygmtsar-2024.4.17.post8/pygmtsar/XYZTiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.4.17.post8/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/__init__.py` & `pygmtsar-2024.4.17.post8/pygmtsar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.4.17.post6'
+__version__ = '2024.4.17.post8'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
```

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/datagrid.py` & `pygmtsar-2024.4.17.post8/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.4.17.post8/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.4.17.post8/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar/utils.py` & `pygmtsar-2024.4.17.post8/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.4.17.post8/pygmtsar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post6
+Version: 2024.4.17.post8
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,15 +21,15 @@
 Requires-Dist: xarray>=2024.1.0
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: numba
 Requires-Dist: pandas>=2.2
 Requires-Dist: geopandas
 Requires-Dist: distributed>=2024.1.0
 Requires-Dist: dask[complete]>=2024.4.1
-Requires-Dist: dask_image
+Requires-Dist: dask-image
 Requires-Dist: joblib
 Requires-Dist: tqdm
 Requires-Dist: scipy==1.11.4
 Requires-Dist: cffi
 Requires-Dist: shapely>=2.0.2
 Requires-Dist: scikit-learn
 Requires-Dist: xmltodict
```

### Comparing `pygmtsar-2024.4.17.post6/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.4.17.post8/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post6/setup.py` & `pygmtsar-2024.4.17.post8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     install_requires=['xarray>=2024.1.0',
                       'numpy>=1.22.4',
                       'numba',
                       'pandas>=2.2',
                       'geopandas',
                       'distributed>=2024.1.0',
                       'dask[complete]>=2024.4.1',
-                      'dask_image',
+                      'dask-image',
                       'joblib',
                       'tqdm',
                       'scipy==1.11.4',
                       'cffi',
                       'shapely>=2.0.2',
                       'scikit-learn',
                       'xmltodict',
```


# Comparing `tmp/xarray-selafin-0.1.5.tar.gz` & `tmp/xarray_selafin-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-selafin-0.1.5.tar", last modified: Thu Mar 21 18:04:57 2024, max compression
+gzip compressed data, was "xarray_selafin-0.1.6.tar", max compression
```

## Comparing `xarray-selafin-0.1.5.tar` & `xarray_selafin-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,12 @@
-drwxrwxr-x   0 tomsail   (1000) tomsail   (1000)        0 2024-03-21 18:04:57.223353 xarray-selafin-0.1.5/
--rw-r--r--   0 tomsail   (1000) tomsail   (1000)     4033 2024-03-21 18:04:57.223353 xarray-selafin-0.1.5/PKG-INFO
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)     3542 2024-03-02 16:51:15.000000 xarray-selafin-0.1.5/README.md
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)      732 2024-03-21 17:58:26.000000 xarray-selafin-0.1.5/pyproject.toml
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)      714 2024-03-21 18:04:57.223353 xarray-selafin-0.1.5/setup.cfg
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)      867 2024-03-21 17:58:38.000000 xarray-selafin-0.1.5/setup.py
-drwxrwxr-x   0 tomsail   (1000) tomsail   (1000)        0 2024-03-21 18:04:57.219353 xarray-selafin-0.1.5/xarray_selafin/
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)    48794 2024-03-21 17:37:40.000000 xarray-selafin-0.1.5/xarray_selafin/Serafin.py
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)        0 2024-03-02 16:51:15.000000 xarray-selafin-0.1.5/xarray_selafin/__init__.py
-drwxrwxr-x   0 tomsail   (1000) tomsail   (1000)        0 2024-03-21 18:04:57.223353 xarray-selafin-0.1.5/xarray_selafin/data/
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)     2562 2024-03-02 16:51:15.000000 xarray-selafin-0.1.5/xarray_selafin/data/Serafin_var2D.csv
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)      790 2024-03-02 16:51:15.000000 xarray-selafin-0.1.5/xarray_selafin/data/Serafin_var3D.csv
-drwxrwxr-x   0 tomsail   (1000) tomsail   (1000)        0 2024-03-21 18:04:57.223353 xarray-selafin-0.1.5/xarray_selafin/variable/
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)        0 2024-03-02 16:51:15.000000 xarray-selafin-0.1.5/xarray_selafin/variable/__init__.py
--rwxrwxr-x   0 tomsail   (1000) tomsail   (1000)    12235 2024-03-02 16:51:15.000000 xarray-selafin-0.1.5/xarray_selafin/variable/variables_2d.py
--rwxrwxr-x   0 tomsail   (1000) tomsail   (1000)     2507 2024-03-02 16:51:15.000000 xarray-selafin-0.1.5/xarray_selafin/variable/variables_3d.py
--rwxrwxr-x   0 tomsail   (1000) tomsail   (1000)     5294 2024-03-02 16:51:15.000000 xarray-selafin-0.1.5/xarray_selafin/variable/variables_utils.py
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)    12221 2024-03-21 17:37:40.000000 xarray-selafin-0.1.5/xarray_selafin/xarray_backend.py
-drwxrwxr-x   0 tomsail   (1000) tomsail   (1000)        0 2024-03-21 18:04:57.223353 xarray-selafin-0.1.5/xarray_selafin.egg-info/
--rw-r--r--   0 tomsail   (1000) tomsail   (1000)     4033 2024-03-21 18:04:57.000000 xarray-selafin-0.1.5/xarray_selafin.egg-info/PKG-INFO
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)      594 2024-03-21 18:04:57.000000 xarray-selafin-0.1.5/xarray_selafin.egg-info/SOURCES.txt
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)        1 2024-03-21 18:04:57.000000 xarray-selafin-0.1.5/xarray_selafin.egg-info/dependency_links.txt
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)       83 2024-03-21 18:04:57.000000 xarray-selafin-0.1.5/xarray_selafin.egg-info/entry_points.txt
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)       73 2024-03-21 18:04:57.000000 xarray-selafin-0.1.5/xarray_selafin.egg-info/requires.txt
--rw-rw-r--   0 tomsail   (1000) tomsail   (1000)       15 2024-03-21 18:04:57.000000 xarray-selafin-0.1.5/xarray_selafin.egg-info/top_level.txt
+-rw-r--r--   0        0        0     3542 2024-03-02 16:51:15.115429 xarray_selafin-0.1.6/README.md
+-rw-r--r--   0        0        0      665 2024-05-20 15:28:47.409556 xarray_selafin-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    48794 2024-05-13 13:55:59.233751 xarray_selafin-0.1.6/xarray_selafin/Serafin.py
+-rw-r--r--   0        0        0        0 2024-03-02 16:51:15.123428 xarray_selafin-0.1.6/xarray_selafin/__init__.py
+-rw-r--r--   0        0        0     2562 2024-03-02 16:51:15.123428 xarray_selafin-0.1.6/xarray_selafin/data/Serafin_var2D.csv
+-rw-r--r--   0        0        0      790 2024-03-02 16:51:15.127427 xarray_selafin-0.1.6/xarray_selafin/data/Serafin_var3D.csv
+-rw-r--r--   0        0        0        0 2024-03-02 16:51:15.127427 xarray_selafin-0.1.6/xarray_selafin/variable/__init__.py
+-rwxr-xr-x   0        0        0    12235 2024-03-02 16:51:15.127427 xarray_selafin-0.1.6/xarray_selafin/variable/variables_2d.py
+-rwxr-xr-x   0        0        0     2507 2024-03-02 16:51:15.127427 xarray_selafin-0.1.6/xarray_selafin/variable/variables_3d.py
+-rwxr-xr-x   0        0        0     5294 2024-03-02 16:51:15.127427 xarray_selafin-0.1.6/xarray_selafin/variable/variables_utils.py
+-rw-r--r--   0        0        0    12221 2024-05-13 13:55:32.190393 xarray_selafin-0.1.6/xarray_selafin/xarray_backend.py
+-rw-r--r--   0        0        0     4218 1970-01-01 00:00:00.000000 xarray_selafin-0.1.6/PKG-INFO
```

### Comparing `xarray-selafin-0.1.5/PKG-INFO` & `xarray_selafin-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: xarray-selafin
-Version: 0.1.5
-Summary: https://github.com/seareport/xarray-selafin
-Author: ['tomsail', 'lucduron']
-Author-email: l.duron@cnr.tm.fr
+Version: 0.1.6
+Summary: 
+Home-page: https://github.com/seareport/xarray-selafin/
+Author: tomsail
+Author-email: saillour.thomas@gmail.com
 Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: netcdf4
 Requires-Dist: numpy
-Requires-Dist: pytest
 Requires-Dist: scipy
 Requires-Dist: shapely
 Requires-Dist: xarray
-Requires-Dist: netcdf4
-Provides-Extra: dask
-Requires-Dist: dask; extra == "dask"
-Provides-Extra: dev
-Requires-Dist: matplotlib; extra == "dev"
+Project-URL: Repository, https://github.com/seareport/xarray-selafin/
+Description-Content-Type: text/markdown
 
 # xarray backend for Selafin formats
 
 Supports lazy loading by default.
 
 ## Dev guide
 
@@ -110,7 +112,8 @@
 | float_size | Float size                                                              | 4 (single precision)     |
 | endian     | File endianness                                                         | ">"                      |
 | params     | Table of integer parameters                                             | (can be rebuilt)         |
 | ikle2      | Connectivity table in 2D (1-indexed)                                    | -                        |
 | ikle3      | Connectivity table in 3D (1-indexed, only in 3D, optional)              | (can be rebuilt from 2D) |
 | variables  | Dictionary with variable names and units (key is variable abbreviation) | -                        |
 | date_start | Starting date with integers (year to seconds)                           | (from first time serie)  |
+
```

### Comparing `xarray-selafin-0.1.5/README.md` & `xarray_selafin-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `xarray-selafin-0.1.5/pyproject.toml` & `xarray_selafin-0.1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 [tool.poetry]
 name = "xarray-selafin"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["tomsail <saillour.thomas@gmail.com>", "lucduron <l.duron@cnr.tm.fr>"]
 readme = "README.md"
 repository = "https://github.com/seareport/xarray-selafin/"
 include = [
     "xarray_selafin/data/*",
     "xarray_selafin/variable/*"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 numpy = "*"
-pytest = "*"
 scipy = "*"
 shapely = "*"
 xarray = "*"
 netcdf4 = "*"
 
-[tool.poetry.group.dask.dependencies]
-dask = "*"
-
 [tool.poetry.plugins."xarray.backends"]
 selafin = "xarray_selafin.xarray_backend:SelafinBackendEntrypoint"
 
 [tool.poetry.group.dev.dependencies]
-matplotlib = "*"
+pytest = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xarray-selafin-0.1.5/xarray_selafin/Serafin.py` & `xarray_selafin-0.1.6/xarray_selafin/Serafin.py`

 * *Files identical despite different names*

### Comparing `xarray-selafin-0.1.5/xarray_selafin/data/Serafin_var2D.csv` & `xarray_selafin-0.1.6/xarray_selafin/data/Serafin_var2D.csv`

 * *Files identical despite different names*

### Comparing `xarray-selafin-0.1.5/xarray_selafin/data/Serafin_var3D.csv` & `xarray_selafin-0.1.6/xarray_selafin/data/Serafin_var3D.csv`

 * *Files identical despite different names*

### Comparing `xarray-selafin-0.1.5/xarray_selafin/variable/variables_2d.py` & `xarray_selafin-0.1.6/xarray_selafin/variable/variables_2d.py`

 * *Files identical despite different names*

### Comparing `xarray-selafin-0.1.5/xarray_selafin/variable/variables_3d.py` & `xarray_selafin-0.1.6/xarray_selafin/variable/variables_3d.py`

 * *Files identical despite different names*

### Comparing `xarray-selafin-0.1.5/xarray_selafin/variable/variables_utils.py` & `xarray_selafin-0.1.6/xarray_selafin/variable/variables_utils.py`

 * *Files identical despite different names*

### Comparing `xarray-selafin-0.1.5/xarray_selafin/xarray_backend.py` & `xarray_selafin-0.1.6/xarray_selafin/xarray_backend.py`

 * *Files identical despite different names*


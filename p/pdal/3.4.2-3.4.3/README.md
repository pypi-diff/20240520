# Comparing `tmp/pdal-3.4.2.tar.gz` & `tmp/pdal-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdal-3.4.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pdal-3.4.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pdal-3.4.2.tar` & `pdal-3.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 pdal-3.4.2/.gitignore
--rw-r--r--   0        0        0     3724 2022-11-09 12:37:21.000000 pdal-3.4.2/CHANGES.txt
--rw-r--r--   0        0        0     1385 2022-11-09 12:37:21.000000 pdal-3.4.2/CMakeLists.txt
--rw-r--r--   0        0        0     1898 2022-11-09 12:37:21.000000 pdal-3.4.2/LICENSE.txt
--rw-r--r--   0        0        0    12093 2022-11-09 12:37:21.000000 pdal-3.4.2/README.rst
--rw-r--r--   0        0        0     1660 2022-11-09 12:37:21.000000 pdal-3.4.2/pyproject.toml
--rw-r--r--   0        0        0     1467 2022-11-09 12:37:21.000000 pdal-3.4.2/setup.py.off
--rw-r--r--   0        0        0     6228 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/PyArray.cpp
--rw-r--r--   0        0        0     3283 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/PyArray.hpp
--rw-r--r--   0        0        0     3219 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/PyDimension.hpp
--rw-r--r--   0        0        0    11691 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/PyPipeline.cpp
--rw-r--r--   0        0        0     3486 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/PyPipeline.hpp
--rw-r--r--   0        0        0     6947 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/StreamableExecutor.cpp
--rw-r--r--   0        0        0     3294 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/StreamableExecutor.hpp
--rw-r--r--   0        0        0      375 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/__init__.py
--rw-r--r--   0        0        0     2130 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/__main__.py
--rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/drivers.py
--rw-r--r--   0        0        0    11626 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/libpdalpython.cpp
--rw-r--r--   0        0        0     8308 2022-11-09 12:37:21.000000 pdal-3.4.2/src/pdal/pipeline.py
--rw-r--r--   0        0        0    36439 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/1.2-with-color.las
--rw-r--r--   0        0        0    37417 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/autzen-utm.las
--rw-r--r--   0        0        0      111 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/bad.json
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/bad.py
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/chip.json
--rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/chip.py
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/mesh.json
--rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/mesh.py
--rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/range.json
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/range.py
--rw-r--r--   0        0        0      724 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/reproject.json
--rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/reproject.py
--rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/sort.json
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/sort.py
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 pdal-3.4.2/test/data/test3d.npy
--rw-r--r--   0        0        0    22155 2022-11-09 12:37:21.000000 pdal-3.4.2/test/test_pipeline.py
--rw-r--r--   0        0        0    15489 2022-11-09 12:37:21.000000 pdal-3.4.2/PKG-INFO
+-rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 pdal-3.4.3/.gitignore
+-rw-r--r--   0        0        0     3724 2022-11-09 12:37:21.000000 pdal-3.4.3/CHANGES.txt
+-rw-r--r--   0        0        0     1385 2022-11-09 12:37:21.000000 pdal-3.4.3/CMakeLists.txt
+-rw-r--r--   0        0        0     1898 2022-11-09 12:37:21.000000 pdal-3.4.3/LICENSE.txt
+-rw-r--r--   0        0        0    12093 2022-11-09 12:37:21.000000 pdal-3.4.3/README.rst
+-rw-r--r--   0        0        0     1660 2022-11-09 12:37:21.000000 pdal-3.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1467 2022-11-09 12:37:21.000000 pdal-3.4.3/setup.py.off
+-rw-r--r--   0        0        0     6228 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/PyArray.cpp
+-rw-r--r--   0        0        0     3283 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/PyArray.hpp
+-rw-r--r--   0        0        0     3219 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/PyDimension.hpp
+-rw-r--r--   0        0        0    11691 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/PyPipeline.cpp
+-rw-r--r--   0        0        0     3486 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/PyPipeline.hpp
+-rw-r--r--   0        0        0     6947 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/StreamableExecutor.cpp
+-rw-r--r--   0        0        0     3294 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/StreamableExecutor.hpp
+-rw-r--r--   0        0        0      375 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/__init__.py
+-rw-r--r--   0        0        0     2175 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/__main__.py
+-rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/drivers.py
+-rw-r--r--   0        0        0    11626 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/libpdalpython.cpp
+-rw-r--r--   0        0        0     8308 2022-11-09 12:37:21.000000 pdal-3.4.3/src/pdal/pipeline.py
+-rw-r--r--   0        0        0    36439 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/1.2-with-color.las
+-rw-r--r--   0        0        0    37417 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/autzen-utm.las
+-rw-r--r--   0        0        0      111 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/bad.json
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/bad.py
+-rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/chip.json
+-rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/chip.py
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/mesh.json
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/mesh.py
+-rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/range.json
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/range.py
+-rw-r--r--   0        0        0      724 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/reproject.json
+-rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/reproject.py
+-rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/sort.json
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/sort.py
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 pdal-3.4.3/test/data/test3d.npy
+-rw-r--r--   0        0        0    22155 2022-11-09 12:37:21.000000 pdal-3.4.3/test/test_pipeline.py
+-rw-r--r--   0        0        0    15489 2022-11-09 12:37:21.000000 pdal-3.4.3/PKG-INFO
```

### Comparing `pdal-3.4.2/CHANGES.txt` & `pdal-3.4.3/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/CMakeLists.txt` & `pdal-3.4.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/LICENSE.txt` & `pdal-3.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/README.rst` & `pdal-3.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/pyproject.toml` & `pdal-3.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/setup.py.off` & `pdal-3.4.3/setup.py.off`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/PyArray.cpp` & `pdal-3.4.3/src/pdal/PyArray.cpp`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/PyArray.hpp` & `pdal-3.4.3/src/pdal/PyArray.hpp`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/PyDimension.hpp` & `pdal-3.4.3/src/pdal/PyDimension.hpp`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/PyPipeline.cpp` & `pdal-3.4.3/src/pdal/PyPipeline.cpp`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/PyPipeline.hpp` & `pdal-3.4.3/src/pdal/PyPipeline.hpp`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/StreamableExecutor.cpp` & `pdal-3.4.3/src/pdal/StreamableExecutor.cpp`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/StreamableExecutor.hpp` & `pdal-3.4.3/src/pdal/StreamableExecutor.hpp`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/__main__.py` & `pdal-3.4.3/src/pdal/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
 def print_driver_path(args):
-    print (os.environ['PDAL_DRIVER_PATH'])
+    if 'PDAL_DRIVER_PATH' in os.environ:
+        print (os.environ['PDAL_DRIVER_PATH'])
 
 def print_plugin_path(args):
     purelib = sysconfig.get_paths()["purelib"]
 
     if sys.platform == "linux" or sys.platform == "linux2":
         suffix = 'so'
         purelib = purelib + os.path.sep + "pdal"
```

### Comparing `pdal-3.4.2/src/pdal/drivers.py` & `pdal-3.4.3/src/pdal/drivers.py`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/libpdalpython.cpp` & `pdal-3.4.3/src/pdal/libpdalpython.cpp`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/src/pdal/pipeline.py` & `pdal-3.4.3/src/pdal/pipeline.py`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/test/data/1.2-with-color.las` & `pdal-3.4.3/test/data/1.2-with-color.las`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/test/data/autzen-utm.las` & `pdal-3.4.3/test/data/autzen-utm.las`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/test/data/reproject.json` & `pdal-3.4.3/test/data/reproject.json`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/test/data/reproject.py` & `pdal-3.4.3/test/data/reproject.py`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/test/test_pipeline.py` & `pdal-3.4.3/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pdal-3.4.2/PKG-INFO` & `pdal-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdal
-Version: 3.4.2
+Version: 3.4.3
 Summary: Point cloud data processing
 Keywords: point,cloud,spatial
 Home-page: https://pdal.io
 Author: Howard Butler
 Author-Email: Unknown <howard@hobu.co>
 Maintainer-Email: Howard Butler <howard@hobu.co>
 License: Unless otherwise indicated, all files in the PDAL distribution are
```


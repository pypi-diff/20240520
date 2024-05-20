# Comparing `tmp/pysma_plus-0.2.7.tar.gz` & `tmp/pysma_plus-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma_plus-0.2.7.tar", last modified: Sat May 18 16:20:43 2024, max compression
+gzip compressed data, was "pysma_plus-0.2.8.tar", last modified: Sun May 19 17:13:01 2024, max compression
```

## Comparing `pysma_plus-0.2.7.tar` & `pysma_plus-0.2.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 16:20:43.938476 pysma_plus-0.2.7/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-18 16:20:43.938476 pysma_plus-0.2.7/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1089 2024-05-18 07:09:53.000000 pysma_plus-0.2.7/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      924 2024-05-18 16:20:40.000000 pysma_plus-0.2.7/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 16:20:43.938476 pysma_plus-0.2.7/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-18 16:20:43.000000 pysma_plus-0.2.7/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1093 2024-05-18 16:20:43.000000 pysma_plus-0.2.7/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-18 16:20:43.000000 pysma_plus-0.2.7/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       58 2024-05-18 16:20:43.000000 pysma_plus-0.2.7/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-18 16:20:43.000000 pysma_plus-0.2.7/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.7/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 16:20:43.935475 pysma_plus-0.2.7/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     2798 2024-05-16 18:50:02.000000 pysma_plus-0.2.7/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    19249 2024-05-16 19:55:39.000000 pysma_plus-0.2.7/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-06 09:37:05.000000 pysma_plus-0.2.7/pysmaplus/const_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    10390 2024-05-10 06:46:58.000000 pysma_plus-0.2.7/pysmaplus/definitions_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    32364 2024-05-18 14:47:57.000000 pysma_plus-0.2.7/pysmaplus/definitions_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21517 2024-05-06 09:37:05.000000 pysma_plus-0.2.7/pysmaplus/definitions_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1437 2024-05-18 14:17:32.000000 pysma_plus-0.2.7/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9957 2024-05-16 19:56:05.000000 pysma_plus-0.2.7/pysmaplus/device_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    12168 2024-05-18 13:46:36.000000 pysma_plus-0.2.7/pysmaplus/device_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    19879 2024-05-18 16:18:16.000000 pysma_plus-0.2.7/pysmaplus/device_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17330 2024-05-06 11:20:09.000000 pysma_plus-0.2.7/pysmaplus/device_webconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1880 2024-05-16 18:57:36.000000 pysma_plus-0.2.7/pysmaplus/discovery.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.7/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.7/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6383 2024-05-06 10:39:02.000000 pysma_plus-0.2.7/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-18 16:20:43.939476 pysma_plus-0.2.7/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-18 16:20:40.000000 pysma_plus-0.2.7/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 16:20:43.937476 pysma_plus-0.2.7/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.7/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.7/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/test_em.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/test_ennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.7/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/test_sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      884 2024-05-03 18:21:37.000000 pysma_plus-0.2.7/tests/test_speedwire.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/test_webconnect.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-18 16:20:43.938476 pysma_plus-0.2.7/tests/testdata/
--rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/testdata/EVCharger-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/testdata/EVCharger-measurements.json.source
--rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/testdata/SunnyHomeManager2.json
--rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/testdata/TripowerX15-deviceinfo.json
--rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/testdata/TripowerX15-measurements.json
--rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.7/tests/testdata/TripowerX15-parameters.json
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.043239 pysma_plus-0.2.8/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1400 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-19 17:13:01.043239 pysma_plus-0.2.8/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1089 2024-05-18 07:09:53.000000 pysma_plus-0.2.8/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      924 2024-05-19 17:12:52.000000 pysma_plus-0.2.8/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.043239 pysma_plus-0.2.8/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3551 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1093 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       58 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-05-19 17:13:01.000000 pysma_plus-0.2.8/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-05-01 08:48:05.000000 pysma_plus-0.2.8/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.041239 pysma_plus-0.2.8/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2798 2024-05-16 18:50:02.000000 pysma_plus-0.2.8/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    19249 2024-05-16 19:55:39.000000 pysma_plus-0.2.8/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-05-06 09:37:05.000000 pysma_plus-0.2.8/pysmaplus/const_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    10406 2024-05-19 16:37:59.000000 pysma_plus-0.2.8/pysmaplus/definitions_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    32359 2024-05-19 13:50:59.000000 pysma_plus-0.2.8/pysmaplus/definitions_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21517 2024-05-06 09:37:05.000000 pysma_plus-0.2.8/pysmaplus/definitions_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1437 2024-05-18 14:17:32.000000 pysma_plus-0.2.8/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9957 2024-05-16 19:56:05.000000 pysma_plus-0.2.8/pysmaplus/device_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    12623 2024-05-19 16:43:23.000000 pysma_plus-0.2.8/pysmaplus/device_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    20092 2024-05-19 13:59:09.000000 pysma_plus-0.2.8/pysmaplus/device_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17330 2024-05-06 11:20:09.000000 pysma_plus-0.2.8/pysmaplus/device_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1880 2024-05-16 18:57:36.000000 pysma_plus-0.2.8/pysmaplus/discovery.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-05-01 08:46:05.000000 pysma_plus-0.2.8/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-05-01 08:46:05.000000 pysma_plus-0.2.8/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6451 2024-05-19 16:33:32.000000 pysma_plus-0.2.8/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-05-19 17:13:01.044239 pysma_plus-0.2.8/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-05-19 17:12:52.000000 pysma_plus-0.2.8/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.041239 pysma_plus-0.2.8/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-05-01 08:46:05.000000 pysma_plus-0.2.8/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     2500 2024-05-03 13:38:38.000000 pysma_plus-0.2.8/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-05-01 08:46:05.000000 pysma_plus-0.2.8/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      884 2024-05-03 18:21:37.000000 pysma_plus-0.2.8/tests/test_speedwire.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-05-19 17:13:01.042239 pysma_plus-0.2.8/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-05-01 08:47:50.000000 pysma_plus-0.2.8/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma_plus-0.2.7/LICENSE` & `pysma_plus-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/PKG-INFO` & `pysma_plus-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.7
+Version: 0.2.8
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.7
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.8
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.7/README.md` & `pysma_plus-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pyproject.toml` & `pysma_plus-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.2.7"
+version = "0.2.8"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma_plus-0.2.7/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.2.8/pysma_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.2.7
+Version: 0.2.8
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.7
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.2.8
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The webconnect Interface was created by kellerza.
         Later Engery-Meter and EnnexOS Support was added by little.yoda.
         Parts of the SMA-Query-Library (https://github.com/Wired-Square/sma-query/) by Garth Berry
         was added to this Library and modified by little.yoda
```

### Comparing `pysma_plus-0.2.7/pysma_plus.egg-info/SOURCES.txt` & `pysma_plus-0.2.8/pysma_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/__init__.py` & `pysma_plus-0.2.8/pysmaplus/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/const.py` & `pysma_plus-0.2.8/pysmaplus/const.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/const_webconnect.py` & `pysma_plus-0.2.8/pysmaplus/const_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/definitions_ennexos.py` & `pysma_plus-0.2.8/pysmaplus/definitions_ennexos.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Definition for all enneoxOS senosrs 
 """
 
 from .sensor import Sensor
 from .const import Identifier
 from .const import SMATagList
 
-
 ennexosSensorProfiles = {
     "Sunny Tripower X ": [
         Sensor("Coolsys.Inverter.TmpVal.1", Identifier.temp_a, factor=1, unit="°C"),
         Sensor("Coolsys.Inverter.TmpVal.2", Identifier.temp_b, factor=1, unit="°C"),
         Sensor("Coolsys.Inverter.TmpVal.3", Identifier.temp_c, factor=1, unit="°C"),
         Sensor("DcMs.Amp.1", Identifier.pv_current_a, factor=1, unit="A"),
         Sensor("DcMs.Amp.2", Identifier.pv_current_b, factor=1, unit="A"),
@@ -153,24 +152,24 @@
             "Wl.SigPwr", None, factor=1, unit=None
         ),  # Signal strength of the selected network
         Sensor(
             "Wl.SoftAcsConnStt", None, factor=1, unit=None
         ),  # Soft Access Point status
         Sensor("Setpoint.PlantControl.InOut.GO1", None, factor=1, unit=None),
     ],
-    "SMA EV Charger ": [
+    "^(SMA EV Charger |EVC22-3AC-10)": [
         Sensor("ChaSess.WhIn", None, factor=1, unit=None),  # charging_session_energy
         Sensor(
             "Chrg.ModSw", None, factor=1, unit=None, mapper=SMATagList
         ),  # position_of_rotary_switch 4950 or 4718
         Sensor(
             "GridMs.A.phsA", Identifier.current_l1, factor=1, unit="A"
         ),  # Netzstrom Phase L1
         Sensor("GridMs.A.phsB", Identifier.current_l2, factor=1, unit="A"),
-        Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
+  #      Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
         Sensor("GridMs.Hz", Identifier.frequency, factor=1, unit="Hz"),
         Sensor(
             "GridMs.PhV.phsA", Identifier.voltage_l1, factor=1, unit="V"
         ),  # Netzspannung Phase L1
         Sensor("GridMs.PhV.phsB", Identifier.voltage_l2, factor=1, unit="V"),
         Sensor("GridMs.PhV.phsC", Identifier.voltage_l3, factor=1, unit="V"),
         Sensor("GridMs.TotPF", None, factor=1, unit=None),
```

### Comparing `pysma_plus-0.2.7/pysmaplus/definitions_speedwire.py` & `pysma_plus-0.2.8/pysmaplus/definitions_speedwire.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,31 +71,31 @@
             ),
             "idx": 0,
         }
     ],
     "40464001": [
         {
             "cmd": "spot_ac_power",
-            "format": "uint",
+            "format": "int",
             "sensor": Sensor("spot_ac_power1", Identifier.power_l1, factor=1, unit="W"),
             "idx": 0,
         }
     ],
     "40464101": [
         {
             "cmd": "spot_ac_power",
-            "format": "uint",
+            "format": "int",
             "sensor": Sensor("spot_ac_power2", Identifier.power_l2, factor=1, unit="W"),
             "idx": 0,
         }
     ],
     "40464201": [
         {
             "cmd": "spot_ac_power",
-            "format": "uint",
+            "format": "int",
             "sensor": Sensor("spot_ac_power3", Identifier.power_l3, factor=1, unit="W"),
             "idx": 0,
         }
     ],
     "08412801": [
         {
             "cmd": "OperatingStatus",
@@ -125,15 +125,15 @@
             "sensor": Sensor("pv_power", Identifier.pv_power, unit="W"),
             "idx": 0,
         }
     ],
     "40263F01": [
         {
             "cmd": "SpotACTotalPower",
-            "format": "uint",
+            "format": "int",
             "sensor": Sensor("grid_power", Identifier.grid_power, unit="W"),
             "idx": 0,
         }
     ],
     "00464801": [
         {
             "cmd": "spot_ac_voltage",
@@ -470,15 +470,15 @@
             ),
             "idx": 0,
         }
     ],
     "40495D01": [
         {
             "cmd": "battery_current_a",
-            "format": "uint",
+            "format": "int",
             "sensor": Sensor(
                 "battery_current_a",
                 Identifier.battery_current_a,
                 unit="A",
                 factor=1000,
             ),
             "idx": 0,
```

### Comparing `pysma_plus-0.2.7/pysmaplus/definitions_webconnect.py` & `pysma_plus-0.2.8/pysmaplus/definitions_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/device.py` & `pysma_plus-0.2.8/pysmaplus/device.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/device_em.py` & `pysma_plus-0.2.8/pysmaplus/device_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/device_ennexos.py` & `pysma_plus-0.2.8/pysmaplus/device_ennexos.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 import asyncio
 import copy
 import json
 import logging
 from typing import Any, Dict, Optional
-
+import re
 
 from aiohttp import ClientSession, ClientTimeout, client_exceptions, hdrs
 from .const_webconnect import (
     DEFAULT_TIMEOUT,
 )
 from .exceptions import (
     SmaAuthenticationException,
@@ -34,17 +34,18 @@
 
     # pylint: disable=too-many-instance-attributes
     _aio_session: ClientSession
     _new_session_data: Optional[dict]
     _url: str
     _token: str
     _authorization_header: dict[str, str]
-    _last_parameters: Any
-    _last_measurements: Any
-    _last_device: Any
+    _last_parameters: Any = {}
+    _last_measurements: Any = {}
+    _last_device: Any = {}
+    _last_notfound: list = []
     _device_info: Dict = None
     _jsessionid: str = None
 
     def __init__(
         self,
         session: ClientSession,
         url: str,
@@ -186,14 +187,17 @@
         """
         liveurl = self._url + "/api/v1/measurements/live"
         postdata = {
             "data": '[{"componentId":"IGULD:SELF"}]',
             "headers": self._authorization_header,
         }
         ret = await self._jsonrequest(liveurl, postdata)
+        return await self._prepare_livedata(ret)
+
+    async def _prepare_livedata(self, ret):
         self._last_measurements = ret
         data = {}
         for d in ret:
             dname = d["channelId"].replace("Measurement.", "").replace("[]", "")
             if "value" in d["values"][0]:
                 v = d["values"][0]["value"]
                 if self._isfloat(v):
@@ -221,31 +225,36 @@
 
         Returns:
             Sensors: Sensors object containing Sensor objects
         """
         if not self._device_info:
             raise SmaReadException("device_info() not called!")
 
+        
         ret = await self._get_livedata()
         _LOGGER.debug("Found Sensors: %s", ret)
+        profile = await self._get_sensor_profile()
+        return profile
 
+    async def _get_sensor_profile(self):
         device_sensors = Sensors()
-        sensors = []
+        expectedSensors = []
 
         # Search for matiching profile
-        for dev in ennexosSensorProfiles.items():
-            if self._device_info["name"].startswith(dev[0]):
-                sensors = dev[1]
-        if len(sensors) == 0:
+        for profil in ennexosSensorProfiles.items():
+            if re.search(profil[0], self._device_info["name"]):
+            #self._device_info["name"].startswith(dev[0]):
+                expectedSensors = profil[1]
+        if len(expectedSensors) == 0:
             _LOGGER.warning(
                 f'Unknown Device: {self._device_info["name"]} {self._device_info["type"]}'
             )
 
         # Add Sensors from profile
-        for s in sensors:
+        for s in expectedSensors:
             if s.name:
                 device_sensors.add(copy.copy(s))
         return device_sensors
 
     async def close_session(self) -> None:
         pass
 
@@ -301,14 +310,15 @@
                         sen.mapped_value = sen.mapper.get(value, str(value))
                     if sen.factor and sen.factor != 1:
                         value = round(value / sen.factor, 4)
                     sen.value = value
                     continue
                 notfound.append(f"{sen.name} [{sen.key}]")
 
+        self._last_notfound = notfound
         if notfound:
             _LOGGER.info(
                 "No values for sensors: %s",
                 ",".join(notfound),
             )
 
         return True
@@ -337,14 +347,15 @@
     async def get_debug(self) -> Dict:
         """Collect all Debug Information"""
         return {
             "device": self._last_device,
             "measurements": self._last_measurements,
             "parameters": self._last_parameters,
             "device_info": self._device_info,
+            "notfound": self._last_notfound
         }
 
     async def detect(self, ip):
         rets = []
         for prefix in ["https", "http"]:
             url = f"{prefix}://{ip}/api/v1/system/info"
             ret = (await super().detect(ip))[0]
```

### Comparing `pysma_plus-0.2.7/pysmaplus/device_speedwire.py` & `pysma_plus-0.2.8/pysmaplus/device_speedwire.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         self.data_values[sen.key] = value
 
     def extractvalues(self, handler: Dict, subdata):
         (formatdef, size, converter) = self._getFormat(handler)
         values = []
         for idx in range(8, len(subdata), size):
             v = struct.unpack(formatdef, subdata[idx : idx + size])[0]
-            if v in [0xFFFFFFFF, 0x80000000, 0xFFFFFFEC]:
+            if v in [0xFFFFFFFF, 0x80000000, 0xFFFFFFEC, -0x80000000]:
                 v = None
             else:
                 if converter:
                     v = converter(v)
                 if "mask" in handler:
                     v = v & handler["mask"]
             values.append(v)
@@ -275,14 +275,15 @@
                         f"No Handler for {c} at register idx {register_idx}: {values}"
                     )
                     continue
                 _LOGGER.debug(
                     f"Special Handler for {c} at register idx {register_idx}: {values}"
                 )
                 sensor = sensor[register_idx]
+            _LOGGER.debug(f"Values {sensor.name}/{sensor.key}: {values[handler['idx']]} {values}")
             self.handle_newvalue(sensor, v)
 
     # Unfortunately, there is no known method of determining the size of the registers
     # from the message. Therefore, the register size is determined from the number of
     # registers and the size of the payload.
     def calc_register(self, data, msg: speedwireHeader6065):
         cnt_registers = msg.lastRegister - msg.firstRegister + 1
@@ -402,22 +403,26 @@
                 if "sensor" in r:
                     sensor = r["sensor"]
                     if isinstance(sensor, Sensor) and sensor.key in sensorname:
                         print("Doppelter Sensorname " + sensor.key)
                         raise RuntimeError("Doppelter Sensorname " + sensor.key)
                     sensorname[name] = 1
 
-    async def new_session(self) -> bool:
+    async def _createEndpoint(self):
         loop = asyncio.get_running_loop()
         on_connection_lost = loop.create_future()
-
         self._transport, self._protocol = await loop.create_datagram_endpoint(
             lambda: SMAClientProtocol(self._password, on_connection_lost, self._options),
             remote_addr=(self._host, 9522),
         )
+
+    async def new_session(self) -> bool:
+        # Create Endpoint
+        await self._createEndpoint()
+
         # Test with device_info if the ip and user/pwd are correct
         await self.device_info()
         if (self._protocol._failedCounter >= self._protocol._sendCounter):
             raise SmaConnectionException("No connection to device: %s:9522",self._host)
 
     async def device_info(self) -> dict:
         fut = asyncio.get_running_loop().create_future()
```

### Comparing `pysma_plus-0.2.7/pysmaplus/device_webconnect.py` & `pysma_plus-0.2.8/pysmaplus/device_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/discovery.py` & `pysma_plus-0.2.8/pysmaplus/discovery.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/helpers.py` & `pysma_plus-0.2.8/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/pysmaplus/sensor.py` & `pysma_plus-0.2.8/pysmaplus/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     unit: str = attr.ib(default=None)
     factor: int = attr.ib(default=None)
     path: Union[list, tuple] = attr.ib(default=None)
     enabled: bool = attr.ib(default=True)
     l10n_translate: bool = attr.ib(default=False)
     value: Any = attr.ib(default=None, init=False)
     key_idx: int = attr.ib(default=0, repr=False, init=False)
-    mapper: dict[int, str] = attr.ib(default=None)
+    mapper: dict[int, str] = attr.ib(default=None,repr=False)
     mapped_value: Any = attr.ib(default=None, init=False)
 
     def __attrs_post_init__(self) -> None:
         """Post init Sensor."""
         key = str(self.key)
         skey = key.split("_")
         if len(skey) > 2 and skey[2].isdigit():
@@ -207,7 +207,11 @@
 
         if sensor.key in self and self[sensor.key].key_idx == sensor.key_idx:
             _LOGGER.warning(
                 "Duplicate SMA sensor key %s (idx: %s)", sensor.key, sensor.key_idx
             )
 
         self.__s.append(sensor)
+
+    def __str__(self):
+        return str(self.__s)
+
```

### Comparing `pysma_plus-0.2.7/setup.py` & `pysma_plus-0.2.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.2.7"
+VERSION = "0.2.8"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma_plus-0.2.7/tests/__init__.py` & `pysma_plus-0.2.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/test_definitions.py` & `pysma_plus-0.2.8/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/test_em.py` & `pysma_plus-0.2.8/tests/test_em.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/test_ennexos.py` & `pysma_plus-0.2.8/tests/test_ennexos.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/test_sensor.py` & `pysma_plus-0.2.8/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/test_speedwire.py` & `pysma_plus-0.2.8/tests/test_speedwire.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/test_webconnect.py` & `pysma_plus-0.2.8/tests/test_webconnect.py`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/testdata/EVCharger-measurements.json` & `pysma_plus-0.2.8/tests/testdata/EVCharger-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/testdata/SunnyHomeManager2.json` & `pysma_plus-0.2.8/tests/testdata/SunnyHomeManager2.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/testdata/TripowerX15-deviceinfo.json` & `pysma_plus-0.2.8/tests/testdata/TripowerX15-deviceinfo.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/testdata/TripowerX15-measurements.json` & `pysma_plus-0.2.8/tests/testdata/TripowerX15-measurements.json`

 * *Files identical despite different names*

### Comparing `pysma_plus-0.2.7/tests/testdata/TripowerX15-parameters.json` & `pysma_plus-0.2.8/tests/testdata/TripowerX15-parameters.json`

 * *Files identical despite different names*


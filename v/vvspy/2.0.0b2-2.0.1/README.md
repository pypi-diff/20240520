# Comparing `tmp/vvspy-2.0.0b2.tar.gz` & `tmp/vvspy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvspy-2.0.0b2.tar", last modified: Sun May 19 14:10:53 2024, max compression
+gzip compressed data, was "vvspy-2.0.1.tar", last modified: Mon May 20 06:50:10 2024, max compression
```

## Comparing `vvspy-2.0.0b2.tar` & `vvspy-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5229 2024-05-19 13:53:52.000000 vvspy-2.0.0b2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4212 2024-05-19 13:54:39.000000 vvspy-2.0.0b2/CONTRIBUTING.md
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1071 2024-05-19 11:23:13.000000 vvspy-2.0.0b2/LICENSE
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      207 2024-05-19 14:09:10.000000 vvspy-2.0.0b2/MANIFEST.in
--rw-r--r--   0 zaanposni  (1000) zaanposni  (1000)     5210 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/PKG-INFO
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      280 2024-05-19 13:54:16.000000 vvspy-2.0.0b2/SECURITY.md
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      313 2024-05-19 13:47:44.000000 vvspy-2.0.0b2/pyproject.toml
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4159 2024-05-19 14:08:59.000000 vvspy-2.0.0b2/readme.md
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       33 2024-05-19 11:23:47.000000 vvspy-2.0.0b2/requirements.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       38 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/setup.cfg
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1382 2024-05-19 14:10:14.000000 vvspy-2.0.0b2/setup.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.236479 vvspy-2.0.0b2/vvspy/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5490 2024-05-19 14:08:36.000000 vvspy-2.0.0b2/vvspy/__init__.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4897 2024-05-19 14:08:39.000000 vvspy-2.0.0b2/vvspy/arrivals.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4785 2024-05-19 14:08:47.000000 vvspy-2.0.0b2/vvspy/departures.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.238479 vvspy-2.0.0b2/vvspy/enums/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       30 2024-05-19 14:07:12.000000 vvspy-2.0.0b2/vvspy/enums/__init__.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)  1576406 2024-05-19 12:37:53.000000 vvspy-2.0.0b2/vvspy/enums/stations.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/vvspy/models/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      334 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/__init__.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4071 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/arrival.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2832 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/connection.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3931 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/departure.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2205 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/destination.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      663 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/line_operator.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2246 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/origin.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2340 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/serving_line.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1561 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/transportation.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1384 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/trip.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5955 2024-05-19 14:08:52.000000 vvspy-2.0.0b2/vvspy/trip.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/vvspy.egg-info/
--rw-r--r--   0 zaanposni  (1000) zaanposni  (1000)     5210 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/PKG-INFO
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      643 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/SOURCES.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        1 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/dependency_links.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       16 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/requires.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        6 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:50:10.057790 vvspy-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-20 06:49:51.000000 vvspy-2.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-20 06:49:51.000000 vvspy-2.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 06:49:51.000000 vvspy-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-20 06:49:51.000000 vvspy-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-20 06:50:10.057790 vvspy-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 06:49:51.000000 vvspy-2.0.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 06:49:51.000000 vvspy-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-20 06:49:51.000000 vvspy-2.0.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 06:49:51.000000 vvspy-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:50:10.057790 vvspy-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-20 06:49:51.000000 vvspy-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:50:10.053789 vvspy-2.0.1/vvspy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/arrivals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/departures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:50:10.053789 vvspy-2.0.1/vvspy/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1576406 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/enums/stations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:50:10.057790 vvspy-2.0.1/vvspy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/arrival.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/departure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/line_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/serving_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/transportation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/models/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-20 06:49:51.000000 vvspy-2.0.1/vvspy/trip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:50:10.057790 vvspy-2.0.1/vvspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-20 06:50:10.000000 vvspy-2.0.1/vvspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-20 06:50:10.000000 vvspy-2.0.1/vvspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:50:10.000000 vvspy-2.0.1/vvspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 06:50:10.000000 vvspy-2.0.1/vvspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 06:50:10.000000 vvspy-2.0.1/vvspy.egg-info/top_level.txt
```

### Comparing `vvspy-2.0.0b2/CODE_OF_CONDUCT.md` & `vvspy-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/CONTRIBUTING.md` & `vvspy-2.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/LICENSE` & `vvspy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/PKG-INFO` & `vvspy-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: vvspy
-Version: 2.0.0b2
+Version: 2.0.1
 Summary: API Wrapper for VVS (Verkehrsverbund Stuttgart)
 Home-page: https://github.com/zaanposni/vvspy
 Author: zaanposni
 Author-email: vvspy@zaanposni.com
 License: MIT
 Keywords: vvs,api,stuttgart,wrapper,json,rest,efa,python
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `vvspy-2.0.0b2/readme.md` & `vvspy-2.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/setup.py` & `vvspy-2.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="vvspy",
-    version="2.0.0-beta.2",
+    version="2.0.1",
     license="MIT",
     description="API Wrapper for VVS (Verkehrsverbund Stuttgart)",
     author="zaanposni",
     author_email="vvspy@zaanposni.com",
     url="https://github.com/zaanposni/vvspy",
     keywords=["vvs", "api", "stuttgart", "wrapper", "json", "rest", "efa", "python"],
     packages=find_packages(exclude=["*tests"]),
     package_data={"vvspy": ["vvspy/*"]},
     python_requires=">=3.6",
     install_requires=[
         "requests",
         "typing",
     ],
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `vvspy-2.0.0b2/vvspy/__init__.py` & `vvspy-2.0.1/vvspy/__init__.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/arrivals.py` & `vvspy-2.0.1/vvspy/arrivals.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             "anySigWhenPerfectNoOtherMatches", 1
         ),
         "limit": limit,
         "depArr": "arrival",
         "type_dm": kwargs.get("type_dm", "any"),
         "anyObjFilter_dm": kwargs.get("anyObjFilter_dm", 2),
         "deleteAssignedStops": kwargs.get("deleteAssignedStops", 1),
-        "name_dm": station_id.value,
+        "name_dm": station_id.value if type(station_id) == "<enum 'Station'>" else str(station_id),
         "mode": kwargs.get("mode", "direct"),
         "dmLineSelectionAll": kwargs.get("dmLineSelectionAll", 1),
         "useRealtime": kwargs.get("useRealtime", 1),  # live delay
         "outputFormat": kwargs.get("outputFormat", "json"),
         "coordOutputFormat": kwargs.get("coordOutputFormat", "WGS84[DD.ddddd]"),
         "itdDateTimeDepArr": "arr",
         "itdDateYear": check_time.strftime("%Y"),
```

### Comparing `vvspy-2.0.0b2/vvspy/departures.py` & `vvspy-2.0.1/vvspy/departures.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             "anySigWhenPerfectNoOtherMatches", 1
         ),
         "limit": limit,
         "depArr": "departure",
         "type_dm": kwargs.get("type_dm", "any"),
         "anyObjFilter_dm": kwargs.get("anyObjFilter_dm", 2),
         "deleteAssignedStops": kwargs.get("deleteAssignedStops", 1),
-        "name_dm": station_id.value,
+        "name_dm": station_id.value if type(station_id) == "<enum 'Station'>" else str(station_id),
         "mode": kwargs.get("mode", "direct"),
         "dmLineSelectionAll": kwargs.get("dmLineSelectionAll", 1),
         "useRealtime": kwargs.get("useRealtime", 1),  # live delay
         "outputFormat": "json",
         "coordOutputFormat": kwargs.get("coordOutputFormat", "WGS84[DD.ddddd]"),
         "itdDateYear": check_time.strftime("%Y"),
         "itdDateMonth": check_time.strftime("%m"),
```

### Comparing `vvspy-2.0.0b2/vvspy/enums/stations.py` & `vvspy-2.0.1/vvspy/enums/stations.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/arrival.py` & `vvspy-2.0.1/vvspy/models/arrival.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/connection.py` & `vvspy-2.0.1/vvspy/models/connection.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/departure.py` & `vvspy-2.0.1/vvspy/models/departure.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/destination.py` & `vvspy-2.0.1/vvspy/models/destination.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/line_operator.py` & `vvspy-2.0.1/vvspy/models/line_operator.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/origin.py` & `vvspy-2.0.1/vvspy/models/origin.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/serving_line.py` & `vvspy-2.0.1/vvspy/models/serving_line.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/transportation.py` & `vvspy-2.0.1/vvspy/models/transportation.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/models/trip.py` & `vvspy-2.0.1/vvspy/models/trip.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b2/vvspy/trip.py` & `vvspy-2.0.1/vvspy/trip.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
         "imparedOptionsActive": kwargs.get("imparedOptionsActive", "1"),
         "itOptionsActive": kwargs.get("itOptionsActive", "1"),
         "itdDate": check_time.strftime("%Y%m%d"),
         "itdTime": check_time.strftime("%H%M"),
         "language": kwargs.get("language", "de"),
         "locationServerActive": kwargs.get("locationServerActive", "1"),
         "macroWebTrip": kwargs.get("macroWebTrip", "true"),
-        "name_destination": destination_station_id.value,
-        "name_origin": origin_station_id.value,
+        "name_destination": destination_station_id.value if type(destination_station_id) == "<enum 'Station'>" else str(destination_station_id),
+        "name_origin": origin_station_id.value if type(origin_station_id) == "<enum 'Station'>" else str(origin_station_id),
         "noElevationProfile": kwargs.get("noElevationProfile", "1"),
         "noElevationSummary": kwargs.get("noElevationSummary", "1"),
         "outputFormat": "rapidJSON",
         "outputOptionsActive": "1",
         "ptOptionsActive": kwargs.get("ptOptionsActive", "1"),
         "routeType": kwargs.get("routeType", "leasttime"),
         "searchLimitMinutes": kwargs.get("searchLimitMinutes", "360"),
```

### Comparing `vvspy-2.0.0b2/vvspy.egg-info/PKG-INFO` & `vvspy-2.0.1/vvspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: vvspy
-Version: 2.0.0b2
+Version: 2.0.1
 Summary: API Wrapper for VVS (Verkehrsverbund Stuttgart)
 Home-page: https://github.com/zaanposni/vvspy
 Author: zaanposni
 Author-email: vvspy@zaanposni.com
 License: MIT
 Keywords: vvs,api,stuttgart,wrapper,json,rest,efa,python
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `vvspy-2.0.0b2/vvspy.egg-info/SOURCES.txt` & `vvspy-2.0.1/vvspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/vvspy-2.0.0b1.tar.gz` & `tmp/vvspy-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvspy-2.0.0b1.tar", last modified: Sun May 19 13:50:33 2024, max compression
+gzip compressed data, was "vvspy-2.0.0b2.tar", last modified: Sun May 19 14:10:53 2024, max compression
```

## Comparing `vvspy-2.0.0b1.tar` & `vvspy-2.0.0b2.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.830130 vvspy-2.0.0b1/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1071 2024-05-19 11:23:13.000000 vvspy-2.0.0b1/LICENSE
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      207 2024-05-19 11:25:25.000000 vvspy-2.0.0b1/MANIFEST.in
--rw-r--r--   0 zaanposni  (1000) zaanposni  (1000)     5250 2024-05-19 13:50:33.830130 vvspy-2.0.0b1/PKG-INFO
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      313 2024-05-19 13:47:44.000000 vvspy-2.0.0b1/pyproject.toml
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4186 2024-05-19 13:41:30.000000 vvspy-2.0.0b1/readme.md
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       33 2024-05-19 11:23:47.000000 vvspy-2.0.0b1/requirements.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       38 2024-05-19 13:50:33.830130 vvspy-2.0.0b1/setup.cfg
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1395 2024-05-19 13:50:26.000000 vvspy-2.0.0b1/setup.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.825130 vvspy-2.0.0b1/vvspy/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5499 2024-05-19 13:11:28.000000 vvspy-2.0.0b1/vvspy/__init__.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4906 2024-05-19 13:20:17.000000 vvspy-2.0.0b1/vvspy/arrivals.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4794 2024-05-19 13:20:15.000000 vvspy-2.0.0b1/vvspy/departures.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.826130 vvspy-2.0.0b1/vvspy/enums/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)  1576406 2024-05-19 12:37:53.000000 vvspy-2.0.0b1/vvspy/enums/stations.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.829130 vvspy-2.0.0b1/vvspy/models/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      334 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/__init__.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4071 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/arrival.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2832 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/connection.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3931 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/departure.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2205 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/destination.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      663 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/line_operator.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2246 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/origin.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2340 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/serving_line.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1561 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/transportation.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1384 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/trip.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5964 2024-05-19 13:19:51.000000 vvspy-2.0.0b1/vvspy/trip.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.829130 vvspy-2.0.0b1/vvspy.egg-info/
--rw-r--r--   0 zaanposni  (1000) zaanposni  (1000)     5250 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/PKG-INFO
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      572 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/SOURCES.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        1 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/dependency_links.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       16 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/requires.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        6 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/top_level.txt
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5229 2024-05-19 13:53:52.000000 vvspy-2.0.0b2/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4212 2024-05-19 13:54:39.000000 vvspy-2.0.0b2/CONTRIBUTING.md
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1071 2024-05-19 11:23:13.000000 vvspy-2.0.0b2/LICENSE
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      207 2024-05-19 14:09:10.000000 vvspy-2.0.0b2/MANIFEST.in
+-rw-r--r--   0 zaanposni  (1000) zaanposni  (1000)     5210 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/PKG-INFO
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      280 2024-05-19 13:54:16.000000 vvspy-2.0.0b2/SECURITY.md
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      313 2024-05-19 13:47:44.000000 vvspy-2.0.0b2/pyproject.toml
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4159 2024-05-19 14:08:59.000000 vvspy-2.0.0b2/readme.md
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       33 2024-05-19 11:23:47.000000 vvspy-2.0.0b2/requirements.txt
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       38 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/setup.cfg
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1382 2024-05-19 14:10:14.000000 vvspy-2.0.0b2/setup.py
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.236479 vvspy-2.0.0b2/vvspy/
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5490 2024-05-19 14:08:36.000000 vvspy-2.0.0b2/vvspy/__init__.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4897 2024-05-19 14:08:39.000000 vvspy-2.0.0b2/vvspy/arrivals.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4785 2024-05-19 14:08:47.000000 vvspy-2.0.0b2/vvspy/departures.py
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.238479 vvspy-2.0.0b2/vvspy/enums/
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       30 2024-05-19 14:07:12.000000 vvspy-2.0.0b2/vvspy/enums/__init__.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)  1576406 2024-05-19 12:37:53.000000 vvspy-2.0.0b2/vvspy/enums/stations.py
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/vvspy/models/
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      334 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/__init__.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4071 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/arrival.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2832 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/connection.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3931 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/departure.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2205 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/destination.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      663 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/line_operator.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2246 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/origin.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2340 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/serving_line.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1561 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/transportation.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1384 2024-05-19 10:57:56.000000 vvspy-2.0.0b2/vvspy/models/trip.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5955 2024-05-19 14:08:52.000000 vvspy-2.0.0b2/vvspy/trip.py
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 14:10:53.242479 vvspy-2.0.0b2/vvspy.egg-info/
+-rw-r--r--   0 zaanposni  (1000) zaanposni  (1000)     5210 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/PKG-INFO
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      643 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        1 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       16 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/requires.txt
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        6 2024-05-19 14:10:53.000000 vvspy-2.0.0b2/vvspy.egg-info/top_level.txt
```

### Comparing `vvspy-2.0.0b1/LICENSE` & `vvspy-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/PKG-INFO` & `vvspy-2.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: vvspy
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: API Wrapper for VVS (Verkehrsverbund Stuttgart)
 Home-page: https://github.com/zaanposni/vvspy
 Author: zaanposni
 Author-email: vvspy@zaanposni.com
 License: MIT
 Keywords: vvs,api,stuttgart,wrapper,json,rest,efa,python
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,15 +44,15 @@
 
 ## Examples
 
 - Detect delay in upcoming departures:
 
 ```python
 from vvspy import get_departures
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 deps = get_departures(Station.HAUPTBAHNHOF__TIEF, limit=3)
 for dep in deps:
     if dep.delay > 0:
         print("Alarm! Delay detected.")
         print(dep)  # [Delayed] [11:47] [RB17]: Stuttgart Hauptbahnhof (oben) - Pforzheim Hauptbahnhof
 
@@ -61,15 +61,15 @@
         print(dep)  # [11:47] [RB17]: Stuttgart Hauptbahnhof (oben) - Pforzheim Hauptbahnhof
 ```
 
 - Get complete trip info between two stations (including interchanges):
 
 ```python
 from vvspy import get_trip  # also usable: get_trips
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 trip = get_trip(Station.HAUPTBAHNHOF__TIEF, Station.HARDTLINDE)
 
 print(f"Duration: {trip.duration / 60} minutes")
 for connection in trip.connections:
     print(f"From: {connection.origin.name} - To: {connection.destination.name}")
 ```
@@ -83,15 +83,15 @@
 From: Marbach (N) Bf - To: Murr Hardtlinde
 ```
 
 - Filter for specific lines:
 
 ```python
 from vvspy import get_departures
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 deps = get_departures(Station.HAUPTBAHNHOF__TIEF)
 for dep in deps:
     if dep.serving_line.symbol == "S4":
         print(f"Departure of S4 at {dep.real_datetime}")
 ```
```

### Comparing `vvspy-2.0.0b1/readme.md` & `vvspy-2.0.0b2/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ## Examples
 
 - Detect delay in upcoming departures:
 
 ```python
 from vvspy import get_departures
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 deps = get_departures(Station.HAUPTBAHNHOF__TIEF, limit=3)
 for dep in deps:
     if dep.delay > 0:
         print("Alarm! Delay detected.")
         print(dep)  # [Delayed] [11:47] [RB17]: Stuttgart Hauptbahnhof (oben) - Pforzheim Hauptbahnhof
 
@@ -33,15 +33,15 @@
         print(dep)  # [11:47] [RB17]: Stuttgart Hauptbahnhof (oben) - Pforzheim Hauptbahnhof
 ```
 
 - Get complete trip info between two stations (including interchanges):
 
 ```python
 from vvspy import get_trip  # also usable: get_trips
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 trip = get_trip(Station.HAUPTBAHNHOF__TIEF, Station.HARDTLINDE)
 
 print(f"Duration: {trip.duration / 60} minutes")
 for connection in trip.connections:
     print(f"From: {connection.origin.name} - To: {connection.destination.name}")
 ```
@@ -55,15 +55,15 @@
 From: Marbach (N) Bf - To: Murr Hardtlinde
 ```
 
 - Filter for specific lines:
 
 ```python
 from vvspy import get_departures
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 deps = get_departures(Station.HAUPTBAHNHOF__TIEF)
 for dep in deps:
     if dep.serving_line.symbol == "S4":
         print(f"Departure of S4 at {dep.real_datetime}")
 ```
```

### Comparing `vvspy-2.0.0b1/setup.py` & `vvspy-2.0.0b2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="vvspy",
-    version="2.0.0-beta.1",
+    version="2.0.0-beta.2",
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
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `vvspy-2.0.0b1/vvspy/__init__.py` & `vvspy-2.0.0b2/vvspy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime as __datetime
 from typing import List as __List
 from typing import Union as __Union
 from requests.models import Response as __Response
 from requests import Session
 import logging as __logging
 
-from .enums.stations import Station
+from .enums import Station
 from .models import Arrival as __Arrival
 from .models import Departure as __Departure
 from .models import Trip as __Trip
 from .trip import get_trips
 from .departures import get_departures
 from .arrivals import get_arrivals
```

### Comparing `vvspy-2.0.0b1/vvspy/arrivals.py` & `vvspy-2.0.0b2/vvspy/arrivals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Union
 from datetime import datetime
 import requests
 from requests.models import Response
 import json
 import logging as __logging
 
-from .enums.stations import Station
+from .enums import Station
 from .models import Arrival
 
 _API_URL = "http://www3.vvs.de/vvs/widget/XML_DM_REQUEST?"
 __logger = __logging.getLogger("vvspy")
 
 def get_arrivals(
     station_id: Union[str, int, Station],
```

### Comparing `vvspy-2.0.0b1/vvspy/departures.py` & `vvspy-2.0.0b2/vvspy/departures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Union
 from datetime import datetime
 import requests
 from requests.models import Response
 import json
 import logging as __logging
 
-from .enums.stations import Station
+from .enums import Station
 from vvspy.models import Departure
 
 __API_URL = "http://www3.vvs.de/vvs/widget/XML_DM_REQUEST?"
 __logger = __logging.getLogger("vvspy")
 
 def get_departures(
     station_id: Union[str, int, Station],
```

### Comparing `vvspy-2.0.0b1/vvspy/enums/stations.py` & `vvspy-2.0.0b2/vvspy/enums/stations.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/arrival.py` & `vvspy-2.0.0b2/vvspy/models/arrival.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/connection.py` & `vvspy-2.0.0b2/vvspy/models/connection.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/departure.py` & `vvspy-2.0.0b2/vvspy/models/departure.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/destination.py` & `vvspy-2.0.0b2/vvspy/models/destination.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/line_operator.py` & `vvspy-2.0.0b2/vvspy/models/line_operator.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/origin.py` & `vvspy-2.0.0b2/vvspy/models/origin.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/serving_line.py` & `vvspy-2.0.0b2/vvspy/models/serving_line.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/transportation.py` & `vvspy-2.0.0b2/vvspy/models/transportation.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/models/trip.py` & `vvspy-2.0.0b2/vvspy/models/trip.py`

 * *Files identical despite different names*

### Comparing `vvspy-2.0.0b1/vvspy/trip.py` & `vvspy-2.0.0b2/vvspy/trip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime, timezone
 import requests
 from requests.models import Response
 import json
 from typing import Union, List
 import logging as __logging
 
-from .enums.stations import Station
+from .enums import Station
 from .models import Trip
 
 __API_URL = "https://www3.vvs.de/mngvvs/XML_TRIP_REQUEST2"
 __logger = __logging.getLogger("vvspy")
 
 def get_trips(
     origin_station_id: Union[str, int, Station],
```

### Comparing `vvspy-2.0.0b1/vvspy.egg-info/PKG-INFO` & `vvspy-2.0.0b2/vvspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: vvspy
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: API Wrapper for VVS (Verkehrsverbund Stuttgart)
 Home-page: https://github.com/zaanposni/vvspy
 Author: zaanposni
 Author-email: vvspy@zaanposni.com
 License: MIT
 Keywords: vvs,api,stuttgart,wrapper,json,rest,efa,python
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,15 +44,15 @@
 
 ## Examples
 
 - Detect delay in upcoming departures:
 
 ```python
 from vvspy import get_departures
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 deps = get_departures(Station.HAUPTBAHNHOF__TIEF, limit=3)
 for dep in deps:
     if dep.delay > 0:
         print("Alarm! Delay detected.")
         print(dep)  # [Delayed] [11:47] [RB17]: Stuttgart Hauptbahnhof (oben) - Pforzheim Hauptbahnhof
 
@@ -61,15 +61,15 @@
         print(dep)  # [11:47] [RB17]: Stuttgart Hauptbahnhof (oben) - Pforzheim Hauptbahnhof
 ```
 
 - Get complete trip info between two stations (including interchanges):
 
 ```python
 from vvspy import get_trip  # also usable: get_trips
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 trip = get_trip(Station.HAUPTBAHNHOF__TIEF, Station.HARDTLINDE)
 
 print(f"Duration: {trip.duration / 60} minutes")
 for connection in trip.connections:
     print(f"From: {connection.origin.name} - To: {connection.destination.name}")
 ```
@@ -83,15 +83,15 @@
 From: Marbach (N) Bf - To: Murr Hardtlinde
 ```
 
 - Filter for specific lines:
 
 ```python
 from vvspy import get_departures
-from vvspy.enums.stations import Station
+from vvspy.enums import Station
 
 deps = get_departures(Station.HAUPTBAHNHOF__TIEF)
 for dep in deps:
     if dep.serving_line.symbol == "S4":
         print(f"Departure of S4 at {dep.real_datetime}")
 ```
```

### Comparing `vvspy-2.0.0b1/vvspy.egg-info/SOURCES.txt` & `vvspy-2.0.0b2/vvspy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
+SECURITY.md
 pyproject.toml
 readme.md
 requirements.txt
 setup.py
 vvspy/__init__.py
 vvspy/arrivals.py
 vvspy/departures.py
 vvspy/trip.py
 vvspy.egg-info/PKG-INFO
 vvspy.egg-info/SOURCES.txt
 vvspy.egg-info/dependency_links.txt
 vvspy.egg-info/requires.txt
 vvspy.egg-info/top_level.txt
+vvspy/enums/__init__.py
 vvspy/enums/stations.py
 vvspy/models/__init__.py
 vvspy/models/arrival.py
 vvspy/models/connection.py
 vvspy/models/departure.py
 vvspy/models/destination.py
 vvspy/models/line_operator.py
```


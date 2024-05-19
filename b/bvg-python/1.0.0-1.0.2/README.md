# Comparing `tmp/bvg-python-1.0.0.tar.gz` & `tmp/bvg_python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bvg-python-1.0.0.tar", last modified: Sun May 19 22:38:50 2024, max compression
+gzip compressed data, was "bvg_python-1.0.2.tar", last modified: Sun May 19 23:25:40 2024, max compression
```

## Comparing `bvg-python-1.0.0.tar` & `bvg_python-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 kpwde     (1000) kpwde     (1000)        0 2024-05-19 22:38:50.861494 bvg-python-1.0.0/
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)     7645 2024-05-19 22:38:50.861494 bvg-python-1.0.0/PKG-INFO
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)     5679 2024-05-19 22:30:45.000000 bvg-python-1.0.0/README.md
-drwxrwxr-x   0 kpwde     (1000) kpwde     (1000)        0 2024-05-19 22:38:50.861494 bvg-python-1.0.0/bvg_python/
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)       24 2024-05-19 22:31:22.000000 bvg-python-1.0.0/bvg_python/__init__.py
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)     6407 2024-05-19 22:17:05.000000 bvg-python-1.0.0/bvg_python/bvg.py
-drwxrwxr-x   0 kpwde     (1000) kpwde     (1000)        0 2024-05-19 22:38:50.861494 bvg-python-1.0.0/bvg_python.egg-info/
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)     7645 2024-05-19 22:38:50.000000 bvg-python-1.0.0/bvg_python.egg-info/PKG-INFO
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)      228 2024-05-19 22:38:50.000000 bvg-python-1.0.0/bvg_python.egg-info/SOURCES.txt
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)        1 2024-05-19 22:38:50.000000 bvg-python-1.0.0/bvg_python.egg-info/dependency_links.txt
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)        9 2024-05-19 22:38:50.000000 bvg-python-1.0.0/bvg_python.egg-info/requires.txt
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)       11 2024-05-19 22:38:50.000000 bvg-python-1.0.0/bvg_python.egg-info/top_level.txt
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)       38 2024-05-19 22:38:50.861494 bvg-python-1.0.0/setup.cfg
--rw-rw-r--   0 kpwde     (1000) kpwde     (1000)      700 2024-05-19 22:38:34.000000 bvg-python-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:25:40.729220 bvg_python-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-19 23:25:36.000000 bvg_python-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-19 23:25:40.729220 bvg_python-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-19 23:25:36.000000 bvg_python-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:25:40.729220 bvg_python-1.0.2/bvg_python/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 23:25:36.000000 bvg_python-1.0.2/bvg_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-19 23:25:36.000000 bvg_python-1.0.2/bvg_python/bvg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:25:40.729220 bvg_python-1.0.2/bvg_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-19 23:25:40.000000 bvg_python-1.0.2/bvg_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-19 23:25:40.000000 bvg_python-1.0.2/bvg_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 23:25:40.000000 bvg_python-1.0.2/bvg_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 23:25:40.000000 bvg_python-1.0.2/bvg_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 23:25:40.000000 bvg_python-1.0.2/bvg_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 23:25:40.729220 bvg_python-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-19 23:25:36.000000 bvg_python-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:25:40.729220 bvg_python-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-19 23:25:36.000000 bvg_python-1.0.2/tests/test_bvg.py
```

### Comparing `bvg-python-1.0.0/README.md` & `bvg_python-1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,44 @@
+Metadata-Version: 2.1
+Name: bvg-python
+Version: 1.0.2
+Summary: Python wrapper for the BVG (Berliner Verkehrsbetriebe) public transportation REST API
+Home-page: https://github.com/tlieshoff/bvg-python
+Author: Tobias Lieshoff
+Author-email: me@tobias-lieshoff.de
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
 # BVG Python API Wrapper
 
 This is a Python wrapper for the BVG (Berliner Verkehrsbetriebe) public transportation REST API. It provides an easy-to-use interface to interact with the BVG API and fetch transportation data such as journeys, stops, departures, nearby locations, and reachable stops.
 
 ## Features
 
 - Fetch journeys between two locations.
 - Get information about specific stops.
 - Get departures from specific stops.
 - Get nearby locations based on latitude and longitude.
 - Get reachable stops from a specific location within a certain time frame.
 
 ## Installation
 
+You can install the package directly from PyPI:
+
+```sh
+pip install bvg-python
+```
+
+Alternatively, you can clone the repository and install the dependencies manually:
+
 1. Clone the repository:
     ```sh
     git clone https://github.com/tlieshoff/bvg-python.git
     cd bvg-python
     ```
 
 2. Set up a virtual environment and activate it:
@@ -32,16 +55,14 @@
 ## Usage
 
 ### Example Script
 
 An example script (`examples/example.py`) is provided to demonstrate the usage of the BVG API wrapper.
 
 ```python
-# examples/example.py
-
 from bvg_python.bvg import BVGApi
 import requests
 import time
 
 def fetch_with_retries(api_call, retries=3, delay=2):
     for i in range(retries):
         try:
@@ -60,23 +81,14 @@
     print("Fetching journey from Alexanderplatz to Rosa-Luxemburg-Platz...")
     journey = fetch_with_retries(lambda: api.get_journeys('S+U Alexanderplatz', 'U Rosa-Luxemburg-Platz'))
     if journey:
         print("Journey Details:", journey)
     else:
         print("No journey details available after retries.")
 
-    # Attempt to fetch journey with different locations as a fallback
-    if not journey:
-        print("\nAttempting alternative journey from Alexanderplatz to Potsdamer Platz...")
-        journey_alt = fetch_with_retries(lambda: api.get_journeys('S+U Alexanderplatz', 'S+U Potsdamer Platz'))
-        if journey_alt:
-            print("Alternative Journey Details:", journey_alt)
-        else:
-            print("No alternative journey details available after retries.")
-
     # Example 2: Get information about a specific stop (Alexanderplatz)
     print("\nFetching stop information for Alexanderplatz...")
     try:
         stop_info = api.get_stop('900100003')
         if stop_info:
             print("Stop Information:", stop_info)
         else:
@@ -115,67 +127,19 @@
         else:
             print("No reachable stops available.")
     except requests.exceptions.RequestException as e:
         print(f"Error fetching reachable stops: {e}")
 
 if __name__ == "__main__":
     main()
-```
-
-### API Methods
-
-#### `get_journeys(from_location, to_location)`
-
-Fetches journeys between two locations.
-
-- **Parameters:**
-  - `from_location` (str): The starting location.
-  - `to_location` (str): The destination location.
-
-- **Returns:** Journey details (JSON).
-
-#### `get_stop(stop_id)`
 
-Fetches information about a specific stop.
-
-- **Parameters:**
-  - `stop_id` (str): The ID of the stop.
-
-- **Returns:** Stop details (JSON).
-
-#### `get_departures(stop_id)`
-
-Fetches departures from a specific stop.
-
-- **Parameters:**
-  - `stop_id` (str): The ID of the stop.
-
-- **Returns:** Departure details (JSON).
-
-#### `get_nearby_locations(latitude, longitude)`
-
-Fetches nearby locations based on latitude and longitude.
-
-- **Parameters:**
-  - `latitude` (float): The latitude of the location.
-  - `longitude` (float): The longitude of the location.
-
-- **Returns:** Nearby locations (JSON).
-
-#### `get_reachable_stops(latitude, longitude, address)`
-
-Fetches reachable stops from a specific location within a certain time frame.
+```
 
-- **Parameters:**
-  - `latitude` (float): The latitude of the location.
-  - `longitude` (float): The longitude of the location.
-  - `address` (str): The address of the location.
+### More Information
 
-- **Returns:** Reachable stops (JSON).
+For more detailed information about the BVG API, you can visit the [API documentation](https://v6.bvg.transport.rest).
 
 ## License
 
-This project is licensed under the MIT License. See the LICENSE file for more details.
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ---
-
-For more information, refer to the official [BVG API documentation](https://v6.bvg.transport.rest/).
```

### Comparing `bvg-python-1.0.0/bvg_python/bvg.py` & `bvg_python-1.0.2/bvg_python/bvg.py`

 * *Files identical despite different names*

### Comparing `bvg-python-1.0.0/setup.py` & `bvg_python-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bvg-python',
-    version='1.0.0',
+    version='1.0.2',
     description='Python wrapper for the BVG (Berliner Verkehrsbetriebe) public transportation REST API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Tobias Lieshoff',
     author_email='me@tobias-lieshoff.de',
     url='https://github.com/tlieshoff/bvg-python',
     packages=find_packages(),
```


# Comparing `tmp/sdkfabric_starwars-0.1.0.tar.gz` & `tmp/sdkfabric_starwars-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_starwars-0.1.0.tar", last modified: Mon May 20 14:45:20 2024, max compression
+gzip compressed data, was "sdkfabric_starwars-0.1.1.tar", last modified: Mon May 20 15:28:37 2024, max compression
```

## Comparing `sdkfabric_starwars-0.1.0.tar` & `sdkfabric_starwars-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:45:20.983334 sdkfabric_starwars-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-20 14:45:20.983334 sdkfabric_starwars-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:45:20.983334 sdkfabric_starwars-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:45:20.979334 sdkfabric_starwars-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:45:20.983334 sdkfabric_starwars-0.1.0/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/film.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/film_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/film_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/people.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/people_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/people_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/planet.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/planet_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/planet_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/specie.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/specie_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/specie_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/starship.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/starship_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/starship_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/vehicle_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 14:45:17.000000 sdkfabric_starwars-0.1.0/src/sdk/vehicle_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:45:20.983334 sdkfabric_starwars-0.1.0/src/sdkfabric_starwars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-20 14:45:20.000000 sdkfabric_starwars-0.1.0/src/sdkfabric_starwars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-20 14:45:20.000000 sdkfabric_starwars-0.1.0/src/sdkfabric_starwars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:45:20.000000 sdkfabric_starwars-0.1.0/src/sdkfabric_starwars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 14:45:20.000000 sdkfabric_starwars-0.1.0/src/sdkfabric_starwars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 14:45:20.000000 sdkfabric_starwars-0.1.0/src/sdkfabric_starwars.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:28:37.130717 sdkfabric_starwars-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/film.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/film_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/film_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/people.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/people_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/people_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/planet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/planet_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/planet_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/specie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/specie_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/specie_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/starship.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/starship_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/starship_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/vehicle_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/vehicle_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/top_level.txt
```

### Comparing `sdkfabric_starwars-0.1.0/LICENSE` & `sdkfabric_starwars-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/PKG-INFO` & `sdkfabric_starwars-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-starwars
-Version: 0.1.0
+Version: 0.1.1
 Summary: Starwars Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/starwars-python
 Project-URL: Issues, https://github.com/sdk-fabric/starwars-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_starwars-0.1.0/README.md` & `sdkfabric_starwars-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/pyproject.toml` & `sdkfabric_starwars-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-starwars"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Starwars Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/client.py` & `sdkfabric_starwars-0.1.1/src/sdk/client.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/collection.py` & `sdkfabric_starwars-0.1.1/src/sdk/collection.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/film.py` & `sdkfabric_starwars-0.1.1/src/sdk/film.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/film_tag.py` & `sdkfabric_starwars-0.1.1/src/sdk/film_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/people.py` & `sdkfabric_starwars-0.1.1/src/sdk/people.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/people_tag.py` & `sdkfabric_starwars-0.1.1/src/sdk/people_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/planet.py` & `sdkfabric_starwars-0.1.1/src/sdk/planet.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/planet_tag.py` & `sdkfabric_starwars-0.1.1/src/sdk/planet_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/specie.py` & `sdkfabric_starwars-0.1.1/src/sdk/specie.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/specie_tag.py` & `sdkfabric_starwars-0.1.1/src/sdk/specie_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/starship.py` & `sdkfabric_starwars-0.1.1/src/sdk/starship.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/starship_tag.py` & `sdkfabric_starwars-0.1.1/src/sdk/starship_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/vehicle.py` & `sdkfabric_starwars-0.1.1/src/sdk/vehicle.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdk/vehicle_tag.py` & `sdkfabric_starwars-0.1.1/src/sdk/vehicle_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.0/src/sdkfabric_starwars.egg-info/PKG-INFO` & `sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-starwars
-Version: 0.1.0
+Version: 0.1.1
 Summary: Starwars Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/starwars-python
 Project-URL: Issues, https://github.com/sdk-fabric/starwars-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_starwars-0.1.0/src/sdkfabric_starwars.egg-info/SOURCES.txt` & `sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/sdk/film_tag.py
 src/sdk/people.py
 src/sdk/people_collection.py
 src/sdk/people_tag.py
 src/sdk/planet.py
 src/sdk/planet_collection.py
 src/sdk/planet_tag.py
+src/sdk/root.py
 src/sdk/specie.py
 src/sdk/specie_collection.py
 src/sdk/specie_tag.py
 src/sdk/starship.py
 src/sdk/starship_collection.py
 src/sdk/starship_tag.py
 src/sdk/vehicle.py
```


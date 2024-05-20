# Comparing `tmp/gmaps_avoid_swiss-0.1.8.tar.gz` & `tmp/gmaps_avoid_swiss-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmaps_avoid_swiss-0.1.8.tar", last modified: Thu Apr 25 11:47:51 2024, max compression
+gzip compressed data, was "gmaps_avoid_swiss-0.1.9.tar", last modified: Mon May 20 06:46:12 2024, max compression
```

## Comparing `gmaps_avoid_swiss-0.1.8.tar` & `gmaps_avoid_swiss-0.1.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/AUTHORS.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/CONTRIBUTING.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/HISTORY.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/LICENSE
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/MANIFEST.in
--rw-r--r--   0 gregor    (1000) gregor    (1000)     2875 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1844 2024-04-22 16:54:22.000000 gmaps_avoid_swiss-0.1.8/README.rst
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.731775 gmaps_avoid_swiss-0.1.8/docs/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/Makefile
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.731775 gmaps_avoid_swiss-0.1.8/docs/_build/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.731775 gmaps_avoid_swiss-0.1.8/docs/_build/html/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/docs/_build/html/_static/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      286 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.8/docs/_build/html/_static/file.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.8/docs/_build/html/_static/minus.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.8/docs/_build/html/_static/plus.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/authors.rst
--rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4934 2024-04-21 02:19:23.000000 gmaps_avoid_swiss-0.1.8/docs/conf.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/contributing.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1152 2024-04-20 18:21:23.000000 gmaps_avoid_swiss-0.1.8/docs/geos.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      881 2024-04-22 16:34:26.000000 gmaps_avoid_swiss-0.1.8/docs/gmaps_avoid_swiss.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/history.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      343 2024-04-21 02:19:08.000000 gmaps_avoid_swiss-0.1.8/docs/index.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/installation.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/make.bat
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-22 16:34:26.000000 gmaps_avoid_swiss-0.1.8/docs/modules.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/docs/readme.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     2453 2024-04-22 17:01:53.000000 gmaps_avoid_swiss-0.1.8/docs/usage.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1449 2024-04-25 11:43:00.000000 gmaps_avoid_swiss-0.1.8/pyproject.toml
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/setup.cfg
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1081 2024-04-25 11:43:00.000000 gmaps_avoid_swiss-0.1.8/setup.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.731775 gmaps_avoid_swiss-0.1.8/src/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      307 2024-04-25 11:43:00.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      674 2024-04-20 16:51:38.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/client.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/data/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)    17771 2024-04-20 19:48:38.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/data/switzerland.geojson
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     4506 2024-04-25 11:42:00.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/geo_check.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     7588 2024-04-25 11:39:10.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/routes.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     2540 2024-04-20 16:57:41.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/waypoints.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/
--rw-r--r--   0 gregor    (1000) gregor    (1000)     2875 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      979 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       76 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/requires.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-25 11:47:51.000000 gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/top_level.txt
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-25 11:47:51.735776 gmaps_avoid_swiss-0.1.8/tests/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.8/tests/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1383 2024-04-21 03:10:41.000000 gmaps_avoid_swiss-0.1.8/tests/test_geo_check.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1460 2024-04-21 03:00:26.000000 gmaps_avoid_swiss-0.1.8/tests/test_gmaps_avoid_swiss.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1550 2024-04-21 03:19:07.000000 gmaps_avoid_swiss-0.1.8/tests/test_routes.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1202 2024-04-19 19:57:47.000000 gmaps_avoid_swiss-0.1.8/tests/test_waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/AUTHORS.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/CONTRIBUTING.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/HISTORY.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/LICENSE
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/MANIFEST.in
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2926 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1895 2024-05-20 06:35:31.000000 gmaps_avoid_swiss-0.1.9/README.rst
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/docs/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/docs/Makefile
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.243569 gmaps_avoid_swiss-0.1.9/docs/_build/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.243569 gmaps_avoid_swiss-0.1.9/docs/_build/html/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/docs/_build/html/_static/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      286 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.9/docs/_build/html/_static/file.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.9/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.9/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/docs/authors.rst
+-rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4934 2024-04-21 02:19:23.000000 gmaps_avoid_swiss-0.1.9/docs/conf.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/docs/contributing.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1152 2024-04-20 18:21:23.000000 gmaps_avoid_swiss-0.1.9/docs/geos.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      881 2024-04-22 16:34:26.000000 gmaps_avoid_swiss-0.1.9/docs/gmaps_avoid_swiss.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/docs/history.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      343 2024-04-21 02:19:08.000000 gmaps_avoid_swiss-0.1.9/docs/index.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/docs/installation.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/docs/make.bat
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-22 16:34:26.000000 gmaps_avoid_swiss-0.1.9/docs/modules.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/docs/readme.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     2453 2024-04-22 17:01:53.000000 gmaps_avoid_swiss-0.1.9/docs/usage.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1449 2024-05-20 06:35:58.000000 gmaps_avoid_swiss-0.1.9/pyproject.toml
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/setup.cfg
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1081 2024-05-20 06:35:58.000000 gmaps_avoid_swiss-0.1.9/setup.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.243569 gmaps_avoid_swiss-0.1.9/src/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      307 2024-05-20 06:35:59.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      674 2024-04-20 16:51:38.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/client.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/data/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)    17771 2024-04-20 19:48:38.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/data/switzerland.geojson
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     4506 2024-05-20 06:32:27.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/geo_check.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     8893 2024-05-20 06:30:37.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/routes.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     2540 2024-04-20 16:57:41.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss.egg-info/
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     2926 2024-05-20 06:46:12.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss.egg-info/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      979 2024-05-20 06:46:12.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-05-20 06:46:12.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       76 2024-05-20 06:46:12.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss.egg-info/requires.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-05-20 06:46:12.000000 gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss.egg-info/top_level.txt
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-05-20 06:46:12.247569 gmaps_avoid_swiss-0.1.9/tests/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.9/tests/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1383 2024-04-21 03:10:41.000000 gmaps_avoid_swiss-0.1.9/tests/test_geo_check.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1460 2024-04-21 03:00:26.000000 gmaps_avoid_swiss-0.1.9/tests/test_gmaps_avoid_swiss.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1550 2024-04-21 03:19:07.000000 gmaps_avoid_swiss-0.1.9/tests/test_routes.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1202 2024-04-19 19:57:47.000000 gmaps_avoid_swiss-0.1.9/tests/test_waypoints.py
```

### Comparing `gmaps_avoid_swiss-0.1.8/CONTRIBUTING.rst` & `gmaps_avoid_swiss-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/LICENSE` & `gmaps_avoid_swiss-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/PKG-INFO` & `gmaps_avoid_swiss-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmaps_avoid_swiss
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 Home-page: https://github.com/xbencat/gmaps_avoid_swiss
 Author: Gregor Bencat
 Author-email: Gregor Bencat <bencat.gregor@gmail.com>
 Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
@@ -52,16 +52,16 @@
 For installation instructions and more details, please refer to `Geos <geos.html>`_ page.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
-* Avoids routing through Switzerland by dynamically selecting alternative cities
-  - If the initial route intersects with Switzerland, the system optimizes the route by selecting intermediate cities to avoid crossing Swiss borders
+* Avoids routing through Switzerland by trying alternative routes or dynamically selecting alternative cities
+  - If the initial route or alternative routes intersects with Switzerland, the system optimizes the route by selecting intermediate cities to avoid crossing Swiss borders
   - The cities are prioritized based on their proximity to the intersection points with Switzerland
   - The system iteratively tries different cities until a route that doesn't pass through Switzerland is found
   - If no valid route is found after exhausting all city options, the system falls back to the original route
 * Right now its only possible to use address in format :code:`{"lat": 48.5734, "lng": 7.7521}`
 
 To-Do List
 ----------
```

### Comparing `gmaps_avoid_swiss-0.1.8/README.rst` & `gmaps_avoid_swiss-0.1.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 For installation instructions and more details, please refer to `Geos <geos.html>`_ page.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
-* Avoids routing through Switzerland by dynamically selecting alternative cities
-  - If the initial route intersects with Switzerland, the system optimizes the route by selecting intermediate cities to avoid crossing Swiss borders
+* Avoids routing through Switzerland by trying alternative routes or dynamically selecting alternative cities
+  - If the initial route or alternative routes intersects with Switzerland, the system optimizes the route by selecting intermediate cities to avoid crossing Swiss borders
   - The cities are prioritized based on their proximity to the intersection points with Switzerland
   - The system iteratively tries different cities until a route that doesn't pass through Switzerland is found
   - If no valid route is found after exhausting all city options, the system falls back to the original route
 * Right now its only possible to use address in format :code:`{"lat": 48.5734, "lng": 7.7521}`
 
 To-Do List
 ----------
```

### Comparing `gmaps_avoid_swiss-0.1.8/docs/Makefile` & `gmaps_avoid_swiss-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/docs/conf.py` & `gmaps_avoid_swiss-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/docs/geos.rst` & `gmaps_avoid_swiss-0.1.9/docs/geos.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/docs/gmaps_avoid_swiss.rst` & `gmaps_avoid_swiss-0.1.9/docs/gmaps_avoid_swiss.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/docs/installation.rst` & `gmaps_avoid_swiss-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/docs/make.bat` & `gmaps_avoid_swiss-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/docs/usage.rst` & `gmaps_avoid_swiss-0.1.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/pyproject.toml` & `gmaps_avoid_swiss-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gmaps_avoid_swiss"
-version = "0.1.8"
+version = "0.1.9"
 description = "A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland."
 readme = "README.rst"
 authors = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
 ]
 maintainers = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
```

### Comparing `gmaps_avoid_swiss-0.1.8/setup.py` & `gmaps_avoid_swiss-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gmaps_avoid_swiss',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/xbencat/gmaps_avoid_swiss',
     license='MIT',
     author='Gregor Bencat',
     author_email='bencat.gregor@gmail.com',
     description='A Python package that customizes Google Maps routing to avoid Swiss routes.',
```

### Comparing `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/client.py` & `gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/client.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/data/switzerland.geojson` & `gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/data/switzerland.geojson`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/geo_check.py` & `gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/geo_check.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/routes.py` & `gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,18 @@
 
         origin_waypoint = create_waypoint(origin)
         destination_waypoint = create_waypoint(destination)
 
         route_fields = self._merge_fields(extra_fields)
         field_mask = ",".join(route_fields)
 
-        request = ComputeRoutesRequest(origin=origin_waypoint, destination=destination_waypoint)
+        request = ComputeRoutesRequest(
+            origin=origin_waypoint,
+            destination=destination_waypoint,
+        )
 
         if self._is_any_location_inside_swiss([origin, destination]):
             return self._perform_route_computation(request, field_mask)
         else:
             return self._handle_routing_around_swiss(request, field_mask)
 
     def _is_any_location_inside_swiss(self, locations: list) -> bool:
@@ -110,30 +113,36 @@
         except Exception as error:
             raise Exception(f"An error occurred: {error}")
 
     def _handle_routing_around_swiss(self, request: ComputeRoutesRequest,
                                      field_mask: str) -> routing_v2.ComputeRoutesResponse:
         """
         Handle routing when both locations are outside Switzerland but need to check if the route goes through
-        Switzerland.
+        Switzerland. If it does, we try alternative routes first, then reroute via common cities.
 
         :param request: The ComputeRoutesRequest object.
         :type request: ComputeRoutesRequest
         :param field_mask: Field mask for the Google Maps Routing API.
         :type field_mask: str
         :return: The response from the routing API.
         :rtype: routing_v2.ComputeRoutesResponse
         """
 
         response = self._perform_route_computation(request, field_mask)
         intersection = self.geo_checker.does_route_cross_swiss(response.routes[0].polyline)
 
         if intersection:
+            alternative_response = self._try_alternative_routes(request, field_mask)
+
+            if alternative_response:
+                return alternative_response
+
             self.geo_checker.sort_cities_by_distance(intersection)
             response = self._reroute_route(request, field_mask)
+
         return response
 
     def _reroute_route(self, request: ComputeRoutesRequest, field_mask: str) -> routing_v2.ComputeRoutesResponse:
         """
         Reroute the request through alternative cities to avoid crossing Switzerland.
 
         :param request: The ComputeRoutesRequest object containing the origin and destination.
@@ -170,11 +179,34 @@
         :rtype: ComputeRoutesRequest
         """
         via = create_waypoint(city)
 
         updated_request = ComputeRoutesRequest(
             origin=request.origin,
             destination=request.destination,
-            intermediates=[via]
+            intermediates=[via],
         )
 
         return updated_request
+
+    def _try_alternative_routes(self, request: ComputeRoutesRequest,
+                                field_mask: str) -> routing_v2.ComputeRoutesResponse | None:
+        """
+        Try computing alternative routes to see if any avoid crossing Switzerland.
+
+        :param request: The ComputeRoutesRequest object.
+        :type request: ComputeRoutesRequest
+        :param field_mask: Field mask for the Google Maps Routing API.
+        :type field_mask: str
+        :return: The response from the routing API, if a valid alternative is found.
+        :rtype: routing_v2.ComputeRoutesResponse
+        """
+        request.compute_alternative_routes = True
+
+        response = self._perform_route_computation(request, field_mask)
+        for route in response.routes:
+            if not self.geo_checker.does_route_cross_swiss(route.polyline):
+                valid_response = routing_v2.ComputeRoutesResponse()
+                valid_response.routes.append(route)
+                return valid_response
+
+        return None
```

### Comparing `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss/waypoints.py` & `gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss/waypoints.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/PKG-INFO` & `gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmaps-avoid-swiss
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 Home-page: https://github.com/xbencat/gmaps_avoid_swiss
 Author: Gregor Bencat
 Author-email: Gregor Bencat <bencat.gregor@gmail.com>
 Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
@@ -52,16 +52,16 @@
 For installation instructions and more details, please refer to `Geos <geos.html>`_ page.
 
 
 Features
 --------
 
 * Calculates duration, transit time, and encoded path from origin to destination
-* Avoids routing through Switzerland by dynamically selecting alternative cities
-  - If the initial route intersects with Switzerland, the system optimizes the route by selecting intermediate cities to avoid crossing Swiss borders
+* Avoids routing through Switzerland by trying alternative routes or dynamically selecting alternative cities
+  - If the initial route or alternative routes intersects with Switzerland, the system optimizes the route by selecting intermediate cities to avoid crossing Swiss borders
   - The cities are prioritized based on their proximity to the intersection points with Switzerland
   - The system iteratively tries different cities until a route that doesn't pass through Switzerland is found
   - If no valid route is found after exhausting all city options, the system falls back to the original route
 * Right now its only possible to use address in format :code:`{"lat": 48.5734, "lng": 7.7521}`
 
 To-Do List
 ----------
```

### Comparing `gmaps_avoid_swiss-0.1.8/src/gmaps_avoid_swiss.egg-info/SOURCES.txt` & `gmaps_avoid_swiss-0.1.9/src/gmaps_avoid_swiss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/tests/test_geo_check.py` & `gmaps_avoid_swiss-0.1.9/tests/test_geo_check.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/tests/test_gmaps_avoid_swiss.py` & `gmaps_avoid_swiss-0.1.9/tests/test_gmaps_avoid_swiss.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/tests/test_routes.py` & `gmaps_avoid_swiss-0.1.9/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.8/tests/test_waypoints.py` & `gmaps_avoid_swiss-0.1.9/tests/test_waypoints.py`

 * *Files identical despite different names*


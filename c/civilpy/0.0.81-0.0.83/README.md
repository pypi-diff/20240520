# Comparing `tmp/civilpy-0.0.81.tar.gz` & `tmp/civilpy-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.81.tar", last modified: Wed May  8 03:53:21 2024, max compression
+gzip compressed data, was "civilpy-0.0.83.tar", last modified: Mon May 20 04:17:14 2024, max compression
```

## Comparing `civilpy-0.0.81.tar` & `civilpy-0.0.83.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.297059 civilpy-0.0.81/
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-08 14:57:28.000000 civilpy-0.0.81/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6696 2024-05-08 03:53:21.293059 civilpy-0.0.81/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4397 2024-03-08 14:57:28.000000 civilpy-0.0.81/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 03:53:21.297059 civilpy-0.0.81/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-08 00:47:47.000000 civilpy-0.0.81/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.285059 civilpy-0.0.81/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-08 00:47:47.000000 civilpy-0.0.81/src/civilpy/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/construction/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/construction/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/environmental/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/environmental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/general/
--rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-27 10:49:10.000000 civilpy-0.0.81/src/civilpy/general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/general/database_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/gis.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/kml_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/math.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/general/microstation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     9875 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/general/photos.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/physics.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/general/plan_development.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/general/pointclouds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/geotechnical/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/geotechnical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/state/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.289059 civilpy-0.0.81/src/civilpy/state/ohio/
--rw-rw-rw-   0 root         (0) root         (0)     2607 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/D6_file_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42166 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/dot.py
--rw-rw-rw-   0 root         (0) root         (0)    16531 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/search_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    91957 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/state/ohio/snbi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy/structural/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/structural/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14167 2024-04-04 19:12:50.000000 civilpy-0.0.81/src/civilpy/structural/arema.py
--rw-rw-rw-   0 root         (0) root         (0)    20863 2024-04-04 19:12:50.000000 civilpy-0.0.81/src/civilpy/structural/beam_bending.py
--rw-rw-rw-   0 root         (0) root         (0)     8467 2024-04-11 05:46:12.000000 civilpy-0.0.81/src/civilpy/structural/midas.py
--rw-rw-rw-   0 root         (0) root         (0)    75517 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/structural/rail_tpg_design.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy/structural/res/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 03:52:54.000000 civilpy-0.0.81/src/civilpy/structural/res/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6559 2024-04-10 14:26:23.000000 civilpy-0.0.81/src/civilpy/structural/res/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    18307 2024-04-10 14:26:23.000000 civilpy-0.0.81/src/civilpy/structural/steel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy/transportation/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/transportation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy/water_resources/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/water_resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18050 2024-03-08 14:57:32.000000 civilpy-0.0.81/src/civilpy/water_resources/hydraulics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 03:53:21.293059 civilpy-0.0.81/src/civilpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6696 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1334 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      720 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-08 03:53:21.000000 civilpy-0.0.81/src/civilpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.284852 civilpy-0.0.83/
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-08 14:57:28.000000 civilpy-0.0.83/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6727 2024-05-20 04:17:14.284852 civilpy-0.0.83/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4397 2024-03-08 14:57:28.000000 civilpy-0.0.83/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 04:17:14.284852 civilpy-0.0.83/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3124 2024-05-20 02:06:05.000000 civilpy-0.0.83/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.276852 civilpy-0.0.83/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.280852 civilpy-0.0.83/src/civilpy/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-05-11 01:09:56.000000 civilpy-0.0.83/src/civilpy/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.280852 civilpy-0.0.83/src/civilpy/construction/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.280852 civilpy-0.0.83/src/civilpy/environmental/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/environmental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.280852 civilpy-0.0.83/src/civilpy/general/
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-03-27 10:49:10.000000 civilpy-0.0.83/src/civilpy/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/general/database_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:16:47.000000 civilpy-0.0.83/src/civilpy/general/gis.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:16:47.000000 civilpy-0.0.83/src/civilpy/general/kml_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:16:47.000000 civilpy-0.0.83/src/civilpy/general/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/general/microstation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2024-05-11 01:09:56.000000 civilpy-0.0.83/src/civilpy/general/pdf_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/general/photos.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:16:47.000000 civilpy-0.0.83/src/civilpy/general/physics.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:16:47.000000 civilpy-0.0.83/src/civilpy/general/plan_development.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/general/pointclouds.py
+-rw-rw-rw-   0 root         (0) root         (0)     4163 2024-05-20 02:06:05.000000 civilpy-0.0.83/src/civilpy/general/software.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.280852 civilpy-0.0.83/src/civilpy/geotechnical/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/geotechnical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.280852 civilpy-0.0.83/src/civilpy/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:16:47.000000 civilpy-0.0.83/src/civilpy/state/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.280852 civilpy-0.0.83/src/civilpy/state/ohio/
+-rw-rw-rw-   0 root         (0) root         (0)     2607 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/state/ohio/D6_file_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/state/ohio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42166 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/state/ohio/dot.py
+-rw-rw-rw-   0 root         (0) root         (0)    16531 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/state/ohio/search_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    91957 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/state/ohio/snbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.284852 civilpy-0.0.83/src/civilpy/structural/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:16:47.000000 civilpy-0.0.83/src/civilpy/structural/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14159 2024-05-11 01:09:56.000000 civilpy-0.0.83/src/civilpy/structural/arema.py
+-rw-rw-rw-   0 root         (0) root         (0)    20863 2024-04-04 19:12:50.000000 civilpy-0.0.83/src/civilpy/structural/beam_bending.py
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2024-04-11 05:46:12.000000 civilpy-0.0.83/src/civilpy/structural/midas.py
+-rw-rw-rw-   0 root         (0) root         (0)    75517 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/structural/rail_tpg_design.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.284852 civilpy-0.0.83/src/civilpy/structural/res/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 04:16:47.000000 civilpy-0.0.83/src/civilpy/structural/res/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6559 2024-04-10 14:26:23.000000 civilpy-0.0.83/src/civilpy/structural/res/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    18307 2024-04-10 14:26:23.000000 civilpy-0.0.83/src/civilpy/structural/steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.284852 civilpy-0.0.83/src/civilpy/transportation/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/transportation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.284852 civilpy-0.0.83/src/civilpy/water_resources/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/water_resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18050 2024-03-08 14:57:32.000000 civilpy-0.0.83/src/civilpy/water_resources/hydraulics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 04:17:14.284852 civilpy-0.0.83/src/civilpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6727 2024-05-20 04:17:14.000000 civilpy-0.0.83/src/civilpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-05-20 04:17:14.000000 civilpy-0.0.83/src/civilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 04:17:14.000000 civilpy-0.0.83/src/civilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-20 04:17:14.000000 civilpy-0.0.83/src/civilpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-20 04:17:14.000000 civilpy-0.0.83/src/civilpy.egg-info/top_level.txt
```

### Comparing `civilpy-0.0.81/LICENSE` & `civilpy-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/PKG-INFO` & `civilpy-0.0.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.81
+Version: 0.0.83
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -22,14 +22,15 @@
 Requires-Dist: Pillow>=10.2.0
 Requires-Dist: Pint>=0.12.2
 Requires-Dist: coverage>=7.1.0
 Requires-Dist: webdriver-manager>=3.8.5
 Requires-Dist: msedge-selenium-tools>=3.141.4
 Requires-Dist: Flask>=2.2.2
 Requires-Dist: PyPDF2>=3.0.1
+Requires-Dist: PyMuPDF>=1.23.7
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: sympy>=1.10.0
 Requires-Dist: sshtunnel>=0.4.0
 Requires-Dist: termcolor>=1.1.0
 Requires-Dist: icalendar>=4.0.7
 Requires-Dist: html5lib>=1.1
 Requires-Dist: geopandas>=0.6.2
```

#### html2text {}

```diff
@@ -1,56 +1,57 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.81 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.83 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Environment :: Console :: Curses
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy>=1.14.5 Requires-Dist: folium>=0.12.1 Requires-Dist: pandas>=1.1.5
 Requires-Dist: Pillow>=10.2.0 Requires-Dist: Pint>=0.12.2 Requires-Dist:
 coverage>=7.1.0 Requires-Dist: webdriver-manager>=3.8.5 Requires-Dist: msedge-
 selenium-tools>=3.141.4 Requires-Dist: Flask>=2.2.2 Requires-Dist:
-PyPDF2>=3.0.1 Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist:
-sympy>=1.10.0 Requires-Dist: sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0
-Requires-Dist: icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist:
-geopandas>=0.6.2 Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7
-Requires-Dist: natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist:
-requests>=2.28.2 Requires-Dist: pyntcloud>=0.3.1 Requires-Dist: openpyxl>=3.1.2
-Requires-Dist: tqdm>=4.65.0 Requires-Dist: pytesseract>=0.3.10 Requires-Dist:
-pytest>=7.4.1 Requires-Dist: pytest-cov>=4.1.0 Provides-Extra: full Requires-
-Dist: matplotlib>=3.6.3; extra == "full" Requires-Dist: selenium>=3.141.0;
-extra == "full" Requires-Dist: msedge-selenium-tools>=3.141.4; extra == "full"
-Requires-Dist: jupyter>=1.0.0; extra == "full" Requires-Dist: simplekml>=1.3.6;
-extra == "full" Requires-Dist: psycopg2-binary>=2.9.5; extra == "full"
-Requires-Dist: sympy>=1.10.0; extra == "full" Requires-Dist: latex>=0.7.0;
-extra == "full" Requires-Dist: laspy>=2.4.1; extra == "full" Requires-Dist:
-earthpy>=0.9.4; extra == "full" Requires-Dist: pymupdf>=1.22.3; extra == "full"
-Requires-Dist: pyodbc>=4.0.39; extra == "full" Requires-Dist: kivymd>=1.1.1;
-extra == "full" Requires-Dist: PyQt5>=5.15.9; extra == "full" Requires-Dist:
-tox>=4.11.1; extra == "full" # CivilPy ![PyPI - License](https://
-img.shields.io/pypi/l/civilpy) [Project badge][PyPI - Python Version][Project
-badge]![PyPI - Downloads](https://img.shields.io/pypi/dm/CivilPy) Code snippets
-for Civil Engineering related tasks ## About (Skip to the "Installation"
-section to start running code) Welcome to the CivilPy repository. This is a
-simple software package to give civil engineers cleaner access to some of the
-packages from the python ecosystem. The package is focused on civil engineering
-related tasks such as file management, pdf data extraction, image manipulation
-mapping and unit conversions. I did my best to make the user interface obvious
-to use and tried to keep the functionality compatible with tools available to
-the average Civil engineer. ## Intro This repository was created in order for
-me to gain a better understanding of software development work flows and how
-they can be re-purposed for civil engineering related tasks. This is by no
-means a comprehensive or even functional repository but is more a way for me to
-track my progress while learning more about another industry. There may
-occasionally be how-tos and other code posted here but this repository is not
-meant as tutorial or in depth explanation for how coding works. For those types
-of things I highly suggest you instead check _Y_o_u_t_u_b_e for general lessons or
-_S_t_a_c_k_ _O_v_e_r_f_l_o_w for specific issues. I highly recommend the _H_a_r_v_a_r_d_ _C_S_5_0_ _Y_o_u_T_u_b_e
+PyPDF2>=3.0.1 Requires-Dist: PyMuPDF>=1.23.7 Requires-Dist:
+beautifulsoup4>=4.11.1 Requires-Dist: sympy>=1.10.0 Requires-Dist:
+sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0 Requires-Dist:
+icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist: geopandas>=0.6.2
+Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7 Requires-Dist:
+natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist: requests>=2.28.2
+Requires-Dist: pyntcloud>=0.3.1 Requires-Dist: openpyxl>=3.1.2 Requires-Dist:
+tqdm>=4.65.0 Requires-Dist: pytesseract>=0.3.10 Requires-Dist: pytest>=7.4.1
+Requires-Dist: pytest-cov>=4.1.0 Provides-Extra: full Requires-Dist:
+matplotlib>=3.6.3; extra == "full" Requires-Dist: selenium>=3.141.0; extra ==
+"full" Requires-Dist: msedge-selenium-tools>=3.141.4; extra == "full" Requires-
+Dist: jupyter>=1.0.0; extra == "full" Requires-Dist: simplekml>=1.3.6; extra ==
+"full" Requires-Dist: psycopg2-binary>=2.9.5; extra == "full" Requires-Dist:
+sympy>=1.10.0; extra == "full" Requires-Dist: latex>=0.7.0; extra == "full"
+Requires-Dist: laspy>=2.4.1; extra == "full" Requires-Dist: earthpy>=0.9.4;
+extra == "full" Requires-Dist: pymupdf>=1.22.3; extra == "full" Requires-Dist:
+pyodbc>=4.0.39; extra == "full" Requires-Dist: kivymd>=1.1.1; extra == "full"
+Requires-Dist: PyQt5>=5.15.9; extra == "full" Requires-Dist: tox>=4.11.1; extra
+== "full" # CivilPy ![PyPI - License](https://img.shields.io/pypi/l/civilpy)
+[Project badge][PyPI - Python Version][Project badge]![PyPI - Downloads](https:
+//img.shields.io/pypi/dm/CivilPy) Code snippets for Civil Engineering related
+tasks ## About (Skip to the "Installation" section to start running code)
+Welcome to the CivilPy repository. This is a simple software package to give
+civil engineers cleaner access to some of the packages from the python
+ecosystem. The package is focused on civil engineering related tasks such as
+file management, pdf data extraction, image manipulation mapping and unit
+conversions. I did my best to make the user interface obvious to use and tried
+to keep the functionality compatible with tools available to the average Civil
+engineer. ## Intro This repository was created in order for me to gain a better
+understanding of software development work flows and how they can be re-
+purposed for civil engineering related tasks. This is by no means a
+comprehensive or even functional repository but is more a way for me to track
+my progress while learning more about another industry. There may occasionally
+be how-tos and other code posted here but this repository is not meant as
+tutorial or in depth explanation for how coding works. For those types of
+things I highly suggest you instead check _Y_o_u_t_u_b_e for general lessons or _S_t_a_c_k
+_O_v_e_r_f_l_o_w for specific issues. I highly recommend the _H_a_r_v_a_r_d_ _C_S_5_0_ _Y_o_u_T_u_b_e
 _C_h_a_n_n_e_l for conceptual level programming lessons or _C_o_r_e_y_M_S_'_s_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l
 for lessons in practical uses of programming. For an interesting somewhat
 working examples see the files `Useful Tricks and Tools.ipynb` and `NBI
 STandards - Conversion` files to have a better understanding of what function
 the DOT/SNBI files are performing. ## Installation Run the following code to
 install the package: ```bash $ pip install civilpy ``` ## Usage to check the
 package installed correctly, run: ```python from civilpy.structural.steel
```

### Comparing `civilpy-0.0.81/README.md` & `civilpy-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/setup.py` & `civilpy-0.0.83/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.81',
+    version='0.0.83',
     packages=find_packages('src', exclude=['test', 'Notebooks', 'secrets', 'docs', 'res']),
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
     license='MIT',
     py_modules=[
@@ -21,14 +21,15 @@
         "civilpy.general.math",
         "civilpy.general.microstation",
         "civilpy.general.pdf",
         "civilpy.general.photos",
         "civilpy.general.physics",
         "civilpy.general.plan_development",
         "civilpy.general.pointclouds",
+        "civilpy.general.software",
         "civilpy.structural.beam_bending",
         "civilpy.structural.search_tools",
         "civilpy.structural.steel",
         "civilpy.structural.midas",
         "civilpy.water_resources.hydraulics",
         "civilpy.CLI",
         "civilpy.kivy"
@@ -53,14 +54,15 @@
         "Pillow>=10.2.0",
         "Pint>=0.12.2",
         "coverage>=7.1.0",
         "webdriver-manager>=3.8.5",
         "msedge-selenium-tools>=3.141.4",
         "Flask>=2.2.2",
         "PyPDF2>=3.0.1",
+        "PyMuPDF>=1.23.7",
         "beautifulsoup4>=4.11.1",
         "sympy>=1.10.0",
         "sshtunnel>=0.4.0",
         "termcolor>=1.1.0",
         "icalendar>=4.0.7",
         "html5lib>=1.1",
         "geopandas>=0.6.2",
```

### Comparing `civilpy-0.0.81/src/civilpy/general/database_tools.py` & `civilpy-0.0.83/src/civilpy/general/database_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/general/microstation.py` & `civilpy-0.0.83/src/civilpy/general/microstation.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/general/photos.py` & `civilpy-0.0.83/src/civilpy/general/photos.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/state/ohio/D6_file_explorer.py` & `civilpy-0.0.83/src/civilpy/state/ohio/D6_file_explorer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/state/ohio/dot.py` & `civilpy-0.0.83/src/civilpy/state/ohio/dot.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/state/ohio/search_tools.py` & `civilpy-0.0.83/src/civilpy/state/ohio/search_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/state/ohio/snbi.py` & `civilpy-0.0.83/src/civilpy/state/ohio/snbi.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/structural/arema.py` & `civilpy-0.0.83/src/civilpy/structural/arema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from civilpy.structural.midas import get_elements_by_section_index, get_api_key, midas_api
 from civilpy.general import pint, units
 
-from src.civilpy.general import PrintColors
-from src.civilpy.structural.midas import analysis_results_request
+from civilpy.general import PrintColors
+from civilpy.structural.midas import analysis_results_request
 
 from pathlib import Path
 import pandas as pd
 import numpy as np
 import os
 
 future_ballast_depth = 6 * units('in')
```

### Comparing `civilpy-0.0.81/src/civilpy/structural/beam_bending.py` & `civilpy-0.0.83/src/civilpy/structural/beam_bending.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/structural/midas.py` & `civilpy-0.0.83/src/civilpy/structural/midas.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/structural/rail_tpg_design.py` & `civilpy-0.0.83/src/civilpy/structural/rail_tpg_design.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/structural/res/definitions.py` & `civilpy-0.0.83/src/civilpy/structural/res/definitions.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/structural/steel.py` & `civilpy-0.0.83/src/civilpy/structural/steel.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy/water_resources/hydraulics.py` & `civilpy-0.0.83/src/civilpy/water_resources/hydraulics.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.81/src/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.83/src/civilpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.81
+Version: 0.0.83
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -22,14 +22,15 @@
 Requires-Dist: Pillow>=10.2.0
 Requires-Dist: Pint>=0.12.2
 Requires-Dist: coverage>=7.1.0
 Requires-Dist: webdriver-manager>=3.8.5
 Requires-Dist: msedge-selenium-tools>=3.141.4
 Requires-Dist: Flask>=2.2.2
 Requires-Dist: PyPDF2>=3.0.1
+Requires-Dist: PyMuPDF>=1.23.7
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: sympy>=1.10.0
 Requires-Dist: sshtunnel>=0.4.0
 Requires-Dist: termcolor>=1.1.0
 Requires-Dist: icalendar>=4.0.7
 Requires-Dist: html5lib>=1.1
 Requires-Dist: geopandas>=0.6.2
```

#### html2text {}

```diff
@@ -1,56 +1,57 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.81 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.83 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Environment :: Console :: Curses
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy>=1.14.5 Requires-Dist: folium>=0.12.1 Requires-Dist: pandas>=1.1.5
 Requires-Dist: Pillow>=10.2.0 Requires-Dist: Pint>=0.12.2 Requires-Dist:
 coverage>=7.1.0 Requires-Dist: webdriver-manager>=3.8.5 Requires-Dist: msedge-
 selenium-tools>=3.141.4 Requires-Dist: Flask>=2.2.2 Requires-Dist:
-PyPDF2>=3.0.1 Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist:
-sympy>=1.10.0 Requires-Dist: sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0
-Requires-Dist: icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist:
-geopandas>=0.6.2 Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7
-Requires-Dist: natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist:
-requests>=2.28.2 Requires-Dist: pyntcloud>=0.3.1 Requires-Dist: openpyxl>=3.1.2
-Requires-Dist: tqdm>=4.65.0 Requires-Dist: pytesseract>=0.3.10 Requires-Dist:
-pytest>=7.4.1 Requires-Dist: pytest-cov>=4.1.0 Provides-Extra: full Requires-
-Dist: matplotlib>=3.6.3; extra == "full" Requires-Dist: selenium>=3.141.0;
-extra == "full" Requires-Dist: msedge-selenium-tools>=3.141.4; extra == "full"
-Requires-Dist: jupyter>=1.0.0; extra == "full" Requires-Dist: simplekml>=1.3.6;
-extra == "full" Requires-Dist: psycopg2-binary>=2.9.5; extra == "full"
-Requires-Dist: sympy>=1.10.0; extra == "full" Requires-Dist: latex>=0.7.0;
-extra == "full" Requires-Dist: laspy>=2.4.1; extra == "full" Requires-Dist:
-earthpy>=0.9.4; extra == "full" Requires-Dist: pymupdf>=1.22.3; extra == "full"
-Requires-Dist: pyodbc>=4.0.39; extra == "full" Requires-Dist: kivymd>=1.1.1;
-extra == "full" Requires-Dist: PyQt5>=5.15.9; extra == "full" Requires-Dist:
-tox>=4.11.1; extra == "full" # CivilPy ![PyPI - License](https://
-img.shields.io/pypi/l/civilpy) [Project badge][PyPI - Python Version][Project
-badge]![PyPI - Downloads](https://img.shields.io/pypi/dm/CivilPy) Code snippets
-for Civil Engineering related tasks ## About (Skip to the "Installation"
-section to start running code) Welcome to the CivilPy repository. This is a
-simple software package to give civil engineers cleaner access to some of the
-packages from the python ecosystem. The package is focused on civil engineering
-related tasks such as file management, pdf data extraction, image manipulation
-mapping and unit conversions. I did my best to make the user interface obvious
-to use and tried to keep the functionality compatible with tools available to
-the average Civil engineer. ## Intro This repository was created in order for
-me to gain a better understanding of software development work flows and how
-they can be re-purposed for civil engineering related tasks. This is by no
-means a comprehensive or even functional repository but is more a way for me to
-track my progress while learning more about another industry. There may
-occasionally be how-tos and other code posted here but this repository is not
-meant as tutorial or in depth explanation for how coding works. For those types
-of things I highly suggest you instead check _Y_o_u_t_u_b_e for general lessons or
-_S_t_a_c_k_ _O_v_e_r_f_l_o_w for specific issues. I highly recommend the _H_a_r_v_a_r_d_ _C_S_5_0_ _Y_o_u_T_u_b_e
+PyPDF2>=3.0.1 Requires-Dist: PyMuPDF>=1.23.7 Requires-Dist:
+beautifulsoup4>=4.11.1 Requires-Dist: sympy>=1.10.0 Requires-Dist:
+sshtunnel>=0.4.0 Requires-Dist: termcolor>=1.1.0 Requires-Dist:
+icalendar>=4.0.7 Requires-Dist: html5lib>=1.1 Requires-Dist: geopandas>=0.6.2
+Requires-Dist: fiona>=1.8.22 Requires-Dist: tifftools>=1.3.7 Requires-Dist:
+natsort>=8.2.0 Requires-Dist: html5lib>=1.1 Requires-Dist: requests>=2.28.2
+Requires-Dist: pyntcloud>=0.3.1 Requires-Dist: openpyxl>=3.1.2 Requires-Dist:
+tqdm>=4.65.0 Requires-Dist: pytesseract>=0.3.10 Requires-Dist: pytest>=7.4.1
+Requires-Dist: pytest-cov>=4.1.0 Provides-Extra: full Requires-Dist:
+matplotlib>=3.6.3; extra == "full" Requires-Dist: selenium>=3.141.0; extra ==
+"full" Requires-Dist: msedge-selenium-tools>=3.141.4; extra == "full" Requires-
+Dist: jupyter>=1.0.0; extra == "full" Requires-Dist: simplekml>=1.3.6; extra ==
+"full" Requires-Dist: psycopg2-binary>=2.9.5; extra == "full" Requires-Dist:
+sympy>=1.10.0; extra == "full" Requires-Dist: latex>=0.7.0; extra == "full"
+Requires-Dist: laspy>=2.4.1; extra == "full" Requires-Dist: earthpy>=0.9.4;
+extra == "full" Requires-Dist: pymupdf>=1.22.3; extra == "full" Requires-Dist:
+pyodbc>=4.0.39; extra == "full" Requires-Dist: kivymd>=1.1.1; extra == "full"
+Requires-Dist: PyQt5>=5.15.9; extra == "full" Requires-Dist: tox>=4.11.1; extra
+== "full" # CivilPy ![PyPI - License](https://img.shields.io/pypi/l/civilpy)
+[Project badge][PyPI - Python Version][Project badge]![PyPI - Downloads](https:
+//img.shields.io/pypi/dm/CivilPy) Code snippets for Civil Engineering related
+tasks ## About (Skip to the "Installation" section to start running code)
+Welcome to the CivilPy repository. This is a simple software package to give
+civil engineers cleaner access to some of the packages from the python
+ecosystem. The package is focused on civil engineering related tasks such as
+file management, pdf data extraction, image manipulation mapping and unit
+conversions. I did my best to make the user interface obvious to use and tried
+to keep the functionality compatible with tools available to the average Civil
+engineer. ## Intro This repository was created in order for me to gain a better
+understanding of software development work flows and how they can be re-
+purposed for civil engineering related tasks. This is by no means a
+comprehensive or even functional repository but is more a way for me to track
+my progress while learning more about another industry. There may occasionally
+be how-tos and other code posted here but this repository is not meant as
+tutorial or in depth explanation for how coding works. For those types of
+things I highly suggest you instead check _Y_o_u_t_u_b_e for general lessons or _S_t_a_c_k
+_O_v_e_r_f_l_o_w for specific issues. I highly recommend the _H_a_r_v_a_r_d_ _C_S_5_0_ _Y_o_u_T_u_b_e
 _C_h_a_n_n_e_l for conceptual level programming lessons or _C_o_r_e_y_M_S_'_s_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l
 for lessons in practical uses of programming. For an interesting somewhat
 working examples see the files `Useful Tricks and Tools.ipynb` and `NBI
 STandards - Conversion` files to have a better understanding of what function
 the DOT/SNBI files are performing. ## Installation Run the following code to
 install the package: ```bash $ pip install civilpy ``` ## Usage to check the
 package installed correctly, run: ```python from civilpy.structural.steel
```

### Comparing `civilpy-0.0.81/src/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.83/src/civilpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 src/civilpy/environmental/__init__.py
 src/civilpy/general/__init__.py
 src/civilpy/general/database_tools.py
 src/civilpy/general/gis.py
 src/civilpy/general/kml_tools.py
 src/civilpy/general/math.py
 src/civilpy/general/microstation.py
-src/civilpy/general/pdf.py
+src/civilpy/general/pdf_tools.py
 src/civilpy/general/photos.py
 src/civilpy/general/physics.py
 src/civilpy/general/plan_development.py
 src/civilpy/general/pointclouds.py
+src/civilpy/general/software.py
 src/civilpy/geotechnical/__init__.py
 src/civilpy/state/__init__.py
 src/civilpy/state/ohio/D6_file_explorer.py
 src/civilpy/state/ohio/__init__.py
 src/civilpy/state/ohio/dot.py
 src/civilpy/state/ohio/search_tools.py
 src/civilpy/state/ohio/snbi.py
```

### Comparing `civilpy-0.0.81/src/civilpy.egg-info/requires.txt` & `civilpy-0.0.83/src/civilpy.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Pillow>=10.2.0
 Pint>=0.12.2
 coverage>=7.1.0
 webdriver-manager>=3.8.5
 msedge-selenium-tools>=3.141.4
 Flask>=2.2.2
 PyPDF2>=3.0.1
+PyMuPDF>=1.23.7
 beautifulsoup4>=4.11.1
 sympy>=1.10.0
 sshtunnel>=0.4.0
 termcolor>=1.1.0
 icalendar>=4.0.7
 html5lib>=1.1
 geopandas>=0.6.2
```


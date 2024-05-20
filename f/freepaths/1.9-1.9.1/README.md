# Comparing `tmp/freepaths-1.9.tar.gz` & `tmp/freepaths-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freepaths-1.9.tar", last modified: Wed Feb 28 17:15:51 2024, max compression
+gzip compressed data, was "freepaths-1.9.1.tar", last modified: Mon May 20 02:43:29 2024, max compression
```

## Comparing `freepaths-1.9.tar` & `freepaths-1.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-02-28 17:15:51.456364 freepaths-1.9/
--rw-r--r--   0 r         (1000) r         (1000)     5602 2024-02-28 17:15:51.456364 freepaths-1.9/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     4731 2024-02-19 15:11:03.000000 freepaths-1.9/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-02-28 17:15:51.456364 freepaths-1.9/freepaths/
--rw-r--r--   0 r         (1000) r         (1000)     1036 2024-02-23 13:21:25.000000 freepaths-1.9/freepaths/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     3730 2023-12-24 09:53:08.000000 freepaths-1.9/freepaths/animation.py
--rw-r--r--   0 r         (1000) r         (1000)     9882 2024-02-28 16:46:29.000000 freepaths-1.9/freepaths/config.py
--rw-r--r--   0 r         (1000) r         (1000)    10196 2023-12-26 10:47:35.000000 freepaths-1.9/freepaths/data.py
--rw-r--r--   0 r         (1000) r         (1000)     2391 2024-02-28 13:21:43.000000 freepaths-1.9/freepaths/default_config.py
--rw-r--r--   0 r         (1000) r         (1000)     2603 2023-12-24 09:53:08.000000 freepaths-1.9/freepaths/flight.py
--rw-r--r--   0 r         (1000) r         (1000)    24249 2024-02-23 16:23:15.000000 freepaths-1.9/freepaths/holes.py
--rw-r--r--   0 r         (1000) r         (1000)     5014 2024-02-28 16:59:34.000000 freepaths-1.9/freepaths/main_mfp_sampling.py
--rw-r--r--   0 r         (1000) r         (1000)    10831 2024-02-28 13:21:43.000000 freepaths-1.9/freepaths/main_tracing.py
--rw-r--r--   0 r         (1000) r         (1000)    17720 2024-02-28 16:59:35.000000 freepaths-1.9/freepaths/maps.py
--rw-r--r--   0 r         (1000) r         (1000)     8851 2024-02-25 14:09:41.000000 freepaths-1.9/freepaths/materials.py
--rw-r--r--   0 r         (1000) r         (1000)      733 2023-12-24 09:53:08.000000 freepaths-1.9/freepaths/move.py
--rw-r--r--   0 r         (1000) r         (1000)     6599 2024-02-28 13:21:43.000000 freepaths-1.9/freepaths/output_info.py
--rw-r--r--   0 r         (1000) r         (1000)    22453 2024-02-28 16:06:17.000000 freepaths-1.9/freepaths/output_plots.py
--rw-r--r--   0 r         (1000) r         (1000)     1338 2024-02-22 15:38:59.000000 freepaths-1.9/freepaths/output_structure.py
--rw-r--r--   0 r         (1000) r         (1000)     5962 2024-02-26 21:08:38.000000 freepaths-1.9/freepaths/phonon.py
--rw-r--r--   0 r         (1000) r         (1000)      580 2023-12-24 09:53:08.000000 freepaths-1.9/freepaths/progress.py
--rw-r--r--   0 r         (1000) r         (1000)     2543 2023-12-24 09:53:08.000000 freepaths-1.9/freepaths/run_phonon.py
--rw-r--r--   0 r         (1000) r         (1000)     5599 2024-02-23 22:03:45.000000 freepaths-1.9/freepaths/scattering.py
--rw-r--r--   0 r         (1000) r         (1000)     9180 2024-02-19 10:46:43.000000 freepaths-1.9/freepaths/scattering_primitives.py
--rw-r--r--   0 r         (1000) r         (1000)    33139 2024-02-19 10:46:43.000000 freepaths-1.9/freepaths/scattering_semicircle.py
--rw-r--r--   0 r         (1000) r         (1000)     1651 2024-02-23 16:23:14.000000 freepaths-1.9/freepaths/scattering_types.py
--rw-r--r--   0 r         (1000) r         (1000)     1832 2024-02-25 14:01:45.000000 freepaths-1.9/freepaths/sources.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-02-28 17:15:51.456364 freepaths-1.9/freepaths.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     5602 2024-02-28 17:15:51.000000 freepaths-1.9/freepaths.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      791 2024-02-28 17:15:51.000000 freepaths-1.9/freepaths.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2024-02-28 17:15:51.000000 freepaths-1.9/freepaths.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       53 2024-02-28 17:15:51.000000 freepaths-1.9/freepaths.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       40 2024-02-28 17:15:51.000000 freepaths-1.9/freepaths.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)       10 2024-02-28 17:15:51.000000 freepaths-1.9/freepaths.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2023-12-24 09:53:08.000000 freepaths-1.9/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2024-02-28 17:15:51.456364 freepaths-1.9/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1451 2023-12-24 09:53:08.000000 freepaths-1.9/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-05-20 02:43:29.653206 freepaths-1.9.1/
+-rw-r--r--   0 r         (1000) r         (1000)     5604 2024-05-20 02:43:29.653206 freepaths-1.9.1/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     4731 2024-02-19 15:11:03.000000 freepaths-1.9.1/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-05-20 02:43:29.653206 freepaths-1.9.1/freepaths/
+-rw-r--r--   0 r         (1000) r         (1000)     1038 2024-05-20 02:43:16.000000 freepaths-1.9.1/freepaths/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     3730 2023-12-24 09:53:08.000000 freepaths-1.9.1/freepaths/animation.py
+-rw-r--r--   0 r         (1000) r         (1000)     9654 2024-03-05 13:15:31.000000 freepaths-1.9.1/freepaths/config.py
+-rw-r--r--   0 r         (1000) r         (1000)    10196 2023-12-26 10:47:35.000000 freepaths-1.9.1/freepaths/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     2391 2024-02-28 13:21:43.000000 freepaths-1.9.1/freepaths/default_config.py
+-rw-r--r--   0 r         (1000) r         (1000)     2603 2023-12-24 09:53:08.000000 freepaths-1.9.1/freepaths/flight.py
+-rw-r--r--   0 r         (1000) r         (1000)    24249 2024-02-23 16:23:15.000000 freepaths-1.9.1/freepaths/holes.py
+-rw-r--r--   0 r         (1000) r         (1000)     5038 2024-03-05 13:05:15.000000 freepaths-1.9.1/freepaths/main_mfp_sampling.py
+-rw-r--r--   0 r         (1000) r         (1000)    10855 2024-03-05 13:05:14.000000 freepaths-1.9.1/freepaths/main_tracing.py
+-rw-r--r--   0 r         (1000) r         (1000)    17720 2024-05-20 02:35:05.000000 freepaths-1.9.1/freepaths/maps.py
+-rw-r--r--   0 r         (1000) r         (1000)     8851 2024-02-25 14:09:41.000000 freepaths-1.9.1/freepaths/materials.py
+-rw-r--r--   0 r         (1000) r         (1000)      733 2023-12-24 09:53:08.000000 freepaths-1.9.1/freepaths/move.py
+-rw-r--r--   0 r         (1000) r         (1000)     6518 2024-03-05 10:24:43.000000 freepaths-1.9.1/freepaths/output_info.py
+-rw-r--r--   0 r         (1000) r         (1000)    22453 2024-02-28 16:06:17.000000 freepaths-1.9.1/freepaths/output_plots.py
+-rw-r--r--   0 r         (1000) r         (1000)     1338 2024-02-22 15:38:59.000000 freepaths-1.9.1/freepaths/output_structure.py
+-rw-r--r--   0 r         (1000) r         (1000)     5962 2024-02-26 21:08:38.000000 freepaths-1.9.1/freepaths/phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)      580 2023-12-24 09:53:08.000000 freepaths-1.9.1/freepaths/progress.py
+-rw-r--r--   0 r         (1000) r         (1000)     2543 2023-12-24 09:53:08.000000 freepaths-1.9.1/freepaths/run_phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)     5599 2024-02-23 22:03:45.000000 freepaths-1.9.1/freepaths/scattering.py
+-rw-r--r--   0 r         (1000) r         (1000)     9180 2024-02-19 10:46:43.000000 freepaths-1.9.1/freepaths/scattering_primitives.py
+-rw-r--r--   0 r         (1000) r         (1000)    33139 2024-02-19 10:46:43.000000 freepaths-1.9.1/freepaths/scattering_semicircle.py
+-rw-r--r--   0 r         (1000) r         (1000)     1651 2024-02-23 16:23:14.000000 freepaths-1.9.1/freepaths/scattering_types.py
+-rw-r--r--   0 r         (1000) r         (1000)     1832 2024-02-25 14:01:45.000000 freepaths-1.9.1/freepaths/sources.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2024-05-20 02:43:29.653206 freepaths-1.9.1/freepaths.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     5604 2024-05-20 02:43:29.000000 freepaths-1.9.1/freepaths.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      791 2024-05-20 02:43:29.000000 freepaths-1.9.1/freepaths.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2024-05-20 02:43:29.000000 freepaths-1.9.1/freepaths.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       53 2024-05-20 02:43:29.000000 freepaths-1.9.1/freepaths.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       40 2024-05-20 02:43:29.000000 freepaths-1.9.1/freepaths.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)       10 2024-05-20 02:43:29.000000 freepaths-1.9.1/freepaths.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2023-12-24 09:53:08.000000 freepaths-1.9.1/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2024-05-20 02:43:29.653206 freepaths-1.9.1/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1451 2023-12-24 09:53:08.000000 freepaths-1.9.1/setup.py
```

### Comparing `freepaths-1.9/PKG-INFO` & `freepaths-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.9
+Version: 1.9.1
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `freepaths-1.9/README.md` & `freepaths-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/__main__.py` & `freepaths-1.9.1/freepaths/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import colorama
 from colorama import Fore, Style
 
 import freepaths.main_tracing
 import freepaths.main_mfp_sampling
 
-__version__ = "1.9"
+__version__ = "1.9.1"
 
 colorama.init()
 
 # Parse user arguments:
 parser = argparse.ArgumentParser(
                 prog = 'FreePATHS',
                 description = 'Phonon Monte Carlo simulator',
```

### Comparing `freepaths-1.9/freepaths/animation.py` & `freepaths-1.9.1/freepaths/animation.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/config.py` & `freepaths-1.9.1/freepaths/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """
 Module that reads the user input file, provides default values,
 checks the validity of the parameters and converts the variables into enums
 """
 
 import sys
 import argparse
+import logging
 from colorama import Fore, Style
 
 from freepaths.sources import Distributions
 from freepaths.holes import *
 
 # Import a default input file:
 from freepaths.default_config import *
 
+# Start logging:
+logging.basicConfig(level=logging.WARNING, format=f"{Fore.RED}%(levelname)s:{Style.RESET_ALL} %(message)s",
+                    handlers=[logging.StreamHandler(), ])
 
 # Parse user arguments:
 WEBSITE = 'https://anufrievroman.gitbook.io/freepaths'
 parser = argparse.ArgumentParser(prog='FreePATHS', description='Monte Carlo simulator',
                                  epilog=f'For more information, visit: {WEBSITE}')
 parser.add_argument('input_file', nargs='?', default=None, help='The input file')
 parser.add_argument("-s", "--sampling", help="Run in MFP sampling mode", action="store_true")
 args = parser.parse_args()
 
 
 # If a file is provided, overwrite the default values:
 if args.input_file:
     exec(open(args.input_file, encoding='utf-8').read(), globals())
 else:
-    print(f"{Fore.RED}You provided no input file, so we will run a demo simulation:{Style.RESET_ALL}")
+    logging.warning("You provided no input file, so we will run a demo simulation:")
 
 
 class Config:
     """Class that contains all the settings for the simulation"""
 
     def __init__(self):
         """Initiate all the parameters from global variables"""
@@ -115,121 +119,113 @@
 
         # Distributions:
         valid_distributions =[member.name.lower() for member in Distributions]
         for source in self.phonon_sources:
             if source.angle_distribution in valid_distributions:
                 source.angle_distribution = Distributions[source.angle_distribution.upper()]
             else:
-                print("ERROR: Parameter angle_distribution of a source is not set correctly.")
-                print("The angle_distribution should be one of the following:")
-                print(*valid_distributions, sep = ", ")
+                logging.error("Parameter angle_distribution of a source is not set correctly.")
                 sys.exit()
 
 
     def check_parameter_validity(self):
         """Check if various parameters are valid"""
         if self.number_of_phonons < self.output_trajectories_of_first:
             self.output_trajectories_of_first = self.number_of_phonons
 
         if self.number_of_timeframes <= self.number_of_stabilization_timeframes:
-            print("ERROR: Parameter NUMBER_OF_STABILIZATION_TIMEFRAMES exceeds or equal to NUMBER_OF_TIMEFRAMES.")
-            print("We need to have at least one timeframe after NUMBER_OF_STABILIZATION_TIMEFRAMES to measure the thermal conductivity.")
+            logging.error("Parameter NUMBER_OF_STABILIZATION_TIMEFRAMES exceeds or equal to NUMBER_OF_TIMEFRAMES.\n" +
+                          "Leave at least one timeframe after NUMBER_OF_STABILIZATION_TIMEFRAMES.\n" +
+                          f"See the documentation at {WEBSITE}")
             sys.exit()
 
         for source in self.phonon_sources:
             if source.y > self.length:
-                print("ERROR: Y coordinate of a source exceeded LENGHT.\n")
+                logging.error("Y coordinate of a source exceeded LENGHT")
                 sys.exit()
 
             if source.y < 0:
-                print("ERROR: Y coordinate of a source is negative.\n")
+                logging.error("Y coordinate of a source is negative.")
                 sys.exit()
 
             if source.y - source.size_y / 2 < 0:
-                print("ERROR: Source size along Y coordinate is too large.\n")
+                logging.error("Source size along Y coordinate is too large")
                 sys.exit()
 
             if abs(source.x) > self.width/2:
-                print("ERROR: X coordinate of a source exceeds WIDTH.\n")
+                logging.error("X coordinate of a source exceeds WIDTH")
                 sys.exit()
 
             if abs(source.x + source.size_x / 2) > self.width/2:
-                print("ERROR: Source size along X coordinate is too large.\n")
+                logging.error("Source size along X coordinate is too large")
                 sys.exit()
 
             if abs(source.z) > self.thickness/2:
-                print("ERROR: Z coordinate of a source exceeds THICKNESS.\n")
+                logging.error("Z coordinate of a source exceeds THICKNESS")
                 sys.exit()
 
             if abs(source.z + source.size_z / 2) > self.thickness/2:
-                print("ERROR: Source size along Z coordinate is too large.\n")
+                logging.error("Source size along Z coordinate is too large")
                 sys.exit()
 
         if self.output_path_animation and self.number_of_timesteps > 5000:
-            print("WARNING: NUMBER_OF_TIMESTEPS is rather large for animation.\n")
+            logging.warning("NUMBER_OF_TIMESTEPS is rather large for animation")
 
         if (self.cold_side_position_top and self.include_top_sidewall or
             self.hot_side_position_top and self.include_top_sidewall or
             self.cold_side_position_top and self.hot_side_position_top):
-            print("ERROR: Top side is assigned multiple functions.\n")
+            logging.error("Top side is assigned multiple functions")
             sys.exit()
 
         if (self.cold_side_position_bottom and self.include_bottom_sidewall or
             self.hot_side_position_bottom and self.include_bottom_sidewall or
             self.cold_side_position_bottom and self.hot_side_position_bottom):
-            print("ERROR: Bottom side is assigned multiple functions.\n")
+            logging.error("Bottom side is assigned multiple functions")
             sys.exit()
 
         if (self.cold_side_position_right and self.include_right_sidewall or
             self.hot_side_position_right and self.include_right_sidewall or
             self.cold_side_position_right and self.hot_side_position_right):
-            print("ERROR: Right side is assigned multiple functions.\n")
+            logging.error("Right side is assigned multiple functions")
             sys.exit()
 
         if (self.cold_side_position_left and self.include_left_sidewall or
             self.hot_side_position_left and self.include_left_sidewall or
             self.cold_side_position_left and self.hot_side_position_left):
-            print("ERROR: Left side is assigned multiple functions.\n")
+            logging.error("Left side is assigned multiple functions")
             sys.exit()
 
 
     def check_depricated_parameters(self):
         """Check for deprecated parameters and warn about them"""
 
-        if 'INCLUDE_TOP_PARABOLA' in globals():
-            print("ERROR: parameter INCLUDE_TOP_PARABOLA is deprecated. Use ParabolaTop hole instead.")
-            sys.exit()
-
-        if 'INCLUDE_BOTTOM_PARABOLA' in globals():
-            print("ERROR: parameter INCLUDE_BOTTOM_PARABOLA is deprecated. Use ParabolaBottom hole instead.")
-            sys.exit()
-
         if 'COLD_SIDE_POSITION' in globals():
-            print("ERROR: parameter COLD_SIDE_POSITION is deprecated.")
-            print("Use specific boolean parameters like COLD_SIDE_POSITION_TOP = True.\n")
+            logging.error("Parameter COLD_SIDE_POSITION is deprecated.\n" +
+                          "Use specific boolean parameters like COLD_SIDE_POSITION_TOP = True\n" +
+                          f"See the documentation at {WEBSITE}")
             sys.exit()
 
         if 'SPECIFIC_HEAT_CAPACITY' in globals():
-            print("Warning: parameter SPECIFIC_HEAT_CAPACITY is deprecated. Heat capacity is automatiacally set by material.")
+            logging.warning("Parameter SPECIFIC_HEAT_CAPACITY is deprecated. Heat capacity is set from material.")
 
         if any([
             'HOT_SIDE_POSITION' in globals(),
             'HOT_SIDE_X' in globals(),
             'HOT_SIDE_Y' in globals(),
             'HOT_SIDE_WIDTH_X' in globals(),
             'HOT_SIDE_WIDTH_Y' in globals(),
             'HOT_SIDE_ANGLE_DISTRIBUTION' in globals(),
             'PHONON_SOURCE_X' in globals(),
             'PHONON_SOURCE_Y' in globals(),
             'PHONON_SOURCE_WIDTH_X' in globals(),
             'PHONON_SOURCE_WIDTH_Y' in globals(),
             'PHONON_SOURCE_ANGLE_DISTRIBUTION' in globals(),
             ]):
-            print("ERROR: parameters related to HOT_SIDE_... or PHONON_SOURCE_.. are deprecated. ")
-            print("Phonon source should be defined through the PHONON_SOURCES variable.\n")
-            print("See updated documentation for more details.\n")
+            logging.error("Parameters related to HOT_SIDE_... or PHONON_SOURCE_... were deprecated.\n" +
+                          "Phonon source should be defined through the PHONON_SOURCES variable.\n" +
+                          f"See the documentation at {WEBSITE}")
             sys.exit()
 
 cf = Config()
 cf.convert_to_enums()
 cf.check_parameter_validity()
 cf.check_depricated_parameters()
```

### Comparing `freepaths-1.9/freepaths/data.py` & `freepaths-1.9.1/freepaths/data.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/default_config.py` & `freepaths-1.9.1/freepaths/default_config.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/flight.py` & `freepaths-1.9.1/freepaths/flight.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/holes.py` & `freepaths-1.9.1/freepaths/holes.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/main_mfp_sampling.py` & `freepaths-1.9.1/freepaths/main_mfp_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 import sys
 import time
 import shutil
 import scipy
 import math
+import logging
 from colorama import Fore, Style
 
 # Modules:
 from freepaths.animation import create_animation
 from freepaths.config import cf
 from freepaths.run_phonon import run_phonon
 from freepaths.phonon import Phonon
@@ -33,15 +34,15 @@
     if cf.media == "Si":
         material = Si(cf.temp, num_points=cf.number_of_phonons +1)
     elif cf.media == "SiC":
         material = SiC(cf.temp, num_points=cf.number_of_phonons+1)
     elif cf.media == "Graphite":
         material = Graphite(cf.temp, num_points=cf.number_of_phonons+1)
     else:
-        print(f"Material {cf.media} is not supported")
+        logging.error(f"Material {cf.media} is not supported")
         sys.exit()
 
     # Initiate data structures:
     scatter_stats = ScatteringData()
     general_stats = GeneralData()
     segment_stats = SegmentData()
     path_stats = PathData()
```

### Comparing `freepaths-1.9/freepaths/main_tracing.py` & `freepaths-1.9.1/freepaths/main_tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 import sys
 import time
 import shutil
 import colorama
 import multiprocessing
+import logging
 from colorama import Fore, Style
 
 # Modules:
 from freepaths.config import cf
 from freepaths.run_phonon import run_phonon
 from freepaths.phonon import Phonon
 from freepaths.flight import Flight
@@ -34,15 +35,15 @@
         if cf.media == "Si":
             self.material = Si(cf.temp)
         elif cf.media == "SiC":
             self.material = SiC(cf.temp)
         elif cf.media == "Graphite":
             self.material = Graphite(cf.temp)
         else:
-            print(f"Material {cf.media} is not supported")
+            logging.error(f"Material {cf.media} is not supported")
             sys.exit()
 
         # Save some general information about the process:
         self.worker_id = worker_id
         self.total_phonons = total_phonons
         self.result_queue = shared_list
         self.creation_time = time.time()
```

### Comparing `freepaths-1.9/freepaths/maps.py` & `freepaths-1.9.1/freepaths/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             # Record energy h*w [J] and heat flux [W/s/m^2] of this phonon into the pixel of thermal map:
             energy = hbar * 2 * pi * ph.f
             self.number_phonons_in_pixel[index_y, index_x] += 1
             self.thermal_map[index_y, index_x] += energy
             self.heat_flux_map_x[index_y, index_x] += energy * sin(ph.theta) * abs(cos(ph.phi)) * ph.speed / self.vol_pixel
             self.heat_flux_map_y[index_y, index_x] += energy * cos(ph.theta) * abs(cos(ph.phi)) * ph.speed / self.vol_pixel
             self.heat_flux_map_xy[index_y, index_x] += np.sqrt(self.heat_flux_map_x[index_y, index_x]**2 +
-                                                               self.heat_flux_map_x[index_y, index_x]**2)
+                                                               self.heat_flux_map_y[index_y, index_x]**2)
 
             # Calculate to which timeframe this timestep belongs:
             timeframe_number = (ph.first_timestep + timestep_number) // self.timepteps_per_timeframe
 
             # Record temperature and energy into the corresponding time segment:
             if timeframe_number < cf.number_of_timeframes:
                 self.effective_heat_flux_profile_x[index_x, timeframe_number] += energy * sin(ph.theta) * abs(cos(ph.phi)) * ph.speed / self.vol_cell_x
```

### Comparing `freepaths-1.9/freepaths/materials.py` & `freepaths-1.9.1/freepaths/materials.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/move.py` & `freepaths-1.9.1/freepaths/move.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/output_info.py` & `freepaths-1.9.1/freepaths/output_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Module that outputs general info and basic scattering statistics"""
 
 import time
+import logging
 import numpy as np
 
 from colorama import Fore, Style
 
 from freepaths.config import cf
 
 
@@ -111,21 +112,21 @@
     # Check if some phonons had longer travel times than stabilization period:
     travel_times = np.loadtxt("Data/All travel times.csv", encoding='utf-8')
     total_time = cf.timestep * cf.number_of_timesteps
     time_of_stabilization = cf.number_of_stabilization_timeframes * total_time / cf. number_of_timeframes
     long_travel_times = travel_times[travel_times > time_of_stabilization]
     percentage = (len(long_travel_times) / len(travel_times)) * 100
     if percentage > 10:
-        print(f'{Fore.RED}Warning: Travel time of {percentage}% of phonons was longer than the stabilization period.')
-        print(f'Increase stabilization period as the thermal conductivity might be incorrect.{Style.RESET_ALL}')
+        logging.warning("Travel time of {percentage}% of phonons was longer than the stabilization period.\n" +
+                          "Increase stabilization period as the thermal conductivity might be incorrect.")
 
     # Check if pixel size is too small:
     speeds = np.loadtxt("Data/All group velocities.csv", encoding='utf-8')
     if max(speeds) * cf.timestep > cf.length / cf.number_of_pixels_y:
-        print(f'{Fore.RED}Warning: Pixels in y direction are smaller than length of one step.{Style.RESET_ALL}')
+        logging.warning("Pixels in y direction are smaller than length of one step")
     if max(speeds) * cf.timestep > cf.width / cf.number_of_pixels_x:
-        print(f'{Fore.RED}Warning: Pixels in x direction are smaller than length of one step.{Style.RESET_ALL}')
+        logging.warning("Pixels in x direction are smaller than length of one step")
 
     # Check how many phonons reached the cold side during simulation:
     percentage = int(100 * np.count_nonzero(travel_times) / cf.number_of_phonons)
     if percentage < 95:
-        print(f'{Fore.RED}Warning: Only {percentage}% of phonons reached the cold side. Increase number of timesteps.{Style.RESET_ALL}')
+        logging.warning("Only {percentage}% of phonons reached the cold side. Increase number of timesteps.")
```

### Comparing `freepaths-1.9/freepaths/output_plots.py` & `freepaths-1.9.1/freepaths/output_plots.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/output_structure.py` & `freepaths-1.9.1/freepaths/output_structure.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/phonon.py` & `freepaths-1.9.1/freepaths/phonon.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/progress.py` & `freepaths-1.9.1/freepaths/progress.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/run_phonon.py` & `freepaths-1.9.1/freepaths/run_phonon.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/scattering.py` & `freepaths-1.9.1/freepaths/scattering.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/scattering_primitives.py` & `freepaths-1.9.1/freepaths/scattering_primitives.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/scattering_semicircle.py` & `freepaths-1.9.1/freepaths/scattering_semicircle.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/scattering_types.py` & `freepaths-1.9.1/freepaths/scattering_types.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths/sources.py` & `freepaths-1.9.1/freepaths/sources.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/freepaths.egg-info/PKG-INFO` & `freepaths-1.9.1/freepaths.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.9
+Version: 1.9.1
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `freepaths-1.9/freepaths.egg-info/SOURCES.txt` & `freepaths-1.9.1/freepaths.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freepaths-1.9/setup.py` & `freepaths-1.9.1/setup.py`

 * *Files identical despite different names*


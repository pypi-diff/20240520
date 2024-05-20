# Comparing `tmp/atspm-1.3.0a1.tar.gz` & `tmp/atspm-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atspm-1.3.0a1.tar", last modified: Thu May  2 16:46:50 2024, max compression
+gzip compressed data, was "atspm-1.4.0.tar", last modified: Mon May 20 19:54:35 2024, max compression
```

## Comparing `atspm-1.3.0a1.tar` & `atspm-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.528613 atspm-1.3.0a1/
--rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.3.0a1/LICENSE
--rw-rw-rw-   0        0        0       85 2024-04-12 01:08:02.000000 atspm-1.3.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     3481 2024-05-02 16:46:50.528613 atspm-1.3.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2024-04-18 18:32:57.000000 atspm-1.3.0a1/README.md
--rw-rw-rw-   0        0        0      627 2024-05-02 16:44:22.000000 atspm-1.3.0a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-02 16:46:50.529610 atspm-1.3.0a1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.451997 atspm-1.3.0a1/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.486880 atspm-1.3.0a1/src/atspm/
--rw-rw-rw-   0        0        0       92 2024-04-18 18:05:56.000000 atspm-1.3.0a1/src/atspm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.507681 atspm-1.3.0a1/src/atspm/data/
--rw-rw-rw-   0        0        0     3321 2024-04-18 18:01:38.000000 atspm-1.3.0a1/src/atspm/data/sample_config.parquet
--rw-rw-rw-   0        0        0   271222 2024-04-16 00:47:05.000000 atspm-1.3.0a1/src/atspm/data/sample_raw_data.parquet
--rw-rw-rw-   0        0        0     1270 2024-05-01 17:20:10.000000 atspm-1.3.0a1/src/atspm/data_aggregator.py
--rw-rw-rw-   0        0        0     1749 2024-05-01 21:44:28.000000 atspm-1.3.0a1/src/atspm/data_loader.py
--rw-rw-rw-   0        0        0     1326 2024-04-18 17:49:58.000000 atspm-1.3.0a1/src/atspm/data_saver.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.526620 atspm-1.3.0a1/src/atspm/queries/
--rw-rw-rw-   0        0        0      348 2024-05-01 17:51:34.000000 atspm-1.3.0a1/src/atspm/queries/actuations.sql
--rw-rw-rw-   0        0        0     3683 2024-05-01 18:13:20.000000 atspm-1.3.0a1/src/atspm/queries/arrival_on_green.sql
--rw-rw-rw-   0        0        0      508 2024-05-01 18:16:22.000000 atspm-1.3.0a1/src/atspm/queries/communications.sql
--rw-rw-rw-   0        0        0      447 2024-05-01 18:22:39.000000 atspm-1.3.0a1/src/atspm/queries/coordination.sql
--rw-rw-rw-   0        0        0     2537 2024-05-01 22:20:36.000000 atspm-1.3.0a1/src/atspm/queries/detector_faults.sql
--rw-rw-rw-   0        0        0      907 2024-05-01 16:24:38.000000 atspm-1.3.0a1/src/atspm/queries/has_data.sql
--rw-rw-rw-   0        0        0      694 2024-05-01 22:26:09.000000 atspm-1.3.0a1/src/atspm/queries/ped.sql
--rw-rw-rw-   0        0        0    10634 2024-05-02 16:35:05.000000 atspm-1.3.0a1/src/atspm/queries/split_failures.sql
--rw-rw-rw-   0        0        0      408 2024-05-01 23:51:36.000000 atspm-1.3.0a1/src/atspm/queries/splits.sql
--rw-rw-rw-   0        0        0      584 2024-05-01 23:54:46.000000 atspm-1.3.0a1/src/atspm/queries/terminations.sql
--rw-rw-rw-   0        0        0     1037 2024-05-01 23:56:18.000000 atspm-1.3.0a1/src/atspm/queries/unique_ped.sql
--rw-rw-rw-   0        0        0     4724 2024-05-02 00:27:14.000000 atspm-1.3.0a1/src/atspm/queries/yellow_red.sql
--rw-rw-rw-   0        0        0      493 2024-04-18 18:04:49.000000 atspm-1.3.0a1/src/atspm/sample_data.py
--rw-rw-rw-   0        0        0     4602 2024-05-02 16:43:31.000000 atspm-1.3.0a1/src/atspm/signal_data_processor.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:46:50.527616 atspm-1.3.0a1/src/atspm.egg-info/
--rw-rw-rw-   0        0        0     3481 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      850 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 16:46:50.000000 atspm-1.3.0a1/src/atspm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.880599 atspm-1.4.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0       85 2024-04-12 01:08:02.000000 atspm-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3851 2024-05-20 19:54:35.880599 atspm-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3255 2024-05-03 01:09:32.000000 atspm-1.4.0/README.md
+-rw-rw-rw-   0        0        0      689 2024-05-20 19:54:26.000000 atspm-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 19:54:35.880599 atspm-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.817701 atspm-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.833329 atspm-1.4.0/src/atspm/
+-rw-rw-rw-   0        0        0      117 2024-05-20 19:52:15.000000 atspm-1.4.0/src/atspm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.865095 atspm-1.4.0/src/atspm/data/
+-rw-rw-rw-   0        0        0     3321 2024-04-18 18:01:38.000000 atspm-1.4.0/src/atspm/data/sample_config.parquet
+-rw-rw-rw-   0        0        0   271222 2024-04-16 00:47:05.000000 atspm-1.4.0/src/atspm/data/sample_raw_data.parquet
+-rw-rw-rw-   0        0        0     1938 2024-05-20 19:08:47.000000 atspm-1.4.0/src/atspm/data_aggregator.py
+-rw-rw-rw-   0        0        0     2847 2024-05-20 18:20:04.000000 atspm-1.4.0/src/atspm/data_loader.py
+-rw-rw-rw-   0        0        0     1326 2024-04-18 17:49:58.000000 atspm-1.4.0/src/atspm/data_saver.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.880599 atspm-1.4.0/src/atspm/queries/
+-rw-rw-rw-   0        0        0      348 2024-05-01 17:51:34.000000 atspm-1.4.0/src/atspm/queries/actuations.sql
+-rw-rw-rw-   0        0        0     3683 2024-05-01 18:13:20.000000 atspm-1.4.0/src/atspm/queries/arrival_on_green.sql
+-rw-rw-rw-   0        0        0      508 2024-05-01 18:16:22.000000 atspm-1.4.0/src/atspm/queries/communications.sql
+-rw-rw-rw-   0        0        0      447 2024-05-01 18:22:39.000000 atspm-1.4.0/src/atspm/queries/coordination.sql
+-rw-rw-rw-   0        0        0     2537 2024-05-01 22:20:36.000000 atspm-1.4.0/src/atspm/queries/detector_faults.sql
+-rw-rw-rw-   0        0        0      907 2024-05-01 16:24:38.000000 atspm-1.4.0/src/atspm/queries/has_data.sql
+-rw-rw-rw-   0        0        0      694 2024-05-01 22:26:09.000000 atspm-1.4.0/src/atspm/queries/ped.sql
+-rw-rw-rw-   0        0        0    10634 2024-05-02 16:35:05.000000 atspm-1.4.0/src/atspm/queries/split_failures.sql
+-rw-rw-rw-   0        0        0      408 2024-05-01 23:51:36.000000 atspm-1.4.0/src/atspm/queries/splits.sql
+-rw-rw-rw-   0        0        0      584 2024-05-01 23:54:46.000000 atspm-1.4.0/src/atspm/queries/terminations.sql
+-rw-rw-rw-   0        0        0     5613 2024-05-20 16:24:50.000000 atspm-1.4.0/src/atspm/queries/timeline.sql
+-rw-rw-rw-   0        0        0     1037 2024-05-01 23:56:18.000000 atspm-1.4.0/src/atspm/queries/unique_ped.sql
+-rw-rw-rw-   0        0        0     4724 2024-05-02 00:27:14.000000 atspm-1.4.0/src/atspm/queries/yellow_red.sql
+-rw-rw-rw-   0        0        0      493 2024-04-18 18:04:49.000000 atspm-1.4.0/src/atspm/sample_data.py
+-rw-rw-rw-   0        0        0     9162 2024-05-20 19:51:05.000000 atspm-1.4.0/src/atspm/signal_data_processor.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:54:35.880599 atspm-1.4.0/src/atspm.egg-info/
+-rw-rw-rw-   0        0        0     3851 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 19:54:35.000000 atspm-1.4.0/src/atspm.egg-info/top_level.txt
```

### Comparing `atspm-1.3.0a1/LICENSE` & `atspm-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/PKG-INFO` & `atspm-1.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: atspm
-Version: 1.3.0a1
-Summary: Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures.
-Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: duckdb<0.10.2,>=0.9.1
-
 # ATSPM Aggregation
 
 `atspm` is a Python package to transform hi-res ATC signal controller data into aggregate ATSPMs (Automated Traffic Signal Performance Measures). It works on multiple devices/detectors at once.
 
 ## Installation
 
 ```bash
@@ -33,30 +20,34 @@
 bin_size = 15
 
 # Set up all parameters
 params = {
     # Global Settings
     'raw_data': sample_data.data, # dataframe or file path to csv/parquet/json
     'detector_config': sample_data.config,
+    'bin_size': 15, # in minutes
     'output_dir': 'test_folder',
     'output_to_separate_folders': True,
     'output_format': 'csv', # csv/parquet/json
     'output_file_prefix': 'test_prefix',
-    # Performance Measure Settings
+    'remove_incomplete': True, # Remove periods with incomplete data by joining to the has_data table
+    # Performance Measures
     'aggregations': [
-        {'name': 'actuations', 'params': {'bin_size': bin_size}},
-        {'name': 'yellow_red', 'params': {'bin_size': bin_size, 'latency_offset_seconds': 1.5}},
-        {'name': 'arrival_on_green', 'params': {'bin_size': bin_size, 'latency_offset_seconds': 0}},
-        #{'name': 'communications', 'params': {'bin_size': bin_size, 'event_codes': '400,503,502'}}, #MaxView Specific
-        {'name': 'coordination', 'params': {'bin_size': bin_size}},
-        {'name': 'terminations', 'params': {'bin_size': bin_size}},
-        {'name': 'split_failures', 'params': {'bin_size': bin_size, 'red_time': 5, 'red_occupancy_threshold': 0.80, 'green_occupancy_threshold': 0.80, 'by_approach': True}},
-        {'name': 'ped', 'params': {'bin_size': bin_size}},
-        {'name': 'unique_ped', 'params': {'bin_size': bin_size, 'seconds_between_actuations': 15}},
-        {'name': 'splits', 'params': {'bin_size': bin_size}},
+        {'name': 'has_data', 'params': {'no_data_min': 3, 'min_data_points': 10}}, # in minutes, ie remove bins with less than 10 rows every 3 minutes
+        {'name': 'actuations', 'params': {}},
+        {'name': 'arrival_on_green', 'params': {'latency_offset_seconds': 0}},
+        {'name': 'communications', 'params': {'event_codes': '400,503,502'}}, # MAXVIEW Specific
+        {'name': 'coordination', 'params': {}}, # MAXTIME Specific
+        # detector faults and detector health almost ready
+        {'name': 'ped', 'params': {}},
+        {'name': 'split_failures', 'params': {'red_time': 5, 'red_occupancy_threshold': 0.80, 'green_occupancy_threshold': 0.70, 'by_approach': True}},
+        {'name': 'splits', 'params': {}}, # MAXTIME Specific
+        {'name': 'terminations', 'params': {}},
+        {'name': 'unique_ped', 'params': {'seconds_between_actuations': 15}},
+        {'name': 'yellow_red', 'params': {'latency_offset_seconds': 1.5, 'min_red_offset': -8}}, # min_red_offset is optional, it filters out actuations occuring -n seconds before start of red
     ]
 }
 
 processor = SignalDataProcessor(**params)
 processor.run()
 ```
```

### Comparing `atspm-1.3.0a1/pyproject.toml` & `atspm-1.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [project]
 name = "atspm"
-version = "1.3.0alpha1"
+version = "1.4.0"
 authors = [
   { name="Shawn Strasser", email="shawn.strasser@odot.oregon.gov" },
 ]
 description = "Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "duckdb>=0.9.1,<0.10.2",
+    "traffic-anomaly>=1.0.0",
+    "ibis-framework[duckdb]==9.0.0"
 ]
 
 [tools.setuptools]
 include_package_data = true
 package_data = {"atspm" = ["queries/*", "data/*"]}
```

### Comparing `atspm-1.3.0a1/src/atspm/data/sample_config.parquet` & `atspm-1.4.0/src/atspm/data/sample_config.parquet`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/data/sample_raw_data.parquet` & `atspm-1.4.0/src/atspm/data/sample_raw_data.parquet`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/data_saver.py` & `atspm-1.4.0/src/atspm/data_saver.py`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/queries/arrival_on_green.sql` & `atspm-1.4.0/src/atspm/queries/arrival_on_green.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/queries/detector_faults.sql` & `atspm-1.4.0/src/atspm/queries/detector_faults.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/queries/has_data.sql` & `atspm-1.4.0/src/atspm/queries/has_data.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/queries/ped.sql` & `atspm-1.4.0/src/atspm/queries/ped.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/queries/split_failures.sql` & `atspm-1.4.0/src/atspm/queries/split_failures.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/queries/terminations.sql` & `atspm-1.4.0/src/atspm/queries/terminations.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/queries/unique_ped.sql` & `atspm-1.4.0/src/atspm/queries/unique_ped.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm/queries/yellow_red.sql` & `atspm-1.4.0/src/atspm/queries/yellow_red.sql`

 * *Files identical despite different names*

### Comparing `atspm-1.3.0a1/src/atspm.egg-info/PKG-INFO` & `atspm-1.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: atspm
-Version: 1.3.0a1
+Version: 1.4.0
 Summary: Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb<0.10.2,>=0.9.1
+Requires-Dist: traffic-anomaly>=1.0.0
+Requires-Dist: ibis-framework[duckdb]==9.0.0
 
 # ATSPM Aggregation
 
 `atspm` is a Python package to transform hi-res ATC signal controller data into aggregate ATSPMs (Automated Traffic Signal Performance Measures). It works on multiple devices/detectors at once.
 
 ## Installation
 
@@ -33,30 +35,34 @@
 bin_size = 15
 
 # Set up all parameters
 params = {
     # Global Settings
     'raw_data': sample_data.data, # dataframe or file path to csv/parquet/json
     'detector_config': sample_data.config,
+    'bin_size': 15, # in minutes
     'output_dir': 'test_folder',
     'output_to_separate_folders': True,
     'output_format': 'csv', # csv/parquet/json
     'output_file_prefix': 'test_prefix',
-    # Performance Measure Settings
+    'remove_incomplete': True, # Remove periods with incomplete data by joining to the has_data table
+    # Performance Measures
     'aggregations': [
-        {'name': 'actuations', 'params': {'bin_size': bin_size}},
-        {'name': 'yellow_red', 'params': {'bin_size': bin_size, 'latency_offset_seconds': 1.5}},
-        {'name': 'arrival_on_green', 'params': {'bin_size': bin_size, 'latency_offset_seconds': 0}},
-        #{'name': 'communications', 'params': {'bin_size': bin_size, 'event_codes': '400,503,502'}}, #MaxView Specific
-        {'name': 'coordination', 'params': {'bin_size': bin_size}},
-        {'name': 'terminations', 'params': {'bin_size': bin_size}},
-        {'name': 'split_failures', 'params': {'bin_size': bin_size, 'red_time': 5, 'red_occupancy_threshold': 0.80, 'green_occupancy_threshold': 0.80, 'by_approach': True}},
-        {'name': 'ped', 'params': {'bin_size': bin_size}},
-        {'name': 'unique_ped', 'params': {'bin_size': bin_size, 'seconds_between_actuations': 15}},
-        {'name': 'splits', 'params': {'bin_size': bin_size}},
+        {'name': 'has_data', 'params': {'no_data_min': 3, 'min_data_points': 10}}, # in minutes, ie remove bins with less than 10 rows every 3 minutes
+        {'name': 'actuations', 'params': {}},
+        {'name': 'arrival_on_green', 'params': {'latency_offset_seconds': 0}},
+        {'name': 'communications', 'params': {'event_codes': '400,503,502'}}, # MAXVIEW Specific
+        {'name': 'coordination', 'params': {}}, # MAXTIME Specific
+        # detector faults and detector health almost ready
+        {'name': 'ped', 'params': {}},
+        {'name': 'split_failures', 'params': {'red_time': 5, 'red_occupancy_threshold': 0.80, 'green_occupancy_threshold': 0.70, 'by_approach': True}},
+        {'name': 'splits', 'params': {}}, # MAXTIME Specific
+        {'name': 'terminations', 'params': {}},
+        {'name': 'unique_ped', 'params': {'seconds_between_actuations': 15}},
+        {'name': 'yellow_red', 'params': {'latency_offset_seconds': 1.5, 'min_red_offset': -8}}, # min_red_offset is optional, it filters out actuations occuring -n seconds before start of red
     ]
 }
 
 processor = SignalDataProcessor(**params)
 processor.run()
 ```
```

### Comparing `atspm-1.3.0a1/src/atspm.egg-info/SOURCES.txt` & `atspm-1.4.0/src/atspm.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,9 +21,10 @@
 src/atspm/queries/coordination.sql
 src/atspm/queries/detector_faults.sql
 src/atspm/queries/has_data.sql
 src/atspm/queries/ped.sql
 src/atspm/queries/split_failures.sql
 src/atspm/queries/splits.sql
 src/atspm/queries/terminations.sql
+src/atspm/queries/timeline.sql
 src/atspm/queries/unique_ped.sql
 src/atspm/queries/yellow_red.sql
```


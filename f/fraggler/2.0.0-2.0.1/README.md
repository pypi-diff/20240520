# Comparing `tmp/fraggler-2.0.0.tar.gz` & `tmp/fraggler-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fraggler-2.0.0.tar", last modified: Tue Feb 20 06:40:54 2024, max compression
+gzip compressed data, was "fraggler-2.0.1.tar", last modified: Mon May 20 19:19:34 2024, max compression
```

## Comparing `fraggler-2.0.0.tar` & `fraggler-2.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.239053 fraggler-2.0.0/
--rw-r--r--   0 wiro0005   (503) staff       (20)     1067 2023-05-22 12:09:35.000000 fraggler-2.0.0/LICENSE
--rw-r--r--   0 wiro0005   (503) staff       (20)     4253 2024-02-20 06:40:54.238964 fraggler-2.0.0/PKG-INFO
--rw-r--r--   0 wiro0005   (503) staff       (20)     3566 2024-02-19 15:21:55.000000 fraggler-2.0.0/README.md
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.234071 fraggler-2.0.0/fraggler/
--rw-r--r--   0 wiro0005   (503) staff       (20)     1691 2023-09-11 13:26:53.000000 fraggler-2.0.0/fraggler/__init__.py
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.235370 fraggler-2.0.0/fraggler/applications/
--rw-r--r--   0 wiro0005   (503) staff       (20)        0 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/applications/__init__.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     7420 2023-06-26 14:34:27.000000 fraggler-2.0.0/fraggler/applications/peak_area_multiplex.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     9052 2024-02-20 06:38:40.000000 fraggler-2.0.0/fraggler/cli.py
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.235641 fraggler-2.0.0/fraggler/functions/
--rw-r--r--   0 wiro0005   (503) staff       (20)        0 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/functions/__init__.py
--rw-r--r--   0 wiro0005   (503) staff       (20)      937 2023-05-24 11:18:45.000000 fraggler-2.0.0/fraggler/functions/generate_peak_table.py
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.236052 fraggler-2.0.0/fraggler/ladder_fitting/
--rw-r--r--   0 wiro0005   (503) staff       (20)        0 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/ladder_fitting/__init__.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     4154 2023-06-27 05:13:23.000000 fraggler-2.0.0/fraggler/ladder_fitting/fit_ladder_model.py
--rw-r--r--   0 wiro0005   (503) staff       (20)    13160 2023-06-27 12:01:43.000000 fraggler-2.0.0/fraggler/ladder_fitting/peak_ladder_assigner.py
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.236380 fraggler-2.0.0/fraggler/ladders/
--rw-r--r--   0 wiro0005   (503) staff       (20)        0 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/ladders/__init__.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     2260 2023-09-21 18:38:10.000000 fraggler-2.0.0/fraggler/ladders/ladders.py
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.237169 fraggler-2.0.0/fraggler/plotting/
--rw-r--r--   0 wiro0005   (503) staff       (20)        0 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/plotting/__init__.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     1475 2023-06-27 12:01:43.000000 fraggler-2.0.0/fraggler/plotting/plot_channels.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     1854 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/plotting/plot_ladder.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     1784 2023-06-26 14:34:27.000000 fraggler-2.0.0/fraggler/plotting/plot_peak_area.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     1175 2023-06-27 09:01:05.000000 fraggler-2.0.0/fraggler/plotting/plot_peaks.py
--rw-r--r--   0 wiro0005   (503) staff       (20)      359 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/plotting/plot_raw_data.py
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.237446 fraggler-2.0.0/fraggler/reports/
--rw-r--r--   0 wiro0005   (503) staff       (20)        0 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/reports/__init__.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     8457 2023-06-27 12:01:43.000000 fraggler-2.0.0/fraggler/reports/reports.py
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.238376 fraggler-2.0.0/fraggler/utils/
--rw-r--r--   0 wiro0005   (503) staff       (20)        0 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/utils/__init__.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     1277 2023-05-22 12:09:35.000000 fraggler-2.0.0/fraggler/utils/baseline_removal.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     3123 2023-06-26 15:23:24.000000 fraggler-2.0.0/fraggler/utils/fraggler_object.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     3604 2023-05-24 08:00:06.000000 fraggler-2.0.0/fraggler/utils/fsa_file.py
--rw-r--r--   0 wiro0005   (503) staff       (20)     7575 2024-02-19 15:34:21.000000 fraggler-2.0.0/fraggler/utils/peak_finder.py
--rw-r--r--   0 wiro0005   (503) staff       (20)      910 2023-06-27 12:01:43.000000 fraggler-2.0.0/fraggler/utils/utils.py
-drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-02-20 06:40:54.238570 fraggler-2.0.0/fraggler.egg-info/
--rw-r--r--   0 wiro0005   (503) staff       (20)     4253 2024-02-20 06:40:54.000000 fraggler-2.0.0/fraggler.egg-info/PKG-INFO
--rw-r--r--   0 wiro0005   (503) staff       (20)     1039 2024-02-20 06:40:54.000000 fraggler-2.0.0/fraggler.egg-info/SOURCES.txt
--rw-r--r--   0 wiro0005   (503) staff       (20)        1 2024-02-20 06:40:54.000000 fraggler-2.0.0/fraggler.egg-info/dependency_links.txt
--rw-r--r--   0 wiro0005   (503) staff       (20)       46 2024-02-20 06:40:54.000000 fraggler-2.0.0/fraggler.egg-info/entry_points.txt
--rw-r--r--   0 wiro0005   (503) staff       (20)      135 2024-02-20 06:40:54.000000 fraggler-2.0.0/fraggler.egg-info/requires.txt
--rw-r--r--   0 wiro0005   (503) staff       (20)        9 2024-02-20 06:40:54.000000 fraggler-2.0.0/fraggler.egg-info/top_level.txt
--rw-r--r--   0 wiro0005   (503) staff       (20)       79 2024-02-20 06:40:54.239267 fraggler-2.0.0/setup.cfg
--rw-r--r--   0 wiro0005   (503) staff       (20)      985 2024-02-20 06:40:01.000000 fraggler-2.0.0/setup.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.585132 fraggler-2.0.1/
+-rw-r--r--   0 wiro0005   (503) staff       (20)     1067 2024-05-17 14:32:09.000000 fraggler-2.0.1/LICENSE
+-rw-r--r--   0 wiro0005   (503) staff       (20)     5619 2024-05-20 19:19:34.582505 fraggler-2.0.1/PKG-INFO
+-rw-r--r--   0 wiro0005   (503) staff       (20)     4932 2024-05-20 19:18:28.000000 fraggler-2.0.1/README.md
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.546014 fraggler-2.0.1/fraggler/
+-rw-r--r--   0 wiro0005   (503) staff       (20)     1705 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/__init__.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.550195 fraggler-2.0.1/fraggler/applications/
+-rw-r--r--   0 wiro0005   (503) staff       (20)        0 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/applications/__init__.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     9029 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/applications/peak_area_multiplex.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     9036 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/cli.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.551305 fraggler-2.0.1/fraggler/functions/
+-rw-r--r--   0 wiro0005   (503) staff       (20)        0 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/functions/__init__.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)      937 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/functions/generate_peak_table.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.554301 fraggler-2.0.1/fraggler/ladder_fitting/
+-rw-r--r--   0 wiro0005   (503) staff       (20)        0 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/ladder_fitting/__init__.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     4199 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/ladder_fitting/fit_ladder_model.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)    13160 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/ladder_fitting/peak_ladder_assigner.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.556395 fraggler-2.0.1/fraggler/ladders/
+-rw-r--r--   0 wiro0005   (503) staff       (20)        0 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/ladders/__init__.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     2260 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/ladders/ladders.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.559663 fraggler-2.0.1/fraggler/plotting/
+-rw-r--r--   0 wiro0005   (503) staff       (20)        0 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/plotting/__init__.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     1475 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/plotting/plot_channels.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     1854 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/plotting/plot_ladder.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     1817 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/plotting/plot_peak_area.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     1175 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/plotting/plot_peaks.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)      359 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/plotting/plot_raw_data.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.560526 fraggler-2.0.1/fraggler/reports/
+-rw-r--r--   0 wiro0005   (503) staff       (20)        0 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/reports/__init__.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     8330 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/reports/reports.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.580090 fraggler-2.0.1/fraggler/utils/
+-rw-r--r--   0 wiro0005   (503) staff       (20)        0 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/utils/__init__.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     1277 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/utils/baseline_removal.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     3123 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/utils/fraggler_object.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     3776 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/utils/fsa_file.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)     9011 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/utils/peak_finder.py
+-rw-r--r--   0 wiro0005   (503) staff       (20)      910 2024-05-17 14:32:09.000000 fraggler-2.0.1/fraggler/utils/utils.py
+drwxr-xr-x   0 wiro0005   (503) staff       (20)        0 2024-05-20 19:19:34.581661 fraggler-2.0.1/fraggler.egg-info/
+-rw-r--r--   0 wiro0005   (503) staff       (20)     5619 2024-05-20 19:19:34.000000 fraggler-2.0.1/fraggler.egg-info/PKG-INFO
+-rw-r--r--   0 wiro0005   (503) staff       (20)     1029 2024-05-20 19:19:34.000000 fraggler-2.0.1/fraggler.egg-info/SOURCES.txt
+-rw-r--r--   0 wiro0005   (503) staff       (20)        1 2024-05-20 19:19:34.000000 fraggler-2.0.1/fraggler.egg-info/dependency_links.txt
+-rw-r--r--   0 wiro0005   (503) staff       (20)       46 2024-05-20 19:19:34.000000 fraggler-2.0.1/fraggler.egg-info/entry_points.txt
+-rw-r--r--   0 wiro0005   (503) staff       (20)      135 2024-05-20 19:19:34.000000 fraggler-2.0.1/fraggler.egg-info/requires.txt
+-rw-r--r--   0 wiro0005   (503) staff       (20)        9 2024-05-20 19:19:34.000000 fraggler-2.0.1/fraggler.egg-info/top_level.txt
+-rw-r--r--   0 wiro0005   (503) staff       (20)       38 2024-05-20 19:19:34.585801 fraggler-2.0.1/setup.cfg
+-rw-r--r--   0 wiro0005   (503) staff       (20)      985 2024-05-20 19:18:14.000000 fraggler-2.0.1/setup.py
```

### Comparing `fraggler-2.0.0/LICENSE` & `fraggler-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/PKG-INFO` & `fraggler-2.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fraggler
-Version: 2.0.0
+Version: 2.0.1
 Summary: Fragment Analysis package in python!
 Home-page: https://github.com/willros/fraggler
 Author: William Rosenbaum and Pär Larsson
 Author-email: william.rosenbaum@umu.se
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -21,60 +21,87 @@
 Requires-Dist: bokeh==3.3.4
 Requires-Dist: fire
 Requires-Dist: openpyxl
 Requires-Dist: colorama
 Requires-Dist: altair
 Requires-Dist: setuptools
 
-# Fraggler
+![Build Status](https://github.com/clinical-genomics-umea/fraggler/actions/workflows/pdoc.yaml/badge.svg)
+[![!pypi](https://img.shields.io/pypi/v/fraggler?color=cyan)](https://pypi.org/project/fraggler/)
+[![Download Status](https://static.pepy.tech/badge/fraggler)](https://pypi.python.org/pypi/fraggler/)
+
 ![logo](examples/logo.png)
 
 ## Description
 Fraggler is for fragment analysis in Python!
-Fraggler is a Python package that provides functionality for analyzing and generating reports for fsa files. It offers both a Python API and a command-line tool for ease of use.
+Fraggler is a Python package that provides functionality for analyzing and generating reports for fsa files. It offers both a Python API and a command-line tool.
 
 ----------------
 
 ### Features
 `Peak Area Report Generation`: Fraggler allows you to generate peak area reports for all input files. The package calculates peak areas based on specified parameters and generates a report summarizing the results.
 
 `Combined Peak Table Generation`: Fraggler provides a command-line tool to generate a combined dataframe of peaks for all input files. This allows you to easily analyze and compare peaks across multiple files.
 
 `Customization Options`: Fraggler offers various customization options to tailor the analysis to your specific needs. You can specify parameters such as ladder type, peak model, minimum ratio, minimum height, cutoff value, trace channel, peak height, and even provide a custom peaks file for specific assays and intervals.
 
 ## Install
 
-Via pip:
 ```bash
 pip install fraggler
 ```
 
-## Usage
+### Dependencies
+Fraggler depends on:
+- pandas
+- numpy
+- scikit-learn
+- networkx
+- lmfit
+- scipy
+- biopython
+- panel
+- fire
+- colorama
+- altair
+
+## Python API
 
-To get an overview how the library can be used in a python environment, please look at `tutorial.ipynb`.
+To get an overview how the library can be used in a python environment, please look at the [tutorial.ipynb](demo/tutorial.ipynb).
 
 
-## CLI Tool
+## CLI
 ### `fraggler area` and `fraggler peak`
 
 #### Usage
 To generate peak area reports and a peak table for all input files, use the `fraggler area` or `fraggler peak` command followed by the required positional arguments and any optional flags.
 
-- If not specified, fraggler finds peaks agnostic in the `fsa file`. To specifiy custom assays with certain peaks and intervals, the user can add a .csv file to the `--custom_peaks` argument. The csv file MUST have the following shape:
-
-| name | start | stop | amount | min_ratio |
-|------|-------|------|--------|-----------|
-| prt1 | 140   | 150  | 2      | 0.2       |
+- If not specified, fraggler finds peaks agnostic in the `fsa file`. To specifiy custom assays with certain peaks and intervals, the user can add a .csv file to the `--custom_peaks` argument. The csv file **MUST** have the following shape:
 
+| name | start | stop | amount | min_ratio | which | peak_distance |
+|------|-------|------|--------|-----------|-------|---------------|
+| prt1 | 140   | 150  | 2      | 0.2       | FIRST | 5             |
+
+##### Example how how a file could look:
+```txt 
+name,start,stop,amount,min_ratio,which,peak_distance
+prt1,135,155,2,0.2,FIRST,
+prt3,190,205,,0.2,FIRST,
+prt2,222,236,2,0.2,FIRST,5
+prt4,262,290,5,,,
+```
 
-If `amount` or `min_ratio` are left emtpy, `fraggler` will take all peaks inside the interval. If amount is not empty, fraggler will include the top `N` peaks in the interval, based on height. If `min_ratio` is set, only peaks with the a ratio of the `min_ratio` of the highest peak is included, *e.g.* if `min_ratio == .02`, only peaks with a height of 20 is included, if the highest peak is 100 units.
+- `name`: Name of the assay
+- `start`: Start of the assay in basepairs
+- `stop`: Stop of the assay in basepairs
+- `amount`: Optional. Amount of peaks in assay. If left empty every peak in the interval is included. 
+- `min_ratio`: Optional. Only peaks with the a ratio of the `min_ratio` of the highest peak is included, *e.g.* if `min_ratio == .02`, only peaks with a height of 20 is included, if the highest peak is 100 units
+- `which`: *LARGEST | FIRST*. Can be left empty. Which peak should be included if there are more peaks than the `amount`. if *FIRST* is set, then the two first peaks are chosen. If *LARGEST* are set, then the two largests peaks in the area are chosen. Defaults to *LARGEST*
+- `peak_distance`: Optional. Distance between peaks must be ***under*** this value.
 
-```console
-fraggler peak IN_PATH OUT_FOLDER --ladder LIZ <flags>
-```
 
 #### Positional Arguments
 The following positional arguments are required:
 
 - `IN_PATH`: Type `str`. Specifies the input path.
 - `OUT_FOLDER`: Type `str`. Specifies the output folder.
 - `LADDER`: Type `str`. Specifies the ladder used in the experiment.
@@ -90,17 +117,18 @@
 - `-t, --trace_channel=TRACE_CHANNEL`: Type `str`. Specifies the trace channel. Default value: 'DATA9'.
 - `--peak_height=PEAK_HEIGHT`: Type `int`. Specifies the peak height. Default value: 200.
 - `--custom_peaks=CUSTOM_PEAKS`: Type `Optional[str]`. Specifies custom peaks. Default value: None.
 - `-e, --excel=EXCEL`: Type: `bool`, Default: True
 
 #### Typical usage
 ```console
-fraggler peak IN_FOLDER OUT_FOLDER ORANGE --min_ratio=0.2 
+fraggler area IN_FOLDER OUT_FOLDER LIZ --min_ratio=0.2 
 ```
 
+#### Documentation
+Click [here](https://clinical-genomics-umea.github.io/fraggler/fraggler.html) to get full documentation of API.
 
+## Output
+One example of the report generated from `fraggler area` can be seen here: [Example report](examples/multiplex_fraggler_area.html)
 
-
-
-
-
-
+## Contributions
+Please check out [How to contribute](CONTRIBUTION.md)
```

### Comparing `fraggler-2.0.0/fraggler/__init__.py` & `fraggler-2.0.1/fraggler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""
-fraggler.
-Easy Fragment Analyzing in python!
+r"""
+.. include:: ../README.md
+.. include:: ../CONTRIBUTION.md
 """
 
 __author__ = "William Rosenbaum and Pär Larsson"
 
 from .ladder_fitting.fit_ladder_model import FitLadderModel
 from .ladder_fitting.peak_ladder_assigner import PeakLadderAssigner
 from .ladders.ladders import LADDERS
```

### Comparing `fraggler-2.0.0/fraggler/applications/peak_area_multiplex.py` & `fraggler-2.0.1/fraggler/applications/peak_area_multiplex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 import re
 import pandas as pd
 import numpy as np
+import matplotlib.pyplot as plt
 from lmfit.models import VoigtModel, GaussianModel, LorentzianModel
 from scipy.signal import find_peaks, peak_widths
 from ..utils.peak_finder import PeakFinder
 
 
 class PeakAreaDeMultiplexIterator:
     def __init__(self, number_of_assays):
         self.number_of_assays = number_of_assays
         self.current = 0
 
     def __next__(self):
         if self.current >= self.number_of_assays:
             raise StopIteration
-        else:
-            result = self.current
-            self.current += 1
-            return result
+        result = self.current
+        self.current += 1
+        return result
 
 
 class PeakAreaDeMultiplex:
     def __init__(
         self,
         peaks: PeakFinder,
         cutoff: float = None,
@@ -30,14 +30,15 @@
         self.peaks = peaks
         self.cutoff = cutoff or None
         self.peaks_dataframe = self.peaks.peaks_dataframe
         self.peak_information = self.peaks.peak_information
         self.file_name = self.peaks.file_name
         self.peaks_index = self.peaks.peaks_index
         self.found_peaks = self.peaks.found_peaks
+        self.area_plots = []
 
         self.find_peak_widths()
         # divade peaks based on their assay they belonging
         self.divided_assays = self.divide_peak_assays()
         # how many assays does this sample contain?
         self.number_of_assays = len(self.divided_assays)
         # divide all peaks in each assay into separate dataframes
@@ -136,19 +137,18 @@
     ) -> None:
 
         """
         :Params:
         """
         areas = np.array([x["amplitude"] for x in self.fit_params])
 
-        right_by_left = True
-        if self.cutoff is not None:
-            if pd.concat(self.fit_df).basepairs.mean() < self.cutoff:
-                right_by_left = False
-
+        right_by_left = (
+            self.cutoff is None
+            or pd.concat(self.fit_df).basepairs.mean() >= self.cutoff
+        )
         # if there only is 1 peak, return 0
         if len(areas) == 1:
             self.quotient = 0
             return
 
         # if there only are 2 peaks, return the quotient
         if len(areas) == 2:
@@ -156,19 +156,20 @@
             if not right_by_left:
                 self.quotient = areas[0] / areas[1]
                 return
             # right peak divided by left peak
             self.quotient = areas[1] / areas[0]
             return
 
-        # TODO change this to the proper assay
         # return the last peak divided by the mean of the peaks to the left of it
         self.quotient = areas[-1] / areas[:-1].mean()
 
-    def peak_position_area_dataframe(self, assay_number: int) -> pd.DataFrame:
+    def peak_position_area_dataframe(
+        self, assay_number: int, name: str
+    ) -> pd.DataFrame:
         """
         Returns a DataFrame of each peak and its properties
         """
         dataframes = []
         for i, _ in enumerate(self.fit_df):
             report = self.fit_report[i]
             r_value = float(re.findall(r"R-squared *= (0\.\d{3})", report)[0])
@@ -184,34 +185,78 @@
                     columns={
                         "peaks": "peak_height",
                         "fitted": "fitted_peak_height",
                     }
                 )
                 .drop_duplicates("peak_name")
                 .assign(file_name=self.file_name)
+                .assign(assay_name=name)
             )
             dataframes.append(df)
 
         self.assay_peak_area_df = pd.concat(dataframes).assign(
             quotient=self.quotient,
             peak_number=lambda x: x.shape[0],
             assay_number=assay_number + 1,
         )
 
+    def plot_areas(self, peak_finding_model: str):
+        fig_areas, axs = plt.subplots(
+            1, len(self.fit_df), sharey=True, figsize=(20, 10)
+        )
+        # if there is only one peak
+        if len(self.fit_df) == 1:
+            axs.plot(self.fit_df[0].basepairs, self.fit_df[0].peaks, "o")
+            axs.plot(self.fit_df[0].basepairs, self.fit_df[0].fitted)
+            axs.set_title(f"Peak 1 area: {self.fit_params[0]['amplitude']: .1f}")
+            axs.grid()
+        # if more than one peak
+        else:
+            for i, ax in enumerate(axs):
+                ax.plot(
+                    self.fit_df[i].basepairs,
+                    self.fit_df[i].peaks,
+                    "o",
+                )
+                ax.plot(self.fit_df[i].basepairs, self.fit_df[i].fitted)
+                ax.set_title(
+                    f"Peak {i + 1} area: {self.fit_params[i]['amplitude']: .1f}"
+                )
+                ax.grid()
+
+        fig_areas.suptitle(f"Quotient: {self.quotient: .2f}")
+        fig_areas.legend(["Raw data", "Model"])
+        fig_areas.supxlabel("basepairs")
+        fig_areas.supylabel("intensity")
+        plt.close()
+
+        return fig_areas
+
     def fit_assay_peaks(
         self,
         peak_finding_model: str,
         assay_number: int,
+        name: str,
     ) -> None:
         """
         Runs fit_lmfit_model, calculate_quotient and peak_position_area_dataframe
         """
         self.fit_lmfit_model(peak_finding_model, assay_number)
         self.calculate_quotient()
-        self.peak_position_area_dataframe(assay_number)
+        self.peak_position_area_dataframe(assay_number, name)
+        # area plots
+        area_plot = self.plot_areas(peak_finding_model)
+        self.area_plots.append(area_plot)
         return self.assay_peak_area_df
 
     def assays_dataframe(self, peak_finding_model: str = "gauss"):
         dfs = []
         for i in self:
-            dfs.append(self.fit_assay_peaks(peak_finding_model, i))
-        return pd.concat(dfs, ignore_index=True)
+            if self.peaks.custom_peaks is not None:
+                name = self.peaks.custom_peaks.name.unique()[i]
+            else:
+                name = ""
+            dfs.append(self.fit_assay_peaks(peak_finding_model, i, name))
+        df = pd.concat(dfs, ignore_index=True)
+        # initialize attribute self.final_df
+        self.final_df = df
+        return df
```

### Comparing `fraggler-2.0.0/fraggler/cli.py` & `fraggler-2.0.1/fraggler/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
           ░▓█▒  ░▒██▀▀█▄  ░██▄▄▄▄██ ░▓█  ██▓░▓█  ██▓▒██░    ▒▓█  ▄ ▒██▀▀█▄
           ░▒█░   ░██▓ ▒██▒ ▓█   ▓██▒░▒▓███▀▒░▒▓███▀▒░██████▒░▒████▒░██▓ ▒██▒
            ▒ ░   ░ ▒▓ ░▒▓░ ▒▒   ▓▒█░ ░▒   ▒  ░▒   ▒ ░ ▒░▓  ░░░ ▒░ ░░ ▒▓ ░▒▓░
            ░       ░▒ ░ ▒░  ▒   ▒▒ ░  ░   ░   ░   ░ ░ ░ ▒  ░ ░ ░  ░  ░▒ ░ ▒░
            ░ ░     ░░   ░   ░   ▒   ░ ░   ░ ░ ░   ░   ░ ░      ░     ░░   ░
                     ░           ░  ░      ░       ░     ░  ░   ░  ░   ░
 """
-print(ASCII_ART)
 
 
 def save_df_format(
     peak_dfs: list,
     out_folder: str,
     in_path: str,
     out_format: str,
@@ -132,14 +131,15 @@
             fsa = fraggler.FsaFile(file, ladder)
             report = fraggler.generate_no_peaks_report(fsa)
             out_name = out_folder / f"{file.stem}_failed.html"
             report.save(out_name)
             continue
 
         # generate report and peak table
+
         peak_dfs.append(fraggler_object.areas.assays_dataframe(peak_model))
         report = fraggler.generate_area_report(fraggler_object, peak_model)
         out_name = out_folder / f"{file.stem}_fraggler_area.html"
         report.save(out_name)
 
     # Save dataframe
     if peak_dfs:
```

### Comparing `fraggler-2.0.0/fraggler/functions/generate_peak_table.py` & `fraggler-2.0.1/fraggler/functions/generate_peak_table.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler/ladder_fitting/fit_ladder_model.py` & `fraggler-2.0.1/fraggler/ladder_fitting/fit_ladder_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
             if df.shape[0] == df.basepairs.nunique():
                 logging.info(f"Ladder fitting model: {self.model}")
                 return df
             # If not all bp are unique
             self.n_knots += 1
             self.fit_model()
 
+        # reaches only if there is a problem
         raise ModelFittingError(
             "There is a problem with the fitting of the model to the ladder"
         )
 
     def _fit_ROX_ladder(self) -> None:
         """
         Fit model with ROX ladder.
```

### Comparing `fraggler-2.0.0/fraggler/ladder_fitting/peak_ladder_assigner.py` & `fraggler-2.0.1/fraggler/ladder_fitting/peak_ladder_assigner.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler/ladders/ladders.py` & `fraggler-2.0.1/fraggler/ladders/ladders.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler/plotting/plot_channels.py` & `fraggler-2.0.1/fraggler/plotting/plot_channels.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler/plotting/plot_ladder.py` & `fraggler-2.0.1/fraggler/plotting/plot_ladder.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler/plotting/plot_peak_area.py` & `fraggler-2.0.1/fraggler/plotting/plot_peak_area.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from fraggler.applications.peak_area_multiplex import PeakAreaDeMultiplex
+from fraggler import PeakAreaDeMultiplex
+
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 class PlotPeakArea:
     def __init__(self, peak_area: PeakAreaDeMultiplex):
         self.peak_area = peak_area
 
     def plot_areas(self, peak_finding_model: str, assay_number: int):
 
-        self.peak_area.fit_assay_peaks(peak_finding_model, assay_number)
+        # TODO: this functions get called again here...
+        self.peak_area.fit_assay_peaks(peak_finding_model, assay_number, name="")
 
         fig_areas, axs = plt.subplots(
             1, len(self.peak_area.fit_df), sharey=True, figsize=(20, 10)
         )
 
         # if there is only one peak
         if len(self.peak_area.fit_df) == 1:
```

### Comparing `fraggler-2.0.0/fraggler/plotting/plot_peaks.py` & `fraggler-2.0.1/fraggler/plotting/plot_peaks.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler/reports/reports.py` & `fraggler-2.0.1/fraggler/reports/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     make_fraggler_peak,
     make_fraggler_area,
 )
 from ..utils.fsa_file import FsaFile
 from ..plotting.plot_channels import plot_fsa_data
 from ..plotting.plot_peaks import PlotPeaks
 from ..plotting.plot_ladder import PlotLadder
-from ..plotting.plot_peak_area import PlotPeakArea
 
 
 pn.extension("tabulator")
 pn.extension("vega", sizing_mode="stretch_width", template="fast")
 pn.widgets.Tabulator.theme = "modern"
 
 
@@ -60,30 +59,30 @@
         height=250,
     )
 
 
 def generate_peak_report(fraggler: FragglerPeak) -> pn.layout.base.Column:
     ### ----- Raw Data ----- ###
     channel_header = header(
-        text=f"## Plot of channels",
+        text="## Plot of channels",
         bg_color="#04c273",
         height=80,
         textalign="left",
     )
     # PLOT
     channel_tab = pn.Tabs()
     for plot, name in plot_fsa_data(fraggler.fsa):
         pane = pn.pane.Vega(plot.interactive(), sizing_mode="stretch_both", name=name)
         channel_tab.append(pane)
 
     channels_section = pn.Column(channel_header, channel_tab)
 
     ### ----- Peaks ----- ###
     peaks_header = header(
-        text=f"## Plot of Peaks",
+        text="## Plot of Peaks",
         bg_color="#04c273",
         height=80,
         textalign="left",
     )
 
     # PLOT
     peaks_plot = PlotPeaks(fraggler.peaks).plot_peaks
@@ -93,15 +92,15 @@
     peaks_tab = pn.Tabs(
         peaks_pane,
     )
     peaks_section = pn.Column(peaks_header, peaks_tab)
 
     ### ----- Ladder Information ----- ###
     ladder_header = header(
-        text=f"## Information about the ladder",
+        text="## Information about the ladder",
         bg_color="#04c273",
         height=80,
         textalign="left",
     )
     # Ladder peak plot
     ladder_plot = PlotLadder(fraggler.model)
     ladder_peak_plot = pn.pane.Matplotlib(
@@ -119,22 +118,19 @@
         ladder_peak_plot,
         ladder_correlation_plot,
     )
     ladder_section = pn.Column(ladder_header, ladder_tab)
 
     ### ----- Peaks dataframe ----- ###
     dataframe_header = header(
-        text=f"## Peaks Table",
-        bg_color="#04c273",
-        height=80,
-        textalign="left",
+        text="## Peaks Table", bg_color="#04c273", height=80, textalign="left"
     )
     # Create dataframe
     df = fraggler.peaks.peak_information.assign(file_name=fraggler.fsa.file_name)[
-        ["file_name", "basepairs", "peaks"]
+        ["file_name", "basepairs", "peaks", "assay_name"]
     ].rename(columns={"peaks": "peak_height"})
     # DataFrame Tabulator
     peaks_df_tab = pn.widgets.Tabulator(
         df,
         layout="fit_columns",
         pagination="local",
         page_size=15,
@@ -171,30 +167,30 @@
 def generate_area_report(
     fraggler: FragglerArea,
     peak_model: str = "gauss",
 ) -> pn.layout.base.Column:
 
     ### ----- Raw Data ----- ###
     channel_header = header(
-        text=f"## Plot of channels",
+        text="## Plot of channels",
         bg_color="#04c273",
         height=80,
         textalign="left",
     )
     # PLOT
     channel_tab = pn.Tabs()
     for plot, name in plot_fsa_data(fraggler.fsa):
         pane = pn.pane.Vega(plot.interactive(), sizing_mode="stretch_both", name=name)
         channel_tab.append(pane)
 
     channels_section = pn.Column(channel_header, channel_tab)
 
     ### ----- Peaks ----- ###
     peaks_header = header(
-        text=f"## Plot of Peaks",
+        text="## Plot of Peaks",
         bg_color="#04c273",
         height=80,
         textalign="left",
     )
 
     # PLOT
     peaks_plot = PlotPeaks(fraggler.peaks).plot_peaks
@@ -204,15 +200,15 @@
     peaks_tab = pn.Tabs(
         peaks_pane,
     )
     peaks_section = pn.Column(peaks_header, peaks_tab)
 
     ### ----- Ladder Information ----- ###
     ladder_header = header(
-        text=f"## Information about the ladder",
+        text="## Information about the ladder",
         bg_color="#04c273",
         height=80,
         textalign="left",
     )
     # Ladder peak plot
     ladder_plot = PlotLadder(fraggler.model)
     ladder_peak_plot = pn.pane.Matplotlib(
@@ -230,39 +226,34 @@
         ladder_peak_plot,
         ladder_correlation_plot,
     )
     ladder_section = pn.Column(ladder_header, ladder_tab)
 
     ### ----- Areas Information ----- ###
     areas_header = header(
-        text=f"## Peak Areas",
-        bg_color="#04c273",
-        height=80,
-        textalign="left",
+        text="## Peak Areas", bg_color="#04c273", height=80, textalign="left"
     )
     areas_tab = pn.Tabs()
-    area_plots = PlotPeakArea(fraggler.areas)
-    for assay in fraggler.areas:
-        plot = area_plots.plot_areas(peak_model, assay)
-        name = f"Assay {assay + 1}"
+    for i, plot in enumerate(fraggler.areas.area_plots):
+        name = f"Assay {i + 1}"
         plot_pane = pn.pane.Matplotlib(plot, name=name)
         areas_tab.append(plot_pane)
 
     # Section
     areas_section = pn.Column(areas_header, areas_tab)
 
     ### ----- Peaks DataFrame ----- ###
     dataframe_header = header(
-        text=f"## Peaks Table",
-        bg_color="#04c273",
-        height=80,
-        textalign="left",
+        text="## Peaks Table", bg_color="#04c273", height=80, textalign="left"
     )
-    # Create dataframe
-    df = fraggler.areas.assays_dataframe(peak_model)
+
+    if not hasattr(fraggler.areas, "final_df"):
+        df = fraggler.areas.assays_dataframe(peak_model)
+    else:
+        df = fraggler.areas.final_df
 
     # DataFrame Tabulator
     peaks_df_tab = pn.widgets.Tabulator(
         df,
         layout="fit_columns",
         pagination="local",
         page_size=15,
@@ -295,15 +286,15 @@
     )
 
     return report
 
 
 def generate_no_peaks_report(fsa: FsaFile):
     channel_header = header(
-        text=f"## Plot of channels",
+        text="## Plot of channels",
         bg_color="#04c273",
         height=80,
         textalign="left",
     )
     # PLOT
     channel_tab = pn.Tabs()
     for plot, name in plot_fsa_data(fsa):
```

### Comparing `fraggler-2.0.0/fraggler/utils/baseline_removal.py` & `fraggler-2.0.1/fraggler/utils/baseline_removal.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler/utils/fraggler_object.py` & `fraggler-2.0.1/fraggler/utils/fraggler_object.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler/utils/fsa_file.py` & `fraggler-2.0.1/fraggler/utils/fsa_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from Bio import SeqIO
 import numpy as np
 
 from fraggler.ladders.ladders import LADDERS
 from fraggler.utils.baseline_removal import baseline_arPLS
 
 
+class LadderNotFoundError(Exception):
+    pass
+
+
 class FsaFile:
     def __init__(
         self,
         file: str,
         ladder: str,
         normalize: bool = False,
         trace_channel: str = "DATA1",
@@ -35,24 +39,26 @@
             None
         """
         peak_count_padding = 3
         self.file = Path(file)
         self.file_name = self.file.parts[-1]
 
         # Extract data from the sequencing file
-        self.fsa = SeqIO.read(file, "abi").annotations["abif_raw"]
+        if ladder not in LADDERS.keys():
+            raise LadderNotFoundError(f"'{ladder}' is not a valid ladder")
         self.ladder = ladder
+        self.fsa = SeqIO.read(file, "abi").annotations["abif_raw"]
         self.trace_channel = trace_channel
         self.normalize = normalize
 
         # Extract data from the ladder reference
         self.ref_sizes = LADDERS[ladder]["sizes"]
         self.ref_count = self.ref_sizes.size
 
-        # Use default values if necessary
+        # Use default values if nothing is given
         self.size_standard_channel = size_standard_channel or LADDERS[ladder]["channel"]
         self.min_interpeak_distance = (
             min_interpeak_distance or LADDERS[ladder]["distance"]
         )
         self.min_height = min_height or LADDERS[ladder]["height"]
         self.max_ladder_trace_distance = (
             max_ladder_trace_distance or LADDERS[ladder]["max_ladder_trace_distance"]
```

### Comparing `fraggler-2.0.0/fraggler/utils/peak_finder.py` & `fraggler-2.0.1/fraggler/utils/peak_finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,46 +23,48 @@
     )
 
     if test.shape[0] != test.intervals.nunique():
         dups = (
             test.value_counts("intervals")
             .reset_index()
             .sort_values("intervals")
-            .loc[lambda x: x[0] > 1]
+            .loc[lambda x: x["count"] > 1]
             .iloc[0, 0]
         )
         logging.warning(
             f"""
         Customized peaks contains overlapping ranges
         Starting at value: {dups}
         """
         )
         return True
     return False
 
 
 def has_columns(df: pd.DataFrame) -> bool:
-    columns = set(["name", "start", "stop", "amount", "min_ratio"])
+    columns = set(
+        ["name", "start", "stop", "amount", "min_ratio", "which", "peak_distance"]
+    )
     df_columns = set(df.columns)
 
     if len(columns) != len(df_columns):
         logging.warning(
             f"""
-        Customized peaks table does not containg the right columns.
+        Customized peaks table does not contain the right columns.
         Current columns: {df_columns}
         Needed columns: {columns}
         """
         )
         return False
 
     intersection = columns.intersection(df_columns)
     if len(intersection) != len(df_columns):
         logging.warning(
             f"""
-        Customized peaks table does not containg the right columns.
+        Customized peaks table does not contain the right columns.
         Current columns: {df_columns}
         Needed columns: {columns}
         """
         )
         return False
 
     return True
@@ -173,16 +175,14 @@
         peaks_index = peak_information.peaks_index.to_numpy()
 
         # update class attributes
         self.peaks_index = peaks_index
         self.peaks_dataframe = peaks_dataframe
         self.peak_information = peak_information
 
-    # TODO
-    # add ratio to this
     def find_peaks_customized(
         self,
         peak_height: int,
     ) -> None:
 
         # Filter where to start search for the peaks
         peaks_dataframe = self.raw_data.loc[
@@ -202,22 +202,49 @@
                 peak_information.loc[lambda x: x.basepairs > assay.start]
                 .loc[lambda x: x.basepairs < assay.stop]
                 .assign(assay=assay.name)
             )
 
             # Rank the peaks by height and filter out the smallest ones
             if assay.amount != 0:
-                df = (
-                    df.assign(rank_peak=lambda x: x.peaks.rank(ascending=False))
-                    .loc[lambda x: x.rank_peak <= assay.amount]
-                    .assign(max_peak=lambda x: x.peaks.max())
-                    .assign(ratio=lambda x: x.peaks / x.max_peak)
-                    .loc[lambda x: x.ratio > assay.min_ratio]
-                    .drop(columns=["rank_peak"])
-                )
+                if assay.which == "LARGEST" or assay.which == "":
+                    df = (
+                        df.assign(max_peak=lambda x: x.peaks.max())
+                        .assign(ratio=lambda x: x.peaks / x.max_peak)
+                        .loc[lambda x: x.ratio > assay.min_ratio]
+                        .assign(rank_peak=lambda x: x.peaks.rank(ascending=False))
+                        .loc[lambda x: x.rank_peak <= assay.amount]
+                        .drop(columns=["rank_peak"])
+                    )
+                    if assay.peak_distance != 0:
+                        df = (
+                            df.assign(distance=lambda x: x.basepairs.diff())
+                            .assign(distance=lambda x: x.distance.fillna(0))
+                            .loc[lambda x: x.distance <= assay.peak_distance]
+                            .drop(columns=["distance"])
+                        )
+
+                elif assay.which == "FIRST":
+                    df = (
+                        df.assign(max_peak=lambda x: x.peaks.max())
+                        .assign(ratio=lambda x: x.peaks / x.max_peak)
+                        .loc[lambda x: x.ratio > assay.min_ratio]
+                        .sort_values("basepairs", ascending=True)
+                        .head(assay.amount)
+                    )
+                    if assay.peak_distance != 0:
+                        df = (
+                            df.assign(distance=lambda x: x.basepairs.diff())
+                            .assign(distance=lambda x: x.distance.fillna(0))
+                            .loc[lambda x: x.distance <= assay.peak_distance]
+                            .drop(columns=["distance"])
+                        )
+                else:
+                    print("[ERROR]: column `which` must be `FIRST` or `LARGEST`")
+                    exit(1)
 
             customized_peaks.append(df)
 
         peak_information = (
             pd.concat(customized_peaks)
             .reset_index()
             .assign(peak_name=lambda x: range(1, x.shape[0] + 1))
```

### Comparing `fraggler-2.0.0/fraggler/utils/utils.py` & `fraggler-2.0.1/fraggler/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fraggler-2.0.0/fraggler.egg-info/PKG-INFO` & `fraggler-2.0.1/fraggler.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fraggler
-Version: 2.0.0
+Version: 2.0.1
 Summary: Fragment Analysis package in python!
 Home-page: https://github.com/willros/fraggler
 Author: William Rosenbaum and Pär Larsson
 Author-email: william.rosenbaum@umu.se
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -21,60 +21,87 @@
 Requires-Dist: bokeh==3.3.4
 Requires-Dist: fire
 Requires-Dist: openpyxl
 Requires-Dist: colorama
 Requires-Dist: altair
 Requires-Dist: setuptools
 
-# Fraggler
+![Build Status](https://github.com/clinical-genomics-umea/fraggler/actions/workflows/pdoc.yaml/badge.svg)
+[![!pypi](https://img.shields.io/pypi/v/fraggler?color=cyan)](https://pypi.org/project/fraggler/)
+[![Download Status](https://static.pepy.tech/badge/fraggler)](https://pypi.python.org/pypi/fraggler/)
+
 ![logo](examples/logo.png)
 
 ## Description
 Fraggler is for fragment analysis in Python!
-Fraggler is a Python package that provides functionality for analyzing and generating reports for fsa files. It offers both a Python API and a command-line tool for ease of use.
+Fraggler is a Python package that provides functionality for analyzing and generating reports for fsa files. It offers both a Python API and a command-line tool.
 
 ----------------
 
 ### Features
 `Peak Area Report Generation`: Fraggler allows you to generate peak area reports for all input files. The package calculates peak areas based on specified parameters and generates a report summarizing the results.
 
 `Combined Peak Table Generation`: Fraggler provides a command-line tool to generate a combined dataframe of peaks for all input files. This allows you to easily analyze and compare peaks across multiple files.
 
 `Customization Options`: Fraggler offers various customization options to tailor the analysis to your specific needs. You can specify parameters such as ladder type, peak model, minimum ratio, minimum height, cutoff value, trace channel, peak height, and even provide a custom peaks file for specific assays and intervals.
 
 ## Install
 
-Via pip:
 ```bash
 pip install fraggler
 ```
 
-## Usage
+### Dependencies
+Fraggler depends on:
+- pandas
+- numpy
+- scikit-learn
+- networkx
+- lmfit
+- scipy
+- biopython
+- panel
+- fire
+- colorama
+- altair
+
+## Python API
 
-To get an overview how the library can be used in a python environment, please look at `tutorial.ipynb`.
+To get an overview how the library can be used in a python environment, please look at the [tutorial.ipynb](demo/tutorial.ipynb).
 
 
-## CLI Tool
+## CLI
 ### `fraggler area` and `fraggler peak`
 
 #### Usage
 To generate peak area reports and a peak table for all input files, use the `fraggler area` or `fraggler peak` command followed by the required positional arguments and any optional flags.
 
-- If not specified, fraggler finds peaks agnostic in the `fsa file`. To specifiy custom assays with certain peaks and intervals, the user can add a .csv file to the `--custom_peaks` argument. The csv file MUST have the following shape:
-
-| name | start | stop | amount | min_ratio |
-|------|-------|------|--------|-----------|
-| prt1 | 140   | 150  | 2      | 0.2       |
+- If not specified, fraggler finds peaks agnostic in the `fsa file`. To specifiy custom assays with certain peaks and intervals, the user can add a .csv file to the `--custom_peaks` argument. The csv file **MUST** have the following shape:
 
+| name | start | stop | amount | min_ratio | which | peak_distance |
+|------|-------|------|--------|-----------|-------|---------------|
+| prt1 | 140   | 150  | 2      | 0.2       | FIRST | 5             |
+
+##### Example how how a file could look:
+```txt 
+name,start,stop,amount,min_ratio,which,peak_distance
+prt1,135,155,2,0.2,FIRST,
+prt3,190,205,,0.2,FIRST,
+prt2,222,236,2,0.2,FIRST,5
+prt4,262,290,5,,,
+```
 
-If `amount` or `min_ratio` are left emtpy, `fraggler` will take all peaks inside the interval. If amount is not empty, fraggler will include the top `N` peaks in the interval, based on height. If `min_ratio` is set, only peaks with the a ratio of the `min_ratio` of the highest peak is included, *e.g.* if `min_ratio == .02`, only peaks with a height of 20 is included, if the highest peak is 100 units.
+- `name`: Name of the assay
+- `start`: Start of the assay in basepairs
+- `stop`: Stop of the assay in basepairs
+- `amount`: Optional. Amount of peaks in assay. If left empty every peak in the interval is included. 
+- `min_ratio`: Optional. Only peaks with the a ratio of the `min_ratio` of the highest peak is included, *e.g.* if `min_ratio == .02`, only peaks with a height of 20 is included, if the highest peak is 100 units
+- `which`: *LARGEST | FIRST*. Can be left empty. Which peak should be included if there are more peaks than the `amount`. if *FIRST* is set, then the two first peaks are chosen. If *LARGEST* are set, then the two largests peaks in the area are chosen. Defaults to *LARGEST*
+- `peak_distance`: Optional. Distance between peaks must be ***under*** this value.
 
-```console
-fraggler peak IN_PATH OUT_FOLDER --ladder LIZ <flags>
-```
 
 #### Positional Arguments
 The following positional arguments are required:
 
 - `IN_PATH`: Type `str`. Specifies the input path.
 - `OUT_FOLDER`: Type `str`. Specifies the output folder.
 - `LADDER`: Type `str`. Specifies the ladder used in the experiment.
@@ -90,17 +117,18 @@
 - `-t, --trace_channel=TRACE_CHANNEL`: Type `str`. Specifies the trace channel. Default value: 'DATA9'.
 - `--peak_height=PEAK_HEIGHT`: Type `int`. Specifies the peak height. Default value: 200.
 - `--custom_peaks=CUSTOM_PEAKS`: Type `Optional[str]`. Specifies custom peaks. Default value: None.
 - `-e, --excel=EXCEL`: Type: `bool`, Default: True
 
 #### Typical usage
 ```console
-fraggler peak IN_FOLDER OUT_FOLDER ORANGE --min_ratio=0.2 
+fraggler area IN_FOLDER OUT_FOLDER LIZ --min_ratio=0.2 
 ```
 
+#### Documentation
+Click [here](https://clinical-genomics-umea.github.io/fraggler/fraggler.html) to get full documentation of API.
 
+## Output
+One example of the report generated from `fraggler area` can be seen here: [Example report](examples/multiplex_fraggler_area.html)
 
-
-
-
-
-
+## Contributions
+Please check out [How to contribute](CONTRIBUTION.md)
```

### Comparing `fraggler-2.0.0/fraggler.egg-info/SOURCES.txt` & `fraggler-2.0.1/fraggler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-setup.cfg
 setup.py
 fraggler/__init__.py
 fraggler/cli.py
 fraggler.egg-info/PKG-INFO
 fraggler.egg-info/SOURCES.txt
 fraggler.egg-info/dependency_links.txt
 fraggler.egg-info/entry_points.txt
```

### Comparing `fraggler-2.0.0/setup.py` & `fraggler-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setuptools.setup(
     name="fraggler",
-    version="2.0.0",
+    version="2.0.1",
     description="Fragment Analysis package in python!",
     url="https://github.com/willros/fraggler",
     author="William Rosenbaum and Pär Larsson",
     author_email="william.rosenbaum@umu.se",
     license="MIT",
     packages=setuptools.find_packages(),
     long_description=long_description,
```


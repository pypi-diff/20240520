# Comparing `tmp/plotnineseqsuite-1.1.0.tar.gz` & `tmp/plotnineseqsuite-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotnineseqsuite-1.1.0.tar", last modified: Fri Mar  8 04:04:00 2024, max compression
+gzip compressed data, was "plotnineseqsuite-1.1.1.tar", last modified: Mon May 20 07:43:32 2024, max compression
```

## Comparing `plotnineseqsuite-1.1.0.tar` & `plotnineseqsuite-1.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 04:04:00.716500 plotnineseqsuite-1.1.0/
--rw-rw-rw-   0        0        0     1087 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1760 2024-03-08 04:04:00.699510 plotnineseqsuite-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1002 2024-03-08 02:53:50.000000 plotnineseqsuite-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-08 04:03:59.787157 plotnineseqsuite-1.1.0/plotnineseqsuite/
--rw-rw-rw-   0        0        0      384 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/__init__.py
--rw-rw-rw-   0        0        0     9312 2024-03-08 01:49:11.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/align.py
--rw-rw-rw-   0        0        0     8531 2024-03-08 01:49:11.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/bar.py
--rw-rw-rw-   0        0        0     5433 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/col_schemes.py
--rw-rw-rw-   0        0        0     2481 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/common.py
-drwxrwxrwx   0        0        0        0 2024-03-08 04:03:59.856755 plotnineseqsuite-1.1.0/plotnineseqsuite/data/
--rw-rw-rw-   0        0        0    21403 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-08 04:04:00.381994 plotnineseqsuite-1.1.0/plotnineseqsuite/font/
--rw-rw-rw-   0        0        0     1844 2024-03-08 02:49:33.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/__init__.py
--rw-rw-rw-   0        0        0   171830 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/akrobat_bold.csv
--rw-rw-rw-   0        0        0   179244 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/akrobat_regular.csv
--rw-rw-rw-   0        0        0   320265 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/arial.csv
--rw-rw-rw-   0        0        0   444613 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/courier_new.csv
--rw-rw-rw-   0        0        0   302058 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/helvetica_bold.csv
--rw-rw-rw-   0        0        0   339579 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/helvetica_light.csv
--rw-rw-rw-   0        0        0   324716 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/helvetica_regular.csv
--rw-rw-rw-   0        0        0   297471 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_bold.csv
--rw-rw-rw-   0        0        0   302627 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_medium.csv
--rw-rw-rw-   0        0        0   310129 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_regular.csv
--rw-rw-rw-   0        0        0   204700 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_slab_bold.csv
--rw-rw-rw-   0        0        0   222455 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_slab_light.csv
--rw-rw-rw-   0        0        0   204700 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_slab_regular.csv
--rw-rw-rw-   0        0        0   455686 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/times_new_roman.csv
--rw-rw-rw-   0        0        0   366621 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/font/xkcd_regular.csv
--rw-rw-rw-   0        0        0    11639 2024-03-08 01:45:28.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/logo.py
--rw-rw-rw-   0        0        0      260 2024-03-08 01:49:11.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/theme.py
--rw-rw-rw-   0        0        0     2139 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/plotnineseqsuite/tool.py
-drwxrwxrwx   0        0        0        0 2024-03-08 04:03:59.833454 plotnineseqsuite-1.1.0/plotnineseqsuite.egg-info/
--rw-rw-rw-   0        0        0     1760 2024-03-08 04:03:58.000000 plotnineseqsuite-1.1.0/plotnineseqsuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1319 2024-03-08 04:03:59.000000 plotnineseqsuite-1.1.0/plotnineseqsuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 04:03:58.000000 plotnineseqsuite-1.1.0/plotnineseqsuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-08 04:03:58.000000 plotnineseqsuite-1.1.0/plotnineseqsuite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-08 04:03:58.000000 plotnineseqsuite-1.1.0/plotnineseqsuite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-08 04:04:00.718500 plotnineseqsuite-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1188 2024-03-08 02:53:50.000000 plotnineseqsuite-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 04:04:00.696513 plotnineseqsuite-1.1.0/tests/
--rw-rw-rw-   0        0        0     1013 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/tests/test_align.py
--rw-rw-rw-   0        0        0     1035 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/tests/test_bar.py
--rw-rw-rw-   0        0        0     1376 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/tests/test_col_schemes.py
--rw-rw-rw-   0        0        0      612 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/tests/test_common.py
--rw-rw-rw-   0        0        0     1213 2024-03-08 02:46:50.000000 plotnineseqsuite-1.1.0/tests/test_font.py
--rw-rw-rw-   0        0        0     5439 2024-03-08 02:58:15.000000 plotnineseqsuite-1.1.0/tests/test_index.py
--rw-rw-rw-   0        0        0     6641 2024-03-08 02:25:55.000000 plotnineseqsuite-1.1.0/tests/test_logo.py
--rw-rw-rw-   0        0        0    10315 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/tests/test_paper.py
--rw-rw-rw-   0        0        0      762 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/tests/test_tool.py
--rw-rw-rw-   0        0        0     1056 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.0/tests/test_zoom.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:43:32.418827 plotnineseqsuite-1.1.1/
+-rw-rw-rw-   0        0        0     1119 2024-03-08 05:38:31.000000 plotnineseqsuite-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1793 2024-05-20 07:43:32.415830 plotnineseqsuite-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1002 2024-05-20 07:33:43.000000 plotnineseqsuite-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 07:43:32.118012 plotnineseqsuite-1.1.1/plotnineseqsuite/
+-rw-rw-rw-   0        0        0      384 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/__init__.py
+-rw-rw-rw-   0        0        0     9312 2024-03-08 01:49:11.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/align.py
+-rw-rw-rw-   0        0        0     8531 2024-03-08 01:49:11.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/bar.py
+-rw-rw-rw-   0        0        0     5433 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/col_schemes.py
+-rw-rw-rw-   0        0        0     2481 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/common.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:43:32.177976 plotnineseqsuite-1.1.1/plotnineseqsuite/data/
+-rw-rw-rw-   0        0        0    21403 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:43:32.263922 plotnineseqsuite-1.1.1/plotnineseqsuite/font/
+-rw-rw-rw-   0        0        0     1844 2024-03-08 02:49:33.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/__init__.py
+-rw-rw-rw-   0        0        0   171830 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/akrobat_bold.csv
+-rw-rw-rw-   0        0        0   179244 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/akrobat_regular.csv
+-rw-rw-rw-   0        0        0   320265 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/arial.csv
+-rw-rw-rw-   0        0        0   444613 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/courier_new.csv
+-rw-rw-rw-   0        0        0   302058 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/helvetica_bold.csv
+-rw-rw-rw-   0        0        0   339579 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/helvetica_light.csv
+-rw-rw-rw-   0        0        0   324716 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/helvetica_regular.csv
+-rw-rw-rw-   0        0        0   297471 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_bold.csv
+-rw-rw-rw-   0        0        0   302627 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_medium.csv
+-rw-rw-rw-   0        0        0   310129 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_regular.csv
+-rw-rw-rw-   0        0        0   204700 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_slab_bold.csv
+-rw-rw-rw-   0        0        0   222455 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_slab_light.csv
+-rw-rw-rw-   0        0        0   204700 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_slab_regular.csv
+-rw-rw-rw-   0        0        0   455686 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/times_new_roman.csv
+-rw-rw-rw-   0        0        0   366621 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/font/xkcd_regular.csv
+-rw-rw-rw-   0        0        0    11639 2024-03-08 01:45:28.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/logo.py
+-rw-rw-rw-   0        0        0      260 2024-03-08 01:49:11.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/theme.py
+-rw-rw-rw-   0        0        0     2139 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/plotnineseqsuite/tool.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:43:32.174977 plotnineseqsuite-1.1.1/plotnineseqsuite.egg-info/
+-rw-rw-rw-   0        0        0     1793 2024-05-20 07:43:31.000000 plotnineseqsuite-1.1.1/plotnineseqsuite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1319 2024-05-20 07:43:31.000000 plotnineseqsuite-1.1.1/plotnineseqsuite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:43:31.000000 plotnineseqsuite-1.1.1/plotnineseqsuite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 07:43:31.000000 plotnineseqsuite-1.1.1/plotnineseqsuite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 07:43:31.000000 plotnineseqsuite-1.1.1/plotnineseqsuite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:43:32.418827 plotnineseqsuite-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1188 2024-05-20 07:41:37.000000 plotnineseqsuite-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:43:32.413829 plotnineseqsuite-1.1.1/tests/
+-rw-rw-rw-   0        0        0     1013 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/tests/test_align.py
+-rw-rw-rw-   0        0        0     1035 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/tests/test_bar.py
+-rw-rw-rw-   0        0        0     1376 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/tests/test_col_schemes.py
+-rw-rw-rw-   0        0        0      612 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/tests/test_common.py
+-rw-rw-rw-   0        0        0     1213 2024-03-08 02:46:50.000000 plotnineseqsuite-1.1.1/tests/test_font.py
+-rw-rw-rw-   0        0        0     5439 2024-03-08 02:58:15.000000 plotnineseqsuite-1.1.1/tests/test_index.py
+-rw-rw-rw-   0        0        0     6641 2024-03-08 02:25:55.000000 plotnineseqsuite-1.1.1/tests/test_logo.py
+-rw-rw-rw-   0        0        0    10315 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/tests/test_paper.py
+-rw-rw-rw-   0        0        0      762 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/tests/test_tool.py
+-rw-rw-rw-   0        0        0     1056 2023-09-15 00:38:30.000000 plotnineseqsuite-1.1.1/tests/test_zoom.py
```

### Comparing `plotnineseqsuite-1.1.0/LICENSE` & `plotnineseqsuite-1.1.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 CaoTianze
+Copyright (c) 2023-present Cao Tianze and other contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `plotnineseqsuite-1.1.0/PKG-INFO` & `plotnineseqsuite-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotnineseqsuite
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for visualizing sequence data using ggplot2 style
 Home-page: https://github.com/caotianze/plotnineseqsuite
 Author: Cao Tianze
 Author-email: hnrcao@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/caotianze/plotnineseqsuite/issues
 Keywords: ggplot2,plotnine,Bioinformatics tool,Sequence logo,Sequence alignment
@@ -12,26 +12,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: plotnine==0.13.5
 
 # plotnineSeqSuite: a Python package for visualizing sequence data using ggplot2 style
 ## Cite this work
 Cao, T., Li, Q., Huang, Y. et al. plotnineSeqSuite: a Python package for visualizing sequence data using ggplot2 style. BMC Genomics 24, 585 (2023). https://doi.org/10.1186/s12864-023-09677-8
 ## Installation
 `pip install plotnineseqsuite`
 ## Getting Started
 See [plotnineSeqSuite Documentation](https://caotianze.github.io/plotnineseqsuite/) 
 ## Gallery
 ![https://caotianze.github.io/plotnineseqsuite/gallery.png](https://caotianze.github.io/plotnineseqsuite/gallery.png)
 ## Development environment 
 PyCharm 2023.2 (Community Edition) and Spyder version: 5.4.3  (conda)
 ## Dependencies
 Python version: 3.11.4 64-bit    
-plotnine: 0.13.1
+plotnine: 0.13.5
 ## Similar projects
 R package [ggmsa](https://github.com/YuLab-SMU/ggmsa) and [ggseqlogo](https://github.com/omarwagih/ggseqlogo)
 ## Derivative projects
 - [Pyggseqlogo](https://github.com/CaoTianze/pyggseqlogo): Python version of ggseqlogo.
```

### Comparing `plotnineseqsuite-1.1.0/README.md` & `plotnineseqsuite-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 See [plotnineSeqSuite Documentation](https://caotianze.github.io/plotnineseqsuite/) 
 ## Gallery
 ![https://caotianze.github.io/plotnineseqsuite/gallery.png](https://caotianze.github.io/plotnineseqsuite/gallery.png)
 ## Development environment 
 PyCharm 2023.2 (Community Edition) and Spyder version: 5.4.3  (conda)
 ## Dependencies
 Python version: 3.11.4 64-bit    
-plotnine: 0.13.1
+plotnine: 0.13.5
 ## Similar projects
 R package [ggmsa](https://github.com/YuLab-SMU/ggmsa) and [ggseqlogo](https://github.com/omarwagih/ggseqlogo)
 ## Derivative projects
 - [Pyggseqlogo](https://github.com/CaoTianze/pyggseqlogo): Python version of ggseqlogo.
```

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/align.py` & `plotnineseqsuite-1.1.1/plotnineseqsuite/align.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/bar.py` & `plotnineseqsuite-1.1.1/plotnineseqsuite/bar.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/col_schemes.py` & `plotnineseqsuite-1.1.1/plotnineseqsuite/col_schemes.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/common.py` & `plotnineseqsuite-1.1.1/plotnineseqsuite/common.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/data/__init__.py` & `plotnineseqsuite-1.1.1/plotnineseqsuite/data/__init__.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/__init__.py` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/__init__.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/akrobat_bold.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/akrobat_bold.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/akrobat_regular.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/akrobat_regular.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/arial.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/arial.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/courier_new.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/courier_new.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/helvetica_bold.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/helvetica_bold.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/helvetica_light.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/helvetica_light.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/helvetica_regular.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/helvetica_regular.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_bold.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_bold.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_medium.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_medium.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_regular.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_regular.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_slab_bold.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_slab_bold.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_slab_light.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_slab_light.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/roboto_slab_regular.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/roboto_slab_regular.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/times_new_roman.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/times_new_roman.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/font/xkcd_regular.csv` & `plotnineseqsuite-1.1.1/plotnineseqsuite/font/xkcd_regular.csv`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/logo.py` & `plotnineseqsuite-1.1.1/plotnineseqsuite/logo.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite/tool.py` & `plotnineseqsuite-1.1.1/plotnineseqsuite/tool.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite.egg-info/PKG-INFO` & `plotnineseqsuite-1.1.1/plotnineseqsuite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotnineseqsuite
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for visualizing sequence data using ggplot2 style
 Home-page: https://github.com/caotianze/plotnineseqsuite
 Author: Cao Tianze
 Author-email: hnrcao@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/caotianze/plotnineseqsuite/issues
 Keywords: ggplot2,plotnine,Bioinformatics tool,Sequence logo,Sequence alignment
@@ -12,26 +12,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: plotnine==0.13.5
 
 # plotnineSeqSuite: a Python package for visualizing sequence data using ggplot2 style
 ## Cite this work
 Cao, T., Li, Q., Huang, Y. et al. plotnineSeqSuite: a Python package for visualizing sequence data using ggplot2 style. BMC Genomics 24, 585 (2023). https://doi.org/10.1186/s12864-023-09677-8
 ## Installation
 `pip install plotnineseqsuite`
 ## Getting Started
 See [plotnineSeqSuite Documentation](https://caotianze.github.io/plotnineseqsuite/) 
 ## Gallery
 ![https://caotianze.github.io/plotnineseqsuite/gallery.png](https://caotianze.github.io/plotnineseqsuite/gallery.png)
 ## Development environment 
 PyCharm 2023.2 (Community Edition) and Spyder version: 5.4.3  (conda)
 ## Dependencies
 Python version: 3.11.4 64-bit    
-plotnine: 0.13.1
+plotnine: 0.13.5
 ## Similar projects
 R package [ggmsa](https://github.com/YuLab-SMU/ggmsa) and [ggseqlogo](https://github.com/omarwagih/ggseqlogo)
 ## Derivative projects
 - [Pyggseqlogo](https://github.com/CaoTianze/pyggseqlogo): Python version of ggseqlogo.
```

### Comparing `plotnineseqsuite-1.1.0/plotnineseqsuite.egg-info/SOURCES.txt` & `plotnineseqsuite-1.1.1/plotnineseqsuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/setup.py` & `plotnineseqsuite-1.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotnineseqsuite",
-    version="1.1.0",
+    version="1.1.1",
     author="Cao Tianze",
     author_email="hnrcao@qq.com",
     description="A Python package for visualizing sequence data using ggplot2 style",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/caotianze/plotnineseqsuite",
     project_urls={
@@ -20,14 +20,14 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=['plotnineseqsuite','plotnineseqsuite.font','plotnineseqsuite.data'],
     python_requires=">=3.11",
-    install_requires=['plotnine==0.13.1'],
+    install_requires=['plotnine==0.13.5'],
     license="MIT",
     keywords=['ggplot2', 'plotnine', 'Bioinformatics tool', 'Sequence logo', 'Sequence alignment'],
     package_data={
         "": ["*.csv"]
     }
 )
```

### Comparing `plotnineseqsuite-1.1.0/tests/test_align.py` & `plotnineseqsuite-1.1.1/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_bar.py` & `plotnineseqsuite-1.1.1/tests/test_bar.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_col_schemes.py` & `plotnineseqsuite-1.1.1/tests/test_col_schemes.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_common.py` & `plotnineseqsuite-1.1.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_font.py` & `plotnineseqsuite-1.1.1/tests/test_font.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_index.py` & `plotnineseqsuite-1.1.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_logo.py` & `plotnineseqsuite-1.1.1/tests/test_logo.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_paper.py` & `plotnineseqsuite-1.1.1/tests/test_paper.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_tool.py` & `plotnineseqsuite-1.1.1/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `plotnineseqsuite-1.1.0/tests/test_zoom.py` & `plotnineseqsuite-1.1.1/tests/test_zoom.py`

 * *Files identical despite different names*


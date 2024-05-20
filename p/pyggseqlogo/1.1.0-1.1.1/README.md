# Comparing `tmp/pyggseqlogo-1.1.0.tar.gz` & `tmp/pyggseqlogo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyggseqlogo-1.1.0.tar", last modified: Fri Mar  8 05:32:55 2024, max compression
+gzip compressed data, was "pyggseqlogo-1.1.1.tar", last modified: Mon May 20 07:54:43 2024, max compression
```

## Comparing `pyggseqlogo-1.1.0.tar` & `pyggseqlogo-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 05:32:55.005030 pyggseqlogo-1.1.0/
--rw-rw-rw-   0        0        0     1087 2023-08-17 13:06:36.000000 pyggseqlogo-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2321 2024-03-08 05:32:55.005030 pyggseqlogo-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1562 2023-10-21 14:58:52.000000 pyggseqlogo-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-08 05:32:54.958152 pyggseqlogo-1.1.0/pyggseqlogo/
--rw-rw-rw-   0        0        0       82 2023-08-17 13:06:36.000000 pyggseqlogo-1.1.0/pyggseqlogo/__init__.py
--rw-rw-rw-   0        0        0      660 2023-08-17 13:06:36.000000 pyggseqlogo-1.1.0/pyggseqlogo/logo.py
--rw-rw-rw-   0        0        0      596 2024-03-08 05:28:51.000000 pyggseqlogo-1.1.0/pyggseqlogo/theme.py
-drwxrwxrwx   0        0        0        0 2024-03-08 05:32:55.005030 pyggseqlogo-1.1.0/pyggseqlogo.egg-info/
--rw-rw-rw-   0        0        0     2321 2024-03-08 05:32:54.000000 pyggseqlogo-1.1.0/pyggseqlogo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-03-08 05:32:54.000000 pyggseqlogo-1.1.0/pyggseqlogo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 05:32:54.000000 pyggseqlogo-1.1.0/pyggseqlogo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-03-08 05:32:54.000000 pyggseqlogo-1.1.0/pyggseqlogo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-08 05:32:54.000000 pyggseqlogo-1.1.0/pyggseqlogo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-08 05:32:55.005030 pyggseqlogo-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1138 2024-03-08 05:27:34.000000 pyggseqlogo-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 05:32:55.005030 pyggseqlogo-1.1.0/tests/
--rw-rw-rw-   0        0        0      288 2023-09-05 05:50:48.000000 pyggseqlogo-1.1.0/tests/test_ggseqlogo.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:54:43.387998 pyggseqlogo-1.1.1/
+-rw-rw-rw-   0        0        0     1119 2024-03-08 05:38:51.000000 pyggseqlogo-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2361 2024-05-20 07:54:43.382001 pyggseqlogo-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1562 2023-10-21 14:58:52.000000 pyggseqlogo-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 07:54:43.336032 pyggseqlogo-1.1.1/pyggseqlogo/
+-rw-rw-rw-   0        0        0       82 2023-08-17 13:06:36.000000 pyggseqlogo-1.1.1/pyggseqlogo/__init__.py
+-rw-rw-rw-   0        0        0      660 2023-08-17 13:06:36.000000 pyggseqlogo-1.1.1/pyggseqlogo/logo.py
+-rw-rw-rw-   0        0        0      596 2024-03-08 05:28:51.000000 pyggseqlogo-1.1.1/pyggseqlogo/theme.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:54:43.371009 pyggseqlogo-1.1.1/pyggseqlogo.egg-info/
+-rw-rw-rw-   0        0        0     2361 2024-05-20 07:54:42.000000 pyggseqlogo-1.1.1/pyggseqlogo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-05-20 07:54:43.000000 pyggseqlogo-1.1.1/pyggseqlogo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:54:42.000000 pyggseqlogo-1.1.1/pyggseqlogo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-20 07:54:42.000000 pyggseqlogo-1.1.1/pyggseqlogo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 07:54:42.000000 pyggseqlogo-1.1.1/pyggseqlogo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:54:43.389996 pyggseqlogo-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-05-20 07:53:58.000000 pyggseqlogo-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:54:43.378005 pyggseqlogo-1.1.1/tests/
+-rw-rw-rw-   0        0        0      288 2023-09-05 05:50:48.000000 pyggseqlogo-1.1.1/tests/test_ggseqlogo.py
```

### Comparing `pyggseqlogo-1.1.0/LICENSE` & `pyggseqlogo-1.1.1/LICENSE`

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

### Comparing `pyggseqlogo-1.1.0/PKG-INFO` & `pyggseqlogo-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyggseqlogo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python version of ggseqlogo. Based on plotnine (Python version of ggplot2). A derivative of plotnineSeqSuite.
 Home-page: https://github.com/caotianze/pyggseqlogo
 Author: Cao Tianze
 Author-email: hnrcao@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/caotianze/pyggseqlogo/issues
 Keywords: ggplot2,plotnine,ggseqlogo,Sequence logo
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: plotnineseqsuite==1.1.2
 
 # Pyggseqlogo
 Python version of [ggseqlogo](https://github.com/omarwagih/ggseqlogo). Based on [plotnine](https://github.com/has2k1/plotnine/) (Python version of ggplot2). A derivative of [plotnineSeqSuite](https://github.com/caotianze/plotnineseqsuite/).
 ## Cite this work
 Cao, T., Li, Q., Huang, Y. et al. plotnineSeqSuite: a Python package for visualizing sequence data using ggplot2 style. BMC Genomics 24, 585 (2023). https://doi.org/10.1186/s12864-023-09677-8
 ## Installation
 `pip install pyggseqlogo`
```

### Comparing `pyggseqlogo-1.1.0/README.md` & `pyggseqlogo-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyggseqlogo-1.1.0/pyggseqlogo/logo.py` & `pyggseqlogo-1.1.1/pyggseqlogo/logo.py`

 * *Files identical despite different names*

### Comparing `pyggseqlogo-1.1.0/pyggseqlogo/theme.py` & `pyggseqlogo-1.1.1/pyggseqlogo/theme.py`

 * *Files identical despite different names*

### Comparing `pyggseqlogo-1.1.0/pyggseqlogo.egg-info/PKG-INFO` & `pyggseqlogo-1.1.1/pyggseqlogo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyggseqlogo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python version of ggseqlogo. Based on plotnine (Python version of ggplot2). A derivative of plotnineSeqSuite.
 Home-page: https://github.com/caotianze/pyggseqlogo
 Author: Cao Tianze
 Author-email: hnrcao@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/caotianze/pyggseqlogo/issues
 Keywords: ggplot2,plotnine,ggseqlogo,Sequence logo
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: plotnineseqsuite==1.1.2
 
 # Pyggseqlogo
 Python version of [ggseqlogo](https://github.com/omarwagih/ggseqlogo). Based on [plotnine](https://github.com/has2k1/plotnine/) (Python version of ggplot2). A derivative of [plotnineSeqSuite](https://github.com/caotianze/plotnineseqsuite/).
 ## Cite this work
 Cao, T., Li, Q., Huang, Y. et al. plotnineSeqSuite: a Python package for visualizing sequence data using ggplot2 style. BMC Genomics 24, 585 (2023). https://doi.org/10.1186/s12864-023-09677-8
 ## Installation
 `pip install pyggseqlogo`
```

### Comparing `pyggseqlogo-1.1.0/setup.py` & `pyggseqlogo-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyggseqlogo",
-    version="1.1.0",
+    version="1.1.1",
     author="Cao Tianze",
     author_email="hnrcao@qq.com",
     description="Python version of ggseqlogo. Based on plotnine (Python version of ggplot2). A derivative of plotnineSeqSuite.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/caotianze/pyggseqlogo",
     project_urls={
@@ -20,14 +20,14 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=['pyggseqlogo'],
     python_requires=">=3.11",
-    install_requires=['plotnineseqsuite==1.1.0'],
+    install_requires=['plotnineseqsuite==1.1.2'],
     license="MIT",
     keywords=['ggplot2', 'plotnine', 'ggseqlogo', 'Sequence logo'],
     package_data={
         "": ["*.csv"]
     }
 )
```


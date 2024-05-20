# Comparing `tmp/rdatapp-0.7.tar.gz` & `tmp/rdatapp-0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdatapp-0.7.tar", last modified: Mon May 20 11:55:39 2024, max compression
+gzip compressed data, was "rdatapp-0.7a0.tar", last modified: Mon May 20 11:49:34 2024, max compression
```

## Comparing `rdatapp-0.7.tar` & `rdatapp-0.7a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:55:39.736243 rdatapp-0.7/
--rw-r--r--   0 ifozmen    (501) staff       (20)     5369 2024-05-20 11:55:39.735931 rdatapp-0.7/PKG-INFO
--rw-r--r--   0 ifozmen    (501) staff       (20)     3914 2024-05-20 11:39:34.000000 rdatapp-0.7/README.md
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:55:39.734150 rdatapp-0.7/rdatapp/
--rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.7/rdatapp/__init__.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1823 2024-05-20 10:38:30.000000 rdatapp-0.7/rdatapp/categorical_encoder.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1404 2024-05-20 10:39:16.000000 rdatapp-0.7/rdatapp/data_type_converter.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1474 2024-05-20 10:39:41.000000 rdatapp-0.7/rdatapp/datetime_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)      969 2024-05-20 10:42:18.000000 rdatapp-0.7/rdatapp/feature_engineer.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     2638 2024-05-20 10:44:02.000000 rdatapp-0.7/rdatapp/missing_value_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1155 2024-05-20 10:45:07.000000 rdatapp-0.7/rdatapp/outlier_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1464 2024-05-20 10:45:34.000000 rdatapp-0.7/rdatapp/scaler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1389 2024-05-20 10:46:15.000000 rdatapp-0.7/rdatapp/text_cleaner.py
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:55:39.735441 rdatapp-0.7/rdatapp.egg-info/
--rw-r--r--   0 ifozmen    (501) staff       (20)     5369 2024-05-20 11:55:39.000000 rdatapp-0.7/rdatapp.egg-info/PKG-INFO
--rw-r--r--   0 ifozmen    (501) staff       (20)      412 2024-05-20 11:55:39.000000 rdatapp-0.7/rdatapp.egg-info/SOURCES.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-20 11:55:39.000000 rdatapp-0.7/rdatapp.egg-info/dependency_links.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       31 2024-05-20 11:55:39.000000 rdatapp-0.7/rdatapp.egg-info/requires.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-20 11:55:39.000000 rdatapp-0.7/rdatapp.egg-info/top_level.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-20 11:55:39.736307 rdatapp-0.7/setup.cfg
--rw-rw-r--   0 ifozmen    (501) staff       (20)     1793 2024-05-20 11:55:17.000000 rdatapp-0.7/setup.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:49:34.451567 rdatapp-0.7a0/
+-rw-r--r--   0 ifozmen    (501) staff       (20)     5280 2024-05-20 11:49:34.451389 rdatapp-0.7a0/PKG-INFO
+-rw-r--r--   0 ifozmen    (501) staff       (20)     3914 2024-05-20 11:39:34.000000 rdatapp-0.7a0/README.md
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:49:34.450057 rdatapp-0.7a0/rdatapp/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.7a0/rdatapp/__init__.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1823 2024-05-20 10:38:30.000000 rdatapp-0.7a0/rdatapp/categorical_encoder.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1404 2024-05-20 10:39:16.000000 rdatapp-0.7a0/rdatapp/data_type_converter.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1474 2024-05-20 10:39:41.000000 rdatapp-0.7a0/rdatapp/datetime_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)      969 2024-05-20 10:42:18.000000 rdatapp-0.7a0/rdatapp/feature_engineer.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     2638 2024-05-20 10:44:02.000000 rdatapp-0.7a0/rdatapp/missing_value_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1155 2024-05-20 10:45:07.000000 rdatapp-0.7a0/rdatapp/outlier_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1464 2024-05-20 10:45:34.000000 rdatapp-0.7a0/rdatapp/scaler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1389 2024-05-20 10:46:15.000000 rdatapp-0.7a0/rdatapp/text_cleaner.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:49:34.450984 rdatapp-0.7a0/rdatapp.egg-info/
+-rw-r--r--   0 ifozmen    (501) staff       (20)     5280 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/PKG-INFO
+-rw-r--r--   0 ifozmen    (501) staff       (20)      412 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/SOURCES.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/dependency_links.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       31 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/requires.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/top_level.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-20 11:49:34.451624 rdatapp-0.7a0/setup.cfg
+-rw-rw-r--   0 ifozmen    (501) staff       (20)     1794 2024-05-20 11:49:24.000000 rdatapp-0.7a0/setup.py
```

### Comparing `rdatapp-0.7/PKG-INFO` & `rdatapp-0.7a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdatapp
-Version: 0.7
+Version: 0.7a0
 Summary: A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding, and more.
 Home-page: https://github.com/Beegash/Recoded-Data-Processing-Library
 Author: Izzettin Furkan Özmen, Ismail Cifci
 Author-email: izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr
 Project-URL: Source, https://github.com/Beegash/Recoded-Data-Processing-Library
 Keywords: data preprocessing data-cleaning one-hot-encoding text-cleaning missing-value-imputation
 Classifier: Development Status :: 3 - Alpha
@@ -18,18 +18,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: scikit-learn
-Requires-Dist: nltk
 
 # RDATAPP: Recoded Data Preprocessing Library
 
 [![PyPI version](https://badge.fury.io/py/rdatapp.svg)](https://badge.fury.io/py/rdatapp)
 [![Python versions](https://img.shields.io/pypi/pyversions/rdatapp.svg)](https://pypi.python.org/pypi/rdatapp)
 [![License](https://img.shields.io/pypi/l/rdatapp.svg)](https://pypi.python.org/pypi/rdatapp)
```

### Comparing `rdatapp-0.7/README.md` & `rdatapp-0.7a0/README.md`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/__init__.py` & `rdatapp-0.7a0/rdatapp/__init__.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/categorical_encoder.py` & `rdatapp-0.7a0/rdatapp/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/data_type_converter.py` & `rdatapp-0.7a0/rdatapp/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/datetime_handler.py` & `rdatapp-0.7a0/rdatapp/datetime_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/feature_engineer.py` & `rdatapp-0.7a0/rdatapp/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/missing_value_handler.py` & `rdatapp-0.7a0/rdatapp/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/outlier_handler.py` & `rdatapp-0.7a0/rdatapp/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/scaler.py` & `rdatapp-0.7a0/rdatapp/scaler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp/text_cleaner.py` & `rdatapp-0.7a0/rdatapp/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.7/rdatapp.egg-info/PKG-INFO` & `rdatapp-0.7a0/rdatapp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdatapp
-Version: 0.7
+Version: 0.7a0
 Summary: A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding, and more.
 Home-page: https://github.com/Beegash/Recoded-Data-Processing-Library
 Author: Izzettin Furkan Özmen, Ismail Cifci
 Author-email: izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr
 Project-URL: Source, https://github.com/Beegash/Recoded-Data-Processing-Library
 Keywords: data preprocessing data-cleaning one-hot-encoding text-cleaning missing-value-imputation
 Classifier: Development Status :: 3 - Alpha
@@ -18,18 +18,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: scikit-learn
-Requires-Dist: nltk
 
 # RDATAPP: Recoded Data Preprocessing Library
 
 [![PyPI version](https://badge.fury.io/py/rdatapp.svg)](https://badge.fury.io/py/rdatapp)
 [![Python versions](https://img.shields.io/pypi/pyversions/rdatapp.svg)](https://pypi.python.org/pypi/rdatapp)
 [![License](https://img.shields.io/pypi/l/rdatapp.svg)](https://pypi.python.org/pypi/rdatapp)
```

### Comparing `rdatapp-0.7/setup.py` & `rdatapp-0.7a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rdatapp',
-    version='0.7',
+    version='0.7a',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk',
     ],
```


# Comparing `tmp/qnngds-2.5.0.tar.gz` & `tmp/qnngds-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-2.5.0.tar", last modified: Mon May 20 15:57:43 2024, max compression
+gzip compressed data, was "qnngds-2.5.1.tar", last modified: Mon May 20 16:46:51 2024, max compression
```

## Comparing `qnngds-2.5.0.tar` & `qnngds-2.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2024-05-20 15:57:30.798371 qnngds-2.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-05-20 15:57:30.798371 qnngds-2.5.0/README.md
--rw-r--r--   0        0        0     1161 2024-05-20 15:57:43.642317 qnngds-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      543 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/__init__.py
--rw-r--r--   0        0        0      290 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/_default_param.py
--rw-r--r--   0        0        0    29539 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/cells.py
--rw-r--r--   0        0        0    10385 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/circuits.py
--rw-r--r--   0        0        0    30497 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/design.py
--rw-r--r--   0        0        0      158 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/__init__.py
--rw-r--r--   0        0        0      231 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/htron.py
--rw-r--r--   0        0        0     1313 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/nanowire.py
--rw-r--r--   0        0        0     3136 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/ntron.py
--rw-r--r--   0        0        0     6365 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/resistor.py
--rw-r--r--   0        0        0     6479 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/devices/snspd.py
--rw-r--r--   0        0        0     1300 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/geometries.py
--rw-r--r--   0        0        0     8683 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/tests.py
--rw-r--r--   0        0        0    30179 2024-05-20 15:57:30.814370 qnngds-2.5.0/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3316 2024-05-20 15:57:30.814370 qnngds-2.5.0/tests/all_dev_on_gds.py
--rw-r--r--   0        0        0     1126 2024-05-20 15:57:30.814370 qnngds-2.5.0/tests/single_dev_on_gds.py
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-20 16:46:48.795296 qnngds-2.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-05-20 16:46:48.795296 qnngds-2.5.1/README.md
+-rw-r--r--   0        0        0     1161 2024-05-20 16:46:51.551344 qnngds-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0      543 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/_default_param.py
+-rw-r--r--   0        0        0    29539 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/cells.py
+-rw-r--r--   0        0        0    10385 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    30497 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/design.py
+-rw-r--r--   0        0        0      158 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/devices/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/devices/htron.py
+-rw-r--r--   0        0        0     1313 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/devices/nanowire.py
+-rw-r--r--   0        0        0     3136 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/devices/ntron.py
+-rw-r--r--   0        0        0     6365 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/devices/resistor.py
+-rw-r--r--   0        0        0     6479 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/devices/snspd.py
+-rw-r--r--   0        0        0     1300 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/geometries.py
+-rw-r--r--   0        0        0     8683 2024-05-20 16:46:48.811296 qnngds-2.5.1/src/qnngds/tests.py
+-rw-r--r--   0        0        0    30179 2024-05-20 16:46:48.815297 qnngds-2.5.1/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3316 2024-05-20 16:46:48.815297 qnngds-2.5.1/tests/all_dev_on_gds.py
+-rw-r--r--   0        0        0     1126 2024-05-20 16:46:48.815297 qnngds-2.5.1/tests/single_dev_on_gds.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.5.1/PKG-INFO
```

### Comparing `qnngds-2.5.0/LICENSE.txt` & `qnngds-2.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/README.md` & `qnngds-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/pyproject.toml` & `qnngds-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "2.5.0"
+version = "2.5.1"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-2.5.0/src/qnngds/__init__.py` & `qnngds-2.5.1/src/qnngds/__init__.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/cells.py` & `qnngds-2.5.1/src/qnngds/cells.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/circuits.py` & `qnngds-2.5.1/src/qnngds/circuits.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/design.py` & `qnngds-2.5.1/src/qnngds/design.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/devices/nanowire.py` & `qnngds-2.5.1/src/qnngds/devices/nanowire.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/devices/ntron.py` & `qnngds-2.5.1/src/qnngds/devices/ntron.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/devices/resistor.py` & `qnngds-2.5.1/src/qnngds/devices/resistor.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/devices/snspd.py` & `qnngds-2.5.1/src/qnngds/devices/snspd.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/geometries.py` & `qnngds-2.5.1/src/qnngds/geometries.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/tests.py` & `qnngds-2.5.1/src/qnngds/tests.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/src/qnngds/utilities.py` & `qnngds-2.5.1/src/qnngds/utilities.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/tests/all_dev_on_gds.py` & `qnngds-2.5.1/tests/all_dev_on_gds.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/tests/single_dev_on_gds.py` & `qnngds-2.5.1/tests/single_dev_on_gds.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.5.0/PKG-INFO` & `qnngds-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 2.5.0
+Version: 2.5.1
 Summary: The QNN library for creating gds files
 Keywords: phidl,nanowire_electronics,nanofabrication,gds
 Author-Email: "A. Jacquillat" <audrey01@mit.edu>, "A. Jacquillat" <audrey.jacquillat@gmail.com>, "R. Foster" <reedf@mit.edu>
 Maintainer-Email: "A. Jacquillat" <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```


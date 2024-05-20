# Comparing `tmp/hyundai_kia_connect_api-3.9.0.tar.gz` & `tmp/hyundai_kia_connect_api-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.9.0.tar", last modified: Mon Sep 18 00:55:36 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.9.1.tar", last modified: Fri Oct  6 23:42:34 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.9.0.tar` & `hyundai_kia_connect_api-3.9.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 00:55:36.768514 hyundai_kia_connect_api-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-09-18 00:55:36.768514 hyundai_kia_connect_api-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 00:55:36.764514 hyundai_kia_connect_api-3.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 00:55:36.768514 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (127)    27427 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (127)    48208 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoApiAU.py
--rw-r--r--   0 runner    (1001) docker     (127)    30103 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (127)    47165 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoApiCN.py
--rw-r--r--   0 runner    (1001) docker     (127)    55198 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 00:55:36.768514 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-09-18 00:55:36.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-09-18 00:55:36.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 00:55:36.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 00:55:36.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-18 00:55:36.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-18 00:55:36.000000 hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-09-18 00:55:36.768514 hyundai_kia_connect_api-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2023-09-18 00:55:19.000000 hyundai_kia_connect_api-3.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 00:55:36.768514 hyundai_kia_connect_api-3.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/tests/au_login_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-09-18 00:54:43.000000 hyundai_kia_connect_api-3.9.0/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 23:42:34.949215 hyundai_kia_connect_api-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2023-10-06 23:42:34.949215 hyundai_kia_connect_api-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 23:42:34.945215 hyundai_kia_connect_api-3.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 23:42:34.945215 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23950 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27427 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48208 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoApiAU.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30103 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47165 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoApiCN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55131 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 23:42:34.949215 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2023-10-06 23:42:34.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-10-06 23:42:34.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 23:42:34.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 23:42:34.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-06 23:42:34.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-06 23:42:34.000000 hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-06 23:42:34.949215 hyundai_kia_connect_api-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2023-10-06 23:42:23.000000 hyundai_kia_connect_api-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 23:42:34.949215 hyundai_kia_connect_api-3.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/tests/au_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2023-10-06 23:41:57.000000 hyundai_kia_connect_api-3.9.1/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.9.0/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/LICENSE` & `hyundai_kia_connect_api-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/PKG-INFO` & `hyundai_kia_connect_api-3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai_kia_connect_api
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,15 +38,15 @@
     brand: int,
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
-    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
+    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA, 5: REGION_AUSTRALIA}
     BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI, 3: BRAND_GENESIS}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
```

### Comparing `hyundai_kia_connect_api-3.9.0/README.rst` & `hyundai_kia_connect_api-3.9.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     brand: int,
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
-    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
+    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA, 5: REGION_AUSTRALIA}
     BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI, 3: BRAND_GENESIS}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
```

### Comparing `hyundai_kia_connect_api-3.9.0/docs/Makefile` & `hyundai_kia_connect_api-3.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/docs/conf.py` & `hyundai_kia_connect_api-3.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/docs/installation.rst` & `hyundai_kia_connect_api-3.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/docs/make.bat` & `hyundai_kia_connect_api-3.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoApiAU.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoApiAU.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoApiCN.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoApiCN.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,19 +311,18 @@
         if value is not None:
             lastTwo = int(value[-2:])
             if lastTwo > 60:
                 value = int(value) + 40
             if int(value) > 1260:
                 value = dt.datetime.strptime(str(value), "%H%M").time()
             else:
-                if timesection == 0:
-                    value = str(value) + " AM"
-                elif timesection == 1:
-                    value = str(value) + " PM"
-                value = dt.datetime.strptime(value, "%I%M %p").time()
+                d = dt.datetime.strptime(value, "%I%M")
+                if timesection > 0:
+                    d += dt.timedelta(hours=12)
+                value = d.time()
         return value
 
     def update_vehicle_with_cached_state(self, token: Token, vehicle: Vehicle) -> None:
         state = self._get_cached_vehicle_state(token, vehicle)
         self._update_vehicle_properties(vehicle, state)
 
         if vehicle.engine_type == ENGINE_TYPES.EV:
```

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/VehicleManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .KiaUvoApiCA import KiaUvoApiCA
 from .KiaUvoApiEU import KiaUvoApiEU
 from .KiaUvoApiCN import KiaUvoApiCN
 from .KiaUvoApiAU import KiaUvoApiAU
 from .Token import Token
 from .Vehicle import Vehicle
 from .const import (
+    BRAND_GENESIS,
     BRAND_HYUNDAI,
     BRAND_KIA,
     BRANDS,
     DOMAIN,
     REGION_AUSTRALIA,
     REGION_CANADA,
     REGION_EUROPE,
@@ -239,15 +240,17 @@
     def get_implementation_by_region_brand(
         region: int, brand: int, language: str
     ) -> ApiImpl:
         if REGIONS[region] == REGION_CANADA:
             return KiaUvoApiCA(region, brand, language)
         elif REGIONS[region] == REGION_EUROPE:
             return KiaUvoApiEU(region, brand, language)
-        elif REGIONS[region] == REGION_USA and BRANDS[brand] == BRAND_HYUNDAI:
+        elif REGIONS[region] == REGION_USA and (
+            BRANDS[brand] == BRAND_HYUNDAI or BRANDS[brand] == BRAND_GENESIS
+        ):
             return HyundaiBlueLinkAPIUSA(region, brand, language)
         elif REGIONS[region] == REGION_USA and BRANDS[brand] == BRAND_KIA:
             return KiaUvoAPIUSA(region, brand, language)
         elif REGIONS[region] == REGION_CHINA:
             return KiaUvoApiCN(region, brand, language)
         elif REGIONS[region] == REGION_AUSTRALIA:
             return KiaUvoApiAU(region, brand, language)
```

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/const.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai-kia-connect-api
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,15 +38,15 @@
     brand: int,
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
-    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
+    REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA, 5: REGION_AUSTRALIA}
     BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI, 3: BRAND_GENESIS}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
```

### Comparing `hyundai_kia_connect_api-3.9.0/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.9.1/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/setup.py` & `hyundai_kia_connect_api-3.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.9.0",
+    version="3.9.1",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.9.0/tests/au_login_test.py` & `hyundai_kia_connect_api-3.9.1/tests/au_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.9.1/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.9.0/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.9.1/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*


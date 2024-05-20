# Comparing `tmp/winterapi-1.3.0.tar.gz` & `tmp/winterapi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winterapi-1.3.0.tar", last modified: Mon Mar  4 23:05:28 2024, max compression
+gzip compressed data, was "winterapi-1.4.0.tar", last modified: Mon May 20 21:29:29 2024, max compression
```

## Comparing `winterapi-1.3.0.tar` & `winterapi-1.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 23:05:28.442733 winterapi-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 23:05:28.438733 winterapi-1.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-04 23:03:40.000000 winterapi-1.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 23:05:28.438733 winterapi-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-04 23:03:40.000000 winterapi-1.3.0/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-04 23:03:40.000000 winterapi-1.3.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-04 23:03:40.000000 winterapi-1.3.0/.github/workflows/continuous_integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-04 23:03:40.000000 winterapi-1.3.0/.github/workflows/isort.yml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-04 23:03:40.000000 winterapi-1.3.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-04 23:03:40.000000 winterapi-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-04 23:03:40.000000 winterapi-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-04 23:03:40.000000 winterapi-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-04 23:05:28.442733 winterapi-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-04 23:03:40.000000 winterapi-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 23:05:28.442733 winterapi-1.3.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-03-04 23:03:40.000000 winterapi-1.3.0/notebooks/Example_1_Setting_Up_Credentials.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-03-04 23:03:40.000000 winterapi-1.3.0/notebooks/Example_2_Submitting_a_ToO.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-03-04 23:03:40.000000 winterapi-1.3.0/notebooks/Example_3_Interacting_with_Observatory_Queue.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   102674 2024-03-04 23:03:40.000000 winterapi-1.3.0/notebooks/Example_4_Finding_Observatory_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-03-04 23:03:40.000000 winterapi-1.3.0/notebooks/Example_5_Downloading_Observatory_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-03-04 23:03:40.000000 winterapi-1.3.0/notebooks/Info_1_Introduction_To_Credentials.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-03-04 23:03:40.000000 winterapi-1.3.0/notebooks/Info_2a_ToO_Parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19222 2024-03-04 23:03:40.000000 winterapi-1.3.0/notebooks/Info_2b_Submitting_ToOs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-04 23:03:40.000000 winterapi-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 23:05:28.442733 winterapi-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 23:05:28.442733 winterapi-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-04 23:03:40.000000 winterapi-1.3.0/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-04 23:03:40.000000 winterapi-1.3.0/tests/test_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 23:05:28.442733 winterapi-1.3.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-04 23:03:40.000000 winterapi-1.3.0/tests/testdata/test_schedule.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 23:05:28.442733 winterapi-1.3.0/winterapi/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-04 23:03:40.000000 winterapi-1.3.0/winterapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-03-04 23:03:40.000000 winterapi-1.3.0/winterapi/base_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-04 23:03:40.000000 winterapi-1.3.0/winterapi/configure_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-03-04 23:03:40.000000 winterapi-1.3.0/winterapi/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-04 23:03:40.000000 winterapi-1.3.0/winterapi/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-03-04 23:03:40.000000 winterapi-1.3.0/winterapi/fidelius.py
--rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-03-04 23:03:40.000000 winterapi-1.3.0/winterapi/messenger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 23:05:28.442733 winterapi-1.3.0/winterapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-04 23:05:28.000000 winterapi-1.3.0/winterapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-04 23:05:28.000000 winterapi-1.3.0/winterapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 23:05:28.000000 winterapi-1.3.0/winterapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-04 23:05:28.000000 winterapi-1.3.0/winterapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-04 23:05:28.000000 winterapi-1.3.0/winterapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.367559 winterapi-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/automerge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/continuous_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/isort.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-20 21:27:34.000000 winterapi-1.4.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-20 21:27:34.000000 winterapi-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-20 21:27:34.000000 winterapi-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 21:27:34.000000 winterapi-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 21:29:29.367559 winterapi-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-20 21:27:34.000000 winterapi-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_1_Setting_Up_Credentials.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_2_Submitting_a_ToO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_3_Interacting_with_Observatory_Queue.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   102674 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_4_Finding_Observatory_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Example_5_Downloading_Observatory_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Info_1_Introduction_To_Credentials.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Info_2a_ToO_Parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19222 2024-05-20 21:27:34.000000 winterapi-1.4.0/notebooks/Info_2b_Submitting_ToOs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-20 21:27:34.000000 winterapi-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:29:29.367559 winterapi-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-20 21:27:34.000000 winterapi-1.4.0/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-20 21:27:34.000000 winterapi-1.4.0/tests/test_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.363559 winterapi-1.4.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-20 21:27:34.000000 winterapi-1.4.0/tests/testdata/test_schedule.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.367559 winterapi-1.4.0/winterapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/configure_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/fidelius.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-05-20 21:27:34.000000 winterapi-1.4.0/winterapi/messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:29:29.367559 winterapi-1.4.0/winterapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 21:29:29.000000 winterapi-1.4.0/winterapi.egg-info/top_level.txt
```

### Comparing `winterapi-1.3.0/.github/workflows/automerge.yml` & `winterapi-1.4.0/.github/workflows/automerge.yml`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/.github/workflows/black.yml` & `winterapi-1.4.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/.github/workflows/continuous_integration.yml` & `winterapi-1.4.0/.github/workflows/continuous_integration.yml`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/.github/workflows/pylint.yml` & `winterapi-1.4.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/.gitignore` & `winterapi-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/.pre-commit-config.yaml` & `winterapi-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/LICENSE` & `winterapi-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/PKG-INFO` & `winterapi-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winterapi
-Version: 1.3.0
+Version: 1.4.0
 Author-email: Robert Stein <rdstein@caltech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/winter-telescope/winterapi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
@@ -24,19 +24,19 @@
 Requires-Dist: packaging
 Requires-Dist: keyring
 Requires-Dist: cryptography
 Requires-Dist: pre-commit
 Requires-Dist: jupyter
 Requires-Dist: backoff
 Requires-Dist: pydantic
-Requires-Dist: wintertoo>=1.5.0
+Requires-Dist: wintertoo>=1.6.1
 Provides-Extra: dev
-Requires-Dist: black==24.2.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: pylint==3.1.0; extra == "dev"
+Requires-Dist: pylint==3.2.2; extra == "dev"
 Requires-Dist: coveralls; extra == "dev"
 
 # winterapi
 API interactions for WINTER
 
 [![Coverage Status](https://coveralls.io/repos/github/winter-telescope/winterapi/badge.svg?branch=tests)](https://coveralls.io/github/winter-telescope/winterapi?branch=tests)
 [![CI](https://github.com/winter-telescope/winterapi/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/winter-telescope/winterapi/actions/workflows/continuous_integration.yml)
```

### Comparing `winterapi-1.3.0/README.md` & `winterapi-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/notebooks/Example_1_Setting_Up_Credentials.ipynb` & `winterapi-1.4.0/notebooks/Example_1_Setting_Up_Credentials.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/notebooks/Example_2_Submitting_a_ToO.ipynb` & `winterapi-1.4.0/notebooks/Example_2_Submitting_a_ToO.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/notebooks/Example_3_Interacting_with_Observatory_Queue.ipynb` & `winterapi-1.4.0/notebooks/Example_3_Interacting_with_Observatory_Queue.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/notebooks/Example_4_Finding_Observatory_Data.ipynb` & `winterapi-1.4.0/notebooks/Example_4_Finding_Observatory_Data.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/notebooks/Example_5_Downloading_Observatory_Data.ipynb` & `winterapi-1.4.0/notebooks/Example_5_Downloading_Observatory_Data.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/notebooks/Info_1_Introduction_To_Credentials.ipynb` & `winterapi-1.4.0/notebooks/Info_1_Introduction_To_Credentials.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/notebooks/Info_2a_ToO_Parameters.ipynb` & `winterapi-1.4.0/notebooks/Info_2a_ToO_Parameters.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/notebooks/Info_2b_Submitting_ToOs.ipynb` & `winterapi-1.4.0/notebooks/Info_2b_Submitting_ToOs.ipynb`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/pyproject.toml` & `winterapi-1.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "winterapi"
-version = "1.3.0"
+version = "1.4.0"
 description = ""
 authors = [
     {name = "Robert Stein", email = "rdstein@caltech.edu"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
@@ -32,21 +32,21 @@
     "packaging",
     "keyring",
     "cryptography",
     "pre-commit",
     "jupyter",
     "backoff",
     "pydantic",
-    "wintertoo>=1.5.0"
+    "wintertoo>=1.6.1"
 ]
 [project.optional-dependencies]
 dev = [
-    "black == 24.2.0",
+    "black == 24.4.2",
     "isort == 5.13.2",
-    "pylint == 3.1.0",
+    "pylint == 3.2.2",
     "coveralls",
 ]
 
 [project.urls]
 Homepage = "https://github.com/winter-telescope/winterapi"
 
 [tool.setuptools]
@@ -85,7 +85,10 @@
 
 [tool.pylint.format]
 max-line-length = "88"
 disable=["logging-fstring-interpolation"]
 good-names=["ax", "ra", "df", "pi", "i"]
 exclude-too-few-public-methods=["pydantic.*"]
 extension-pkg-whitelist=["pydantic"]
+
+[tool.pylint.typecheck]
+generated-members=["u.*"]
```

### Comparing `winterapi-1.3.0/tests/test_schedule.py` & `winterapi-1.4.0/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/tests/testdata/test_schedule.csv` & `winterapi-1.4.0/tests/testdata/test_schedule.csv`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 targName,raDeg,decDeg,fieldID,filter,visitExpTime,singleExpTime,priority,progPI,progName,progID,validStart,validStop,observed,maxAirmass,ditherNumber,ditherStepSize,bestDetector,obsHistID
-test_field,211.56398,54.0,3944,Y,300.0,33.333333333333336,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,9,30.0,True,0
-test_field,211.56398,54.0,3944,J,300.0,33.333333333333336,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,9,30.0,True,1
-test_field,211.56398,54.0,3944,Hs,300.0,33.333333333333336,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,9,30.0,True,2
-test_radec,210.910674637,54.3116510708,999999999,Y,300.0,37.5,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,8,30.0,True,3
-test_radec,210.910674637,54.3116510708,999999999,J,300.0,37.5,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,8,30.0,True,4
-test_radec,210.910674637,54.3116510708,999999999,Hs,300.0,37.5,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,8,30.0,True,5
+test_field,211.56398,54.0,3944,Y,300.0,33.333333333333336,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,9,90.0,True,0
+test_field,211.56398,54.0,3944,J,300.0,33.333333333333336,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,9,90.0,True,1
+test_field,211.56398,54.0,3944,Hs,300.0,33.333333333333336,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,9,90.0,True,2
+test_radec,210.910674637,54.3116510708,999999999,Y,300.0,37.5,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,8,90.0,True,3
+test_radec,210.910674637,54.3116510708,999999999,J,300.0,37.5,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,8,90.0,True,4
+test_radec,210.910674637,54.3116510708,999999999,Hs,300.0,37.5,50.0,Stein,2023A999,0,62721.1894969287,62722.1894969452,False,2.0,8,90.0,True,5
```

### Comparing `winterapi-1.3.0/winterapi/base_api.py` & `winterapi-1.4.0/winterapi/base_api.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/winterapi/configure_tests.py` & `winterapi-1.4.0/winterapi/configure_tests.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/winterapi/credentials.py` & `winterapi-1.4.0/winterapi/credentials.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/winterapi/endpoints.py` & `winterapi-1.4.0/winterapi/endpoints.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/winterapi/fidelius.py` & `winterapi-1.4.0/winterapi/fidelius.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/winterapi/messenger.py` & `winterapi-1.4.0/winterapi/messenger.py`

 * *Files identical despite different names*

### Comparing `winterapi-1.3.0/winterapi.egg-info/PKG-INFO` & `winterapi-1.4.0/winterapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winterapi
-Version: 1.3.0
+Version: 1.4.0
 Author-email: Robert Stein <rdstein@caltech.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/winter-telescope/winterapi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
@@ -24,19 +24,19 @@
 Requires-Dist: packaging
 Requires-Dist: keyring
 Requires-Dist: cryptography
 Requires-Dist: pre-commit
 Requires-Dist: jupyter
 Requires-Dist: backoff
 Requires-Dist: pydantic
-Requires-Dist: wintertoo>=1.5.0
+Requires-Dist: wintertoo>=1.6.1
 Provides-Extra: dev
-Requires-Dist: black==24.2.0; extra == "dev"
+Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
-Requires-Dist: pylint==3.1.0; extra == "dev"
+Requires-Dist: pylint==3.2.2; extra == "dev"
 Requires-Dist: coveralls; extra == "dev"
 
 # winterapi
 API interactions for WINTER
 
 [![Coverage Status](https://coveralls.io/repos/github/winter-telescope/winterapi/badge.svg?branch=tests)](https://coveralls.io/github/winter-telescope/winterapi?branch=tests)
 [![CI](https://github.com/winter-telescope/winterapi/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/winter-telescope/winterapi/actions/workflows/continuous_integration.yml)
```

### Comparing `winterapi-1.3.0/winterapi.egg-info/SOURCES.txt` & `winterapi-1.4.0/winterapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/pytest-nhsd-apim-3.3.8.tar.gz` & `tmp/pytest-nhsd-apim-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-nhsd-apim-3.3.8.tar", last modified: Fri Sep  8 14:00:01 2023, max compression
+gzip compressed data, was "pytest-nhsd-apim-3.3.9.tar", last modified: Mon Sep 18 10:52:54 2023, max compression
```

## Comparing `pytest-nhsd-apim-3.3.8.tar` & `pytest-nhsd-apim-3.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:00:01.725516 pytest-nhsd-apim-3.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2023-09-08 14:00:01.725516 pytest-nhsd-apim-3.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-08 14:00:01.725516 pytest-nhsd-apim-3.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:00:01.721516 pytest-nhsd-apim-3.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:00:01.721516 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57430 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/apigee_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/apigee_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/auth_journey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19766 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/identity_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/nhsd_apim_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/pytest_nhsd_apim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/token_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:00:01.725516 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2023-09-08 14:00:01.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-09-08 14:00:01.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 14:00:01.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-08 14:00:01.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-09-08 14:00:01.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-08 14:00:01.000000 pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:00:01.725516 pytest-nhsd-apim-3.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/tests/test_apigee_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15648 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-09-08 13:59:21.000000 pytest-nhsd-apim-3.3.8/tests/test_nhsd_apim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:52:54.801469 pytest-nhsd-apim-3.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2023-09-18 10:52:54.801469 pytest-nhsd-apim-3.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-18 10:52:54.801469 pytest-nhsd-apim-3.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:52:54.797469 pytest-nhsd-apim-3.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:52:54.801469 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57430 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/apigee_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/apigee_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/auth_journey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/identity_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/nhsd_apim_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/pytest_nhsd_apim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/token_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:52:54.801469 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2023-09-18 10:52:54.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2023-09-18 10:52:54.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 10:52:54.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-18 10:52:54.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-09-18 10:52:54.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-18 10:52:54.000000 pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:52:54.801469 pytest-nhsd-apim-3.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/tests/test_apigee_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15648 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2023-09-18 10:52:01.000000 pytest-nhsd-apim-3.3.9/tests/test_nhsd_apim.py
```

### Comparing `pytest-nhsd-apim-3.3.8/PKG-INFO` & `pytest-nhsd-apim-3.3.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pytest-nhsd-apim
-Version: 3.3.8
-Summary: Pytest plugin accessing NHSDigital's APIM proxies
-Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
-Author: Adrian Ciobanita
-Author-email: adrian.ciobanita1@nhs.net
-Maintainer: Alex Carrie
-Maintainer-email: alexander.carrie1@nhs.net
-License: MIT
-Classifier: Framework :: Pytest
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # pytest-nhsd-apim
 
 A pytest extension for NHSDigital's API Mangement suite.
 
 ## Installation
 In your project's virtual environment
 ```code()
```

### Comparing `pytest-nhsd-apim-3.3.8/README.md` & `pytest-nhsd-apim-3.3.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: pytest-nhsd-apim
+Version: 3.3.9
+Summary: Pytest plugin accessing NHSDigital's APIM proxies
+Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
+Author: Adrian Ciobanita
+Author-email: adrian.ciobanita1@nhs.net
+Maintainer: Alex Carrie
+Maintainer-email: alexander.carrie1@nhs.net
+License: MIT
+Classifier: Framework :: Pytest
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: Authlib==0.15.5
+Requires-Dist: cryptography<42.0.0,===36.0.1
+Requires-Dist: lxml==4.9.1
+Requires-Dist: pycryptodome==3.13.0
+Requires-Dist: PyJWT==2.8.0
+Requires-Dist: pyotp==2.6.0
+Requires-Dist: pytest==6.2.5
+Requires-Dist: requests==2.31.0
+Requires-Dist: toml==0.10.2
+Requires-Dist: typing-extensions==4.3.0
+Requires-Dist: pydantic==1.9.1
+Requires-Dist: wheel<0.39.0,===0.37.1
+
 # pytest-nhsd-apim
 
 A pytest extension for NHSDigital's API Mangement suite.
 
 ## Installation
 In your project's virtual environment
 ```code()
```

### Comparing `pytest-nhsd-apim-3.3.8/pyproject.toml` & `pytest-nhsd-apim-3.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "pytest-nhsd-apim"
-version = "3.3.8"
+version = "3.3.9"
 description = "Pytest plugin accessing NHSDigital's APIM proxies"
 authors = ["Adrian Ciobanita <adrian.ciobanita1@nhs.net>", "Alex Carrie <alexander.carrie1@nhs.net>", "Lucas Fantini <lucas.fantini@nhs.net>"]
 maintainers = ["Alex Carrie <alexander.carrie1@nhs.net>", "Alex Hawdon <alex.hawdon1@nhs.net"]
 readme = "README.md"
 repository = "https://github.com/NHSDigital/pytest-nhsd-apim"
 classifiers = ["Framework :: Pytest"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 Authlib = "^0.15.5"
 cryptography = ">=36.0.1,<42.0.0"
 lxml = "^4.9.1"
 python = "^3.8"
 pycryptodome = "^3.13.0"
-PyJWT = "^2.3.0"
+PyJWT = "^2.8.0"
 pyotp = "^2.6.0"
 pytest = "^6.2.5"
-requests = "^2.27.1"
+requests = "^2.31.0"
 toml = "^0.10.2"
 typing-extensions = "^4.3.0"
 pydantic = "^1.9.1"
 wheel = ">=0.37.1,<0.39.0"
 
 
 [tool.poetry.dev-dependencies]
```

### Comparing `pytest-nhsd-apim-3.3.8/setup.py` & `pytest-nhsd-apim-3.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/apigee_apis.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/apigee_apis.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/apigee_edge.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/apigee_edge.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/auth_journey.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/auth_journey.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/config.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/config.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/identity_service.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/identity_service.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/log.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/log.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/nhsd_apim_authorization.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/nhsd_apim_authorization.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/pytest_nhsd_apim.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/pytest_nhsd_apim.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/secrets.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/secrets.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim/token_cache.py` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim/token_cache.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/PKG-INFO` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 Metadata-Version: 2.1
 Name: pytest-nhsd-apim
-Version: 3.3.8
+Version: 3.3.9
 Summary: Pytest plugin accessing NHSDigital's APIM proxies
 Home-page: https://github.com/NHSDigital/pytest-nhsd-apim
 Author: Adrian Ciobanita
 Author-email: adrian.ciobanita1@nhs.net
 Maintainer: Alex Carrie
 Maintainer-email: alexander.carrie1@nhs.net
 License: MIT
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: Authlib==0.15.5
+Requires-Dist: cryptography<42.0.0,===36.0.1
+Requires-Dist: lxml==4.9.1
+Requires-Dist: pycryptodome==3.13.0
+Requires-Dist: PyJWT==2.8.0
+Requires-Dist: pyotp==2.6.0
+Requires-Dist: pytest==6.2.5
+Requires-Dist: requests==2.31.0
+Requires-Dist: toml==0.10.2
+Requires-Dist: typing-extensions==4.3.0
+Requires-Dist: pydantic==1.9.1
+Requires-Dist: wheel<0.39.0,===0.37.1
 
 # pytest-nhsd-apim
 
 A pytest extension for NHSDigital's API Mangement suite.
 
 ## Installation
 In your project's virtual environment
```

### Comparing `pytest-nhsd-apim-3.3.8/src/pytest_nhsd_apim.egg-info/SOURCES.txt` & `pytest-nhsd-apim-3.3.9/src/pytest_nhsd_apim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/tests/test_apigee_apis.py` & `pytest-nhsd-apim-3.3.9/tests/test_apigee_apis.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/tests/test_examples.py` & `pytest-nhsd-apim-3.3.9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pytest-nhsd-apim-3.3.8/tests/test_nhsd_apim.py` & `pytest-nhsd-apim-3.3.9/tests/test_nhsd_apim.py`

 * *Files identical despite different names*


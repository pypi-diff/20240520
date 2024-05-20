# Comparing `tmp/audiconnectpy-2.2.0.tar.gz` & `tmp/audiconnectpy-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.2.0.tar", last modified: Sun May 19 17:02:41 2024, max compression
+gzip compressed data, was "audiconnectpy-2.2.1.tar", last modified: Sun May 19 17:06:29 2024, max compression
```

## Comparing `audiconnectpy-2.2.0.tar` & `audiconnectpy-2.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:02:41.548861 audiconnectpy-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:02:41.544861 audiconnectpy-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:02:41.544861 audiconnectpy-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:02:41.544861 audiconnectpy-2.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 17:02:41.548861 audiconnectpy-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:02:41.548861 audiconnectpy-2.2.0/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26067 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:02:41.548861 audiconnectpy-2.2.0/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 17:02:41.000000 audiconnectpy-2.2.0/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 17:02:41.000000 audiconnectpy-2.2.0/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:02:41.000000 audiconnectpy-2.2.0/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:02:41.000000 audiconnectpy-2.2.0/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 17:02:41.000000 audiconnectpy-2.2.0/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 17:02:41.000000 audiconnectpy-2.2.0/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:02:41.548861 audiconnectpy-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:02:41.548861 audiconnectpy-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:02:41.548861 audiconnectpy-2.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-19 17:02:31.000000 audiconnectpy-2.2.0/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.870228 audiconnectpy-2.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.870228 audiconnectpy-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.870228 audiconnectpy-2.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.870228 audiconnectpy-2.2.1/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26065 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/test_home.py
```

### Comparing `audiconnectpy-2.2.0/.github/dependabot.yml` & `audiconnectpy-2.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/.github/workflows/auto-approve.yml` & `audiconnectpy-2.2.1/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.2.1/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.2.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/.github/workflows/release.yml` & `audiconnectpy-2.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/.gitignore` & `audiconnectpy-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/.pre-commit-config.yaml` & `audiconnectpy-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/LICENSE` & `audiconnectpy-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/PKG-INFO` & `audiconnectpy-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.0
+Version: 2.2.1
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.0/README.md` & `audiconnectpy-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/audiconnectpy/api.py` & `audiconnectpy-2.2.1/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/audiconnectpy/auth.py` & `audiconnectpy-2.2.1/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/audiconnectpy/const.py` & `audiconnectpy-2.2.1/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/audiconnectpy/helpers.py` & `audiconnectpy-2.2.1/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/audiconnectpy/model.py` & `audiconnectpy-2.2.1/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/audiconnectpy/vehicle.py` & `audiconnectpy-2.2.1/audiconnectpy/vehicle.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     SUCCEEDED,
     SUCCESSFUL,
 )
 from .exceptions import HttpRequestError, TimeoutExceededError
 from .helpers import ExtendedDict, remove_value, spin_hash
 from .model import Information, Location, Model, Position
 
-_LOGGER = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 class Globals:
     """Global variables."""
 
     def __init__(self, unit: str) -> None:
         """Initilaze."""
@@ -634,15 +634,15 @@
 
         if stauts_good is False:
             raise TimeoutExceededError(("Cannot %s, operation timed out", action))
 
     async def _async_get_security_token(self, action: str) -> str:
         """Get security token."""
         if self.spin is None:
-            logging.error("Security PIN not found")
+            logger.error("Security PIN not found")
             return ""
 
         # Challenge
         headers = await self.auth.async_get_headers(token_type="mbb", okhttp=True)
         rsp = await self.auth.request(
             "GET",
             f"{self.uris['url_setter']}/rolesrights/authorization/v2/vehicles/{self.vin}/services/{action}/security-pin-auth-requested",
```

### Comparing `audiconnectpy-2.2.0/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.2.1/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.0
+Version: 2.2.1
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.0/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.2.1/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/example.py` & `audiconnectpy-2.2.1/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/pyproject.toml` & `audiconnectpy-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/tests/conftest.py` & `audiconnectpy-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/tests/fixtures/audi0.json` & `audiconnectpy-2.2.1/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/tests/fixtures/audi1.json` & `audiconnectpy-2.2.1/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/tests/fixtures/audi2.json` & `audiconnectpy-2.2.1/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.2.1/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/tests/fixtures/location.json` & `audiconnectpy-2.2.1/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.0/tests/test_home.py` & `audiconnectpy-2.2.1/tests/test_home.py`

 * *Files identical despite different names*


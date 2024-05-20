# Comparing `tmp/audiconnectpy-2.2.2.tar.gz` & `tmp/audiconnectpy-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.2.2.tar", last modified: Mon May 20 11:47:49 2024, max compression
+gzip compressed data, was "audiconnectpy-2.2.3.tar", last modified: Mon May 20 12:45:58 2024, max compression
```

## Comparing `audiconnectpy-2.2.2.tar` & `audiconnectpy-2.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.521695 audiconnectpy-2.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.521695 audiconnectpy-2.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.521695 audiconnectpy-2.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.521695 audiconnectpy-2.2.2/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23057 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.837413 audiconnectpy-2.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.837413 audiconnectpy-2.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.837413 audiconnectpy-2.2.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.837413 audiconnectpy-2.2.3/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23323 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/test_home.py
```

### Comparing `audiconnectpy-2.2.2/.github/dependabot.yml` & `audiconnectpy-2.2.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/.github/workflows/auto-approve.yml` & `audiconnectpy-2.2.3/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.2.3/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.2.3/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/.github/workflows/release.yml` & `audiconnectpy-2.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/.gitignore` & `audiconnectpy-2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/.pre-commit-config.yaml` & `audiconnectpy-2.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/LICENSE` & `audiconnectpy-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/PKG-INFO` & `audiconnectpy-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.2
+Version: 2.2.3
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.2/README.md` & `audiconnectpy-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/audiconnectpy/api.py` & `audiconnectpy-2.2.3/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/audiconnectpy/auth.py` & `audiconnectpy-2.2.3/audiconnectpy/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         # IDK token
         self._idk_token = await self._async_get_idk_token(
             code=authcode_strings["code"][0], code_verifier=code_verifier
         )
 
         # Audi token
         self._audi_token = await self._async_get_azs_token(
-            id_token=self._idk_token["access_token"]
+            id_token=self._idk_token["id_token"]
         )
 
         # mbboauth client register
         self._x_client_id = await self._async_register_idk()
 
         # MBB token
         self._mbb_token = await self._async_get_mbb_token(
@@ -292,18 +292,20 @@
             seconds=self._mbb_token["expires_in"]
         )
 
         # Here token
         self._here_token = await self._async_get_here_token(
             id_token=self._idk_token["id_token"]
         )
+        if "refresh_token" in self._here_token:
+            self._mbb_token["refresh_token"] = self._here_token["refresh_token"]
 
     async def async_refresh_tokens(self) -> None:
         """Refresh token if."""
-        if self._mbb_token_expired and datetime.now() > self._mbb_token_expired:
+        if self._mbb_token_expired and datetime.now() < self._mbb_token_expired:
             try:
                 _LOGGER.debug("Refresh MBB token")
                 refresh_token = self._mbb_token["refresh_token"]
                 self._mbb_token = await self._async_get_mbb_token(
                     refresh_token=refresh_token
                 )
                 # TR/2022-02-10: If a new refresh_token is provided, save it for further refreshes
@@ -318,21 +320,23 @@
                 _LOGGER.debug("Refresh IDK token")
                 self._idk_token = await self._async_get_idk_token(
                     refresh_token=self._idk_token["refresh_token"]
                 )
 
                 _LOGGER.debug("Refresh Audi token")
                 self._audi_token = await self._async_get_azs_token(
-                    id_token=self._idk_token["access_token"]
+                    id_token=self._idk_token["id_token"]
                 )
 
                 _LOGGER.debug("Refresh Here token")
                 self._here_token = await self._async_get_here_token(
                     id_token=self._idk_token["id_token"]
                 )
+                if "refresh_token" in self._here_token:
+                    self._mbb_token["refresh_token"] = self._here_token["refresh_token"]
 
             except AudiException as error:
                 _LOGGER.error("Refresh token failed: %s", error)
                 self.binded = False
 
     async def async_get_action_headers(
         self, content_type: str, security_token: str | None, x_security: bool = False
```

### Comparing `audiconnectpy-2.2.2/audiconnectpy/const.py` & `audiconnectpy-2.2.3/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/audiconnectpy/helpers.py` & `audiconnectpy-2.2.3/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/audiconnectpy/model.py` & `audiconnectpy-2.2.3/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/audiconnectpy/vehicle.py` & `audiconnectpy-2.2.3/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.2.3/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.2
+Version: 2.2.3
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.2/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.2.3/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/example.py` & `audiconnectpy-2.2.3/example.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 import logging
 
 from aiohttp import ClientSession
 import yaml
 
 from audiconnectpy import AudiConnect, AudiException
 
-logger = logging.getLogger(__name__)
-logger.setLevel("DEBUG")
-# logger.setLevel("INFO")
 # create console handler and set level to debug
+logger = logging.getLogger()
+logger.setLevel("DEBUG")
 ch = logging.StreamHandler()
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 
 
 # Fill out the secrets in secrets.yaml, you can find an example
 # _secrets.yaml file, which has to be renamed after filling out the secrets.
-
 with open("./secrets.yaml", encoding="UTF-8") as file:
     secrets = yaml.safe_load(file)
 
 USERNAME = secrets["USERNAME"]
 PASSWORD = secrets["PASSWORD"]
 COUNTRY = "FR"
 SPIN = secrets["SPIN"]
 
 
 async def main() -> None:
     """Run Main method."""
     async with ClientSession() as session:
         api = AudiConnect(session, USERNAME, PASSWORD, COUNTRY, SPIN)
-
         try:
             await api.async_login()
-            if api.is_connected:
+        except AudiException as error:
+            logger.error(error)
+        while api.is_connected:
+            try:
                 for vehicle in api.vehicles:
                     logger.info(vehicle.vin)
                     logger.info(vehicle.infos)
                     logger.info(vehicle.fuel_status)
                     logger.info(vehicle.last_access)
                     logger.info(vehicle.position)
                     # logger.info(vehicle.location)
@@ -53,17 +53,20 @@
                     logger.info(vehicle.vehicle_lights)
                     logger.info(vehicle.vehicle_health_inspection)
                     logger.info(vehicle.measurements)
                     logger.info(vehicle.vehicle_health_warnings)
                     logger.info(vehicle.infos)
                     # await vehicle.async_set_lock(True)
                     # await vehicle.async_refresh_vehicle_data()
-                    # await vehicle.async_update()
-                    logger.info(vehicle.last_access)
-        except AudiException as error:
-            logger.error(error)
+                    await vehicle.async_update()
+            except AudiException as error:
+                logger.error(error)
+            finally:
+                await asyncio.sleep(600)
+
+            await api.async_close()
 
 
 if __name__ == "__main__":
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     asyncio.run(main())
```

### Comparing `audiconnectpy-2.2.2/pyproject.toml` & `audiconnectpy-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/tests/conftest.py` & `audiconnectpy-2.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/tests/fixtures/audi0.json` & `audiconnectpy-2.2.3/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/tests/fixtures/audi1.json` & `audiconnectpy-2.2.3/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/tests/fixtures/audi2.json` & `audiconnectpy-2.2.3/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.2.3/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/tests/fixtures/location.json` & `audiconnectpy-2.2.3/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.2/tests/test_home.py` & `audiconnectpy-2.2.3/tests/test_home.py`

 * *Files identical despite different names*


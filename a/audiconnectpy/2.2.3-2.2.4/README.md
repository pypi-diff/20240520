# Comparing `tmp/audiconnectpy-2.2.3.tar.gz` & `tmp/audiconnectpy-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.2.3.tar", last modified: Mon May 20 12:45:58 2024, max compression
+gzip compressed data, was "audiconnectpy-2.2.4.tar", last modified: Mon May 20 12:50:04 2024, max compression
```

## Comparing `audiconnectpy-2.2.3.tar` & `audiconnectpy-2.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.837413 audiconnectpy-2.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.837413 audiconnectpy-2.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.837413 audiconnectpy-2.2.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.837413 audiconnectpy-2.2.3/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23323 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 12:45:58.000000 audiconnectpy-2.2.3/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:58.841413 audiconnectpy-2.2.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-20 12:45:48.000000 audiconnectpy-2.2.3/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.990760 audiconnectpy-2.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.990760 audiconnectpy-2.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.990760 audiconnectpy-2.2.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.990760 audiconnectpy-2.2.4/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23323 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 12:50:04.000000 audiconnectpy-2.2.4/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:50:04.994760 audiconnectpy-2.2.4/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-20 12:49:50.000000 audiconnectpy-2.2.4/tests/test_home.py
```

### Comparing `audiconnectpy-2.2.3/.github/dependabot.yml` & `audiconnectpy-2.2.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/.github/workflows/auto-approve.yml` & `audiconnectpy-2.2.4/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.2.4/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.2.4/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/.github/workflows/release.yml` & `audiconnectpy-2.2.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/.gitignore` & `audiconnectpy-2.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/.pre-commit-config.yaml` & `audiconnectpy-2.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/LICENSE` & `audiconnectpy-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/PKG-INFO` & `audiconnectpy-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.3
+Version: 2.2.4
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.3/README.md` & `audiconnectpy-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/audiconnectpy/api.py` & `audiconnectpy-2.2.4/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/audiconnectpy/auth.py` & `audiconnectpy-2.2.4/audiconnectpy/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
             id_token=self._idk_token["id_token"]
         )
         if "refresh_token" in self._here_token:
             self._mbb_token["refresh_token"] = self._here_token["refresh_token"]
 
     async def async_refresh_tokens(self) -> None:
         """Refresh token if."""
-        if self._mbb_token_expired and datetime.now() < self._mbb_token_expired:
+        if self._mbb_token_expired and datetime.now() > self._mbb_token_expired:
             try:
                 _LOGGER.debug("Refresh MBB token")
                 refresh_token = self._mbb_token["refresh_token"]
                 self._mbb_token = await self._async_get_mbb_token(
                     refresh_token=refresh_token
                 )
                 # TR/2022-02-10: If a new refresh_token is provided, save it for further refreshes
```

### Comparing `audiconnectpy-2.2.3/audiconnectpy/const.py` & `audiconnectpy-2.2.4/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/audiconnectpy/helpers.py` & `audiconnectpy-2.2.4/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/audiconnectpy/model.py` & `audiconnectpy-2.2.4/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/audiconnectpy/vehicle.py` & `audiconnectpy-2.2.4/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.2.4/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.3
+Version: 2.2.4
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.3/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.2.4/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/example.py` & `audiconnectpy-2.2.4/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/pyproject.toml` & `audiconnectpy-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/tests/conftest.py` & `audiconnectpy-2.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/tests/fixtures/audi0.json` & `audiconnectpy-2.2.4/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/tests/fixtures/audi1.json` & `audiconnectpy-2.2.4/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/tests/fixtures/audi2.json` & `audiconnectpy-2.2.4/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.2.4/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/tests/fixtures/location.json` & `audiconnectpy-2.2.4/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.3/tests/test_home.py` & `audiconnectpy-2.2.4/tests/test_home.py`

 * *Files identical despite different names*


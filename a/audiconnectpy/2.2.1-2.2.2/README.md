# Comparing `tmp/audiconnectpy-2.2.1.tar.gz` & `tmp/audiconnectpy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.2.1.tar", last modified: Sun May 19 17:06:29 2024, max compression
+gzip compressed data, was "audiconnectpy-2.2.2.tar", last modified: Mon May 20 11:47:49 2024, max compression
```

## Comparing `audiconnectpy-2.2.1.tar` & `audiconnectpy-2.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.870228 audiconnectpy-2.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.870228 audiconnectpy-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.870228 audiconnectpy-2.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.870228 audiconnectpy-2.2.1/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26065 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 17:06:29.000000 audiconnectpy-2.2.1/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:06:29.874228 audiconnectpy-2.2.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-19 17:06:18.000000 audiconnectpy-2.2.1/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.521695 audiconnectpy-2.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.521695 audiconnectpy-2.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.521695 audiconnectpy-2.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.521695 audiconnectpy-2.2.2/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23057 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 11:47:49.000000 audiconnectpy-2.2.2/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:47:49.525695 audiconnectpy-2.2.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-20 11:47:35.000000 audiconnectpy-2.2.2/tests/test_home.py
```

### Comparing `audiconnectpy-2.2.1/.github/dependabot.yml` & `audiconnectpy-2.2.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/.github/workflows/auto-approve.yml` & `audiconnectpy-2.2.2/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.2.2/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.2.2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/.github/workflows/release.yml` & `audiconnectpy-2.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/.gitignore` & `audiconnectpy-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/.pre-commit-config.yaml` & `audiconnectpy-2.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/LICENSE` & `audiconnectpy-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/PKG-INFO` & `audiconnectpy-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.1
+Version: 2.2.2
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.1/README.md` & `audiconnectpy-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/audiconnectpy/auth.py` & `audiconnectpy-2.2.2/audiconnectpy/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,33 @@
 from urllib.parse import parse_qs, urlencode, urlparse
 import uuid
 
 import aiohttp
 import async_timeout
 from bs4 import BeautifulSoup
 
+from .const import (
+    CLIENT_ID,
+    DELAY,
+    HDR_USER_AGENT,
+    HDR_XAPP_VERSION,
+    MARKET_URL,
+    MBB_URL,
+    TIMEOUT,
+    URL_HERE_COM,
+    URL_INFO_USER,
+)
 from .exceptions import (
     AudiException,
     AuthorizationError,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
 )
-
-TIMEOUT = 120
-DELAY = 10
-HDR_XAPP_VERSION = "4.24.2"
-HDR_USER_AGENT = "Android/4.24.2 (Build 800240338.root project 'onetouch-android'.ext.buildTime) Android/11"
-MARKET_URL = "https://content.app.my.audi.com/service/mobileapp/configurations"
-CLIENT_ID = "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com"
-MBB_URL = "https://mbboauth-1d.prd.ece.vwg-connect.com/mbbcoauth"
+from .helpers import ExtendedDict
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Auth:
     """Authentication."""
 
@@ -54,14 +58,16 @@
         self.user_id = ""
         self._mbb_token: dict[str, Any] = {}
         self._here_token: dict[str, Any] = {}
         self._mbb_token_expired: datetime | None = None
         self._idk_token: dict[str, str] = {}
         self._audi_token: dict[str, str] = {}
         self.uris: dict[str, str] = {}
+        self.binded: bool = False
+        self.country: str = ""
 
     async def request(
         self,
         method: str,
         url: str,
         raw_reply: bool = False,
         raw_rsp: bool = False,
@@ -111,30 +117,37 @@
             rsp = await response.text()
 
         if raw_reply and raw_rsp:
             return response, rsp
         return rsp
 
     async def async_connect(
-        self, username: str, password: str, uris: dict[str, str], tries: int = 3
+        self, username: str, password: str, country: str, tries: int = 3
     ) -> None:
         """Connect to API."""
+        self.country = country
+        try:
+            await self._async_retrieve_url_service()
+        except HttpRequestError as error:
+            self.binded = False
+            raise AudiException("Failed retrieve urls service (%s)", error)
+
         try:
-            self.uris = uris
             await self._async_login(username, password)
+            self.binded = True
         except HttpRequestError as error:
             if tries > 1:
                 _LOGGER.warning(
                     "Login to Audi service failed, trying again in %s seconds [ERROR:%s]",
                     DELAY,
                     str(error),
                 )
                 await asyncio.sleep(DELAY)
-                return await self.async_connect(username, password, uris, tries - 1)
-
+                return await self.async_connect(username, password, country, tries - 1)
+            self.binded = False
             raise AuthorizationError("Login to Audi service failed: %s ", error)
 
     async def _async_login(self, user: str, password: str) -> None:
         """Request login."""
 
         # Generate code_challenge
         code_verifier = str(base64.urlsafe_b64encode(os.urandom(32)), "utf-8").strip(
@@ -284,46 +297,46 @@
             id_token=self._idk_token["id_token"]
         )
 
     async def async_refresh_tokens(self) -> None:
         """Refresh token if."""
         if self._mbb_token_expired and datetime.now() > self._mbb_token_expired:
             try:
-                _LOGGER.debug("Refresh token if necessary")
-                # MBB Token
+                _LOGGER.debug("Refresh MBB token")
                 refresh_token = self._mbb_token["refresh_token"]
                 self._mbb_token = await self._async_get_mbb_token(
                     refresh_token=refresh_token
                 )
                 # TR/2022-02-10: If a new refresh_token is provided, save it for further refreshes
                 if "refresh_token" not in self._mbb_token:
                     _LOGGER.debug("refresh token not provided")
                     self._mbb_token["refresh_token"] = refresh_token
 
                 self._mbb_token_expired = datetime.now() + timedelta(
                     seconds=self._mbb_token["expires_in"]
                 )
 
-                # IDK Token
+                _LOGGER.debug("Refresh IDK token")
                 self._idk_token = await self._async_get_idk_token(
                     refresh_token=self._idk_token["refresh_token"]
                 )
 
-                # Audi token
+                _LOGGER.debug("Refresh Audi token")
                 self._audi_token = await self._async_get_azs_token(
                     id_token=self._idk_token["access_token"]
                 )
 
-                # Here token
+                _LOGGER.debug("Refresh Here token")
                 self._here_token = await self._async_get_here_token(
                     id_token=self._idk_token["id_token"]
                 )
 
-            except AudiException as error:  # pylint: disable=broad-except
-                _LOGGER.error("Refresh token failed: %s", str(error))
+            except AudiException as error:
+                _LOGGER.error("Refresh token failed: %s", error)
+                self.binded = False
 
     async def async_get_action_headers(
         self, content_type: str, security_token: str | None, x_security: bool = False
     ) -> dict[str, str]:
         """Return header for vehicle action."""
         headers = {
             "Content-Type": content_type,
@@ -583,7 +596,62 @@
             self.uris["mbb_url"] + "/mobile/oauth2/v1/token",
             data=encoded_hereoauth_data,
             headers=headers,
             allow_redirects=False,
         )
         _LOGGER.debug("Here Token: %s", hereoauth_json)
         return hereoauth_json
+
+    async def _async_retrieve_url_service(self) -> None:
+        """Get urls for request."""
+        # Get markets to get language
+        country = self.country.upper()
+        markets_json = await self.request("GET", f"{MARKET_URL}/markets")
+
+        country_spec = ExtendedDict(markets_json).getr(
+            "countries.countrySpecifications"
+        )
+        if country not in country_spec:
+            raise AudiException("Country not found")
+
+        language = country_spec[country].get("defaultLanguage")
+
+        # Get market config
+        services = await self.request(
+            "GET", f"{MARKET_URL}/market/{country}/{language}"
+        )
+
+        client_id = services.get("idkClientIDAndroidLive", CLIENT_ID)
+        audi_baseurl = services.get(
+            "myAudiAuthorizationServerProxyServiceURLProduction"
+        )
+        profil_url = (
+            services.get("idkCustomerProfileMicroserviceBaseURLLive", "") + "/v3"
+        )
+        mbb_baseurl = services.get("mbbOAuthBaseURLLive", MBB_URL)
+        cvvsb_base_url = services.get("connectedVehicleVehicleServiceBaseURLProduction")
+
+        # Get openId config
+        openid_url = services.get("idkLoginServiceConfigurationURLProduction")
+        _LOGGER.debug("IDK Base Url: %s", openid_url)
+        openid_json = await self.request("GET", openid_url)
+
+        authorization_endpoint_url = openid_json.get("authorization_endpoint", "")
+        token_endpoint_url = openid_json.get("token_endpoint", "")
+        revocation_endpoint_url = openid_json.get("revocation_endpoint", "")
+
+        self.uris = {
+            "client_id": client_id,
+            "audi_url": audi_baseurl,
+            "profil_url": profil_url,
+            "mbb_url": mbb_baseurl,
+            "here_url": URL_HERE_COM,
+            "cv_url": cvvsb_base_url,
+            "user_url": URL_INFO_USER,
+            "authorization_endpoint": authorization_endpoint_url,
+            "token_endpoint": token_endpoint_url,
+            "revocation_endpoint": revocation_endpoint_url,
+            "language": language,
+            "country": country,
+        }
+
+        _LOGGER.debug("Urls of service: %s", self.uris)
```

### Comparing `audiconnectpy-2.2.1/audiconnectpy/const.py` & `audiconnectpy-2.2.2/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/audiconnectpy/helpers.py` & `audiconnectpy-2.2.2/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/audiconnectpy/model.py` & `audiconnectpy-2.2.2/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/audiconnectpy/vehicle.py` & `audiconnectpy-2.2.2/audiconnectpy/vehicle.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,23 +50,25 @@
 class Vehicle(DataClassDictMixin):  # type: ignore
     """Vehicle class."""
 
     vin: str
     csid: str
     nickname: str | None = None
     last_access: datetime | None = None
-    uris: dict[str, str] = field(init=False)
+    uris: dict[str, Any] = field(init=False)
+    fill_region: Any = field(init=False)
     auth: Any = field(init=False)
     spin: str | None = field(init=False, default=None)
     infos: Information | None = field(
         metadata=field_options(alias="vehicle"), default=None
     )
     capabilities: list[str] | None = field(init=False, default=None)
     position: Position | None = field(init=False, default=None)
     location: Location | None = field(init=False, default=None)
+    last_update: datetime | None = field(init=False, default=None)
 
     @property
     def api_level(self) -> dict[str, int]:
         """Return API Level."""
         return {
             "climatisation": 2,  # 2 or 3
             "ventilation": 1,  # 1 or other
@@ -117,14 +119,15 @@
                 "addresses": [
                     item
                     for item in location.get("data", [])
                     if "proprietaryData" in item
                 ],
             }
         )
+        self.last_update = datetime.now()
 
     async def async_get_location(self) -> Any:
         """Get destination data."""
         headers = await self.auth.async_get_headers(token_type="here")
         data = await self.auth.request(
             "GET", f"{self.uris['here_url']}/location", headers=headers
         )
@@ -146,14 +149,24 @@
         data = await self.auth.request(
             "GET",
             f"{self.uris['cv_url']}/vehicles/{self.vin}/capabilities",
             headers=headers,
         )
         return data
 
+    async def async_get(self, path: str) -> Any:
+        """Get data."""
+        headers = await self.auth.async_get_headers(token_type="idk")
+        data = await self.auth.request(
+            "GET",
+            f"{self.uris['cv_url']}/vehicles/{self.vin}/{path}",
+            headers=headers,
+        )
+        return data
+
     async def async_get_selectivestatus(self, jobs: Iterable[str] | None = None) -> Any:
         """Get capabilities."""
         if jobs is None:
             headers = await self.auth.async_get_headers(token_type="idk")
             capabilities = await self.auth.request(
                 "GET",
                 f"{self.uris['cv_url']}/vehicles/{self.vin}/selectivestatus?jobs=userCapabilities",
@@ -187,21 +200,21 @@
         data: str | dict[str, Any] = (
             '<?xml version="1.0" encoding= "UTF-8" ?>'
             + f'<rluAction xmlns="http://audi.de/connect/rlu"><action>{"lock" if lock else "unlock"}</action></rluAction>'
         )
 
         rsp = await self.auth.request(
             "POST",
-            f"{self.uris['url']}/bs/rlu/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/actions",
+            f"{self.fill_region.url}/bs/rlu/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/actions",
             headers=headers,
             data=data,
         )
         request_id = ExtendedDict(rsp).getr("rluActionResponse.requestId", "")
         await self._async_check_request(
-            f"{self.uris['url']}/bs/rlu/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/requests/{request_id}/status",
+            f"{self.fill_region.url}/bs/rlu/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/requests/{request_id}/status",
             "lock vehicle" if lock else "unlock vehicle",
             REQUEST_SUCCESSFUL,
             REQUEST_FAILED,
             "requestStatusResponse.status",
         )
 
     async def async_set_climater(
@@ -254,21 +267,21 @@
                 if start
                 else {"action": {"type": "stopClimatisation"}}
             )
             data = json.dumps(data)
 
         rsp = await self.auth.request(
             "POST",
-            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
+            f"{self.fill_region.url}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
         )
         actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
-            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
+            f"{self.fill_region.url}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "start climatisation" if start else "stop climatisation",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_climater_temp(
@@ -322,21 +335,21 @@
                         },
                     },
                 }
             }
             data = json.dumps(data)
         rsp = await self.auth.request(
             "POST",
-            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
+            f"{self.fill_region.url}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
         )
         actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
-            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
+            f"{self.fill_region.url}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "set target temperature",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_pre_heating(self, start: bool, duration: int = 60) -> None:
@@ -369,15 +382,15 @@
                 if start
                 else {"performAction": {"quickstop": {"active": False}}}
             )
             data = json.dumps(data)
 
         await self.auth.request(
             "POST",
-            f"{self.uris['url']}/bs/rs/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/action",
+            f"{self.fill_region.url}/bs/rs/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/action",
             headers=headers,
             data=data,
         )
 
     async def async_set_ventilation(self, start: bool, duration: int = 60) -> None:
         """Set ventilation."""
         security_token = await self._async_get_security_token(
@@ -417,15 +430,15 @@
                 if start
                 else {"performAction": {"quickstop": {"active": False}}}
             )
             data = json.dumps(data)
 
         await self.auth.request(
             "POST",
-            f"{self.uris['url']}/bs/rs/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/action",
+            f"{self.fill_region.url}/bs/rs/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/action",
             headers=headers,
             data=data,
         )
 
     async def async_set_battery_charger(self, start: bool, timer: bool = False) -> None:
         """Set battery charger."""
         if self.api_level["charger"] == 2:
@@ -456,21 +469,21 @@
             headers = await self.auth.async_get_action_headers(
                 "application/vnd.vwg.mbb.ChargerAction_v1_0_0+xml", None
             )
             data = f'<?xml version="1.0" encoding="UTF-8" ?><action><type>{"start" if start else "stop"}</type></action>'
 
         rsp = await self.auth.request(
             "POST",
-            f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions",
+            f"{self.fill_region.url}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions",
             headers=headers,
             data=data,
         )
         actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
-            f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions/{actionid}",
+            f"{self.fill_region.url}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions/{actionid}",
             "start charger" if start else "stop charger",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_charger_max(self, current: float = 32) -> None:
@@ -492,21 +505,21 @@
             data = (
                 '<?xml version="1.0" encoding="UTF-8" ?><action><type>setSettings</type>'
                 + f"<settings><maxChargeCurrent>{current}</maxChargeCurrent></settings></action>"
             )
 
         rsp = await self.auth.request(
             "POST",
-            f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions",
+            f"{self.fill_region.url}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions",
             headers=headers,
             data=data,
         )
         actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
-            f"{self.uris['url']}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions/{actionid}",
+            f"{self.fill_region.url}/bs/batterycharge/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/charger/actions/{actionid}",
             "set charger max current",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_window_heating(self, start: bool) -> None:
@@ -525,21 +538,21 @@
             )
             data = (
                 '<?xml version="1.0" encoding= "UTF-8" ?>'
                 + f"<action><type>{'startWindowHeating' if start else 'stopWindowHeating'}</type></action>"
             )
         rsp = await self.auth.request(
             "POST",
-            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
+            f"{self.fill_region.url}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions",
             headers=headers,
             data=data,
         )
         actionid = ExtendedDict(rsp).getr("action.actionId", "")
         await self._async_check_request(
-            f"{self.uris['url']}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
+            f"{self.fill_region.url}/bs/climatisation/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/climater/actions/{actionid}",
             "start window heating" if start else "stop window heating",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def async_set_honkflash(
@@ -558,15 +571,15 @@
                         "latitude": self.position.latitude,
                         "longitude": self.position.longitude,
                     },
                 }
             }
             await self.auth.request(
                 "POST",
-                f"{self.uris['url']}/bs/rhf/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/honkAndFlash",
+                f"{self.fill_region.url}/bs/rhf/v1/{BRAND}/{self.uris['country']}/vehicles/{self.vin}/honkAndFlash",
                 headers=headers,
                 json=data,
             )
 
     async def async_refresh_vehicle_data(self) -> None:
         """Refresh vehicle data."""
         headers = await self.auth.async_get_headers(token_type="idk")
@@ -641,15 +654,15 @@
             logger.error("Security PIN not found")
             return ""
 
         # Challenge
         headers = await self.auth.async_get_headers(token_type="mbb", okhttp=True)
         rsp = await self.auth.request(
             "GET",
-            f"{self.uris['url_setter']}/rolesrights/authorization/v2/vehicles/{self.vin}/services/{action}/security-pin-auth-requested",
+            f"{self.fill_region.url_setter}/rolesrights/authorization/v2/vehicles/{self.vin}/services/{action}/security-pin-auth-requested",
             headers=headers,
         )
         rsp = ExtendedDict(rsp)
         sec_token: str = rsp.getr("securityPinAuthInfo.securityToken")
         challenge: str = rsp.getr(
             "securityPinAuthInfo.securityPinTransmission.challenge"
         )
@@ -663,12 +676,12 @@
                     "securityPinHash": spin_hash(self.spin, challenge),
                 },
                 "securityToken": sec_token,
             }
         }
         response = await self.auth.request(
             "POST",
-            f"{self.uris['url_setter']}/rolesrights/authorization/v2/security-pin-auth-completed",
+            f"{self.fill_region.url_setter}/rolesrights/authorization/v2/security-pin-auth-completed",
             headers=headers,
             json=data,
         )
         return cast(str, response.get("securityToken", ""))
```

### Comparing `audiconnectpy-2.2.1/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.2.2/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.1
+Version: 2.2.2
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.1/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.2.2/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/example.py` & `audiconnectpy-2.2.2/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/pyproject.toml` & `audiconnectpy-2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/tests/conftest.py` & `audiconnectpy-2.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/tests/fixtures/audi0.json` & `audiconnectpy-2.2.2/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/tests/fixtures/audi1.json` & `audiconnectpy-2.2.2/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/tests/fixtures/audi2.json` & `audiconnectpy-2.2.2/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.2.2/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/tests/fixtures/location.json` & `audiconnectpy-2.2.2/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.1/tests/test_home.py` & `audiconnectpy-2.2.2/tests/test_home.py`

 * *Files identical despite different names*


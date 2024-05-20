# Comparing `tmp/goslide-api-0.6.7.tar.gz` & `tmp/goslide-api-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goslide-api-0.6.7.tar", last modified: Thu Dec 21 11:33:59 2023, max compression
+gzip compressed data, was "goslide-api-0.6.8.tar", last modified: Mon May 20 16:41:35 2024, max compression
```

## Comparing `goslide-api-0.6.7.tar` & `goslide-api-0.6.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2023-12-21 11:33:59.208206 goslide-api-0.6.7/
--rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)     1077 2023-12-21 11:33:59.208206 goslide-api-0.6.7/PKG-INFO
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1121 2020-04-17 08:21:18.000000 goslide-api-0.6.7/README.md
-drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2023-12-21 11:33:59.208206 goslide-api-0.6.7/goslide_api.egg-info/
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1077 2023-12-21 11:33:59.000000 goslide-api-0.6.7/goslide_api.egg-info/PKG-INFO
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)      240 2023-12-21 11:33:59.000000 goslide-api-0.6.7/goslide_api.egg-info/SOURCES.txt
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)        1 2023-12-21 11:33:59.000000 goslide-api-0.6.7/goslide_api.egg-info/dependency_links.txt
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)        8 2023-12-21 11:33:59.000000 goslide-api-0.6.7/goslide_api.egg-info/requires.txt
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)       11 2023-12-21 11:33:59.000000 goslide-api-0.6.7/goslide_api.egg-info/top_level.txt
-drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2023-12-21 11:33:59.208206 goslide-api-0.6.7/goslideapi/
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)       80 2020-01-26 08:18:44.000000 goslide-api-0.6.7/goslideapi/__init__.py
--rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)    25511 2023-12-21 11:33:09.000000 goslide-api-0.6.7/goslideapi/goslideapi.py
--rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)       38 2023-12-21 11:33:59.208206 goslide-api-0.6.7/setup.cfg
--rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1000 2023-12-21 11:33:56.000000 goslide-api-0.6.7/setup.py
+drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-20 16:41:35.103896 goslide-api-0.6.8/
+-rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)     1169 2024-05-20 16:41:35.103896 goslide-api-0.6.8/PKG-INFO
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1500 2024-05-20 15:11:10.000000 goslide-api-0.6.8/README.md
+drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-20 16:41:35.103896 goslide-api-0.6.8/goslide_api.egg-info/
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)     1169 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/PKG-INFO
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)      240 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)        1 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)        8 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/requires.txt
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)       11 2024-05-20 16:41:35.000000 goslide-api-0.6.8/goslide_api.egg-info/top_level.txt
+drwxr-xr-x   0 aakuiper  (1000) aakuiper  (1000)        0 2024-05-20 16:41:35.103896 goslide-api-0.6.8/goslideapi/
+-rw-rw-r--   0 aakuiper  (1000) aakuiper  (1000)       80 2020-01-26 08:18:44.000000 goslide-api-0.6.8/goslideapi/__init__.py
+-rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)    26303 2024-05-20 16:23:57.000000 goslide-api-0.6.8/goslideapi/goslideapi.py
+-rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)       38 2024-05-20 16:41:35.103896 goslide-api-0.6.8/setup.cfg
+-rw-r--r--   0 aakuiper  (1000) aakuiper  (1000)     1100 2024-05-20 15:01:51.000000 goslide-api-0.6.8/setup.py
```

### Comparing `goslide-api-0.6.7/PKG-INFO` & `goslide-api-0.6.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: goslide-api
-Version: 0.6.7
+Version: 0.6.8
 Summary: Python API to utilise the Slide Open Cloud and Local API
 Home-page: https://github.com/ualex73/goslide-api
 Author: Alexander Kuiper
 Author-email: ualex73@gmail.com
 License: Apache License 2.0
 Description: 
         # GoSlide Open Cloud API
         
-        Python API to utilise the GoSlide Open Cloud and Local JSON API
+        Python API to utilise the GoSlide Local and Cloud API
         
         ## Requirements
         
         - Python >= 3.5.2
         
         ## Usage
         
@@ -26,11 +26,13 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5.2
 Description-Content-Type: text/markdown
```

### Comparing `goslide-api-0.6.7/README.md` & `goslide-api-0.6.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,31 @@
 
 Python API to utilise the GoSlide Open Cloud and Local JSON API
 
 ## Requirements
 
 - Python >= 3.5.2
 
-## Usage
+## Usage Local
+```python
+
+import asyncio
+from goslideapi import GoSlideLocal
+
+loop = asyncio.get_event_loop()
+goslide = GoSlideLocal
+
+result = loop.run_until_complete(goslide.slide_add("192.168.1.1", "anypassword", 2))
+slide = loop.run_until_complete(goslide.slide_info("192.168.1.1"))
+loop.run_until_complete(goslide.slide_open("192.168.1.1"))
+loop.run_until_complete(goslide.slide_close("192.168.1.1"))
+
+```
+
+## Usage Cloud
 ```python
 
 import asyncio
 from goslideapi import GoSlideCloud
 
 loop = asyncio.get_event_loop()
 goslide = GoSlideCloud('email', 'password')
@@ -39,15 +55,11 @@
     result = loop.run_until_complete(goslide.slide_close(1))
 
     loop.run_until_complete(goslide.logout())
 else:
     print('login failed')
 ```
 
-## TODO
-
-- Expose more API functions
-
 ## License
 
 Apache License 2.0
```

### Comparing `goslide-api-0.6.7/goslide_api.egg-info/PKG-INFO` & `goslide-api-0.6.8/goslide_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: goslide-api
-Version: 0.6.7
+Version: 0.6.8
 Summary: Python API to utilise the Slide Open Cloud and Local API
 Home-page: https://github.com/ualex73/goslide-api
 Author: Alexander Kuiper
 Author-email: ualex73@gmail.com
 License: Apache License 2.0
 Description: 
         # GoSlide Open Cloud API
         
-        Python API to utilise the GoSlide Open Cloud and Local JSON API
+        Python API to utilise the GoSlide Local and Cloud API
         
         ## Requirements
         
         - Python >= 3.5.2
         
         ## Usage
         
@@ -26,11 +26,13 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5.2
 Description-Content-Type: text/markdown
```

### Comparing `goslide-api-0.6.7/goslideapi/goslideapi.py` & `goslide-api-0.6.8/goslideapi/goslideapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -429,22 +429,22 @@
         )
         return bool(resp)
 
 
 class GoSlideLocal:
     """API Wrapper for the Go Slide devices, local connectivity."""
 
-    def __init__(self, timeout=DEFAULT_TIMEOUT, authexception=True, apiversion=2):
+    def __init__(self, timeout=DEFAULT_TIMEOUT, authexception=True):
         """Create the object with required parameters."""
         self._timeout = timeout
         self._authexception = authexception
-        self._apiversion = apiversion
         self._cnoncecount = 0
         self._requestcount = 0
-        self._slides = {}
+        self._slide_passwd = {}
+        self._slide_api = {}
 
     def _md5_utf8(self, x):
         if isinstance(x, str):
             x = x.encode("utf-8")
         return hashlib.md5(x).hexdigest()
 
     def _make_digest_auth(self, username, password, method, uri, my_auth):
@@ -572,15 +572,15 @@
             aiohttp.client_exceptions.ClientConnectionError,
             aiohttp.client_exceptions.ClientConnectorError,
         ) as err:
             raise ClientConnectionError(str(err)) from None
         except asyncio.TimeoutError as err:
             raise ClientTimeoutError("Connection Timeout") from None
 
-    async def _request(self, hostname, password, reqtype, uri, data=None):
+    async def _request(self, hostname, password, apiversion, reqtype, uri, data=None):
         """Digest authentication using dorequest."""
 
         # Local API uses digest authentication:
         # https://en.wikipedia.org/wiki/Digest_access_authentication
 
         # We need to send 2 requests:
         #  - first request will result in a 401 with a response header "WWW-Authenticate"
@@ -589,20 +589,20 @@
         # format URL with hostname/ip and uri value
         url = "http://{}{}".format(hostname, uri)
 
         # First request, should return a 401 error for v1
         # First request is not required for v2
 
         # Default is version 1, when we do WWW-Authentication
-        if self._apiversion == 1:
+        if apiversion == 1:
 
-            #do request to obtain a WWW-authentication header:
+            # do request to obtain a WWW-authentication header:
             respstatus, resptext = await self._dorequest(reqtype, url)
 
-            #Only a 401 response is correct
+            # Only a 401 response is correct
             if respstatus == 401:
 
                 # The resptext contains the WWW-Authentication header
                 auth = self._make_digest_auth("user", password, reqtype, uri, resptext)
 
                 respstatus, resptext = await self._dorequest(
                     reqtype, url, digestauth=auth, data=data
@@ -615,54 +615,59 @@
                 _LOGGER.error(
                     "Failed request with Local API Digest Authentication challenge. HTTPCode=%s",
                     respstatus,
                 )
             else:
                 # We expected a 401 Digest Auth here
                 _LOGGER.error(
-                    "Failed request with Local API v1. Received HTTPCode=%s, expected HTTPCode=401. Maybe try switching to v2?",
+                    "Failed request with Local API v1. Received HTTPCode=%s, expected HTTPCode=401. Maybe try switching to api version 2?",
                     respstatus,
                 )
 
-        elif self._apiversion == 2:
+        elif apiversion == 2:
 
-                respstatus, resptext = await self._dorequest(
-                    reqtype, url, data=data
-                )
+            respstatus, resptext = await self._dorequest(reqtype, url, data=data)
 
-                if respstatus == 200:
-                    return resptext
+            if respstatus == 200:
+                return resptext
 
-                # Anything else is an error
-                _LOGGER.error(
-                    "Failed request Local API v2. HTTPCode=%s",
-                    respstatus,
-                )
+            # Anything else is an error
+            _LOGGER.error(
+                "Failed request Local API v2. HTTPCode=%s",
+                respstatus,
+            )
 
         else:
             _LOGGER.error(
                 "Only v1 and v2 is supported.",
             )
 
         return None
 
-    async def slide_add(self, hostname, password):
+    async def slide_add(self, hostname, password, api=2):
         """Add slide to internal table, then you can use the local API."""
-        self._slides[hostname] = password
+        self._slide_passwd[hostname] = password
+        self._slide_api[hostname] = api
 
     async def slide_del(self, hostname):
         """Delete slide from internal table."""
-        if hostname in self._slides:
-            self._slides.remove(hostname)
+        if hostname in self._slide_passwd:
+            self._slide_passwd.remove(hostname)
+        if hostname in self._slide_api:
+            self._slide_api.remove(hostname)
         else:
             _LOGGER.error("Tried to delete none-existing '%s' from list", hostname)
 
+    async def slide_list(self):
+        """List all registered slides."""
+        return list(self._slide_passwd.keys())
+
     async def _slide_exist(self, hostname):
         """Function to check if slide exist in internal table."""
-        if hostname in self._slides:
+        if hostname in self._slide_passwd:
             return True
         else:
             _LOGGER.error(
                 "Cannot find hostname '%s' in list, forgot to call 'slide_add'?",
                 hostname,
             )
             return False
@@ -682,15 +687,19 @@
         #   "touch_go": true
         # }
 
         if not await self._slide_exist(hostname):
             return None
 
         result = await self._request(
-            hostname, self._slides[hostname], "POST", "/rpc/Slide.GetInfo"
+            hostname,
+            self._slide_passwd[hostname],
+            self._slide_api[hostname],
+            "POST",
+            "/rpc/Slide.GetInfo",
         )
 
         return result
 
     async def slide_get_position(self, hostname):
         """Retrieve the slide position."""
         result = await self.slide_info(hostname)
@@ -715,64 +724,88 @@
             _LOGGER.error("SlideSetPosition: '%s' has to be between 0.0-1.0", pos)
             return False
 
         if not await self._slide_exist(hostname):
             return False
 
         resp = await self._request(
-            hostname, self._slides[hostname], "POST", "/rpc/Slide.SetPos", {"pos": pos}
+            hostname,
+            self._slide_passwd[hostname],
+            self._slide_api[hostname],
+            "POST",
+            "/rpc/Slide.SetPos",
+            data={"pos": pos},
         )
         return bool(resp)
 
     async def slide_open(self, hostname):
         """Open a slide."""
         if not await self._slide_exist(hostname):
             return False
 
         resp = await self._request(
-            hostname, self._slides[hostname], "POST", "/rpc/Slide.SetPos", {"pos": 0.0}
+            hostname,
+            self._slide_passwd[hostname],
+            self._slide_api[hostname],
+            "POST",
+            "/rpc/Slide.SetPos",
+            data={"pos": 0.0},
         )
         return bool(resp)
 
     async def slide_close(self, hostname):
         """Close a slide."""
         if not await self._slide_exist(hostname):
             return False
 
         resp = await self._request(
-            hostname, self._slides[hostname], "POST", "/rpc/Slide.SetPos", {"pos": 1.0}
+            hostname,
+            self._slide_passwd[hostname],
+            self._slide_api[hostname],
+            "POST",
+            "/rpc/Slide.SetPos",
+            data={"pos": 1.0},
         )
         return bool(resp)
 
     async def slide_stop(self, hostname):
         """Stop a slide."""
         if not await self._slide_exist(hostname):
             return False
 
         resp = await self._request(
-            hostname, self._slides[hostname], "POST", "/rpc/Slide.Stop"
+            hostname,
+            self._slide_passwd[hostname],
+            self._slide_api[hostname],
+            "POST",
+            "/rpc/Slide.Stop",
         )
         return bool(resp)
 
     async def slide_calibrate(self, hostname):
         """Calibrate a slide."""
         if not await self._slide_exist(hostname):
             return False
 
         resp = await self._request(
-            hostname, self._slides[hostname], "POST", "/rpc/Slide.Calibrate"
+            hostname,
+            self._slide_passwd[hostname],
+            self._slide_api[hostname],
+            "POST",
+            "/rpc/Slide.Calibrate",
         )
         return bool(resp)
 
     async def slide_configwifi(self, hostname, ssid, password):
         """Configure slide wifi."""
         if not await self._slide_exist(hostname):
             return False
 
         resp = await self._request(
             hostname,
-            self._slides[hostname],
+            self._slide_passwd[hostname],
+            self._slide_api[hostname],
             "POST",
             "/rpc/Slide.Config.Wifi",
             {"ssid": ssid, "pass": password},
         )
         return bool(resp)
```

### Comparing `goslide-api-0.6.7/setup.py` & `goslide-api-0.6.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.pypi') as f:
     LONG_DESCRIPTION = f.read()
 
 setuptools.setup(
     name='goslide-api',
-    version='0.6.7',
+    version='0.6.8',
     url='https://github.com/ualex73/goslide-api',
     license='Apache License 2.0',
     author='Alexander Kuiper',
     author_email='ualex73@gmail.com',
     description='Python API to utilise the Slide Open Cloud and Local API',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
@@ -22,11 +22,13 @@
     python_requires='>=3.5.2',
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
 )
```


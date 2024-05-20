# Comparing `tmp/trio_binance-0.4.0.tar.gz` & `tmp/trio_binance-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trio_binance-0.4.0.tar", max compression
+gzip compressed data, was "trio_binance-0.4.1.tar", max compression
```

## Comparing `trio_binance-0.4.0.tar` & `trio_binance-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.4.0/LICENSE
--rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.4.0/README.rst
--rw-r--r--   0        0        0     1080 2024-05-08 09:50:15.170478 trio_binance-0.4.0/pyproject.toml
--rwxr-xr-x   0        0        0       67 2024-05-08 09:50:15.173637 trio_binance-0.4.0/trio_binance/__init__.py
--rwxr-xr-x   0        0        0    79850 2024-05-08 09:09:24.261092 trio_binance-0.4.0/trio_binance/client.py
--rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.4.0/trio_binance/enums.py
--rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.4.0/trio_binance/exceptions.py
--rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.4.0/trio_binance/helpers.py
--rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.4.0/trio_binance/streams.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 trio_binance-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-11-18 07:43:08.000000 trio_binance-0.4.1/LICENSE
+-rwxr-xr-x   0        0        0     1143 2022-01-12 05:13:36.000000 trio_binance-0.4.1/README.rst
+-rw-r--r--   0        0        0     1080 2024-05-20 01:43:11.707867 trio_binance-0.4.1/pyproject.toml
+-rwxr-xr-x   0        0        0       67 2024-05-20 01:43:15.853942 trio_binance-0.4.1/trio_binance/__init__.py
+-rwxr-xr-x   0        0        0    79811 2024-05-16 06:18:42.288051 trio_binance-0.4.1/trio_binance/client.py
+-rw-r--r--   0        0        0     1891 2024-04-23 01:56:20.850456 trio_binance-0.4.1/trio_binance/enums.py
+-rw-r--r--   0        0        0     2260 2024-04-23 02:07:31.211547 trio_binance-0.4.1/trio_binance/exceptions.py
+-rw-r--r--   0        0        0     1493 2024-04-23 02:07:31.211671 trio_binance-0.4.1/trio_binance/helpers.py
+-rw-r--r--   0        0        0     3780 2024-04-23 05:34:24.595456 trio_binance-0.4.1/trio_binance/streams.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 trio_binance-0.4.1/PKG-INFO
```

### Comparing `trio_binance-0.4.0/LICENSE` & `trio_binance-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.0/README.rst` & `trio_binance-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.0/pyproject.toml` & `trio_binance-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trio-binance"
-version = "0.4.0"
+version = "0.4.1"
 description = "trio based asynchronous binance SDK"
 authors = ["Shu Wang <halfelf.ronin@gmail.com>"]
 keywords = ["binance", "python-trio"]
 readme = "README.rst"
 license = "MIT"
 homepage = "https://github.com/halfelf/trio-binance"
 repository = "https://github.com/halfelf/trio-binance"
```

### Comparing `trio_binance-0.4.0/trio_binance/client.py` & `trio_binance-0.4.1/trio_binance/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,14 @@
         self.FUTURES_COIN_URL = self.FUTURES_COIN_URL.format(tld)
         self.FUTURES_COIN_DATA_URL = self.FUTURES_COIN_DATA_URL.format(tld)
         self.OPTIONS_URL = self.OPTIONS_URL.format(tld)
         self.OPTIONS_TESTNET_URL = self.OPTIONS_TESTNET_URL.format(tld)
 
         self.API_KEY = api_key
         self._requests_params = requests_params
-        self.response = None
         self.testnet = testnet
         self.timestamp_offset = 0
         if sign_style != "HMAC" and sign_style != "RSA" and sign_style != "Ed25519":
             raise ValueError("Invalid sign style. Must be HMAC or RSA")
         self.sign_style = sign_style
         self.API_SECRET: Union[Ed25519PrivateKey, RSAPrivateKey, str]
         if self.sign_style != "HMAC":
@@ -374,16 +373,16 @@
         kwargs = self._get_request_kwargs(method, signed, force_params, **kwargs)
         if method.lower() == "get":
             req = self.session.build_request(method, uri, params=kwargs.get("params", ""), timeout=self.REQUEST_TIMEOUT)
         else:
             req = self.session.build_request(
                 method, uri, json=dict(kwargs.get("data", {})), timeout=self.REQUEST_TIMEOUT
             )
-        self.response = await self.session.send(req)
-        return await self._handle_response(self.response)
+        response = await self.session.send(req)
+        return await self._handle_response(response)
 
     @staticmethod
     async def _handle_response(response: httpx.Response):
         """Internal helper for handling API responses from the Binance server.
         Raises the appropriate exceptions when necessary; otherwise, returns the
         response.
         """
```

### Comparing `trio_binance-0.4.0/trio_binance/enums.py` & `trio_binance-0.4.1/trio_binance/enums.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.0/trio_binance/exceptions.py` & `trio_binance-0.4.1/trio_binance/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.0/trio_binance/helpers.py` & `trio_binance-0.4.1/trio_binance/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.0/trio_binance/streams.py` & `trio_binance-0.4.1/trio_binance/streams.py`

 * *Files identical despite different names*

### Comparing `trio_binance-0.4.0/PKG-INFO` & `trio_binance-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-binance
-Version: 0.4.0
+Version: 0.4.1
 Summary: trio based asynchronous binance SDK
 Home-page: https://github.com/halfelf/trio-binance
 License: MIT
 Keywords: binance,python-trio
 Author: Shu Wang
 Author-email: halfelf.ronin@gmail.com
 Requires-Python: >=3.11,<4.0
```


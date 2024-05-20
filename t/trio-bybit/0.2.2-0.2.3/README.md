# Comparing `tmp/trio_bybit-0.2.2.tar.gz` & `tmp/trio_bybit-0.2.3.tar.gz`

## Comparing `trio_bybit-0.2.2.tar` & `trio_bybit-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/keypair.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/pkcs8.key
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/pytest.ini
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/tests/test_async_client.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/tests/test_rsa.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/tests/test_streams.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/trio_bybit/__init__.py
--rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/trio_bybit/client.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/trio_bybit/enums.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/trio_bybit/exceptions.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/trio_bybit/helpers.py
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/trio_bybit/streams.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/LICENSE
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/README.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 trio_bybit-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/keypair.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/pkcs8.key
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/pytest.ini
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/tests/test_async_client.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/tests/test_rsa.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/tests/test_streams.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/trio_bybit/__init__.py
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/trio_bybit/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/trio_bybit/enums.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/trio_bybit/exceptions.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/trio_bybit/helpers.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/trio_bybit/streams.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/LICENSE
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/README.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 trio_bybit-0.2.3/PKG-INFO
```

### Comparing `trio_bybit-0.2.2/keypair.pem` & `trio_bybit-0.2.3/keypair.pem`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/pkcs8.key` & `trio_bybit-0.2.3/pkcs8.key`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/test.py` & `trio_bybit-0.2.3/test.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/tests/test_async_client.py` & `trio_bybit-0.2.3/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/tests/test_rsa.py` & `trio_bybit-0.2.3/tests/test_rsa.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/tests/test_streams.py` & `trio_bybit-0.2.3/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/trio_bybit/client.py` & `trio_bybit-0.2.3/trio_bybit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         self.API_SECRET: RSAPrivateKey | str
         self.sign_style = sign_style
         if self.sign_style != "HMAC":
             with open(api_secret, "rb") as f:
                 self.API_SECRET = load_pem_private_key(f.read(), password=None)
         else:
             self.API_SECRET = api_secret
-        self.response = None
         self.receive_window = receive_window
         if sign_style != "HMAC" and sign_style != "RSA":
             raise ValueError("Invalid sign style. Must be HMAC or RSA")
         self.sign_style = sign_style
         self.timestamp_offset = 0
         if alternative_net == "test":
             self.base = self.TEST_NET_API_URL
@@ -146,17 +145,16 @@
     async def close_connection(self):
         if self.session:
             assert self.session
             await self.session.aclose()
 
     async def _request(self, method, uri: httpx.URL, signed: bool, **kwargs):
         request: httpx.Request = self._get_request(method, uri, signed, **kwargs)
-        self.response = await self.session.send(request)
-        # self.response = await getattr(self.session, method)(uri, **kwargs)
-        return await self._handle_response(self.response)
+        response = await self.session.send(request)
+        return await self._handle_response(response)
 
     @staticmethod
     async def _handle_response(response: httpx.Response):
         """Internal helper for handling API responses from the server.
         Raises the appropriate exceptions when necessary; otherwise, returns the
         response.
         """
```

### Comparing `trio_bybit-0.2.2/trio_bybit/exceptions.py` & `trio_bybit-0.2.3/trio_bybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/trio_bybit/helpers.py` & `trio_bybit-0.2.3/trio_bybit/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/trio_bybit/streams.py` & `trio_bybit-0.2.3/trio_bybit/streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,18 @@
             signature = self.api_secret.sign(
                 f"GET/realtime{expires}".encode("utf-8"), padding.PKCS1v15(), hashes.SHA256()
             )
             signature = base64.b64encode(signature).decode()
         await self.ws.send_message(orjson.dumps({"op": "auth", "args": [self.api_key, expires, signature]}))
         auth_ret = orjson.loads(await self.ws.get_message())
         if auth_ret["op"] == "auth":
-            assert auth_ret["success"]
+            try:
+                assert auth_ret["success"]
+            except AssertionError:
+                raise BybitWebsocketOpError(auth_ret)
             self.conn_id = auth_ret["conn_id"]
 
     async def subscribe(self, subscription: dict):
         """
         Subscribe or unsubscribe to a websocket stream.
         :param subscription: (un)subscription message, e.g. {"op": "subscribe", "args": ["publicTrade.BTCUSDT"]}
         """
```

### Comparing `trio_bybit-0.2.2/.gitignore` & `trio_bybit-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/LICENSE` & `trio_bybit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/README.md` & `trio_bybit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.2/pyproject.toml` & `trio_bybit-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trio-bybit"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python bybit async SDK based on trio."
 authors = [
     { name = "Shu Wang", email = "halfelf.ronin@gmail.com" }
 ]
 dependencies = [
     "trio>=0.25.0",
     "httpx[http2]>=0.27.0",
```

### Comparing `trio_bybit-0.2.2/PKG-INFO` & `trio_bybit-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trio-bybit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python bybit async SDK based on trio.
 Project-URL: Repository, https://github.com/halfelf/trio-bybit
 Author-email: Shu Wang <halfelf.ronin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shu Wang <halfelf.ronin@gmail.com>
```


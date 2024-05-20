# Comparing `tmp/aiocmcapi-0.6.4.tar.gz` & `tmp/aiocmcapi-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocmcapi-0.6.4.tar", last modified: Sat May 18 11:54:12 2024, max compression
+gzip compressed data, was "aiocmcapi-0.6.5.tar", last modified: Mon May 20 10:06:37 2024, max compression
```

## Comparing `aiocmcapi-0.6.4.tar` & `aiocmcapi-0.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 11:54:12.634490 aiocmcapi-0.6.4/
--rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.6.4/LICENSE
--rw-rw-rw-   0        0        0     2047 2024-05-18 11:54:12.633490 aiocmcapi-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 11:54:12.628489 aiocmcapi-0.6.4/aiocmcapi/
--rw-rw-rw-   0        0        0       61 2024-05-13 02:36:12.000000 aiocmcapi-0.6.4/aiocmcapi/__init__.py
--rw-rw-rw-   0        0        0      738 2024-05-12 15:05:54.000000 aiocmcapi-0.6.4/aiocmcapi/client.py
--rw-rw-rw-   0        0        0     1057 2024-05-18 11:52:43.000000 aiocmcapi-0.6.4/aiocmcapi/currency.py
-drwxrwxrwx   0        0        0        0 2024-05-18 11:54:12.632489 aiocmcapi-0.6.4/aiocmcapi.egg-info/
--rw-rw-rw-   0        0        0     2047 2024-05-18 11:54:12.000000 aiocmcapi-0.6.4/aiocmcapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-05-18 11:54:12.000000 aiocmcapi-0.6.4/aiocmcapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 11:54:12.000000 aiocmcapi-0.6.4/aiocmcapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-18 11:54:12.000000 aiocmcapi-0.6.4/aiocmcapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 11:54:12.000000 aiocmcapi-0.6.4/aiocmcapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      354 2024-05-18 11:54:07.000000 aiocmcapi-0.6.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 11:54:12.634490 aiocmcapi-0.6.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 10:06:37.018355 aiocmcapi-0.6.5/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0     3423 2024-05-20 10:06:37.017354 aiocmcapi-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3153 2024-05-20 09:59:10.000000 aiocmcapi-0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 10:06:37.012373 aiocmcapi-0.6.5/aiocmcapi/
+-rw-rw-rw-   0        0        0       61 2024-05-13 02:36:12.000000 aiocmcapi-0.6.5/aiocmcapi/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-05-12 15:05:54.000000 aiocmcapi-0.6.5/aiocmcapi/client.py
+-rw-rw-rw-   0        0        0     1352 2024-05-20 09:36:16.000000 aiocmcapi-0.6.5/aiocmcapi/currency.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:06:37.016357 aiocmcapi-0.6.5/aiocmcapi.egg-info/
+-rw-rw-rw-   0        0        0     3423 2024-05-20 10:06:36.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-05-20 10:06:37.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 10:06:36.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-20 10:06:36.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-20 10:06:36.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      354 2024-05-20 10:06:30.000000 aiocmcapi-0.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 10:06:37.018355 aiocmcapi-0.6.5/setup.cfg
```

### Comparing `aiocmcapi-0.6.4/LICENSE` & `aiocmcapi-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.6.4/PKG-INFO` & `aiocmcapi-0.6.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-Metadata-Version: 2.1
-Name: aiocmcapi
-Version: 0.6.4
-Summary: Async wrapper for CoinMarketCap API
-Author-email: alobuzy <amozebus@gmail.com>
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp>=3.9.5
+![logo](https://github.com/alobuzy/aiocmcapi/assets/115936023/5e8fb136-9613-4369-9c68-260144a4f6bf)
 
 # aiocmcapi
+
 CoinMarketCap API async wrapper
 
 ## Installation
 
 pip
 
 ```sh
@@ -33,18 +26,18 @@
 from aiocmcapi import APIClient, Currency
 
 async def main():
     client = APIClient(
         api_key="YOUR_API_KEY_HERE"
     )
 
-    bitcoin = Currency(cmc_id=1)
+    btc = Currency(cmc_id=1)
 
-    await bitcoin.update(client)
-    print(f"Name: {bitcoin.name}\nPrice: {round(bitcoin.price, 2)}$")
+    await btc.update_data(client)
+    print(f"{btc.name} | {btc.symbol}\nPrice: {round(btc.price, 2)}$\nCMC Link: https://www.coinmarketcap.com/currencies/{btc.slug}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 or
 
@@ -57,54 +50,86 @@
     client = APIClient(
         api_key="YOUR_API_KEY_HERE"
     )
 
     cmc_id = 1
 
     r_json = await client.get(
-        endpoint_path="/v2/cryptocurrency/quotes/latest",
+        endpoint="/v2/cryptocurrency/quotes/latest",
         params={
             'id': cmc_id
         }
     )
-    data = r_json['data'][cmc_id]
+    data = r_json['data'][str(cmc_id)]
 
-    print(f"Name: {data['name']}\nPrice: {round(data['quote']['USD']['price'], 2)}$")
+    print(f"{data['name']} | {data['symbol']}\nPrice: {round(data['quote']['USD']['price'], 2)}$\nCMC Link: https://www.coinmarketcap.com/currencies/{data['slug']}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 Output:
 
 ```
-Name: Bitcoin
+Bitcoin | BTC
 Price: 62930.79$
+CMC Link: https://www.coinmarketcap.com/currencies/bitcoin
+```
+
+### For currency metadata
+
+```python
+import asyncio
+
+from aiocmcapi import APIClient, Currency
+
+async def main():
+    client = APIClient(
+        api_key="YOUR_API_KEY_HERE"
+    )
+
+    btc = Currency(cmc_id=1)
+    await btc.update_meta(client)
+
+    print(f"{btc.meta['name']} | {btc.meta['symbol']}\nDescription: {btc.meta['description']}\nWebsite: {btc.meta['urls']['website'][0]}")
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+Output:
+
+```
+Bitcoin | BTC
+Description: Bitcoin (BTC) is a cryptocurrency launched in 2010. Users are able to generate BTC through the process of mining. Bitcoin has a current supply of 19,700,812. The last known price of Bitcoin is 66,941.7329356 USD and is down -0.14 over the last 24 hours. It is currently trading on 11048 active market(s) with $23,083,624,310.30 traded over the last 24 hours. More information can be found at https://bitcoin.org/.
+Website: https://bitcoin.org/
 ```
 
 ## Example for other API endpoints
 
+[CoinMarketCap API endpoint overview](https://coinmarketcap.com/api/documentation/v1/#section/Endpoint-Overview)
+
 ```python
 import asyncio
 
 from aiocmcapi import APIClient
 
 async def main():
     client = APIClient(
         api_key="YOUR_API_KEY_HERE"
     )
 
     r_json = await client.get(
-        endpoint_path="/v1/cryptocurrency/listings/latest"
+        endpoint="/v1/cryptocurrency/listings/latest"
     )
 
     print(r_json)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 Output:
 
 ```
 {'status': {'timestamp': '2024-05-11T05:09:27.205Z', 'error_code': 0, 'error_message': None, 'elapsed': 21, 'credit_count': 1, 'notice': None, 'total_count': 9933}, 'data': [{'id': 1, 'name': 'Bitcoin', 'symbol': 'BTC', 'slug': ...
-```
+```
```

### Comparing `aiocmcapi-0.6.4/aiocmcapi/client.py` & `aiocmcapi-0.6.5/aiocmcapi/client.py`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.6.4/aiocmcapi/currency.py` & `aiocmcapi-0.6.5/aiocmcapi/currency.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,31 +8,41 @@
 
         self.price: float
         self.market_cap: float
 
         self.change_periods: dict
 
         self.data: dict
+        self.meta: dict
+
         self.cmc_id: int = cmc_id
 
-    async def update(self, client: APIClient):
-        json = await client.get(
+    async def update_data(self, client: APIClient):
+        r_json = await client.get(
             endpoint="/v2/cryptocurrency/quotes/latest",
             params={'id': self.cmc_id}
         )
         
-        self.data = json['data'][str(self.cmc_id)]
+        self.data = r_json['data'][str(self.cmc_id)]
         root = self.data['quote']['USD']
 
         self.name = self.data['name']
         self.slug = self.data['slug']
         self.symbol = self.data['symbol']
 
         self.price = root['price']
         self.market_cap = root['market_cap']
 
         self.change_periods = {
             '1h': root['percent_change_1h'],
             '24h': root['percent_change_24h'],
             '7d': root['percent_change_7d'],
             '30d': root['percent_change_30d']
-        }
+        }
+    
+    async def update_meta(self, client: APIClient):
+        r_json = await client.get(
+            endpoint="/v2/cryptocurrency/info",
+            params={'id': self.cmc_id}
+        )
+        
+        self.meta = r_json['data'][str(self.cmc_id)]
```


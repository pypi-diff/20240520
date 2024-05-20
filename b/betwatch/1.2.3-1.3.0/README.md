# Comparing `tmp/betwatch-1.2.3.tar.gz` & `tmp/betwatch-1.3.0.tar.gz`

## Comparing `betwatch-1.2.3.tar` & `betwatch-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 betwatch-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 betwatch-1.2.3/requirements-dev.lock
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 betwatch-1.2.3/requirements.lock
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.2.3/.github/dependabot.yml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-1.2.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/__about__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/__init__.py
--rw-r--r--   0        0        0    11385 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/client.py
--rw-r--r--   0        0        0    31756 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/client_async.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/exceptions.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/types/filters.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/types/markets.py
--rw-r--r--   0        0        0    12404 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.2.3/betwatch/types/updates.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 betwatch-1.2.3/examples/get_race_prices.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 betwatch-1.2.3/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 betwatch-1.2.3/examples/get_races.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 betwatch-1.2.3/examples/get_races_async.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 betwatch-1.2.3/examples/get_races_async_lightweight.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 betwatch-1.2.3/examples/subscriptions.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 betwatch-1.2.3/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.2.3/tests/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 betwatch-1.2.3/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 betwatch-1.2.3/tests/test_get_race.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 betwatch-1.2.3/tests/test_get_race_async.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 betwatch-1.2.3/tests/test_get_races.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 betwatch-1.2.3/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 betwatch-1.2.3/tests/test_subscribe_race_updates.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 betwatch-1.2.3/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.2.3/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.2.3/README.md
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 betwatch-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 betwatch-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 betwatch-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 betwatch-1.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 betwatch-1.3.0/requirements.lock
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/__about__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/__init__.py
+-rw-r--r--   0        0        0    11385 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/client.py
+-rw-r--r--   0        0        0    32194 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/client_async.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/exceptions.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12404 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_races.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_races_async.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_races_async_lightweight.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/subscriptions.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_get_race.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_get_races.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_subscribe_race_updates.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 betwatch-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.3.0/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 betwatch-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 betwatch-1.3.0/PKG-INFO
```

### Comparing `betwatch-1.2.3/.github/workflows/test.yml` & `betwatch-1.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/betwatch/__init__.py` & `betwatch-1.3.0/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/betwatch/client.py` & `betwatch-1.3.0/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/betwatch/client_async.py` & `betwatch-1.3.0/betwatch/client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,30 +48,27 @@
 
 
 class BetwatchAsyncClient:
     def __init__(
         self,
         api_key: Optional[str] = None,
         transport_logging_level: int = logging.WARNING,
-        host="api.betwatch.com",
         request_timeout: int = 60,
     ):
         if not api_key:
             api_key = os.environ.get("BETWATCH_API_KEY")
         if not api_key:
             raise APIKeyNotSetError()
         self.api_key = api_key
 
         self._gql_sub_transport: WebsocketsTransport
         self._gql_transport: HTTPXAsyncTransport
         self._gql_sub_client: Client
         self._gql_client: Client
 
-        self._host = host
-
         self.connect(request_timeout)
 
         self._http_session: Union[
             None, ReconnectingAsyncClientSession, AsyncClientSession
         ] = None
 
         # flag to indicate if we have entered the context manager
@@ -95,24 +92,38 @@
         self._subscriptions_prices: Dict[str, asyncio.Task] = {}
         self._subscriptions_updates: Dict[Tuple[str, str], asyncio.Task] = {}
 
         self._monitor_task: Union[asyncio.Task, None] = None
         self._last_reconnect: float = monotonic()
 
     def connect(self, request_timeout: int):
+        sub_url = "wss://api.betwatch.com/sub"
+        url = "https://api.betwatch.com/query"
+
+        # Check for url environment override
+        env_api_url = os.getenv("BETWATCH_API_URL")
+        env_sub_url = os.getenv("BETWATCH_API_SUB_URL")
+        if env_api_url:
+            logging.info(f"Using API URL override: {env_api_url}")
+            url = env_api_url
+        if env_sub_url:
+            logging.info(f"Using API SUB URL override: {env_sub_url}")
+            sub_url = env_sub_url
+
         self._gql_sub_transport = WebsocketsTransport(
-            url=f"wss://{self._host}/sub",
+            url=sub_url,
             headers={
                 "X-API-KEY": self.api_key,
                 "User-Agent": f"betwatch-sdk-python-{__version__}",
             },
             init_payload={"apiKey": self.api_key},
+            ssl=sub_url.startswith("wss"),
         )
         self._gql_transport = HTTPXAsyncTransport(
-            url=f"https://{self._host}/query",
+            url=url,
             headers={
                 "X-API-KEY": self.api_key,
                 "User-Agent": f"betwatch-sdk-python-{__version__}",
             },
             timeout=request_timeout,
         )
         # Create a GraphQL client using the defined transport
```

### Comparing `betwatch-1.2.3/betwatch/queries.py` & `betwatch-1.3.0/betwatch/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
 def subscription_race_price_updates(projection: RaceProjection) -> DocumentNode:
     return gql(
         """
     subscription PriceUpdates($id: ID!) {
       priceUpdates(id: $id) {
         id
+        selectionId
         bookmaker
         fixedWin {
           price
           lastUpdated
           flucs {
             price
             lastUpdated
@@ -123,14 +124,15 @@
 
 
 SUBSCRIPTION_BETFAIR_UPDATES = gql(
     """
     subscription BetfairUpdates($id: ID!) {
       betfairUpdates(id: $id) {
         id
+        selectionId
         sp
         totalMatched
         marketTotalMatched
         back {
           price
           size
           lastUpdated
```

### Comparing `betwatch-1.2.3/betwatch/types/bookmakers.py` & `betwatch-1.3.0/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/betwatch/types/filters.py` & `betwatch-1.3.0/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/betwatch/types/markets.py` & `betwatch-1.3.0/betwatch/types/markets.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,16 @@
     FIXED_PLACE = "FIXED_PLACE"
 
 
 @dataclass
 class BookmakerMarket:
     id: str
     _bookmaker: Union[Bookmaker, str] = field(metadata={"name": "bookmaker"})
+    selection_id: Optional[str] = field(metadata={"name": "selectionId"}, default=None)
+    # race_id: Optional[str] = field(metadata={"name": "raceId"}, default=None)
     _fixed_win: Union[None, Price, str] = field(
         metadata={"name": "fixedWin"}, default=None
     )
     _fixed_place: Union[None, Price, str] = field(
         metadata={"name": "fixedPlace"}, default=None
     )
 
@@ -145,14 +147,15 @@
 
 @dataclass
 class BetfairMarket:
     id: str
     total_matched: float = field(metadata={"name": "totalMatched"})
     market_total_matched: float = field(metadata={"name": "marketTotalMatched"})
     starting_price: float = field(metadata={"name": "sp"})
+    selection_id: Optional[str] = field(metadata={"name": "selectionId"}, default=None)
 
     back: Optional[List[BetfairTick]] = field(default_factory=list)
     lay: Optional[List[BetfairTick]] = field(default_factory=list)
 
     market_name: Optional[str] = field(metadata={"name": "marketName"}, default=None)
     last_price_traded: Optional[float] = field(
         metadata={"name": "lastPriceTraded"}, default=None
```

### Comparing `betwatch-1.2.3/betwatch/types/race.py` & `betwatch-1.3.0/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/examples/get_race_prices.py` & `betwatch-1.3.0/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/examples/get_race_prices_async.py` & `betwatch-1.3.0/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/examples/get_races.py` & `betwatch-1.3.0/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/examples/get_races_async.py` & `betwatch-1.3.0/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/examples/get_races_async_lightweight.py` & `betwatch-1.3.0/examples/get_races_async_lightweight.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/examples/subscriptions.py` & `betwatch-1.3.0/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/examples/update_rated_prices.py` & `betwatch-1.3.0/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/tests/test_get_race.py` & `betwatch-1.3.0/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/tests/test_get_race_async.py` & `betwatch-1.3.0/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/tests/test_get_races.py` & `betwatch-1.3.0/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/tests/test_get_races_async.py` & `betwatch-1.3.0/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/tests/test_subscribe_race_updates.py` & `betwatch-1.3.0/tests/test_subscribe_race_updates.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/.gitignore` & `betwatch-1.3.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -132,8 +132,10 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 demos/
 scripts/
 .rtx.toml
-playground/
+playground/
+.DS_Store
+.mise.toml
```

### Comparing `betwatch-1.2.3/LICENSE.txt` & `betwatch-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/README.md` & `betwatch-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.2.3/pyproject.toml` & `betwatch-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "betwatch"
-version = "1.2.3"
+version = "1.3.0"
 description = 'A Python package for interacting with the Betwatch.com API'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["betwatch", "betting", "sports", "api", "sdk"]
 authors = [{ name = "Jamie Watts", email = "jamie@betwatch.com" }]
 classifiers = [
@@ -42,18 +42,17 @@
 [tool.rye.scripts]
 test = "pytest"
 
 [tool.hatch.version]
 path = "betwatch/__about__.py"
 
 [tool.ruff]
+exclude = [".rye"]
 # Enable Pyflakes and pycodestyle rules.
-select = ["E", "F", "B"]
-
+lint.select = ["E", "F", "B"]
 # Never enforce `E501` (line length violations).
-ignore = ["E501"]
-
+lint.ignore = ["E501"]
 fix = true
 
 # Ignore `E402` (import violations) in all `__init__.py` files
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "E402"]
```

### Comparing `betwatch-1.2.3/PKG-INFO` & `betwatch-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: betwatch
-Version: 1.2.3
+Version: 1.3.0
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-Expression: MIT
```


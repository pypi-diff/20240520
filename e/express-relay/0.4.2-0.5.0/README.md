# Comparing `tmp/express_relay-0.4.2.tar.gz` & `tmp/express_relay-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express_relay-0.4.2.tar", max compression
+gzip compressed data, was "express_relay-0.5.0.tar", max compression
```

## Comparing `express_relay-0.4.2.tar` & `express_relay-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      949 2024-04-26 12:32:02.467973 express_relay-0.4.2/README.md
--rw-r--r--   0        0        0        0 2024-04-26 12:32:02.467973 express_relay-0.4.2/express_relay/__init__.py
--rw-r--r--   0        0        0    17136 2024-04-26 12:32:02.467973 express_relay-0.4.2/express_relay/client.py
--rw-r--r--   0        0        0     9559 2024-04-26 12:32:02.467973 express_relay-0.4.2/express_relay/express_relay_types.py
--rw-r--r--   0        0        0     5045 2024-04-26 12:32:02.467973 express_relay-0.4.2/express_relay/searcher/examples/simple_searcher.py
--rw-r--r--   0        0        0      612 2024-04-26 12:32:02.471973 express_relay-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 express_relay-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      949 2024-05-20 18:38:26.401841 express_relay-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 18:38:26.401841 express_relay-0.5.0/express_relay/__init__.py
+-rw-r--r--   0        0        0    17136 2024-05-20 18:38:26.401841 express_relay-0.5.0/express_relay/client.py
+-rw-r--r--   0        0        0     9645 2024-05-20 18:38:26.401841 express_relay-0.5.0/express_relay/express_relay_types.py
+-rw-r--r--   0        0        0     5184 2024-05-20 18:38:26.401841 express_relay-0.5.0/express_relay/searcher/examples/simple_searcher.py
+-rw-r--r--   0        0        0      612 2024-05-20 18:38:26.401841 express_relay-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 express_relay-0.5.0/PKG-INFO
```

### Comparing `express_relay-0.4.2/README.md` & `express_relay-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `express_relay-0.4.2/express_relay/client.py` & `express_relay-0.5.0/express_relay/client.py`

 * *Files identical despite different names*

### Comparing `express_relay-0.4.2/express_relay/express_relay_types.py` & `express_relay-0.5.0/express_relay/express_relay_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,49 +98,52 @@
     target_calldata: HexString
     chain_id: str
     target_contract: Address
     permission_key: HexString
 
 
 class BidStatus(Enum):
+    PENDING = "pending"
     SUBMITTED = "submitted"
     LOST = "lost"
-    PENDING = "pending"
-    SIMULATION_FAILED = "simulation_failed"
+    WON = "won"
 
 
 class BidStatusUpdate(BaseModel):
     """
     Attributes:
         id: The ID of the bid.
         bid_status: The current status of the bid.
-        result: The result of the bid: a transaction hash if the status is SUBMITTED or LOST, else None.
-        index: The index of the bid in the submitted transaction; None if the status is not SUBMITTED.
+        result: The result of the bid: a transaction hash if the status is SUBMITTED or WON. The LOST status may have a result.
+        index: The index of the bid in the submitted transaction.
     """
 
     id: UUIDString
     bid_status: BidStatus
     result: Bytes32 | None = Field(default=None)
     index: int | None = Field(default=None)
 
     @model_validator(mode="after")
     def check_result(self):
-        if self.bid_status in [
-            BidStatus("pending"),
-            BidStatus("simulation_failed"),
-        ]:
+        if self.bid_status == BidStatus("pending"):
             assert self.result is None, "result must be None"
+        elif self.bid_status == BidStatus("lost"):
+            pass
         else:
             assert self.result is not None, "result must be a valid 32-byte hash"
         return self
 
     @model_validator(mode="after")
     def check_index(self):
-        if self.bid_status == BidStatus("submitted"):
+        if self.bid_status == BidStatus("submitted") or self.bid_status == BidStatus(
+            "won"
+        ):
             assert self.index is not None, "index must be a valid integer"
+        elif self.bid_status == BidStatus("lost"):
+            pass
         else:
             assert self.index is None, "index must be None"
         return self
 
 
 class OpportunityBid(BaseModel):
     """
```

### Comparing `express_relay-0.4.2/express_relay/searcher/examples/simple_searcher.py` & `express_relay-0.5.0/express_relay/searcher/examples/simple_searcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,22 +71,24 @@
 
         Args:
             bid_status_update: An object representing an update to the status of a bid.
         """
         id = bid_status_update.id
         bid_status = bid_status_update.bid_status
         result = bid_status_update.result
+        index = bid_status_update.index
 
         result_details = ""
-        if bid_status == BidStatus("submitted"):
-            result_details = (
-                f", transaction {result}, index {bid_status_update.index} of multicall"
-            )
+        if bid_status == BidStatus("submitted") or bid_status == BidStatus("won"):
+            result_details = f", transaction {result}, index {index} of multicall"
         elif bid_status == BidStatus("lost"):
-            result_details = f", transaction {result}"
+            if result:
+                result_details = f", transaction {result}"
+            if index:
+                result_details += f", index {index} of multicall"
         logger.error(
             f"Bid status for bid {id}: {bid_status.value.replace('_', ' ')}{result_details}"
         )
 
 
 async def main():
     parser = argparse.ArgumentParser()
```

### Comparing `express_relay-0.4.2/pyproject.toml` & `express_relay-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "express-relay"
-version = "0.4.2"
+version = "0.5.0"
 description = "Utilities for searchers and protocols to interact with the Express Relay protocol."
 authors = ["dourolabs"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `express_relay-0.4.2/PKG-INFO` & `express_relay-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-relay
-Version: 0.4.2
+Version: 0.5.0
 Summary: Utilities for searchers and protocols to interact with the Express Relay protocol.
 License: Proprietary
 Author: dourolabs
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


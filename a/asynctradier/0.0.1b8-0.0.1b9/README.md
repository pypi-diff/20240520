# Comparing `tmp/asynctradier-0.0.1b8.tar.gz` & `tmp/asynctradier-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynctradier-0.0.1b8.tar", max compression
+gzip compressed data, was "asynctradier-0.0.1b9.tar", max compression
```

## Comparing `asynctradier-0.0.1b8.tar` & `asynctradier-0.0.1b9.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/LICENSE
--rw-r--r--   0        0        0     1552 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/README.md
--rw-r--r--   0        0        0       29 2024-01-10 00:31:04.843872 asynctradier-0.0.1b8/asynctradier/__init__.py
--rw-r--r--   0        0        0      903 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/asynctradier/common/__init__.py
--rw-r--r--   0        0        0     3370 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/asynctradier/common/order.py
--rw-r--r--   0        0        0      818 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/asynctradier/common/position.py
--rw-r--r--   0        0        0     1940 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/asynctradier/exceptions/__init__.py
--rw-r--r--   0        0        0    13069 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/asynctradier/tradier.py
--rw-r--r--   0        0        0        0 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/asynctradier/utils/__init__.py
--rw-r--r--   0        0        0     1785 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/asynctradier/utils/common.py
--rw-r--r--   0        0        0     3932 2024-01-10 00:30:19.719717 asynctradier-0.0.1b8/asynctradier/utils/webutils.py
--rw-r--r--   0        0        0      868 2024-01-10 00:31:04.839872 asynctradier-0.0.1b8/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 asynctradier-0.0.1b8/setup.py
--rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 asynctradier-0.0.1b8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-13 15:29:07.774062 asynctradier-0.0.1b9/LICENSE
+-rw-r--r--   0        0        0     2002 2024-01-13 15:29:07.774062 asynctradier-0.0.1b9/README.md
+-rw-r--r--   0        0        0       29 2024-01-13 15:29:48.458988 asynctradier-0.0.1b9/asynctradier/__init__.py
+-rw-r--r--   0        0        0     3161 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/__init__.py
+-rw-r--r--   0        0        0      538 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/expiration.py
+-rw-r--r--   0        0        0     2105 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/option_contract.py
+-rw-r--r--   0        0        0     3851 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/order.py
+-rw-r--r--   0        0        0      818 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/position.py
+-rw-r--r--   0        0        0     6322 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/common/quote.py
+-rw-r--r--   0        0        0     1940 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/exceptions/__init__.py
+-rw-r--r--   0        0        0    21472 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/tradier.py
+-rw-r--r--   0        0        0        0 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/utils/__init__.py
+-rw-r--r--   0        0        0     1785 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/utils/common.py
+-rw-r--r--   0        0        0     3871 2024-01-13 15:29:07.778062 asynctradier-0.0.1b9/asynctradier/utils/webutils.py
+-rw-r--r--   0        0        0      868 2024-01-13 15:29:48.458988 asynctradier-0.0.1b9/pyproject.toml
+-rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 asynctradier-0.0.1b9/setup.py
+-rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 asynctradier-0.0.1b9/PKG-INFO
```

### Comparing `asynctradier-0.0.1b8/LICENSE` & `asynctradier-0.0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `asynctradier-0.0.1b8/asynctradier/common/order.py` & `asynctradier-0.0.1b9/asynctradier/common/order.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,70 @@
 """
 This module defines the Order class, which represents an order in a trading system.
 """
-from asynctradier.common import Duration, OptionOrderSide, OrderClass, OrderType
+from asynctradier.common import Duration, OrderClass, OrderSide, OrderStatus, OrderType
 
 
 class Order:
     """
     Represent an Order object.
 
     Args:
         **kwargs: Additional keyword arguments representing the order attributes.
 
     Attributes:
         id (int): The ID of the order.
         type (OrderType): The type of the order.
         symbol (str): The symbol of the order.
-        side (OptionOrderSide): The side of the order.
+        side (OrderSide): The side of the order.
         quantity (float): The quantity of the order.
         status (str): The status of the order.
         duration (Duration): The duration of the order.
         avg_fill_price (float): The average fill price of the order.
         exec_quantity (float): The executed quantity of the order.
         last_fill_price (float): The last fill price of the order.
         last_fill_quantity (float): The last fill quantity of the order.
         remaining_quantity (float): The remaining quantity of the order.
         create_date (str): The creation date of the order.
         transaction_date (str): The transaction date of the order.
         class_ (OrderClass): The class of the order.
         option_symbol (str): The option symbol of the order.
+        price (float): The price of the order.
+        number_of_legs (int): The number of legs of the order.
+        legs (list[Order]): The legs of the order.
     """
 
     def __init__(
         self,
         **kwargs,
     ) -> None:
         assert kwargs.get("id", None) is not None
         self.id = kwargs["id"]
         self.type = OrderType(kwargs["type"]) if kwargs.get("type", None) else None
         self.symbol = kwargs.get("symbol", None)
-        self.side = (
-            OptionOrderSide(kwargs["side"]) if kwargs.get("side", None) else None
-        )
+        self.side = OrderSide(kwargs["side"]) if kwargs.get("side", None) else None
         self.quantity = kwargs.get("quantity", None)
-        self.status = kwargs.get("status", None)
+        self.status = (
+            OrderStatus(kwargs["status"]) if kwargs.get("status", None) else None
+        )
         self.duration = (
             Duration(kwargs["duration"]) if kwargs.get("duration", None) else None
         )
         self.avg_fill_price = kwargs.get("avg_fill_price", None)
         self.exec_quantity = kwargs.get("exec_quantity", None)
         self.last_fill_price = kwargs.get("last_fill_price", None)
         self.last_fill_quantity = kwargs.get("last_fill_quantity", None)
         self.remaining_quantity = kwargs.get("remaining_quantity", None)
         self.create_date = kwargs.get("create_date", None)
         self.transaction_date = kwargs.get("transaction_date", None)
         self.class_ = OrderClass(kwargs["class"]) if kwargs.get("class", None) else None
         self.option_symbol = kwargs.get("option_symbol", None)
+        self.price = kwargs.get("price", None)
+        self.number_of_legs = kwargs.get("num_legs", None)
+        self.legs = [Order(**leg) for leg in kwargs.get("leg", [])]
 
     def __str__(self) -> str:
         """
         Return a string representation of the Order object.
 
         Returns:
             str: A string representation of the Order object.
@@ -67,10 +73,12 @@
             f"Order(id={self.id}, type={self.type}, symbol={self.symbol}, "
             f"side={self.side}, quantity={self.quantity}, status={self.status}, "
             f"duration={self.duration}, avg_fill_price={self.avg_fill_price}, "
             f"exec_quantity={self.exec_quantity}, last_fill_price={self.last_fill_price}, "
             f"last_fill_quantity={self.last_fill_quantity}, "
             f"remaining_quantity={self.remaining_quantity}, "
             f"create_date={self.create_date}, "
-            f"transaction_date={self.transaction_date}, class={self.class_}, "
-            f"option_symbol={self.option_symbol})"
+            f"transaction_date={self.transaction_date}, "
+            f"class={self.class_}, option_symbol={self.option_symbol}, "
+            f"price={self.price}, number_of_legs={self.number_of_legs}, "
+            f"legs={self.legs})"
         )
```

### Comparing `asynctradier-0.0.1b8/asynctradier/common/position.py` & `asynctradier-0.0.1b9/asynctradier/common/position.py`

 * *Files identical despite different names*

### Comparing `asynctradier-0.0.1b8/asynctradier/exceptions/__init__.py` & `asynctradier-0.0.1b9/asynctradier/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `asynctradier-0.0.1b8/asynctradier/utils/common.py` & `asynctradier-0.0.1b9/asynctradier/utils/common.py`

 * *Files identical despite different names*

### Comparing `asynctradier-0.0.1b8/asynctradier/utils/webutils.py` & `asynctradier-0.0.1b9/asynctradier/utils/webutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,15 @@
                 method, url, params=params, headers=headers, data=data
             ) as resp:
                 if resp.status != 200:
                     raise BadRequestException(resp.status, await resp.text())
                 response = await resp.json()
 
                 if "errors" in response:
-                    raise BadRequestException(
-                        400, response["errors"]["error"]["description"]
-                    )
+                    raise BadRequestException(400, response["errors"]["error"])
                 return response
 
     async def get(self, path: str, params: dict = None):
         """
         Makes an asynchronous GET request.
 
         Args:
```

### Comparing `asynctradier-0.0.1b8/pyproject.toml` & `asynctradier-0.0.1b9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Jiakuan Li <jiakuan.li.cs@gmail.com>"]
 description = "Async api wrapper for [Tradier](https://documentation.tradier.com/)."
 name = "asynctradier"
 packages = [{include = "asynctradier"}]
 readme = "README.md"
-version = "0.0.1-beta.8"
+version = "0.0.1-beta.9"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.9.1"
 python = "^3.9"
 strenum = "^0.4.15"
 websockets = "^12.0"
```


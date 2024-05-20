# Comparing `tmp/fastmqtt-0.1.4.tar.gz` & `tmp/fastmqtt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmqtt-0.1.4.tar", max compression
+gzip compressed data, was "fastmqtt-0.1.5.tar", max compression
```

## Comparing `fastmqtt-0.1.4.tar` & `fastmqtt-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/LICENSE
--rw-r--r--   0        0        0     1812 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/README.md
--rw-r--r--   0        0        0      306 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/__init__.py
--rw-r--r--   0        0        0       41 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/exceptions.py
--rw-r--r--   0        0        0     5200 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/fastmqtt.py
--rw-r--r--   0        0        0     3437 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/message_handler.py
--rw-r--r--   0        0        0     3749 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/response.py
--rw-r--r--   0        0        0     2931 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/router.py
--rw-r--r--   0        0        0     1178 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/structures.py
--rw-r--r--   0        0        0     2434 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/subscription_manager.py
--rw-r--r--   0        0        0      641 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/fastmqtt/utils.py
--rw-r--r--   0        0        0      856 2024-03-26 08:28:43.160881 fastmqtt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 fastmqtt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-20 11:17:23.504988 fastmqtt-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1812 2024-05-20 11:17:23.504988 fastmqtt-0.1.5/README.md
+-rw-r--r--   0        0        0      306 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/__init__.py
+-rw-r--r--   0        0        0       41 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/exceptions.py
+-rw-r--r--   0        0        0     5320 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/fastmqtt.py
+-rw-r--r--   0        0        0     3437 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/message_handler.py
+-rw-r--r--   0        0        0     3749 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/response.py
+-rw-r--r--   0        0        0     2931 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/router.py
+-rw-r--r--   0        0        0     1178 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/structures.py
+-rw-r--r--   0        0        0     2434 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/subscription_manager.py
+-rw-r--r--   0        0        0      641 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/fastmqtt/utils.py
+-rw-r--r--   0        0        0      857 2024-05-20 11:17:23.508988 fastmqtt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2430 1970-01-01 00:00:00.000000 fastmqtt-0.1.5/PKG-INFO
```

### Comparing `fastmqtt-0.1.4/LICENSE` & `fastmqtt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmqtt-0.1.4/README.md` & `fastmqtt-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fastmqtt-0.1.4/fastmqtt/fastmqtt.py` & `fastmqtt-0.1.5/fastmqtt/fastmqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import asyncio
 import logging
 import ssl
-from typing import Any, Callable, Iterable, Sequence
+from typing import Any, Callable, Iterable, Literal, Sequence
 
-import paho.mqtt.client as mqtt
 from aiomqtt import Client as MQTTClient
 from aiomqtt import (
     Message,
     ProtocolVersion,
     ProxySettings,
     TLSParameters,
     Will,
 )
 from aiomqtt.types import PayloadType, SocketOption
+from paho.mqtt import client as mqtt
+from paho.mqtt import properties as mqtt_properties
 from paho.mqtt.packettypes import PacketTypes
 
 from .message_handler import MessageHandler
 from .response import ResponseContext
 from .router import MQTTRouter
 from .subscription_manager import Subscription, SubscriptionManager
 from .utils import properties_from_dict
@@ -33,25 +34,25 @@
         username: str | None = None,
         password: str | None = None,
         logger: logging.Logger | None = None,
         identifier: str | None = None,
         queue_type: type[asyncio.Queue[Message]] | None = None,
         will: Will | None = None,
         clean_session: bool | None = None,
-        transport: str = "tcp",
+        transport: Literal["tcp", "websockets"] = "tcp",
         timeout: float | None = None,
         keepalive: int = 60,
         bind_address: str = "",
         bind_port: int = 0,
-        clean_start: int = mqtt.MQTT_CLEAN_START_FIRST_ONLY,
+        clean_start: mqtt.CleanStartOption = mqtt.MQTT_CLEAN_START_FIRST_ONLY,
         max_queued_incoming_messages: int | None = None,
         max_queued_outgoing_messages: int | None = None,
         max_inflight_messages: int | None = None,
         max_concurrent_outgoing_calls: int | None = None,
-        properties: mqtt.Properties | None = None,
+        properties: mqtt_properties.Properties | None = None,
         tls_context: ssl.SSLContext | None = None,
         tls_params: TLSParameters | None = None,
         tls_insecure: bool | None = None,
         proxy: ProxySettings | None = None,
         socket_options: Iterable[SocketOption] | None = None,
         websocket_path: str | None = None,
         websocket_headers: WebSocketHeaders | None = None,
```

### Comparing `fastmqtt-0.1.4/fastmqtt/message_handler.py` & `fastmqtt-0.1.5/fastmqtt/message_handler.py`

 * *Files identical despite different names*

### Comparing `fastmqtt-0.1.4/fastmqtt/response.py` & `fastmqtt-0.1.5/fastmqtt/response.py`

 * *Files identical despite different names*

### Comparing `fastmqtt-0.1.4/fastmqtt/router.py` & `fastmqtt-0.1.5/fastmqtt/router.py`

 * *Files identical despite different names*

### Comparing `fastmqtt-0.1.4/fastmqtt/structures.py` & `fastmqtt-0.1.5/fastmqtt/structures.py`

 * *Files identical despite different names*

### Comparing `fastmqtt-0.1.4/fastmqtt/subscription_manager.py` & `fastmqtt-0.1.5/fastmqtt/subscription_manager.py`

 * *Files identical despite different names*

### Comparing `fastmqtt-0.1.4/fastmqtt/utils.py` & `fastmqtt-0.1.5/fastmqtt/utils.py`

 * *Files identical despite different names*

### Comparing `fastmqtt-0.1.4/pyproject.toml` & `fastmqtt-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "fastmqtt"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["toxazhl <zhltoxa@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/toxazhl/fastmqtt"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-aiomqtt = "2.0.1"
+python = "^3.9"
+aiomqtt = "^2.1.0"
+libcst = "^1.3.1"
 
 [tool.poetry.dev-dependencies]
-libcst = "^1.1.0"
-black = "^23.12.1"
-ruff = "^0.1.14"
+libcst = "*"
+black = "*"
+ruff = "*"
 
 [tool.black]
-line_length = 99
+line-length = 99
 exclude = "\\.?venv|\\.?tests|\\.cache"
 
 
 [tool.ruff]
 target-version = "py38"
 line-length = 99
 select = [
```

### Comparing `fastmqtt-0.1.4/PKG-INFO` & `fastmqtt-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fastmqtt
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/toxazhl/fastmqtt
 Author: toxazhl
 Author-email: zhltoxa@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiomqtt (==2.0.1)
+Requires-Dist: aiomqtt (>=2.1.0,<3.0.0)
+Requires-Dist: libcst (>=1.3.1,<2.0.0)
 Project-URL: Repository, https://github.com/toxazhl/fastmqtt
 Description-Content-Type: text/markdown
 
 # FastMQTT
 
 A performant, flexible, and user-friendly MQTT client library built on top of aiomqtt. FastMQTT simplifies message handling, advanced subscriptions, and convenient request-response patterns within the MQTT protocol.
```


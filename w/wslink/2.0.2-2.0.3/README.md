# Comparing `tmp/wslink-2.0.2.tar.gz` & `tmp/wslink-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wslink-2.0.2.tar", last modified: Thu Apr 18 23:22:34 2024, max compression
+gzip compressed data, was "wslink-2.0.3.tar", last modified: Mon May 20 14:36:46 2024, max compression
```

## Comparing `wslink-2.0.2.tar` & `wslink-2.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.727270 wslink-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 23:22:03.000000 wslink-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-18 23:22:34.727270 wslink-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-18 23:22:03.000000 wslink-2.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 23:22:34.727270 wslink-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-18 23:22:03.000000 wslink-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.719271 wslink-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.723271 wslink-2.0.2/src/wslink/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.723271 wslink-2.0.2/src/wslink/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.723271 wslink-2.0.2/src/wslink/backends/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/aiohttp/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/aiohttp/relay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.723271 wslink-2.0.2/src/wslink/backends/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/generic/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.727270 wslink-2.0.2/src/wslink/backends/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/jupyter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.727270 wslink-2.0.2/src/wslink/backends/tornado/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/backends/tornado/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/chunking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21170 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/ssl_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-18 23:22:03.000000 wslink-2.0.2/src/wslink/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:34.727270 wslink-2.0.2/src/wslink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 23:22:34.000000 wslink-2.0.2/src/wslink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.574564 wslink-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 14:36:19.000000 wslink-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-20 14:36:46.574564 wslink-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-20 14:36:19.000000 wslink-2.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 14:36:46.574564 wslink-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-20 14:36:19.000000 wslink-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.566563 wslink-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.570563 wslink-2.0.3/src/wslink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.570563 wslink-2.0.3/src/wslink/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.570563 wslink-2.0.3/src/wslink/backends/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/aiohttp/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/aiohttp/relay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.570563 wslink-2.0.3/src/wslink/backends/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/generic/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.570563 wslink-2.0.3/src/wslink/backends/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/jupyter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.574564 wslink-2.0.3/src/wslink/backends/tornado/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/backends/tornado/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/chunking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21170 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/ssl_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-20 14:36:19.000000 wslink-2.0.3/src/wslink/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:46.574564 wslink-2.0.3/src/wslink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-20 14:36:46.000000 wslink-2.0.3/src/wslink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-20 14:36:46.000000 wslink-2.0.3/src/wslink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:36:46.000000 wslink-2.0.3/src/wslink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 14:36:46.000000 wslink-2.0.3/src/wslink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 14:36:46.000000 wslink-2.0.3/src/wslink.egg-info/top_level.txt
```

### Comparing `wslink-2.0.2/PKG-INFO` & `wslink-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wslink-2.0.2/README.rst` & `wslink-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/setup.py` & `wslink-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/LICENSE` & `wslink-2.0.3/src/wslink/LICENSE`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/__init__.py` & `wslink-2.0.3/src/wslink/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/backends/__init__.py` & `wslink-2.0.3/src/wslink/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/backends/aiohttp/__init__.py` & `wslink-2.0.3/src/wslink/backends/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/backends/aiohttp/launcher.py` & `wslink-2.0.3/src/wslink/backends/aiohttp/launcher.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/backends/aiohttp/relay.py` & `wslink-2.0.3/src/wslink/backends/aiohttp/relay.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/backends/generic/core.py` & `wslink-2.0.3/src/wslink/backends/generic/core.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/backends/jupyter/core.py` & `wslink-2.0.3/src/wslink/backends/jupyter/core.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/backends/tornado/core.py` & `wslink-2.0.3/src/wslink/backends/tornado/core.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/chunking.py` & `wslink-2.0.3/src/wslink/chunking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import sys
 import secrets
 import msgpack
 from typing import Dict, Tuple, Union
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict  # pylint: disable=no-name-in-module
@@ -83,15 +84,15 @@
 # Chunks across messages can be interleaved.
 class UnChunker:
     pending_messages: Dict[bytes, PendingMessage]
     max_message_size: int
 
     def __init__(self):
         self.pending_messages = {}
-        self.max_message_size = 512
+        self.max_message_size = int(os.environ.get("WSLINK_AUTH_MSG_SIZE", 512))
 
     def set_max_message_size(self, size):
         self.max_message_size = size
 
     def release_pending_messages(self):
         self.pending_messages = {}
```

### Comparing `wslink-2.0.2/src/wslink/launcher.py` & `wslink-2.0.3/src/wslink/launcher.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/protocol.py` & `wslink-2.0.3/src/wslink/protocol.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/publish.py` & `wslink-2.0.3/src/wslink/publish.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/server.py` & `wslink-2.0.3/src/wslink/server.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/ssl_context.py` & `wslink-2.0.3/src/wslink/ssl_context.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink/websocket.py` & `wslink-2.0.3/src/wslink/websocket.py`

 * *Files identical despite different names*

### Comparing `wslink-2.0.2/src/wslink.egg-info/PKG-INFO` & `wslink-2.0.3/src/wslink.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wslink-2.0.2/src/wslink.egg-info/SOURCES.txt` & `wslink-2.0.3/src/wslink.egg-info/SOURCES.txt`

 * *Files identical despite different names*


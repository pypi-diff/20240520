# Comparing `tmp/era_5g_server-0.4.0.tar.gz` & `tmp/era_5g_server-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_server-0.4.0.tar", last modified: Tue Feb 27 13:14:36 2024, max compression
+gzip compressed data, was "era_5g_server-0.5.0.tar", last modified: Mon May 20 10:51:23 2024, max compression
```

## Comparing `era_5g_server-0.4.0.tar` & `era_5g_server-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-02-27 13:14:36.796320 era_5g_server-0.4.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-02-27 13:14:35.000000 era_5g_server-0.4.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-02-27 13:14:36.796320 era_5g_server-0.4.0/PKG-INFO
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-02-27 13:14:35.000000 era_5g_server-0.4.0/backend_shim.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-02-27 13:14:36.792320 era_5g_server-0.4.0/era_5g_server/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-02-27 13:14:35.000000 era_5g_server-0.4.0/era_5g_server/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-02-27 13:14:35.000000 era_5g_server-0.4.0/era_5g_server/py.typed
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14324 2024-02-27 13:14:35.000000 era_5g_server-0.4.0/era_5g_server/server.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-02-27 13:14:36.792320 era_5g_server-0.4.0/era_5g_server.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-02-27 13:14:36.000000 era_5g_server-0.4.0/era_5g_server.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      339 2024-02-27 13:14:36.000000 era_5g_server-0.4.0/era_5g_server.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-02-27 13:14:36.000000 era_5g_server-0.4.0/era_5g_server.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-02-27 13:14:36.000000 era_5g_server-0.4.0/era_5g_server.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      119 2024-02-27 13:14:36.000000 era_5g_server-0.4.0/era_5g_server.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       14 2024-02-27 13:14:36.000000 era_5g_server-0.4.0/era_5g_server.egg-info/top_level.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-02-27 13:14:36.796320 era_5g_server-0.4.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1014 2024-02-27 13:14:35.000000 era_5g_server-0.4.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:51:23.363062 era_5g_server-0.5.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-05-20 10:51:22.000000 era_5g_server-0.5.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-05-20 10:51:23.363062 era_5g_server-0.5.0/PKG-INFO
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-05-20 10:51:22.000000 era_5g_server-0.5.0/backend_shim.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:51:23.359062 era_5g_server-0.5.0/era_5g_server/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:51:22.000000 era_5g_server-0.5.0/era_5g_server/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:51:22.000000 era_5g_server-0.5.0/era_5g_server/py.typed
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14681 2024-05-20 10:51:22.000000 era_5g_server-0.5.0/era_5g_server/server.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:51:23.359062 era_5g_server-0.5.0/era_5g_server.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-05-20 10:51:23.000000 era_5g_server-0.5.0/era_5g_server.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      339 2024-05-20 10:51:23.000000 era_5g_server-0.5.0/era_5g_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-05-20 10:51:23.000000 era_5g_server-0.5.0/era_5g_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-05-20 10:51:23.000000 era_5g_server-0.5.0/era_5g_server.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      119 2024-05-20 10:51:23.000000 era_5g_server-0.5.0/era_5g_server.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       14 2024-05-20 10:51:23.000000 era_5g_server-0.5.0/era_5g_server.egg-info/top_level.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-05-20 10:51:23.363062 era_5g_server-0.5.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1014 2024-05-20 10:51:22.000000 era_5g_server-0.5.0/setup.py
```

### Comparing `era_5g_server-0.4.0/backend_shim.py` & `era_5g_server-0.5.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_server-0.4.0/era_5g_server/server.py` & `era_5g_server-0.5.0/era_5g_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import math
 import os
 from multiprocessing import Process
 from typing import Any, Callable, Dict, Optional, Tuple
+from urllib.parse import urljoin
 
 import socketio
 import ujson
 from engineio.payload import Payload
 from flask import Flask
 
 from era_5g_interface.channels import COMMAND_ERROR_EVENT, CONTROL_NAMESPACE, DATA_NAMESPACE, CallbackInfoServer
@@ -25,17 +26,18 @@
 NETAPP_ID_ROS = NETAPP_ID.replace("-", "_")
 
 NETAPP_NAME = str(os.getenv("NETAPP_NAME", "Unknown"))
 
 # Used for Network Application heartbeat.
 MAX_LATENCY = float(os.getenv("NETAPP_MAX_LATENCY", 100))
 
-NETAPP_STATUS_ADDRESS = (
-    MIDDLEWARE_ADDRESS if MIDDLEWARE_ADDRESS.endswith("/status/netapp") else MIDDLEWARE_ADDRESS + "/status/netapp"
-)
+if MIDDLEWARE_ADDRESS.endswith("/status/netapp"):
+    NETAPP_STATUS_ADDRESS = MIDDLEWARE_ADDRESS
+else:
+    NETAPP_STATUS_ADDRESS = urljoin(MIDDLEWARE_ADDRESS, "status/netapp")
 
 
 def generate_application_heartbeat_data(
     avg_latency: float,
     queue_size: int,
     queue_occupancy: float,
     current_robot_count: int,
@@ -121,14 +123,15 @@
             *args: Process arguments.
             command_callback (Callable[[ControlCommand, str], None], optional): On control command callback.
             disconnect_callback (Callable[[str], None], optional): On data namespace disconnect callback.
             back_pressure_size (int, optional): Back pressure size - max size of eio.sockets[eio_sid].queue.qsize().
             recreate_coder_attempts_count (int): How many times try to recreate the frame encoder/decoder.
             disconnect_on_unhandled (bool): Whether to call self._sio.disconnect(...) if unhandled exception occurs.
             stats (bool): Store output data sizes.
+            extended_measuring (bool): Enable logging of measuring.
             host (str): The IP address of the interface, where the websocket server should run. Defaults to "0.0.0.0".
             async_handlers (bool): Specify, if the incoming messages. Defaults to False.
             max_message_size (float): The maximum size of the message to be passed in MB. Defaults to 5.
             **kwargs: Process arguments.
         """
 
         super().__init__(*args, **kwargs)
@@ -256,14 +259,23 @@
 
         Returns:
             Client eio sid of CONTROL_NAMESPACE.
         """
 
         return self._channels.get_client_eio_sid(sid, CONTROL_NAMESPACE)
 
+    def disconnect(self, sid: str) -> None:
+        """Disconnects the client from DATA_NAMESPACE by sid.
+
+        Args:
+            sid (str): Namespace sid.
+        """
+
+        self._sio.disconnect(sid, DATA_NAMESPACE)
+
     def send_command_error(self, message: str, sid: str):
         """Send control command error message to client.
 
         Args:
             message (str): Error message.
             sid (str): Namespace sid.
         """
```

### Comparing `era_5g_server-0.4.0/setup.py` & `era_5g_server-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_server',
     ),
     'python_requires': '>=3.8',
-    'version': '0.4.0',
+    'version': '0.5.0',
 })
```


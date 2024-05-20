# Comparing `tmp/era_5g_client-1.0.0.tar.gz` & `tmp/era_5g_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_client-1.0.0.tar", last modified: Mon Apr 29 08:03:41 2024, max compression
+gzip compressed data, was "era_5g_client-1.1.0.tar", last modified: Mon May 20 10:29:44 2024, max compression
```

## Comparing `era_5g_client-1.0.0.tar` & `era_5g_client-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:41.008369 era_5g_client-1.0.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-04-29 08:03:41.008369 era_5g_client-1.0.0/PKG-INFO
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/backend_shim.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:41.004369 era_5g_client-1.0.0/era_5g_client/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14764 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/client.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    13441 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/client_base.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      559 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/dataclasses.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      784 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/exceptions.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3748 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/middleware_resource_checker.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/py.typed
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:41.004369 era_5g_client-1.0.0/era_5g_client.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      470 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      134 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       14 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/top_level.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-29 08:03:41.008369 era_5g_client-1.0.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1029 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:29:44.834467 era_5g_client-1.1.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-05-20 10:29:44.834467 era_5g_client-1.1.0/PKG-INFO
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/backend_shim.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:29:44.830467 era_5g_client-1.1.0/era_5g_client/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/era_5g_client/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14995 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/era_5g_client/client.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14251 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/era_5g_client/client_base.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      559 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/era_5g_client/dataclasses.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      784 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/era_5g_client/exceptions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3748 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/era_5g_client/middleware_resource_checker.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/era_5g_client/py.typed
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-20 10:29:44.834467 era_5g_client-1.1.0/era_5g_client.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-05-20 10:29:44.000000 era_5g_client-1.1.0/era_5g_client.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      470 2024-05-20 10:29:44.000000 era_5g_client-1.1.0/era_5g_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-05-20 10:29:44.000000 era_5g_client-1.1.0/era_5g_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-05-20 10:29:44.000000 era_5g_client-1.1.0/era_5g_client.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      134 2024-05-20 10:29:44.000000 era_5g_client-1.1.0/era_5g_client.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       14 2024-05-20 10:29:44.000000 era_5g_client-1.1.0/era_5g_client.egg-info/top_level.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-05-20 10:29:44.834467 era_5g_client-1.1.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1029 2024-05-20 10:29:43.000000 era_5g_client-1.1.0/setup.py
```

### Comparing `era_5g_client-1.0.0/backend_shim.py` & `era_5g_client-1.1.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-1.0.0/era_5g_client/client.py` & `era_5g_client-1.1.0/era_5g_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,38 +157,41 @@
 
     def register(
         self,
         netapp_address: str,
         args: Optional[Dict[str, Any]] = None,
         wait_until_available: bool = False,
         wait_timeout: int = -1,
+        wait_until_initialized: bool = True,
     ) -> None:
         """Wait for ready Middleware resources and connects to the 5G-ERA Network Application server DATA_NAMESPACE and
         CONTROL_NAMESPACE.
 
         Args:
             netapp_address (str): The URL of the network application interface, including the scheme and optionally
                 port and path to the interface, e.g. http://localhost:80 or http://gateway/path_to_interface.
             args (Dict[str, Any], optional): 5G-ERA Network Application specific arguments. Defaults to None.
             wait_until_available: If True, the client will repeatedly try to register with the Network Application
                 until it is available. Defaults to False.
             wait_timeout: How long the client will try to connect to network application. Only used if
                 wait_until_available is True. If negative, the client will wait indefinitely. Defaults to -1.
+            wait_until_initialized (bool): If True, the client will repeatedly wait for the Network Application
+                initialization. Defaults to True.
 
         Raises:
             NetAppNotReady: Raised when register called before the 5G-ERA Network Application is ready.
         """
 
         if not self.resource_checker:
             raise NetAppNotReady("Not connected to the Middleware.")
 
         if not self.resource_checker.is_ready():
             raise NetAppNotReady("Not ready.")
         self.args = args
-        super().register(netapp_address, args, wait_until_available, wait_timeout)
+        super().register(netapp_address, args, wait_until_available, wait_timeout, wait_until_initialized)
 
     @property
     def switching(self) -> bool:
         """Specify if the client is in the process of the edge switchover (reconnecting from one server to another)."""
         return self._switching
 
     def netapp_address_changed(self):
```

### Comparing `era_5g_client-1.0.0/era_5g_client/client_base.py` & `era_5g_client-1.1.0/era_5g_client/client_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 from collections.abc import Callable
 from dataclasses import asdict
 from typing import Any, Dict, Optional, Tuple, Union
 
 import socketio
 import ujson
+from requests import JSONDecodeError
 from socketio.exceptions import ConnectionError
 
 from era_5g_client.exceptions import FailedToConnect
 from era_5g_interface.channels import (
     COMMAND_ERROR_EVENT,
     COMMAND_EVENT,
     COMMAND_RESULT_EVENT,
@@ -119,67 +120,78 @@
         # Substitute send function calls.
         self.send_image = self._channels.send_image
         self.send_data = self._channels.send_data
 
         # Args for registration.
         self._args: Optional[Dict[str, Any]] = None
 
+        self._initialized = False  # Initialization flag.
+
     def register(
         self,
         netapp_address: str,
         args: Optional[Dict[str, Any]] = None,
         wait_until_available: bool = False,
         wait_timeout: int = -1,
+        wait_until_initialized: bool = True,
     ) -> None:
         """Connects to the 5G-ERA Network Application server DATA_NAMESPACE and CONTROL_NAMESPACE.
 
         Args:
             netapp_address (str): The URL of the 5G-ERA Network Application server, including the scheme and optionally
                 port and path to the interface, e.g. http://localhost:80 or http://gateway/path_to_interface.
             args (Dict, optional): Optional parameters to be passed to the 5G-ERA Network Application, in the form of
                 dict. Defaults to None.
-            wait_until_available: If True, the client will repeatedly try to register with the Network Application
+            wait_until_available (bool): If True, the client will repeatedly try to register with the Network Application
                 until it is available. Defaults to False.
-            wait_timeout: How long the client will try to connect to network application. Only used if
+            wait_timeout (int): How long the client will try to connect to Network Application. Only used if
                 wait_until_available is True. If negative, the client will wait indefinitely. Defaults to -1.
+            wait_until_initialized (bool): If True, the client will repeatedly wait for the Network Application
+                initialization. Defaults to True.
 
         Raises:
-            FailedToConnect: Failed to connect to network application exception.
+            FailedToConnect: Failed to connect to Network Application exception.
 
         Returns:
             Response: response from the 5G-ERA Network Application.
         """
 
         # Store args for repeat registration.
         self._args = args
         # Connect to server
         self.netapp_address = netapp_address
         namespaces_to_connect = [DATA_NAMESPACE, CONTROL_NAMESPACE]
         start_time = time.time()
         while True:
             try:
-                self.logger.info(f"Trying to connect to the network application: {netapp_address}")
+                self.logger.info(f"Trying to connect to the Network Application: {netapp_address}")
                 self._sio.connect(
                     netapp_address,
                     namespaces=namespaces_to_connect,
                     wait_timeout=10,
                 )
                 break
-            except ConnectionError as ex:
+            except (ConnectionError, JSONDecodeError) as ex:
                 self.logger.debug(f"Failed to connect: {repr(ex)}")
                 if not wait_until_available or (wait_timeout > 0 and start_time + wait_timeout < time.time()):
                     raise FailedToConnect(ex)
-                self.logger.warning("Failed to connect to network application. Retrying in 1 second.")
+                self.logger.warning("Failed to connect to Network Application. Retrying in 1 second.")
                 time.sleep(1)
 
         self.logger.info(f"Client connected to namespaces: {namespaces_to_connect}")
 
+        if wait_until_initialized:
+            while not self._initialized:
+                self.logger.warning("Waiting for successful initialization by INIT command. Retrying in 1 second.")
+                time.sleep(1)
+
     def disconnect(self) -> None:
         """Disconnects the WebSocket connection."""
 
+        self._initialized = False
         if self._sio.connected:
             self._sio.disconnect()
 
     def print_stats(self):
         """Print stats info - transferred bytes."""
 
         if self._channels.stats:
@@ -193,14 +205,23 @@
                 )
 
     def wait(self) -> None:
         """Blocking infinite waiting."""
 
         self._sio.wait()
 
+    @property
+    def initialized(self) -> bool:
+        """Is the Network Application initialized by ControlCmdType.INIT?
+
+        Returns: True if Network Application was initialized, False otherwise.
+        """
+
+        return self._initialized
+
     def data_connect_callback(self) -> None:
         """The callback called once the connection to the 5G-ERA Network Application DATA_NAMESPACE is made."""
 
         self.logger.info(
             f"Connected to server {DATA_NAMESPACE}, eio_sid" f" {self._channels.get_client_eio_sid(DATA_NAMESPACE)}"
         )
 
@@ -208,24 +229,25 @@
         """The callback called once the connection to the 5G-ERA Network Application CONTROL_NAMESPACE is made."""
 
         self.logger.info(
             f"Connected to server {CONTROL_NAMESPACE}, eio_sid "
             f"{self._channels.get_client_eio_sid(CONTROL_NAMESPACE)}"
         )
 
-        # Initialize the network application with desired parameters using the init command.
+        self._initialized = False
+        # Initialize the Network Application with desired parameters using the init command.
         control_command = ControlCommand(ControlCmdType.INIT, clear_queue=False, data=self._args)
-        self.logger.info(f"Initialize the network application using the init command {control_command}")
+        self.logger.info(f"Initialize the Network Application using the INIT command {control_command}")
         initialized, message = self.send_control_command(control_command)
         if not initialized:
             self.disconnect()
-            self.logger.error(f"Failed to initialize the network application: {message}")
+            self.logger.error(f"Failed to initialize the Network Application: {message}")
             logging.shutdown()  # should flush the logger
             os._exit(1)
-            # raise FailedToInitialize(f"Failed to initialize the network application: {message}")
+        self._initialized = True
 
     def data_disconnect_callback(self) -> None:
         """The callback called once the connection to the 5G-ERA Network Application DATA_NAMESPACE is lost."""
 
         self.logger.info(
             f"Disconnected from server {DATA_NAMESPACE}, eio_sid "
             f"{self._channels.get_client_eio_sid(DATA_NAMESPACE)}"
```

### Comparing `era_5g_client-1.0.0/era_5g_client/dataclasses.py` & `era_5g_client-1.1.0/era_5g_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-1.0.0/era_5g_client/exceptions.py` & `era_5g_client-1.1.0/era_5g_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-1.0.0/era_5g_client/middleware_resource_checker.py` & `era_5g_client-1.1.0/era_5g_client/middleware_resource_checker.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-1.0.0/setup.py` & `era_5g_client-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_client',
     ),
     'python_requires': '>=3.8',
-    'version': '1.0.0',
+    'version': '1.1.0',
 })
```


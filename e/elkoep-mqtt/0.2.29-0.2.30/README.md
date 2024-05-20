# Comparing `tmp/elkoep_mqtt-0.2.29.tar.gz` & `tmp/elkoep_mqtt-0.2.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkoep_mqtt-0.2.29.tar", last modified: Tue May  7 14:28:07 2024, max compression
+gzip compressed data, was "elkoep_mqtt-0.2.30.tar", last modified: Mon May 20 10:56:22 2024, max compression
```

## Comparing `elkoep_mqtt-0.2.29.tar` & `elkoep_mqtt-0.2.30.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:28:07.000000 elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/inelsmqtt/
--rw-r--r--   0 runner    (1001) docker     (127)    18542 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22709 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/inelsmqtt/devices/
--rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/devices/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   105922 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/inelsmqtt/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:07.728944 elkoep_mqtt-0.2.29/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/devices/device_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/discovery_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/inels_mqtt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-07 14:27:54.000000 elkoep_mqtt-0.2.29/tests/online_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:56:22.497289 elkoep_mqtt-0.2.30/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-20 10:56:22.497289 elkoep_mqtt-0.2.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:56:22.497289 elkoep_mqtt-0.2.30/elkoep_mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-20 10:56:22.000000 elkoep_mqtt-0.2.30/elkoep_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-20 10:56:22.000000 elkoep_mqtt-0.2.30/elkoep_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:56:22.000000 elkoep_mqtt-0.2.30/elkoep_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:56:22.000000 elkoep_mqtt-0.2.30/elkoep_mqtt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 10:56:22.000000 elkoep_mqtt-0.2.30/elkoep_mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:56:22.497289 elkoep_mqtt-0.2.30/inelsmqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)    18542 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/inelsmqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/inelsmqtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22709 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/inelsmqtt/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:56:22.497289 elkoep_mqtt-0.2.30/inelsmqtt/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/inelsmqtt/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/inelsmqtt/devices/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/inelsmqtt/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/inelsmqtt/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105922 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/inelsmqtt/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-20 10:56:22.497289 elkoep_mqtt-0.2.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:56:22.497289 elkoep_mqtt-0.2.30/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:56:22.497289 elkoep_mqtt-0.2.30/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/tests/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/tests/devices/device_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/tests/discovery_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/tests/inels_mqtt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-20 10:56:15.000000 elkoep_mqtt-0.2.30/tests/online_test.py
```

### Comparing `elkoep_mqtt-0.2.29/LICENSE` & `elkoep_mqtt-0.2.30/LICENSE`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/PKG-INFO` & `elkoep_mqtt-0.2.30/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkoep-mqtt
-Version: 0.2.29
+Version: 0.2.30
 Summary: Python library for iNELS mqtt protocol
 Home-page: https://github.com/epdevlab/elkoep-mqtt
 Author: Elko EP s.r.o.
 Author-email: epdevlab@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elkoep_mqtt-0.2.29/README.md` & `elkoep_mqtt-0.2.30/README.md`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/PKG-INFO` & `elkoep_mqtt-0.2.30/elkoep_mqtt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkoep-mqtt
-Version: 0.2.29
+Version: 0.2.30
 Summary: Python library for iNELS mqtt protocol
 Home-page: https://github.com/epdevlab/elkoep-mqtt
 Author: Elko EP s.r.o.
 Author-email: epdevlab@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elkoep_mqtt-0.2.29/elkoep_mqtt.egg-info/SOURCES.txt` & `elkoep_mqtt-0.2.30/elkoep_mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/inelsmqtt/__init__.py` & `elkoep_mqtt-0.2.30/inelsmqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/inelsmqtt/config.py` & `elkoep_mqtt-0.2.30/inelsmqtt/config.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/inelsmqtt/const.py` & `elkoep_mqtt-0.2.30/inelsmqtt/const.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/inelsmqtt/devices/__init__.py` & `elkoep_mqtt-0.2.30/inelsmqtt/devices/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             set_topic (str): Sring format of set topic
             title (str, optional): Formal name of the device. When None
             then will be same as unique_id. Defaults to None.
         """
         fragments = state_topic.split("/")
 
         self.__mqtt = mqtt
+        self.__device_class = fragments[TOPIC_FRAGMENTS[FRAGMENT_DEVICE_TYPE]]
         self.__device_type = DEVICE_TYPE_DICT[
             fragments[TOPIC_FRAGMENTS[FRAGMENT_DEVICE_TYPE]]
         ]
         self.__inels_type = INELS_DEVICE_TYPE_DICT[
             fragments[TOPIC_FRAGMENTS[FRAGMENT_DEVICE_TYPE]]
         ]
 
@@ -144,15 +145,19 @@
             if not GW_CONNECTED.get(gw):
                 return False
 
         val = self.__mqtt.messages().get(self._Device__connected_topic)
         if isinstance(val, (bytes, bytearray)):
             val = val.decode()
 
-        return DEVICE_CONNECTED.get(val) and self.__values is not None and self.__values._DeviceValue__ha_value is not None
+        # Temporary workaround to provide an always-online status for DT [164, 165, 166, 167, 168]
+        if self.__device_class in ["164", "165", "166", "167", "168"]:
+            return self.__values is not None and self.__values._DeviceValue__ha_value is not None
+        else:
+            return DEVICE_CONNECTED.get(val) and self.__values is not None and self.__values._DeviceValue__ha_value is not None
 
     @property
     def set_topic(self) -> str:
         """Set topic
 
         Returns:
             str: string of the set topic
```

### Comparing `elkoep_mqtt-0.2.29/inelsmqtt/devices/switch.py` & `elkoep_mqtt-0.2.30/inelsmqtt/devices/switch.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/inelsmqtt/discovery.py` & `elkoep_mqtt-0.2.30/inelsmqtt/discovery.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/inelsmqtt/mqtt_client.py` & `elkoep_mqtt-0.2.30/inelsmqtt/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/inelsmqtt/util.py` & `elkoep_mqtt-0.2.30/inelsmqtt/util.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/setup.py` & `elkoep_mqtt-0.2.30/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup script for elkoep-mqtt package."""
 from setuptools import setup, find_packages
 
 setup(
     name="elkoep-mqtt",
-    version="0.2.29",
+    version="0.2.30",
     url="https://github.com/epdevlab/elkoep-mqtt",
     license="MIT",
     author="Elko EP s.r.o.",
     author_email="epdevlab@gmail.com",
     description="Python library for iNELS mqtt protocol",
     keywords=["iNels", "Elko EP", "Home assistant integration"],
     long_description_content_type="text/markdown",
```

### Comparing `elkoep_mqtt-0.2.29/tests/const.py` & `elkoep_mqtt-0.2.30/tests/const.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/tests/devices/device_test.py` & `elkoep_mqtt-0.2.30/tests/devices/device_test.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/tests/discovery_test.py` & `elkoep_mqtt-0.2.30/tests/discovery_test.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/tests/inels_mqtt_test.py` & `elkoep_mqtt-0.2.30/tests/inels_mqtt_test.py`

 * *Files identical despite different names*

### Comparing `elkoep_mqtt-0.2.29/tests/online_test.py` & `elkoep_mqtt-0.2.30/tests/online_test.py`

 * *Files identical despite different names*


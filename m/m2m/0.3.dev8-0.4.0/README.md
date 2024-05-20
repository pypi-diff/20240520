# Comparing `tmp/m2m-0.3.dev8.tar.gz` & `tmp/m2m-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m2m-0.3.dev8.tar", last modified: Tue Aug  2 18:10:06 2022, max compression
+gzip compressed data, was "m2m-0.4.0.tar", last modified: Mon May 20 21:02:50 2024, max compression
```

## Comparing `m2m-0.3.dev8.tar` & `m2m-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-08-02 18:10:06.080710 m2m-0.3.dev8/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       52 2022-03-20 10:49:19.000000 m2m-0.3.dev8/AUTHORS
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       17 2022-03-20 10:19:42.000000 m2m-0.3.dev8/BUGS.md
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       56 2022-03-20 10:49:19.000000 m2m-0.3.dev8/CHANGES.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1092 2022-03-20 10:49:19.000000 m2m-0.3.dev8/LICENSE
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      436 2022-05-14 05:33:58.000000 m2m-0.3.dev8/MANIFEST.in
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     2423 2022-08-02 18:10:06.080710 m2m-0.3.dev8/PKG-INFO
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      465 2022-08-02 18:08:23.000000 m2m-0.3.dev8/PUBLISH_HOWTO.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1562 2022-03-20 20:14:50.000000 m2m-0.3.dev8/README.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      228 2022-03-20 10:19:42.000000 m2m-0.3.dev8/TODO.md
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-08-02 18:10:06.080710 m2m-0.3.dev8/bin/
--rwxr-xr-x   0 jeremie   (1010) jeremie   (1010)      407 2022-03-20 20:25:14.000000 m2m-0.3.dev8/bin/http2influx
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-08-02 18:10:06.080710 m2m-0.3.dev8/docs/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7594 2022-03-20 10:49:19.000000 m2m-0.3.dev8/docs/Makefile
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      275 2022-03-20 10:49:19.000000 m2m-0.3.dev8/docs/api.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      126 2022-03-20 10:19:42.000000 m2m-0.3.dev8/docs/api_TODO_MODULE_NAME.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    10776 2022-03-20 10:49:19.000000 m2m-0.3.dev8/docs/conf.py
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     5166 2022-03-20 10:49:19.000000 m2m-0.3.dev8/docs/developer.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      689 2022-03-20 10:49:19.000000 m2m-0.3.dev8/docs/index.rst
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      836 2022-03-20 10:49:19.000000 m2m-0.3.dev8/docs/init_sphinx.sh
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      201 2022-03-20 10:49:19.000000 m2m-0.3.dev8/docs/intro.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7726 2022-03-20 10:49:19.000000 m2m-0.3.dev8/docs/make.bat
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-08-02 18:10:06.080710 m2m-0.3.dev8/m2m/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1121 2022-08-02 18:07:30.000000 m2m-0.3.dev8/m2m/__init__.py
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      478 2022-05-02 09:39:09.000000 m2m-0.3.dev8/m2m/config.py
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)     7243 2022-03-21 15:50:32.000000 m2m-0.3.dev8/m2m/http2influx.py
--rwxr-xr-x   0 jeremie   (1010) jeremie   (1010)     4408 2022-05-14 07:19:46.000000 m2m-0.3.dev8/m2m/meteofrance2mqtt.py
--rwxr-xr-x   0 jeremie   (1010) jeremie   (1010)     6161 2022-05-14 06:17:06.000000 m2m-0.3.dev8/m2m/mqtt2influx.py
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      970 2022-05-02 09:35:23.000000 m2m-0.3.dev8/m2m/path.py
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-08-02 18:10:06.080710 m2m-0.3.dev8/m2m.egg-info/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     2423 2022-08-02 18:10:06.000000 m2m-0.3.dev8/m2m.egg-info/PKG-INFO
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      537 2022-08-02 18:10:06.000000 m2m-0.3.dev8/m2m.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        1 2022-08-02 18:10:06.000000 m2m-0.3.dev8/m2m.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       98 2022-08-02 18:10:06.000000 m2m-0.3.dev8/m2m.egg-info/entry_points.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        4 2022-08-02 18:10:06.000000 m2m-0.3.dev8/m2m.egg-info/top_level.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       84 2022-03-20 11:32:42.000000 m2m-0.3.dev8/pyproject.toml
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       61 2022-05-13 20:50:00.000000 m2m-0.3.dev8/requirements.txt
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)     1033 2022-08-02 18:10:06.080710 m2m-0.3.dev8/setup.cfg
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2024-05-20 21:02:50.240782 m2m-0.4.0/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       52 2022-03-20 10:49:19.000000 m2m-0.4.0/AUTHORS
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       17 2022-03-20 10:19:42.000000 m2m-0.4.0/BUGS.md
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       56 2022-03-20 10:49:19.000000 m2m-0.4.0/CHANGES.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1092 2022-03-20 10:49:19.000000 m2m-0.4.0/LICENSE
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        0 2024-05-20 15:13:21.000000 m2m-0.4.0/MANIFEST.in
+-rw-r--r--   0 jeremie   (1010) jeremie   (1010)     3135 2024-05-20 21:02:50.240782 m2m-0.4.0/PKG-INFO
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      465 2024-05-20 15:13:21.000000 m2m-0.4.0/PUBLISH_HOWTO.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     2474 2024-05-20 16:48:28.000000 m2m-0.4.0/README.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      228 2022-03-20 10:19:42.000000 m2m-0.4.0/TODO.md
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2024-05-20 21:02:50.236782 m2m-0.4.0/bin/
+-rwxr-xr-x   0 jeremie   (1010) jeremie   (1010)      407 2022-03-20 20:25:14.000000 m2m-0.4.0/bin/http2influx
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2024-05-20 21:02:50.240782 m2m-0.4.0/docs/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7594 2022-03-20 10:49:19.000000 m2m-0.4.0/docs/Makefile
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      275 2022-03-20 10:49:19.000000 m2m-0.4.0/docs/api.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      126 2022-03-20 10:19:42.000000 m2m-0.4.0/docs/api_TODO_MODULE_NAME.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    10776 2022-03-20 10:49:19.000000 m2m-0.4.0/docs/conf.py
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     5166 2022-03-20 10:49:19.000000 m2m-0.4.0/docs/developer.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      689 2022-03-20 10:49:19.000000 m2m-0.4.0/docs/index.rst
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      836 2022-03-20 10:49:19.000000 m2m-0.4.0/docs/init_sphinx.sh
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      201 2022-03-20 10:49:19.000000 m2m-0.4.0/docs/intro.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7726 2022-03-20 10:49:19.000000 m2m-0.4.0/docs/make.bat
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2024-05-20 21:02:50.240782 m2m-0.4.0/m2m/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1098 2024-05-20 15:13:21.000000 m2m-0.4.0/m2m/__init__.py
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      478 2022-05-02 09:39:09.000000 m2m-0.4.0/m2m/config.py
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)     7243 2022-03-21 15:50:32.000000 m2m-0.4.0/m2m/http2influx.py
+-rwxr-xr-x   0 jeremie   (1010) jeremie   (1010)     4408 2022-05-14 07:19:46.000000 m2m-0.4.0/m2m/meteofrance2mqtt.py
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)     7307 2024-05-20 18:10:21.000000 m2m-0.4.0/m2m/mqtt2influx.py
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      970 2022-05-02 09:35:23.000000 m2m-0.4.0/m2m/path.py
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2024-05-20 21:02:50.240782 m2m-0.4.0/m2m.egg-info/
+-rw-r--r--   0 jeremie   (1010) jeremie   (1010)     3135 2024-05-20 21:02:50.000000 m2m-0.4.0/m2m.egg-info/PKG-INFO
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      553 2024-05-20 21:02:50.000000 m2m-0.4.0/m2m.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        1 2024-05-20 21:02:50.000000 m2m-0.4.0/m2m.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       98 2024-05-20 21:02:50.000000 m2m-0.4.0/m2m.egg-info/entry_points.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       69 2024-05-20 21:02:50.000000 m2m-0.4.0/m2m.egg-info/requires.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        4 2024-05-20 21:02:50.000000 m2m-0.4.0/m2m.egg-info/top_level.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1030 2024-05-20 21:01:37.000000 m2m-0.4.0/pyproject.toml
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       69 2024-05-20 17:12:34.000000 m2m-0.4.0/requirements.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       38 2024-05-20 21:02:50.240782 m2m-0.4.0/setup.cfg
```

### Comparing `m2m-0.3.dev8/LICENSE` & `m2m-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/docs/Makefile` & `m2m-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/docs/conf.py` & `m2m-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/docs/developer.rst` & `m2m-0.4.0/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/docs/index.rst` & `m2m-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/docs/init_sphinx.sh` & `m2m-0.4.0/docs/init_sphinx.sh`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/docs/make.bat` & `m2m-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/m2m/__init__.py` & `m2m-0.4.0/m2m/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,13 +32,11 @@
 # X.YbN # Beta release         
 # X.YrcN # Release Candidate   
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '0.3.dev8'
+__version__ = '0.4.0'
 
 def get_version():
     return __version__
-
-__all__ = ['TODO']
```

### Comparing `m2m-0.3.dev8/m2m/http2influx.py` & `m2m-0.4.0/m2m/http2influx.py`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/m2m/meteofrance2mqtt.py` & `m2m-0.4.0/m2m/meteofrance2mqtt.py`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/m2m/mqtt2influx.py` & `m2m-0.4.0/m2m/mqtt2influx.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,62 +2,74 @@
 
 # https://pypi.org/project/paho-mqtt/#id2
 # https://medium.com/python-point/mqtt-basics-with-python-examples-7c758e605d4
 
 import m2m
 
 import argparse
+import math
 import paho.mqtt.client as mqtt
 import json
 import sys
 import traceback
 
 from influxdb_client import InfluxDBClient
 from influxdb_client.client.write_api import SYNCHRONOUS
 
 class MQTT2Influx:
 
-    def __init__(self, config_path, verbose=False):
+    def __init__(self, config_path, verbose=False, dry=False):
 
         self.verbose = verbose
+        self.dry = dry
 
         # Get config
 
         self.cfg, self.config_path = m2m.config.get_config(config_path)
 
         # Setup MQTT
 
-        self.mqtt_client = mqtt.Client(self.cfg["mqtt2influx"]["mqtt"]["client_name"])
+        self.mqtt_client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2)
         self.mqtt_client.on_connect = self.mqtt_on_connect_callback
         self.mqtt_client.on_message = self.mqtt_on_message_callback
         self.mqtt_client.connect(self.cfg["mqtt2influx"]["mqtt"]["broker_address"])
 
         # Setup InfluxDB
 
-        self.influxdb_org = self.cfg["mqtt2influx"]["influxdb"]["org"]
-        self.influxdb_bucket = self.cfg["mqtt2influx"]["influxdb"]["bucket"]
-
-        self.influxdb_client = InfluxDBClient(url=self.cfg["mqtt2influx"]["influxdb"]["url"],
-                                              token=self.cfg["mqtt2influx"]["influxdb"]["token"],
-                                              org=self.influxdb_org)
-        self.influxdb_write_api = self.influxdb_client.write_api(write_options=SYNCHRONOUS)
+        if not dry:
+            self.influxdb_org = self.cfg["mqtt2influx"]["influxdb"]["org"]
+            self.influxdb_bucket = self.cfg["mqtt2influx"]["influxdb"]["bucket"]
+
+            self.influxdb_client = InfluxDBClient(url=self.cfg["mqtt2influx"]["influxdb"]["url"],
+                                                  token=self.cfg["mqtt2influx"]["influxdb"]["token"],
+                                                  org=self.influxdb_org)
+            self.influxdb_write_api = self.influxdb_client.write_api(write_options=SYNCHRONOUS)
 
 
     # The callback for when the client receives a CONNACK response from the server.
     # Subscribing in on_connect() means that if we lose the connection and reconnect then subscriptions will be renewed.
-    def mqtt_on_connect_callback(self, mqtt_client, userdata, flags, rc):
+    def mqtt_on_connect_callback(self, mqtt_client, userdata, flags, reason_code, properties):
         # Print a confirmation message
-        print(f'Connected to the MQTT broker at {self.cfg["mqtt2influx"]["mqtt"]["broker_address"]} with result code ' + str(rc))
+        print(f'Connected to the MQTT broker at {self.cfg["mqtt2influx"]["mqtt"]["broker_address"]} with result code {reason_code}')
 
         # Subscribe to MQTT topics
+        # Subscribing in on_connect() means that if we lose the connection and reconnect then subscriptions will be renewed.
         for topic_str in self.cfg["mqtt2influx"]["mqtt"]["subscribed_topic_list"]:
             print(f"Subscribe to {topic_str}")
             mqtt_client.subscribe(topic_str)
 
 
+    # def on_disconnect(mqttc, userdata, rc):
+    #     if rc != 0:
+    #         print("Unexpected disconnection. Reconnecting...")
+    #         mqttc.reconnect()
+    #     else:
+    #         print("Disconnected successfully")
+
+
     def mqtt_on_message_callback(self, client, userdata, message):
         #print(message)
 
         try:
             topic = message.topic
 
             device_desc = None
@@ -83,26 +95,34 @@
                         default_value = measure_schema_dict["default_value"]
                         if default_value == "nan":
                             default_value = float("nan")
 
                         value = data_dict.get(measure_schema_dict["mqtt_measurement_name"], default_value)
                         if "discrete_value_converter_dict" in measure_schema_dict:
                             discrete_value_converter_dict = measure_schema_dict["discrete_value_converter_dict"]
-                            value = int(discrete_value_converter_dict[value])
+                            try:
+                                if value != 'nan':
+                                    value = int(discrete_value_converter_dict[str(value)])
+                            except:
+                                print(f'Unexpected value "{value}" (of type "{type(value)}") in {discrete_value_converter_dict}', file=sys.stderr)
+                                print(f"data_dict: {data_dict}", file=sys.stderr)
+                                print(f"topic: {topic}", file=sys.stderr)
+                                raise
                         elif "boolean_true_value" in measure_schema_dict:
                             value = 1 if value==measure_schema_dict["boolean_true_value"] else 0
                         elif "boolean_false_value" in measure_schema_dict:
                             value = 0 if value==measure_schema_dict["boolean_false_value"] else 1 
 
                         data_str = f'{measure_schema_dict["influxdb_measurement_name"]},device_id={device_id},zone_name={zone_name},device_type={device_type},unit={measure_schema_dict["unit"]} value={value}'
 
                         if self.verbose:
                             print(data_str)
 
-                        self.influxdb_write_api.write(self.influxdb_bucket, self.influxdb_org, [data_str])
+                        if not self.dry:
+                            self.influxdb_write_api.write(self.influxdb_bucket, self.influxdb_org, [data_str])
 
 
         except Exception as e:
             print("Error: ", e, file=sys.stderr)
             print(traceback.format_exc(), file=sys.stderr)
 
 
@@ -122,27 +142,30 @@
     # PARSE OPTIONS ###########################################################
 
     parser = argparse.ArgumentParser(description="MQTT2Influx Daemon")
 
     parser.add_argument("--version", "-V", action="store_true",
                         help="Print the M2M Daemons version and exit.")
 
+    parser.add_argument("--dry", "-d", action="store_true",
+                        help="Read and log MQTT messages but don't write them into InfluxDB.")
+
     parser.add_argument("--verbose", "-v", action="store_true",
                         help="Print debug messages.")
 
     parser.add_argument("--config-path", default=None, metavar="FILE",
                         help="Configuration file path.")
 
     args = parser.parse_args()
 
     ###########################################################################
 
     if args.version:
         print(m2m.get_version())
     else:
         print(f"Starting MQTT2Influx Daemon {m2m.get_version()}")
-        daemon = MQTT2Influx(args.config_path, verbose=args.verbose)
+        daemon = MQTT2Influx(args.config_path, verbose=args.verbose, dry=args.dry)
         daemon.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `m2m-0.3.dev8/m2m/path.py` & `m2m-0.4.0/m2m/path.py`

 * *Files identical despite different names*

### Comparing `m2m-0.3.dev8/m2m.egg-info/SOURCES.txt` & `m2m-0.4.0/m2m.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 LICENSE
 MANIFEST.in
 PUBLISH_HOWTO.rst
 README.rst
 TODO.md
 pyproject.toml
 requirements.txt
-setup.cfg
 bin/http2influx
 docs/Makefile
 docs/api.rst
 docs/api_TODO_MODULE_NAME.rst
 docs/conf.py
 docs/developer.rst
 docs/index.rst
@@ -25,8 +24,9 @@
 m2m/meteofrance2mqtt.py
 m2m/mqtt2influx.py
 m2m/path.py
 m2m.egg-info/PKG-INFO
 m2m.egg-info/SOURCES.txt
 m2m.egg-info/dependency_links.txt
 m2m.egg-info/entry_points.txt
+m2m.egg-info/requires.txt
 m2m.egg-info/top_level.txt
```


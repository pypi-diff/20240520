# Comparing `tmp/tplinkrouterc6u-4.0.2.tar.gz` & `tmp/tplinkrouterc6u-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tplinkrouterc6u-4.0.2.tar", last modified: Wed May 15 07:22:27 2024, max compression
+gzip compressed data, was "tplinkrouterc6u-4.1.0.tar", last modified: Mon May 20 13:01:52 2024, max compression
```

## Comparing `tplinkrouterc6u-4.0.2.tar` & `tplinkrouterc6u-4.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:22:27.229189 tplinkrouterc6u-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30473 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/test/test_client_deco.py
--rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/test/test_client_mr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/tplinkrouterc6u/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48732 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 07:22:23.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:22:27.233189 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 07:22:27.000000 tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:01:52.683497 tplinkrouterc6u-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-20 13:01:52.683497 tplinkrouterc6u-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:01:52.683497 tplinkrouterc6u-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:01:52.683497 tplinkrouterc6u-4.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30588 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/test/test_client_deco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23145 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/test/test_client_mr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:01:52.683497 tplinkrouterc6u-4.1.0/tplinkrouterc6u/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48906 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 13:01:48.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:01:52.683497 tplinkrouterc6u-4.1.0/tplinkrouterc6u.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-20 13:01:52.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-20 13:01:52.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:01:52.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 13:01:52.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 13:01:52.000000 tplinkrouterc6u-4.1.0/tplinkrouterc6u.egg-info/top_level.txt
```

### Comparing `tplinkrouterc6u-4.0.2/LICENSE` & `tplinkrouterc6u-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.2/PKG-INFO` & `tplinkrouterc6u-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplinkrouterc6u
-Version: 4.0.2
+Version: 4.1.0
 Summary: TP-Link Router API
 Home-page: https://github.com/AlexandrErohin/TP-Link-Archer-C6U
 Author: Alex Erohin
 Author-email: alexanderErohin@yandex.ru
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -156,14 +156,16 @@
 | macaddr | client mac address | str |
 | macaddress | client mac address | macaddress |
 | ipaddr | client ip address | str |
 | ipaddress | client ip address | ipaddress |
 | hostname | client hostname | str |
 | packets_sent | total packets sent | int, None |
 | packets_received | total packets received | int, None |
+| down_speed | download speed | int, None |
+| up_speed | upload speed | int, None |
 
 ### <a id="IPv4Reservation">IPv4Reservation</a>
 | Field | Description | Type |
 | --- |---|---|
 | macaddr | client mac address | str |
 | macaddress| client mac address | macaddress |
 | ipaddr | client ip address | str |
@@ -224,14 +226,15 @@
 - Archer A7 V5
 - Archer AX10 v1.0
 - Archer AX12 v1.0
 - Archer AX20 v1.0
 - Archer AX21 v1.20
 - Archer AX23 v1.0
 - Archer AX50 v1.0
+- Archer AX53 v2
 - Archer AX55 v1.0
 - Archer AX55 V1.60
 - Archer AX72 V1
 - Archer AX73 V1
 - Archer AX75 V1
 - Archer AXE75 V1
 - Archer AX3000 V1
```

### Comparing `tplinkrouterc6u-4.0.2/README.md` & `tplinkrouterc6u-4.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,16 @@
 | macaddr | client mac address | str |
 | macaddress | client mac address | macaddress |
 | ipaddr | client ip address | str |
 | ipaddress | client ip address | ipaddress |
 | hostname | client hostname | str |
 | packets_sent | total packets sent | int, None |
 | packets_received | total packets received | int, None |
+| down_speed | download speed | int, None |
+| up_speed | upload speed | int, None |
 
 ### <a id="IPv4Reservation">IPv4Reservation</a>
 | Field | Description | Type |
 | --- |---|---|
 | macaddr | client mac address | str |
 | macaddress| client mac address | macaddress |
 | ipaddr | client ip address | str |
@@ -203,14 +205,15 @@
 - Archer A7 V5
 - Archer AX10 v1.0
 - Archer AX12 v1.0
 - Archer AX20 v1.0
 - Archer AX21 v1.20
 - Archer AX23 v1.0
 - Archer AX50 v1.0
+- Archer AX53 v2
 - Archer AX55 v1.0
 - Archer AX55 V1.60
 - Archer AX72 V1
 - Archer AX73 V1
 - Archer AX75 V1
 - Archer AXE75 V1
 - Archer AX3000 V1
```

### Comparing `tplinkrouterc6u-4.0.2/setup.py` & `tplinkrouterc6u-4.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tplinkrouterc6u",
-    version="4.0.2",
+    version="4.1.0",
     author="Alex Erohin",
     author_email="alexanderErohin@yandex.ru",
     description="TP-Link Router API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AlexandrErohin/TP-Link-Archer-C6U",
     packages=setuptools.find_packages(),
```

### Comparing `tplinkrouterc6u-4.0.2/test/test_client.py` & `tplinkrouterc6u-4.1.0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.2/test/test_client_deco.py` & `tplinkrouterc6u-4.1.0/test/test_client_deco.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,14 +242,16 @@
         self.assertEqual(status.wifi_5g_enable, False)
         self.assertEqual(status.wifi_6g_enable, True)
 
         self.assertEqual(len(status.devices), 5)
         self.assertIsInstance(status.devices[0], Device)
         self.assertEqual(status.devices[0].type, Connection.HOST_5G)
         self.assertEqual(status.devices[0].macaddr, 'CF-51-C9-04-E1-02')
+        self.assertEqual(status.devices[0].down_speed, 3)
+        self.assertEqual(status.devices[0].up_speed, 17)
         self.assertIsInstance(status.devices[0].macaddress, macaddress.EUI48)
         self.assertIsInstance(status.devices[1], Device)
         self.assertEqual(status.devices[1].type, Connection.IOT_2G)
         self.assertEqual(status.devices[1].macaddr, '5F-F8-08-28-AF-54')
         self.assertIsInstance(status.devices[2], Device)
         self.assertEqual(status.devices[2].type, Connection.IOT_5G)
         self.assertEqual(status.devices[2].macaddr, '5F-F8-08-28-AF-55')
```

### Comparing `tplinkrouterc6u-4.0.2/test/test_client_mr.py` & `tplinkrouterc6u-4.1.0/test/test_client_mr.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.2/tplinkrouterc6u/client.py` & `tplinkrouterc6u-4.1.0/tplinkrouterc6u/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,18 +571,21 @@
                 status.guest_clients_total += 1
             elif conn.is_iot():
                 if status.iot_clients_total is None:
                     status.iot_clients_total = 0
                 status.iot_clients_total += 1
 
             ip = item['ip'] if item.get('ip') else '0.0.0.0'
-            devices.append(Device(conn,
+            device = Device(conn,
                                   macaddress.EUI48(item['mac']),
                                   ipaddress.IPv4Address(ip),
-                                  base64.b64decode(item['name']).decode()))
+                                  base64.b64decode(item['name']).decode())
+            device.down_speed = item.get('down_speed')
+            device.up_speed = item.get('up_speed')
+            devices.append(device)
 
         status.clients_total = (status.wired_total + status.wifi_clients_total + status.guest_clients_total
                                 + (0 if status.iot_clients_total is None else status.iot_clients_total))
         status.devices = devices
 
         return status
 
@@ -691,14 +694,15 @@
         )
 
         try:
             self._stok = response.json().get('data').get('stok')
             regex_result = re.search('sysauth=(.*);', response.headers['set-cookie'])
             self._sysauth = regex_result.group(1)
             self._logged = True
+            self._smart_network = False
 
         except Exception as e:
             error = "TplinkRouter - C1200 - Cannot authorize! Error - {}; Response - {}".format(e, response.text)
             if self._logger:
                 self._logger.error(error)
             raise ClientException(error)
```

### Comparing `tplinkrouterc6u-4.0.2/tplinkrouterc6u/dataclass.py` & `tplinkrouterc6u-4.1.0/tplinkrouterc6u/dataclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     def __init__(self, type: Connection, macaddr: macaddress, ipaddr: ipaddress, hostname: str) -> None:
         self.type = type
         self._macaddr = macaddr
         self._ipaddr = ipaddr
         self.hostname = hostname
         self.packets_sent: int | None = None
         self.packets_received: int | None = None
+        self.down_speed: int | None = None
+        self.up_speed: int | None = None
 
     @property
     def macaddr(self):
         return str(self._macaddr)
 
     @property
     def macaddress(self):
```

### Comparing `tplinkrouterc6u-4.0.2/tplinkrouterc6u/encryption.py` & `tplinkrouterc6u-4.1.0/tplinkrouterc6u/encryption.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.2/tplinkrouterc6u/enum.py` & `tplinkrouterc6u-4.1.0/tplinkrouterc6u/enum.py`

 * *Files identical despite different names*

### Comparing `tplinkrouterc6u-4.0.2/tplinkrouterc6u.egg-info/PKG-INFO` & `tplinkrouterc6u-4.1.0/tplinkrouterc6u.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplinkrouterc6u
-Version: 4.0.2
+Version: 4.1.0
 Summary: TP-Link Router API
 Home-page: https://github.com/AlexandrErohin/TP-Link-Archer-C6U
 Author: Alex Erohin
 Author-email: alexanderErohin@yandex.ru
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -156,14 +156,16 @@
 | macaddr | client mac address | str |
 | macaddress | client mac address | macaddress |
 | ipaddr | client ip address | str |
 | ipaddress | client ip address | ipaddress |
 | hostname | client hostname | str |
 | packets_sent | total packets sent | int, None |
 | packets_received | total packets received | int, None |
+| down_speed | download speed | int, None |
+| up_speed | upload speed | int, None |
 
 ### <a id="IPv4Reservation">IPv4Reservation</a>
 | Field | Description | Type |
 | --- |---|---|
 | macaddr | client mac address | str |
 | macaddress| client mac address | macaddress |
 | ipaddr | client ip address | str |
@@ -224,14 +226,15 @@
 - Archer A7 V5
 - Archer AX10 v1.0
 - Archer AX12 v1.0
 - Archer AX20 v1.0
 - Archer AX21 v1.20
 - Archer AX23 v1.0
 - Archer AX50 v1.0
+- Archer AX53 v2
 - Archer AX55 v1.0
 - Archer AX55 V1.60
 - Archer AX72 V1
 - Archer AX73 V1
 - Archer AX75 V1
 - Archer AXE75 V1
 - Archer AX3000 V1
```


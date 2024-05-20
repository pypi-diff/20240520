# Comparing `tmp/bluepy3-2.6.1.tar.gz` & `tmp/bluepy3-2.8.1.tar.gz`

## Comparing `bluepy3-2.6.1.tar` & `bluepy3-2.8.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/Makefile
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/__init__.py
--rwxr-xr-x   0        0        0     5144 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/blescan.py
--rw-r--r--   0        0        0    58458 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0        0        0    40792 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/btle.py
--rwxr-xr-x   0        0        0    10019 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/get_services.py
--rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/helpermaker.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/py.typed
--rw-r--r--   0        0        0    37880 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/uuids.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/version.h
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.47.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.50.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.60.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.66.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.68.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.70.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.71.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.72.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.73.h
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.6.1/bluepy3/config/config.5.75.h
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 bluepy3-2.6.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bluepy3-2.6.1/LICENSE
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 bluepy3-2.6.1/README.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 bluepy3-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 bluepy3-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/Makefile
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/__init__.py
+-rwxr-xr-x   0        0        0     5144 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/blescan.py
+-rw-r--r--   0        0        0    58458 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0        0        0    40922 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/btle.py
+-rwxr-xr-x   0        0        0    10019 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/get_services.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/helpermaker.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/py.typed
+-rw-r--r--   0        0        0    37880 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/uuids.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/version.h
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.47.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.50.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.60.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.66.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.68.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.70.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.71.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.72.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.73.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.75.h
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 bluepy3-2.8.1/bluepy3/config/config.5.76.h
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 bluepy3-2.8.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 bluepy3-2.8.1/LICENSE
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 bluepy3-2.8.1/README.md
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 bluepy3-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 bluepy3-2.8.1/PKG-INFO
```

### Comparing `bluepy3-2.6.1/bluepy3/Makefile` & `bluepy3-2.8.1/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/blescan.py` & `bluepy3-2.8.1/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/bluepy3-helper.c` & `bluepy3-2.8.1/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/btle.py` & `bluepy3-2.8.1/bluepy3/btle.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 import json
 import os
 import signal
 import struct
 import subprocess  # nosec: B404
 import sys
 import time
+
 from queue import Queue, Empty
 from threading import Thread
-from typing import Any, Generator, Optional, TextIO
+from typing import Any, Generator, Self, TextIO, Union
 
 
 Debugging = False
 SCRIPT_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)))
 HELPER_PATH = os.path.join(SCRIPT_PATH, "bluepy3-helper")
 
 # If the executable `bluepy3-helper` does not exist
@@ -279,25 +280,25 @@
         self.addrType: str = ""
         self.rssi: float = 0.0
         self.connectable: bool = False
         self.rawData = None
         self.scanData: dict = {}
         self.updateCount: int = 0
 
-    def _decodeUUID(self, val, nbytes):
+    def _decodeUUID(self, val, nbytes: int):
         if len(val) < nbytes:
             return None
         bval = bytearray(val)
-        rs = ""
+        rs: str = ""
         # Bytes are little-endian; convert to big-endian string
         for i in range(nbytes):
             rs = f"{bval[i]:02X}{rs}"
         return UUID(rs)
 
-    def _decodeUUIDlist(self, val, nbytes):
+    def _decodeUUIDlist(self, val, nbytes: int):
         result = []
         for i in range(0, len(val), nbytes):
             if len(val) >= (i + nbytes):
                 result.append(self._decodeUUID(val[i : i + nbytes], nbytes))
         return result
 
     def getDescription(self, sdid) -> str:
@@ -329,16 +330,16 @@
             return self._decodeUUIDlist(val, 4)
         if sdid in [ScanEntry.INCOMPLETE_128B_SERVICES, ScanEntry.COMPLETE_128B_SERVICES]:
             return self._decodeUUIDlist(val, 16)
         return val
 
     def getValueText(self, sdid):
         val = self.getValue(sdid)
-        if val is None:
-            return None
+        if not val:
+            return ""
         if sdid in [ScanEntry.SHORT_LOCAL_NAME, ScanEntry.COMPLETE_LOCAL_NAME]:
             return val
         if isinstance(val, list):
             return ",".join(str(v) for v in val)
         return binascii.b2a_hex(val).decode("ascii")
 
     def update(self, resp: dict[str, list[Any]]) -> bool:
@@ -544,16 +545,16 @@
                 self._aita += 1
                 if self._aita > 3:
                     self._stopHelper()
                     raise BTLEInternalError("Device keeps repeating itself. Giving up.", resp)
 
             try:
                 respType = resp["rsp"][0]
-            except KeyError:
-                raise BTLEInternalError("Unexpected absence of response 'rsp'", resp)
+            except KeyError as her:
+                raise BTLEInternalError("Unexpected absence of response 'rsp'", resp) from her
 
             # always check for MTU updates
             if "mtu" in resp and len(resp["mtu"]) > 0:
                 new_mtu = int(resp["mtu"][0])
                 if self._mtu != new_mtu:
                     self._mtu = new_mtu
                     DBG(f"    -btle- Updated MTU: {str(self._mtu)}")
@@ -610,15 +611,15 @@
                 resp[tag].append(val)
         return resp
 
     def status(self) -> dict[str, list[Any]]:
         self._writeCmd("stat\n")
         return self._waitResp(["stat"])
 
-    def withDelegate(self, delegate_: DefaultDelegate):
+    def withDelegate(self, delegate_: DefaultDelegate) -> Self:
         self.delegate = delegate_
         return self
 
 
 class Peripheral(Bluepy3Helper):
     # fmt: off
     def __init__(self, addr: str = "", addrType: str = ADDR_TYPE_PUBLIC, iface: str = "", timeout: float = BTLE_TIMEOUT) -> None:
@@ -654,16 +655,16 @@
     ) -> dict[str, list[Any]]:
         while True:
             resp: dict[str, list[Any]] = self._waitResp(wantType + ["ntfy", "ind"], timeout)
             if not resp:
                 return {}
             try:
                 respType = resp["rsp"][0]
-            except KeyError:
-                raise BTLEInternalError("Unexpected absence of response 'rsp'", resp)
+            except KeyError as her:
+                raise BTLEInternalError("Unexpected absence of response 'rsp'", resp) from her
             if respType in ["ntfy", "ind"]:
                 hnd = resp["hnd"][0]
                 data = resp["d"][0]
                 if self.delegate is not None:
                     self.delegate.handleNotification(hnd, data)
             if respType not in wantType:
                 continue
@@ -796,15 +797,15 @@
         # In bluez 5.25 and later, gatt_discover_desc() in attrib/gatt.c does the retry
         # so bluetooth_helper always returns a full list.
         # This was broken in earlier versions.
         resp: dict[str, list[Any]] = self._getResp(["desc"])
         ndesc: int = len(resp["hnd"])
         return [Descriptor(self, resp["uuid"][i], resp["hnd"][i]) for i in range(ndesc)]
 
-    def setDelegate(self, delegate_):  # same as withDelegate(), deprecated
+    def setDelegate(self, delegate_) -> Self:  # same as withDelegate(), deprecated
         return self.withDelegate(delegate_)
 
     def getLocalOOB(self, iface=None):
         cmd: str = ""
         if self._helper is None:
             self._startHelper(iface)
         self.iface = iface
@@ -945,36 +946,36 @@
 
     def _cmd(self) -> str:
         return "pasv" if self.passive else "scan"
 
     def clear(self) -> None:
         self.scanned = {}
 
-    def getDevices(self):
+    def getDevices(self) -> list:
         return list(self.scanned.values())
 
-    def process(self, timeout=10.0) -> None:
+    def process(self, timeout=BTLE_TIMEOUT) -> None:
         if self._helper is None:
             raise BTLEInternalError("Helper not started (did you call start()?)")
         start = time.time()
         while True:
             if timeout:
-                remain = start + timeout - time.time()
+                remain: float = start + timeout - time.time()
                 if remain <= 0.0:
                     break
             else:
-                remain = None
+                remain = 0.0
             resp: dict[str, list[Any]] = self._waitResp(["scan", "stat"], remain)
             if not resp:
                 break
 
             try:
                 respType = resp["rsp"][0]
-            except KeyError:
-                raise BTLEInternalError("Unexpected absence of response 'rsp'", resp)
+            except KeyError as her:
+                raise BTLEInternalError("Unexpected absence of response 'rsp'", resp) from her
 
             if respType == "stat":
                 # if scan ended, restart it
                 if resp["state"][0] == "disc":
                     self._mgmtCmd(self._cmd())
             elif respType == "scan":
                 # device found
@@ -987,15 +988,15 @@
                     self.scanned[addr] = dev
                 isNewData = dev.update(resp)
                 if self.delegate is not None:
                     self.delegate.handleDiscovery(dev, (dev.updateCount <= 1), isNewData)
             else:
                 raise BTLEInternalError(f"Unexpected response: {respType}", resp)
 
-    def scan(self, timeout=10, passive=False):
+    def scan(self, timeout=BTLE_TIMEOUT, passive=False) -> list:
         self.clear()
         self.start(passive=passive)
         self.process(timeout)
         self.stop()
         return self.getDevices()
 
     def start(self, passive: bool = False) -> None:
@@ -1037,15 +1038,15 @@
 def capitaliseName(descr) -> str:
     words = descr.replace("(", " ").replace(")", " ").replace("-", " ").split(" ")
     capWords = [words[0].lower()]
     capWords += [w[0:1].upper() + w[1:].lower() for w in words[1:]]
     return "".join(capWords)
 
 
-def get_json_uuid():
+def get_json_uuid() -> Generator:
     # an entry in the uuid_list is a list containing an `int`` and two `str`
     # example: [10082, 'day', 'time (day)']
     with open(os.path.join(SCRIPT_PATH, "uuids.json"), "rb") as fp:
         _uuid_data = json.loads(fp.read().decode("utf-8"))
     for _, _v in _uuid_data.items():
         for number, cname, name in _v:
             yield UUID(number, cname)
```

### Comparing `bluepy3-2.6.1/bluepy3/get_services.py` & `bluepy3-2.8.1/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/helpermaker.py` & `bluepy3-2.8.1/bluepy3/helpermaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     # read the Makefile
     with open(MAKEFILE, "r", encoding="utf-8") as makefile:
         lines: list[str] = makefile.readlines()
     # write the Makefile while inserting the desired BLUEZ_VERSION
     with open(MAKEFILE, "w", encoding="utf-8") as makefile:
         for line in lines:
             if line.startswith("BLUEZ_VERSION"):
-                line: str = f"BLUEZ_VERSION={BLUEZ_VERSION}\n"
+                line = f"BLUEZ_VERSION={BLUEZ_VERSION}\n"
             makefile.write(line)
     if platform.system().lower() == "linux":
         # Windows and macOS are not supported
         _LOGGER.info("*** Building bluepy3-helper")
         for cmd in [f"make -C {APP_ROOT} clean", f"make -C {APP_ROOT} -j1"]:
             _LOGGER.info(f"Execute {cmd}")
             msgs: bytes = b""
```

### Comparing `bluepy3-2.6.1/bluepy3/uuids.json` & `bluepy3-2.8.1/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.47.h` & `bluepy3-2.8.1/bluepy3/config/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.50.h` & `bluepy3-2.8.1/bluepy3/config/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.60.h` & `bluepy3-2.8.1/bluepy3/config/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.66.h` & `bluepy3-2.8.1/bluepy3/config/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.68.h` & `bluepy3-2.8.1/bluepy3/config/config.5.68.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.70.h` & `bluepy3-2.8.1/bluepy3/config/config.5.70.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.71.h` & `bluepy3-2.8.1/bluepy3/config/config.5.71.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.72.h` & `bluepy3-2.8.1/bluepy3/config/config.5.72.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.73.h` & `bluepy3-2.8.1/bluepy3/config/config.5.73.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/bluepy3/config/config.5.75.h` & `bluepy3-2.8.1/bluepy3/config/config.5.75.h`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/.gitignore` & `bluepy3-2.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/LICENSE` & `bluepy3-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/README.md` & `bluepy3-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `bluepy3-2.6.1/pyproject.toml` & `bluepy3-2.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bluepy3"
-version = "2.6.1"  # latest/current distribution version
-# version = "2.5.1"  # latest test version
+version = "2.8.1"  # latest/current distribution version
+# version = "2.7.5"  # latest test version
 description = "A Python3 module for interfacing with Bluetooth LE devices on Linux."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 # license-files = { paths = ["LICENSE"] }
 authors = [
     { name="Mausy5043" },
```

### Comparing `bluepy3-2.6.1/PKG-INFO` & `bluepy3-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bluepy3
-Version: 2.6.1
+Version: 2.8.1
 Summary: A Python3 module for interfacing with Bluetooth LE devices on Linux.
 Project-URL: Homepage, https://github.com/Mausy5043/bluepy3
 Project-URL: Bug Tracker, https://github.com/Mausy5043/bluepy3/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Keywords: BLE,Bluetooth,Bluetooth Low Energy,Bluetooth Smart,Raspberry Pi
```


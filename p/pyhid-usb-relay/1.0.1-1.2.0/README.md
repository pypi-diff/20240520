# Comparing `tmp/pyhid_usb_relay-1.0.1.tar.gz` & `tmp/pyhid_usb_relay-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhid_usb_relay-1.0.1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyhid_usb_relay-1.0.1.tar` & `pyhid_usb_relay-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0     4051 2023-10-31 16:07:03.929453 pyhid_usb_relay-1.0.1/README.md
--rw-r--r--   0        0        0      188 2023-10-31 16:07:03.929453 pyhid_usb_relay-1.0.1/pyhid_usb_relay/__init__.py
--rw-r--r--   0        0        0     4690 2023-10-31 16:07:03.929453 pyhid_usb_relay-1.0.1/pyhid_usb_relay/controller.py
--rw-r--r--   0        0        0      134 2023-10-31 16:07:03.929453 pyhid_usb_relay-1.0.1/pyhid_usb_relay/exceptions.py
--rw-r--r--   0        0        0     1872 2023-10-31 16:07:03.929453 pyhid_usb_relay-1.0.1/pyhid_usb_relay/find.py
--rw-r--r--   0        0        0     5339 2023-10-31 16:07:03.929453 pyhid_usb_relay-1.0.1/pyhid_usb_relay/main.py
--rw-r--r--   0        0        0      734 2023-10-31 16:07:03.929453 pyhid_usb_relay-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4944 1970-01-01 00:00:00.000000 pyhid_usb_relay-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/.flake8
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/.github/workflows/test.yaml
+-rwxr-xr-x   0        0        0      672 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/examples/test.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/__main__.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/controller.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/exceptions.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/find.py
+-rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/main.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/version.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/COPYING
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/README.md
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 pyhid_usb_relay-1.2.0/PKG-INFO
```

### Comparing `pyhid_usb_relay-1.0.1/README.md` & `pyhid_usb_relay-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,31 +5,14 @@
 # Installation
 
 The latest version can be installed using pip:
 ```
 python3 -m pip install pyhid-usb-relay
 ```
 
-## Manual Installation
-
-The library can be manually installed using [poetry](https://python-poetry.org/):
-```
-poetry install
-```
-
-From here, you can either run the `pyhid-usb-relay` command with:
-```
-poetry run pyhid-usb-relay
-```
-
-If you want to build a wheel for installation, run
-```
-poetry build
-```
-
 # Usage
 
 ## Standalone app outside of python
 ```shell
 pyhid-usb-relay --help
 ```
 
@@ -133,7 +116,19 @@
 The `pyhid-usb-relay` tool can be used to help resolve this by using the
 `get-serial` subcommand, which will fetch the HID serial number from the device
 with a udev rule that looks like:
 
 ```
 SUBSYSTEM=="usb", ATTR{idVendor}=="16c0", ATTR{idProduct}=="05df", ACTION=="add", PROGRAM="/usr/local/bin/pyhid-usb-relay get-serial '%E{BUSNUM}' '%E{DEVNUM}'", ENV{ID_SERIAL}:="%c"
 ```
+
+# Development
+
+Development of `pyhid-usb-relay` can be done inside of a virtual environment.
+To get started, create a virtual environment and then install the project in
+editable mode:
+
+```shell
+python3 -m venv .venv
+. .venv/bin/activate
+pip install -e ".[dev]"
+```
```

### Comparing `pyhid_usb_relay-1.0.1/pyhid_usb_relay/controller.py` & `pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 MAIN_REPORT = 0
 
 
 def xor(a, b):
     return bool(a) != bool(b)
 
 
+def bcd_to_int(b):
+    return (b & 0x0F) + ((b & 0xF0) >> 4) * 10
+
+
 class Controller(object):
     def __init__(self, device, timeout=5000):
         self.device = device
         self.timeout = timeout
         self.product = usb.util.get_string(device, device.iProduct)
         self.num_relays = int(self.product[8:])
 
@@ -44,14 +48,20 @@
             if self.serial in config:
                 self.aliases = config[self.serial].get("aliases", {})
                 self.defaults = config[self.serial].get("defaults", {})
 
         except FileNotFoundError:
             pass
 
+    @property
+    def version(self):
+        major = bcd_to_int(self.device.bcdDevice >> 8)
+        minor = bcd_to_int(self.device.bcdDevice & 0xFF)
+        return major, minor
+
     def get_property(self, relay, name, default=None):
         value = self.defaults.get(name, default)
         if relay != "all" and relay in self.aliases:
             value = self.aliases[relay].get(name, value)
         return value
 
     def set_serial(self, new_serial):
```

### Comparing `pyhid_usb_relay-1.0.1/pyhid_usb_relay/find.py` & `pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/find.py`

 * *Files identical despite different names*

### Comparing `pyhid_usb_relay-1.0.1/pyhid_usb_relay/main.py` & `pyhid_usb_relay-1.2.0/src/pyhid_usb_relay/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 # Copyright 2021 Joshua Watt <JPEWhacker@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import sys
 import time
-from pyhid_usb_relay import find, DeviceNotFoundError
+from . import find, DeviceNotFoundError, VERSION
 
 
 def main():
     def onoff(state):
         if state:
             return "on"
         return "off"
 
     def print_status(d):
-        print("Board ID=[%s] State: %02x" % (d.serial, d.state))
+        major, minor = d.version
+        print(
+            "Board ID=[%s] ver %d.%d, State: %02x" % (d.serial, major, minor, d.state)
+        )
 
     def pulse_sleep(d, relay):
         time.sleep(d.get_property(relay, "pulse-time", 1.0))
 
     def set_relay(args, value):
         device = find(serial=args.serial)
 
@@ -80,14 +83,15 @@
 
             device.set_serial(args.new_serial)
 
         except DeviceNotFoundError:
             return 1
 
     parser = argparse.ArgumentParser(description="USB HID Relay control")
+    parser.add_argument("--version", "-V", action="version", version=VERSION)
 
     subparser = parser.add_subparsers(title="Subcommands", dest="cmd")
     subparser.required = True
 
     enum_parser = subparser.add_parser("enum", help="Enumerate devices")
     enum_parser.set_defaults(func=relay_enum)
```

### Comparing `pyhid_usb_relay-1.0.1/PKG-INFO` & `pyhid_usb_relay-1.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,65 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyhid-usb-relay
-Version: 1.0.1
+Version: 1.2.0
 Summary: A tool for controlling USB HID relays
-Home-page: https://github.com/JPEWdev/pyhid-usb-relay
-License: MIT
-Author: Joshua Watt
-Author-email: JPEWhacker@gmail.com
-Requires-Python: >=3.8.0,<4.0
+Project-URL: Homepage, https://github.com/JPEWdev/pyhid-usb-relay
+Project-URL: Repository, https://github.com/JPEWdev/pyhid-usb-relay.git
+Project-URL: Issues, https://github.com/JPEWdev/pyhid-usb-relay/issues
+Author-email: Joshua Watt <JPEWhacker@gmail.com>
+Maintainer-email: Joshua Watt <JPEWhacker@gmail.com>
+License: Copyright 2020 Joshua Watt <JPEWhacker@gmail.com>
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of
+        this software and associated documentation files (the "Software"), to deal in
+        the Software without restriction, including without limitation the rights to
+        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+        of the Software, and to permit persons to whom the Software is furnished to do
+        so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: COPYING
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: libusb (>=1.0.26b5,<2.0.0) ; sys_platform == "win32"
-Requires-Dist: pyusb (>=1.2.1,<2.0.0)
-Requires-Dist: xdg (>=5.1.1,<6.0.0)
-Project-URL: Repository, https://github.com/JPEWdev/pyhid-usb-relay
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: libusb>=1.0.26b5; sys_platform == 'win32'
+Requires-Dist: pyusb>=1.2.1
+Requires-Dist: pyyaml>=6.0
+Requires-Dist: xdg>=5.1.1
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: pytest>=7.4; extra == 'dev'
 Description-Content-Type: text/markdown
 
 Python Utility for controlling HID USB Relays
 
 This utility is a Python version of [usb-relay-hid](https://github.com/pavel-a/usb-relay-hid)
 
 # Installation
 
 The latest version can be installed using pip:
 ```
 python3 -m pip install pyhid-usb-relay
 ```
 
-## Manual Installation
-
-The library can be manually installed using [poetry](https://python-poetry.org/):
-```
-poetry install
-```
-
-From here, you can either run the `pyhid-usb-relay` command with:
-```
-poetry run pyhid-usb-relay
-```
-
-If you want to build a wheel for installation, run
-```
-poetry build
-```
-
 # Usage
 
 ## Standalone app outside of python
 ```shell
 pyhid-usb-relay --help
 ```
 
@@ -157,7 +164,18 @@
 `get-serial` subcommand, which will fetch the HID serial number from the device
 with a udev rule that looks like:
 
 ```
 SUBSYSTEM=="usb", ATTR{idVendor}=="16c0", ATTR{idProduct}=="05df", ACTION=="add", PROGRAM="/usr/local/bin/pyhid-usb-relay get-serial '%E{BUSNUM}' '%E{DEVNUM}'", ENV{ID_SERIAL}:="%c"
 ```
 
+# Development
+
+Development of `pyhid-usb-relay` can be done inside of a virtual environment.
+To get started, create a virtual environment and then install the project in
+editable mode:
+
+```shell
+python3 -m venv .venv
+. .venv/bin/activate
+pip install -e ".[dev]"
+```
```


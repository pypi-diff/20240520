# Comparing `tmp/icp10125-0.0.1.tar.gz` & `tmp/icp10125-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/icp10125-0.0.1.tar", last modified: Tue Nov  2 09:28:33 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `icp10125-0.0.1.tar` & `icp10125-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-11-02 09:28:33.000000 icp10125-0.0.1/
--rw-r--r--   0 pi        (1000) pi        (1000)      109 2021-11-01 14:37:07.000000 icp10125-0.0.1/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)       31 2021-11-01 14:37:07.000000 icp10125-0.0.1/CHANGELOG.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-11-02 09:28:33.000000 icp10125-0.0.1/icp10125/
--rw-r--r--   0 pi        (1000) pi        (1000)     4518 2021-11-01 15:20:11.000000 icp10125-0.0.1/icp10125/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2288 2021-11-02 09:28:33.000000 icp10125-0.0.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1171 2021-11-02 09:23:27.000000 icp10125-0.0.1/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-11-02 09:28:33.000000 icp10125-0.0.1/icp10125.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)        9 2021-11-02 09:28:33.000000 icp10125-0.0.1/icp10125.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      261 2021-11-02 09:28:33.000000 icp10125-0.0.1/icp10125.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-11-02 09:28:33.000000 icp10125-0.0.1/icp10125.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     2288 2021-11-02 09:28:33.000000 icp10125-0.0.1/icp10125.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2021-11-02 09:28:33.000000 icp10125-0.0.1/icp10125.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       98 2021-11-01 14:37:07.000000 icp10125-0.0.1/pyproject.toml
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1388 2021-11-01 14:37:07.000000 icp10125-0.0.1/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2021-11-01 14:37:07.000000 icp10125-0.0.1/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1092 2021-11-02 09:28:33.000000 icp10125-0.0.1/setup.cfg
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 icp10125-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 icp10125-1.0.0/Makefile
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 icp10125-1.0.0/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 icp10125-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 icp10125-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 icp10125-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 icp10125-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 icp10125-1.0.0/uninstall.sh
+-rwxr-xr-x   0        0        0     1025 2020-02-02 00:00:00.000000 icp10125-1.0.0/examples/altitude.py
+-rwxr-xr-x   0        0        0     3360 2020-02-02 00:00:00.000000 icp10125-1.0.0/examples/bargraph.py
+-rwxr-xr-x   0        0        0      299 2020-02-02 00:00:00.000000 icp10125-1.0.0/examples/basic.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 icp10125-1.0.0/icp10125/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 icp10125-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 icp10125-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 icp10125-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 icp10125-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 icp10125-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 icp10125-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `icp10125-0.0.1/icp10125/__init__.py` & `icp10125-1.0.0/icp10125/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import time
 import struct
+import time
+
 from smbus2 import SMBus, i2c_msg
 
-__version__ = '0.0.1'
+__version__ = "1.0.0"
 
 NORMAL = 0x6825
 LOW_POWER = 0x609C
 LOW_NOISE = 0x70DF
 ULTRA_LOW_NOISE = 0x7866
 NORMAL_T_FIRST = 0x6825
 NORMAL_P_FIRST = 0x48A3
@@ -44,20 +45,20 @@
             address = DEFAULT_I2C_ADDRESS
         self.address = address
 
         self.bus = SMBus(1)
 
         chip_id = self.chip_id()
         if chip_id != CHIP_ID:
-            raise RuntimeError("ICP10125: Invalid Chip ID {:02x}, expected: {:02x}".format(chip_id, CHIP_ID))
+            raise RuntimeError(f"ICP10125: Invalid Chip ID {chip_id:02x}, expected: {CHIP_ID:02x}")
 
         self.read_otp()
 
     def rdwr(self, command, length=0, delay=0):
-        if type(command) is int:
+        if isinstance(command, int):
             msg_w = i2c_msg.write(self.address, struct.pack(">H", command))
         else:
             msg_w = i2c_msg.write(self.address, command)
 
         self.bus.i2c_rdwr(msg_w)
 
         time.sleep(delay / 1000.0)
@@ -67,32 +68,32 @@
             self.bus.i2c_rdwr(msg_r)
             if length == 1:
                 return list(msg_r)[0]
             else:
                 result = list(msg_r)
                 data = []
                 for chunk in range(0, len(result), 3):
-                    if self.crc8(result[chunk:chunk + 2]) != result[chunk + 2]:
+                    if self.crc8(result[chunk : chunk + 2]) != result[chunk + 2]:
                         raise ValueError("ICP10125: Invalid CRC8 in response.")
                     data.append((result[chunk] << 8) | result[chunk + 1])
                 if len(data) == 1:
                     return data[0]
                 else:
                     return data
 
         return []
 
     def chip_id(self):
         result = self.rdwr(READ_ID, 3)
-        return result & 0x3f
+        return result & 0x3F
 
     def read_otp(self):
         move_address_ptr = [
             MOVE_ADDRESS_PTR >> 8, MOVE_ADDRESS_PTR & 0xff,
-            0x00, 0x66, 0x9c  # Address CRC8
+            0x00, 0x66, 0x9C  # Address CRC8
         ]
         self.rdwr(move_address_ptr)
 
         for x in range(4):
             self.sensor_constants[x] = self.rdwr(READ_OTP, 3)
 
     def reset(self):
@@ -106,14 +107,17 @@
         temperature = result[0]
         pressure = (result[1] << 8) | (result[2] >> 8)
 
         self.process_data(pressure, temperature)
 
         return self.pressure, self.temperature
 
+    def calculate_altitude(self, pressure, qnh=1013.25):
+        return 44330.0 * (1.0 - pow(pressure / qnh, 1.0 / 5.255))
+
     def process_data(self, p_LSB, T_LSB):
         LUT_lower = 3.5 * (1 << 20)
         LUT_upper = 11.5 * (1 << 20)
         quadr_factor = 1.0 / 16777216.0
         offst_factor = 2048.0
 
         t = T_LSB - 32768
@@ -136,17 +140,17 @@
         p_LUT[1] * (p_Pa[2] - p_Pa[0]))
         A = (p_Pa[0] * p_LUT[0] - p_Pa[1] * p_LUT[1] - (p_Pa[1] - p_Pa[0]) * C) / (p_LUT[0] - p_LUT[1])
         B = (p_Pa[0] - A) * (p_LUT[0] + C)
 
         return A, B, C
 
     def crc8(self, data, polynomial=0x31):
-        result = 0xff
+        result = 0xFF
         for byte in data:
             result ^= byte
             for bit in range(8):
                 if result & 0x80:
                     result <<= 1
                     result ^= polynomial
                 else:
                     result <<= 1
-        return result & 0xff
+        return result & 0xFF
```

### Comparing `icp10125-0.0.1/setup.py` & `icp10125-1.0.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Copyright (c) 2016 Pimoroni
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Copyright (c) 2018 Pimoroni Ltd.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-"""
-
-from setuptools import setup, __version__
-from pkg_resources import parse_version
-
-minimum_version = parse_version('30.4.0')
-
-if parse_version(__version__) < minimum_version:
-    raise RuntimeError("Package setuptools must be at least version {}".format(minimum_version))
-
-setup()
```


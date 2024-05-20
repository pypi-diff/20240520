# Comparing `tmp/icm20948-0.0.2.tar.gz` & `tmp/icm20948-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/icm20948-0.0.2.tar", last modified: Tue Nov  3 16:00:04 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `icm20948-0.0.2.tar` & `icm20948-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-11-03 16:00:04.000000 icm20948-0.0.2/
--rw-r--r--   0 pi        (1000) pi        (1000)      109 2020-11-03 15:56:24.000000 icm20948-0.0.2/MANIFEST.in
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-11-03 16:00:04.000000 icm20948-0.0.2/icm20948/
--rw-r--r--   0 pi        (1000) pi        (1000)     9832 2020-11-03 15:56:59.000000 icm20948-0.0.2/icm20948/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      105 2020-11-03 15:56:24.000000 icm20948-0.0.2/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      820 2020-11-03 15:56:24.000000 icm20948-0.0.2/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)     1090 2020-11-03 16:00:04.000000 icm20948-0.0.2/setup.cfg
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2020-11-03 16:00:04.000000 icm20948-0.0.2/icm20948.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2020-11-03 16:00:04.000000 icm20948-0.0.2/icm20948.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2020-11-03 16:00:04.000000 icm20948-0.0.2/icm20948.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      246 2020-11-03 16:00:04.000000 icm20948-0.0.2/icm20948.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        9 2020-11-03 16:00:04.000000 icm20948-0.0.2/icm20948.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1818 2020-11-03 16:00:04.000000 icm20948-0.0.2/icm20948.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2020-11-03 13:59:50.000000 icm20948-0.0.2/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1818 2020-11-03 16:00:04.000000 icm20948-0.0.2/PKG-INFO
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1388 2020-11-03 15:56:24.000000 icm20948-0.0.2/setup.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 icm20948-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 icm20948-1.0.0/Makefile
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 icm20948-1.0.0/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 icm20948-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 icm20948-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 icm20948-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 icm20948-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 icm20948-1.0.0/uninstall.sh
+-rwxr-xr-x   0        0        0     3103 2020-02-02 00:00:00.000000 icm20948-1.0.0/examples/bargraph.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 icm20948-1.0.0/examples/magnetometer-to-rgb5x5.py
+-rwxr-xr-x   0        0        0     2575 2020-02-02 00:00:00.000000 icm20948-1.0.0/examples/magnetometer.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 icm20948-1.0.0/examples/read-all.py
+-rw-r--r--   0        0        0     9789 2020-02-02 00:00:00.000000 icm20948-1.0.0/icm20948/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 icm20948-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 icm20948-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 icm20948-1.0.0/tests/test_read.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 icm20948-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 icm20948-1.0.0/tests/tools.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 icm20948-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 icm20948-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 icm20948-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 icm20948-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `icm20948-0.0.2/icm20948/__init__.py` & `icm20948-1.0.0/icm20948/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import time
 import struct
+import time
 
-__version__ = '0.0.2'
+__version__ = '1.0.0'
 
 CHIP_ID = 0xEA
 I2C_ADDR = 0x68
 I2C_ADDR_ALT = 0x69
 ICM20948_BANK_SEL = 0x7f
 
 ICM20948_I2C_MST_ODR_CONFIG = 0x00
@@ -207,19 +207,19 @@
         self.bank(2)
         value = self.read(ICM20948_ACCEL_CONFIG) & 0b10001110
         if enabled:
             value |= 0b1
         value |= (mode & 0x07) << 4
         self.write(ICM20948_ACCEL_CONFIG, value)
 
-    def set_gyro_sample_rate(self, rate=100):
+    def set_gyro_sample_rate(self, rate=125):
         """Set the gyro sample rate in Hz."""
         self.bank(2)
-        # 100Hz sample rate - 1.1 kHz / (1 + rate)
-        rate = int((1100.0 / rate) - 1)
+        # 125Hz sample rate - 1.125 kHz / (1 + rate)
+        rate = int((1125.0 / rate) - 1)
         self.write(ICM20948_GYRO_SMPLRT_DIV, rate)
 
     def set_gyro_full_scale(self, scale=250):
         """Set the gyro full scale range to +- supplied value."""
         self.bank(2)
         value = self.read(ICM20948_GYRO_CONFIG_1) & 0b11111001
         value |= {250: 0b00, 500: 0b01, 1000: 0b10, 2000: 0b11}[scale] << 1
@@ -244,15 +244,15 @@
         return temperature_deg_c
 
     def __init__(self, i2c_addr=I2C_ADDR, i2c_bus=None):
         self._bank = -1
         self._addr = i2c_addr
 
         if i2c_bus is None:
-            from smbus import SMBus
+            from smbus2 import SMBus
             self._bus = SMBus(1)
         else:
             self._bus = i2c_bus
 
         self.bank(0)
         if not self.read(ICM20948_WHO_AM_I) == CHIP_ID:
             raise RuntimeError("Unable to find ICM20948")
@@ -291,15 +291,13 @@
 if __name__ == "__main__":
     imu = ICM20948()
 
     while True:
         x, y, z = imu.read_magnetometer_data()
         ax, ay, az, gx, gy, gz = imu.read_accelerometer_gyro_data()
 
-        print("""
-Accel: {:05.2f} {:05.2f} {:05.2f}
-Gyro:  {:05.2f} {:05.2f} {:05.2f}
-Mag:   {:05.2f} {:05.2f} {:05.2f}""".format(
-            ax, ay, az, gx, gy, gz, x, y, z
-        ))
+        print(f"""
+Accel: {ax:05.2f} {ay:05.2f} {az:05.2f}
+Gyro:  {gx:05.2f} {gy:05.2f} {gz:05.2f}
+Mag:   {x:05.2f} {y:05.2f} {z:05.2f}""")
 
         time.sleep(0.25)
```

### Comparing `icm20948-0.0.2/LICENSE.txt` & `icm20948-1.0.0/LICENSE`

 * *Files identical despite different names*


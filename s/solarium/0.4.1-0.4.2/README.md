# Comparing `tmp/solarium-0.4.1.tar.gz` & `tmp/solarium-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarium-0.4.1.tar", last modified: Sun May 19 15:48:30 2024, max compression
+gzip compressed data, was "solarium-0.4.2.tar", last modified: Mon May 20 14:15:56 2024, max compression
```

## Comparing `solarium-0.4.1.tar` & `solarium-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:48:30.489814 solarium-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 15:48:12.000000 solarium-0.4.1/.bandit
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-19 15:48:12.000000 solarium-0.4.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 15:48:12.000000 solarium-0.4.1/.fussyfox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:48:30.485814 solarium-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:48:30.489814 solarium-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 15:48:12.000000 solarium-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-19 15:48:12.000000 solarium-0.4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 15:48:12.000000 solarium-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 15:48:12.000000 solarium-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 15:48:12.000000 solarium-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-19 15:48:30.489814 solarium-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-19 15:48:12.000000 solarium-0.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-19 15:48:30.489814 solarium-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-19 15:48:12.000000 solarium-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:48:30.489814 solarium-0.4.1/solarium/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-19 15:48:12.000000 solarium-0.4.1/solarium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-19 15:48:12.000000 solarium-0.4.1/solarium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-19 15:48:12.000000 solarium-0.4.1/solarium/led.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 15:48:12.000000 solarium-0.4.1/solarium/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-19 15:48:12.000000 solarium-0.4.1/solarium/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:48:30.489814 solarium-0.4.1/solarium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-19 15:48:30.000000 solarium-0.4.1/solarium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-19 15:48:30.000000 solarium-0.4.1/solarium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:48:30.000000 solarium-0.4.1/solarium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 15:48:30.000000 solarium-0.4.1/solarium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 15:48:30.000000 solarium-0.4.1/solarium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 15:48:30.000000 solarium-0.4.1/solarium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:15:56.592852 solarium-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 14:15:36.000000 solarium-0.4.2/.bandit
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-20 14:15:36.000000 solarium-0.4.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 14:15:36.000000 solarium-0.4.2/.fussyfox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:15:56.588852 solarium-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:15:56.588852 solarium-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 14:15:36.000000 solarium-0.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-20 14:15:36.000000 solarium-0.4.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-20 14:15:36.000000 solarium-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 14:15:36.000000 solarium-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 14:15:36.000000 solarium-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-20 14:15:56.592852 solarium-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-20 14:15:36.000000 solarium-0.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-20 14:15:56.592852 solarium-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-20 14:15:36.000000 solarium-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:15:56.588852 solarium-0.4.2/solarium/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 14:15:36.000000 solarium-0.4.2/solarium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-20 14:15:36.000000 solarium-0.4.2/solarium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-20 14:15:36.000000 solarium-0.4.2/solarium/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-20 14:15:36.000000 solarium-0.4.2/solarium/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-20 14:15:36.000000 solarium-0.4.2/solarium/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:15:56.592852 solarium-0.4.2/solarium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-20 14:15:56.000000 solarium-0.4.2/solarium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-20 14:15:56.000000 solarium-0.4.2/solarium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:15:56.000000 solarium-0.4.2/solarium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 14:15:56.000000 solarium-0.4.2/solarium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 14:15:56.000000 solarium-0.4.2/solarium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 14:15:56.000000 solarium-0.4.2/solarium.egg-info/top_level.txt
```

### Comparing `solarium-0.4.1/.github/workflows/ci.yml` & `solarium-0.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/.github/workflows/release.yml` & `solarium-0.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/.gitignore` & `solarium-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/LICENSE` & `solarium-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/PKG-INFO` & `solarium-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarium
-Version: 0.4.1
+Version: 0.4.2
 Summary: RaspberryPi based LED controller for artificial sunlight
 Home-page: https://github.com/codingjoe/solarium
 Author: Johannes Maron
 Author-email: info@johanneshoppe.com
 License: MIT
 Keywords: led,raspberrypi
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `solarium-0.4.1/README.rst` & `solarium-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/setup.cfg` & `solarium-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/solarium/__main__.py` & `solarium-0.4.2/solarium/__main__.py`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/solarium/led.py` & `solarium-0.4.2/solarium/led.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,23 +73,25 @@
 
 
 def init(
     host="localhost",
     warm_pin=12,
     cold_pin=13,
     power_pin=17,
-    power_led_pin=25,
+    power_led_pin=26,
     frequency=100,
 ):
     logger.debug("warm LED: %s:%d@%dHz", host, warm_pin, frequency)
     logger.debug("cold LED: %s:%d@%dHz", host, cold_pin, frequency)
     factory = PiGPIOFactory(host=host)
 
     power_led = gpiozero.LED(power_led_pin, pin_factory=factory)
-    power_button = PowerToggle(power_pin, pin_factory=factory, power_led=power_led)
+    power_button = PowerToggle(
+        power_pin, pin_factory=factory, power_led=power_led, bounce_time=1
+    )
     power_button.when_pressed = lambda: power_button.toggle()
     warm = PWMLED(warm_pin, name="warm", power_state=power_button, pin_factory=factory)
     cold = PWMLED(cold_pin, name="cold", power_state=power_button, pin_factory=factory)
     warm.frequency = frequency
     cold.frequency = frequency
 
     return warm, cold, power_button
```

### Comparing `solarium-0.4.1/solarium/player.py` & `solarium-0.4.2/solarium/player.py`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/solarium/utils.py` & `solarium-0.4.2/solarium/utils.py`

 * *Files identical despite different names*

### Comparing `solarium-0.4.1/solarium.egg-info/PKG-INFO` & `solarium-0.4.2/solarium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarium
-Version: 0.4.1
+Version: 0.4.2
 Summary: RaspberryPi based LED controller for artificial sunlight
 Home-page: https://github.com/codingjoe/solarium
 Author: Johannes Maron
 Author-email: info@johanneshoppe.com
 License: MIT
 Keywords: led,raspberrypi
 Classifier: License :: OSI Approved :: MIT License
```


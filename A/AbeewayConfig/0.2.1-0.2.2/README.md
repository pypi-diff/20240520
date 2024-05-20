# Comparing `tmp/abeewayconfig-0.2.1.tar.gz` & `tmp/abeewayconfig-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abeewayconfig-0.2.1.tar", last modified: Sun May 19 01:51:44 2024, max compression
+gzip compressed data, was "abeewayconfig-0.2.2.tar", last modified: Mon May 20 13:22:43 2024, max compression
```

## Comparing `abeewayconfig-0.2.1.tar` & `abeewayconfig-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-19 01:51:44.692732 abeewayconfig-0.2.1/
--rw-r--r--   0 lucas     (1000) lucas     (1000)    35149 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/LICENSE
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1414 2024-05-19 01:51:44.692732 abeewayconfig-0.2.1/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1051 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/README.md
--rw-r--r--   0 lucas     (1000) lucas     (1000)       38 2024-05-19 01:51:44.692732 abeewayconfig-0.2.1/setup.cfg
--rw-r--r--   0 lucas     (1000) lucas     (1000)      753 2024-05-19 01:51:22.000000 abeewayconfig-0.2.1/setup.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-19 01:51:44.689399 abeewayconfig-0.2.1/src/
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-19 01:51:44.689399 abeewayconfig-0.2.1/src/AbeewayConfig/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1881 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/Config.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     2259 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/Device.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)       32 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4769 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/abeewayconfig.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4026 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/smartbadgecfgdict.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-19 01:51:44.692732 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1414 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)      434 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       67 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       12 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       14 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.2/LICENSE
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1414 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1051 2024-05-16 14:51:58.000000 abeewayconfig-0.2.2/README.md
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/setup.cfg
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      753 2024-05-20 13:22:06.000000 abeewayconfig-0.2.2/setup.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/src/
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/src/AbeewayConfig/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     2248 2024-05-20 13:12:46.000000 abeewayconfig-0.2.2/src/AbeewayConfig/Config.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     2261 2024-05-20 13:16:13.000000 abeewayconfig-0.2.2/src/AbeewayConfig/Device.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.2/src/AbeewayConfig/__init__.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4788 2024-05-20 13:14:44.000000 abeewayconfig-0.2.2/src/AbeewayConfig/abeewayconfig.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.2/src/AbeewayConfig/smartbadgecfgdict.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1414 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      434 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       67 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       12 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/top_level.txt
```

### Comparing `abeewayconfig-0.2.1/LICENSE` & `abeewayconfig-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.1/PKG-INFO` & `abeewayconfig-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.1
+Version: 0.2.2
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `abeewayconfig-0.2.1/README.md` & `abeewayconfig-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.1/setup.py` & `abeewayconfig-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="AbeewayConfig",
-    version="0.2.1",
+    version="0.2.2",
     description="Abeeway configuration tool",
     author="João Lucas",
     url="https://github.com/jlabbude/AbeewayConfig",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "pyserial",
```

### Comparing `abeewayconfig-0.2.1/src/AbeewayConfig/Config.py` & `abeewayconfig-0.2.2/src/AbeewayConfig/Config.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,20 @@
         with open(config_file, 'r') as config:
             for line in config:
                 config_parameter_cfg = Config.get_config_parameter_from_cfg(line)
                 config_value_cfg = Config.get_config_value_from_cfg(config_parameter_cfg, line)
                 config_name = config_dict.get(config_parameter_cfg)
                 if config_parameter_cfg is not None or config_value_cfg is not None:
                     config_value_dev = Device.get_config_value_from_dev(device_config, config_name)
+
+                    if config_parameter_cfg is 249 and config_value_dev is 5:
+                        console_output.insert(tk.END, f"Config error: {deveui} \n")
+                        console_output.insert(tk.END, f"An error occurred. Please try starting the device, then configuring again. \n")
+                        return False
+
                     if config_value_cfg != config_value_dev:
                         console_output.insert(tk.END, f"Config error: {deveui} \n")
-                        console_output.insert(tk.END, f"[{config_name} : {config_value_cfg}] -> [{config_value_dev}] \n")
+                        console_output.insert(tk.END, f"[Parameter : {config_name}] - Current: [{config_value_dev}] | Correct: [{config_value_cfg}] \n")
                         return False
 
         console_output.insert(tk.END, f"Done: {deveui} \n")
         return True
-
```

### Comparing `abeewayconfig-0.2.1/src/AbeewayConfig/Device.py` & `abeewayconfig-0.2.2/src/AbeewayConfig/Device.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,18 @@
             ser.write(b'system buzzer 6\r')
             ser.close()
 
     # This doesn't actually talk to the device directly, rather it just grabs the value from a string
     # Might move it back to the main module
     def get_config_value_from_dev(config_name: str, parameter: int) -> int:
         if parameter is not None:
-            match_line = re.search(r".*%s\s*=\s*(-?\d+)" % parameter, config_name)
+            match_line = re.search(r".* %s\s*=\s*(-?\d+)" % parameter, config_name)
             if match_line is not None:
                 return int(match_line.group(1))
 
     def config_show_at_device(serial_port: str, br: int) -> str:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
             ser.write(b'config show\r')
-            output = ser.read(8000)
+            output = ser.read(16000)
             ser.close()
             return output.decode('utf-8')
```

### Comparing `abeewayconfig-0.2.1/src/AbeewayConfig/abeewayconfig.py` & `abeewayconfig-0.2.2/src/AbeewayConfig/abeewayconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import shutil
 import sys
-import time
+from time import sleep
 import serial.tools.list_ports
 import tkinter as tk
 from glob import glob
 from platform import system
 from threading import Thread
 from tkinter import filedialog, Button, Text
 
@@ -68,19 +68,20 @@
 
 
 def config_process(console_output) -> None:
     # Hacky way of detecting new badges after the program has already started
     define_os_specific_params()
 
     serial_parallel_process(target=Device.start_dev)
+    sleep(5)
 
     serial_parallel_process(target=Device.set_config_on_device)
 
     discrepancy_parallel_process(target=Config.check_config_discrepancy, console_output=console_output)
-    time.sleep(5)
+    sleep(5)
 
     serial_parallel_process(target=Device.reset_dev)
 
 
 def main():
     define_os_specific_params()
     root = tk.Tk()
```

### Comparing `abeewayconfig-0.2.1/src/AbeewayConfig/smartbadgecfgdict.py` & `abeewayconfig-0.2.2/src/AbeewayConfig/smartbadgecfgdict.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/PKG-INFO` & `abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.1
+Version: 0.2.2
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


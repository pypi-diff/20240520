# Comparing `tmp/pyuptech-0.1.5.tar.gz` & `tmp/pyuptech-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.5.tar", last modified: Mon May 20 13:13:05 2024, max compression
+gzip compressed data, was "pyuptech-0.1.5.1.tar", last modified: Mon May 20 14:14:49 2024, max compression
```

## Comparing `pyuptech-0.1.5.tar` & `pyuptech-0.1.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     8846 2024-05-20 13:12:45.680397 pyuptech-0.1.5/README.md
--rw-r--r--   0        0        0      545 2024-05-20 13:13:05.792607 pyuptech-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1230 2024-05-20 13:12:45.680397 pyuptech-0.1.5/src/pyuptech/__init__.py
--rw-r--r--   0        0        0   219512 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/lib/libuptech.so
--rw-r--r--   0        0        0      190 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     2060 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/emulation.py
--rw-r--r--   0        0        0     1007 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1761 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    10688 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0    13793 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     6240 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0      252 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      371 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/display_tests.py
--rw-r--r--   0        0        0     1036 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/perf_tests.py
--rw-r--r--   0        0        0     1220 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/test_sensor.py
--rw-r--r--   0        0        0      424 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/utils.py
--rw-r--r--   0        0        0     9161 1970-01-01 00:00:00.000000 pyuptech-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     8829 2024-05-20 14:14:30.990193 pyuptech-0.1.5.1/README.md
+-rw-r--r--   0        0        0      547 2024-05-20 14:14:49.222094 pyuptech-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1148 2024-05-20 14:14:30.990193 pyuptech-0.1.5.1/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      190 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     2060 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/emulation.py
+-rw-r--r--   0        0        0     1007 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1761 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10688 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0    13793 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     6515 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0      252 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      456 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/display_tests.py
+-rw-r--r--   0        0        0     1036 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/perf_tests.py
+-rw-r--r--   0        0        0     1220 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/test_sensor.py
+-rw-r--r--   0        0        0      424 2024-05-20 14:14:30.994193 pyuptech-0.1.5.1/tests/utils.py
+-rw-r--r--   0        0        0     9146 1970-01-01 00:00:00.000000 pyuptech-0.1.5.1/PKG-INFO
```

### Comparing `pyuptech-0.1.5/README.md` & `pyuptech-0.1.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -197,26 +197,27 @@
 
 ## 调试
 
 通过 `tools.display` 可以将传感器数据打印到终端或者主板板载LCD屏幕上
 
 ```python
 from pyuptech import (
-    set_emulation_mode,
+    SensorEmulator,
     mpu_display_on_lcd,
-    mpu_display_on_console,
+    make_mpu_table,
     adc_io_display_on_lcd,
-    adc_io_display_on_console)
+    make_adc_io_table,
+    Screen)
 
-# 关闭模拟模式，不关闭将无法进行正常的实机运行
-set_emulation_mode("off")
+emu = SensorEmulator()
+scr = Screen(screen_dir=2)
 
-mpu_display_on_console()  # 将MPU6500数据打印到终端
+print(make_mpu_table(sensors=emu))
 
-mpu_display_on_lcd(mode="acc")  # 将MPU6500加速度数据打印到LCD
+mpu_display_on_lcd(sensors=emu, screen=scr, mode="acc")  # 将MPU6500加速度数据打印到LCD
 
 # 定义ADC标签索引字典，可以空缺部分键值
 adc_labels = {
     6: 'EDGE_FL',
     7: "EDGE_RL",
     2: 'EDGE_FR',
     1: 'EDGE_RR',
@@ -231,17 +232,17 @@
     2: "gray r",
 
     7: 'ftl',
     6: 'ftr',
     5: 'rtr'
 }
 
-adc_io_display_on_lcd(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
+adc_io_display_on_lcd(sensors=emu, screen=scr, adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
 
-adc_io_display_on_console(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
+make_adc_io_table(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
 
 
 ```
 
 ## 使用传感器仿真器
 
 通过 `modules.emulation.SensorEmulator` 可以使用传感器仿真器
@@ -262,20 +263,23 @@
 
 ```
 
 配合 `modules.display` 使用
 
 ```python
 from pyuptech import (
-    set_emulation_mode,
-    mpu_display_on_console,
-    adc_io_display_on_console)
+    Screen, SensorEmulator,
+    make_mpu_table,
+    make_adc_io_table)
 
 # 启动模拟模式，以便打印可以正常使用随机生成的数据进行工作
-set_emulation_mode("on")
+scr = Screen()
+emu = SensorEmulator()
 
-mpu_display_on_console()  # 将MPU6500数据打印到终端
+print(make_mpu_table(sensors=emu))
+# 将MPU6500数据打印到终端
 
-adc_io_display_on_console()  # 将ADC和GPIO数据打印到终端
+print(make_adc_io_table(sensors=emu))
+# 将ADC和GPIO数据打印到终端
 
 ```
```

### Comparing `pyuptech-0.1.5/pyproject.toml` & `pyuptech-0.1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyuptech"
-version = "0.1.5"
+version = "0.1.5.1"
 description = "A Python wrapper for the uptech binary lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "terminaltables>=3.1.10",
```

### Comparing `pyuptech-0.1.5/src/pyuptech/__init__.py` & `pyuptech-0.1.5.1/src/pyuptech/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,19 +11,18 @@
     PinModeSetter,
     IndexedGetter,
     IndexedSetter,
 )
 from .modules.screen import Screen, Color, FontSize
 from .modules.sensors import OnBoardSensors, ADCArrayType, MPUArrayType
 from .tools.display import (
-    set_emulation_mode,
     adc_io_display_on_lcd,
-    adc_io_display_on_console,
+    make_adc_io_table,
     mpu_display_on_lcd,
-    mpu_display_on_console,
+    make_mpu_table,
 )
 
 __all__ = [
     "OnBoardSensors",
     "SensorEmulator",
     "Screen",
     "Color",
@@ -38,13 +37,12 @@
     "MPUArrayType",
     "PinGetter",
     "PinSetter",
     "PinModeSetter",
     "IndexedGetter",
     "IndexedSetter",
     # tools
-    "set_emulation_mode",
     "adc_io_display_on_lcd",
-    "adc_io_display_on_console",
+    "make_adc_io_table",
     "mpu_display_on_lcd",
-    "mpu_display_on_console",
+    "make_mpu_table",
 ]
```

### Comparing `pyuptech-0.1.5/src/pyuptech/lib/libuptech.so` & `pyuptech-0.1.5.1/src/pyuptech/lib/libuptech.so`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/src/pyuptech/modules/emulation.py` & `pyuptech-0.1.5.1/src/pyuptech/modules/emulation.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/src/pyuptech/modules/loader.py` & `pyuptech-0.1.5.1/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/src/pyuptech/modules/logger.py` & `pyuptech-0.1.5.1/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/src/pyuptech/modules/pins.py` & `pyuptech-0.1.5.1/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/src/pyuptech/modules/screen.py` & `pyuptech-0.1.5.1/src/pyuptech/modules/screen.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.5.1/src/pyuptech/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/src/pyuptech/tools/display.py` & `pyuptech-0.1.5.1/src/pyuptech/tools/display.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,23 @@
 import time
 from typing import Literal, Dict
 
-from ..modules.emulation import SensorEmulator
 from ..modules.screen import Screen, Color, FontSize
 from ..modules.sensors import OnBoardSensors
 
-sensors: OnBoardSensors | SensorEmulator | None = None
-screen: Screen | None = None
 
-
-def set_emulation_mode(mode: Literal["on", "off"]):
-    """
-    Sets the emulation mode of the sensors.
-
-    Args:
-        mode (Literal["on", "off"]): The emulation mode to set. Must be either "on" or "off".
-
-    Returns:
-        None
-
-    This function sets the emulation mode of the sensors. If the mode is "on", it creates a new instance of the SensorEmulator class and assigns it to the global variable "sensors". If the mode is "off", it creates a new instance of the OnBoardSensors class and assigns it to the global variable "sensors".
-
-    Raises:
-        None
-    """
-    global sensors, screen
-    match mode:
-        case "on":
-            #  仿真器不需要启动adc-io等硬件设备
-            sensors = SensorEmulator()
-            screen = None  # 仿真模式下，假设屏幕是脱机的
-        case "off":
-            sensors = (
-                OnBoardSensors()
-                .adc_io_open()
-                .set_all_io_mode(0)
-                .set_all_io_level(1)
-                .MPU6500_Open()
-            )
-            screen = (
-                Screen()
-                .open()
-                .fill_screen(Color.BLACK)
-                .refresh()
-                .set_led_color(0, Color.BROWN)
-                .set_led_color(1, Color.GRED)
-            )
-
-
-def mpu_display_on_lcd(mode: Literal["atti", "acc", "gyro"]):
+def mpu_display_on_lcd(
+    screen: Screen, sensors: OnBoardSensors, mode: Literal["atti", "acc", "gyro"]
+):
     """
     Display the specified mode on the screen.
 
     Parameters:
+        screen: An instance of the `Screen` class.
+        sensors: An instance of the `OnBoardSensors` class.
         mode (Literal["atti", "acc", "gyro"]): The mode to display.
 
     Returns:
         None
     """
     match mode:
         case "atti":
@@ -73,98 +34,119 @@
             accel = sensors.acc_all()
             screen.put_string(0, 30, f"ACC X :{accel[0]:.2f}")
             screen.put_string(0, 44, f"ACC Y :{accel[1]:.2f}")
             screen.put_string(0, 54, f"ACC Z :{accel[2]:.2f}")
     screen.refresh()
 
 
-def mpu_display_on_console():
+def make_mpu_table(sensors: OnBoardSensors) -> str:
     """
-    Display the MPU data in a formatted table in the terminal.
+    Generate and return a formatted string containing a table with accelerometer, gyroscope, and attitude information.
 
-    This function combines the ACC, GYRO, and ATTI data into a structured list and creates a table using the
-    `terminaltables` library. The table is then printed to the console.
+    This function extracts acceleration, gyroscope, and attitude data from sensor readings and formats it into an
+    aesthetically pleasing table, displaying the values for each axis of acceleration, gyroscope, and attitude angles.
+
+    Parameters:
+        sensors: An instance of the `OnBoardSensors` class.
 
+    Returns:
+        str: A formatted table string.
     """
     from terminaltables import DoubleTable
 
-    # Combine data into one structured list
+    # Initialize the data list to store table data
     combined_data = [
         ["ACC", "Value", "GYRO", "Value", "ATTI", "Value"],
     ]
     acc_names = ["X_ACC", "Y_ACC", "Z_ACC"]
 
     gyro_names = ["X_GYRO", "Y_GYRO", "Z_GYRO"]
 
     atti_names = ["Pitch", "Roll", "Yaw"]
+    # Iterate through acceleration, gyroscope, and attitude data, adding them to the combined_data list
     for i in range(len(acc_names)):
         combined_data.append(
             [
                 acc_names[i],
-                f"{sensors.acc_all()[i]:.2f}",
+                f"{sensors.acc_all()[i]:.2f}",  # Acceleration value
                 gyro_names[i],
-                f"{sensors.gyro_all()[i]:.2f}",
+                f"{sensors.gyro_all()[i]:.2f}",  # Gyroscope value
                 atti_names[i],
-                f"{sensors.atti_all()[i]:.2f}",
+                f"{sensors.atti_all()[i]:.2f}",  # Attitude value
             ]
         )
 
-    # Create and print the table
+    # Create a table using the DoubleTable class and customize its style
     table = DoubleTable(combined_data)
-    table.inner_row_border = True  # Add inner row borders for clarity
-    print(table.table)
+    table.inner_row_border = True  # Add inner row borders for improved readability
+    return table.table
 
 
-def adc_io_display_on_console(
-    adc_labels: Dict[int, str] = None, io_labels: Dict[int, str] = None
-):
+def make_adc_io_table(
+    sensors: OnBoardSensors,
+    adc_labels: Dict[int, str] = None,
+    io_labels: Dict[int, str] = None,
+) -> str:
     """
-    Displays ADC and IO channel values on the console using the terminaltables library.
+    Generate and return a formatted string table containing ADC (Analog-to-Digital Converter) and IO (Input/Output) channel information.
 
-    Args:
-        adc_labels (Dict[int, str], optional): A dictionary mapping ADC channel indices to custom labels. Defaults to None.
-        io_labels (Dict[int, str], optional): A dictionary mapping IO channel indices to custom labels. Defaults to None.
+    Parameters:
+        sensors: An instance of the `OnBoardSensors` class.
+        adc_labels: A dictionary mapping ADC channel numbers (int) to custom names (str). Defaults to None, indicating no custom names are used.
+        io_labels: A dictionary mapping IO channel numbers (int) to custom names (str). Defaults to None, indicating no custom names are used.
 
     Returns:
-        None
-
-    Raises:
-        None
-
+        A string representation of the table, formatted using the terminaltables library.
 
+    Dependencies:
+        This function relies on external functions `adc_all_channels()`, `io_all_channels()`, and `get_all_io_mode()` from the `sensors` module.
     """
-    from terminaltables import DoubleTable
 
+    from terminaltables import (
+        DoubleTable,
+    )  # Import library for formatting the table output
+
+    # Use empty dictionaries as default values if adc_labels or io_labels are not provided
     adc_labels = adc_labels or {}
     io_labels = io_labels or {}
+
+    # Retrieve all ADC and IO channel data from the sensors module
     adc = sensors.adc_all_channels()
     io = sensors.io_all_channels()
     io_modes = sensors.get_all_io_mode()
 
+    # Construct the rows of the table
     rows = [
-        ["ADC Name"] + ([adc_labels.get(i, f"ADC{i}") for i in range(10)]),
-        ["ADC Data"] + [f"{x}" for x in adc],
-        ["IO Name"] + ([io_labels.get(i, f"IO{i}") for i in range(8)]),
-        ["IO Data"] + [int(bit) for bit in f"{io:08b}"],
-        ["IO Mode"] + [int(bit) for bit in f"{io_modes:08b}"],
+        ["ADC Name"]
+        + [adc_labels.get(i, f"ADC{i}") for i in range(10)],  # ADC Name row
+        ["ADC Data"] + [f"{x}" for x in adc],  # ADC Data row
+        ["IO Name"] + [io_labels.get(i, f"IO{i}") for i in range(8)],  # IO Name row
+        ["IO Data"] + [int(bit) for bit in f"{io:08b}"],  # IO Data row (binary)
+        ["IO Mode"] + [int(bit) for bit in f"{io_modes:08b}"],  # IO Mode row (binary)
     ]
+
+    # Format the row data into a table using DoubleTable class
     table = DoubleTable(rows)
-    table.inner_row_border = True
-    print(table.table)
+    table.inner_row_border = True  # Enable inner row borders
+    return table.table  # Return the formatted table string
 
 
 def adc_io_display_on_lcd(
+    sensors: OnBoardSensors,
+    screen: Screen,
     interval: float = 0.01,
     adc_labels: Dict[int, str] = None,
     io_labels: Dict[int, str] = None,
 ):
     """
     Reads sensor values from ADC and IO channels and displays them on the screen.
 
     Args:
+        sensors: An instance of the `OnBoardSensors` class.
+        screen: An instance of the `Screen` class.
         interval (float, optional): The time interval between sensor readings in seconds. Defaults to 0.01.
         adc_labels (Dict[int, str], optional): A dictionary mapping ADC channel indices to custom labels. Defaults to None.
         io_labels (Dict[int, str], optional): A dictionary mapping IO channel indices to custom labels. Defaults to None.
 
     Returns:
         None
```

### Comparing `pyuptech-0.1.5/tests/perf_tests.py` & `pyuptech-0.1.5.1/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/tests/test_sensor.py` & `pyuptech-0.1.5.1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.5/PKG-INFO` & `pyuptech-0.1.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
@@ -208,26 +208,27 @@
 
 ## 调试
 
 通过 `tools.display` 可以将传感器数据打印到终端或者主板板载LCD屏幕上
 
 ```python
 from pyuptech import (
-    set_emulation_mode,
+    SensorEmulator,
     mpu_display_on_lcd,
-    mpu_display_on_console,
+    make_mpu_table,
     adc_io_display_on_lcd,
-    adc_io_display_on_console)
+    make_adc_io_table,
+    Screen)
 
-# 关闭模拟模式，不关闭将无法进行正常的实机运行
-set_emulation_mode("off")
+emu = SensorEmulator()
+scr = Screen(screen_dir=2)
 
-mpu_display_on_console()  # 将MPU6500数据打印到终端
+print(make_mpu_table(sensors=emu))
 
-mpu_display_on_lcd(mode="acc")  # 将MPU6500加速度数据打印到LCD
+mpu_display_on_lcd(sensors=emu, screen=scr, mode="acc")  # 将MPU6500加速度数据打印到LCD
 
 # 定义ADC标签索引字典，可以空缺部分键值
 adc_labels = {
     6: 'EDGE_FL',
     7: "EDGE_RL",
     2: 'EDGE_FR',
     1: 'EDGE_RR',
@@ -242,17 +243,17 @@
     2: "gray r",
 
     7: 'ftl',
     6: 'ftr',
     5: 'rtr'
 }
 
-adc_io_display_on_lcd(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
+adc_io_display_on_lcd(sensors=emu, screen=scr, adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到LCD 
 
-adc_io_display_on_console(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
+make_adc_io_table(adc_labels=adc_labels, io_labels=io_labels)  # 将ADC和GPIO数据打印到终端 
 
 
 ```
 
 ## 使用传感器仿真器
 
 通过 `modules.emulation.SensorEmulator` 可以使用传感器仿真器
@@ -273,20 +274,23 @@
 
 ```
 
 配合 `modules.display` 使用
 
 ```python
 from pyuptech import (
-    set_emulation_mode,
-    mpu_display_on_console,
-    adc_io_display_on_console)
+    Screen, SensorEmulator,
+    make_mpu_table,
+    make_adc_io_table)
 
 # 启动模拟模式，以便打印可以正常使用随机生成的数据进行工作
-set_emulation_mode("on")
+scr = Screen()
+emu = SensorEmulator()
 
-mpu_display_on_console()  # 将MPU6500数据打印到终端
+print(make_mpu_table(sensors=emu))
+# 将MPU6500数据打印到终端
 
-adc_io_display_on_console()  # 将ADC和GPIO数据打印到终端
+print(make_adc_io_table(sensors=emu))
+# 将ADC和GPIO数据打印到终端
 
 ```
```


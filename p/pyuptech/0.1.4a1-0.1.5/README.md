# Comparing `tmp/pyuptech-0.1.4a1.tar.gz` & `tmp/pyuptech-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.4a1.tar", last modified: Sun Apr 21 11:35:46 2024, max compression
+gzip compressed data, was "pyuptech-0.1.5.tar", last modified: Mon May 20 13:13:05 2024, max compression
```

## Comparing `pyuptech-0.1.4a1.tar` & `pyuptech-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     8297 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/README.md
--rw-r--r--   0        0        0      547 2024-04-21 11:35:46.454119 pyuptech-0.1.4a1/pyproject.toml
--rw-r--r--   0        0        0     1280 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/__init__.py
--rw-r--r--   0        0        0   219512 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/lib/libuptech.so
--rw-r--r--   0        0        0      110 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     2043 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/modules/emulation.py
--rw-r--r--   0        0        0     1096 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      577 2024-04-21 11:35:28.293904 pyuptech-0.1.4a1/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0     1761 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/src/pyuptech/modules/pins.py
--rw-r--r--   0        0        0    10454 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0    11278 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0     6148 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/src/pyuptech/tools/display.py
--rw-r--r--   0        0        0      252 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/tests/__init__.py
--rw-r--r--   0        0        0      386 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/tests/display_tests.py
--rw-r--r--   0        0        0     1036 2024-04-21 11:35:28.297904 pyuptech-0.1.4a1/tests/perf_tests.py
--rw-r--r--   0        0        0     8614 1970-01-01 00:00:00.000000 pyuptech-0.1.4a1/PKG-INFO
+-rw-r--r--   0        0        0     8846 2024-05-20 13:12:45.680397 pyuptech-0.1.5/README.md
+-rw-r--r--   0        0        0      545 2024-05-20 13:13:05.792607 pyuptech-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1230 2024-05-20 13:12:45.680397 pyuptech-0.1.5/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0   219512 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/lib/libuptech.so
+-rw-r--r--   0        0        0      190 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     2060 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/emulation.py
+-rw-r--r--   0        0        0     1007 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1761 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10688 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0    13793 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0     6240 2024-05-20 13:12:45.684397 pyuptech-0.1.5/src/pyuptech/tools/display.py
+-rw-r--r--   0        0        0      252 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      371 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/display_tests.py
+-rw-r--r--   0        0        0     1036 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/perf_tests.py
+-rw-r--r--   0        0        0     1220 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/test_sensor.py
+-rw-r--r--   0        0        0      424 2024-05-20 13:12:45.684397 pyuptech-0.1.5/tests/utils.py
+-rw-r--r--   0        0        0     9161 1970-01-01 00:00:00.000000 pyuptech-0.1.5/PKG-INFO
```

### Comparing `pyuptech-0.1.4a1/README.md` & `pyuptech-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,31 @@
 ---
 
 # 安装
 
 使用`pdm`安装
 
 ```shell
+# 安装pdm
+python -m pip install pdm
+
+# 切换源
+pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
+
+# 安装pyuptech
 pdm add pyuptech
+
+# 或者安装不稳定版
+pdm add pyuptech --pre
+
 ```
 
 ## OnBoardSensors
 
-**简介**
-
-`OnBoardSensors`是一个Python类，封装了对嵌入式硬件板载传感器和输入/输出接口的操作，如ADC、GPIO以及MPU6500六轴传感器。该类通过ctypes库调用预编译的C库函数实现底层硬件交互。
+> `OnBoardSensors`是一个Python类，封装了对嵌入式硬件板载传感器和输入/输出接口的操作，如ADC、GPIO以及MPU6500六轴传感器。该类通过ctypes库调用预编译的C库函数实现底层硬件交互。
 
 ### 类方法概览
 
 - **初始化**: 初始化所有IO通道模式为输入，并设置初始电平为高，同时初始化ADC插件。
 
 - **ADC操作**:
     - `adc_min_sample_interval_ms`: 获取和设置ADC采样间隔（以毫秒为单位，内部存储为纳秒）。
@@ -44,44 +53,53 @@
 - 获取ADC和GPIO的数据。
 - 初始化和读取MPU6500六轴传感器数据。
 
 ### QUICKSTART
 
 ```python
 from pyuptech import OnBoardSensors
-from ctypes import c_uint8, Array
+from typing import Tuple
 
 # 创建OnBoardSensors对象，设置模拟量传感器最小采样间隔为5ms
 sensor_controller = OnBoardSensors(adc_min_sample_interval_ms=5)
 
 # 初始化ADC,设置所有GPIO引脚为输入，设置初始电平为高
 sensor_controller.adc_io_open().set_all_io_mode(0).set_all_io_level(1)
 
 # 设置ADC最小采样间隔为10ms，防止请求堵塞STM32从机
 sensor_controller.adc_min_sample_interval_ms = 10
 
 # 获取所有GPIO引脚当前电平
-gpio_levels: c_uint8 = sensor_controller.io_all_channels()
-print(gpio_levels.value)
+gpio_levels: int = sensor_controller.io_all_channels()
+print(f'{gpio_levels:08b}')  # 打印GPIO引脚电平，每一位代表一个引脚，1表示高电平，0表示低电平，从低位到高位索引
+
+# 例如： 0000 0001 表示下标为0的传感器为高电平 
+# 例如： 0000 0100 表示下标为2的传感器为高电平 
 
 # 初始化并读取MPU6500加速度数据
 sensor_controller.MPU6500_Open()
-acceleration_data: Array = sensor_controller.acc_all()
+acceleration_data: Tuple[float, float, float] = sensor_controller.acc_all()
+# (x, y, z) = acceleration_data
+
 
 # 设置第3号GPIO引脚为输出并设置电平为低
 sensor_controller.set_io_mode(2, 1)
 sensor_controller.set_io_level(2, 0)
+
+# 设置第4号GPIO引脚为输入并设置电平为低
+sensor_controller.set_io_mode(3, 0)
+sensor_controller.set_io_level(3, 1)
 ```
 
 ---
 
 # Screen
 
-本模块定义了一个名为 `Screen`
-的类，用于操作和管理LCD屏幕。该类提供了一系列方法，允许用户设置字体大小、颜色、显示方向以及在屏幕上绘制字符串、填充颜色区域等多种操作。每个方法都返回 `Self`
+>
+用于操作和管理LCD屏幕。该类提供了一系列方法，允许用户设置字体大小、颜色、显示方向以及在屏幕上绘制字符串、填充颜色区域等多种操作。每个方法都返回 `Self`
 实例，支持链式调用。
 
 ### **已完成功能**
 
 - **初始化与打开屏幕**：`Screen` 类在实例化时可以自动打开屏幕并设置初始显示方向为水平（通过参数 `direction=2`
   ），同时清空屏幕背景色为黑色。
```

### Comparing `pyuptech-0.1.4a1/pyproject.toml` & `pyuptech-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyuptech"
-version = "0.1.4a1"
+version = "0.1.5"
 description = "A Python wrapper for the uptech binary lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "terminaltables>=3.1.10",
```

### Comparing `pyuptech-0.1.4a1/src/pyuptech/__init__.py` & `pyuptech-0.1.5/src/pyuptech/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .modules.emulation import SensorEmulator
-from .modules.loader import load_lib, TECHSTAR_LIB
+from .modules.loader import load_lib
 from .modules.logger import set_log_level
 from .modules.pins import (
     pin_setter_constructor,
     pin_getter_constructor,
     pin_mode_setter_constructor,
     multiple_pin_mode_setter_constructor,
     PinGetter,
@@ -24,16 +24,14 @@
 
 __all__ = [
     "OnBoardSensors",
     "SensorEmulator",
     "Screen",
     "Color",
     "FontSize",
-    "TECHSTAR_LIB",
-    "load_lib",
     "set_log_level",
     "pin_getter_constructor",
     "pin_setter_constructor",
     "multiple_pin_mode_setter_constructor",
     "pin_mode_setter_constructor",
     # typing
     "ADCArrayType",
```

### Comparing `pyuptech-0.1.4a1/src/pyuptech/lib/libuptech.so` & `pyuptech-0.1.5/src/pyuptech/lib/libuptech.so`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a1/src/pyuptech/modules/emulation.py` & `pyuptech-0.1.5/src/pyuptech/modules/emulation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import ctypes
 from random import randint
 from typing import Self, Literal, Any
 
+from .constant import BinaryIO
 from .sensors import OnBoardSensors, MPUDataPack, ADCDataPack
 
 
 class SensorEmulator(OnBoardSensors):
     mpu_rand_range = (0, 2**32 - 1)
     adc_rand_range = (0, 2**16 - 1)
     io_rand_range = (0, 2**8 - 1)
 
     def adc_io_open(self) -> Self:
         return self
 
     def adc_io_close(self) -> Self:
         return self
 
-    def set_io_level(self, index: int, level: Literal[0, 1]) -> Self:
+    def set_io_level(self, index: int, level: BinaryIO) -> Self:
         return self
 
-    def set_io_mode(self, index: int, mode: Literal[0, 1]) -> Self:
+    def set_io_mode(self, index: int, mode: BinaryIO) -> Self:
         return self
 
-    def set_all_io_mode(self, mode: Literal[0, 1]) -> Self:
+    def set_all_io_mode(self, mode: BinaryIO) -> Self:
         return self
 
-    def set_all_io_level(self, level: Literal[0, 1]) -> Self:
+    def set_all_io_level(self, level: BinaryIO) -> Self:
         return self
 
     @staticmethod
     def io_all_channels() -> int:
         return ctypes.c_uint8(randint(*SensorEmulator.io_rand_range)).value
 
     def adc_all_channels(self) -> ADCDataPack:
@@ -54,15 +55,15 @@
 
     def atti_all(self) -> MPUDataPack:
         for i in range(3):
             self._atti_all[i] = randint(*self.mpu_rand_range)
         return tuple(self._atti_all)  # type: ignore
 
     @staticmethod
-    def get_io_level(index: Literal[0, 1, 2, 3, 4, 5, 6, 7]) -> int:
+    def get_io_level(index: Literal[0, 1, 2, 3, 4, 5, 6, 7] | int) -> int:
         return randint(0, 1)
 
     @staticmethod
     def get_all_io_mode() -> int:
         return ctypes.c_char(randint(*SensorEmulator.io_rand_range)).value[0]
 
     @staticmethod
```

### Comparing `pyuptech-0.1.4a1/src/pyuptech/modules/loader.py` & `pyuptech-0.1.5/src/pyuptech/modules/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import ctypes
 from functools import lru_cache
 
-from .constant import LIB_FILE_PATH
 from .logger import _logger
 
 
 @lru_cache(maxsize=None)
 def load_lib(lib_file_path: str) -> ctypes.CDLL | None:
     """
     Load a dynamic library from the given file path and return a ctypes.CDLL object.
@@ -29,11 +28,9 @@
     except Exception as e:
         _logger.critical(f"Can't load lib [{lib_file_path}],{e}")
         return None
     _logger.info(f"Lib [{lib_file_path}] loaded")
     return obj
 
 
-TECHSTAR_LIB: ctypes.CDLL = load_lib(LIB_FILE_PATH)
-
 if __name__ == "__main__":
     pass
```

### Comparing `pyuptech-0.1.4a1/src/pyuptech/modules/logger.py` & `pyuptech-0.1.5/src/pyuptech/modules/logger.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a1/src/pyuptech/modules/pins.py` & `pyuptech-0.1.5/src/pyuptech/modules/pins.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a1/src/pyuptech/modules/screen.py` & `pyuptech-0.1.5/src/pyuptech/modules/screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,43 +62,54 @@
 
     This class represents an LCD screen and provides methods to manipulate it.
     Each method returns self to enable chainable calls.
     """
 
     lib = load_lib(LIB_FILE_PATH)
 
-    def __init__(self, screen_dir: Literal[1, 2] = None):
+    def __init__(self, screen_dir: Literal[1, 2] | int = None):
         """
         Initializes the Screen class.
 
         Parameters:
             screen_dir (Literal[1, 2], optional): The direction to open the screen in. Defaults to None.
 
         Returns:
             None
         """
 
         if screen_dir is not None:
             self.open(direction=screen_dir).fill_screen(Color.BLACK).refresh()
 
-    def open(self, direction: Literal[1, 2] = 2) -> Self:
+    def open(self, direction: Literal[1, 2] | int = 2) -> Self:
         """
         Open the LCD and set the displaying direction.
 
         Args:
           direction (Literal[1, 2]): Display direction; 1 for vertical, 2 for horizontal.
 
         Returns:
           Self for chainable calls.
         """
 
         _logger.info(f"Open LCD with direction: {direction}")
         self.lib.lcd_open(direction)
         return self
 
+    def close(self) -> Self:
+        """
+        Close the LCD.
+
+        Returns:
+          Self for chainable calls.
+        """
+        _logger.info("Closing LCD")
+        self.lib.lcd_close()
+        return self
+
     def refresh(self) -> Self:
         """
         Refresh the screen, printing the display data from the cache onto the screen.
 
         Returns:
           Self for chainable calls.
         """
@@ -140,15 +151,15 @@
 
         Returns:
           Self for chainable calls.
         """
         self.lib.UG_SetBackcolor(color)
         return self
 
-    def set_led_color(self, index: Literal[0, 1], color: Color) -> Self:
+    def set_led_color(self, index: Literal[0, 1] | int, color: Color) -> Self:
         """
         Set the LED color at a specific index.
 
         Parameters:
             index (Literal[0, 1]): The index of the LED to set the color for.
             color (Color): The color to set for the LED.
```

### Comparing `pyuptech-0.1.4a1/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.5/src/pyuptech/modules/sensors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import ctypes
+from ctypes import c_byte
 from time import perf_counter_ns
 from typing import Self, Literal, Any, Callable, Tuple, TypeAlias
 
-from .loader import TECHSTAR_LIB
+from .constant import LIB_FILE_PATH, BinaryIO
+from .loader import load_lib
 from .logger import _logger
 
 E6 = 1000000
 
 """
 Only For IO, mode and level
 OUTPUT = 1
@@ -18,14 +20,19 @@
 ADCArrayType: Callable = ctypes.c_uint16 * 10  # type: ignore
 # on 32bit machine, this will create a C array of 3 floats with bit-width of 4 bytes
 MPUArrayType: Callable = ctypes.c_float * 3  # type: ignore
 
 ADCDataPack: TypeAlias = Tuple[int, int, int, int, int, int, int, int, int, int]
 MPUDataPack: TypeAlias = Tuple[float, float, float]
 
+__TECHSTAR_LIB__: ctypes.CDLL = load_lib(LIB_FILE_PATH)
+
+# 定义_WORD为无符号短整型
+_WORD = ctypes.c_uint16
+
 
 class OnBoardSensors:
     """
     provides sealed methods accessing to the IOs and builtin sensors
 
     Owns 10 ADC channels and 3 MPU channels  and 8 IO channels
 
@@ -81,26 +88,26 @@
         self.__adc_min_sample_interval_ns = value * E6
 
     def adc_io_open(self) -> Self:
         """
         open the adc-io plug
         """
         _logger.info("Initializing ADC-IO")
-        if open_times := TECHSTAR_LIB.adc_io_open() == -1:
+        if open_times := __TECHSTAR_LIB__.adc_io_open() == -1:
             _logger.error("Failed to open ADC-IO")
         else:
             _logger.debug(f"ADC-IO open {open_times} times")
         return self
 
     def adc_io_close(self) -> Self:
         """
         close the adc-io plug
         """
         _logger.info("Closing ADC-IO")
-        if TECHSTAR_LIB.adc_io_close() == -1:
+        if __TECHSTAR_LIB__.adc_io_close() == -1:
             _logger.error("Failed to close ADC-IO")
         return self
 
     def adc_all_channels(self) -> ADCDataPack:
         """
         Get all the ADC channels. Length = 10
 
@@ -111,20 +118,20 @@
         can_update_time = (
             self.__adc_last_sample_timestamp + self.__adc_min_sample_interval_ns
         )
         if can_update_time > (current := perf_counter_ns()):
 
             return self._adc_cache
         self.__adc_last_sample_timestamp = current
-        if TECHSTAR_LIB.ADC_GetAll(self._adc_all):
+        if __TECHSTAR_LIB__.ADC_GetAll(self._adc_all):
             _logger.error("Failed to get all ADC channels")
         self._adc_cache = tuple(self._adc_all)
         return self._adc_cache  # type: ignore
 
-    def set_io_level(self, index: int, level: Literal[0, 1]) -> Self:
+    def set_io_level(self, index: int, level: BinaryIO) -> Self:
         """
         Set the level of the specified IO index.
 
         Args:
             index (int): The index of the IO.
             level (Literal[0, 1]): The level to set.
 
@@ -135,19 +142,19 @@
             None
 
         Description:
             This function sets the level of the specified IO index using the `adc_io_Set` method from the `OnBoardSensors` class.
             If the `adc_io_Set` method returns a truthy value, an error message is logged.
             The function returns the instance of the class.
         """
-        if TECHSTAR_LIB.adc_io_Set(index, level):
+        if __TECHSTAR_LIB__.adc_io_Set(index, level):
             _logger.error(f"Failed to set IO level, index: {index}, level: {level}")
         return self
 
-    def set_all_io_level(self, level: Literal[0, 1]) -> Self:
+    def set_all_io_level(self, level: BinaryIO) -> Self:
         """
         Sets the level of all IOs to the specified level.
 
         Args:
             level (Literal[0, 1]): The level to set for all IOs.
 
         Returns:
@@ -157,15 +164,15 @@
             None
 
         Description:
             This function sets the level of all IOs to the specified level using the `adc_io_SetAll` method from the `OnBoardSensors` class.
             If the `adc_io_SetAll` method returns a truthy value, an error message is logged.
             The function returns the instance of the class.
         """
-        if TECHSTAR_LIB.adc_io_SetAll(level):
+        if __TECHSTAR_LIB__.adc_io_SetAll(level):
             _logger.error("Failed to set all IO level")
         return self
 
     @staticmethod
     def get_all_io_mode() -> int:
         """
         Get all IO modes. length = 8,store as bit0,bit1,bit2,bit3,bit4,bit5,bit6,bit7
@@ -173,33 +180,33 @@
         Returns:
             int: A buffer containing all IO modes.
         Examples:
             0b10000000 => 第io7为输出模式，可用于驱动舵机
             0b00000001 => 第io0为输入模式，可用于外接传感器
         """
         buffer = ctypes.c_char()
-        if TECHSTAR_LIB.adc_io_ModeGetAll(buffer):
+        if __TECHSTAR_LIB__.adc_io_ModeGetAll(buffer):
             _logger.error("Failed to get all IO mode")
         return buffer.value[0]
 
     @staticmethod
-    def get_io_level(index: Literal[0, 1, 2, 3, 4, 5, 6, 7]) -> int:
+    def get_io_level(index: int) -> int:
         """
         Get the level of the specified IO index.
 
         Args:
-            index (Literal[0, 1, 2, 3, 4, 5, 6, 7]): The index of the IO.
+            index (int): The index of the IO.
 
         Returns:
             int: The level of the specified IO index, which is calculated based on the result of adc_io_InputGetAll().
 
         """
-        return (TECHSTAR_LIB.adc_io_InputGetAll() >> index) & 1
+        return (__TECHSTAR_LIB__.adc_io_InputGetAll() >> index) & 1
 
-    def set_all_io_mode(self, mode: Literal[0, 1]) -> Self:
+    def set_all_io_mode(self, mode: BinaryIO) -> Self:
         """
         Sets the mode of all IOs to the specified mode.
 
         Args:
             mode (Literal[0, 1]): The mode to set for all IOs. Must be either 0 or 1.
 
         Returns:
@@ -209,20 +216,20 @@
             None
 
         Description:
             This function sets the mode of all IOs to the specified mode using the `adc_io_ModeSetAll` method from the `TECHSTAR_LIB` library.
             If the `adc_io_ModeSetAll` method returns a truthy value, an error message is logged.
             The function returns the instance of the class.
         """
-        if TECHSTAR_LIB.adc_io_ModeSetAll(mode):
+        if __TECHSTAR_LIB__.adc_io_ModeSetAll(mode):
             _logger.error(f"Failed to set all IO mode to {mode}")
         return self
 
     def set_io_mode(
-        self, index: Literal[0, 1, 2, 3, 4, 5, 6, 7], mode: Literal[0, 1]
+        self, index: Literal[0, 1, 2, 3, 4, 5, 6, 7] | int, mode: BinaryIO
     ) -> Self:
         """
         Sets the mode of the specified IO index to the specified mode.
 
         Args:
             index (Literal[0, 1]): The index of the IO. Must be either 0 or 1.
             mode (Literal[0, 1]): The mode to set for the IO. Must be either 0 or 1.
@@ -234,57 +241,59 @@
             None
 
         Description:
             This function sets the mode of the specified IO index to the specified mode using the `adc_io_ModeSet` method from the `TECHSTAR_LIB` library.
             If the `adc_io_ModeSet` method returns a truthy value, an error message is logged.
             The function returns the instance of the class.
         """
-        if TECHSTAR_LIB.adc_io_ModeSet(index, mode):
+        if __TECHSTAR_LIB__.adc_io_ModeSet(index, mode):
             _logger.error(f"Failed to set IO mode, index: {index}, mode: {mode}")
         return self
 
     @staticmethod
     def io_all_channels() -> int:
         """
         get all io plug input levels
 
         uint8, each bit represents a channel, 1 for high, 0 for low
 
         Examples:
             0b10000000 => 第io7为高电平
             0b00000001 => 第io0为高电平
         """
-        return TECHSTAR_LIB.adc_io_InputGetAll().value
+        return __TECHSTAR_LIB__.adc_io_InputGetAll()
 
     def MPU6500_Open(self) -> Self:
         """
         initialize the 6-axis enhancer MPU6500
         default settings:
             acceleration: -+8G
             gyro: -+2000 degree/s
             sampling rate: 1kHz
         """
         _logger.info("Initializing MPU6500...")
-        if TECHSTAR_LIB.mpu6500_dmp_init():
+        if __TECHSTAR_LIB__.mpu6500_dmp_init():
             _logger.warning("Failed to initialize MPU6500")
+            return self
+        _logger.info("MPU6500 initialized")
         return self
 
     def acc_all(self) -> MPUDataPack:
         """
         Retrieves the acceleration data from the MPU6500 sensor.
 
         Returns:
             MPUDataPack: An array containing the acceleration data.
         Notes:
             length = 3
             [0] ==> axis X
             [1] ==> axis Y
             [2] ==> axis Z
         """
-        TECHSTAR_LIB.mpu6500_Get_Accel(
+        __TECHSTAR_LIB__.mpu6500_Get_Accel(
             self._accel_all
         )  # this function return a C pointer to the self._accel_all
         return tuple(self._accel_all)  # type: ignore
 
     def gyro_all(self) -> MPUDataPack:
         """
         Retrieves the gyroscope data from the MPU6500 sensor.
@@ -295,15 +304,15 @@
         Notes:
             length = 3
             [0] ==> axis X
             [1] ==> axis Y
             [2] ==> axis Z
         """
 
-        TECHSTAR_LIB.mpu6500_Get_Gyro(
+        __TECHSTAR_LIB__.mpu6500_Get_Gyro(
             self._gyro_all
         )  # this function return a C pointer to the self._gyro_all
 
         return tuple(self._gyro_all)  # type: ignore
 
     def atti_all(self) -> MPUDataPack:
         """
@@ -314,15 +323,15 @@
 
         Notes:
             length = 3
             [0] ==> Pitch|axis X
             [1] ==> Roll |axis Y
             [2] ==> Yaw  |axis Z
         """
-        TECHSTAR_LIB.mpu6500_Get_Attitude(
+        __TECHSTAR_LIB__.mpu6500_Get_Attitude(
             self._atti_all
         )  # this function return a C pointer to the self._atti_all
 
         return tuple(self._atti_all)  # type: ignore
 
     @staticmethod
     def get_handle(attr_name: str) -> Any:
@@ -334,8 +343,70 @@
 
         Returns:
             Any: The value of the attribute.
 
         Raises:
             AttributeError: If the attribute does not exist in the TECHSTAR_LIB object.
         """
-        return getattr(TECHSTAR_LIB, attr_name)
+        return getattr(__TECHSTAR_LIB__, attr_name)
+
+    @staticmethod
+    def get_gyro_fsr() -> int:
+        """
+        Retrieves the Full Scale Range (FSR) of the gyroscope.
+
+        This method queries and returns the FSR value of the gyroscope from the technology library.
+
+        Returns:
+            int: The Full Scale Range value of the gyroscope.
+        """
+
+        # Calls the technology library function to obtain the gyroscope's FSR, storing the result in fsr_value
+        __TECHSTAR_LIB__.mpu_get_gyro_fsr(ctypes.byref(fsr_value := _WORD()))
+        return fsr_value.value
+
+    @staticmethod
+    def get_acc_fsr() -> int:
+        """
+        Retrieves the accelerometer full-scale range.
+
+        This static method fetches the current full-scale range for the accelerometer from the TECHSTAR_LIB.
+
+        Returns:
+            int: The value representing the accelerometer full-scale range.
+        """
+
+        # Request the accelerometer full-scale range value
+        __TECHSTAR_LIB__.mpu_get_accel_fsr(ctypes.byref(fsr_value := c_byte()))
+        # Return the obtained accelerometer full-scale range value
+        return fsr_value.value
+
+    def mpu_set_gyro_fsr(self, fsr: Literal[250, 500, 1000, 2000] | int) -> Self:
+        """
+        Sets the full-scale range for the gyroscope in the MPU.
+
+        Parameters:
+            fsr (Literal[250, 500, 1000, 2000] | int): Gyroscope full-scale range, can be one of 250, 500, 1000, or 2000 degrees per second.
+
+        Returns:
+            Self: Returns an instance of the function for method chaining.
+        """
+
+        # Call the underlying library function to set the gyroscope's full-scale range
+        __TECHSTAR_LIB__.mpu_set_gyro_fsr(ctypes.c_uint(fsr))
+        return self
+
+    def mpu_set_accel_fsr(self, fsr: Literal[2, 4, 8, 16] | int) -> Self:
+        """
+        Sets the accelerometer full-scale range (FSR) for the MPU.
+
+        Parameters:
+            fsr: Literal[2, 4, 8, 16] | int - The full-scale range of the accelerometer, with options being 2g, 4g, 8g, and 16g.
+
+        Returns:
+            Self: Returns the object itself to support method chaining.
+        """
+
+        __TECHSTAR_LIB__.mpu_set_accel_fsr(
+            ctypes.c_int(fsr)
+        )  # Invokes the library function to set the accelerometer's FSR
+        return self
```

### Comparing `pyuptech-0.1.4a1/src/pyuptech/tools/display.py` & `pyuptech-0.1.5/src/pyuptech/tools/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,19 @@
     match mode:
         case "on":
             #  仿真器不需要启动adc-io等硬件设备
             sensors = SensorEmulator()
             screen = None  # 仿真模式下，假设屏幕是脱机的
         case "off":
             sensors = (
-                OnBoardSensors().adc_io_open().set_all_io_mode(0).set_all_io_level(1)
+                OnBoardSensors()
+                .adc_io_open()
+                .set_all_io_mode(0)
+                .set_all_io_level(1)
+                .MPU6500_Open()
             )
             screen = (
                 Screen()
                 .open()
                 .fill_screen(Color.BLACK)
                 .refresh()
                 .set_led_color(0, Color.BROWN)
@@ -58,22 +62,22 @@
         case "atti":
             attitude = sensors.atti_all()
             screen.put_string(0, 30, f"Pitch:{attitude[0]:.2f}  ")
             screen.put_string(0, 48, f"Roll :{attitude[1]:.2f}  ")
             screen.put_string(0, 66, f"Yaw  :{attitude[2]:.2f}  ")
         case "gyro":
             gyro = sensors.gyro_all()
-            screen.put_string(0, 30, f"Gyro x {gyro[0]:.2}")
-            screen.put_string(0, 48, f"Gyro y {gyro[1]:.2}")
-            screen.put_string(0, 66, f"Gyro z {gyro[2]:.2}")
+            screen.put_string(0, 30, f"Gyro X {gyro[0]:.2f}")
+            screen.put_string(0, 48, f"Gyro Y {gyro[1]:.2f}")
+            screen.put_string(0, 66, f"Gyro Z {gyro[2]:.2f}")
         case "acc":
             accel = sensors.acc_all()
-            screen.put_string(0, 30, f"x_acc :{accel[0]:.2}")
-            screen.put_string(0, 44, f"y_acc :{accel[1]:.2}")
-            screen.put_string(0, 54, f"z_acc :{accel[2]:.2}")
+            screen.put_string(0, 30, f"ACC X :{accel[0]:.2f}")
+            screen.put_string(0, 44, f"ACC Y :{accel[1]:.2f}")
+            screen.put_string(0, 54, f"ACC Z :{accel[2]:.2f}")
     screen.refresh()
 
 
 def mpu_display_on_console():
     """
     Display the MPU data in a formatted table in the terminal.
 
@@ -92,19 +96,19 @@
     gyro_names = ["X_GYRO", "Y_GYRO", "Z_GYRO"]
 
     atti_names = ["Pitch", "Roll", "Yaw"]
     for i in range(len(acc_names)):
         combined_data.append(
             [
                 acc_names[i],
-                f"{sensors.acc_all()[i]:.2}",
+                f"{sensors.acc_all()[i]:.2f}",
                 gyro_names[i],
-                f"{sensors.gyro_all()[i]:.2}",
+                f"{sensors.gyro_all()[i]:.2f}",
                 atti_names[i],
-                f"{sensors.atti_all()[i]:.2}",
+                f"{sensors.atti_all()[i]:.2f}",
             ]
         )
 
     # Create and print the table
     table = DoubleTable(combined_data)
     table.inner_row_border = True  # Add inner row borders for clarity
     print(table.table)
```

### Comparing `pyuptech-0.1.4a1/tests/perf_tests.py` & `pyuptech-0.1.5/tests/perf_tests.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.4a1/PKG-INFO` & `pyuptech-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuptech
-Version: 0.1.4a1
+Version: 0.1.5
 Summary: A Python wrapper for the uptech binary lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: terminaltables>=3.1.10
 Description-Content-Type: text/markdown
@@ -15,22 +15,31 @@
 ---
 
 # 安装
 
 使用`pdm`安装
 
 ```shell
+# 安装pdm
+python -m pip install pdm
+
+# 切换源
+pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
+
+# 安装pyuptech
 pdm add pyuptech
+
+# 或者安装不稳定版
+pdm add pyuptech --pre
+
 ```
 
 ## OnBoardSensors
 
-**简介**
-
-`OnBoardSensors`是一个Python类，封装了对嵌入式硬件板载传感器和输入/输出接口的操作，如ADC、GPIO以及MPU6500六轴传感器。该类通过ctypes库调用预编译的C库函数实现底层硬件交互。
+> `OnBoardSensors`是一个Python类，封装了对嵌入式硬件板载传感器和输入/输出接口的操作，如ADC、GPIO以及MPU6500六轴传感器。该类通过ctypes库调用预编译的C库函数实现底层硬件交互。
 
 ### 类方法概览
 
 - **初始化**: 初始化所有IO通道模式为输入，并设置初始电平为高，同时初始化ADC插件。
 
 - **ADC操作**:
     - `adc_min_sample_interval_ms`: 获取和设置ADC采样间隔（以毫秒为单位，内部存储为纳秒）。
@@ -55,44 +64,53 @@
 - 获取ADC和GPIO的数据。
 - 初始化和读取MPU6500六轴传感器数据。
 
 ### QUICKSTART
 
 ```python
 from pyuptech import OnBoardSensors
-from ctypes import c_uint8, Array
+from typing import Tuple
 
 # 创建OnBoardSensors对象，设置模拟量传感器最小采样间隔为5ms
 sensor_controller = OnBoardSensors(adc_min_sample_interval_ms=5)
 
 # 初始化ADC,设置所有GPIO引脚为输入，设置初始电平为高
 sensor_controller.adc_io_open().set_all_io_mode(0).set_all_io_level(1)
 
 # 设置ADC最小采样间隔为10ms，防止请求堵塞STM32从机
 sensor_controller.adc_min_sample_interval_ms = 10
 
 # 获取所有GPIO引脚当前电平
-gpio_levels: c_uint8 = sensor_controller.io_all_channels()
-print(gpio_levels.value)
+gpio_levels: int = sensor_controller.io_all_channels()
+print(f'{gpio_levels:08b}')  # 打印GPIO引脚电平，每一位代表一个引脚，1表示高电平，0表示低电平，从低位到高位索引
+
+# 例如： 0000 0001 表示下标为0的传感器为高电平 
+# 例如： 0000 0100 表示下标为2的传感器为高电平 
 
 # 初始化并读取MPU6500加速度数据
 sensor_controller.MPU6500_Open()
-acceleration_data: Array = sensor_controller.acc_all()
+acceleration_data: Tuple[float, float, float] = sensor_controller.acc_all()
+# (x, y, z) = acceleration_data
+
 
 # 设置第3号GPIO引脚为输出并设置电平为低
 sensor_controller.set_io_mode(2, 1)
 sensor_controller.set_io_level(2, 0)
+
+# 设置第4号GPIO引脚为输入并设置电平为低
+sensor_controller.set_io_mode(3, 0)
+sensor_controller.set_io_level(3, 1)
 ```
 
 ---
 
 # Screen
 
-本模块定义了一个名为 `Screen`
-的类，用于操作和管理LCD屏幕。该类提供了一系列方法，允许用户设置字体大小、颜色、显示方向以及在屏幕上绘制字符串、填充颜色区域等多种操作。每个方法都返回 `Self`
+>
+用于操作和管理LCD屏幕。该类提供了一系列方法，允许用户设置字体大小、颜色、显示方向以及在屏幕上绘制字符串、填充颜色区域等多种操作。每个方法都返回 `Self`
 实例，支持链式调用。
 
 ### **已完成功能**
 
 - **初始化与打开屏幕**：`Screen` 类在实例化时可以自动打开屏幕并设置初始显示方向为水平（通过参数 `direction=2`
   ），同时清空屏幕背景色为黑色。
```


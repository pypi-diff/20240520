# Comparing `tmp/wlkata_mirobot_Virtual-1.2.2.tar.gz` & `tmp/wlkata_mirobot_Virtual-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkata_mirobot_Virtual-1.2.2.tar", last modified: Fri May 17 08:40:00 2024, max compression
+gzip compressed data, was "wlkata_mirobot_Virtual-1.2.3.tar", last modified: Mon May 20 03:28:27 2024, max compression
```

## Comparing `wlkata_mirobot_Virtual-1.2.2.tar` & `wlkata_mirobot_Virtual-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 08:40:00.532626 wlkata_mirobot_Virtual-1.2.2/
--rw-rw-rw-   0        0        0      110 2024-05-17 08:40:00.531629 wlkata_mirobot_Virtual-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-05-13 07:29:56.000000 wlkata_mirobot_Virtual-1.2.2/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 08:40:00.532626 wlkata_mirobot_Virtual-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      236 2024-05-17 08:39:11.000000 wlkata_mirobot_Virtual-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:40:00.526643 wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual/
--rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual/__init__.py
--rw-rw-rw-   0        0        0    19597 2024-05-17 08:38:35.000000 wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:40:00.530632 wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual.egg-info/
--rw-rw-rw-   0        0        0      110 2024-05-17 08:40:00.000000 wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-17 08:40:00.000000 wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 08:40:00.000000 wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-17 08:40:00.000000 wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 03:28:27.488248 wlkata_mirobot_Virtual-1.2.3/
+-rw-rw-rw-   0        0        0      110 2024-05-20 03:28:27.487251 wlkata_mirobot_Virtual-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-05-13 07:29:56.000000 wlkata_mirobot_Virtual-1.2.3/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 03:28:27.488248 wlkata_mirobot_Virtual-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      236 2024-05-20 03:28:04.000000 wlkata_mirobot_Virtual-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:28:27.483261 wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual/
+-rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual/__init__.py
+-rw-rw-rw-   0        0        0    19641 2024-05-20 03:27:09.000000 wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:28:27.487251 wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual.egg-info/
+-rw-rw-rw-   0        0        0      110 2024-05-20 03:28:27.000000 wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-20 03:28:27.000000 wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 03:28:27.000000 wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-20 03:28:27.000000 wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual.egg-info/top_level.txt
```

### Comparing `wlkata_mirobot_Virtual-1.2.2/license.txt` & `wlkata_mirobot_Virtual-1.2.3/license.txt`

 * *Files identical despite different names*

### Comparing `wlkata_mirobot_Virtual-1.2.2/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py` & `wlkata_mirobot_Virtual-1.2.3/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,28 +90,28 @@
                     
                 extracted_values = [value for sublist in P for value in sublist]
                 for i, value in enumerate(extracted_values, start=1):
                     self.slave.set_values("robot_Virtual", i, value)  
 
         except Exception as e:
             robot_logger.error(f"modbus_Set_robot_Angles error: {e}")
-    ### DI信号寄存器地址70开始
+    ### DI信号寄存器地址73开始
     def modbus_Set_Input_Status(self, input_status):
         try:
-            extracted_values = input_status
-            for i, value in enumerate(extracted_values, start=70):
+            extracted_values = [value for sublist in input_status for value in sublist]
+            for i, value in enumerate(extracted_values, start=73):
                 self.slave.set_values("robot_Virtual", i, value) 
         
         except Exception as e:
             robot_logger.error(f"modbus_Set_Input_Status error: {e}")
-    ### DO信号寄存器地址90开始
+    ### DO信号寄存器地址94开始
     def modbus_Set_Output_Status(self, output_status):
         try:
             extracted_values = output_status
-            for i, value in enumerate(extracted_values, start=90):
+            for i, value in enumerate(extracted_values, start=94):
                 self.slave.set_values("robot_Virtual", i, value) 
         
         except Exception as e:
             robot_logger.error(f"modbus_Set_Output_Status error: {e}")
 
     def float2int16s(self, f):
         ## 将浮点数打包成32位二进制数据
```


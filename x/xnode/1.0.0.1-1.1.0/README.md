# Comparing `tmp/xnode-1.0.0.1.tar.gz` & `tmp/xnode-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnode-1.0.0.1.tar", last modified: Thu Apr 11 05:21:11 2024, max compression
+gzip compressed data, was "xnode-1.1.0.tar", last modified: Mon May 20 07:45:38 2024, max compression
```

## Comparing `xnode-1.0.0.1.tar` & `xnode-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 05:21:11.835149 xnode-1.0.0.1/
--rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 xnode-1.0.0.1/LICENSE
--rw-rw-rw-   0        0        0       19 2024-04-08 06:03:18.000000 xnode-1.0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2299 2024-04-11 05:21:11.834143 xnode-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1727 2024-04-08 06:00:19.000000 xnode-1.0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 05:21:11.835149 xnode-1.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1018 2024-04-08 05:23:52.000000 xnode-1.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 05:21:11.785470 xnode-1.0.0.1/xnode/
--rw-rw-rw-   0        0        0       23 2024-04-08 05:23:46.000000 xnode-1.0.0.1/xnode/__init__.py
--rw-rw-rw-   0        0        0     8587 2024-04-08 08:02:01.000000 xnode-1.0.0.1/xnode/cli.py
--rw-rw-rw-   0        0        0     6621 2024-04-08 04:23:48.000000 xnode-1.0.0.1/xnode/files.py
-drwxrwxrwx   0        0        0        0 2024-04-11 05:21:11.831732 xnode-1.0.0.1/xnode/pop/
--rw-rw-rw-   0        0        0     6846 2024-01-17 23:46:57.000000 xnode-1.0.0.1/xnode/pop/autoctrl.py
--rw-rw-rw-   0        0        0     5172 2024-02-07 04:10:07.000000 xnode-1.0.0.1/xnode/pop/core.py
--rw-rw-rw-   0        0        0     4579 2024-01-30 00:49:42.000000 xnode-1.0.0.1/xnode/pop/ext.py
--rw-rw-rw-   0        0        0     7396 2024-02-19 04:38:47.000000 xnode-1.0.0.1/xnode/pop/tphg.py
--rw-rw-rw-   0        0        0     6497 2023-10-05 06:33:32.000000 xnode-1.0.0.1/xnode/pyboard.py
--rw-rw-rw-   0        0        0      793 2024-01-25 00:42:40.000000 xnode-1.0.0.1/xnode/xnode.py
-drwxrwxrwx   0        0        0        0 2024-04-11 05:21:11.832741 xnode-1.0.0.1/xnode.egg-info/
--rw-rw-rw-   0        0        0     2299 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 07:45:38.204118 xnode-1.1.0/
+-rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 xnode-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       19 2024-04-08 06:03:18.000000 xnode-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2296 2024-05-20 07:45:38.203119 xnode-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1727 2024-04-08 06:00:19.000000 xnode-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:45:38.204118 xnode-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-20 07:39:37.000000 xnode-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:45:38.150717 xnode-1.1.0/xnode/
+-rw-rw-rw-   0        0        0       21 2024-05-20 07:42:14.000000 xnode-1.1.0/xnode/__init__.py
+-rw-rw-rw-   0        0        0     8587 2024-04-08 08:02:01.000000 xnode-1.1.0/xnode/cli.py
+-rw-rw-rw-   0        0        0     6621 2024-04-08 04:23:48.000000 xnode-1.1.0/xnode/files.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:45:38.199121 xnode-1.1.0/xnode/pop/
+-rw-rw-rw-   0        0        0     6846 2024-01-17 23:46:57.000000 xnode-1.1.0/xnode/pop/autoctrl.py
+-rw-rw-rw-   0        0        0     5314 2024-04-19 07:31:40.000000 xnode-1.1.0/xnode/pop/core.py
+-rw-rw-rw-   0        0        0     4580 2024-04-19 05:07:43.000000 xnode-1.1.0/xnode/pop/ext.py
+-rw-rw-rw-   0        0        0     7396 2024-02-19 04:38:47.000000 xnode-1.1.0/xnode/pop/tphg.py
+-rw-rw-rw-   0        0        0     6497 2023-10-05 06:33:32.000000 xnode-1.1.0/xnode/pyboard.py
+-rw-rw-rw-   0        0        0      793 2024-01-25 00:42:40.000000 xnode-1.1.0/xnode/xnode.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:45:38.201119 xnode-1.1.0/xnode.egg-info/
+-rw-rw-rw-   0        0        0     2296 2024-05-20 07:45:37.000000 xnode-1.1.0/xnode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-20 07:45:38.000000 xnode-1.1.0/xnode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:45:37.000000 xnode-1.1.0/xnode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-20 07:45:37.000000 xnode-1.1.0/xnode.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-20 07:45:37.000000 xnode-1.1.0/xnode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       29 2024-05-20 07:45:37.000000 xnode-1.1.0/xnode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 07:45:38.000000 xnode-1.1.0/xnode.egg-info/top_level.txt
```

### Comparing `xnode-1.0.0.1/LICENSE` & `xnode-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0.1/PKG-INFO` & `xnode-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: xnode
-Version: 1.0.0.1
+Version: 1.1.0
 Summary: This is a CLI management tool for MicroPython-based XNode.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: micropython,xnode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: pyserial
 
 This is a CLI management tool for MicroPython-based XNode.
```

### Comparing `xnode-1.0.0.1/README.md` & `xnode-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0.1/setup.py` & `xnode-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name='xnode',
-    version='1.0.0.1',
+    version='1.1.0',
     description='This is a CLI management tool for MicroPython-based XNode.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='chanmin.park',
     author_email='devcamp@gmail.com',
     url='https://github.com/planxstudio/xkit',
     install_requires=['click', 'python-dotenv', 'pyserial'],
     packages=find_packages(exclude=[]),
     keywords=['micropython', 'xnode'],
-    python_requires='>=3.11',
+    python_requires='>=3.8',
     package_data={},
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `xnode-1.0.0.1/xnode/cli.py` & `xnode-1.1.0/xnode/cli.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0.1/xnode/files.py` & `xnode-1.1.0/xnode/files.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0.1/xnode/pop/autoctrl.py` & `xnode-1.1.0/xnode/pop/autoctrl.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0.1/xnode/pop/core.py` & `xnode-1.1.0/xnode/pop/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import uos
 import machine 
 from micropython import const
 
 def sqrt(x, epsilon=1e-10):
     guess = x / 2.0
 
-    while abs(guess * guess - x) > epsilon:
+    op_limit = 5
+    while abs(guess * guess - x) > epsilon and op_limit:
         guess = (guess + x / guess) / 2.0
+        op_limit -= 1
 
     return guess
 
 def abs(x):
   return x if x >= 0 else -x
 
 def rand(size=4):
@@ -32,28 +34,30 @@
         RED = "\u001b[31m"
         GREEN = "\u001b[32m"
         YELLOW = "\u001b[33m"
         BLUE = "\u001b[34m"
         MAGENTA = "\u001b[35m"
         CYAN = "\u001b[36m"
         WHITE = "\u001b[37m"
-
-        def rgb(r, g, b): return "\u001b[38;2;{};{};{}m".format(r, g, b)
+        
+        @classmethod
+        def rgb(cls, r, g, b): return "\u001b[38;2;{};{};{}m".format(r, g, b)
 
     class BG:
         BLACK = "\u001b[40m"
         RED = "\u001b[41m"
         GREEN = "\u001b[42m"
         YELLOW = "\u001b[43m"
         BLUE = "\u001b[44m"
         MAGENTA = "\u001b[45m"
         CYAN = "\u001b[46m"
         WHITE = "\u001b[47m"
-
-        def rgb(r, g, b): return "\u001b[48;2;{};{};{}m".format(r, g, b)
+        
+        @classmethod
+        def rgb(cls, r, g, b): return "\u001b[48;2;{};{};{}m".format(r, g, b)
 
     class OP:
         RESET = "\u001b[0m"
         BOLD = "\u001b[1m"
         UNDER_LINE = "\u001b[4m"
         REVERSE = "\u001b[7m"
         CLEAR = "\u001b[2J"
@@ -62,69 +66,70 @@
         DOWN = "\u001b[1B"
         RIGHT = "\u001b[1C"
         LEFT = "\u001b[1D"
         NEXT_LINE = "\u001b[1E"
         PREV_LINE = "\u001b[1F"
         TOP = "\u001b[0;0H"
         
-        def to(row, colum):
+        @classmethod
+        def to(cls, row, colum):
             return "\u001b[{};{}H".format(row, colum)
 
 class Uart:
     SLIP_END = const(b'\xC0')		# dec: 192
     SLIP_ESC = const(b'\xDB')		# dec: 219
     SLIP_ESC_END = const(b'\xDC')	# dec: 220
     SLIP_ESC_ESC = const(b'\xDD')	# dec: 221
     
     @classmethod
-    def read(self, size=0, **kwargs):
+    def read(cls, size, **kwargs):
         slip = kwargs['slip'] if 'slip' in kwargs.keys() else False
         decoding = kwargs['decoding'] if 'decoding' in kwargs.keys() else True
         
         if not slip:
-            if n == 0:
-                raise ValueError("n >= 1")
+            if size == 0:
+                raise ValueError("size >= 1")
             data = sys.stdin.buffer.read(size)
         else:
             started = False
             skip= False
             data = b''
             while True:
                 char = sys.stdin.buffer.read(1)
                 if not skip:
-                    if char == self.SLIP_END:
+                    if char == cls.SLIP_END:
                         if not started:
                             started = True
                         else:                                  
-                            data.replace(self.SLIP_ESC + self.SLIP_ESC_END, self.SLIP_END).replace(self.SLIP_ESC + self.SLIP_ESC_ESC, self.SLIP_ESC)        
+                            data.replace(cls.SLIP_ESC + cls.SLIP_ESC_END, cls.SLIP_END).replace(cls.SLIP_ESC + cls.SLIP_ESC_ESC, cls.SLIP_ESC)        
                             break
                     else:
                         if not started:
                             skip = True
                         else:
                             data += char
                 else:
-                    if char == self.SLIP_END:
+                    if char == cls.SLIP_END:
                         skip = False
         
         return data.decode() if decoding else data
                         
     @classmethod
-    def write(self, *data, **kwargs):
+    def write(cls, *data, **kwargs):
         end = kwargs['end'] if 'end' in kwargs.keys() else '\n'
         sep = kwargs['sep'] if 'sep' in kwargs.keys() else ' '
         slip = kwargs['slip'] if 'slip' in kwargs.keys() else False
 
         t_data = ''
         for d in data:
             t_data += str(d) + sep
         data = t_data
                 
         if not slip:        
-            data[-1] = end
+            data += end
             sys.stdout.buffer.write(data)
         else:
             data = data.rstrip()
             data = bytes(data.encode())
             sys.stdout.buffer.write(self.SLIP_END + data.replace(self.SLIP_ESC, self.SLIP_ESC + self.SLIP_ESC_ESC).replace(self.SLIP_END, self.SLIP_ESC + self.SLIP_ESC_END) + self.SLIP_END)
```

### Comparing `xnode-1.0.0.1/xnode/pop/ext.py` & `xnode-1.1.0/xnode/pop/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         time.sleep_ms(650)
         self.__i2c.writeto_mem(self.__BNO055_ADDR, 0X3E, bytes([0x00])) #Power Resiter, Set to normal power. cf) low power is 0x01
         self.__i2c.writeto_mem(self.__BNO055_ADDR, 0X07, bytes([0x00])) #Page Register, Make sure we're in config mode and on page0(param, data), page1(conf)
         self.__i2c.writeto_mem(self.__BNO055_ADDR, 0X3F, bytes([0x80])) #Trigger Register, External oscillator
         self.__i2c.writeto_mem(self.__BNO055_ADDR, 0X3F, bytes([0x00])) #Trigger Register,
         time.sleep_ms(10)
         self.__i2c.writeto_mem(self.__BNO055_ADDR, 0X3D, bytes([0x0C])) #Mode Register, Enter normal operation (NDOF)
-        time.sleep_ms(20)
+        time.sleep_ms(200)
 
     def __read_temperature(self, addr):
         t = self.__i2c.readfrom_mem(self.__BNO055_ADDR, addr, 1)[0]
         return t - 256 if t > 127 else t
 
     def __read_quaternion(self, addr):
         t = self.__i2c.readfrom_mem(self.__BNO055_ADDR, addr, 8)
```

### Comparing `xnode-1.0.0.1/xnode/pop/tphg.py` & `xnode-1.1.0/xnode/pop/tphg.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0.1/xnode/pyboard.py` & `xnode-1.1.0/xnode/pyboard.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0.1/xnode/xnode.py` & `xnode-1.1.0/xnode/xnode.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0.1/xnode.egg-info/PKG-INFO` & `xnode-1.1.0/xnode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: xnode
-Version: 1.0.0.1
+Version: 1.1.0
 Summary: This is a CLI management tool for MicroPython-based XNode.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: micropython,xnode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: pyserial
 
 This is a CLI management tool for MicroPython-based XNode.
```


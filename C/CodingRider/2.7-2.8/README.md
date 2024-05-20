# Comparing `tmp/codingrider-2.7.tar.gz` & `tmp/codingrider-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codingrider-2.7.tar", last modified: Thu May 16 07:04:14 2024, max compression
+gzip compressed data, was "codingrider-2.8.tar", last modified: Mon May 20 02:40:13 2024, max compression
```

## Comparing `codingrider-2.7.tar` & `codingrider-2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:04:14.180271 codingrider-2.7/
-drwxrwxrwx   0        0        0        0 2024-05-16 07:04:14.156143 codingrider-2.7/CodingRider/
--rw-rw-rw-   0        0        0      109 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      484 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/crc.py
--rw-rw-rw-   0        0        0    41310 2024-05-16 06:25:01.000000 codingrider-2.7/CodingRider/drone.py
--rw-rw-rw-   0        0        0    61138 2024-05-16 06:58:18.000000 codingrider-2.7/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     1696 2024-05-16 06:55:33.000000 codingrider-2.7/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10845 2024-05-16 06:25:19.000000 codingrider-2.7/CodingRider/system.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:04:14.177445 codingrider-2.7/CodingRider/tools/
--rw-rw-rw-   0        0        0       48 2024-05-14 06:50:08.000000 codingrider-2.7/CodingRider/tools/__init__.py
--rw-rw-rw-   0        0        0    29709 2024-05-14 06:50:01.000000 codingrider-2.7/CodingRider/tools/parser.py
--rw-rw-rw-   0        0        0     9495 2024-05-14 06:53:10.000000 codingrider-2.7/CodingRider/tools/update.py
--rw-rw-rw-   0        0        0     9515 2024-05-14 03:59:45.000000 codingrider-2.7/CodingRider/update.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:04:14.179254 codingrider-2.7/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      718 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 07:04:14.000000 codingrider-2.7/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-14 03:14:00.000000 codingrider-2.7/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-14 03:14:00.000000 codingrider-2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      718 2024-05-16 07:04:14.180271 codingrider-2.7/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-05-14 03:14:00.000000 codingrider-2.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 07:04:14.181277 codingrider-2.7/setup.cfg
--rw-rw-rw-   0        0        0      772 2024-05-16 07:04:07.000000 codingrider-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:40:13.662588 codingrider-2.8/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:40:13.653186 codingrider-2.8/CodingRider/
+-rw-rw-rw-   0        0        0      109 2024-05-14 03:59:45.000000 codingrider-2.8/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-05-14 03:59:45.000000 codingrider-2.8/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2024-05-14 03:59:45.000000 codingrider-2.8/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    41310 2024-05-20 02:34:53.000000 codingrider-2.8/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    61138 2024-05-20 02:36:56.000000 codingrider-2.8/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2024-05-14 03:59:45.000000 codingrider-2.8/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1696 2024-05-16 06:55:33.000000 codingrider-2.8/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10845 2024-05-16 06:25:19.000000 codingrider-2.8/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:40:13.659549 codingrider-2.8/CodingRider/tools/
+-rw-rw-rw-   0        0        0       48 2024-05-14 06:50:08.000000 codingrider-2.8/CodingRider/tools/__init__.py
+-rw-rw-rw-   0        0        0    29709 2024-05-20 02:35:31.000000 codingrider-2.8/CodingRider/tools/parser.py
+-rw-rw-rw-   0        0        0     9495 2024-05-14 06:53:10.000000 codingrider-2.8/CodingRider/tools/update.py
+-rw-rw-rw-   0        0        0     9515 2024-05-14 03:59:45.000000 codingrider-2.8/CodingRider/update.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:40:13.659549 codingrider-2.8/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      718 2024-05-20 02:40:13.000000 codingrider-2.8/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2024-05-20 02:40:13.000000 codingrider-2.8/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 02:40:13.000000 codingrider-2.8/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-20 02:40:13.000000 codingrider-2.8/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 02:40:13.000000 codingrider-2.8/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-14 03:14:00.000000 codingrider-2.8/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-14 03:14:00.000000 codingrider-2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      718 2024-05-20 02:40:13.662588 codingrider-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-14 03:14:00.000000 codingrider-2.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 02:40:13.662588 codingrider-2.8/setup.cfg
+-rw-rw-rw-   0        0        0      772 2024-05-20 02:39:00.000000 codingrider-2.8/setup.py
```

### Comparing `codingrider-2.7/CodingRider/crc.py` & `codingrider-2.8/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.7/CodingRider/drone.py` & `codingrider-2.8/CodingRider/drone.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
         header.length   = Command.getSize()
         header.from_    = DeviceType.Base
         header.to_      = DeviceType.Drone
 
         data = Command()
 
         data.commandType    = CommandType.FlightEvent
-        data.option         = FlightEvent.TakeOff.value
+        data.option         = FlightEvent.Takeoff.value
 
         return self.transfer(header, data)
 
 
 
     def sendLanding(self):
```

### Comparing `codingrider-2.7/CodingRider/protocol.py` & `codingrider-2.8/CodingRider/protocol.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.7/CodingRider/receiver.py` & `codingrider-2.8/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.7/CodingRider/storage.py` & `codingrider-2.8/CodingRider/storage.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.7/CodingRider/system.py` & `codingrider-2.8/CodingRider/system.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.7/CodingRider/tools/parser.py` & `codingrider-2.8/CodingRider/tools/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
             # 이륙
             #                   0
             # python -m CodingRider Takeoff
             elif    ((self.count == 1) and 
                     (self.arguments[0] == "takeoff")):
                 print (Fore.YELLOW + "takeoff" + Style.RESET_ALL)
-                self.command(CommandType.FlightEvent, FlightEvent.TakeOff.value)
+                self.command(CommandType.FlightEvent, FlightEvent.Takeoff.value)
                 return
 
             # 착륙
             #                   0
             # python -m CodingRider Landing
             elif    ((self.count == 1) and 
                     (self.arguments[0] == "landing")):
```

### Comparing `codingrider-2.7/CodingRider/tools/update.py` & `codingrider-2.8/CodingRider/tools/update.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.7/CodingRider/update.py` & `codingrider-2.8/CodingRider/update.py`

 * *Files identical despite different names*

### Comparing `codingrider-2.7/CodingRider.egg-info/PKG-INFO` & `codingrider-2.8/CodingRider.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.7
+Version: 2.8
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
```

### Comparing `codingrider-2.7/PKG-INFO` & `codingrider-2.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 2.7
+Version: 2.8
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
```

### Comparing `codingrider-2.7/setup.py` & `codingrider-2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "2.7",
+    version = "2.8",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
```


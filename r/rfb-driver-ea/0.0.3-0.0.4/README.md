# Comparing `tmp/rfb_driver_ea-0.0.3.tar.gz` & `tmp/rfb_driver_ea-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfb_driver_ea-0.0.3.tar", last modified: Thu May 16 09:54:09 2024, max compression
+gzip compressed data, was "rfb_driver_ea-0.0.4.tar", last modified: Mon May 20 07:50:38 2024, max compression
```

## Comparing `rfb_driver_ea-0.0.3.tar` & `rfb_driver_ea-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:54:09.706729 rfb_driver_ea-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-05-16 09:54:09.702729 rfb_driver_ea-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:54:09.706729 rfb_driver_ea-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:54:09.702729 rfb_driver_ea-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:54:09.702729 rfb_driver_ea-0.0.3/src/rfb_driver_ea/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    25331 2024-05-16 09:53:55.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea/drv_ea.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:54:09.702729 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 09:54:09.000000 rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:50:38.000609 rfb_driver_ea-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 07:50:23.000000 rfb_driver_ea-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 07:50:23.000000 rfb_driver_ea-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-05-20 07:50:38.000609 rfb_driver_ea-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 07:50:23.000000 rfb_driver_ea-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-20 07:50:23.000000 rfb_driver_ea-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 07:50:23.000000 rfb_driver_ea-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 07:50:38.000609 rfb_driver_ea-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:50:37.996609 rfb_driver_ea-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:50:38.000609 rfb_driver_ea-0.0.4/src/rfb_driver_ea/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 07:50:23.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 07:50:37.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-20 07:50:23.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25220 2024-05-20 07:50:23.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea/drv_ea.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:50:38.000609 rfb_driver_ea-0.0.4/src/rfb_driver_ea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42503 2024-05-20 07:50:37.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 07:50:37.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:50:37.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 07:50:37.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 07:50:37.000000 rfb_driver_ea-0.0.4/src/rfb_driver_ea.egg-info/top_level.txt
```

### Comparing `rfb_driver_ea-0.0.3/LICENSE.txt` & `rfb_driver_ea-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rfb_driver_ea-0.0.3/PKG-INFO` & `rfb_driver_ea-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-driver-ea
-Version: 0.0.3
+Version: 0.0.4
 Summary: Driver to control EA Power Electronics devices.
 Author-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 Maintainer-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rfb_driver_ea-0.0.3/pyproject.toml` & `rfb_driver_ea-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rfb_driver_ea-0.0.3/src/rfb_driver_ea/context.py` & `rfb_driver_ea-0.0.4/src/rfb_driver_ea/context.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_ea-0.0.3/src/rfb_driver_ea/drv_ea.py` & `rfb_driver_ea-0.0.4/src/rfb_driver_ea/drv_ea.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         Returns:
             None
         """
         i = 0
         while i < DEFAULT_MAX_READS and not self.__rx_chan.is_empty(): #pylint: disable=too-many-nested-blocks
             msg: DrvScpiCmdDataC = self.__rx_chan.receive_data_unblocking()
             if msg is not None:
-                log.critical(f"Message received: {msg.data_type.name}")
+                log.debug(f"Message received: {msg.data_type.name}")
                 if msg.data_type == DrvScpiCmdTypeE.ERROR:
 
                     log.critical("ERROR DEVICE NOT ADDED IN SCPI")
                     add_msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.ADD_DEV,
                                     port = self.__port,
                                     payload = self.__config,
                                     rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1])
@@ -350,16 +350,14 @@
         if self.properties.max_power_limit != 0:
             max_power_limit = self.properties.max_power_limit / _MILI_UNITS
             if current * voltage > max_power_limit:
                 voltage = max_power_limit / curr_ref
         else:
             current = 0
             voltage = 0
-        log.critical(self.properties.model)
-        log.critical(self.properties.model.startswith("PSB"))
         if self.properties.model.startswith("PSB"):
             msg = DrvScpiCmdDataC(data_type = DrvScpiCmdTypeE.WRITE,
                 rx_chan_name = DEFAULT_RX_CHAN+'_'+self.__port.split('/')[-1],
                 port = self.__port, payload = "SINK:"+_ScpiCmds.SEND_CURR.value + str(current))
             self.__tx_chan.send_data(msg)
             self.read_buffer()
```

### Comparing `rfb_driver_ea-0.0.3/src/rfb_driver_ea.egg-info/PKG-INFO` & `rfb_driver_ea-0.0.4/src/rfb_driver_ea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb-driver-ea
-Version: 0.0.3
+Version: 0.0.4
 Summary: Driver to control EA Power Electronics devices.
 Author-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 Maintainer-email: Raldea <r.aldea.csic+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```


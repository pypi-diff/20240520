# Comparing `tmp/mm_wlan-0.3.tar.gz` & `tmp/mm_wlan-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mm_wlan-0.3.tar", last modified: Thu Jan 11 15:39:47 2024, max compression
+gzip compressed data, was "mm_wlan-0.4.tar", last modified: Mon May 20 13:15:56 2024, max compression
```

## Comparing `mm_wlan-0.3.tar` & `mm_wlan-0.4.tar`

### file list

```diff
@@ -1,7 +1,14 @@
-drwxr-xr-x   0 si         (502) staff       (20)        0 2024-01-11 15:39:47.634813 mm_wlan-0.3/
--rw-r--r--   0 si         (502) staff       (20)      690 2024-01-11 15:39:47.634975 mm_wlan-0.3/PKG-INFO
-drwxr-xr-x   0 si         (502) staff       (20)        0 2024-01-11 15:39:47.634724 mm_wlan-0.3/mm_wlan/
--rw-r--r--   0 si         (502) staff       (20)       61 2024-01-11 15:35:33.645965 mm_wlan-0.3/mm_wlan/__init__.py
--rw-------   0 si         (502) staff       (20)      952 2022-09-09 11:32:13.991000 mm_wlan-0.3/mm_wlan/mm_wlan.py
--rw-r--r--   0 si         (502) staff       (20)       61 2023-10-05 12:41:54.026000 mm_wlan-0.3/setup.cfg
--rw-r--r--   0 si         (502) staff       (20)      889 2024-01-11 15:39:11.650849 mm_wlan-0.3/setup.py
+drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-20 13:15:56.125109 mm_wlan-0.4/
+-rw-r--r--   0 si         (502) staff       (20)     1062 2023-10-05 12:41:54.000000 mm_wlan-0.4/LICENSE.txt
+-rw-r--r--   0 si         (502) staff       (20)      701 2024-05-20 13:15:56.124828 mm_wlan-0.4/PKG-INFO
+-rw-r--r--   0 si         (502) staff       (20)     2053 2024-05-20 13:05:12.000000 mm_wlan-0.4/README.md
+drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-20 13:15:56.121532 mm_wlan-0.4/mm_wlan/
+-rw-r--r--   0 si         (502) staff       (20)       61 2024-01-11 15:35:33.000000 mm_wlan-0.4/mm_wlan/__init__.py
+-rw-r--r--   0 si         (502) staff       (20)     1119 2024-05-20 13:05:12.000000 mm_wlan-0.4/mm_wlan/mm_wlan.py
+drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-20 13:15:56.124203 mm_wlan-0.4/mm_wlan.egg-info/
+-rw-r--r--   0 si         (502) staff       (20)      701 2024-05-20 13:15:56.000000 mm_wlan-0.4/mm_wlan.egg-info/PKG-INFO
+-rw-r--r--   0 si         (502) staff       (20)      203 2024-05-20 13:15:56.000000 mm_wlan-0.4/mm_wlan.egg-info/SOURCES.txt
+-rw-r--r--   0 si         (502) staff       (20)        1 2024-05-20 13:15:56.000000 mm_wlan-0.4/mm_wlan.egg-info/dependency_links.txt
+-rw-r--r--   0 si         (502) staff       (20)        8 2024-05-20 13:15:56.000000 mm_wlan-0.4/mm_wlan.egg-info/top_level.txt
+-rw-r--r--   0 si         (502) staff       (20)       79 2024-05-20 13:15:56.125723 mm_wlan-0.4/setup.cfg
+-rw-r--r--   0 si         (502) staff       (20)      913 2024-05-20 13:14:39.000000 mm_wlan-0.4/setup.py
```

### Comparing `mm_wlan-0.3/PKG-INFO` & `mm_wlan-0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mm_wlan
-Version: 0.3
+Version: 0.4
 Summary: WLAN Connection functions in MicroPython
 Home-page: https://github.com/monkmakes/mm_wlan
-Author: Simon Monk
+Download-URL: https://github.com/monkmakes/mm_wlan/archive/refs/tags/v_02.tar.gz
+Author: Simon Monk and José Antonio Vacas
 Author-email: simon@monkmakes.com
 License: MIT
-Download-URL: https://github.com/monkmakes/mm_wlan/archive/refs/tags/v_02.tar.gz
-Description: UNKNOWN
 Keywords: WLAN,micropython,webserver
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE.txt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mm_wlan-0.3/mm_wlan/mm_wlan.py` & `mm_wlan-0.4/mm_wlan/mm_wlan.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,30 +3,40 @@
 --------
 The ``mm_wlan`` module defines a couple of methods to simplify connecting to a 
 wireless network. https://github.com/monkmakes/mm_wlan
 
 """
 
 
-import network, time
+import network, time, sys
 
 wlan = network.WLAN(network.STA_IF)
 
 def connect_to_network(ssid, password, retries=10, verbose=True):
     wlan.active(True)
-    wlan.config(pm = 0xa11140)  # Disable power-save mode
+    if sys.platform != 'esp32':
+        wlan.config(pm = 0xa11140)  # Disable power-save mode
     wlan.connect(ssid, password)
     if verbose: print('Connecting to ' + ssid, end=' ')
         
     while retries > 0 and wlan.status() != network.STAT_GOT_IP:
         retries -= 1
         if verbose: print('.', end='')
         time.sleep(1)    
         
-    if wlan.status() != network.STAT_GOT_IP:
+    if is_connected():
         if verbose: print('\nConnection failed. Check ssid and password')
         raise RuntimeError('WLAN connection failed')
     else:
-        if verbose: print('\nConnected. IP Address = ' + wlan.ifconfig()[0])
+        if verbose: print('\nConnected. IP Address = ' + get_ip())
+
+def get_ip():
+    if is_connected():
+        return wlan.ifconfig()[0]
+    else:
+        if verbose: print('\nNot connected')
+        return None
+        
 
 def is_connected():
-    return wlan.status() == network.STAT_GOT_IP
+    return wlan.status() == network.STAT_GOT_IP
+
```

### Comparing `mm_wlan-0.3/setup.py` & `mm_wlan-0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 setup(
   name = 'mm_wlan',         
   packages = ['mm_wlan'],   
-  version = '0.3',      
+  version = '0.4',      
   license='MIT',       
   description = 'WLAN Connection functions in MicroPython',  
-  author = 'Simon Monk',                  
+  author = 'Simon Monk and José Antonio Vacas',                  
   author_email = 'simon@monkmakes.com',      
   url = 'https://github.com/monkmakes/mm_wlan',  
   download_url = 'https://github.com/monkmakes/mm_wlan/archive/refs/tags/v_02.tar.gz',   
   keywords = ['WLAN', 'micropython', 'webserver'],  
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


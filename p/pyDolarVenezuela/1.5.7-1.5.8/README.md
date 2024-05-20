# Comparing `tmp/pydolarvenezuela-1.5.7.tar.gz` & `tmp/pydolarvenezuela-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.5.7.tar", last modified: Sun May 19 07:38:30 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.5.8.tar", last modified: Mon May 20 18:40:53 2024, max compression
```

## Comparing `pydolarvenezuela-1.5.7.tar` & `pydolarvenezuela-1.5.8.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 07:38:30.795722 pydolarvenezuela-1.5.7/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.7/LICENSE
--rw-rw-rw-   0        0        0     7221 2024-05-19 07:38:30.790725 pydolarvenezuela-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     4830 2024-05-08 05:23:24.000000 pydolarvenezuela-1.5.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 07:38:30.512719 pydolarvenezuela-1.5.7/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2879 2024-05-19 07:37:22.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:38:30.544718 pydolarvenezuela-1.5.7/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:38:30.694720 pydolarvenezuela-1.5.7/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/models/images.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:38:30.730721 pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     5657 2024-05-19 07:33:09.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2328 2024-05-19 06:17:16.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2081 2024-05-19 06:50:07.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2627 2024-05-19 05:56:01.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1282 2024-05-04 08:02:51.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:38:30.744727 pydolarvenezuela-1.5.7/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0    12380 2024-05-19 06:16:03.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:38:30.779722 pydolarvenezuela-1.5.7/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7221 2024-05-19 07:38:29.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2024-05-19 07:38:30.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 07:38:29.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-19 07:38:30.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 07:38:30.000000 pydolarvenezuela-1.5.7/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-05-19 07:37:34.000000 pydolarvenezuela-1.5.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-19 07:38:30.796723 pydolarvenezuela-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-05-19 07:37:28.000000 pydolarvenezuela-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:40:53.067018 pydolarvenezuela-1.5.8/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.8/LICENSE
+-rw-rw-rw-   0        0        0     7221 2024-05-20 18:40:53.050974 pydolarvenezuela-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4830 2024-05-08 05:23:24.000000 pydolarvenezuela-1.5.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 18:40:52.765226 pydolarvenezuela-1.5.8/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2879 2024-05-20 18:40:00.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:40:52.823647 pydolarvenezuela-1.5.8/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:40:52.881963 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/images.py
+-rw-rw-rw-   0        0        0      773 2024-05-20 18:37:09.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/monitor.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:40:52.986001 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     5651 2024-05-20 18:32:08.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2328 2024-05-19 06:17:16.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2081 2024-05-19 06:50:07.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2627 2024-05-19 05:56:01.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1282 2024-05-04 08:02:51.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:40:53.050974 pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0    12380 2024-05-19 06:16:03.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:40:53.050974 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7221 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 18:40:52.000000 pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-05-20 18:40:16.000000 pydolarvenezuela-1.5.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 18:40:53.067018 pydolarvenezuela-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-05-20 18:40:10.000000 pydolarvenezuela-1.5.8/setup.py
```

### Comparing `pydolarvenezuela-1.5.7/LICENSE` & `pydolarvenezuela-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/PKG-INFO` & `pydolarvenezuela-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.7
+Version: 1.5.8
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.5.7/README.md` & `pydolarvenezuela-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import network
 from .models.pages import Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.5.7'
+version = '1.5.8'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca
```

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 from typing import Any
+from dataclasses import asdict
 from .bcv import BCV
 from .criptodolar import CriptoDolar
 from .exchangemonitor import ExchangeMonitor
 from .italcambio import Italcambio
 
 from ..data.redis import Cache
+from ..models.monitor import MonitorDB
 from ..models.database import Redis
 from ..models.pages import Page
 from ..pages import BCV as B, CriptoDolar as C, ExchangeMonitor as E, Italcambio as I
 from ..utils import currencies_list
 
 monitor_classes = [
     {
@@ -61,22 +63,19 @@
                 value = monitor_data[name_property]
                 return f'Bs. {value}' if prettify and name_property == 'price' else value
             return monitor_data
         except KeyError:
             raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
 
     def _update_item(existing_data_dict: dict, i: Any, last_data: dict):
+        structure_monitor = asdict(MonitorDB(**existing_data_dict[i]))
         for key in list(existing_data_dict[i].keys()):
-            if key not in last_data[i]:
+            if structure_monitor[key] is None:
                 del existing_data_dict[i][key]
         
-        for key in last_data[i].keys():
-            if key not in existing_data_dict[i]:
-                existing_data_dict[i][key] = last_data[i][key]
-
         if existing_data_dict[i]['price'] != last_data[i]['price']:
             price = existing_data_dict[i]['price']
             new_price = last_data[i]['price']
             price_old = last_data[i].get('price_old', None)
             change  = round(float(new_price - price), 2)
             percent = float(f'{round(float((change / new_price) * 100 if price != 0 else 0), 2)}'.replace('-', ' '))
             symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
```

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/provider/italcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.5.8/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.7
+Version: 1.5.8
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.5.7/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.5.8/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pyDolarVenezuela.egg-info/requires.txt
 pyDolarVenezuela.egg-info/top_level.txt
 pyDolarVenezuela/data/__init__.py
 pyDolarVenezuela/data/redis.py
 pyDolarVenezuela/models/__init__.py
 pyDolarVenezuela/models/database.py
 pyDolarVenezuela/models/images.py
+pyDolarVenezuela/models/monitor.py
 pyDolarVenezuela/models/pages.py
 pyDolarVenezuela/provider/__init__.py
 pyDolarVenezuela/provider/bcv.py
 pyDolarVenezuela/provider/criptodolar.py
 pyDolarVenezuela/provider/exchangemonitor.py
 pyDolarVenezuela/provider/italcambio.py
 pyDolarVenezuela/tools/__init__.py
```

### Comparing `pydolarvenezuela-1.5.7/pyproject.toml` & `pydolarvenezuela-1.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.5.7"
+version = "1.5.8"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.5.7/setup.py` & `pydolarvenezuela-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.5.7'
+VERSION = '1.5.8'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```


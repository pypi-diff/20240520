# Comparing `tmp/duwi_smarthome_sdk-0.1.2.tar.gz` & `tmp/duwi_smarthome_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smarthome_sdk-0.1.2.tar", last modified: Wed May 15 08:28:02 2024, max compression
+gzip compressed data, was "duwi_smarthome_sdk-0.1.3.tar", last modified: Mon May 20 07:44:27 2024, max compression
```

## Comparing `duwi_smarthome_sdk-0.1.2.tar` & `duwi_smarthome_sdk-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.494152 duwi_smarthome_sdk-0.1.2/
--rw-rw-rw-   0        0        0      705 2024-05-15 08:28:02.493170 duwi_smarthome_sdk-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-05-15 08:27:04.000000 duwi_smarthome_sdk-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.449229 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.467780 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2428 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/account.py
--rw-rw-rw-   0        0        0     1759 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/control.py
--rw-rw-rw-   0        0        0     4536 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2647 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/floor.py
--rw-rw-rw-   0        0        0     2675 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/house.py
--rw-rw-rw-   0        0        0     2145 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     2755 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/room.py
--rw-rw-rw-   0        0        0     3137 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/terminal.py
--rw-rw-rw-   0        0        0     4788 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.472664 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       91 2024-05-15 08:04:07.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.473641 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.476571 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.485360 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/floor.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/room.py
--rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/terminal.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.489263 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.492196 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/
--rw-rw-rw-   0        0        0      705 2024-05-15 08:28:02.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2024-05-15 08:28:02.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 08:28:02.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-15 08:28:02.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-15 08:28:02.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-15 08:28:02.000000 duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 08:28:02.494152 duwi_smarthome_sdk-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      937 2024-05-15 08:27:25.000000 duwi_smarthome_sdk-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:28:02.491217 duwi_smarthome_sdk-0.1.2/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.661948 duwi_smarthome_sdk-0.1.3/
+-rw-rw-rw-   0        0        0      705 2024-05-20 07:44:27.660379 duwi_smarthome_sdk-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-05-15 08:27:04.000000 duwi_smarthome_sdk-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.603898 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.623930 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2428 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/account.py
+-rw-rw-rw-   0        0        0     1759 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4536 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2647 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/floor.py
+-rw-rw-rw-   0        0        0     2675 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2145 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2755 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/room.py
+-rw-rw-rw-   0        0        0     3137 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/terminal.py
+-rw-rw-rw-   0        0        0     4788 2024-05-15 08:25:26.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.627898 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       91 2024-05-15 08:04:07.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/const/const.py
+-rw-rw-rw-   0        0        0      603 2024-05-20 07:42:46.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.630533 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.633100 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.644390 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/floor.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/room.py
+-rw-rw-rw-   0        0        0     1185 2024-05-14 02:44:23.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.655540 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.659345 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/
+-rw-rw-rw-   0        0        0      705 2024-05-20 07:44:27.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2024-05-20 07:44:27.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:44:27.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-20 07:44:27.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-20 07:44:27.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-20 07:44:27.000000 duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:44:27.662080 duwi_smarthome_sdk-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      937 2024-05-20 07:42:58.000000 duwi_smarthome_sdk-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:44:27.656544 duwi_smarthome_sdk-0.1.3/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smarthome_sdk-0.1.3/test/__init__.py
```

### Comparing `duwi_smarthome_sdk-0.1.2/PKG-INFO` & `duwi_smarthome_sdk-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: duwitech@163.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/account.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/control.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/discover.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/floor.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/house.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/refresh_token.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/room.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/terminal.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/api/ws.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/const/status.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/const/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,7 +17,9 @@
     SYSTEM_RATE_LIMIT = '99004'
     # 系统分钟频率限制
     SYSTEM_MINUTE_RATE_LIMIT = '99005'
     # 系统小时频率限制
     SYSTEM_HOUR_RATE_LIMIT = '99006'
     # 网关系统错误
     GATEWAY_SYS_ERROR = '99999'
+
+
```

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/const/type_map.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/req/device_control.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/auth.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/device.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/floor.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/house.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/room.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/model/resp/terminal.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/model/resp/terminal.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/util/http.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk/util/sign.py` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/PKG-INFO` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smarthome_sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: sdk for duwi third platform
 Home-page: https://github.com/duwi2024/homeassistant-sdk
 Author: duwi
 Author-email: duwitech@163.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smarthome_sdk-0.1.2/duwi_smarthome_sdk.egg-info/SOURCES.txt` & `duwi_smarthome_sdk-0.1.3/duwi_smarthome_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smarthome_sdk-0.1.2/setup.py` & `duwi_smarthome_sdk-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smarthome_sdk",
     version=VERSION,
     author="duwi",
     author_email="duwitech@163.com",
```


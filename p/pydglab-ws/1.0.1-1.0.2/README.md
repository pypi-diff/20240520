# Comparing `tmp/pydglab_ws-1.0.1.tar.gz` & `tmp/pydglab_ws-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydglab_ws-1.0.1.tar", max compression
+gzip compressed data, was "pydglab_ws-1.0.2.tar", max compression
```

## Comparing `pydglab_ws-1.0.1.tar` & `pydglab_ws-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1535 2024-05-19 08:12:18.910165 pydglab_ws-1.0.1/LICENSE
--rw-r--r--   0        0        0     6092 2024-05-19 08:12:18.910165 pydglab_ws-1.0.1/README.md
--rw-r--r--   0        0        0      179 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/__init__.py
--rw-r--r--   0        0        0       82 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/client/__init__.py
--rw-r--r--   0        0        0     9795 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/client/base.py
--rw-r--r--   0        0        0      923 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/client/connect.py
--rw-r--r--   0        0        0     1552 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/client/local.py
--rw-r--r--   0        0        0     1910 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/client/ws.py
--rw-r--r--   0        0        0     3433 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/enums.py
--rw-r--r--   0        0        0      724 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/exceptions.py
--rw-r--r--   0        0        0     3214 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/models.py
--rw-r--r--   0        0        0       22 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/server/__init__.py
--rw-r--r--   0        0        0    17992 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/server/server.py
--rw-r--r--   0        0        0      755 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/typing.py
--rw-r--r--   0        0        0     4032 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pydglab_ws/utils.py
--rw-r--r--   0        0        0     1293 2024-05-19 08:12:18.914165 pydglab_ws-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7176 1970-01-01 00:00:00.000000 pydglab_ws-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1535 2024-05-20 06:36:18.807150 pydglab_ws-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6092 2024-05-20 06:36:18.807150 pydglab_ws-1.0.2/README.md
+-rw-r--r--   0        0        0      179 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/__init__.py
+-rw-r--r--   0        0        0     9795 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/base.py
+-rw-r--r--   0        0        0      923 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/connect.py
+-rw-r--r--   0        0        0     1552 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/local.py
+-rw-r--r--   0        0        0     1910 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/client/ws.py
+-rw-r--r--   0        0        0     3433 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/enums.py
+-rw-r--r--   0        0        0      724 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/exceptions.py
+-rw-r--r--   0        0        0     3214 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/models.py
+-rw-r--r--   0        0        0       22 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/server/__init__.py
+-rw-r--r--   0        0        0    17992 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/server/server.py
+-rw-r--r--   0        0        0      755 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/typing.py
+-rw-r--r--   0        0        0     4032 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pydglab_ws/utils.py
+-rw-r--r--   0        0        0     1293 2024-05-20 06:36:18.811150 pydglab_ws-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7176 1970-01-01 00:00:00.000000 pydglab_ws-1.0.2/PKG-INFO
```

### Comparing `pydglab_ws-1.0.1/LICENSE` & `pydglab_ws-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/README.md` & `pydglab_ws-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/client/base.py` & `pydglab_ws-1.0.2/pydglab_ws/client/base.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/client/connect.py` & `pydglab_ws-1.0.2/pydglab_ws/client/connect.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/client/local.py` & `pydglab_ws-1.0.2/pydglab_ws/client/local.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/client/ws.py` & `pydglab_ws-1.0.2/pydglab_ws/client/ws.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/enums.py` & `pydglab_ws-1.0.2/pydglab_ws/enums.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/exceptions.py` & `pydglab_ws-1.0.2/pydglab_ws/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/models.py` & `pydglab_ws-1.0.2/pydglab_ws/models.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/server/server.py` & `pydglab_ws-1.0.2/pydglab_ws/server/server.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/typing.py` & `pydglab_ws-1.0.2/pydglab_ws/typing.py`

 * *Files identical despite different names*

### Comparing `pydglab_ws-1.0.1/pydglab_ws/utils.py` & `pydglab_ws-1.0.2/pydglab_ws/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,18 +109,17 @@
     生成下放波形操作的数据
 
     :param channel: 通道选择
     :param pulses: 波形操作数据
     :return: 返回数据可作为 WebSocket 消息中的 ``message``
     :raise InvalidPulseOperation: [`InvalidPulseOperation`][pydglab_ws.exceptions.InvalidPulseOperation]
     """
-    dict_data = {
-        f"{MessageDataHead.PULSE.value}-{channel.value}": [dump_pulse_operation(pulse) for pulse in pulses]
-    }
-    return json.dumps(dict_data)
+
+    return (f"{MessageDataHead.PULSE.value}-{channel.name}"
+            f":{json.dumps([dump_pulse_operation(pulse) for pulse in pulses], separators=(',', ':'))}")
 
 
 def dg_lab_client_qrcode(uri: str, client_id: UUID4) -> str:
     """
     生成终端二维码，二维码图像需要自行生成
 
     :param uri: WebSocket 服务端 URI，例如：``ws://107.47.91.92:4567``
```

### Comparing `pydglab_ws-1.0.1/pyproject.toml` & `pydglab_ws-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydglab-ws"
-version = "1.0.1"
+version = "1.0.2"
 description = "一个通过 WebSocket 控制郊狼 DG-Lab 的 Python 库"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.asia>"]
 readme = "README.md"
 homepage = "https://pydglab-ws.readthedocs.io"
 repository = "https://github.com/Ljzd-PRO/PyDGLab-WS"
 documentation = "https://pydglab-ws.readthedocs.io"
```

### Comparing `pydglab_ws-1.0.1/PKG-INFO` & `pydglab_ws-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydglab-ws
-Version: 1.0.1
+Version: 1.0.2
 Summary: 一个通过 WebSocket 控制郊狼 DG-Lab 的 Python 库
 Home-page: https://pydglab-ws.readthedocs.io
 Keywords: dg-lab,dg-lab-v3,websocket,library,os-independent
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.asia
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
```


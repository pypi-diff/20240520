# Comparing `tmp/opentakserver-1.1.8.tar.gz` & `tmp/opentakserver-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentakserver-1.1.8.tar", max compression
+gzip compressed data, was "opentakserver-1.1.9.tar", max compression
```

## Comparing `opentakserver-1.1.8.tar` & `opentakserver-1.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.8/LICENSE
--rw-r--r--   0        0        0      125 2024-05-10 13:07:25.180510 opentakserver-1.1.8/opentakserver/__init__.py
--rw-r--r--   0        0        0    11359 2024-05-10 01:15:33.729313 opentakserver-1.1.8/opentakserver/app.py
--rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.8/opentakserver/blueprints/__init__.py
--rw-r--r--   0        0        0    46981 2024-05-10 01:15:33.731265 opentakserver-1.1.8/opentakserver/blueprints/api.py
--rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.8/opentakserver/blueprints/config.py
--rw-r--r--   0        0        0    26797 2024-05-10 13:01:12.713678 opentakserver-1.1.8/opentakserver/blueprints/marti.py
--rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.8/opentakserver/blueprints/ots_socketio.py
--rw-r--r--   0        0        0     4580 2024-04-21 19:26:51.395692 opentakserver-1.1.8/opentakserver/blueprints/scheduled_jobs.py
--rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.8/opentakserver/blueprints/scheduler_api.py
--rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.8/opentakserver/ca_config.py
--rw-r--r--   0        0        0    21365 2024-05-10 01:15:33.733274 opentakserver-1.1.8/opentakserver/certificate_authority.py
--rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.8/opentakserver/controllers/__init__.py
--rw-r--r--   0        0        0    10751 2024-05-10 01:15:33.734257 opentakserver-1.1.8/opentakserver/controllers/client_controller.py
--rw-r--r--   0        0        0    35116 2024-05-10 01:15:43.056867 opentakserver-1.1.8/opentakserver/controllers/cot_controller.py
--rw-r--r--   0        0        0     4153 2024-05-10 01:15:33.736251 opentakserver-1.1.8/opentakserver/defaultconfig.py
--rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.8/opentakserver/EmailValidator.py
--rw-r--r--   0        0        0      377 2024-05-10 01:15:33.738247 opentakserver-1.1.8/opentakserver/extensions.py
--rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.8/opentakserver/forms/__init__.py
--rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.8/opentakserver/forms/MediaMTXGlobalConfig.py
--rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.8/opentakserver/forms/MediaMTXPathConfig.py
--rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.8/opentakserver/functions.py
--rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.8/opentakserver/models/__init__.py
--rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.8/opentakserver/models/Alert.py
--rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.8/opentakserver/models/Base.py
--rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.8/opentakserver/models/CasEvac.py
--rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.8/opentakserver/models/Certificate.py
--rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.8/opentakserver/models/Chatrooms.py
--rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.8/opentakserver/models/ChatroomsUids.py
--rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.8/opentakserver/models/Config.py
--rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.8/opentakserver/models/CoT.py
--rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.8/opentakserver/models/DataPackage.py
--rw-r--r--   0        0        0     3716 2024-05-10 01:15:33.739243 opentakserver-1.1.8/opentakserver/models/EUD.py
--rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.8/opentakserver/models/GeoChat.py
--rw-r--r--   0        0        0     1427 2024-05-10 01:15:33.740241 opentakserver-1.1.8/opentakserver/models/Icon.py
--rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.8/opentakserver/models/Marker.py
--rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.8/opentakserver/models/Point.py
--rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.8/opentakserver/models/RBLine.py
--rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.8/opentakserver/models/role.py
--rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.8/opentakserver/models/Team.py
--rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.8/opentakserver/models/user.py
--rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.8/opentakserver/models/VideoRecording.py
--rw-r--r--   0        0        0     5476 2024-04-16 19:41:24.153676 opentakserver-1.1.8/opentakserver/models/VideoStream.py
--rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.8/opentakserver/models/WebAuthn.py
--rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.8/opentakserver/models/ZMIST.py
--rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.8/opentakserver/mumble/__init__.py
--rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.8/opentakserver/mumble/mumble_authenticator.py
--rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.8/opentakserver/mumble/mumble_ice_app.py
--rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.8/opentakserver/mumble/Murmur.ice
--rw-r--r--   0        0        0      524 2024-05-10 01:15:33.726316 opentakserver-1.1.8/opentakserver/PasswordValidator.py
--rw-r--r--   0        0        0     3527 2024-04-25 01:40:11.215290 opentakserver-1.1.8/opentakserver/SocketServer.py
--rw-r--r--   0        0        0     1679 2024-05-10 13:07:25.173527 opentakserver-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     2073 2024-04-11 21:18:43.687758 opentakserver-1.1.8/README.md
--rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 opentakserver-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.9/LICENSE
+-rw-r--r--   0        0        0      125 2024-05-15 19:38:48.377285 opentakserver-1.1.9/opentakserver/__init__.py
+-rw-r--r--   0        0        0    11359 2024-05-15 19:08:47.119054 opentakserver-1.1.9/opentakserver/app.py
+-rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.9/opentakserver/blueprints/__init__.py
+-rw-r--r--   0        0        0    46981 2024-05-15 19:08:47.121048 opentakserver-1.1.9/opentakserver/blueprints/api.py
+-rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.9/opentakserver/blueprints/config.py
+-rw-r--r--   0        0        0    26797 2024-05-15 19:08:47.123044 opentakserver-1.1.9/opentakserver/blueprints/marti.py
+-rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.9/opentakserver/blueprints/ots_socketio.py
+-rw-r--r--   0        0        0     4580 2024-04-21 19:26:51.395692 opentakserver-1.1.9/opentakserver/blueprints/scheduled_jobs.py
+-rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.9/opentakserver/blueprints/scheduler_api.py
+-rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.9/opentakserver/ca_config.py
+-rw-r--r--   0        0        0    21365 2024-05-15 19:08:47.125039 opentakserver-1.1.9/opentakserver/certificate_authority.py
+-rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.9/opentakserver/controllers/__init__.py
+-rw-r--r--   0        0        0    10751 2024-05-15 19:08:47.127035 opentakserver-1.1.9/opentakserver/controllers/client_controller.py
+-rw-r--r--   0        0        0    35116 2024-05-15 19:14:37.833569 opentakserver-1.1.9/opentakserver/controllers/cot_controller.py
+-rw-r--r--   0        0        0     4153 2024-05-15 19:08:47.129027 opentakserver-1.1.9/opentakserver/defaultconfig.py
+-rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.9/opentakserver/EmailValidator.py
+-rw-r--r--   0        0        0      377 2024-05-15 19:08:47.131037 opentakserver-1.1.9/opentakserver/extensions.py
+-rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.9/opentakserver/forms/__init__.py
+-rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.9/opentakserver/forms/MediaMTXGlobalConfig.py
+-rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.9/opentakserver/forms/MediaMTXPathConfig.py
+-rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.9/opentakserver/functions.py
+-rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.9/opentakserver/models/__init__.py
+-rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.9/opentakserver/models/Alert.py
+-rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.9/opentakserver/models/Base.py
+-rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.9/opentakserver/models/CasEvac.py
+-rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.9/opentakserver/models/Certificate.py
+-rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.9/opentakserver/models/Chatrooms.py
+-rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.9/opentakserver/models/ChatroomsUids.py
+-rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.9/opentakserver/models/Config.py
+-rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.9/opentakserver/models/CoT.py
+-rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.9/opentakserver/models/DataPackage.py
+-rw-r--r--   0        0        0     3716 2024-05-15 19:08:47.132021 opentakserver-1.1.9/opentakserver/models/EUD.py
+-rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.9/opentakserver/models/GeoChat.py
+-rw-r--r--   0        0        0     1427 2024-05-15 19:08:47.133019 opentakserver-1.1.9/opentakserver/models/Icon.py
+-rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.9/opentakserver/models/Marker.py
+-rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.9/opentakserver/models/Point.py
+-rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.9/opentakserver/models/RBLine.py
+-rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.9/opentakserver/models/role.py
+-rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.9/opentakserver/models/Team.py
+-rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.9/opentakserver/models/user.py
+-rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.9/opentakserver/models/VideoRecording.py
+-rw-r--r--   0        0        0     5476 2024-04-16 19:41:24.153676 opentakserver-1.1.9/opentakserver/models/VideoStream.py
+-rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.9/opentakserver/models/WebAuthn.py
+-rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.9/opentakserver/models/ZMIST.py
+-rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.9/opentakserver/mumble/__init__.py
+-rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.9/opentakserver/mumble/mumble_authenticator.py
+-rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.9/opentakserver/mumble/mumble_ice_app.py
+-rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.9/opentakserver/mumble/Murmur.ice
+-rw-r--r--   0        0        0      524 2024-05-15 19:08:47.115067 opentakserver-1.1.9/opentakserver/PasswordValidator.py
+-rw-r--r--   0        0        0     3527 2024-04-25 01:40:11.215290 opentakserver-1.1.9/opentakserver/SocketServer.py
+-rw-r--r--   0        0        0     1679 2024-05-15 19:38:48.365315 opentakserver-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2073 2024-04-11 21:18:43.687758 opentakserver-1.1.9/README.md
+-rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 opentakserver-1.1.9/PKG-INFO
```

### Comparing `opentakserver-1.1.8/LICENSE` & `opentakserver-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/app.py` & `opentakserver-1.1.9/opentakserver/app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/blueprints/api.py` & `opentakserver-1.1.9/opentakserver/blueprints/api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/blueprints/config.py` & `opentakserver-1.1.9/opentakserver/blueprints/config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/blueprints/marti.py` & `opentakserver-1.1.9/opentakserver/blueprints/marti.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/blueprints/ots_socketio.py` & `opentakserver-1.1.9/opentakserver/blueprints/ots_socketio.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/blueprints/scheduled_jobs.py` & `opentakserver-1.1.9/opentakserver/blueprints/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/blueprints/scheduler_api.py` & `opentakserver-1.1.9/opentakserver/blueprints/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/ca_config.py` & `opentakserver-1.1.9/opentakserver/ca_config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/certificate_authority.py` & `opentakserver-1.1.9/opentakserver/certificate_authority.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/controllers/client_controller.py` & `opentakserver-1.1.9/opentakserver/controllers/client_controller.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/controllers/cot_controller.py` & `opentakserver-1.1.9/opentakserver/controllers/cot_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             chat_group = event.find('chatgrp')
             remarks = event.find('remarks')
 
             chatroom = Chatroom()
 
             chatroom.name = chat.attrs['chatroom']
             chatroom.id = chat.attrs['id']
-            chatroom.parent = chat.attrs['parent']
+            chatroom.parent = chat.attrs['parent'] if 'parent' in chat.attrs else None
 
             with self.context:
                 try:
                     self.db.session.add(chatroom)
                     self.db.session.commit()
                 except exc.IntegrityError:
                     self.db.session.rollback()
@@ -698,15 +698,14 @@
             return "uav"
 
     def on_message(self, unused_channel, basic_deliver, properties, body):
         try:
             body = json.loads(body)
             soup = BeautifulSoup(body['cot'], 'xml')
             event = soup.find('event')
-            self.logger.info(event)
             if event:
                 self.parse_device_info(body['uid'], soup, event)
                 cot_pk = self.insert_cot(soup, event, body['uid'])
                 point_pk = self.parse_point(event, body['uid'], cot_pk)
                 self.parse_geochat(event, cot_pk, point_pk)
                 self.parse_video(event, cot_pk)
                 self.parse_alert(event, body['uid'], point_pk, cot_pk)
```

### Comparing `opentakserver-1.1.8/opentakserver/defaultconfig.py` & `opentakserver-1.1.9/opentakserver/defaultconfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/EmailValidator.py` & `opentakserver-1.1.9/opentakserver/EmailValidator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/forms/MediaMTXGlobalConfig.py` & `opentakserver-1.1.9/opentakserver/forms/MediaMTXGlobalConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/forms/MediaMTXPathConfig.py` & `opentakserver-1.1.9/opentakserver/forms/MediaMTXPathConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/Alert.py` & `opentakserver-1.1.9/opentakserver/models/Alert.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/CasEvac.py` & `opentakserver-1.1.9/opentakserver/models/CasEvac.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/Certificate.py` & `opentakserver-1.1.9/opentakserver/models/Certificate.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/Chatrooms.py` & `opentakserver-1.1.9/opentakserver/models/Chatrooms.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/ChatroomsUids.py` & `opentakserver-1.1.9/opentakserver/models/ChatroomsUids.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/CoT.py` & `opentakserver-1.1.9/opentakserver/models/CoT.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/DataPackage.py` & `opentakserver-1.1.9/opentakserver/models/DataPackage.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/EUD.py` & `opentakserver-1.1.9/opentakserver/models/EUD.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/GeoChat.py` & `opentakserver-1.1.9/opentakserver/models/GeoChat.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/Icon.py` & `opentakserver-1.1.9/opentakserver/models/Icon.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/Marker.py` & `opentakserver-1.1.9/opentakserver/models/Marker.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/Point.py` & `opentakserver-1.1.9/opentakserver/models/Point.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/RBLine.py` & `opentakserver-1.1.9/opentakserver/models/RBLine.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/Team.py` & `opentakserver-1.1.9/opentakserver/models/Team.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/user.py` & `opentakserver-1.1.9/opentakserver/models/user.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/VideoRecording.py` & `opentakserver-1.1.9/opentakserver/models/VideoRecording.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/VideoStream.py` & `opentakserver-1.1.9/opentakserver/models/VideoStream.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/models/ZMIST.py` & `opentakserver-1.1.9/opentakserver/models/ZMIST.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/mumble/mumble_authenticator.py` & `opentakserver-1.1.9/opentakserver/mumble/mumble_authenticator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/mumble/mumble_ice_app.py` & `opentakserver-1.1.9/opentakserver/mumble/mumble_ice_app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/mumble/Murmur.ice` & `opentakserver-1.1.9/opentakserver/mumble/Murmur.ice`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/PasswordValidator.py` & `opentakserver-1.1.9/opentakserver/PasswordValidator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/opentakserver/SocketServer.py` & `opentakserver-1.1.9/opentakserver/SocketServer.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/pyproject.toml` & `opentakserver-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenTAKServer"
-version = "1.1.8"
+version = "1.1.9"
 description = "A server for ATAK, WinTAK, and iTAK"
 authors = ["OpenTAKServer <opentakserver@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/brian7704/OpenTAKServer"
 documentation = "https://docs.opentakserver.io"
```

### Comparing `opentakserver-1.1.8/README.md` & `opentakserver-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.8/PKG-INFO` & `opentakserver-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenTAKServer
-Version: 1.1.8
+Version: 1.1.9
 Summary: A server for ATAK, WinTAK, and iTAK
 Home-page: https://github.com/brian7704/OpenTAKServer
 License: GPL-3.0-or-later
 Author: OpenTAKServer
 Author-email: opentakserver@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```


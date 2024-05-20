# Comparing `tmp/sais_notify-0.0.2.tar.gz` & `tmp/sais_notify-0.0.3.tar.gz`

## Comparing `sais_notify-0.0.2.tar` & `sais_notify-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.2/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/auth/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/auth/auth_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/clients/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/clients/notify_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/config/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/config/const.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/config/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/handler/__init__.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/handler/message_handler.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/model/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/model/message_model.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/types/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.2/.gitignore
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 sais_notify-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 sais_notify-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/auth/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/auth/auth_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/clients/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/clients/notify_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/config/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/config/const.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/config/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/handler/__init__.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/handler/message_handler.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/model/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/model/message_model.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/types/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sais_notify-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 sais_notify-0.0.3/PKG-INFO
```

### Comparing `sais_notify-0.0.2/README.md` & `sais_notify-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.2/sais/notify/clients/notify_client.py` & `sais_notify-0.0.3/sais/notify/clients/notify_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import json
 from http import HTTPStatus
 
 import requests
-from fastapi.logger import logger
-
+import logging
 from sais.notify.auth.auth_info import EnvVarCredentialsProvider
+from sais.notify.config.const import LOGGER_NAME
 from sais.notify.model import MessageModel
 
 
 class NotifyClient(object):
     def __init__(self, endpoint, auth_provider: EnvVarCredentialsProvider):
         self.endpoint = endpoint
         self.auth_provider = auth_provider
+        self.logger = logging.getLogger(LOGGER_NAME)
 
     def send_notification_feishu(self, message: MessageModel) -> bool:
         headers = {
             'Authorization': self.auth_provider.token,
             'Content-Type': 'application/json'
         }
 
         payload = message.model_dump_json()
         response = requests.post(f'{self.endpoint}/api/v1/notify/send', headers=headers, data=json.dumps(payload))
 
         if response.status_code == HTTPStatus.OK:
-            logger.info(f'Notification sent successfully')
+            self.logger.info(f'Notification sent successfully')
             return response.json()
         else:
             raise Exception(f'Error sending notification: {response.status_code} - {response.text}')
```

### Comparing `sais_notify-0.0.2/sais/notify/handler/message_handler.py` & `sais_notify-0.0.3/sais/notify/handler/message_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from fastapi.logger import logger
 
 from sais.notify.auth.auth_info import EnvVarCredentialsProvider
 from sais.notify.clients.notify_client import NotifyClient
 from sais.notify.config import const
 from sais.notify.config.const import ENDPOINT, NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU, \
-    NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP
+    NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP, LOGGER_NAME
 from sais.notify.model.message_model import NotificationRequest, MessageModel
 from sais.notify.types import NotifyType
+import logging
 
 
 class MessageHandler(object):
     def __init__(self, auth_provider: EnvVarCredentialsProvider):
         self.auth_provider = auth_provider
+        self.logger = logging.getLogger(LOGGER_NAME)
 
     def send_notification(self, notify_type: NotifyType, to: str, message: str) -> bool:
         request = NotificationRequest(notify_type=notify_type, to=to, message=message)
         request.model_dump()
         if notify_type in (NotifyType.FEISHU_USER_TEXT, NotifyType.FEISHU_USER_RICH_TEXT,
                            NotifyType.FEISHU_GROUP_TEXT, NotifyType.FEISHU_GROUP_MESSAGE_CARD):
             return self.__send_notification_feishu(notify_type, to, message)
```

### Comparing `sais_notify-0.0.2/pyproject.toml` & `sais_notify-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling>=1.8.0"]
+requires = ["hatchling>=1.8.0", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sais-notify"
-dynamic = ["version"]
+dynamic = ["version", "readme"]
 description = "sais notify python sdk"
 license = {text = "Apache License 2.0"}
 authors = [
   {name = "SAIS Contributors"},
   {email = "sais@example.com"}
 ]
 keywords = ["sais-notify", "sais"]
@@ -29,14 +29,20 @@
 test = []
 
 [project.urls]
 repository = "https://github.com/xxx/xxxx"
 
 [project.scripts]
 
+[tool.hatch.metadata.hooks.fancy-pypi-readme]
+content-type = "text/markdown"
+fragments = [
+  { path = "README.md" },
+]
+
 [tool.hatch.version]
 path = 'sais/notify/config/version.py'
 
 [tool.hatch.build.targets.sdist]
 exclude = []
 
 [tool.hatch.build.targets.wheel]
```


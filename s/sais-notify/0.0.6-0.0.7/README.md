# Comparing `tmp/sais_notify-0.0.6.tar.gz` & `tmp/sais_notify-0.0.7.tar.gz`

## Comparing `sais_notify-0.0.6.tar` & `sais_notify-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.6/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/auth/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/auth/auth_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/clients/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/clients/notify_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/config/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/config/const.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/config/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/handler/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/handler/message_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/model/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/model/message_model.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/types/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.6/.gitignore
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sais_notify-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 sais_notify-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 sais_notify-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/auth/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/auth/auth_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/clients/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/clients/notify_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/config/__init__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/config/const.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/config/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/handler/__init__.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/handler/message_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/model/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/model/message_model.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 sais_notify-0.0.7/sais/notify/types/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 sais_notify-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 sais_notify-0.0.7/PKG-INFO
```

### Comparing `sais_notify-0.0.6/sais/notify/clients/notify_client.py` & `sais_notify-0.0.7/sais/notify/clients/notify_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,30 +2,36 @@
 import logging
 from http import HTTPStatus
 
 import requests
 
 from sais.notify.auth.auth_info import EnvVarCredentialsProvider
 from sais.notify.config.const import LOGGER_NAME
-from sais.notify.model import MessageModel
+from sais.notify.model.message_model import MessageModel
+
+logger = logging.getLogger(LOGGER_NAME)
+logging.basicConfig(level=logging.INFO)
 
 
 class NotifyClient(object):
     def __init__(self, endpoint, auth_provider: EnvVarCredentialsProvider):
         self.endpoint = endpoint
         self.auth_provider = auth_provider
-        self.logger = logging.getLogger(LOGGER_NAME)
 
-    def send_notification_feishu(self, message: MessageModel) -> bool:
+    def send_notification_feishu(self, message_info: MessageModel) -> bool:
         headers = {
             'Authorization': self.auth_provider.token,
             'Content-Type': 'application/json'
         }
-
-        payload = message.model_dump_json()
-        response = requests.post(f'{self.endpoint}/api/v1/notify/send', headers=headers, data=json.dumps(payload))
+        response = requests.post(f'{self.endpoint}/api/v1/notify/send', headers=headers,
+                                 json=message_info.model_dump(by_alias=True, exclude_none=True))
 
         if response.status_code == HTTPStatus.OK:
-            self.logger.info(f'Notification sent successfully')
-            return response.json()
+            response_data = response.json()
+            if response_data.get('msgCode') == '10000':
+                logger.info(f'Notification sent successfully')
+                return True
+            else:
+                logger.error(f'Error sending notification: {response.status_code} - {response.text}')
         else:
-            raise Exception(f'Error sending notification: {response.status_code} - {response.text}')
+            logger.error(f'Error sending notification: {response.status_code}')
+        return False
```

### Comparing `sais_notify-0.0.6/sais/notify/handler/message_handler.py` & `sais_notify-0.0.7/sais/notify/handler/message_handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,39 +4,59 @@
 from sais.notify.clients.notify_client import NotifyClient
 from sais.notify.config import const
 from sais.notify.config.const import ENDPOINT, NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU, \
     NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP, LOGGER_NAME
 from sais.notify.model.message_model import NotificationRequest, MessageModel
 from sais.notify.types import NotifyType
 
+logger = logging.getLogger(LOGGER_NAME)
+logging.basicConfig(level=logging.INFO)
+
 
 class MessageHandler(object):
     def __init__(self, auth_provider: EnvVarCredentialsProvider):
         self.auth_provider = auth_provider
-        self.logger = logging.getLogger(LOGGER_NAME)
 
     def send_notification(self, notify_type: NotifyType, to: str, message: str) -> bool:
+        """
+        发送通知的函数。
+
+        参数:
+        - notify_type: 通知类型，枚举类型NotifyType指定。
+        - to: 接收通知的目标标识，可以是用户或群组的标识。
+        - message: 要发送的消息内容。
+
+        返回值:
+        - bool: 发送成功返回True，失败返回False。
+        """
+        logger.info(f'info send notification: {notify_type}, {to}, {message}')
+        logger.debug(f'debug send notification: {notify_type}, {to}, {message}')
         request = NotificationRequest(notify_type=notify_type, to=to, message=message)
         request.model_dump()
         if notify_type in (NotifyType.FEISHU_USER_TEXT, NotifyType.FEISHU_USER_RICH_TEXT,
                            NotifyType.FEISHU_GROUP_TEXT, NotifyType.FEISHU_GROUP_MESSAGE_CARD):
             return self.__send_notification_feishu(notify_type, to, message)
         else:
-            self.logger.error(f'not support notify type: {notify_type}')
+            logger.error(f'not support notify type: {notify_type}')
         return False
 
     def __send_notification_feishu(self, notify_type: NotifyType, to: str, message: str) -> bool:
         client = NotifyClient(ENDPOINT, self.auth_provider)
-        message_model = MessageModel(message=message, to=to)
-        if notify_type == NotifyType.FEISHU_USER_TEXT:
-            message_model.set_type(NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU)
-            return client.send_notification_feishu(message_model)
-        elif notify_type == NotifyType.FEISHU_USER_RICH_TEXT:
-            message_model.set_type(NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU)
-            message_model.set_robot_name(const.SAIS_ROBOT_NAME)
-            return client.send_notification_feishu(message_model)
-        elif notify_type == NotifyType.FEISHU_GROUP_TEXT:
-            message_model.set_type(NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP)
-            return client.send_notification_feishu(message_model)
-        elif notify_type == NotifyType.FEISHU_GROUP_MESSAGE_CARD:
-            message_model.set_type(NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP)
-            return client.send_notification_feishu(message_model)
+        message_model = MessageModel(
+            message=message,
+            to=to,
+            type={
+                NotifyType.FEISHU_USER_TEXT: NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU,
+                NotifyType.FEISHU_USER_RICH_TEXT: NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU,
+                NotifyType.FEISHU_GROUP_TEXT: NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP,
+                NotifyType.FEISHU_GROUP_MESSAGE_CARD: NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP,
+            }.get(notify_type, None)
+        )
+
+        robot_name = const.SAIS_ROBOT_NAME if notify_type == NotifyType.FEISHU_USER_RICH_TEXT else None
+        message_model.robot_name = robot_name
+
+        if message_model.type is None:
+            logger.error(f'not support notify type: {notify_type}')
+            return False
+
+        return client.send_notification_feishu(message_model)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sais_notify-0.0.6/pyproject.toml` & `sais_notify-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "Programming Language :: Python :: 3.8",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
+"pydantic~=2.4.2",
 "requests~=2.28.2",
 "tqdm~=4.65.0",
 "setuptools~=60.2.0",
 ]
 
 [project.optional-dependencies]
 test = []
```


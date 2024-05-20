# Comparing `tmp/sais_notify-0.0.3.tar.gz` & `tmp/sais_notify-0.0.4.tar.gz`

## Comparing `sais_notify-0.0.3.tar` & `sais_notify-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.3/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/auth/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/auth/auth_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/clients/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/clients/notify_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/config/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/config/const.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/config/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/handler/__init__.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/handler/message_handler.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/model/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/model/message_model.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.3/sais/notify/types/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.3/.gitignore
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sais_notify-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 sais_notify-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/auth/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/auth/auth_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/clients/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/clients/notify_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/config/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/config/const.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/config/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/handler/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/handler/message_handler.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/model/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/model/message_model.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/types/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sais_notify-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 sais_notify-0.0.4/PKG-INFO
```

### Comparing `sais_notify-0.0.3/README.md` & `sais_notify-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.3/sais/notify/clients/notify_client.py` & `sais_notify-0.0.4/sais/notify/clients/notify_client.py`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.3/sais/notify/handler/message_handler.py` & `sais_notify-0.0.4/sais/notify/handler/message_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from fastapi.logger import logger
-
 from sais.notify.auth.auth_info import EnvVarCredentialsProvider
 from sais.notify.clients.notify_client import NotifyClient
 from sais.notify.config import const
 from sais.notify.config.const import ENDPOINT, NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU, \
     NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP, LOGGER_NAME
 from sais.notify.model.message_model import NotificationRequest, MessageModel
 from sais.notify.types import NotifyType
@@ -18,15 +16,15 @@
     def send_notification(self, notify_type: NotifyType, to: str, message: str) -> bool:
         request = NotificationRequest(notify_type=notify_type, to=to, message=message)
         request.model_dump()
         if notify_type in (NotifyType.FEISHU_USER_TEXT, NotifyType.FEISHU_USER_RICH_TEXT,
                            NotifyType.FEISHU_GROUP_TEXT, NotifyType.FEISHU_GROUP_MESSAGE_CARD):
             return self.__send_notification_feishu(notify_type, to, message)
         else:
-            logger.error(f'not support notify type: {notify_type}')
+            self.logger.error(f'not support notify type: {notify_type}')
         return False
 
     def __send_notification_feishu(self, notify_type: NotifyType, to: str, message: str) -> bool:
         client = NotifyClient(ENDPOINT, self.auth_provider)
         message_model = MessageModel(message=message, to=to)
         if notify_type == NotifyType.FEISHU_USER_TEXT:
             message_model.set_type(NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU)
```

### Comparing `sais_notify-0.0.3/pyproject.toml` & `sais_notify-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.3/PKG-INFO` & `sais_notify-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sais-notify
-Version: 0.0.3
+Version: 0.0.4
 Summary: sais notify python sdk
 Project-URL: repository, https://github.com/xxx/xxxx
 Author: SAIS Contributors
 Author-email: sais@example.com
 License: Apache License 2.0
 Keywords: sais,sais-notify
 Classifier: Programming Language :: Python :: 3.8
```


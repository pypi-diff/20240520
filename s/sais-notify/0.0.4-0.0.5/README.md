# Comparing `tmp/sais_notify-0.0.4.tar.gz` & `tmp/sais_notify-0.0.5.tar.gz`

## Comparing `sais_notify-0.0.4.tar` & `sais_notify-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.4/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/auth/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/auth/auth_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/clients/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/clients/notify_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/config/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/config/const.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/config/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/handler/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/handler/message_handler.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/model/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/model/message_model.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.4/sais/notify/types/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.4/.gitignore
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sais_notify-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 sais_notify-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/auth/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/auth/auth_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/clients/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/clients/notify_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/config/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/config/const.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/config/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/handler/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/handler/message_handler.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/model/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/model/message_model.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/types/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sais_notify-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 sais_notify-0.0.5/PKG-INFO
```

### Comparing `sais_notify-0.0.4/README.md` & `sais_notify-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.4/sais/notify/clients/notify_client.py` & `sais_notify-0.0.5/sais/notify/clients/notify_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
+import logging
 from http import HTTPStatus
 
 import requests
-import logging
+
 from sais.notify.auth.auth_info import EnvVarCredentialsProvider
 from sais.notify.config.const import LOGGER_NAME
 from sais.notify.model import MessageModel
 
 
 class NotifyClient(object):
     def __init__(self, endpoint, auth_provider: EnvVarCredentialsProvider):
```

### Comparing `sais_notify-0.0.4/sais/notify/handler/message_handler.py` & `sais_notify-0.0.5/sais/notify/handler/message_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import logging
+
 from sais.notify.auth.auth_info import EnvVarCredentialsProvider
 from sais.notify.clients.notify_client import NotifyClient
 from sais.notify.config import const
 from sais.notify.config.const import ENDPOINT, NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU, \
     NOTIFY_SERVICE_NOTIFY_TYPE_FEISHU_GROUP, LOGGER_NAME
 from sais.notify.model.message_model import NotificationRequest, MessageModel
 from sais.notify.types import NotifyType
-import logging
 
 
 class MessageHandler(object):
     def __init__(self, auth_provider: EnvVarCredentialsProvider):
         self.auth_provider = auth_provider
         self.logger = logging.getLogger(LOGGER_NAME)
```

### Comparing `sais_notify-0.0.4/pyproject.toml` & `sais_notify-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.4/PKG-INFO` & `sais_notify-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sais-notify
-Version: 0.0.4
+Version: 0.0.5
 Summary: sais notify python sdk
 Project-URL: repository, https://github.com/xxx/xxxx
 Author: SAIS Contributors
 Author-email: sais@example.com
 License: Apache License 2.0
 Keywords: sais,sais-notify
 Classifier: Programming Language :: Python :: 3.8
```


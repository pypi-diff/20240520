# Comparing `tmp/sais_notify-0.0.1.tar.gz` & `tmp/sais_notify-0.0.2.tar.gz`

## Comparing `sais_notify-0.0.1.tar` & `sais_notify-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.1/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/requirements.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/auth/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/auth/auth_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/clients/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/clients/notify_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/config/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/config/const.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/config/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/handler/__init__.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/handler/message_handler.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/model/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/model/message_model.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.1/sais/notify/types/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.1/.gitignore
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 sais_notify-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 sais_notify-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/auth/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/auth/auth_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/clients/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/clients/notify_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/config/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/config/const.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/config/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/handler/__init__.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/handler/message_handler.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/model/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/model/message_model.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.2/sais/notify/types/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 sais_notify-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 sais_notify-0.0.2/PKG-INFO
```

### Comparing `sais_notify-0.0.1/README.md` & `sais_notify-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.1/sais/notify/clients/notify_client.py` & `sais_notify-0.0.2/sais/notify/clients/notify_client.py`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.1/sais/notify/handler/message_handler.py` & `sais_notify-0.0.2/sais/notify/handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.1/pyproject.toml` & `sais_notify-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.1/PKG-INFO` & `sais_notify-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sais-notify
-Version: 0.0.1
+Version: 0.0.2
 Summary: sais notify python sdk
 Project-URL: repository, https://github.com/xxx/xxxx
 Author: SAIS Contributors
 Author-email: sais@example.com
 License: Apache License 2.0
 Keywords: sais,sais-notify
 Classifier: Programming Language :: Python :: 3.8
```


# Comparing `tmp/sais_notify-0.0.5.tar.gz` & `tmp/sais_notify-0.0.6.tar.gz`

## Comparing `sais_notify-0.0.5.tar` & `sais_notify-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.5/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/auth/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/auth/auth_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/clients/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/clients/notify_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/config/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/config/const.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/config/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/handler/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/handler/message_handler.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/model/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/model/message_model.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.5/sais/notify/types/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.5/.gitignore
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sais_notify-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 sais_notify-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/auth/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/auth/auth_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/clients/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/clients/notify_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/config/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/config/const.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/config/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/handler/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/handler/message_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/model/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/model/message_model.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify-0.0.6/sais/notify/types/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 sais_notify-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 sais_notify-0.0.6/PKG-INFO
```

### Comparing `sais_notify-0.0.5/README.md` & `sais_notify-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.5/sais/notify/clients/notify_client.py` & `sais_notify-0.0.6/sais/notify/clients/notify_client.py`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.5/sais/notify/handler/message_handler.py` & `sais_notify-0.0.6/sais/notify/handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.5/pyproject.toml` & `sais_notify-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sais_notify-0.0.5/PKG-INFO` & `sais_notify-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sais-notify
-Version: 0.0.5
+Version: 0.0.6
 Summary: sais notify python sdk
 Project-URL: repository, https://github.com/xxx/xxxx
 Author: SAIS Contributors
 Author-email: sais@example.com
 License: Apache License 2.0
 Keywords: sais,sais-notify
 Classifier: Programming Language :: Python :: 3.8
```


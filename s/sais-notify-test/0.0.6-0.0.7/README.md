# Comparing `tmp/sais_notify_test-0.0.6.tar.gz` & `tmp/sais_notify_test-0.0.7.tar.gz`

## Comparing `sais_notify_test-0.0.6.tar` & `sais_notify_test-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/auth/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/auth/auth_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/clients/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/clients/notify_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/config/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/config/const.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/config/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/handler/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/handler/message_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/model/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/model/message_model.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/sais/notify/types/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/.gitignore
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 sais_notify_test-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/auth/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/auth/auth_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/clients/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/clients/notify_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/config/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/config/const.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/config/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/handler/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/handler/message_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/model/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/model/message_model.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/sais/notify/types/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 sais_notify_test-0.0.7/PKG-INFO
```

### Comparing `sais_notify_test-0.0.6/README.md` & `sais_notify_test-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sais_notify_test-0.0.6/sais/notify/clients/notify_client.py` & `sais_notify_test-0.0.7/sais/notify/clients/notify_client.py`

 * *Files identical despite different names*

### Comparing `sais_notify_test-0.0.6/sais/notify/handler/message_handler.py` & `sais_notify_test-0.0.7/sais/notify/handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `sais_notify_test-0.0.6/pyproject.toml` & `sais_notify_test-0.0.7/pyproject.toml`

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

### Comparing `sais_notify_test-0.0.6/PKG-INFO` & `sais_notify_test-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: sais-notify-test
-Version: 0.0.6
+Version: 0.0.7
 Summary: sais notify python sdk
 Project-URL: repository, https://github.com/xxx/xxxx
 Author: SAIS Contributors
 Author-email: sais@example.com
 License: Apache License 2.0
 Keywords: sais,sais-notify-test
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
+Requires-Dist: pydantic~=2.4.2
 Requires-Dist: requests~=2.28.2
 Requires-Dist: setuptools~=60.2.0
 Requires-Dist: tqdm~=4.65.0
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # sais-notify
```


# Comparing `tmp/infolab_common_lib-1.0.0.tar.gz` & `tmp/infolab_common_lib-1.0.1.tar.gz`

## Comparing `infolab_common_lib-1.0.0.tar` & `infolab_common_lib-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.0/common_lib/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.0/common_lib/http_utils.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.0/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.1/common_lib/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.1/common_lib/http_utils.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.1/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 infolab_common_lib-1.0.1/PKG-INFO
```

### Comparing `infolab_common_lib-1.0.0/common_lib/http_utils.py` & `infolab_common_lib-1.0.1/common_lib/http_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class HttpClientUtils:
 
     def __init__(self, proxy_enabled=False, proxies=None, timeout=0.5):
         if proxies is None:
             proxies = []
 
         if proxy_enabled and not proxies:
-            raise ValueError("Proxies is empty")
+            raise ValueError("Empty proxies")
 
         self.proxy_enabled = proxy_enabled
         self.proxies = proxies
         self.thread_local = threading.local()
         self.timeout = timeout
 
     def get_client(self):
```

### Comparing `infolab_common_lib-1.0.0/.gitignore` & `infolab_common_lib-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `infolab_common_lib-1.0.0/LICENSE` & `infolab_common_lib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infolab_common_lib-1.0.0/pyproject.toml` & `infolab_common_lib-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "infolab-common-lib"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "anhnd15", email = "anhnd15@vng.com.vn" },
 ]
 description = "Infolab Common Lib"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `infolab_common_lib-1.0.0/PKG-INFO` & `infolab_common_lib-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infolab-common-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Infolab Common Lib
 Project-URL: Homepage, https://zalogit2.zing.vn/infolab/infolab-common-lib
 Project-URL: Bug Tracker, https://zalogit2.zing.vn/infolab/infolab-common-lib/-/issues
 Author-email: anhnd15 <anhnd15@vng.com.vn>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


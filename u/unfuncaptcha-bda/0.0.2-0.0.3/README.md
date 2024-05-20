# Comparing `tmp/unfuncaptcha_bda-0.0.2.tar.gz` & `tmp/unfuncaptcha_bda-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfuncaptcha_bda-0.0.2.tar", last modified: Wed Mar 13 07:25:55 2024, max compression
+gzip compressed data, was "unfuncaptcha_bda-0.0.3.tar", last modified: Mon May 20 06:28:28 2024, max compression
```

## Comparing `unfuncaptcha_bda-0.0.2.tar` & `unfuncaptcha_bda-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-03-13 07:25:55.077416 unfuncaptcha_bda-0.0.2/
--rw-r--r--   0 camel      (501) staff       (20)    34888 2024-03-13 04:19:50.000000 unfuncaptcha_bda-0.0.2/LICENSE
--rw-r--r--   0 camel      (501) staff       (20)     1357 2024-03-13 07:25:55.077190 unfuncaptcha_bda-0.0.2/PKG-INFO
--rw-r--r--   0 camel      (501) staff       (20)      835 2024-03-13 04:19:50.000000 unfuncaptcha_bda-0.0.2/README.md
--rw-r--r--   0 camel      (501) staff       (20)      591 2024-03-13 07:25:44.000000 unfuncaptcha_bda-0.0.2/pyproject.toml
--rw-r--r--   0 camel      (501) staff       (20)       38 2024-03-13 07:25:55.077458 unfuncaptcha_bda-0.0.2/setup.cfg
-drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-03-13 07:25:55.075415 unfuncaptcha_bda-0.0.2/src/
-drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-03-13 07:25:55.076305 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda/
--rw-r--r--   0 camel      (501) staff       (20)       49 2024-03-13 04:19:50.000000 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda/__init__.py
--rw-r--r--   0 camel      (501) staff       (20)     1580 2024-03-13 04:19:50.000000 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda/crypto.py
--rw-r--r--   0 camel      (501) staff       (20)     2794 2024-03-13 07:15:34.000000 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda/fingerprint.py
-drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-03-13 07:25:55.076994 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda.egg-info/
--rw-r--r--   0 camel      (501) staff       (20)     1357 2024-03-13 07:25:55.000000 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda.egg-info/PKG-INFO
--rw-r--r--   0 camel      (501) staff       (20)      308 2024-03-13 07:25:55.000000 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda.egg-info/SOURCES.txt
--rw-r--r--   0 camel      (501) staff       (20)        1 2024-03-13 07:25:55.000000 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda.egg-info/dependency_links.txt
--rw-r--r--   0 camel      (501) staff       (20)       17 2024-03-13 07:25:55.000000 unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda.egg-info/top_level.txt
+drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-20 06:28:28.325940 unfuncaptcha_bda-0.0.3/
+-rw-r--r--   0 camel      (501) staff       (20)    34888 2024-05-17 19:39:57.000000 unfuncaptcha_bda-0.0.3/LICENSE
+-rw-r--r--   0 camel      (501) staff       (20)     1357 2024-05-20 06:28:28.325733 unfuncaptcha_bda-0.0.3/PKG-INFO
+-rw-r--r--   0 camel      (501) staff       (20)      835 2024-05-17 19:39:57.000000 unfuncaptcha_bda-0.0.3/README.md
+-rw-r--r--   0 camel      (501) staff       (20)      591 2024-05-20 06:27:57.000000 unfuncaptcha_bda-0.0.3/pyproject.toml
+-rw-r--r--   0 camel      (501) staff       (20)       38 2024-05-20 06:28:28.326021 unfuncaptcha_bda-0.0.3/setup.cfg
+drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-20 06:28:28.324018 unfuncaptcha_bda-0.0.3/src/
+drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-20 06:28:28.324802 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/
+-rw-r--r--   0 camel      (501) staff       (20)       49 2024-05-17 19:39:57.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/__init__.py
+-rw-r--r--   0 camel      (501) staff       (20)     1580 2024-05-18 07:16:49.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/crypto.py
+-rw-r--r--   0 camel      (501) staff       (20)     3040 2024-05-17 21:11:50.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/fingerprint.py
+drwxr-xr-x   0 camel      (501) staff       (20)        0 2024-05-20 06:28:28.325528 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/
+-rw-r--r--   0 camel      (501) staff       (20)     1357 2024-05-20 06:28:28.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/PKG-INFO
+-rw-r--r--   0 camel      (501) staff       (20)      308 2024-05-20 06:28:28.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/SOURCES.txt
+-rw-r--r--   0 camel      (501) staff       (20)        1 2024-05-20 06:28:28.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/dependency_links.txt
+-rw-r--r--   0 camel      (501) staff       (20)       17 2024-05-20 06:28:28.000000 unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/top_level.txt
```

### Comparing `unfuncaptcha_bda-0.0.2/LICENSE` & `unfuncaptcha_bda-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unfuncaptcha_bda-0.0.2/PKG-INFO` & `unfuncaptcha_bda-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfuncaptcha_bda
-Version: 0.0.2
+Version: 0.0.3
 Summary: View, edit, and repackage Arkose Labs Funcaptcha fingerprints
 Author-email: bc <no@dont.email.me>
 Project-URL: Homepage, https://github.com/unfuncaptcha/bda
 Project-URL: Issues, https://github.com/unfuncaptcha/bda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unfuncaptcha_bda-0.0.2/README.md` & `unfuncaptcha_bda-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `unfuncaptcha_bda-0.0.2/pyproject.toml` & `unfuncaptcha_bda-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unfuncaptcha_bda"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "bc", email = "no@dont.email.me" }]
 description = "View, edit, and repackage Arkose Labs Funcaptcha fingerprints"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda/crypto.py` & `unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/crypto.py`

 * *Files identical despite different names*

### Comparing `unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda/fingerprint.py` & `unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda/fingerprint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import Any, Callable, List, Optional
 from .crypto import BDACrypto
 import base64
 import json
 import time
 
 class ArkoseBrowserFingerprint(object):
-    def __init__(self, encoded_fingerprint: str, user_agent: str, timestamp: int = None):
-        now = time.time()
-        self._timestamp = str(int(now - (now % 21600))) if not timestamp else timestamp
+    def __init__(self, encoded_fingerprint: str, user_agent: str, timestamp: int = int(time.time())):
+        self._timestamp = str(int(timestamp - (timestamp % 21600)))
         self._key = user_agent + str(self._timestamp)
 
         self.crypto = BDACrypto(self._key)
         self._raw_fingeprint = json.loads(base64.b64decode(encoded_fingerprint)) # {"ct": ..., "s": ..., "iv": ... }
         self.fingerprint: list[dict[str, Any]] = json.loads(self.crypto.decrypt(self._raw_fingeprint).decode())
 
 
@@ -21,45 +20,60 @@
             separators=(',', ':'),
             sort_keys=True
         )
 
         return repacked_bda if not encode_base64 else base64.b64encode(repacked_bda.encode()).decode()
 
 
-    def core_key_operation(self, 
-        key: str, 
+    def _core_key_operation(self, 
+        key: str,
         operation: Callable, 
-        value: Any, 
+        value: Any = None,
         container: Optional[List[dict[str, Any]]] = None, 
         key_required_for_operation: Optional[bool] = True
     ) -> Any:
-        container = self.fingerprint if container is None else container
+        container = container or self.fingerprint
         items = list(filter(lambda item: item['key'] == key, container))
         
         if not items and key_required_for_operation:
             raise KeyError(f"Key '{key}' not found in the container.")
 
         return operation(items[0] if key_required_for_operation else None, value, container)
 
 
     def fetch_key(self, key: str, container: Optional[List[dict[str, Any]]] = None) -> Any:
-        return self.core_key_operation(key, lambda item, _, __: item['value'], None, container)
+        return self._core_key_operation(
+            key,
+            operation = lambda item, _, __: item['value'], 
+            container = container
+        )
 
 
     def insert_key(self, key: str, value: Any, container: Optional[List[dict[str, Any]]] = None) -> Any:
-        return self.core_key_operation(key, lambda _, value, container: container.append({'key': key, 'value': value}) or value, value, container, False)
+        return self._core_key_operation(
+            key, 
+            operation = lambda _, value, container: container.append({'key': key, 'value': value}) or value, 
+            value = value, 
+            container = container, 
+            key_required_for_operation = False
+        )
 
 
     def edit_key(self, key: str, value: Any, container: Optional[List[dict[str, Any]]] = None) -> Any:
-        return self.core_key_operation(key, lambda item, value, _: item.__setitem__('value', value) or value, value, container)
+        return self._core_key_operation(
+            key, 
+            operation = lambda item, value, _: item.__setitem__('value', value) or value, 
+            value = value, 
+            container = container
+        )
 
 
     def fetch_enhanced_fp_key(self, enhanced_fp_key: str) -> Any:
         return self.fetch_key(enhanced_fp_key, self.fetch_key("enhanced_fp"))
 
 
     def insert_enhanced_fp_key(self, key: str, value: Any) -> Any:
         return self.insert_key(key, value, self.fetch_key("enhanced_fp"))
 
 
     def edit_enhanced_fp_key(self, key: str, value: Any) -> Any:
-        return self.edit_key(key, value, self.fetch_key("enhanced_fp"))
+        return self.edit_key(key, value, self.fetch_key("enhanced_fp"))
```

### Comparing `unfuncaptcha_bda-0.0.2/src/unfuncaptcha_bda.egg-info/PKG-INFO` & `unfuncaptcha_bda-0.0.3/src/unfuncaptcha_bda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfuncaptcha_bda
-Version: 0.0.2
+Version: 0.0.3
 Summary: View, edit, and repackage Arkose Labs Funcaptcha fingerprints
 Author-email: bc <no@dont.email.me>
 Project-URL: Homepage, https://github.com/unfuncaptcha/bda
 Project-URL: Issues, https://github.com/unfuncaptcha/bda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


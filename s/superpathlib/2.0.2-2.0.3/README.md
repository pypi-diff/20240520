# Comparing `tmp/superpathlib-2.0.2.tar.gz` & `tmp/superpathlib-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpathlib-2.0.2.tar", last modified: Tue Mar  5 07:54:17 2024, max compression
+gzip compressed data, was "superpathlib-2.0.3.tar", last modified: Mon May 20 00:15:05 2024, max compression
```

## Comparing `superpathlib-2.0.2.tar` & `superpathlib-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 07:54:17.320029 superpathlib-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-05 07:54:07.000000 superpathlib-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-05 07:54:17.320029 superpathlib-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-03-05 07:54:07.000000 superpathlib-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-05 07:54:07.000000 superpathlib-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 07:54:17.320029 superpathlib-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 07:54:17.316029 superpathlib-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 07:54:17.316029 superpathlib-2.0.2/src/superpathlib/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/cached_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/common_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/content_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/extra_functionality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/metadata_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/override.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/path.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-05 07:54:07.000000 superpathlib-2.0.2/src/superpathlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 07:54:17.320029 superpathlib-2.0.2/src/superpathlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-05 07:54:17.000000 superpathlib-2.0.2/src/superpathlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-05 07:54:17.000000 superpathlib-2.0.2/src/superpathlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 07:54:17.000000 superpathlib-2.0.2/src/superpathlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-05 07:54:17.000000 superpathlib-2.0.2/src/superpathlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-05 07:54:17.000000 superpathlib-2.0.2/src/superpathlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 07:54:17.320029 superpathlib-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-05 07:54:07.000000 superpathlib-2.0.2/tests/test_cached_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-05 07:54:07.000000 superpathlib-2.0.2/tests/test_common_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-05 07:54:07.000000 superpathlib-2.0.2/tests/test_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-05 07:54:07.000000 superpathlib-2.0.2/tests/test_encrypted_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-03-05 07:54:07.000000 superpathlib-2.0.2/tests/test_functionality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-05 07:54:07.000000 superpathlib-2.0.2/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:15:05.555190 superpathlib-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-20 00:14:43.000000 superpathlib-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-20 00:15:05.555190 superpathlib-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-20 00:14:43.000000 superpathlib-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-20 00:14:43.000000 superpathlib-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:15:05.555190 superpathlib-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:15:05.547190 superpathlib-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:15:05.551190 superpathlib-2.0.3/src/superpathlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/cached_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/common_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/content_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/extra_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/metadata_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/override.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 00:14:43.000000 superpathlib-2.0.3/src/superpathlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:15:05.551190 superpathlib-2.0.3/src/superpathlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-20 00:15:05.000000 superpathlib-2.0.3/src/superpathlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-20 00:15:05.000000 superpathlib-2.0.3/src/superpathlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:15:05.000000 superpathlib-2.0.3/src/superpathlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-20 00:15:05.000000 superpathlib-2.0.3/src/superpathlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 00:15:05.000000 superpathlib-2.0.3/src/superpathlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:15:05.551190 superpathlib-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-20 00:14:43.000000 superpathlib-2.0.3/tests/test_cached_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-20 00:14:43.000000 superpathlib-2.0.3/tests/test_common_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-20 00:14:43.000000 superpathlib-2.0.3/tests/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-20 00:14:43.000000 superpathlib-2.0.3/tests/test_encrypted_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-20 00:14:43.000000 superpathlib-2.0.3/tests/test_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-20 00:14:43.000000 superpathlib-2.0.3/tests/test_metadata.py
```

### Comparing `superpathlib-2.0.2/LICENSE` & `superpathlib-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/PKG-INFO` & `superpathlib-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 2.0.2
+Version: 2.0.3
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `superpathlib-2.0.2/README.md` & `superpathlib-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/pyproject.toml` & `superpathlib-2.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "superpathlib"
-version = "2.0.2"
+version = "2.0.3"
 description = "Extended Pathlib"
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "simple-classproperty >=4.0.2, <5",
```

### Comparing `superpathlib-2.0.2/src/superpathlib/base.py` & `superpathlib-2.0.3/src/superpathlib/base.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib/cached_content.py` & `superpathlib-2.0.3/src/superpathlib/cached_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib/common_folders.py` & `superpathlib-2.0.3/src/superpathlib/common_folders.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib/content_properties.py` & `superpathlib-2.0.3/src/superpathlib/content_properties.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib/encryption.py` & `superpathlib-2.0.3/src/superpathlib/encryption.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib/extra_functionality.py` & `superpathlib-2.0.3/src/superpathlib/extra_functionality.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib/metadata_properties.py` & `superpathlib-2.0.3/src/superpathlib/metadata_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,17 @@
     def mtime(self) -> float:
         return self.stat().st_mtime
 
     @mtime.setter
     def mtime(self, time: float) -> None:
         os.utime(self, (time, time))  # set create time as well
 
+        command = "touch", "-d", f"@{time}", self
         try:
-            subprocess.run(("touch", "-d", "@%f" % time, self))
+            subprocess.run(command)
         except subprocess.CalledProcessError:  # pragma: nocover
             pass  # Doesn't work on Windows
 
     @property
     def tags(self) -> list[str]:
         from .tags import XDGTags  # noqa: E402, autoimport
 
@@ -98,27 +99,27 @@
     def filetype(self) -> str | None:
         filetype = mimetypes.guess_type(self)[0]
         if filetype:
             filetype = filetype.split("/")[0]
         return filetype
 
     @property
-    def content_hash(self) -> str:
+    def content_hash(self) -> str | None:
         return self.file_content_hash if self.is_file() else self.dir_content_hash
 
     @property
-    def dir_content_hash(self) -> str:
+    def dir_content_hash(self) -> str | None:
         # dirhash package throws annoying warnings
         warnings.filterwarnings(
             action="ignore", module="pkg_resources|dirhash", category=DeprecationWarning
         )
 
         import dirhash  # noqa: E402, F401, autoimport
 
         # use default algorithm used in cloud provider checksums
         # can be efficient because not used for cryptographic security
-        content_hash = dirhash.dirhash(self, "md5")
+        content_hash = dirhash.dirhash(self, "md5") if self.exists() else None
         return typing.cast(str, content_hash)
 
     @property
     def file_content_hash(self) -> str:
         return hashlib.new("sha512", data=self.byte_content).hexdigest()
```

### Comparing `superpathlib-2.0.2/src/superpathlib/override.py` & `superpathlib-2.0.3/src/superpathlib/override.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib/tags.py` & `superpathlib-2.0.3/src/superpathlib/tags.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib/utils.py` & `superpathlib-2.0.3/src/superpathlib/utils.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/src/superpathlib.egg-info/PKG-INFO` & `superpathlib-2.0.3/src/superpathlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 2.0.2
+Version: 2.0.3
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `superpathlib-2.0.2/src/superpathlib.egg-info/SOURCES.txt` & `superpathlib-2.0.3/src/superpathlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/tests/test_cached_content.py` & `superpathlib-2.0.3/tests/test_cached_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/tests/test_common_folders.py` & `superpathlib-2.0.3/tests/test_common_folders.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/tests/test_content.py` & `superpathlib-2.0.3/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/tests/test_encrypted_content.py` & `superpathlib-2.0.3/tests/test_encrypted_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/tests/test_functionality.py` & `superpathlib-2.0.3/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `superpathlib-2.0.2/tests/test_metadata.py` & `superpathlib-2.0.3/tests/test_metadata.py`

 * *Files identical despite different names*


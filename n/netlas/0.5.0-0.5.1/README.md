# Comparing `tmp/netlas-0.5.0.tar.gz` & `tmp/netlas-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlas-0.5.0.tar", last modified: Fri May 17 12:09:19 2024, max compression
+gzip compressed data, was "netlas-0.5.1.tar", last modified: Mon May 20 12:26:39 2024, max compression
```

## Comparing `netlas-0.5.0.tar` & `netlas-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-17 12:09:19.871703 netlas-0.5.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1242 2022-12-07 13:16:10.000000 netlas-0.5.0/CHANGELOG.md
--rw-rw-r--   0 user      (1000) user      (1000)    15072 2024-05-17 12:04:14.000000 netlas-0.5.0/LICENSE.md
--rw-r--r--   0 user      (1000) user      (1000)      102 2022-11-25 12:28:45.000000 netlas-0.5.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     3882 2024-05-17 12:09:19.871703 netlas-0.5.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3231 2024-05-17 12:04:14.000000 netlas-0.5.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-17 12:09:19.867703 netlas-0.5.0/docs/
--rw-r--r--   0 user      (1000) user      (1000)      634 2022-11-25 12:28:47.000000 netlas-0.5.0/docs/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     2461 2022-12-07 13:03:53.000000 netlas-0.5.0/docs/conf.py
--rw-rw-r--   0 user      (1000) user      (1000)     3218 2023-06-05 08:54:45.000000 netlas-0.5.0/docs/getting_started.rst
--rw-r--r--   0 user      (1000) user      (1000)      244 2022-11-25 12:28:47.000000 netlas-0.5.0/docs/index.rst
--rw-r--r--   0 user      (1000) user      (1000)      795 2022-11-25 12:28:47.000000 netlas-0.5.0/docs/make.bat
--rw-r--r--   0 user      (1000) user      (1000)      264 2022-11-25 12:28:47.000000 netlas-0.5.0/docs/netlas.rst
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-17 12:09:19.867703 netlas-0.5.0/netlas/
--rw-r--r--   0 user      (1000) user      (1000)       71 2022-11-25 12:28:47.000000 netlas-0.5.0/netlas/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14256 2024-05-17 09:44:08.000000 netlas-0.5.0/netlas/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    11117 2024-05-17 11:50:35.000000 netlas-0.5.0/netlas/client.py
--rw-r--r--   0 user      (1000) user      (1000)      177 2022-11-25 12:28:47.000000 netlas-0.5.0/netlas/exception.py
--rw-rw-r--   0 user      (1000) user      (1000)     5781 2024-05-17 09:44:08.000000 netlas-0.5.0/netlas/helpers.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-17 12:09:19.871703 netlas-0.5.0/netlas.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3882 2024-05-17 12:09:19.000000 netlas-0.5.0/netlas.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      443 2024-05-17 12:09:19.000000 netlas-0.5.0/netlas.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-17 12:09:19.000000 netlas-0.5.0/netlas.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       48 2024-05-17 12:09:19.000000 netlas-0.5.0/netlas.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       97 2024-05-17 12:09:19.000000 netlas-0.5.0/netlas.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2024-05-17 12:09:19.000000 netlas-0.5.0/netlas.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       96 2024-05-17 09:44:08.000000 netlas-0.5.0/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-17 12:09:19.871703 netlas-0.5.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      871 2024-05-17 12:03:08.000000 netlas-0.5.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 12:26:39.597779 netlas-0.5.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     1242 2022-12-07 13:16:10.000000 netlas-0.5.1/CHANGELOG.md
+-rw-rw-r--   0 user      (1000) user      (1000)    15072 2024-05-17 12:04:14.000000 netlas-0.5.1/LICENSE.md
+-rw-r--r--   0 user      (1000) user      (1000)      102 2022-11-25 12:28:45.000000 netlas-0.5.1/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3882 2024-05-20 12:26:39.593779 netlas-0.5.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3231 2024-05-17 12:04:14.000000 netlas-0.5.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 12:26:39.593779 netlas-0.5.1/docs/
+-rw-r--r--   0 user      (1000) user      (1000)      634 2022-11-25 12:28:47.000000 netlas-0.5.1/docs/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     2461 2022-12-07 13:03:53.000000 netlas-0.5.1/docs/conf.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3218 2023-06-05 08:54:45.000000 netlas-0.5.1/docs/getting_started.rst
+-rw-r--r--   0 user      (1000) user      (1000)      244 2022-11-25 12:28:47.000000 netlas-0.5.1/docs/index.rst
+-rw-r--r--   0 user      (1000) user      (1000)      795 2022-11-25 12:28:47.000000 netlas-0.5.1/docs/make.bat
+-rw-r--r--   0 user      (1000) user      (1000)      264 2022-11-25 12:28:47.000000 netlas-0.5.1/docs/netlas.rst
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 12:26:39.593779 netlas-0.5.1/netlas/
+-rw-r--r--   0 user      (1000) user      (1000)       71 2022-11-25 12:28:47.000000 netlas-0.5.1/netlas/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14256 2024-05-17 09:44:08.000000 netlas-0.5.1/netlas/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11269 2024-05-20 11:58:29.000000 netlas-0.5.1/netlas/client.py
+-rw-r--r--   0 user      (1000) user      (1000)      177 2022-11-25 12:28:47.000000 netlas-0.5.1/netlas/exception.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5781 2024-05-17 09:44:08.000000 netlas-0.5.1/netlas/helpers.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-20 12:26:39.593779 netlas-0.5.1/netlas.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3882 2024-05-20 12:26:39.000000 netlas-0.5.1/netlas.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      443 2024-05-20 12:26:39.000000 netlas-0.5.1/netlas.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-20 12:26:39.000000 netlas-0.5.1/netlas.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       48 2024-05-20 12:26:39.000000 netlas-0.5.1/netlas.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       97 2024-05-20 12:26:39.000000 netlas-0.5.1/netlas.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2024-05-20 12:26:39.000000 netlas-0.5.1/netlas.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       96 2024-05-17 09:44:08.000000 netlas-0.5.1/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-20 12:26:39.597779 netlas-0.5.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      871 2024-05-20 12:23:00.000000 netlas-0.5.1/setup.py
```

### Comparing `netlas-0.5.0/CHANGELOG.md` & `netlas-0.5.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/LICENSE.md` & `netlas-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/PKG-INFO` & `netlas-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlas
-Version: 0.5.0
+Version: 0.5.1
 Summary: Netlas.io API package
 Home-page: https://github.com/netlas-io/netlas-python
 Author: Netlas Team
 Author-email: support@netlas.io
 Keywords: security,network
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netlas-0.5.0/README.md` & `netlas-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/docs/Makefile` & `netlas-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/docs/conf.py` & `netlas-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/docs/getting_started.rst` & `netlas-0.5.1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/docs/make.bat` & `netlas-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/netlas/__main__.py` & `netlas-0.5.1/netlas/__main__.py`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/netlas/client.py` & `netlas-0.5.1/netlas/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,22 +80,26 @@
         try:
             with requests.post(
                 f"{self.apibase}{endpoint}",
                 json=params,
                 headers=self.headers,
                 verify=self.verify_ssl,
                 stream=True,
+                timeout=60.0
             ) as r:
                 check_status_code(request=r, debug=self.debug, ret=ret)
                 for chunk in r.iter_lines():
                     # skip keep-alive chunks
                     if chunk:
                         yield chunk
-        except:
-            ret["error"] = f"Unexpected Stream error"
+        except requests.exceptions.RequestException as ex:
+            try:
+                ret["error"] = str(ex)
+            except:
+                ret["error"] = f"Unexpected Stream error"
             raise APIError(ret["error"])
 
     def search(
         self, query: str, datatype: str = "response", page: int = 0, indices: str = "", fields: str = None, exclude_fields: bool = False
     ) -> dict:
         """Send search query to Netlas API
```

### Comparing `netlas-0.5.0/netlas/helpers.py` & `netlas-0.5.1/netlas/helpers.py`

 * *Files identical despite different names*

### Comparing `netlas-0.5.0/netlas.egg-info/PKG-INFO` & `netlas-0.5.1/netlas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlas
-Version: 0.5.0
+Version: 0.5.1
 Summary: Netlas.io API package
 Home-page: https://github.com/netlas-io/netlas-python
 Author: Netlas Team
 Author-email: support@netlas.io
 Keywords: security,network
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netlas-0.5.0/setup.py` & `netlas-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 DEPENDENCIES = open("requirements.txt", "r").read().split("\n")
 
 setup(
     name="netlas",
-    version="0.5.0",
+    version="0.5.1",
     author="Netlas Team",
     author_email="support@netlas.io",
     description="Netlas.io API package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/netlas-io/netlas-python",
     packages=["netlas"],
```


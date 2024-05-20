# Comparing `tmp/pypomes_http-0.1.6.tar.gz` & `tmp/pypomes_http-0.1.7.tar.gz`

## Comparing `pypomes_http-0.1.6.tar` & `pypomes_http-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/src/pypomes_http/__init__.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/src/pypomes_http/http_async.py
--rw-r--r--   0        0        0    15862 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/src/pypomes_http/http_pomes.py
--rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/src/pypomes_http/http_statuses.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/src/pypomes_http/__init__.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/src/pypomes_http/http_async.py
+-rw-r--r--   0        0        0    15862 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/src/pypomes_http/http_pomes.py
+-rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/src/pypomes_http/http_statuses.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/PKG-INFO
```

### Comparing `pypomes_http-0.1.6/src/pypomes_http/__init__.py` & `pypomes_http-0.1.7/src/pypomes_http/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.6/src/pypomes_http/http_async.py` & `pypomes_http-0.1.7/src/pypomes_http/http_async.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.6/src/pypomes_http/http_pomes.py` & `pypomes_http-0.1.7/src/pypomes_http/http_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.6/src/pypomes_http/http_statuses.py` & `pypomes_http-0.1.7/src/pypomes_http/http_statuses.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.6/LICENSE` & `pypomes_http-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.6/pyproject.toml` & `pypomes_http-0.1.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_http"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (HTTP modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=0.9.0",
+    "pypomes_core>=1.0.5",
     "pypomes_security>=0.1.3",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
```

### Comparing `pypomes_http-0.1.6/PKG-INFO` & `pypomes_http-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_http
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of Python pomes, pennyeach (HTTP modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-HTTP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-HTTP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.9.0
+Requires-Dist: pypomes-core>=1.0.5
 Requires-Dist: pypomes-security>=0.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```


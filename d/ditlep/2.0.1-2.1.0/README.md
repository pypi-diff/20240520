# Comparing `tmp/ditlep-2.0.1.tar.gz` & `tmp/ditlep-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditlep-2.0.1.tar", max compression
+gzip compressed data, was "ditlep-2.1.0.tar", max compression
```

## Comparing `ditlep-2.0.1.tar` & `ditlep-2.1.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     6711 2024-02-16 13:33:06.308724 ditlep-2.0.1/ditlep/__init__.py
--rw-r--r--   0        0        0      525 2024-02-16 15:11:35.922028 ditlep-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     8992 2024-02-16 15:11:21.125741 ditlep-2.0.1/README.md
--rw-r--r--   0        0        0     9447 1970-01-01 00:00:00.000000 ditlep-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5668 2024-05-20 13:17:49.343505 ditlep-2.1.0/ditlep/__init__.py
+-rw-r--r--   0        0        0     1083 2024-02-16 13:51:52.617802 ditlep-2.1.0/LICENCE
+-rw-r--r--   0        0        0      525 2024-05-20 13:18:13.188680 ditlep-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8774 2024-05-20 13:16:55.029760 ditlep-2.1.0/README.md
+-rw-r--r--   0        0        0     9288 1970-01-01 00:00:00.000000 ditlep-2.1.0/PKG-INFO
```

### Comparing `ditlep-2.0.1/pyproject.toml` & `ditlep-2.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ditlep"
-version = "2.0.1"
+version = "2.1.0"
 description = "Well, this package is a Ditlep API wrapper with a data decryption layer."
 authors = ["Marcuth <example@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.6.1"
```

### Comparing `ditlep-2.0.1/README.md` & `ditlep-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ditlep
 
-Well, this package is a Ditlep API wrapper with a data decryption layer.
+Well, this package is a wrapper for the Ditlep API, a Dragon City information website.
 
 I then intend to add a translation layer using my other library, [`dragon-city-utils`](https://github.com/1Marcuth/py.dragon-city-utils) to obtain translated data regardless of the language, different from what we see on the Ditlep website, which is only in English, but well, that's for sure. when you feel like using this library again ;)
 
 ---
 
 ## Installation
 
@@ -12,30 +12,22 @@
 
 ```
 pip install ditlep
 ```
 
 ## Usage
 
-To use this library is very simple, you just need to create an instance of the Ditlep object and pass some parameters:
+To use this library is very simple, just create an instance of the Ditlep object:
 
 ```python
 from ditlep import Ditlep
 
-ditlep = Ditlep(
-    iv = "...",
-    password = "...",
-    salt = "...",
-    dk_len = ...,
-    count = ...
-)
+ditlep = Ditlep()
 ```
 
-> If you don't know the decryption parameters you can try to contact me so I can give you them
-
 ---
 
 Well, now just be happy, this object can get different information from Ditlep, not all of it because I haven't explored all of Ditlep's existing endpoints, especially since they ended up updating their website recently...
 
 Here's an example of how to get data from the Heroic Race:
 
 ```python
```

### Comparing `ditlep-2.0.1/PKG-INFO` & `ditlep-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: ditlep
-Version: 2.0.1
+Version: 2.1.0
 Summary: Well, this package is a Ditlep API wrapper with a data decryption layer.
 Author: Marcuth
 Author-email: example@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dragon-city-utils (>=2.0.3,<3.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Ditlep
 
-Well, this package is a Ditlep API wrapper with a data decryption layer.
+Well, this package is a wrapper for the Ditlep API, a Dragon City information website.
 
 I then intend to add a translation layer using my other library, [`dragon-city-utils`](https://github.com/1Marcuth/py.dragon-city-utils) to obtain translated data regardless of the language, different from what we see on the Ditlep website, which is only in English, but well, that's for sure. when you feel like using this library again ;)
 
 ---
 
 ## Installation
 
@@ -27,30 +28,22 @@
 
 ```
 pip install ditlep
 ```
 
 ## Usage
 
-To use this library is very simple, you just need to create an instance of the Ditlep object and pass some parameters:
+To use this library is very simple, just create an instance of the Ditlep object:
 
 ```python
 from ditlep import Ditlep
 
-ditlep = Ditlep(
-    iv = "...",
-    password = "...",
-    salt = "...",
-    dk_len = ...,
-    count = ...
-)
+ditlep = Ditlep()
 ```
 
-> If you don't know the decryption parameters you can try to contact me so I can give you them
-
 ---
 
 Well, now just be happy, this object can get different information from Ditlep, not all of it because I haven't explored all of Ditlep's existing endpoints, especially since they ended up updating their website recently...
 
 Here's an example of how to get data from the Heroic Race:
 
 ```python
```


# Comparing `tmp/dawgie-1.4.3rc5.tar.gz` & `tmp/dawgie-1.4.3rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.3rc5.tar", last modified: Tue May  7 22:29:28 2024, max compression
+gzip compressed data, was "dawgie-1.4.3rc6.tar", last modified: Mon May 20 00:34:32 2024, max compression
```

## Comparing `dawgie-1.4.3rc5.tar` & `dawgie-1.4.3rc6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-05-07 22:29:28.738619 dawgie-1.4.3rc5/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2024-05-07 22:29:28.000000 dawgie-1.4.3rc5/LICENSE
--rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-05-07 22:29:28.738619 dawgie-1.4.3rc5/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2024-05-07 22:29:28.000000 dawgie-1.4.3rc5/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-05-07 22:29:28.738619 dawgie-1.4.3rc5/dawgie.egg-info/
--rw-r--r--   0 niessner  (1000) niessner  (1000)     9940 2024-05-07 22:29:28.000000 dawgie-1.4.3rc5/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6632 2024-05-07 22:29:28.000000 dawgie-1.4.3rc5/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2024-05-07 22:29:28.000000 dawgie-1.4.3rc5/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      245 2024-05-07 22:29:28.000000 dawgie-1.4.3rc5/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2024-05-07 22:29:28.000000 dawgie-1.4.3rc5/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2024-05-07 22:29:28.738619 dawgie-1.4.3rc5/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6410 2024-05-07 22:28:20.000000 dawgie-1.4.3rc5/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-05-20 00:34:32.916480 dawgie-1.4.3rc6/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2024-05-20 00:34:32.000000 dawgie-1.4.3rc6/LICENSE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2024-05-20 00:34:32.916480 dawgie-1.4.3rc6/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2024-05-20 00:34:32.000000 dawgie-1.4.3rc6/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2024-05-20 00:34:32.916480 dawgie-1.4.3rc6/dawgie.egg-info/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2024-05-20 00:34:32.000000 dawgie-1.4.3rc6/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6632 2024-05-20 00:34:32.000000 dawgie-1.4.3rc6/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2024-05-20 00:34:32.000000 dawgie-1.4.3rc6/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      245 2024-05-20 00:34:32.000000 dawgie-1.4.3rc6/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2024-05-20 00:34:32.000000 dawgie-1.4.3rc6/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2024-05-20 00:34:32.916480 dawgie-1.4.3rc6/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6410 2024-05-20 00:32:13.000000 dawgie-1.4.3rc6/setup.py
```

### Comparing `dawgie-1.4.3rc5/LICENSE` & `dawgie-1.4.3rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.3rc5/PKG-INFO` & `dawgie-1.4.3rc6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,22 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.3rc5
+Version: 1.4.3rc6
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Free To Use But Restricted
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: bokeh>=1.2
-Requires-Dist: boto3>=1.7.80
-Requires-Dist: cryptography>=2.1.4
-Requires-Dist: dawgie-pydot3==1.0.11
-Requires-Dist: GitPython>=2.1.11
-Requires-Dist: matplotlib>=2.1.1
-Requires-Dist: psycopg>3.0.0
-Requires-Dist: psycopg-binary>3.0.0
-Requires-Dist: pyparsing>=2.4.7
-Requires-Dist: pyOpenSSL>=19.1.0
-Requires-Dist: python-gnupg==0.4.9
-Requires-Dist: requests>=2.20.0
-Requires-Dist: transitions==0.6.8
-Requires-Dist: twisted>=18.7.0
 
 ## DAWGIE
 
 ### Data and Algorithm Work-flow Generation, Introspection, and Execution
 
 The DAWGIE software accomplishes:
```

### Comparing `dawgie-1.4.3rc5/README.md` & `dawgie-1.4.3rc6/README.md`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.3rc5/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.3rc6/dawgie.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,22 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.3rc5
+Version: 1.4.3rc6
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Free To Use But Restricted
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: bokeh>=1.2
-Requires-Dist: boto3>=1.7.80
-Requires-Dist: cryptography>=2.1.4
-Requires-Dist: dawgie-pydot3==1.0.11
-Requires-Dist: GitPython>=2.1.11
-Requires-Dist: matplotlib>=2.1.1
-Requires-Dist: psycopg>3.0.0
-Requires-Dist: psycopg-binary>3.0.0
-Requires-Dist: pyparsing>=2.4.7
-Requires-Dist: pyOpenSSL>=19.1.0
-Requires-Dist: python-gnupg==0.4.9
-Requires-Dist: requests>=2.20.0
-Requires-Dist: transitions==0.6.8
-Requires-Dist: twisted>=18.7.0
 
 ## DAWGIE
 
 ### Data and Algorithm Work-flow Generation, Introspection, and Execution
 
 The DAWGIE software accomplishes:
```

### Comparing `dawgie-1.4.3rc5/setup.py` & `dawgie-1.4.3rc6/setup.py`

 * *Files identical despite different names*


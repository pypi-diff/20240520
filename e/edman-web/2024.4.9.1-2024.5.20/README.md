# Comparing `tmp/edman_web-2024.4.9.1.tar.gz` & `tmp/edman_web-2024.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_web-2024.4.9.1.tar", last modified: Tue Apr  9 04:38:30 2024, max compression
+gzip compressed data, was "edman_web-2024.5.20.tar", last modified: Mon May 20 06:15:31 2024, max compression
```

## Comparing `edman_web-2024.4.9.1.tar` & `edman_web-2024.5.20.tar`

### file list

```diff
@@ -1,35 +1,23 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:38:30.050264 edman_web-2024.4.9.1/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2024.4.9.1/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2516 2024-04-09 04:38:30.050264 edman_web-2024.4.9.1/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      693 2024-04-09 04:37:09.000000 edman_web-2024.4.9.1/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:38:30.050264 edman_web-2024.4.9.1/edman_web/
--rw-r--r--   0 ohno      (1000) ohno      (1000)       82 2023-05-24 06:10:37.000000 edman_web-2024.4.9.1/edman_web/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     9483 2024-02-05 21:30:17.000000 edman_web-2024.4.9.1/edman_web/file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:36:23.000000 edman_web-2024.4.9.1/edman_web/py.typed
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1743 2023-12-06 06:02:11.000000 edman_web-2024.4.9.1/edman_web/search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:38:30.050264 edman_web-2024.4.9.1/edman_web.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2516 2024-04-09 04:38:30.000000 edman_web-2024.4.9.1/edman_web.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      636 2024-04-09 04:38:30.000000 edman_web-2024.4.9.1/edman_web.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-04-09 04:38:30.000000 edman_web-2024.4.9.1/edman_web.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       64 2024-04-09 04:38:30.000000 edman_web-2024.4.9.1/edman_web.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       32 2024-04-09 04:38:30.000000 edman_web-2024.4.9.1/edman_web.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1009 2024-04-09 04:37:09.000000 edman_web-2024.4.9.1/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-04-09 04:38:30.050264 edman_web-2024.4.9.1/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:38:30.050264 edman_web-2024.4.9.1/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    18418 2024-02-05 15:37:54.000000 edman_web-2024.4.9.1/tests/test_file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5897 2023-12-06 06:02:12.000000 edman_web-2024.4.9.1/tests/test_search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:38:30.050264 edman_web-2024.4.9.1/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:38:30.050264 edman_web-2024.4.9.1/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2024-04-09 04:29:55.000000 edman_web-2024.4.9.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:15:31.817570 edman_web-2024.5.20/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2024.5.20/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2514 2024-05-20 06:15:31.817570 edman_web-2024.5.20/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      693 2024-04-09 04:37:09.000000 edman_web-2024.5.20/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:15:31.817570 edman_web-2024.5.20/edman_web/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       82 2023-05-24 06:10:37.000000 edman_web-2024.5.20/edman_web/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     9483 2024-02-05 21:30:17.000000 edman_web-2024.5.20/edman_web/file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:36:23.000000 edman_web-2024.5.20/edman_web/py.typed
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1743 2023-12-06 06:02:11.000000 edman_web-2024.5.20/edman_web/search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:15:31.817570 edman_web-2024.5.20/edman_web.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2514 2024-05-20 06:15:31.000000 edman_web-2024.5.20/edman_web.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      367 2024-05-20 06:15:31.000000 edman_web-2024.5.20/edman_web.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-05-20 06:15:31.000000 edman_web-2024.5.20/edman_web.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       63 2024-05-20 06:15:31.000000 edman_web-2024.5.20/edman_web.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       32 2024-05-20 06:15:31.000000 edman_web-2024.5.20/edman_web.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1007 2024-05-20 06:14:07.000000 edman_web-2024.5.20/pyproject.toml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-05-20 06:15:31.817570 edman_web-2024.5.20/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:15:31.817570 edman_web-2024.5.20/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    18418 2024-02-05 15:37:54.000000 edman_web-2024.5.20/tests/test_file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5897 2023-12-06 06:02:12.000000 edman_web-2024.5.20/tests/test_search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:15:31.817570 edman_web-2024.5.20/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:15:31.817570 edman_web-2024.5.20/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2024-04-09 04:29:55.000000 edman_web-2024.5.20/venv/bin/jp.py
```

### Comparing `edman_web-2024.4.9.1/LICENSE.txt` & `edman_web-2024.5.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2024.4.9.1/PKG-INFO` & `edman_web-2024.5.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_web
-Version: 2024.4.9.1
+Version: 2024.5.20
 Summary: Sub-package of edman for web applications.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno, Yusuke Yamada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: pymongo~=4.6.2
-Requires-Dist: edman~=2024.4.9.1
-Requires-Dist: Werkzeug~=3.0.2
+Requires-Dist: pymongo~=4.7.2
+Requires-Dist: edman~=2024.5.20
+Requires-Dist: Werkzeug~=3.0.3
 Requires-Dist: Pillow~=10.3.0
 
 edman_web
 =========
 
 |py_version|
```

### Comparing `edman_web-2024.4.9.1/README.rst` & `edman_web-2024.5.20/README.rst`

 * *Files identical despite different names*

### Comparing `edman_web-2024.4.9.1/edman_web/file_manager.py` & `edman_web-2024.5.20/edman_web/file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.4.9.1/edman_web/search_manager.py` & `edman_web-2024.5.20/edman_web/search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.4.9.1/edman_web.egg-info/PKG-INFO` & `edman_web-2024.5.20/edman_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_web
-Version: 2024.4.9.1
+Version: 2024.5.20
 Summary: Sub-package of edman for web applications.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno, Yusuke Yamada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: pymongo~=4.6.2
-Requires-Dist: edman~=2024.4.9.1
-Requires-Dist: Werkzeug~=3.0.2
+Requires-Dist: pymongo~=4.7.2
+Requires-Dist: edman~=2024.5.20
+Requires-Dist: Werkzeug~=3.0.3
 Requires-Dist: Pillow~=10.3.0
 
 edman_web
 =========
 
 |py_version|
```

### Comparing `edman_web-2024.4.9.1/pyproject.toml` & `edman_web-2024.5.20/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
-    "pymongo~=4.6.2",
-    "edman~=2024.4.9.1",
-    "Werkzeug~=3.0.2",
+    "pymongo~=4.7.2",
+    "edman~=2024.5.20",
+    "Werkzeug~=3.0.3",
     "Pillow~=10.3.0"
 ]
-version = "2024.4.9.1"
+version = "2024.5.20"
 
 [project.urls]
 "documentation" = "https://ryde.github.io/edman_web/"
 "repository" = "https://github.com/ryde/edman_web"
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
```

### Comparing `edman_web-2024.4.9.1/tests/test_file_manager.py` & `edman_web-2024.5.20/tests/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.4.9.1/tests/test_search_manager.py` & `edman_web-2024.5.20/tests/test_search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.4.9.1/venv/bin/jp.py` & `edman_web-2024.5.20/venv/bin/jp.py`

 * *Files identical despite different names*


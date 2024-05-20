# Comparing `tmp/edman_cli-2024.4.9.1.tar.gz` & `tmp/edman_cli-2024.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_cli-2024.4.9.1.tar", last modified: Tue Apr  9 04:22:07 2024, max compression
+gzip compressed data, was "edman_cli-2024.5.20.tar", last modified: Mon May 20 06:01:52 2024, max compression
```

## Comparing `edman_cli-2024.4.9.1.tar` & `edman_cli-2024.5.20.tar`

### file list

```diff
@@ -1,46 +1,34 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:22:07.400293 edman_cli-2024.4.9.1/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2024.4.9.1/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7268 2024-04-09 04:22:07.400293 edman_cli-2024.4.9.1/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5613 2024-04-09 04:20:08.000000 edman_cli-2024.4.9.1/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:22:07.400293 edman_cli-2024.4.9.1/edman_cli.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7268 2024-04-09 04:22:07.000000 edman_cli-2024.4.9.1/edman_cli.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      853 2024-04-09 04:22:07.000000 edman_cli-2024.4.9.1/edman_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-04-09 04:22:07.000000 edman_cli-2024.4.9.1/edman_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2024-04-09 04:22:07.000000 edman_cli-2024.4.9.1/edman_cli.egg-info/entry_points.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       78 2024-04-09 04:22:07.000000 edman_cli-2024.4.9.1/edman_cli.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2024-04-09 04:22:07.000000 edman_cli-2024.4.9.1/edman_cli.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1475 2024-04-09 04:20:08.000000 edman_cli-2024.4.9.1/pyproject.toml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:22:07.400293 edman_cli-2024.4.9.1/scripts/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16648 2023-11-17 06:13:18.000000 edman_cli-2024.4.9.1/scripts/action.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2305 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/assign_bson_type.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3523 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/db_create.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2757 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/db_destroy.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1626 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2666 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/entry.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2297 2023-11-17 06:13:18.000000 edman_cli-2024.4.9.1/scripts/file_add.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3033 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/file_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2519 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/file_dl.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2406 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/find.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2708 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/item_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2166 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/pullout.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2492 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/structure_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2163 2023-05-24 05:52:45.000000 edman_cli-2024.4.9.1/scripts/update.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-04-09 04:22:07.400293 edman_cli-2024.4.9.1/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:22:07.400293 edman_cli-2024.4.9.1/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    11565 2023-12-06 06:13:48.000000 edman_cli-2024.4.9.1/tests/test_action.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:22:07.390293 edman_cli-2024.4.9.1/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:22:07.400293 edman_cli-2024.4.9.1/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2024-04-09 04:10:40.000000 edman_cli-2024.4.9.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:01:52.617831 edman_cli-2024.5.20/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2024.5.20/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7266 2024-05-20 06:01:52.617831 edman_cli-2024.5.20/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5613 2024-04-09 04:20:08.000000 edman_cli-2024.5.20/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:01:52.617831 edman_cli-2024.5.20/edman_cli.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7266 2024-05-20 06:01:52.000000 edman_cli-2024.5.20/edman_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      584 2024-05-20 06:01:52.000000 edman_cli-2024.5.20/edman_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-05-20 06:01:52.000000 edman_cli-2024.5.20/edman_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2024-05-20 06:01:52.000000 edman_cli-2024.5.20/edman_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       77 2024-05-20 06:01:52.000000 edman_cli-2024.5.20/edman_cli.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2024-05-20 06:01:52.000000 edman_cli-2024.5.20/edman_cli.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1473 2024-05-20 06:00:19.000000 edman_cli-2024.5.20/pyproject.toml
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:01:52.617831 edman_cli-2024.5.20/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16648 2023-11-17 06:13:18.000000 edman_cli-2024.5.20/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2305 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3523 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2757 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1626 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2666 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2297 2023-11-17 06:13:18.000000 edman_cli-2024.5.20/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3033 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2519 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2406 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2708 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2166 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2492 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2163 2023-05-24 05:52:45.000000 edman_cli-2024.5.20/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-05-20 06:01:52.617831 edman_cli-2024.5.20/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:01:52.617831 edman_cli-2024.5.20/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    11565 2023-12-06 06:13:48.000000 edman_cli-2024.5.20/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:01:52.617831 edman_cli-2024.5.20/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 06:01:52.617831 edman_cli-2024.5.20/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2024-04-09 04:10:40.000000 edman_cli-2024.5.20/venv/bin/jp.py
```

### Comparing `edman_cli-2024.4.9.1/LICENSE.txt` & `edman_cli-2024.5.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/PKG-INFO` & `edman_cli-2024.5.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_cli
-Version: 2024.4.9.1
+Version: 2024.5.20
 Summary: Sub-package of edman for cli applications and scripts.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: pymongo~=4.6.2
+Requires-Dist: pymongo~=4.7.2
 Requires-Dist: python-dateutil~=2.9.0.post0
 Requires-Dist: jmespath~=1.0.1
-Requires-Dist: edman~=2024.4.9.1
+Requires-Dist: edman~=2024.5.20
 
 edman_cli
 =========
 
 |py_version|
 
 |  EDMAN(KEK IMSS SBRC/PF Experimental Data Management System)用のコマンドラインスクリプト。
```

### Comparing `edman_cli-2024.4.9.1/README.rst` & `edman_cli-2024.5.20/README.rst`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/edman_cli.egg-info/PKG-INFO` & `edman_cli-2024.5.20/edman_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_cli
-Version: 2024.4.9.1
+Version: 2024.5.20
 Summary: Sub-package of edman for cli applications and scripts.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: pymongo~=4.6.2
+Requires-Dist: pymongo~=4.7.2
 Requires-Dist: python-dateutil~=2.9.0.post0
 Requires-Dist: jmespath~=1.0.1
-Requires-Dist: edman~=2024.4.9.1
+Requires-Dist: edman~=2024.5.20
 
 edman_cli
 =========
 
 |py_version|
 
 |  EDMAN(KEK IMSS SBRC/PF Experimental Data Management System)用のコマンドラインスクリプト。
```

### Comparing `edman_cli-2024.4.9.1/edman_cli.egg-info/SOURCES.txt` & `edman_cli-2024.5.20/edman_cli.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -19,20 +19,8 @@
 scripts/file_dl.py
 scripts/find.py
 scripts/item_delete.py
 scripts/pullout.py
 scripts/structure_convert.py
 scripts/update.py
 tests/test_action.py
-venv/bin/jp.py
-venv/bin/rst2html.py
-venv/bin/rst2html4.py
-venv/bin/rst2html5.py
-venv/bin/rst2latex.py
-venv/bin/rst2man.py
-venv/bin/rst2odt.py
-venv/bin/rst2odt_prepstyles.py
-venv/bin/rst2pseudoxml.py
-venv/bin/rst2s5.py
-venv/bin/rst2xetex.py
-venv/bin/rst2xml.py
-venv/bin/rstpep2html.py
+venv/bin/jp.py
```

### Comparing `edman_cli-2024.4.9.1/edman_cli.egg-info/entry_points.txt` & `edman_cli-2024.5.20/edman_cli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/pyproject.toml` & `edman_cli-2024.5.20/pyproject.toml`

 * *Files 21% similar despite different names*

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
+    "pymongo~=4.7.2",
     "python-dateutil~=2.9.0.post0",
     "jmespath~=1.0.1",
-    "edman~=2024.4.9.1",
+    "edman~=2024.5.20",
 ]
-version = "2024.4.9.1"
+version = "2024.5.20"
 
 [project.urls]
 "repository" = "https://github.com/ryde/edman_cli"
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
```

### Comparing `edman_cli-2024.4.9.1/scripts/action.py` & `edman_cli-2024.5.20/scripts/action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/assign_bson_type.py` & `edman_cli-2024.5.20/scripts/assign_bson_type.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/db_create.py` & `edman_cli-2024.5.20/scripts/db_create.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/db_destroy.py` & `edman_cli-2024.5.20/scripts/db_destroy.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/delete.py` & `edman_cli-2024.5.20/scripts/delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/entry.py` & `edman_cli-2024.5.20/scripts/entry.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/file_add.py` & `edman_cli-2024.5.20/scripts/file_add.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/file_delete.py` & `edman_cli-2024.5.20/scripts/file_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/file_dl.py` & `edman_cli-2024.5.20/scripts/file_dl.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/find.py` & `edman_cli-2024.5.20/scripts/find.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/item_delete.py` & `edman_cli-2024.5.20/scripts/item_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/pullout.py` & `edman_cli-2024.5.20/scripts/pullout.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/structure_convert.py` & `edman_cli-2024.5.20/scripts/structure_convert.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/scripts/update.py` & `edman_cli-2024.5.20/scripts/update.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/tests/test_action.py` & `edman_cli-2024.5.20/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.4.9.1/venv/bin/jp.py` & `edman_cli-2024.5.20/venv/bin/jp.py`

 * *Files identical despite different names*


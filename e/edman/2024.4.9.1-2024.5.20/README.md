# Comparing `tmp/edman-2024.4.9.1.tar.gz` & `tmp/edman-2024.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman-2024.4.9.1.tar", last modified: Tue Apr  9 04:11:51 2024, max compression
+gzip compressed data, was "edman-2024.5.20.tar", last modified: Mon May 20 02:34:48 2024, max compression
```

## Comparing `edman-2024.4.9.1.tar` & `edman-2024.5.20.tar`

### file list

```diff
@@ -1,61 +1,49 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.970306 edman-2024.4.9.1/.github/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/.github/workflows/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1575 2024-04-09 03:58:46.000000 edman-2024.4.9.1/.github/workflows/unittest.yml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2283 2023-12-04 07:30:57.000000 edman-2024.4.9.1/.gitignore
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/.idea/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2024.4.9.1/.idea/.gitignore
--rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2024-04-09 03:58:46.000000 edman-2024.4.9.1/.idea/edman.iml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/.idea/inspectionProfiles/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2024.4.9.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      414 2024-04-09 03:58:46.000000 edman-2024.4.9.1/.idea/misc.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2024.4.9.1/.idea/modules.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2024.4.9.1/.idea/vcs.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2024.4.9.1/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)    13451 2024-04-09 04:11:51.980306 edman-2024.4.9.1/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)    11982 2024-04-09 03:58:46.000000 edman-2024.4.9.1/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/edman/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      169 2024-04-08 07:28:55.000000 edman-2024.4.9.1/edman/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1537 2023-11-15 06:06:42.000000 edman-2024.4.9.1/edman/config.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16853 2023-12-04 07:30:57.000000 edman-2024.4.9.1/edman/convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    50847 2024-02-02 05:59:23.000000 edman-2024.4.9.1/edman/db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      849 2023-12-04 07:30:57.000000 edman-2024.4.9.1/edman/exceptions.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    26367 2023-12-04 07:30:57.000000 edman-2024.4.9.1/edman/file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1748 2023-12-04 07:30:57.000000 edman-2024.4.9.1/edman/json_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-22 08:18:53.000000 edman-2024.4.9.1/edman/py.typed
--rw-r--r--   0 ohno      (1000) ohno      (1000)    14173 2024-04-08 07:30:17.000000 edman-2024.4.9.1/edman/search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    11156 2023-12-04 07:30:57.000000 edman-2024.4.9.1/edman/utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/edman.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    13451 2024-04-09 04:11:51.000000 edman-2024.4.9.1/edman.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      986 2024-04-09 04:11:51.000000 edman-2024.4.9.1/edman.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-04-09 04:11:51.000000 edman-2024.4.9.1/edman.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       60 2024-04-09 04:11:51.000000 edman-2024.4.9.1/edman.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2024-04-09 04:11:51.000000 edman-2024.4.9.1/edman.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1131 2024-04-09 03:58:46.000000 edman-2024.4.9.1/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1000 2024-04-09 01:29:54.000000 edman-2024.4.9.1/requirements.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-04-09 04:11:51.980306 edman-2024.4.9.1/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2024.4.9.1/tests/__init__.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/tests/ini/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2024.4.9.1/tests/ini/test_db.ini.sample
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12919 2023-12-04 07:30:57.000000 edman-2024.4.9.1/tests/test_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)   109061 2024-02-02 05:59:23.000000 edman-2024.4.9.1/tests/test_db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    45802 2023-12-04 07:30:57.000000 edman-2024.4.9.1/tests/test_file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6644 2023-12-04 07:30:57.000000 edman-2024.4.9.1/tests/test_multiuser.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    38599 2023-12-19 08:12:30.000000 edman-2024.4.9.1/tests/test_search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     8682 2023-12-04 07:30:57.000000 edman-2024.4.9.1/tests/test_utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.970306 edman-2024.4.9.1/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 04:11:51.980306 edman-2024.4.9.1/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      626 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2024-04-09 02:20:12.000000 edman-2024.4.9.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/.github/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/.github/workflows/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1575 2024-04-09 03:58:46.000000 edman-2024.5.20/.github/workflows/unittest.yml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2283 2023-12-04 07:30:57.000000 edman-2024.5.20/.gitignore
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/.idea/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2024.5.20/.idea/.gitignore
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2024-05-20 02:19:59.000000 edman-2024.5.20/.idea/edman.iml
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/.idea/inspectionProfiles/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2024.5.20/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      414 2024-05-20 02:19:59.000000 edman-2024.5.20/.idea/misc.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2024.5.20/.idea/modules.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2024.5.20/.idea/vcs.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2024.5.20/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    13450 2024-05-20 02:34:48.271642 edman-2024.5.20/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    11982 2024-04-09 03:58:46.000000 edman-2024.5.20/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/edman/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      169 2024-04-08 07:28:55.000000 edman-2024.5.20/edman/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1537 2023-11-15 06:06:42.000000 edman-2024.5.20/edman/config.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16853 2023-12-04 07:30:57.000000 edman-2024.5.20/edman/convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    50847 2024-02-02 05:59:23.000000 edman-2024.5.20/edman/db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      849 2023-12-04 07:30:57.000000 edman-2024.5.20/edman/exceptions.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    26367 2023-12-04 07:30:57.000000 edman-2024.5.20/edman/file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1748 2023-12-04 07:30:57.000000 edman-2024.5.20/edman/json_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-22 08:18:53.000000 edman-2024.5.20/edman/py.typed
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    14173 2024-04-08 07:30:17.000000 edman-2024.5.20/edman/search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    11156 2023-12-04 07:30:57.000000 edman-2024.5.20/edman/utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/edman.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    13450 2024-05-20 02:34:48.000000 edman-2024.5.20/edman.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      717 2024-05-20 02:34:48.000000 edman-2024.5.20/edman.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-05-20 02:34:48.000000 edman-2024.5.20/edman.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       60 2024-05-20 02:34:48.000000 edman-2024.5.20/edman.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2024-05-20 02:34:48.000000 edman-2024.5.20/edman.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1130 2024-05-20 02:19:59.000000 edman-2024.5.20/pyproject.toml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1001 2024-05-20 02:19:59.000000 edman-2024.5.20/requirements.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-05-20 02:34:48.271642 edman-2024.5.20/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2024.5.20/tests/__init__.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/tests/ini/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2024.5.20/tests/ini/test_db.ini.sample
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12919 2023-12-04 07:30:57.000000 edman-2024.5.20/tests/test_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)   109061 2024-02-02 05:59:23.000000 edman-2024.5.20/tests/test_db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    45802 2023-12-04 07:30:57.000000 edman-2024.5.20/tests/test_file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6644 2023-12-04 07:30:57.000000 edman-2024.5.20/tests/test_multiuser.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    38599 2023-12-19 08:12:30.000000 edman-2024.5.20/tests/test_search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     8682 2023-12-04 07:30:57.000000 edman-2024.5.20/tests/test_utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-05-20 02:34:48.271642 edman-2024.5.20/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2024-04-09 02:20:12.000000 edman-2024.5.20/venv/bin/jp.py
```

### Comparing `edman-2024.4.9.1/.github/workflows/unittest.yml` & `edman-2024.5.20/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/.gitignore` & `edman-2024.5.20/.gitignore`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/.idea/edman.iml` & `edman-2024.5.20/.idea/edman.iml`

 * *Files 1% similar despite different names*

#### Comparing `edman-2024.4.9.1/.idea/edman.iml` & `edman-2024.5.20/.idea/edman.iml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <module type="PYTHON_MODULE" version="4">
   <component name="NewModuleRootManager">
     <content url="file://$MODULE_DIR$">
       <sourceFolder url="file://$MODULE_DIR$/tests" isTestSource="true"/>
       <sourceFolder url="file://$MODULE_DIR$/edman" isTestSource="false"/>
     </content>
-    <orderEntry type="jdk" jdkName="Python 3.12.2 WSL (Ubuntu): (/home/ohno/dev/new_edman/edman/venv/bin/python)" jdkType="Python SDK"/>
+    <orderEntry type="jdk" jdkName="Python 3.12.3 WSL (Ubuntu): (/home/ohno/dev/new_edman/edman/venv/bin/python)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
 </module>
```

### Comparing `edman-2024.4.9.1/LICENSE.txt` & `edman-2024.5.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/PKG-INFO` & `edman-2024.5.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2024.4.9.1
+Version: 2024.5.20
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: pymongo>=4.6.2
+Requires-Dist: pymongo>=4.7.2
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: jmespath>=1.0.1
 
 edman
 =====
 
 |py_version|
```

### Comparing `edman-2024.4.9.1/README.rst` & `edman-2024.5.20/README.rst`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman/config.py` & `edman-2024.5.20/edman/config.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman/convert.py` & `edman-2024.5.20/edman/convert.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman/db.py` & `edman-2024.5.20/edman/db.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman/exceptions.py` & `edman-2024.5.20/edman/exceptions.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman/file.py` & `edman-2024.5.20/edman/file.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman/json_manager.py` & `edman-2024.5.20/edman/json_manager.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman/search.py` & `edman-2024.5.20/edman/search.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman/utils.py` & `edman-2024.5.20/edman/utils.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/edman.egg-info/PKG-INFO` & `edman-2024.5.20/edman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2024.4.9.1
+Version: 2024.5.20
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: pymongo>=4.6.2
+Requires-Dist: pymongo>=4.7.2
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: jmespath>=1.0.1
 
 edman
 =====
 
 |py_version|
```

### Comparing `edman-2024.4.9.1/pyproject.toml` & `edman-2024.5.20/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
-    "pymongo>=4.6.2",
+    "pymongo>=4.7.2",
     "python-dateutil>=2.9.0.post0",
     "jmespath>=1.0.1",
 ]
-version = "2024.4.9.1"
+version = "2024.5.20"
 # dynamic = ["version"]
 
 [project.urls]
 "documentation" = "https://ryde.github.io/edman/"
 "repository" = "https://github.com/ryde/edman"
 
 [tool.setuptools.packages.find]
```

### Comparing `edman-2024.4.9.1/requirements.txt` & `edman-2024.5.20/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-backports.tarfile==1.0.0
+backports.tarfile==1.1.1
 build==1.2.1
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
-cryptography==42.0.5
+cryptography==42.0.7
 dnspython==2.6.1
-docutils==0.20.1
+docutils==0.21.2
 flake8==7.0.0
-idna==3.6
+idna==3.7
 importlib_metadata==7.1.0
 iniconfig==2.0.0
 isort==5.13.2
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
-jaraco.functools==4.0.0
+jaraco.functools==4.0.1
 jeepney==0.8.0
 jmespath==1.0.1
-keyring==25.1.0
+keyring==25.2.1
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.2.0
-mypy==1.9.0
+mypy==1.10.0
 mypy-extensions==1.0.0
 nh3==0.2.17
 packaging==24.0
 pkginfo==1.10.0
-pluggy==1.4.0
+pluggy==1.5.0
 pycodestyle==2.11.1
 pycparser==2.22
 pyflakes==3.2.0
-Pygments==2.17.2
-pymongo==4.6.2
-pyproject_hooks==1.0.0
-pytest==8.1.1
+Pygments==2.18.0
+pymongo==4.7.2
+pyproject_hooks==1.1.0
+pytest==8.2.1
 python-dateutil==2.9.0.post0
 readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 SecretStorage==3.3.3
 six==1.16.0
 toml==0.10.2
 tomli==2.0.1
-twine==5.0.0
+twine==5.1.0
 types-jmespath==1.0.2.20240106
 types-python-dateutil==2.9.0.20240316
 typing_extensions==4.11.0
 urllib3==2.2.1
-zipp==3.18.1
+zipp==3.18.2
```

### Comparing `edman-2024.4.9.1/tests/test_convert.py` & `edman-2024.5.20/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/tests/test_db.py` & `edman-2024.5.20/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/tests/test_file.py` & `edman-2024.5.20/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/tests/test_multiuser.py` & `edman-2024.5.20/tests/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/tests/test_search.py` & `edman-2024.5.20/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/tests/test_utils.py` & `edman-2024.5.20/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edman-2024.4.9.1/venv/bin/jp.py` & `edman-2024.5.20/venv/bin/jp.py`

 * *Files identical despite different names*


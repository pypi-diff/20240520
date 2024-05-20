# Comparing `tmp/BarteSDK-0.1.3.tar.gz` & `tmp/BarteSDK-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-0.1.3.tar", last modified: Thu May 16 16:54:39 2024, max compression
+gzip compressed data, was "BarteSDK-0.1.4.tar", last modified: Mon May 20 18:14:04 2024, max compression
```

## Comparing `BarteSDK-0.1.3.tar` & `BarteSDK-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:54:39.805626 BarteSDK-0.1.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:54:39.801626 BarteSDK-0.1.3/BarteChargesAPI/
--rw-rw-r--   0 root         (0) root         (0)       34 2024-05-16 16:51:06.000000 BarteSDK-0.1.3/BarteChargesAPI/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      405 2024-05-16 16:51:06.000000 BarteSDK-0.1.3/BarteChargesAPI/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:54:39.801626 BarteSDK-0.1.3/BarteReportAPI/
--rw-rw-r--   0 root         (0) root         (0)       33 2024-05-16 16:51:06.000000 BarteSDK-0.1.3/BarteReportAPI/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      718 2024-05-16 16:51:06.000000 BarteSDK-0.1.3/BarteReportAPI/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:54:39.805626 BarteSDK-0.1.3/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4072 2024-05-16 16:54:39.000000 BarteSDK-0.1.3/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-16 16:54:39.000000 BarteSDK-0.1.3/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 16:54:39.000000 BarteSDK-0.1.3/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-16 16:54:39.000000 BarteSDK-0.1.3/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-16 16:54:39.000000 BarteSDK-0.1.3/BarteSDK.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-16 16:51:06.000000 BarteSDK-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4072 2024-05-16 16:54:39.805626 BarteSDK-0.1.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3796 2024-05-16 16:54:21.000000 BarteSDK-0.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 16:54:39.805626 BarteSDK-0.1.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      562 2024-05-16 16:54:24.000000 BarteSDK-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:14:04.005409 BarteSDK-0.1.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:14:04.001409 BarteSDK-0.1.4/BarteChargesAPI/
+-rw-rw-r--   0 root         (0) root         (0)       34 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/BarteChargesAPI/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      405 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/BarteChargesAPI/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:14:04.001409 BarteSDK-0.1.4/BarteReportAPI/
+-rw-rw-r--   0 root         (0) root         (0)       33 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/BarteReportAPI/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      718 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/BarteReportAPI/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:14:04.001409 BarteSDK-0.1.4/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4072 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4072 2024-05-20 18:14:04.005409 BarteSDK-0.1.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3796 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 18:14:04.005409 BarteSDK-0.1.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      562 2024-05-20 18:13:42.000000 BarteSDK-0.1.4/setup.py
```

### Comparing `BarteSDK-0.1.3/BarteReportAPI/main.py` & `BarteSDK-0.1.4/BarteReportAPI/main.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-0.1.3/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-0.1.4/BarteSDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-0.1.3/PKG-INFO` & `BarteSDK-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-0.1.3/README.md` & `BarteSDK-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-0.1.3/setup.py` & `BarteSDK-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```


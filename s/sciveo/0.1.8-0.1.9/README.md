# Comparing `tmp/sciveo-0.1.8.tar.gz` & `tmp/sciveo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.1.8.tar", last modified: Mon May  6 11:13:19 2024, max compression
+gzip compressed data, was "sciveo-0.1.9.tar", last modified: Thu May 16 11:30:25 2024, max compression
```

## Comparing `sciveo-0.1.8.tar` & `sciveo-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.841565 sciveo-0.1.8/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6829 2024-05-06 11:13:19.841400 sciveo-0.1.8/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6677 2024-05-06 11:12:30.000000 sciveo-0.1.8/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.817572 sciveo-0.1.8/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.825704 sciveo-0.1.8/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.8/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1873 2024-05-06 10:10:30.000000 sciveo-0.1.8/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.8/sciveo/api/upload.py
--rwxr-xr-x   0 sgeorgiev   (501) staff       (20)     1192 2024-05-06 10:11:13.000000 sciveo-0.1.8/sciveo/cli.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.828107 sciveo-0.1.8/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.8/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.8/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.8/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.8/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.8/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.831650 sciveo-0.1.8/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.8/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1744 2024-05-06 10:29:34.000000 sciveo-0.1.8/sciveo/common/tools/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.8/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-21 12:16:37.000000 sciveo-0.1.8/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1145 2024-05-06 10:13:15.000000 sciveo-0.1.8/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/common/tools/synchronized.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/common/tools/timers.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.833562 sciveo-0.1.8/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.8/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.8/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.8/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.8/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.8/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.835942 sciveo-0.1.8/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.8/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5903 2024-04-21 12:33:00.000000 sciveo-0.1.8/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3790 2024-04-21 07:50:35.000000 sciveo-0.1.8/sciveo/monitoring/network.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.8/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-05-06 05:53:05.000000 sciveo-0.1.8/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.824403 sciveo-0.1.8/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6829 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1049 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       43 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/entry_points.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-05-06 11:13:19.000000 sciveo-0.1.8/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-05-06 11:13:19.841624 sciveo-0.1.8/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      901 2024-05-06 09:54:04.000000 sciveo-0.1.8/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-06 11:13:19.840989 sciveo-0.1.8/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.8/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.8/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.8/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.8/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.511246 sciveo-0.1.9/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6829 2024-05-16 11:30:25.511096 sciveo-0.1.9/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6677 2024-05-06 11:12:30.000000 sciveo-0.1.9/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.490437 sciveo-0.1.9/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.9/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.500774 sciveo-0.1.9/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.9/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1873 2024-05-06 10:10:30.000000 sciveo-0.1.9/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.9/sciveo/api/upload.py
+-rwxr-xr-x   0 sgeorgiev   (501) staff       (20)     1192 2024-05-06 10:11:13.000000 sciveo-0.1.9/sciveo/cli.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.502506 sciveo-0.1.9/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.9/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.9/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.9/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.9/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.9/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.505862 sciveo-0.1.9/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.9/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1744 2024-05-06 10:29:34.000000 sciveo-0.1.9/sciveo/common/tools/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.9/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.9/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-21 12:16:37.000000 sciveo-0.1.9/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1145 2024-05-06 10:13:15.000000 sciveo-0.1.9/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.9/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.9/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.507577 sciveo-0.1.9/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.9/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.9/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.9/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.9/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.9/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.509019 sciveo-0.1.9/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.9/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5903 2024-04-21 12:33:00.000000 sciveo-0.1.9/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2921 2024-05-16 11:28:14.000000 sciveo-0.1.9/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.9/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-05-16 11:04:13.000000 sciveo-0.1.9/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.499249 sciveo-0.1.9/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6829 2024-05-16 11:30:25.000000 sciveo-0.1.9/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1049 2024-05-16 11:30:25.000000 sciveo-0.1.9/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-05-16 11:30:25.000000 sciveo-0.1.9/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       43 2024-05-16 11:30:25.000000 sciveo-0.1.9/sciveo.egg-info/entry_points.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-05-16 11:30:25.000000 sciveo-0.1.9/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-05-16 11:30:25.000000 sciveo-0.1.9/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-05-16 11:30:25.511297 sciveo-0.1.9/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      901 2024-05-06 09:54:04.000000 sciveo-0.1.9/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-05-16 11:30:25.510732 sciveo-0.1.9/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.9/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.9/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.9/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.9/test/test_sampling.py
```

### Comparing `sciveo-0.1.8/PKG-INFO` & `sciveo-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
```

### Comparing `sciveo-0.1.8/README.md` & `sciveo-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/__init__.py` & `sciveo-0.1.9/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/api/base.py` & `sciveo-0.1.9/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/api/upload.py` & `sciveo-0.1.9/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/cli.py` & `sciveo-0.1.9/sciveo/cli.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/configuration.py` & `sciveo-0.1.9/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/model.py` & `sciveo-0.1.9/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/optimizers.py` & `sciveo-0.1.9/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/sampling.py` & `sciveo-0.1.9/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/tools/configuration.py` & `sciveo-0.1.9/sciveo/common/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/tools/daemon.py` & `sciveo-0.1.9/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/tools/formating.py` & `sciveo-0.1.9/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/tools/hardware.py` & `sciveo-0.1.9/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/tools/logger.py` & `sciveo-0.1.9/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/tools/synchronized.py` & `sciveo-0.1.9/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/common/tools/timers.py` & `sciveo-0.1.9/sciveo/common/tools/timers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/content/dataset.py` & `sciveo-0.1.9/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/content/experiment.py` & `sciveo-0.1.9/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/content/project.py` & `sciveo-0.1.9/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/content/runner.py` & `sciveo-0.1.9/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/monitoring/monitor.py` & `sciveo-0.1.9/sciveo/monitoring/monitor.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo/monitoring/network.py` & `sciveo-0.1.9/sciveo/monitoring/network.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,49 +6,20 @@
 # from the owner. For licensing inquiries, please
 # contact pavlin@softel.bg.
 #
 # 2024
 #
 
 import socket
-import asyncio
+import threading
 
 from sciveo.common.tools.logger import *
 from sciveo.common.tools.timers import Timer
 
 
-class NetworkScanner:
-  def __init__(self, timeout=1.0):
-    self.timeout = timeout
-
-  async def scan_port(self, ip, port):
-    try:
-      reader, writer = await asyncio.wait_for(asyncio.open_connection(ip, port), timeout=self.timeout)
-      writer.close()
-      await writer.wait_closed()
-      return (ip, port)
-    except Exception as e:
-      # print("Exception", e)
-      return None
-
-  async def scan_all_ports(self, ip, ports):
-    tasks = [self.scan_port(ip, port) for port in ports]
-    return await asyncio.gather(*tasks)
-
-  async def scan_async(self, ips, ports):
-    results = []
-    for ip in ips:
-      results.extend(await self.scan_all_ports(ip, ports))
-    results = [x for x in results if x is not None]
-    return results
-
-  def scan(self, ips, ports):
-    return asyncio.run(self.scan_async(ips, ports))
-
-
 class NetworkTools:
   def __init__(self, **kwargs):
     self.default_arguments = {
       "timeout": 0.1,
       "localhost": False,
     }
 
@@ -56,14 +27,17 @@
     for k, v in self.default_arguments.items():
       self.arguments[k] = kwargs.get(k, v)
 
     self.net_classes = ["192.168.", "10."]
     for i in range(16, 32):
       self.net_classes.append(f"172.{i}.")
 
+    self.data = {"scan": {}}
+    self.data_lock = threading.Lock()
+
   def get_local_nets(self):
     list_local_ips = []
     try:
       import netifaces
       interfaces = netifaces.interfaces()
       for interface in interfaces:
         addrs = netifaces.ifaddresses(interface)
@@ -79,52 +53,45 @@
   def generate_ip_list(self, base_ip):
     octets = base_ip.split('.')
     network_prefix = '.'.join(octets[:3])
     return [f'{network_prefix}.{i}' for i in range(1, 255)]
 
   def scan_port(self, port=22):
     t = Timer()
-    result = []
     list_local_ips = self.get_local_nets()
     debug(type(self).__name__, "scan_port", "list_local_ips", list_local_ips)
     for local_ip in list_local_ips:
       list_ip = self.generate_ip_list(local_ip)
-      result += self.scan_port_hosts(list_ip, port)
+      self.scan_port_hosts(list_ip, port)
     if self.arguments["localhost"]:
-      result += self.scan_port_hosts(["127.0.0.1"], port)
-    debug(type(self).__name__, "scan_port elapsed time", t.stop(), "result", result)
-    return result
+      self.scan_port_hosts(["127.0.0.1"], port)
+    debug(type(self).__name__, f"scan_port [{port}] elapsed time", t.stop(), self.data["scan"][port])
+    return self.data["scan"][port]
 
   def scan_port_hosts(self, list_ip, port=22):
-    list_hosts = []
     timeout = self.arguments["timeout"]
+    list_threads = []
     for ip in list_ip:
-      try:
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
-          sock.settimeout(timeout)
-          result = sock.connect_ex((ip, port))
-          if result == 0:
-            list_hosts.append(ip)
-          # debug(type(self).__name__, "scan_ports", ip, port, result)
-      except socket.error:
-        pass
-    return list_hosts
+      t = threading.Thread(target=self.scan_host_port, args=(ip, port, timeout))
+      t.start()
+      list_threads.append(t)
+    for t in list_threads:
+      t.join()
+
+  def scan_host_port(self, ip, port, timeout):
+    try:
+      with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
+        sock.settimeout(timeout)
+        result = sock.connect_ex((ip, port))
+        if result == 0:
+          with self.data_lock:
+            self.data["scan"].setdefault(port, [])
+            self.data["scan"][port].append(ip)
+        # debug(type(self).__name__, "scan_ports", ip, port, result)
+    except socket.error:
+      pass
 
 
 if __name__ == "__main__":
-  t1 = Timer()
   net = NetworkTools(timeout=0.5, localhost=True)
-  result = net.scan_port(port=22)
-  t1 = t1.stop()
-  print(result, "elapsed", t1)
-
-  t2 = Timer()
-  list_local_ips = net.get_local_nets()
-  list_scan_ips = []
-  for local_ip in list_local_ips:
-    list_scan_ips += net.generate_ip_list(local_ip)
-  # print(list_scan_ips)
-  ns = NetworkScanner(timeout=0.5)
-  result = ns.scan(list_scan_ips, [22])
-  t2 = t2.stop()
-  print(result, "elapsed", t2)
-  print("elapsed", t1, t2, t1 - t2)
+  list_hosts = net.scan_port(port=22)
+  print(list_hosts)
```

### Comparing `sciveo-0.1.8/sciveo/monitoring/start.py` & `sciveo-0.1.9/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/sciveo.egg-info/PKG-INFO` & `sciveo-0.1.9/sciveo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
```

### Comparing `sciveo-0.1.8/sciveo.egg-info/SOURCES.txt` & `sciveo-0.1.9/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/setup.py` & `sciveo-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/test/test_configuration.py` & `sciveo-0.1.9/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/test/test_monitoring.py` & `sciveo-0.1.9/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/test/test_runner.py` & `sciveo-0.1.9/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.8/test/test_sampling.py` & `sciveo-0.1.9/test/test_sampling.py`

 * *Files identical despite different names*


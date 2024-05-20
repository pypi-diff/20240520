# Comparing `tmp/bridgecrew-3.2.96.tar.gz` & `tmp/bridgecrew-3.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bridgecrew-3.2.96.tar", last modified: Sun May 19 06:29:37 2024, max compression
+gzip compressed data, was "dist/bridgecrew-3.2.97.tar", last modified: Sun May 19 12:32:32 2024, max compression
```

## Comparing `bridgecrew-3.2.96.tar` & `bridgecrew-3.2.97.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/
--rw-r--r--   0 root         (0) root         (0)     1462 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      505 2024-02-06 13:10:24.000000 bridgecrew-3.2.96/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/bin/
--rwxr-xr-x   0 root         (0) root         (0)       93 2024-02-06 13:10:24.000000 bridgecrew-3.2.96/bin/bridgecrew
--rw-r--r--   0 root         (0) root         (0)     1368 2024-02-06 13:10:24.000000 bridgecrew-3.2.96/bin/bridgecrew.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/bridgecrew/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-06 13:10:24.000000 bridgecrew-3.2.96/bridgecrew/__init__.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-02-06 13:10:24.000000 bridgecrew-3.2.96/bridgecrew/banner.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-02-06 13:10:24.000000 bridgecrew-3.2.96/bridgecrew/main.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-19 06:29:34.000000 bridgecrew-3.2.96/bridgecrew/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/bridgecrew.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1462 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/bridgecrew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/bridgecrew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/bridgecrew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/bridgecrew.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/bridgecrew.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 06:29:37.000000 bridgecrew-3.2.96/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2024-02-06 13:10:24.000000 bridgecrew-3.2.96/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/
+-rw-r--r--   0 root         (0) root         (0)     1462 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      505 2024-01-22 12:14:48.000000 bridgecrew-3.2.97/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/bin/
+-rwxr-xr-x   0 root         (0) root         (0)       93 2024-01-22 12:14:48.000000 bridgecrew-3.2.97/bin/bridgecrew
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-01-22 12:14:48.000000 bridgecrew-3.2.97/bin/bridgecrew.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/bridgecrew/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-22 12:14:48.000000 bridgecrew-3.2.97/bridgecrew/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-01-22 12:14:48.000000 bridgecrew-3.2.97/bridgecrew/banner.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-01-22 12:14:48.000000 bridgecrew-3.2.97/bridgecrew/main.py
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-19 12:32:29.000000 bridgecrew-3.2.97/bridgecrew/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/bridgecrew.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1462 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/bridgecrew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/bridgecrew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/bridgecrew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/bridgecrew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/bridgecrew.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 12:32:32.000000 bridgecrew-3.2.97/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-01-22 12:14:48.000000 bridgecrew-3.2.97/setup.py
```

### Comparing `bridgecrew-3.2.96/PKG-INFO` & `bridgecrew-3.2.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 3.2.96
+Version: 3.2.97
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Description: # DEPRECATED: This project is no longer supported and will be archived end of 2023. Please use [checkov](https://github.com/bridgecrewio/checkov) instead.
```

### Comparing `bridgecrew-3.2.96/bin/bridgecrew.cmd` & `bridgecrew-3.2.97/bin/bridgecrew.cmd`

 * *Files identical despite different names*

### Comparing `bridgecrew-3.2.96/bridgecrew.egg-info/PKG-INFO` & `bridgecrew-3.2.97/bridgecrew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 3.2.96
+Version: 3.2.97
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Description: # DEPRECATED: This project is no longer supported and will be archived end of 2023. Please use [checkov](https://github.com/bridgecrewio/checkov) instead.
```

### Comparing `bridgecrew-3.2.96/setup.py` & `bridgecrew-3.2.97/setup.py`

 * *Files identical despite different names*


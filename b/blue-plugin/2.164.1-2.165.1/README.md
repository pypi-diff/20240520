# Comparing `tmp/blue_plugin-2.164.1.tar.gz` & `tmp/blue_plugin-2.165.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_plugin-2.164.1.tar", last modified: Sun May 19 22:45:23 2024, max compression
+gzip compressed data, was "blue_plugin-2.165.1.tar", last modified: Sun May 19 22:46:31 2024, max compression
```

## Comparing `blue_plugin-2.164.1.tar` & `blue_plugin-2.165.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:45:23.830794 blue_plugin-2.164.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-2.164.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)      161 2024-05-19 22:45:23.829905 blue_plugin-2.164.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      758 2024-03-31 23:20:44.000000 blue_plugin-2.164.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:45:23.824793 blue_plugin-2.164.1/blue_plugin/
--rw-r--r--   0 kamangir   (502) staff       (20)      123 2024-05-19 22:45:19.000000 blue_plugin-2.164.1/blue_plugin/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      878 2024-04-27 03:51:32.000000 blue_plugin-2.164.1/blue_plugin/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-2.164.1/blue_plugin/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-2.164.1/blue_plugin/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-2.164.1/blue_plugin/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-2.164.1/blue_plugin/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-2.164.1/blue_plugin/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:45:23.829172 blue_plugin-2.164.1/blue_plugin.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      161 2024-05-19 22:45:23.000000 blue_plugin-2.164.1/blue_plugin.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      323 2024-05-19 22:45:23.000000 blue_plugin-2.164.1/blue_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:45:23.000000 blue_plugin-2.164.1/blue_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-19 22:45:23.000000 blue_plugin-2.164.1/blue_plugin.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:45:23.831003 blue_plugin-2.164.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      266 2024-04-15 03:52:41.000000 blue_plugin-2.164.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:46:31.024019 blue_plugin-2.165.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-2.165.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)      960 2024-05-19 22:46:31.023340 blue_plugin-2.165.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      758 2024-03-31 23:20:44.000000 blue_plugin-2.165.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:46:31.021051 blue_plugin-2.165.1/blue_plugin/
+-rw-r--r--   0 kamangir   (502) staff       (20)      123 2024-05-19 22:46:26.000000 blue_plugin-2.165.1/blue_plugin/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      878 2024-04-27 03:51:32.000000 blue_plugin-2.165.1/blue_plugin/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-2.165.1/blue_plugin/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-2.165.1/blue_plugin/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-2.165.1/blue_plugin/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-2.165.1/blue_plugin/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-2.165.1/blue_plugin/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:46:31.022937 blue_plugin-2.165.1/blue_plugin.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)      960 2024-05-19 22:46:31.000000 blue_plugin-2.165.1/blue_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      323 2024-05-19 22:46:31.000000 blue_plugin-2.165.1/blue_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:46:31.000000 blue_plugin-2.165.1/blue_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-19 22:46:31.000000 blue_plugin-2.165.1/blue_plugin.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:46:31.024162 blue_plugin-2.165.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      568 2024-05-19 22:46:20.000000 blue_plugin-2.165.1/setup.py
```

### Comparing `blue_plugin-2.164.1/LICENSE` & `blue_plugin-2.165.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_plugin-2.164.1/README.md` & `blue_plugin-2.165.1/README.md`

 * *Files identical despite different names*

### Comparing `blue_plugin-2.164.1/blue_plugin/__main__.py` & `blue_plugin-2.165.1/blue_plugin/__main__.py`

 * *Files identical despite different names*


# Comparing `tmp/blue_plugin-2.167.1.tar.gz` & `tmp/blue_plugin-2.168.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_plugin-2.167.1.tar", last modified: Sun May 19 22:51:11 2024, max compression
+gzip compressed data, was "blue_plugin-2.168.1.tar", last modified: Sun May 19 22:59:02 2024, max compression
```

## Comparing `blue_plugin-2.167.1.tar` & `blue_plugin-2.168.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:51:11.933743 blue_plugin-2.167.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-2.167.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)      962 2024-05-19 22:51:11.931898 blue_plugin-2.167.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      754 2024-05-19 22:49:48.000000 blue_plugin-2.167.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:51:11.926956 blue_plugin-2.167.1/blue_plugin/
--rw-r--r--   0 kamangir   (502) staff       (20)      129 2024-05-19 22:51:06.000000 blue_plugin-2.167.1/blue_plugin/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      878 2024-04-27 03:51:32.000000 blue_plugin-2.167.1/blue_plugin/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-2.167.1/blue_plugin/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-2.167.1/blue_plugin/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-2.167.1/blue_plugin/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-2.167.1/blue_plugin/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-2.167.1/blue_plugin/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:51:11.930803 blue_plugin-2.167.1/blue_plugin.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      962 2024-05-19 22:51:11.000000 blue_plugin-2.167.1/blue_plugin.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      323 2024-05-19 22:51:11.000000 blue_plugin-2.167.1/blue_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:51:11.000000 blue_plugin-2.167.1/blue_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-19 22:51:11.000000 blue_plugin-2.167.1/blue_plugin.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:51:11.933999 blue_plugin-2.167.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      568 2024-05-19 22:46:20.000000 blue_plugin-2.167.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:59:02.943658 blue_plugin-2.168.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-2.168.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)      962 2024-05-19 22:59:02.943123 blue_plugin-2.168.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      754 2024-05-19 22:49:48.000000 blue_plugin-2.168.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:59:02.940411 blue_plugin-2.168.1/blue_plugin/
+-rw-r--r--   0 kamangir   (502) staff       (20)      129 2024-05-19 22:58:58.000000 blue_plugin-2.168.1/blue_plugin/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      878 2024-04-27 03:51:32.000000 blue_plugin-2.168.1/blue_plugin/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-2.168.1/blue_plugin/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-2.168.1/blue_plugin/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-2.168.1/blue_plugin/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-2.168.1/blue_plugin/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-2.168.1/blue_plugin/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-19 22:59:02.942529 blue_plugin-2.168.1/blue_plugin.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)      962 2024-05-19 22:59:02.000000 blue_plugin-2.168.1/blue_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      323 2024-05-19 22:59:02.000000 blue_plugin-2.168.1/blue_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-19 22:59:02.000000 blue_plugin-2.168.1/blue_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-19 22:59:02.000000 blue_plugin-2.168.1/blue_plugin.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-19 22:59:02.943739 blue_plugin-2.168.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      560 2024-05-19 22:57:48.000000 blue_plugin-2.168.1/setup.py
```

### Comparing `blue_plugin-2.167.1/LICENSE` & `blue_plugin-2.168.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_plugin-2.167.1/PKG-INFO` & `blue_plugin-2.168.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 2.167.1
+Version: 2.168.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🌀 blue-plugin
```

### Comparing `blue_plugin-2.167.1/README.md` & `blue_plugin-2.168.1/README.md`

 * *Files identical despite different names*

### Comparing `blue_plugin-2.167.1/blue_plugin/__main__.py` & `blue_plugin-2.168.1/blue_plugin/__main__.py`

 * *Files identical despite different names*

### Comparing `blue_plugin-2.167.1/blue_plugin.egg-info/PKG-INFO` & `blue_plugin-2.168.1/blue_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 2.167.1
+Version: 2.168.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Author: arash@kamangir.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🌀 blue-plugin
```

### Comparing `blue_plugin-2.167.1/setup.py` & `blue_plugin-2.168.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 from blue_plugin import NAME, VERSION, DESCRIPTION
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as f:
     long_description = f.read().replace(
         "./",
-        "https://github.com/kamangir/awesome-bash-cli/raw/current/",
+        "https://github.com/kamangir/blue-plugin/raw/main/",
     )
 
 
 setup(
     name=NAME,
     author="arash@kamangir.net",
     version=VERSION,
```


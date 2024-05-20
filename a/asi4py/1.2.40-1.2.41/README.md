# Comparing `tmp/asi4py-1.2.40.tar.gz` & `tmp/asi4py-1.2.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asi4py-1.2.40.tar", last modified: Wed Apr  3 16:33:11 2024, max compression
+gzip compressed data, was "asi4py-1.2.41.tar", last modified: Mon May 20 19:21:41 2024, max compression
```

## Comparing `asi4py-1.2.40.tar` & `asi4py-1.2.41.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:33:11.510376 asi4py-1.2.40/
--rw-rw-rw-   0 root         (0) root         (0)     1180 2022-07-19 20:58:13.000000 asi4py-1.2.40/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4498 2024-04-03 16:33:11.509376 asi4py-1.2.40/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2558 2022-07-19 20:58:13.000000 asi4py-1.2.40/README.md
--rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-03 16:32:37.000000 asi4py-1.2.40/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 16:33:11.510376 asi4py-1.2.40/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:33:11.507376 asi4py-1.2.40/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:33:11.508376 asi4py-1.2.40/src/asi4py/
--rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-23 22:51:32.000000 asi4py-1.2.40/src/asi4py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2568 2023-04-19 19:59:38.000000 asi4py-1.2.40/src/asi4py/asecalc.py
--rw-rw-rw-   0 root         (0) root         (0)    19321 2024-04-03 16:32:37.000000 asi4py-1.2.40/src/asi4py/pyasi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:33:11.509376 asi4py-1.2.40/src/asi4py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4498 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:21:41.290352 asi4py-1.2.41/
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2022-07-19 20:58:13.000000 asi4py-1.2.41/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4498 2024-05-20 19:21:41.290352 asi4py-1.2.41/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2022-07-19 20:58:13.000000 asi4py-1.2.41/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-05-16 15:50:14.000000 asi4py-1.2.41/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 19:21:41.290352 asi4py-1.2.41/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:21:41.288352 asi4py-1.2.41/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:21:41.289352 asi4py-1.2.41/src/asi4py/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-23 22:51:32.000000 asi4py-1.2.41/src/asi4py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2568 2023-04-19 19:59:38.000000 asi4py-1.2.41/src/asi4py/asecalc.py
+-rw-rw-rw-   0 root         (0) root         (0)    19321 2024-05-16 16:07:55.000000 asi4py-1.2.41/src/asi4py/pyasi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:21:41.290352 asi4py-1.2.41/src/asi4py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4498 2024-05-20 19:21:41.000000 asi4py-1.2.41/src/asi4py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2024-05-20 19:21:41.000000 asi4py-1.2.41/src/asi4py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 19:21:41.000000 asi4py-1.2.41/src/asi4py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-20 19:21:41.000000 asi4py-1.2.41/src/asi4py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-20 19:21:41.000000 asi4py-1.2.41/src/asi4py.egg-info/top_level.txt
```

### Comparing `asi4py-1.2.40/LICENSE` & `asi4py-1.2.41/LICENSE`

 * *Files identical despite different names*

### Comparing `asi4py-1.2.40/PKG-INFO` & `asi4py-1.2.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asi4py
-Version: 1.2.40
+Version: 1.2.41
 Summary: A Python wrapper for Atomic Simulation Interface API
 Author-email: Pavel Stishenko <pstishenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Pavel V Stishenko, Andrew Logsdail, Reinhard Maurer, 
         Volker Blum, Mariana Rossi, Ben Hourahine, Scott Woodley, Thomas Keal
```

### Comparing `asi4py-1.2.40/README.md` & `asi4py-1.2.41/README.md`

 * *Files identical despite different names*

### Comparing `asi4py-1.2.40/src/asi4py/asecalc.py` & `asi4py-1.2.41/src/asi4py/asecalc.py`

 * *Files identical despite different names*

### Comparing `asi4py-1.2.40/src/asi4py/pyasi.py` & `asi4py-1.2.41/src/asi4py/pyasi.py`

 * *Files identical despite different names*

### Comparing `asi4py-1.2.40/src/asi4py.egg-info/PKG-INFO` & `asi4py-1.2.41/src/asi4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asi4py
-Version: 1.2.40
+Version: 1.2.41
 Summary: A Python wrapper for Atomic Simulation Interface API
 Author-email: Pavel Stishenko <pstishenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Pavel V Stishenko, Andrew Logsdail, Reinhard Maurer, 
         Volker Blum, Mariana Rossi, Ben Hourahine, Scott Woodley, Thomas Keal
```


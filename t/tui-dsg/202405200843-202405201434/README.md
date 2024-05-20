# Comparing `tmp/tui_dsg-202405200843.tar.gz` & `tmp/tui_dsg-202405201434.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsg-202405200843.tar", last modified: Mon May 20 08:43:02 2024, max compression
+gzip compressed data, was "tui_dsg-202405201434.tar", last modified: Mon May 20 14:34:42 2024, max compression
```

## Comparing `tui_dsg-202405200843.tar` & `tui_dsg-202405201434.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 08:43:02.048732 tui_dsg-202405200843/
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-20 08:43:02.048732 tui_dsg-202405200843/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 08:43:02.048732 tui_dsg-202405200843/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1524 2024-05-20 08:27:37.000000 tui_dsg-202405200843/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 08:43:02.048732 tui_dsg-202405200843/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 08:43:02.048732 tui_dsg-202405200843/src/tui_dsg/
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-20 07:56:05.000000 tui_dsg-202405200843/src/tui_dsg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 08:43:02.048732 tui_dsg-202405200843/src/tui_dsg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-20 08:43:02.000000 tui_dsg-202405200843/src/tui_dsg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-20 08:43:02.000000 tui_dsg-202405200843/src/tui_dsg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 08:43:02.000000 tui_dsg-202405200843/src/tui_dsg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      348 2024-05-20 08:43:02.000000 tui_dsg-202405200843/src/tui_dsg.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-20 08:43:02.000000 tui_dsg-202405200843/src/tui_dsg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:34:42.102856 tui_dsg-202405201434/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-20 14:34:42.102856 tui_dsg-202405201434/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 14:34:42.102856 tui_dsg-202405201434/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1524 2024-05-20 14:34:34.000000 tui_dsg-202405201434/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:34:42.098856 tui_dsg-202405201434/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:34:42.098856 tui_dsg-202405201434/src/tui_dsg/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-20 07:56:05.000000 tui_dsg-202405201434/src/tui_dsg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:34:42.102856 tui_dsg-202405201434/src/tui_dsg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-20 14:34:42.000000 tui_dsg-202405201434/src/tui_dsg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-20 14:34:42.000000 tui_dsg-202405201434/src/tui_dsg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 14:34:42.000000 tui_dsg-202405201434/src/tui_dsg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      348 2024-05-20 14:34:42.000000 tui_dsg-202405201434/src/tui_dsg.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-20 14:34:42.000000 tui_dsg-202405201434/src/tui_dsg.egg-info/top_level.txt
```

### Comparing `tui_dsg-202405200843/PKG-INFO` & `tui_dsg-202405201434/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsg
-Version: 202405200843
+Version: 202405201434
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-grundlagen
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsg-202405200843/setup.py` & `tui_dsg-202405201434/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsg-202405200843/src/tui_dsg.egg-info/PKG-INFO` & `tui_dsg-202405201434/src/tui_dsg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsg
-Version: 202405200843
+Version: 202405201434
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-grundlagen
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/negar-gui-0.8.3.tar.gz` & `tmp/negar_gui-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negar-gui-0.8.3.tar", last modified: Fri Aug 18 17:06:21 2023, max compression
+gzip compressed data, was "negar_gui-0.8.4.tar", last modified: Mon May 20 20:53:43 2024, max compression
```

## Comparing `negar-gui-0.8.3.tar` & `negar_gui-0.8.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-18 17:06:21.789055 negar-gui-0.8.3/
--rw-r--r--   0 javad     (1000) javad     (1000)    35149 2023-04-01 17:16:18.000000 negar-gui-0.8.3/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      121 2023-04-01 17:16:18.000000 negar-gui-0.8.3/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     2899 2023-08-18 17:06:21.789055 negar-gui-0.8.3/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     2517 2023-08-15 09:20:21.000000 negar-gui-0.8.3/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-18 17:06:21.789055 negar-gui-0.8.3/negar_gui/
--rw-r--r--   0 javad     (1000) javad     (1000)     2280 2023-04-01 17:16:18.000000 negar-gui-0.8.3/negar_gui/Ui_hwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)    35703 2023-08-14 05:52:45.000000 negar-gui-0.8.3/negar_gui/Ui_mwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)     2960 2023-04-07 20:19:39.000000 negar-gui-0.8.3/negar_gui/Ui_uwin.py
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2023-04-01 17:16:18.000000 negar-gui-0.8.3/negar_gui/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)      379 2023-08-18 17:00:02.000000 negar-gui-0.8.3/negar_gui/constants.py
--rw-r--r--   0 javad     (1000) javad     (1000)    14828 2023-07-22 12:11:53.000000 negar-gui-0.8.3/negar_gui/gui.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-18 17:06:21.789055 negar-gui-0.8.3/negar_gui/icons/
--rw-r--r--   0 javad     (1000) javad     (1000)     1551 2023-04-01 17:20:04.000000 negar-gui-0.8.3/negar_gui/icons/logo.png
--rw-r--r--   0 javad     (1000) javad     (1000)    33240 2023-08-18 16:58:08.000000 negar-gui-0.8.3/negar_gui/main.py
--rw-r--r--   0 javad     (1000) javad     (1000)   301781 2023-08-16 02:44:05.000000 negar-gui-0.8.3/negar_gui/resource_rc.py
--rw-r--r--   0 javad     (1000) javad     (1000)     4938 2023-04-01 17:16:18.000000 negar-gui-0.8.3/negar_gui/style.qss
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-18 17:06:21.789055 negar-gui-0.8.3/negar_gui/ts/
--rw-r--r--   0 javad     (1000) javad     (1000)     5234 2023-04-01 17:20:04.000000 negar-gui-0.8.3/negar_gui/ts/fa.qm
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-08-18 17:06:21.789055 negar-gui-0.8.3/negar_gui.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     2899 2023-08-18 17:06:21.000000 negar-gui-0.8.3/negar_gui.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      470 2023-08-18 17:06:21.000000 negar-gui-0.8.3/negar_gui.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-08-18 17:06:21.000000 negar-gui-0.8.3/negar_gui.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       85 2023-08-18 17:06:21.000000 negar-gui-0.8.3/negar_gui.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       96 2023-08-18 17:06:21.000000 negar-gui-0.8.3/negar_gui.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       10 2023-08-18 17:06:21.000000 negar-gui-0.8.3/negar_gui.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-08-18 17:06:21.789055 negar-gui-0.8.3/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1188 2023-08-15 20:03:53.000000 negar-gui-0.8.3/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-20 20:53:43.467507 negar_gui-0.8.4/
+-rw-r--r--   0 javad     (1000) javad     (1000)    35149 2023-04-01 17:16:18.000000 negar_gui-0.8.4/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      121 2023-04-01 17:16:18.000000 negar_gui-0.8.4/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     3140 2024-05-20 20:53:43.467507 negar_gui-0.8.4/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     2517 2023-08-15 09:20:21.000000 negar_gui-0.8.4/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-20 20:53:43.467507 negar_gui-0.8.4/negar_gui/
+-rw-r--r--   0 javad     (1000) javad     (1000)     2280 2023-04-01 17:16:18.000000 negar_gui-0.8.4/negar_gui/Ui_hwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    35703 2023-08-14 05:52:45.000000 negar_gui-0.8.4/negar_gui/Ui_mwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     2960 2023-04-07 20:19:39.000000 negar_gui-0.8.4/negar_gui/Ui_uwin.py
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2023-04-01 17:16:18.000000 negar_gui-0.8.4/negar_gui/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)      379 2024-05-20 20:19:20.000000 negar_gui-0.8.4/negar_gui/constants.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    14828 2023-07-22 12:11:53.000000 negar_gui-0.8.4/negar_gui/gui.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-20 20:53:43.467507 negar_gui-0.8.4/negar_gui/icons/
+-rw-r--r--   0 javad     (1000) javad     (1000)     1551 2023-04-01 17:20:04.000000 negar_gui-0.8.4/negar_gui/icons/logo.png
+-rw-r--r--   0 javad     (1000) javad     (1000)    33332 2024-05-20 20:43:12.000000 negar_gui-0.8.4/negar_gui/main.py
+-rw-r--r--   0 javad     (1000) javad     (1000)   301781 2023-08-16 02:44:05.000000 negar_gui-0.8.4/negar_gui/resource_rc.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     4938 2023-04-01 17:16:18.000000 negar_gui-0.8.4/negar_gui/style.qss
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-20 20:53:43.467507 negar_gui-0.8.4/negar_gui/ts/
+-rw-r--r--   0 javad     (1000) javad     (1000)     5234 2023-04-01 17:20:04.000000 negar_gui-0.8.4/negar_gui/ts/fa.qm
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2024-05-20 20:53:43.467507 negar_gui-0.8.4/negar_gui.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     3140 2024-05-20 20:53:43.000000 negar_gui-0.8.4/negar_gui.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      470 2024-05-20 20:53:43.000000 negar_gui-0.8.4/negar_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2024-05-20 20:53:43.000000 negar_gui-0.8.4/negar_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       84 2024-05-20 20:53:43.000000 negar_gui-0.8.4/negar_gui.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       96 2024-05-20 20:53:43.000000 negar_gui-0.8.4/negar_gui.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       10 2024-05-20 20:53:43.000000 negar_gui-0.8.4/negar_gui.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2024-05-20 20:53:43.467507 negar_gui-0.8.4/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1188 2023-08-15 20:03:53.000000 negar_gui-0.8.4/setup.py
```

### Comparing `negar-gui-0.8.3/LICENSE` & `negar_gui-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/PKG-INFO` & `negar_gui-0.8.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: negar-gui
-Version: 0.8.3
-Summary: Graphical User Interface for Negar -- Persian Text Editor
-Home-page: http://github.com/javadr/negar-gui
-Author: Javad Razavian
-Author-email: javadr@gmail.com
-License: GPLv3
-Keywords: Spellcheck Persian Text-Editor
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ﻿Negar-GUI
 ==============
 [![PyPI](https://img.shields.io/pypi/v/negar-gui?style=social)](https://pypi.org/project/negar-gui/)
 [![code size](https://img.shields.io/github/languages/code-size/javadr/negar-gui?style=social)](https://github.com/javadr/negar-gui/archive/master.zip)
 [![GitHub forks](https://img.shields.io/github/forks/javadr/negar-gui?style=social)](https://github.com/javadr/negar-gui/network/members)
 [![GitHub license](https://img.shields.io/github/license/javadr/negar-gui?style=social)](https://github.com/javadr/negar-gui/blob/main/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/javadr/negar-gui?style=social)](https://github.com/javadr/negar-gui/stargazers)
@@ -78,9 +64,7 @@
 Just use one of the following in your terminal.
 
     $ negar-gui
 
 or simply
 
     $ negar
-
-
```

### Comparing `negar-gui-0.8.3/negar_gui/Ui_hwin.py` & `negar_gui-0.8.4/negar_gui/Ui_hwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/negar_gui/Ui_mwin.py` & `negar_gui-0.8.4/negar_gui/Ui_mwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/negar_gui/Ui_uwin.py` & `negar_gui-0.8.4/negar_gui/Ui_uwin.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/negar_gui/gui.py` & `negar_gui-0.8.4/negar_gui/gui.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/negar_gui/icons/logo.png` & `negar_gui-0.8.4/negar_gui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/negar_gui/main.py` & `negar_gui-0.8.4/negar_gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -770,15 +770,18 @@
 def main(args=docopt(__doc__)):
     """Program entry point."""
     if args["--version"]:
         print(f"negar-gui, Version {__version__}")
         sys.exit()
 
     global MAIN_WINDOW
-    qdarktheme.enable_hi_dpi()
+    try:
+        qdarktheme.enable_hi_dpi()
+    except AttributeError:
+        qdarktheme.setup_theme = lambda x, **kw: ()
     app = QApplication(sys.argv)
     qdarktheme.setup_theme("dark")
     MAIN_WINDOW = MyWindow()
     MAIN_WINDOW.show()
     sys.exit(app.exec_())
```

### Comparing `negar-gui-0.8.3/negar_gui/resource_rc.py` & `negar_gui-0.8.4/negar_gui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/negar_gui/style.qss` & `negar_gui-0.8.4/negar_gui/style.qss`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/negar_gui/ts/fa.qm` & `negar_gui-0.8.4/negar_gui/ts/fa.qm`

 * *Files identical despite different names*

### Comparing `negar-gui-0.8.3/setup.py` & `negar_gui-0.8.4/setup.py`

 * *Files identical despite different names*


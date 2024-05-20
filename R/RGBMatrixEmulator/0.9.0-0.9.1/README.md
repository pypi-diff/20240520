# Comparing `tmp/RGBMatrixEmulator-0.9.0.tar.gz` & `tmp/RGBMatrixEmulator-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RGBMatrixEmulator-0.9.0.tar", last modified: Sun Jun 11 21:36:37 2023, max compression
+gzip compressed data, was "dist\RGBMatrixEmulator-0.9.1.tar", last modified: Wed Jun 21 03:34:04 2023, max compression
```

## Comparing `RGBMatrixEmulator-0.9.0.tar` & `RGBMatrixEmulator-0.9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.554601 RGBMatrixEmulator-0.9.0/
--rw-rw-rw-   0        0        0     1076 2021-04-21 03:23:52.000000 RGBMatrixEmulator-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      370 2022-05-05 17:49:25.000000 RGBMatrixEmulator-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1733 2023-06-11 21:36:37.553600 RGBMatrixEmulator-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     7247 2023-06-11 21:34:14.000000 RGBMatrixEmulator-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.463599 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/
--rw-rw-rw-   0        0        0      219 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.502601 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/
--rw-rw-rw-   0        0        0     1895 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/__init__.py
--rw-rw-rw-   0        0        0     2491 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/base.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.508598 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/
--rw-rw-rw-   0        0        0        0 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/__init__.py
--rw-rw-rw-   0        0        0     2063 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/adapter.py
--rw-rw-rw-   0        0        0     2774 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/server.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.517595 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.541597 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/
--rw-rw-rw-   0        0        0     3812 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js
--rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico
--rw-rw-rw-   0        0        0      311 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/styles.css
--rw-rw-rw-   0        0        0     5068 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/index.html
--rw-rw-rw-   0        0        0      889 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py
--rw-rw-rw-   0        0        0     2547 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/pygame_adapter.py
--rw-rw-rw-   0        0        0     2859 2023-06-11 21:34:14.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/sixel_adapter.py
--rw-rw-rw-   0        0        0     1387 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/terminal_adapter.py
--rw-rw-rw-   0        0        0     2666 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/tkinter_adapter.py
--rw-rw-rw-   0        0        0     3150 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/turtle_adapter.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.547605 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/
--rw-rw-rw-   0        0        0        0 2021-04-24 19:55:28.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/__init__.py
--rw-rw-rw-   0        0        0     1806 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/canvas.py
--rw-rw-rw-   0        0        0     1449 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/matrix.py
--rw-rw-rw-   0        0        0     7244 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/options.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.551601 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/
--rw-rw-rw-   0        0        0     4460 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/__init__.py
--rw-rw-rw-   0        0        0      881 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/color.py
--rw-rw-rw-   0        0        0     1085 2022-05-05 19:55:29.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/font.py
--rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/icon.ico
--rw-rw-rw-   0        0        0     8514 2022-06-08 18:26:14.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/icon.png
--rw-rw-rw-   0        0        0      781 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/logger.py
--rw-rw-rw-   0        0        0      114 2023-06-11 21:34:28.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/version.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:36:37.490597 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/
--rw-rw-rw-   0        0        0     1733 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-11 21:36:37.000000 RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      760 2022-02-05 15:41:33.000000 RGBMatrixEmulator-0.9.0/description.md
--rw-rw-rw-   0        0        0       42 2023-06-11 21:36:37.554601 RGBMatrixEmulator-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2153 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.096392 RGBMatrixEmulator-0.9.1/
+-rw-rw-rw-   0        0        0     1076 2021-04-21 03:23:52.000000 RGBMatrixEmulator-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      370 2022-05-05 17:49:25.000000 RGBMatrixEmulator-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1733 2023-06-21 03:34:04.095389 RGBMatrixEmulator-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7247 2023-06-11 21:34:14.000000 RGBMatrixEmulator-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.014394 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/
+-rw-rw-rw-   0        0        0      219 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.046391 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/
+-rw-rw-rw-   0        0        0     1895 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/__init__.py
+-rw-rw-rw-   0        0        0     2491 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/base.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.053392 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/
+-rw-rw-rw-   0        0        0        0 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/__init__.py
+-rw-rw-rw-   0        0        0     2063 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/adapter.py
+-rw-rw-rw-   0        0        0     2774 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/server.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.055392 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/static/
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.080394 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/static/assets/
+-rw-rw-rw-   0        0        0     3114 2023-06-21 03:23:13.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/static/assets/client.js
+-rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico
+-rw-rw-rw-   0        0        0      311 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/static/assets/styles.css
+-rw-rw-rw-   0        0        0     5068 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/static/index.html
+-rw-rw-rw-   0        0        0      889 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py
+-rw-rw-rw-   0        0        0     2547 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/pygame_adapter.py
+-rw-rw-rw-   0        0        0     2859 2023-06-11 21:34:14.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/sixel_adapter.py
+-rw-rw-rw-   0        0        0     1387 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/terminal_adapter.py
+-rw-rw-rw-   0        0        0     2666 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/tkinter_adapter.py
+-rw-rw-rw-   0        0        0     3150 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/turtle_adapter.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.087394 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/emulators/
+-rw-rw-rw-   0        0        0        0 2021-04-24 19:55:28.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/emulators/__init__.py
+-rw-rw-rw-   0        0        0     1806 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/emulators/canvas.py
+-rw-rw-rw-   0        0        0     1449 2022-09-03 18:17:23.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/emulators/matrix.py
+-rw-rw-rw-   0        0        0     7244 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/emulators/options.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.093392 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/graphics/
+-rw-rw-rw-   0        0        0     4460 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/graphics/__init__.py
+-rw-rw-rw-   0        0        0      881 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/graphics/color.py
+-rw-rw-rw-   0        0        0     1085 2022-05-05 19:55:29.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/graphics/font.py
+-rw-rw-rw-   0        0        0     3426 2022-05-03 21:48:25.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/icon.ico
+-rw-rw-rw-   0        0        0     8514 2022-06-08 18:26:14.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/icon.png
+-rw-rw-rw-   0        0        0      781 2023-03-12 20:12:58.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/logger.py
+-rw-rw-rw-   0        0        0      114 2023-06-21 03:24:25.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/version.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:34:04.032389 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator.egg-info/
+-rw-rw-rw-   0        0        0     1733 2023-06-21 03:34:03.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-06-21 03:34:03.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:34:03.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-21 03:34:03.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-21 03:34:03.000000 RGBMatrixEmulator-0.9.1/RGBMatrixEmulator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      760 2022-02-05 15:41:33.000000 RGBMatrixEmulator-0.9.1/description.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:34:04.096392 RGBMatrixEmulator-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     2153 2023-06-11 21:33:56.000000 RGBMatrixEmulator-0.9.1/setup.py
```

### Comparing `RGBMatrixEmulator-0.9.0/LICENSE` & `RGBMatrixEmulator-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/PKG-INFO` & `RGBMatrixEmulator-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RGBMatrixEmulator
-Version: 0.9.0
+Version: 0.9.1
 Summary: A PC emulator for Raspberry Pi LED matrices driven by rpi-rgb-led-matrix
 Home-page: https://github.com/ty-porter/RGBMatrixEmulator
 Author: Tyler Porter
 Author-email: tyler.b.porter@gmail.com
 License: MIT
 Description: # `RGBMatrixEmulator`
```

### Comparing `RGBMatrixEmulator-0.9.0/README.md` & `RGBMatrixEmulator-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/__init__.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/base.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/base.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/adapter.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/server.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/server.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/static/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/static/index.html` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/static/index.html`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/browser_adapter/web_socket.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/pygame_adapter.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/pygame_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/sixel_adapter.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/sixel_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/terminal_adapter.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/terminal_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/tkinter_adapter.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/tkinter_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/adapters/turtle_adapter.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/adapters/turtle_adapter.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/canvas.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/emulators/canvas.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/matrix.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/emulators/matrix.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/emulators/options.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/emulators/options.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/__init__.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/color.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/graphics/color.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/graphics/font.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/graphics/font.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/icon.ico` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/icon.ico`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/icon.png` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/icon.png`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator/logger.py` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator/logger.py`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/PKG-INFO` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RGBMatrixEmulator
-Version: 0.9.0
+Version: 0.9.1
 Summary: A PC emulator for Raspberry Pi LED matrices driven by rpi-rgb-led-matrix
 Home-page: https://github.com/ty-porter/RGBMatrixEmulator
 Author: Tyler Porter
 Author-email: tyler.b.porter@gmail.com
 License: MIT
 Description: # `RGBMatrixEmulator`
```

### Comparing `RGBMatrixEmulator-0.9.0/RGBMatrixEmulator.egg-info/SOURCES.txt` & `RGBMatrixEmulator-0.9.1/RGBMatrixEmulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/description.md` & `RGBMatrixEmulator-0.9.1/description.md`

 * *Files identical despite different names*

### Comparing `RGBMatrixEmulator-0.9.0/setup.py` & `RGBMatrixEmulator-0.9.1/setup.py`

 * *Files identical despite different names*


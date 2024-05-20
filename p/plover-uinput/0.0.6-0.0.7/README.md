# Comparing `tmp/plover_uinput-0.0.6.tar.gz` & `tmp/plover_uinput-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover_uinput-0.0.6.tar", last modified: Mon May 20 16:59:44 2024, max compression
+gzip compressed data, was "plover_uinput-0.0.7.tar", last modified: Mon May 20 17:17:47 2024, max compression
```

## Comparing `plover_uinput-0.0.6.tar` & `plover_uinput-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:59:44.507330 plover_uinput-0.0.6/
--rw-r--r--   0 olai      (1000) users      (100)     1053 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/LICENSE
--rw-r--r--   0 olai      (1000) users      (100)     2458 2024-05-20 16:59:44.507330 plover_uinput-0.0.6/PKG-INFO
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:59:44.506330 plover_uinput-0.0.6/plover_uinput/
--rw-r--r--   0 olai      (1000) users      (100)     9545 2024-05-20 16:59:18.000000 plover_uinput-0.0.6/plover_uinput/__init__.py
--rw-r--r--   0 olai      (1000) users      (100)      130 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/plover_uinput/all_keys.py
--rw-r--r--   0 olai      (1000) users      (100)    10000 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/plover_uinput/keys.py
--rw-r--r--   0 olai      (1000) users      (100)     2019 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/plover_uinput/symbols.py
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:59:44.507330 plover_uinput-0.0.6/plover_uinput.egg-info/
--rw-r--r--   0 olai      (1000) users      (100)     2458 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/PKG-INFO
--rw-r--r--   0 olai      (1000) users      (100)      374 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/SOURCES.txt
--rw-r--r--   0 olai      (1000) users      (100)        1 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/dependency_links.txt
--rw-r--r--   0 olai      (1000) users      (100)      119 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/entry_points.txt
--rw-r--r--   0 olai      (1000) users      (100)       45 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/requires.txt
--rw-r--r--   0 olai      (1000) users      (100)       14 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/top_level.txt
--rw-r--r--   0 olai      (1000) users      (100)       89 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/pyproject.toml
--rw-r--r--   0 olai      (1000) users      (100)      993 2024-05-20 16:58:01.000000 plover_uinput-0.0.6/readme.md
--rw-r--r--   0 olai      (1000) users      (100)      670 2024-05-20 16:59:44.508330 plover_uinput-0.0.6/setup.cfg
--rw-r--r--   0 olai      (1000) users      (100)       62 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/setup.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 17:17:47.404507 plover_uinput-0.0.7/
+-rw-r--r--   0 olai      (1000) users      (100)     1053 2024-05-20 16:28:07.000000 plover_uinput-0.0.7/LICENSE
+-rw-r--r--   0 olai      (1000) users      (100)     2458 2024-05-20 17:17:47.404507 plover_uinput-0.0.7/PKG-INFO
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 17:17:47.403507 plover_uinput-0.0.7/plover_uinput/
+-rw-r--r--   0 olai      (1000) users      (100)     9545 2024-05-20 17:17:21.000000 plover_uinput-0.0.7/plover_uinput/__init__.py
+-rw-r--r--   0 olai      (1000) users      (100)      130 2024-05-20 16:28:07.000000 plover_uinput-0.0.7/plover_uinput/all_keys.py
+-rw-r--r--   0 olai      (1000) users      (100)    10000 2024-05-20 16:28:07.000000 plover_uinput-0.0.7/plover_uinput/keys.py
+-rw-r--r--   0 olai      (1000) users      (100)     2019 2024-05-20 16:28:07.000000 plover_uinput-0.0.7/plover_uinput/symbols.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 17:17:47.404507 plover_uinput-0.0.7/plover_uinput.egg-info/
+-rw-r--r--   0 olai      (1000) users      (100)     2458 2024-05-20 17:17:47.000000 plover_uinput-0.0.7/plover_uinput.egg-info/PKG-INFO
+-rw-r--r--   0 olai      (1000) users      (100)      374 2024-05-20 17:17:47.000000 plover_uinput-0.0.7/plover_uinput.egg-info/SOURCES.txt
+-rw-r--r--   0 olai      (1000) users      (100)        1 2024-05-20 17:17:47.000000 plover_uinput-0.0.7/plover_uinput.egg-info/dependency_links.txt
+-rw-r--r--   0 olai      (1000) users      (100)      119 2024-05-20 17:17:47.000000 plover_uinput-0.0.7/plover_uinput.egg-info/entry_points.txt
+-rw-r--r--   0 olai      (1000) users      (100)       45 2024-05-20 17:17:47.000000 plover_uinput-0.0.7/plover_uinput.egg-info/requires.txt
+-rw-r--r--   0 olai      (1000) users      (100)       14 2024-05-20 17:17:47.000000 plover_uinput-0.0.7/plover_uinput.egg-info/top_level.txt
+-rw-r--r--   0 olai      (1000) users      (100)       89 2024-05-20 16:28:07.000000 plover_uinput-0.0.7/pyproject.toml
+-rw-r--r--   0 olai      (1000) users      (100)      993 2024-05-20 16:58:01.000000 plover_uinput-0.0.7/readme.md
+-rw-r--r--   0 olai      (1000) users      (100)      670 2024-05-20 17:17:47.404507 plover_uinput-0.0.7/setup.cfg
+-rw-r--r--   0 olai      (1000) users      (100)       62 2024-05-20 16:28:07.000000 plover_uinput-0.0.7/setup.py
```

### Comparing `plover_uinput-0.0.6/LICENSE` & `plover_uinput-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.6/PKG-INFO` & `plover_uinput-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.6
+Version: 0.0.7
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `plover_uinput-0.0.6/plover_uinput/__init__.py` & `plover_uinput-0.0.7/plover_uinput/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,20 +236,20 @@
         self._press_key(key, True)
         self._press_key(key, False)
         self._ui.syn()
 
     # Send unicode character (through iBus)
     def _send_unicode(self, hex):
         self._press_key(modifiers["control_l"], True)
-        self._press_key(modifiers["shift_l"], False)
+        self._press_key(modifiers["shift_r"], False)
         sleep(self._delay)
         self._send_key(keys["u"])
         sleep(self._delay)
         self._press_key(modifiers["control_l"], False)
-        self._press_key(modifiers["shift_l"], False)
+        self._press_key(modifiers["shift_r"], False)
         sleep(self._delay)
         self.send_string(hex)
         sleep(self._delay)
         self._send_key(keys["\n"])
 
     def _send_char(self, char):
         # === Key can be sent with a key combination ===
```

### Comparing `plover_uinput-0.0.6/plover_uinput/keys.py` & `plover_uinput-0.0.7/plover_uinput/keys.py`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.6/plover_uinput/symbols.py` & `plover_uinput-0.0.7/plover_uinput/symbols.py`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.6/plover_uinput.egg-info/PKG-INFO` & `plover_uinput-0.0.7/plover_uinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.6
+Version: 0.0.7
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `plover_uinput-0.0.6/readme.md` & `plover_uinput-0.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.6/setup.cfg` & `plover_uinput-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-uinput
-version = 0.0.6
+version = 0.0.7
 author = LilleAila
 description = Plover output plugin for linux using evdev / uinput
 long_description = file: readme.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/LilleAila/plover-uinput
 keywords = plover plover_plugin
```


# Comparing `tmp/plover-uinput-0.0.4.tar.gz` & `tmp/plover_uinput-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-uinput-0.0.4.tar", last modified: Sun Apr 28 13:54:15 2024, max compression
+gzip compressed data, was "plover_uinput-0.0.5.tar", last modified: Mon May 20 16:29:02 2024, max compression
```

## Comparing `plover-uinput-0.0.4.tar` & `plover_uinput-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-28 13:54:15.346328 plover-uinput-0.0.4/
--rw-r--r--   0 olai      (1000) users      (100)     1053 2024-04-11 16:08:24.000000 plover-uinput-0.0.4/LICENSE
--rw-r--r--   0 olai      (1000) users      (100)     2208 2024-04-28 13:54:15.346328 plover-uinput-0.0.4/PKG-INFO
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-28 13:54:15.345328 plover-uinput-0.0.4/plover_uinput/
--rw-r--r--   0 olai      (1000) users      (100)     9403 2024-04-28 13:53:32.000000 plover-uinput-0.0.4/plover_uinput/__init__.py
--rw-r--r--   0 olai      (1000) users      (100)      130 2024-04-09 10:35:53.000000 plover-uinput-0.0.4/plover_uinput/all_keys.py
--rw-r--r--   0 olai      (1000) users      (100)    10000 2024-04-09 10:31:51.000000 plover-uinput-0.0.4/plover_uinput/keys.py
--rw-r--r--   0 olai      (1000) users      (100)     2019 2024-04-11 13:38:12.000000 plover-uinput-0.0.4/plover_uinput/symbols.py
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-28 13:54:15.346328 plover-uinput-0.0.4/plover_uinput.egg-info/
--rw-r--r--   0 olai      (1000) users      (100)     2208 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/PKG-INFO
--rw-r--r--   0 olai      (1000) users      (100)      374 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/SOURCES.txt
--rw-r--r--   0 olai      (1000) users      (100)        1 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/dependency_links.txt
--rw-r--r--   0 olai      (1000) users      (100)      119 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/entry_points.txt
--rw-r--r--   0 olai      (1000) users      (100)       45 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/requires.txt
--rw-r--r--   0 olai      (1000) users      (100)       14 2024-04-28 13:54:15.000000 plover-uinput-0.0.4/plover_uinput.egg-info/top_level.txt
--rw-r--r--   0 olai      (1000) users      (100)       89 2024-04-11 16:18:33.000000 plover-uinput-0.0.4/pyproject.toml
--rw-r--r--   0 olai      (1000) users      (100)      743 2024-04-16 14:42:09.000000 plover-uinput-0.0.4/readme.md
--rw-r--r--   0 olai      (1000) users      (100)      670 2024-04-28 13:54:15.346328 plover-uinput-0.0.4/setup.cfg
--rw-r--r--   0 olai      (1000) users      (100)       62 2024-04-09 17:27:40.000000 plover-uinput-0.0.4/setup.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:29:02.150649 plover_uinput-0.0.5/
+-rw-r--r--   0 olai      (1000) users      (100)     1053 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/LICENSE
+-rw-r--r--   0 olai      (1000) users      (100)     2208 2024-05-20 16:29:02.150649 plover_uinput-0.0.5/PKG-INFO
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:29:02.149649 plover_uinput-0.0.5/plover_uinput/
+-rw-r--r--   0 olai      (1000) users      (100)     9402 2024-05-20 16:28:48.000000 plover_uinput-0.0.5/plover_uinput/__init__.py
+-rw-r--r--   0 olai      (1000) users      (100)      130 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/plover_uinput/all_keys.py
+-rw-r--r--   0 olai      (1000) users      (100)    10000 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/plover_uinput/keys.py
+-rw-r--r--   0 olai      (1000) users      (100)     2019 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/plover_uinput/symbols.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:29:02.150649 plover_uinput-0.0.5/plover_uinput.egg-info/
+-rw-r--r--   0 olai      (1000) users      (100)     2208 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/PKG-INFO
+-rw-r--r--   0 olai      (1000) users      (100)      374 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/SOURCES.txt
+-rw-r--r--   0 olai      (1000) users      (100)        1 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/dependency_links.txt
+-rw-r--r--   0 olai      (1000) users      (100)      119 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/entry_points.txt
+-rw-r--r--   0 olai      (1000) users      (100)       45 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/requires.txt
+-rw-r--r--   0 olai      (1000) users      (100)       14 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/top_level.txt
+-rw-r--r--   0 olai      (1000) users      (100)       89 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/pyproject.toml
+-rw-r--r--   0 olai      (1000) users      (100)      743 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/readme.md
+-rw-r--r--   0 olai      (1000) users      (100)      670 2024-05-20 16:29:02.151649 plover_uinput-0.0.5/setup.cfg
+-rw-r--r--   0 olai      (1000) users      (100)       62 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/setup.py
```

### Comparing `plover-uinput-0.0.4/LICENSE` & `plover_uinput-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.4/PKG-INFO` & `plover_uinput-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.4
+Version: 0.0.5
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `plover-uinput-0.0.4/plover_uinput/__init__.py` & `plover_uinput-0.0.5/plover_uinput/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         self._press_key(modifiers["shift_l"], False)
         sleep(self._delay)
         self._send_key(keys["u"])
         sleep(self._delay)
         self._press_key(modifiers["control_l"], False)
         self._press_key(modifiers["shift_l"], False)
         sleep(self._delay)
-        self._send_string(hex)
+        self.send_string(hex)
         self._send_key(keys["\n"])
 
     def _send_char(self, char):
         # === Key can be sent with a key combination ===
         if char in self._symbols:
             (base, mods) = self._symbols[char]
             for mod in mods.split():
```

### Comparing `plover-uinput-0.0.4/plover_uinput/keys.py` & `plover_uinput-0.0.5/plover_uinput/keys.py`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.4/plover_uinput/symbols.py` & `plover_uinput-0.0.5/plover_uinput/symbols.py`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.4/plover_uinput.egg-info/PKG-INFO` & `plover_uinput-0.0.5/plover_uinput.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.4
+Version: 0.0.5
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `plover-uinput-0.0.4/readme.md` & `plover_uinput-0.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.4/setup.cfg` & `plover_uinput-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-uinput
-version = 0.0.4
+version = 0.0.5
 author = LilleAila
 description = Plover output plugin for linux using evdev / uinput
 long_description = file: readme.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/LilleAila/plover-uinput
 keywords = plover plover_plugin
```


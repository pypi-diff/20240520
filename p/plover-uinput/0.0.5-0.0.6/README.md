# Comparing `tmp/plover_uinput-0.0.5.tar.gz` & `tmp/plover_uinput-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover_uinput-0.0.5.tar", last modified: Mon May 20 16:29:02 2024, max compression
+gzip compressed data, was "plover_uinput-0.0.6.tar", last modified: Mon May 20 16:59:44 2024, max compression
```

## Comparing `plover_uinput-0.0.5.tar` & `plover_uinput-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:29:02.150649 plover_uinput-0.0.5/
--rw-r--r--   0 olai      (1000) users      (100)     1053 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/LICENSE
--rw-r--r--   0 olai      (1000) users      (100)     2208 2024-05-20 16:29:02.150649 plover_uinput-0.0.5/PKG-INFO
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:29:02.149649 plover_uinput-0.0.5/plover_uinput/
--rw-r--r--   0 olai      (1000) users      (100)     9402 2024-05-20 16:28:48.000000 plover_uinput-0.0.5/plover_uinput/__init__.py
--rw-r--r--   0 olai      (1000) users      (100)      130 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/plover_uinput/all_keys.py
--rw-r--r--   0 olai      (1000) users      (100)    10000 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/plover_uinput/keys.py
--rw-r--r--   0 olai      (1000) users      (100)     2019 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/plover_uinput/symbols.py
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:29:02.150649 plover_uinput-0.0.5/plover_uinput.egg-info/
--rw-r--r--   0 olai      (1000) users      (100)     2208 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/PKG-INFO
--rw-r--r--   0 olai      (1000) users      (100)      374 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/SOURCES.txt
--rw-r--r--   0 olai      (1000) users      (100)        1 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/dependency_links.txt
--rw-r--r--   0 olai      (1000) users      (100)      119 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/entry_points.txt
--rw-r--r--   0 olai      (1000) users      (100)       45 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/requires.txt
--rw-r--r--   0 olai      (1000) users      (100)       14 2024-05-20 16:29:02.000000 plover_uinput-0.0.5/plover_uinput.egg-info/top_level.txt
--rw-r--r--   0 olai      (1000) users      (100)       89 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/pyproject.toml
--rw-r--r--   0 olai      (1000) users      (100)      743 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/readme.md
--rw-r--r--   0 olai      (1000) users      (100)      670 2024-05-20 16:29:02.151649 plover_uinput-0.0.5/setup.cfg
--rw-r--r--   0 olai      (1000) users      (100)       62 2024-05-20 16:28:07.000000 plover_uinput-0.0.5/setup.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:59:44.507330 plover_uinput-0.0.6/
+-rw-r--r--   0 olai      (1000) users      (100)     1053 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/LICENSE
+-rw-r--r--   0 olai      (1000) users      (100)     2458 2024-05-20 16:59:44.507330 plover_uinput-0.0.6/PKG-INFO
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:59:44.506330 plover_uinput-0.0.6/plover_uinput/
+-rw-r--r--   0 olai      (1000) users      (100)     9545 2024-05-20 16:59:18.000000 plover_uinput-0.0.6/plover_uinput/__init__.py
+-rw-r--r--   0 olai      (1000) users      (100)      130 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/plover_uinput/all_keys.py
+-rw-r--r--   0 olai      (1000) users      (100)    10000 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/plover_uinput/keys.py
+-rw-r--r--   0 olai      (1000) users      (100)     2019 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/plover_uinput/symbols.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 16:59:44.507330 plover_uinput-0.0.6/plover_uinput.egg-info/
+-rw-r--r--   0 olai      (1000) users      (100)     2458 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/PKG-INFO
+-rw-r--r--   0 olai      (1000) users      (100)      374 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/SOURCES.txt
+-rw-r--r--   0 olai      (1000) users      (100)        1 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/dependency_links.txt
+-rw-r--r--   0 olai      (1000) users      (100)      119 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/entry_points.txt
+-rw-r--r--   0 olai      (1000) users      (100)       45 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/requires.txt
+-rw-r--r--   0 olai      (1000) users      (100)       14 2024-05-20 16:59:44.000000 plover_uinput-0.0.6/plover_uinput.egg-info/top_level.txt
+-rw-r--r--   0 olai      (1000) users      (100)       89 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/pyproject.toml
+-rw-r--r--   0 olai      (1000) users      (100)      993 2024-05-20 16:58:01.000000 plover_uinput-0.0.6/readme.md
+-rw-r--r--   0 olai      (1000) users      (100)      670 2024-05-20 16:59:44.508330 plover_uinput-0.0.6/setup.cfg
+-rw-r--r--   0 olai      (1000) users      (100)       62 2024-05-20 16:28:07.000000 plover_uinput-0.0.6/setup.py
```

### Comparing `plover_uinput-0.0.5/LICENSE` & `plover_uinput-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.5/PKG-INFO` & `plover_uinput-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.5
+Version: 0.0.6
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plover>=4.0.0rc2
 Requires-Dist: evdev>=1.7.0
 Requires-Dist: xkbcommon>=0.8
 
 # Plover output plugin for linux using uinput
 
-If you experience any problems, feel free to open an issue, pull request or send a message on discord (`lilleaila`)!
+If you experience any problems, feel free to open an issue, pull request or send a message on discord (`lilleaila`)! Before asking for help, please check if the plugin is enabled in the settings..
 
 ## Setup
 Add your user to the `input` group, and add this `udev` rule:
 ```
 KERNEL=="uinput", GROUP="input", MODE="0660", OPTIONS+="static_node=uinput"
 ```
-Set the `PLOVER_UINPUT_LAYOUT` environment variable to your two-letter `xkb` keyboard layout, for example `us`, `no` or `fr`.
+Set the `PLOVER_UINPUT_LAYOUT` environment variable to your two-letter `xkb` keyboard layout, for example `us`, `no` or `fr`. This is not necessary if you're using a US keyboard.
 
 ## Unicode characters
-If you want to use unicode characters, `iBus` has to be installed.
+If you want to use unicode characters, either `iBus` or `fcitx5` has to be installed. You should also increase the key press delay in plover if some characters do not output properly.
 
 ## Inspired by:
 - [halbGefressen/plover-output-dotool](https://github.com/halbGefressen/plover-output-dotool)
 - [svenkeidel/plover-wtype-output](https://github.com/svenkeidel/plover-wtype-output/tree/main)
 
 Copyright (c) 2024 LilleAila
```

### Comparing `plover_uinput-0.0.5/plover_uinput/__init__.py` & `plover_uinput-0.0.6/plover_uinput/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,24 @@
 except ImportError:
     pass
 
 
 modifiers = {
     "alt_l": e.KEY_LEFTALT,
     "alt_r": e.KEY_RIGHTALT,
+    "alt": e.KEY_LEFTALT,
     "control_l": e.KEY_LEFTCTRL,
     "control_r": e.KEY_RIGHTCTRL,
+    "control": e.KEY_LEFTCTRL,
     "shift_l": e.KEY_LEFTSHIFT,
     "shift_r": e.KEY_RIGHTSHIFT,
+    "shift": e.KEY_LEFTSHIFT,
     "super_l": e.KEY_LEFTMETA,
     "super_r": e.KEY_RIGHTMETA,
+    "super": e.KEY_LEFTMETA,
 }
 
 
 keys = {
     # Lowercase
     "a": e.KEY_A,
     "b": e.KEY_B,
@@ -240,14 +244,15 @@
         sleep(self._delay)
         self._send_key(keys["u"])
         sleep(self._delay)
         self._press_key(modifiers["control_l"], False)
         self._press_key(modifiers["shift_l"], False)
         sleep(self._delay)
         self.send_string(hex)
+        sleep(self._delay)
         self._send_key(keys["\n"])
 
     def _send_char(self, char):
         # === Key can be sent with a key combination ===
         if char in self._symbols:
             (base, mods) = self._symbols[char]
             for mod in mods.split():
```

### Comparing `plover_uinput-0.0.5/plover_uinput/keys.py` & `plover_uinput-0.0.6/plover_uinput/keys.py`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.5/plover_uinput/symbols.py` & `plover_uinput-0.0.6/plover_uinput/symbols.py`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.5/plover_uinput.egg-info/PKG-INFO` & `plover_uinput-0.0.6/plover_uinput.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.5
+Version: 0.0.6
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plover>=4.0.0rc2
 Requires-Dist: evdev>=1.7.0
 Requires-Dist: xkbcommon>=0.8
 
 # Plover output plugin for linux using uinput
 
-If you experience any problems, feel free to open an issue, pull request or send a message on discord (`lilleaila`)!
+If you experience any problems, feel free to open an issue, pull request or send a message on discord (`lilleaila`)! Before asking for help, please check if the plugin is enabled in the settings..
 
 ## Setup
 Add your user to the `input` group, and add this `udev` rule:
 ```
 KERNEL=="uinput", GROUP="input", MODE="0660", OPTIONS+="static_node=uinput"
 ```
-Set the `PLOVER_UINPUT_LAYOUT` environment variable to your two-letter `xkb` keyboard layout, for example `us`, `no` or `fr`.
+Set the `PLOVER_UINPUT_LAYOUT` environment variable to your two-letter `xkb` keyboard layout, for example `us`, `no` or `fr`. This is not necessary if you're using a US keyboard.
 
 ## Unicode characters
-If you want to use unicode characters, `iBus` has to be installed.
+If you want to use unicode characters, either `iBus` or `fcitx5` has to be installed. You should also increase the key press delay in plover if some characters do not output properly.
 
 ## Inspired by:
 - [halbGefressen/plover-output-dotool](https://github.com/halbGefressen/plover-output-dotool)
 - [svenkeidel/plover-wtype-output](https://github.com/svenkeidel/plover-wtype-output/tree/main)
 
 Copyright (c) 2024 LilleAila
```

### Comparing `plover_uinput-0.0.5/readme.md` & `plover_uinput-0.0.6/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Plover output plugin for linux using uinput
 
-If you experience any problems, feel free to open an issue, pull request or send a message on discord (`lilleaila`)!
+If you experience any problems, feel free to open an issue, pull request or send a message on discord (`lilleaila`)! Before asking for help, please check if the plugin is enabled in the settings..
 
 ## Setup
 Add your user to the `input` group, and add this `udev` rule:
 ```
 KERNEL=="uinput", GROUP="input", MODE="0660", OPTIONS+="static_node=uinput"
 ```
-Set the `PLOVER_UINPUT_LAYOUT` environment variable to your two-letter `xkb` keyboard layout, for example `us`, `no` or `fr`.
+Set the `PLOVER_UINPUT_LAYOUT` environment variable to your two-letter `xkb` keyboard layout, for example `us`, `no` or `fr`. This is not necessary if you're using a US keyboard.
 
 ## Unicode characters
-If you want to use unicode characters, `iBus` has to be installed.
+If you want to use unicode characters, either `iBus` or `fcitx5` has to be installed. You should also increase the key press delay in plover if some characters do not output properly.
 
 ## Inspired by:
 - [halbGefressen/plover-output-dotool](https://github.com/halbGefressen/plover-output-dotool)
 - [svenkeidel/plover-wtype-output](https://github.com/svenkeidel/plover-wtype-output/tree/main)
```

### Comparing `plover_uinput-0.0.5/setup.cfg` & `plover_uinput-0.0.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-uinput
-version = 0.0.5
+version = 0.0.6
 author = LilleAila
 description = Plover output plugin for linux using evdev / uinput
 long_description = file: readme.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/LilleAila/plover-uinput
 keywords = plover plover_plugin
```


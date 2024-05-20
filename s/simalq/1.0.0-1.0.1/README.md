# Comparing `tmp/simalq-1.0.0.tar.gz` & `tmp/simalq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simalq-1.0.0.tar", last modified: Fri Mar  1 21:59:16 2024, max compression
+gzip compressed data, was "simalq-1.0.1.tar", last modified: Mon May 20 21:33:25 2024, max compression
```

## Comparing `simalq-1.0.0.tar` & `simalq-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-03-01 21:59:16.489664 simalq-1.0.0/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    10161 2024-03-01 21:59:16.489664 simalq-1.0.0/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     9653 2024-03-01 21:44:13.000000 simalq-1.0.0/README.rst
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2024-03-01 21:59:16.489664 simalq-1.0.0/setup.cfg
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1091 2024-03-01 21:57:09.000000 simalq-1.0.0/setup.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-03-01 21:59:16.489664 simalq-1.0.0/simalq/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      103 2024-03-01 21:57:09.000000 simalq-1.0.0/simalq/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       76 2024-02-23 19:30:05.000000 simalq-1.0.0/simalq/__main__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4345 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/cmdline.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1563 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/color.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    12374 2024-02-28 19:24:39.000000 simalq-1.0.0/simalq/commands.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    13106 2024-03-01 20:21:12.000000 simalq-1.0.0/simalq/display.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     6902 2024-02-28 20:26:10.000000 simalq-1.0.0/simalq/game_state.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     8171 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/geometry.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      905 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/keyboard.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     6708 2024-02-28 20:26:10.000000 simalq-1.0.0/simalq/macros.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    10855 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/main.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2742 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/quest.hy
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-03-01 21:59:16.489664 simalq-1.0.0/simalq/quest_definition/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5581 2024-02-28 19:12:49.000000 simalq-1.0.0/simalq/quest_definition/__init__.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    20149 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/quest_definition/tutorial.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3926 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/save_load.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5140 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/strings.hy
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-03-01 21:59:16.489664 simalq-1.0.0/simalq/tile/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    16736 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/tile/__init__.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    26215 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/tile/item.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    32915 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/tile/monster.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3510 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/tile/player.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    36650 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/tile/scenery.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3930 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/tile/tilepedia.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1137 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/tile/unimplemented.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    13485 2024-02-28 02:37:18.000000 simalq-1.0.0/simalq/un_iq.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5892 2024-02-28 19:24:39.000000 simalq-1.0.0/simalq/util.hy
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-03-01 21:59:16.489664 simalq-1.0.0/simalq.egg-info/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    10161 2024-03-01 21:59:16.000000 simalq-1.0.0/simalq.egg-info/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      709 2024-03-01 21:59:16.000000 simalq-1.0.0/simalq.egg-info/SOURCES.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2024-03-01 21:59:16.000000 simalq-1.0.0/simalq.egg-info/dependency_links.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      110 2024-03-01 21:59:16.000000 simalq-1.0.0/simalq.egg-info/requires.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       13 2024-03-01 21:59:16.000000 simalq-1.0.0/simalq.egg-info/top_level.txt
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-03-01 21:59:16.489664 simalq-1.0.0/tests/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2024-02-23 19:30:05.000000 simalq-1.0.0/tests/__init__.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 21:33:25.341440 simalq-1.0.1/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    10394 2024-05-20 21:33:25.341440 simalq-1.0.1/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     9847 2024-05-20 21:33:14.000000 simalq-1.0.1/README.rst
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2024-05-20 21:33:25.341440 simalq-1.0.1/setup.cfg
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1129 2024-05-20 21:33:14.000000 simalq-1.0.1/setup.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 21:33:25.337440 simalq-1.0.1/simalq/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      103 2024-05-20 21:33:14.000000 simalq-1.0.1/simalq/__init__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       76 2024-02-23 19:30:05.000000 simalq-1.0.1/simalq/__main__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4345 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/cmdline.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1563 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/color.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    12374 2024-05-01 14:10:18.000000 simalq-1.0.1/simalq/commands.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    13106 2024-03-21 18:43:57.000000 simalq-1.0.1/simalq/display.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     6902 2024-02-28 20:26:10.000000 simalq-1.0.1/simalq/game_state.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     8172 2024-03-21 18:43:57.000000 simalq-1.0.1/simalq/geometry.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      905 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/keyboard.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3265 2024-03-21 18:43:57.000000 simalq-1.0.1/simalq/macros.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    10855 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/main.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2742 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/quest.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 21:33:25.337440 simalq-1.0.1/simalq/quest_definition/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     5546 2024-05-20 20:38:19.000000 simalq-1.0.1/simalq/quest_definition/__init__.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    20130 2024-03-21 18:43:57.000000 simalq-1.0.1/simalq/quest_definition/tutorial.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3926 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/save_load.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     5178 2024-03-21 18:43:57.000000 simalq-1.0.1/simalq/strings.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 21:33:25.341440 simalq-1.0.1/simalq/tile/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    16736 2024-03-21 18:43:57.000000 simalq-1.0.1/simalq/tile/__init__.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    26215 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/tile/item.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    32932 2024-03-22 15:47:36.000000 simalq-1.0.1/simalq/tile/monster.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3510 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/tile/player.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    36650 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/tile/scenery.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3916 2024-03-22 15:45:46.000000 simalq-1.0.1/simalq/tile/tilepedia.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1137 2024-02-28 02:37:18.000000 simalq-1.0.1/simalq/tile/unimplemented.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    13347 2024-03-21 18:43:57.000000 simalq-1.0.1/simalq/un_iq.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     5577 2024-03-21 18:43:57.000000 simalq-1.0.1/simalq/util.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 21:33:25.337440 simalq-1.0.1/simalq.egg-info/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    10394 2024-05-20 21:33:25.000000 simalq-1.0.1/simalq.egg-info/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      709 2024-05-20 21:33:25.000000 simalq-1.0.1/simalq.egg-info/SOURCES.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2024-05-20 21:33:25.000000 simalq-1.0.1/simalq.egg-info/dependency_links.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      110 2024-05-20 21:33:25.000000 simalq-1.0.1/simalq.egg-info/requires.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       13 2024-05-20 21:33:25.000000 simalq-1.0.1/simalq.egg-info/top_level.txt
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 21:33:25.341440 simalq-1.0.1/tests/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2024-02-23 19:30:05.000000 simalq-1.0.1/tests/__init__.py
```

### Comparing `simalq-1.0.0/PKG-INFO` & `simalq-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: simalq
-Version: 1.0.0
+Version: 1.0.1
 Summary: Infinitesimal Quest 2 + ε: A turn-based puzzling dungeon crawler
 Author: Kodi B. Arfer
 Project-URL: Homepage, http://hylang.org/simalq
 Project-URL: Source Code, https://github.com/hylang/simalq
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Hy
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
 Requires-Python: >= 3.10
 Description-Content-Type: text/x-rst
 
 Infinitesimal Quest 2 + ε
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 `Source code (GitHub) <https://github.com/hylang/simalq>`_
@@ -80,19 +81,22 @@
 - Managing global variables and several notions of global state: see ``Global``
 - Writing a terminal-based game with `blessed <https://pypi.org/project/blessed>`__
 - Parsing a novel binary format with `construct <https://pypi.org/project/construct>`__
 - Generating HTML with a minimal ``ElementTree``-like interface: see ``simalq.tile.tilepedia``
 - Testing a Hy program with `pytest <https://pytest.org>`__ (and with tests that are themselves written in Hy)
 - Creating a new quest for SQ: duplicate the file ``tutorial.hy``, edit it to taste, and put it in the same directory (``quest_definition``)
 
+Some of SQ's approach and a little of its code descends from my earlier unfinished game `Rogue TV <https://github.com/Kodiologist/Rogue-TV>`__.
+
 Version history
 ============================================================
 
 This section lists the most important user-visible changes in each release. Typically, saved games for each version *aren't* compatible with other versions, but release numbers marked with an asterisk (*) should be compatible with saved games from the previous release. Unless making a backward-compatible upgrade of this kind, you should delete all your saved games before upgrading the game.
 
+- 1.0.1* (2024-05-20): Largely internal changes.
 - 1.0.0 (2024-03-01): Various improvements to the display.
 - 0.6.0 (2024-02-19): The IQ quest BoneQuest is now fully playable.
 - 0.5.0 (2024-01-10): Largely internal changes. The new script ``util/gate_map.hy`` may be useful for mapping mazes of teleportation gates, such as New Nightmare level 10.
 - 0.4.0* (2023-09-08): SQ now uses `platformdirs <https://pypi.org/project/platformdirs>`__ to set data directories.
 - 0.3.0 (2023-09-01): There are now difficulty options available through the command line. Variability in the movement of wandering monsters, such as bats, has been improved.
 - 0.2.0* (2023-07-23): The IQ quest New Nightmare has been denazified and added to ``--quests``.
 - 0.1.0 (2023-07-13): First playable release.
```

### Comparing `simalq-1.0.0/README.rst` & `simalq-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,22 @@
 - Managing global variables and several notions of global state: see ``Global``
 - Writing a terminal-based game with `blessed <https://pypi.org/project/blessed>`__
 - Parsing a novel binary format with `construct <https://pypi.org/project/construct>`__
 - Generating HTML with a minimal ``ElementTree``-like interface: see ``simalq.tile.tilepedia``
 - Testing a Hy program with `pytest <https://pytest.org>`__ (and with tests that are themselves written in Hy)
 - Creating a new quest for SQ: duplicate the file ``tutorial.hy``, edit it to taste, and put it in the same directory (``quest_definition``)
 
+Some of SQ's approach and a little of its code descends from my earlier unfinished game `Rogue TV <https://github.com/Kodiologist/Rogue-TV>`__.
+
 Version history
 ============================================================
 
 This section lists the most important user-visible changes in each release. Typically, saved games for each version *aren't* compatible with other versions, but release numbers marked with an asterisk (*) should be compatible with saved games from the previous release. Unless making a backward-compatible upgrade of this kind, you should delete all your saved games before upgrading the game.
 
+- 1.0.1* (2024-05-20): Largely internal changes.
 - 1.0.0 (2024-03-01): Various improvements to the display.
 - 0.6.0 (2024-02-19): The IQ quest BoneQuest is now fully playable.
 - 0.5.0 (2024-01-10): Largely internal changes. The new script ``util/gate_map.hy`` may be useful for mapping mazes of teleportation gates, such as New Nightmare level 10.
 - 0.4.0* (2023-09-08): SQ now uses `platformdirs <https://pypi.org/project/platformdirs>`__ to set data directories.
 - 0.3.0 (2023-09-01): There are now difficulty options available through the command line. Variability in the movement of wandering monsters, such as bats, has been improved.
 - 0.2.0* (2023-07-23): The IQ quest New Nightmare has been denazified and added to ``--quests``.
 - 0.1.0 (2023-07-13): First playable release.
```

### Comparing `simalq-1.0.0/setup.py` & `simalq-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dependencies = [
-    'hy == 0.28.0',
-    'hyrule == 0.5.0',
-    'toolz >= 0.12.0',
+    'hy == 0.29.0',
+    'hyrule == 0.6.0',
+    'toolz >= 0.12.1',
     'construct >= 2.10.70',
     'blessed >= 1.20.0',
-    'platformdirs >= 4.1.0',
+    'platformdirs >= 4.2.2',
     'metadict >= 0.1.3']
 
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name = 'simalq',
-    version = '1.0.0',
+    version = '1.0.1',
     author = 'Kodi B. Arfer',
     description = 'Infinitesimal Quest 2 + ε: A turn-based puzzling dungeon crawler',
     long_description = Path('README.rst').read_text(),
     long_description_content_type = 'text/x-rst',
     project_urls = {
         'Homepage': 'http://hylang.org/simalq',
         'Source Code': 'https://github.com/hylang/simalq'},
@@ -25,8 +25,9 @@
     packages = setuptools.find_packages(),
     package_data = dict(simalq = [
         str(p.relative_to('simalq'))
         for p in Path('simalq').rglob('*.hy')]),
     classifiers = [
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent',
+        'Programming Language :: Hy',
         'Topic :: Games/Entertainment :: Puzzle Games'])
```

### Comparing `simalq-1.0.0/simalq/cmdline.hy` & `simalq-1.0.1/simalq/cmdline.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/color.hy` & `simalq-1.0.1/simalq/color.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/commands.hy` & `simalq-1.0.1/simalq/commands.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/display.hy` & `simalq-1.0.1/simalq/display.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/game_state.hy` & `simalq-1.0.1/simalq/game_state.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/geometry.hy` & `simalq-1.0.1/simalq/geometry.hy`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 ;; --------------------------------------------------------------
 
 (require
   hyrule [unless do-n]
   simalq.macros [defdataclass defmeth])
 (import
   itertools [chain]
+  hyrule [sign thru]
   toolz [unique]
-  simalq.util [seq sign]
   simalq.game-state [G])
 (setv  T True  F False)
 
 ;; --------------------------------------------------------------
 ;; * Helpers
 ;; --------------------------------------------------------------
 
@@ -220,20 +220,20 @@
   important property of it is that activating monsters in this order
   allows monsters closer to the player to move first, so a line of
   monsters can march toward the player without creating gaps.
 
   If `exclude-center` is true, the center position isn't returned."
 
   (unique (gfor
-    c (seq 0 (min size (max center.map.width center.map.height)))
+    c (thru 0 (min size (max center.map.width center.map.height)))
     [x y] (py "chain(
-      (( x, -c) for x in seq(    -c,      c,  1)),
-      (( c,  y) for y in seq(-c + 1,      c,  1)),
-      (( x,  c) for x in seq( c - 1,     -c, -1)),
-      ((-c,  y) for y in seq( c - 1, -c + 1, -1)))")
+      (( x, -c) for x in thru(    -c,      c,  1)),
+      (( c,  y) for y in thru(-c + 1,      c,  1)),
+      (( x,  c) for x in thru( c - 1,     -c, -1)),
+      ((-c,  y) for y in thru( c - 1, -c + 1, -1)))")
     :setv p (try
       (Pos center.map (+ center.x x) (+ center.y y))
       (except [GeometryError]))
     :if (and p (not (and exclude-center (= p center))))
     p)))
 
 (defn burst-size [size [article? True]]
```

### Comparing `simalq-1.0.0/simalq/keyboard.hy` & `simalq-1.0.1/simalq/keyboard.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/main.hy` & `simalq-1.0.1/simalq/main.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/quest.hy` & `simalq-1.0.1/simalq/quest.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/quest_definition/__init__.hy` & `simalq-1.0.1/simalq/quest_definition/__init__.hy`

 * *Files 7% similar despite different names*

```diff
@@ -166,12 +166,11 @@
 ;; --------------------------------------------------
 ;; * Load built-in quests
 ;; --------------------------------------------------
 
 (setv builtin-quests (dfor
   ; Every module in this directory should have the members `name` and
   ; `quest-fn`.
-  [finder m _] (hy.I.pkgutil.walk-packages __path__)
-  :setv spec (.find-spec finder m)
-  :setv m (hy.I.importlib/util.module-from-spec spec)
-  :do (.loader.exec-module spec m)
+  p (.iterdir (hy.I.pathlib.Path (get __path__ 0)))
+  :if (not-in p.name ["__init__.hy" "__pycache__"])
+  :setv m (hy.I.hyrule.import-path p)
   m.name m.quest-fn))
```

### Comparing `simalq-1.0.0/simalq/quest_definition/tutorial.hy` & `simalq-1.0.1/simalq/quest_definition/tutorial.hy`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ;; * Front matter
 
 (import
   fractions [Fraction :as f/]
-  simalq.util [seq]
   simalq.quest-definition [mk-quest])
 (setv  T True  F False)
 
 (setv name "Tutorial Quest")
 
 (defn quest-fn []
 
@@ -141,15 +140,15 @@
     "x " ["wallfall trap" :wallnum 1]
     "X " ["trapped wall" :wallnum 1]
     "☉o" ["generator" :hp 3
       :summon-class "orc"
       :summon-frequency (f/ 1 2)
       :summon-hp 1]
     #** (dfor
-      i (seq 1 8)
+      i (range 10)
       mon ["orc" "wizard"]
       f"{(get mon 0)}{i}" [mon :hp i])}]
 
 6 [:title "Monsters aren't very bright. Take advantage of their simplemindedness to even the odds.\n\nCan you complete this level without taking damage? Don't forget that you can undo moves that you regret."
   :map "
   ▒▒▒▒▒▒. . . . ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
   ▒▒. . . . . . . . ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
```

### Comparing `simalq-1.0.0/simalq/save_load.hy` & `simalq-1.0.1/simalq/save_load.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/strings.hy` & `simalq-1.0.1/simalq/strings.hy`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,15 @@
   "You miss Geralt."
   "You smell something familiar."
   "You sneeze."
   "You suddenly think of a great recipe for muffins."
   "You suddenly yearn for your distant homeland."
   "You summon a butterfly. It flies away."
   "You've got mail."
+  "Your dad turns into a chickenrat."
   "Your skin turns orange."
   "python3: segmentation fault (core dumped)"
   #[[The wand asks "For what do you wish?" After you reply, it says "Yeah, me too."]]
   #[[The wand says "I've not seen such bravery!".]]
   #[[The wand says "Moof!".]]
   #[[The wand says "Prince Argonn, you are about to die."]]))
```

### Comparing `simalq-1.0.0/simalq/tile/__init__.hy` & `simalq-1.0.1/simalq/tile/__init__.hy`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ;; --------------------------------------------------------------
 ;; * Imports
 ;; --------------------------------------------------------------
 
 (require
-  hyrule [unless]
-  simalq.macros [field-defaults defmeth defmacro-kwargs])
+  hyrule [unless defmacro-kwargs]
+  simalq.macros [field-defaults defmeth])
 (import
   copy [deepcopy]
   re
   simalq.color :as color
   simalq.game-state [G]
   simalq.util [player-melee-damage DamageType]
   simalq.geometry [at])
```

### Comparing `simalq-1.0.0/simalq/tile/item.hy` & `simalq-1.0.1/simalq/tile/item.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/tile/monster.hy` & `simalq-1.0.1/simalq/tile/monster.hy`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 ;; --------------------------------------------------------------
 ;; * Imports
 ;; --------------------------------------------------------------
 
 (require
-  hyrule [unless do-n list-n]
-  simalq.macros [field-defaults pop-integer-part defmeth defmacro-kwargs]
+  hyrule [unless do-n list-n defmacro-kwargs]
+  simalq.macros [field-defaults pop-integer-part defmeth]
   simalq.tile [deftile])
 (import
   re
   fractions [Fraction :as f/]
   enum [Enum]
+  hyrule [thru]
   toolz [unique]
-  simalq.util [DamageType StatusEffect next-in-cycle mixed-number seq]
+  simalq.util [DamageType StatusEffect next-in-cycle mixed-number]
   simalq.geometry [Direction at dist adjacent? dir-to turn-and-pos-seed ray]
   simalq.game-state [G]
   simalq.tile [Tile Actor Damageable]
   simalq.tile.scenery [Scenery walkability can-occupy?])
 (setv  T True  F False)
 
 ;; --------------------------------------------------------------
@@ -413,15 +414,15 @@
     (deftile ~mapsym ~name [Generated ~@superc]
       :iq-ix-mapper ["hp"
         ~(dict (zip iq-ix-mon [1 2 3]))]
       :destruction-points ~points-mon
       :points-for-generator (classmethod (fn [cls] ~points-gen))
       :flavor ~flavor-mon
       :flavor-for-generator ~flavor-gen
-      ~@(sum :start [] (gfor
+      ~@(hy.I.toolz.concat (gfor
         [k v] (.items kwargs)
         [(hy.models.Keyword k) v])))
 
     ((fn [] (for [[iq-ix hp] (zip ~iq-ix-gen [1 2 3])]
       (setv (get Tile.types-by-iq-ix iq-ix) (fn [pos _ te-v2 [hp hp]]
         ; We need `[hp hp]` above to be sure we get a separate variable
         ; for each closure.
@@ -784,15 +785,15 @@
       (return))
     (when (@try-to-attack-player :dry-run T)
       (+= @shot-power @shot-frequency)
       (when (pop-integer-part @shot-power)
         (@try-to-attack-player)
         (return)))
     (for [
-        dist-from-player [#* (seq 2 G.rules.reality-bubble-size) 1]
+        dist-from-player [#* (thru 2 G.rules.reality-bubble-size) 1]
         direction Direction.all
         :if (setx target (.+n G.player.pos dist-from-player direction))]
       (when (and
           (or
             (= target @pos)
             (can-occupy? target :monster? T :ethereal-to #()))
           (@try-to-attack-player :dry-run T :pos target))
```

### Comparing `simalq-1.0.0/simalq/tile/player.hy` & `simalq-1.0.1/simalq/tile/player.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/tile/scenery.hy` & `simalq-1.0.1/simalq/tile/scenery.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/tile/tilepedia.hy` & `simalq-1.0.1/simalq/tile/tilepedia.hy`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 "Render all tile info screens into a single HTML page."
 
 
 (import
+  toolz [concat]
   metadict [MetaDict]
   simalq.color
   simalq.game-state [G]
   simalq.tile [Tile Player]
   simalq.display [color-tile])
 (setv  T True  F False)
 
@@ -93,17 +94,17 @@
         [superclass-name tiles] (.items info)
         (E.li superclass-name (E.ul #* (gfor
           tile tiles
           (E.li (mapsym tile) (E.a tile.long-name
             :href (+ "#" tile.id)))))))))
 
     ; One section of info screens per superclass
-    #* (cat (gfor
+    #* (concat (gfor
       [superclass-name tiles] (.items info)
-      [(E.h2 superclass-name) #* (cat (gfor
+      [(E.h2 superclass-name) #* (concat (gfor
         ; One info screen per tile type
         tile tiles
         [(E.h3 (mapsym tile) tile.long-name :id tile.id)
           (E.ul #* (gfor
             bullet tile.bullets
             (E.li #* (if (isinstance bullet tuple)
               [(E.strong (get bullet 0) ": ") (str (get bullet 1))]
@@ -127,13 +128,9 @@
     (.join " " (gfor
       [k v] (.items attrs)
       f"{(hesc k)}='{(hesc v)}'"))
     (.join "" (map render-elem kids))
     (if self-closing "" f"</{(hesc tag)}>")))
 
 
-(defn cat [l]
-  (sum :start [] l))
-
-
 (when (= __name__ "__main__")
   (print (html)))
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-"Render all tile info screens into a single HTML page." (import metadict
-[MetaDict] simalq.color simalq.game-state [G] simalq.tile [Tile Player]
-simalq.display [color-tile]) (setv T True F False) (defn get-info [] "Compile
-all the tile info screens into a dictionary." ; Initialize `G`. (hy.I.simalq/
-quest.start-quest (hy.I.simalq/un-iq.iq-quest "Boot Camp 2")) (hy.I.simalq/
-quest.start-level 1) (setv tiles (lfor tt (.values Tile.types) (if (is tt
-Player) G.player (tt)))) (MetaDict (dfor [name superclass] (.items
+"Render all tile info screens into a single HTML page." (import toolz [concat]
+metadict [MetaDict] simalq.color simalq.game-state [G] simalq.tile [Tile
+Player] simalq.display [color-tile]) (setv T True F False) (defn get-info []
+"Compile all the tile info screens into a dictionary." ; Initialize `G`.
+(hy.I.simalq/quest.start-quest (hy.I.simalq/un-iq.iq-quest "Boot Camp 2"))
+(hy.I.simalq/quest.start-level 1) (setv tiles (lfor tt (.values Tile.types) (if
+(is tt Player) G.player (tt)))) (MetaDict (dfor [name superclass] (.items
 Tile.superclasses) name (lfor tile tiles :if (isinstance tile superclass) (dict
 :id (.replace tile.stem " " "-") :long-name tile.name-with-article :mapsym
 (lfor cc (color-tile tile) (dict :char cc.char :colors (lfor color [ (or cc.fg
 simalq.color.default-fg) (or cc.bg simalq.color.default-bg)] (get
 simalq.color.by-name color)) :bold cc.bold)) :bullets (lfor bullet (.info-
 bullets tile) :if bullet bullet) :flavor tile.flavor))))) (defn html [] "Use
 `get-info` to construct an HTML document." (defn mapsym [tile] (E.code :class
@@ -22,22 +22,21 @@
 page header (E.h1 "Tilepedia") (E.p "This page is a compendium of info screens
 for every tile type in " (E.a :href "https://hylang.org/simalq" "Infinitesimal
 Quest 2 + Îµ") ". It's generated by " (E.code "simalq.tile.tilepedia.html") ".
 It reflects default values for each type; " "in game, for example, monsters can
 have more than 1 HP.") ; The table of contents (E.nav (E.h2 "Contents") (E.ul
 #* (gfor [superclass-name tiles] (.items info) (E.li superclass-name (E.ul #*
 (gfor tile tiles (E.li (mapsym tile) (E.a tile.long-name :href (+ "#"
-tile.id))))))))) ; One section of info screens per superclass #* (cat (gfor
-[superclass-name tiles] (.items info) [(E.h2 superclass-name) #* (cat (gfor ;
-One info screen per tile type tile tiles [(E.h3 (mapsym tile) tile.long-name :
-id tile.id) (E.ul #* (gfor bullet tile.bullets (E.li #* (if (isinstance bullet
+tile.id))))))))) ; One section of info screens per superclass #* (concat (gfor
+[superclass-name tiles] (.items info) [(E.h2 superclass-name) #* (concat (gfor
+; One info screen per tile type tile tiles [(E.h3 (mapsym tile) tile.long-name
+:id tile.id) (E.ul #* (gfor bullet tile.bullets (E.li #* (if (isinstance bullet
 tuple) [(E.strong (get bullet 0) ": ") (str (get bullet 1))] [(E.strong
 bullet)])))) (E.div :class "flavor" tile.flavor)]))])))))) ; In combination
 with `render-elem`, `E` works roughly like ; `lxml.builder.ElementMaker`. (setv
 E ((type "ElementMaker" #() (dict :__getattr__ (fn [self tag] (fn [#* kids
 [_self-closing F] #** attrs] #(tag attrs kids _self-closing))))))) (defn
 render-elem [x] (import html [escape :as hesc]) (when (isinstance x str)
 (return (hesc x :quote F))) (setv [tag attrs kids self-closing] x) (.format "<
 {} {}>{}{}" (hesc tag) (.join " " (gfor [k v] (.items attrs) f"{(hesc k)}='{
 (hesc v)}'")) (.join "" (map render-elem kids)) (if self-closing "" f"
-(hesc tag)}>"))) (defn cat [l] (sum :start [] l)) (when (= __name__ "__main__")
-(print (html)))
+(hesc tag)}>"))) (when (= __name__ "__main__") (print (html)))
```

### Comparing `simalq-1.0.0/simalq/tile/unimplemented.hy` & `simalq-1.0.1/simalq/tile/unimplemented.hy`

 * *Files identical despite different names*

### Comparing `simalq-1.0.0/simalq/un_iq.hy` & `simalq-1.0.1/simalq/un_iq.hy`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,42 @@
 (require
   hyrule [unless case])
 (import
   types [FunctionType]
   fractions [Fraction :as f/]
   zipfile [ZipFile]
   functools [cache]
+  hyrule [thru]
   construct
   toolz [partition]
-  simalq.util [cache-dir seq]
+  simalq.util [cache-dir]
   simalq.geometry [Map Pos]
   simalq.quest [Quest Level]
   simalq.tile [Tile])
 (setv  T True  F False)
 
 ;; --------------------------------------------------------------
 ;; * Helpers
 ;; --------------------------------------------------------------
 
 (setv FLOOR 1)
   ; The IQ index number for plain floor.
 
-(eval-when-compile (defn replace-atoms [x f]
-  (import hyrule [coll?])
-  (if (coll? x)
-    ((type x) (gfor  elem x  (replace-atoms elem f)))
-    (f x))))
-
 (defmacro with-construct [#* body]
   "Replace all symbols starting with an uppercase letter, like
   `Foo`, with `construct.Foo`, plus `this`, minus booleans and
   `None`."
-  `(do ~@(replace-atoms body (fn [x]
-    (if (or
+  `(do ~@(hy.I.hyrule.map-model body (fn [x]
+    (when (or
           (= x 'this)
           (and
             (isinstance x hy.models.Symbol)
             (.isupper (get x 0))
             (not-in x '[True False T F None])))
-      `(. construct ~x)
-      x)))))
+      `(. construct ~x))))))
 
 (defmacro kw-struct [#* args]
   "Create a `construct.Struct`, naming the fields with Hy keyword
   objects."
   `(construct.Struct ~@((fn []
     (setv xs (list args))
     (while xs
@@ -202,16 +196,16 @@
         "Convert from IQ coordinates (1-based indices, y = 1 on top, 0
         means missing) to SQ coordinates (0-based indices with y = 0 on
         bottom, None means missing)."
         (if (and #* xy)
           (Pos m (- (get xy 0) 1) (- m.height (get xy 1)))
           None))
       :setv iq-ixes (dfor
-        ix (seq 1 m.width)
-        iy (seq 1 m.height)
+        ix (thru 1 m.width)
+        iy (thru 1 m.height)
         (mk-pos #(ix iy)) (get l.map (+ (* (- ix 1) l.height) (- iy 1))))
       :setv tile-extras (dfor
         pair l.tile-extras
         (mk-pos pair.pos) (tuple pair.data))
 
       :do (for [x (range m.width)  y (range m.height)]
         ; Fill in `m`.
@@ -357,15 +351,15 @@
           ██████████, ██████████
           █3. ☉G> ██. ██> ☉G. █2
           ██████████d ██████████
           , . d . o . o . d . ██
           ██████████████████, ██"
         :map-marks {
           #** (dfor
-            i (seq 1 4)
+            i (thru 1 4)
             f"█{i}" ["trapped wall" :wallnum i])
           ", " "broken trap"
           "o " ["orc" :hp 3]
           "☉G" ["generator"
             :hp 3
             :summon-class "ghost"
             :summon-frequency (f/ 1)
```

### Comparing `simalq-1.0.0/simalq/util.hy` & `simalq-1.0.1/simalq/util.hy`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,14 @@
 
 (setv platform-dirs (hy.I.platformdirs.PlatformDirs
   :appname "simalq" :appauthor "hylang"))
 (setv cache-dir (Path platform-dirs.user-cache-dir))
 (setv saved-games-dir (/ (Path platform-dirs.user-data-dir) "save"))
 
 
-(defn seq [a b [step 1]]
-  "A version of `range` that includes both ends (given a compatible
-  step size)."
-  (range a (+ b step) step))
-
-(defn sign [x]
-  "N.B. This function returns 0 for -0.0, and raises `TypeError` for NaN."
-  (cond
-    (< x 0) -1
-    (> x 0)  1
-    (= x 0)  0
-    True     (raise TypeError)))
-
 (defn mixed-number [fraction]
   (setv n (pop-integer-part fraction))
   (or
     (.join " " (lfor  x [n fraction]  :if x  (str x)))
     "0"))
 
 (defn next-in-cycle [sequence e]
```

### Comparing `simalq-1.0.0/simalq.egg-info/PKG-INFO` & `simalq-1.0.1/simalq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: simalq
-Version: 1.0.0
+Version: 1.0.1
 Summary: Infinitesimal Quest 2 + ε: A turn-based puzzling dungeon crawler
 Author: Kodi B. Arfer
 Project-URL: Homepage, http://hylang.org/simalq
 Project-URL: Source Code, https://github.com/hylang/simalq
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Hy
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
 Requires-Python: >= 3.10
 Description-Content-Type: text/x-rst
 
 Infinitesimal Quest 2 + ε
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 `Source code (GitHub) <https://github.com/hylang/simalq>`_
@@ -80,19 +81,22 @@
 - Managing global variables and several notions of global state: see ``Global``
 - Writing a terminal-based game with `blessed <https://pypi.org/project/blessed>`__
 - Parsing a novel binary format with `construct <https://pypi.org/project/construct>`__
 - Generating HTML with a minimal ``ElementTree``-like interface: see ``simalq.tile.tilepedia``
 - Testing a Hy program with `pytest <https://pytest.org>`__ (and with tests that are themselves written in Hy)
 - Creating a new quest for SQ: duplicate the file ``tutorial.hy``, edit it to taste, and put it in the same directory (``quest_definition``)
 
+Some of SQ's approach and a little of its code descends from my earlier unfinished game `Rogue TV <https://github.com/Kodiologist/Rogue-TV>`__.
+
 Version history
 ============================================================
 
 This section lists the most important user-visible changes in each release. Typically, saved games for each version *aren't* compatible with other versions, but release numbers marked with an asterisk (*) should be compatible with saved games from the previous release. Unless making a backward-compatible upgrade of this kind, you should delete all your saved games before upgrading the game.
 
+- 1.0.1* (2024-05-20): Largely internal changes.
 - 1.0.0 (2024-03-01): Various improvements to the display.
 - 0.6.0 (2024-02-19): The IQ quest BoneQuest is now fully playable.
 - 0.5.0 (2024-01-10): Largely internal changes. The new script ``util/gate_map.hy`` may be useful for mapping mazes of teleportation gates, such as New Nightmare level 10.
 - 0.4.0* (2023-09-08): SQ now uses `platformdirs <https://pypi.org/project/platformdirs>`__ to set data directories.
 - 0.3.0 (2023-09-01): There are now difficulty options available through the command line. Variability in the movement of wandering monsters, such as bats, has been improved.
 - 0.2.0* (2023-07-23): The IQ quest New Nightmare has been denazified and added to ``--quests``.
 - 0.1.0 (2023-07-13): First playable release.
```

### Comparing `simalq-1.0.0/simalq.egg-info/SOURCES.txt` & `simalq-1.0.1/simalq.egg-info/SOURCES.txt`

 * *Files identical despite different names*


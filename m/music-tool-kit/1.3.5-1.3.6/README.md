# Comparing `tmp/music-tool-kit-1.3.5.tar.gz` & `tmp/music-tool-kit-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music-tool-kit-1.3.5.tar", last modified: Tue Mar 12 06:57:55 2024, max compression
+gzip compressed data, was "music-tool-kit-1.3.6.tar", last modified: Mon May 20 05:57:25 2024, max compression
```

## Comparing `music-tool-kit-1.3.5.tar` & `music-tool-kit-1.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:57:55.373577 music-tool-kit-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-12 06:57:37.000000 music-tool-kit-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-03-12 06:57:55.373577 music-tool-kit-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-12 06:57:37.000000 music-tool-kit-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:57:55.373577 music-tool-kit-1.3.5/mk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 06:57:37.000000 music-tool-kit-1.3.5/mk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-03-12 06:57:37.000000 music-tool-kit-1.3.5/mk/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:57:55.373577 music-tool-kit-1.3.5/music_tool_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-03-12 06:57:55.000000 music-tool-kit-1.3.5/music_tool_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-12 06:57:55.000000 music-tool-kit-1.3.5/music_tool_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 06:57:55.000000 music-tool-kit-1.3.5/music_tool_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-12 06:57:55.000000 music-tool-kit-1.3.5/music_tool_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 06:57:55.000000 music-tool-kit-1.3.5/music_tool_kit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-12 06:57:55.000000 music-tool-kit-1.3.5/music_tool_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-12 06:57:55.000000 music-tool-kit-1.3.5/music_tool_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 06:57:55.373577 music-tool-kit-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-12 06:57:37.000000 music-tool-kit-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:57:25.819848 music-tool-kit-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 05:57:07.000000 music-tool-kit-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-20 05:57:25.819848 music-tool-kit-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-20 05:57:07.000000 music-tool-kit-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:57:25.819848 music-tool-kit-1.3.6/mk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:57:07.000000 music-tool-kit-1.3.6/mk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-05-20 05:57:07.000000 music-tool-kit-1.3.6/mk/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:57:25.819848 music-tool-kit-1.3.6/music_tool_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-20 05:57:25.000000 music-tool-kit-1.3.6/music_tool_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 05:57:25.000000 music-tool-kit-1.3.6/music_tool_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:57:25.000000 music-tool-kit-1.3.6/music_tool_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 05:57:25.000000 music-tool-kit-1.3.6/music_tool_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:57:25.000000 music-tool-kit-1.3.6/music_tool_kit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 05:57:25.000000 music-tool-kit-1.3.6/music_tool_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-20 05:57:25.000000 music-tool-kit-1.3.6/music_tool_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:57:25.819848 music-tool-kit-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-20 05:57:07.000000 music-tool-kit-1.3.6/setup.py
```

### Comparing `music-tool-kit-1.3.5/LICENSE` & `music-tool-kit-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `music-tool-kit-1.3.5/PKG-INFO` & `music-tool-kit-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-tool-kit
-Version: 1.3.5
+Version: 1.3.6
 Summary: A tool kit for music download and clip
 Home-page: https://github.com/nichuanfang/music-tool-kit
 Author: Nichuan Fang
 Author-email: f18326186224@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/nichuanfang/music-tool-kit
 Project-URL: Bug Tracker, https://github.com/nichuanfang/music-tool-kit/issues
```

### Comparing `music-tool-kit-1.3.5/README.md` & `music-tool-kit-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `music-tool-kit-1.3.5/mk/__main__.py` & `music-tool-kit-1.3.6/mk/__main__.py`

 * *Files identical despite different names*

### Comparing `music-tool-kit-1.3.5/music_tool_kit.egg-info/PKG-INFO` & `music-tool-kit-1.3.6/music_tool_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-tool-kit
-Version: 1.3.5
+Version: 1.3.6
 Summary: A tool kit for music download and clip
 Home-page: https://github.com/nichuanfang/music-tool-kit
 Author: Nichuan Fang
 Author-email: f18326186224@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/nichuanfang/music-tool-kit
 Project-URL: Bug Tracker, https://github.com/nichuanfang/music-tool-kit/issues
```

### Comparing `music-tool-kit-1.3.5/setup.py` & `music-tool-kit-1.3.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     readme = f.read()
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read()
 
 setup(
     name='music-tool-kit',
-    version='1.3.5',
+    version='1.3.6',
     description='A tool kit for music download and clip',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/nichuanfang/music-tool-kit',
 
     project_urls={
         'Source Code': 'https://github.com/nichuanfang/music-tool-kit',
```


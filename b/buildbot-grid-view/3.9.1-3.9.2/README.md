# Comparing `tmp/buildbot-grid-view-3.9.1.tar.gz` & `tmp/buildbot-grid-view-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-grid-view-3.9.1.tar", last modified: Sat Sep  2 16:04:01 2023, max compression
+gzip compressed data, was "buildbot-grid-view-3.9.2.tar", last modified: Sat Sep  2 20:52:12 2023, max compression
```

## Comparing `buildbot-grid-view-3.9.1.tar` & `buildbot-grid-view-3.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:01.153432 buildbot-grid-view-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      262 2023-09-02 16:04:01.153432 buildbot-grid-view-3.9.1/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:01.153432 buildbot-grid-view-3.9.1/buildbot_grid_view/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      861 2023-09-02 16:00:07.000000 buildbot-grid-view-3.9.1/buildbot_grid_view/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:01.153432 buildbot-grid-view-3.9.1/buildbot_grid_view/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9944 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31122 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view/static/scripts.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      545 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view/static/styles.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      837 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view/static/styles.css.map
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:01.153432 buildbot-grid-view-3.9.1/buildbot_grid_view.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      262 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      445 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       49 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-09-02 16:04:01.000000 buildbot-grid-view-3.9.1/buildbot_grid_view.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 16:04:01.153432 buildbot-grid-view-3.9.1/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1533 2023-09-02 16:00:07.000000 buildbot-grid-view-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:12.615054 buildbot-grid-view-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      262 2023-09-02 20:52:12.615054 buildbot-grid-view-3.9.2/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:12.611055 buildbot-grid-view-3.9.2/buildbot_grid_view/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      861 2023-09-02 20:48:25.000000 buildbot-grid-view-3.9.2/buildbot_grid_view/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:12.615054 buildbot-grid-view-3.9.2/buildbot_grid_view/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9944 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31122 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view/static/scripts.js.map
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      545 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view/static/styles.css
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      837 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view/static/styles.css.map
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:12.611055 buildbot-grid-view-3.9.2/buildbot_grid_view.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      262 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      445 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       49 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-09-02 20:52:12.000000 buildbot-grid-view-3.9.2/buildbot_grid_view.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 20:52:12.615054 buildbot-grid-view-3.9.2/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1533 2023-09-02 20:48:25.000000 buildbot-grid-view-3.9.2/setup.py
```

### Comparing `buildbot-grid-view-3.9.1/buildbot_grid_view/__init__.py` & `buildbot-grid-view-3.9.2/buildbot_grid_view/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.9.1/buildbot_grid_view/static/scripts.js` & `buildbot-grid-view-3.9.2/buildbot_grid_view/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.9.1/buildbot_grid_view/static/scripts.js.map` & `buildbot-grid-view-3.9.2/buildbot_grid_view/static/scripts.js.map`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.9.1/buildbot_grid_view/static/styles.css` & `buildbot-grid-view-3.9.2/buildbot_grid_view/static/styles.css`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.9.1/buildbot_grid_view/static/styles.css.map` & `buildbot-grid-view-3.9.2/buildbot_grid_view/static/styles.css.map`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.9.1/setup.py` & `buildbot-grid-view-3.9.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/buildbot-react-grid-view-3.9.1.tar.gz` & `tmp/buildbot-react-grid-view-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-react-grid-view-3.9.1.tar", last modified: Sat Sep  2 16:04:07 2023, max compression
+gzip compressed data, was "buildbot-react-grid-view-3.9.2.tar", last modified: Sat Sep  2 20:52:18 2023, max compression
```

## Comparing `buildbot-react-grid-view-3.9.1.tar` & `buildbot-react-grid-view-3.9.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:07.013503 buildbot-react-grid-view-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      276 2023-09-02 16:04:07.013503 buildbot-react-grid-view-3.9.1/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:07.013503 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 16:04:06.000000 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      861 2023-09-02 16:00:07.000000 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:07.013503 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    29690 2023-09-02 16:04:06.000000 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view/static/scripts.js
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:07.013503 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      276 2023-09-02 16:04:06.000000 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      374 2023-09-02 16:04:06.000000 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:04:06.000000 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       61 2023-09-02 16:04:06.000000 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       25 2023-09-02 16:04:06.000000 buildbot-react-grid-view-3.9.1/buildbot_react_grid_view.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 16:04:07.013503 buildbot-react-grid-view-3.9.1/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1563 2023-09-02 16:00:07.000000 buildbot-react-grid-view-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:18.547048 buildbot-react-grid-view-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      276 2023-09-02 20:52:18.547048 buildbot-react-grid-view-3.9.2/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:18.543048 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 20:52:18.000000 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      861 2023-09-02 20:48:25.000000 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:18.547048 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    29690 2023-09-02 20:52:18.000000 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view/static/scripts.js
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:18.547048 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      276 2023-09-02 20:52:18.000000 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      374 2023-09-02 20:52:18.000000 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:52:18.000000 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       61 2023-09-02 20:52:18.000000 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       25 2023-09-02 20:52:18.000000 buildbot-react-grid-view-3.9.2/buildbot_react_grid_view.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 20:52:18.547048 buildbot-react-grid-view-3.9.2/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1563 2023-09-02 20:48:25.000000 buildbot-react-grid-view-3.9.2/setup.py
```

### Comparing `buildbot-react-grid-view-3.9.1/buildbot_react_grid_view/__init__.py` & `buildbot-react-grid-view-3.9.2/buildbot_react_grid_view/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-react-grid-view-3.9.1/buildbot_react_grid_view/static/scripts.js` & `buildbot-react-grid-view-3.9.2/buildbot_react_grid_view/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-react-grid-view-3.9.1/setup.py` & `buildbot-react-grid-view-3.9.2/setup.py`

 * *Files identical despite different names*


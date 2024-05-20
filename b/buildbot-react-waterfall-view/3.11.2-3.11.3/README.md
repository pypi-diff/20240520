# Comparing `tmp/buildbot_react_waterfall_view-3.11.2.tar.gz` & `tmp/buildbot_react_waterfall_view-3.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot_react_waterfall_view-3.11.2.tar", last modified: Sat May  4 22:43:09 2024, max compression
+gzip compressed data, was "buildbot_react_waterfall_view-3.11.3.tar", last modified: Mon May 20 17:14:09 2024, max compression
```

## Comparing `buildbot_react_waterfall_view-3.11.2.tar` & `buildbot_react_waterfall_view-3.11.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-04 22:43:09.354442 buildbot_react_waterfall_view-3.11.2/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      283 2024-05-04 22:43:09.354442 buildbot_react_waterfall_view-3.11.2/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-04 22:43:09.350442 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        6 2024-05-04 22:43:09.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      866 2024-05-04 22:38:21.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-04 22:43:09.354442 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   183718 2024-05-04 22:43:09.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3116 2024-05-04 22:43:09.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/static/styles.css
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-04 22:43:09.354442 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      283 2024-05-04 22:43:09.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      462 2024-05-04 22:43:09.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2024-05-04 22:43:09.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       71 2024-05-04 22:43:09.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       30 2024-05-04 22:43:09.000000 buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2024-05-04 22:43:09.354442 buildbot_react_waterfall_view-3.11.2/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1615 2024-05-04 22:38:21.000000 buildbot_react_waterfall_view-3.11.2/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-20 17:14:09.237849 buildbot_react_waterfall_view-3.11.3/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      283 2024-05-20 17:14:09.237849 buildbot_react_waterfall_view-3.11.3/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-20 17:14:09.237849 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        6 2024-05-20 17:14:09.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      866 2024-05-20 17:08:54.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-20 17:14:09.237849 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   183718 2024-05-20 17:14:09.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3116 2024-05-20 17:14:09.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/static/styles.css
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-20 17:14:09.237849 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      283 2024-05-20 17:14:09.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      462 2024-05-20 17:14:09.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2024-05-20 17:14:09.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       71 2024-05-20 17:14:09.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       30 2024-05-20 17:14:09.000000 buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2024-05-20 17:14:09.237849 buildbot_react_waterfall_view-3.11.3/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1615 2024-05-20 17:08:54.000000 buildbot_react_waterfall_view-3.11.3/setup.py
```

### Comparing `buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/__init__.py` & `buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/static/scripts.js` & `buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot_react_waterfall_view-3.11.2/buildbot_react_waterfall_view/static/styles.css` & `buildbot_react_waterfall_view-3.11.3/buildbot_react_waterfall_view/static/styles.css`

 * *Files identical despite different names*

### Comparing `buildbot_react_waterfall_view-3.11.2/setup.py` & `buildbot_react_waterfall_view-3.11.3/setup.py`

 * *Files identical despite different names*


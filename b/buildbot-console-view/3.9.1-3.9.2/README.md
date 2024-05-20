# Comparing `tmp/buildbot-console-view-3.9.1.tar.gz` & `tmp/buildbot-console-view-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-console-view-3.9.1.tar", last modified: Sat Sep  2 16:03:44 2023, max compression
+gzip compressed data, was "buildbot-console-view-3.9.2.tar", last modified: Sat Sep  2 20:51:56 2023, max compression
```

## Comparing `buildbot-console-view-3.9.1.tar` & `buildbot-console-view-3.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:44.937235 buildbot-console-view-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      264 2023-09-02 16:03:44.937235 buildbot-console-view-3.9.1/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:44.933235 buildbot-console-view-3.9.1/buildbot_console_view/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      860 2023-09-02 16:00:07.000000 buildbot-console-view-3.9.1/buildbot_console_view/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:44.937235 buildbot-console-view-3.9.1/buildbot_console_view/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12053 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    40229 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view/static/scripts.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1161 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view/static/styles.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1660 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view/static/styles.css.map
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:44.933235 buildbot-console-view-3.9.1/buildbot_console_view.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      264 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      478 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       55 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       22 2023-09-02 16:03:44.000000 buildbot-console-view-3.9.1/buildbot_console_view.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 16:03:44.937235 buildbot-console-view-3.9.1/setup.cfg
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     1544 2023-09-02 16:00:07.000000 buildbot-console-view-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:51:56.747070 buildbot-console-view-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      264 2023-09-02 20:51:56.747070 buildbot-console-view-3.9.2/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:51:56.747070 buildbot-console-view-3.9.2/buildbot_console_view/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      860 2023-09-02 20:48:25.000000 buildbot-console-view-3.9.2/buildbot_console_view/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:51:56.747070 buildbot-console-view-3.9.2/buildbot_console_view/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12053 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    40229 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view/static/scripts.js.map
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1161 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view/static/styles.css
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1660 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view/static/styles.css.map
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:51:56.747070 buildbot-console-view-3.9.2/buildbot_console_view.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      264 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      478 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       55 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       22 2023-09-02 20:51:56.000000 buildbot-console-view-3.9.2/buildbot_console_view.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 20:51:56.747070 buildbot-console-view-3.9.2/setup.cfg
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     1544 2023-09-02 20:48:25.000000 buildbot-console-view-3.9.2/setup.py
```

### Comparing `buildbot-console-view-3.9.1/buildbot_console_view/__init__.py` & `buildbot-console-view-3.9.2/buildbot_console_view/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.9.1/buildbot_console_view/static/scripts.js` & `buildbot-console-view-3.9.2/buildbot_console_view/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.9.1/buildbot_console_view/static/scripts.js.map` & `buildbot-console-view-3.9.2/buildbot_console_view/static/scripts.js.map`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.9.1/buildbot_console_view/static/styles.css` & `buildbot-console-view-3.9.2/buildbot_console_view/static/styles.css`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.9.1/buildbot_console_view/static/styles.css.map` & `buildbot-console-view-3.9.2/buildbot_console_view/static/styles.css.map`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.9.1/setup.py` & `buildbot-console-view-3.9.2/setup.py`

 * *Files identical despite different names*


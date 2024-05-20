# Comparing `tmp/buildbot-react-console-view-3.9.1.tar.gz` & `tmp/buildbot-react-console-view-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-react-console-view-3.9.1.tar", last modified: Sat Sep  2 16:03:51 2023, max compression
+gzip compressed data, was "buildbot-react-console-view-3.9.2.tar", last modified: Sat Sep  2 20:52:02 2023, max compression
```

## Comparing `buildbot-react-console-view-3.9.1.tar` & `buildbot-react-console-view-3.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:51.149310 buildbot-react-console-view-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      278 2023-09-02 16:03:51.149310 buildbot-react-console-view-3.9.1/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:51.145310 buildbot-react-console-view-3.9.1/buildbot_react_console_view/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 16:03:51.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      864 2023-09-02 16:00:07.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:51.149310 buildbot-react-console-view-3.9.1/buildbot_react_console_view/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    62416 2023-09-02 16:03:51.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      507 2023-09-02 16:03:51.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view/static/styles.css
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:51.145310 buildbot-react-console-view-3.9.1/buildbot_react_console_view.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      278 2023-09-02 16:03:51.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      444 2023-09-02 16:03:51.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:03:51.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       67 2023-09-02 16:03:51.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       28 2023-09-02 16:03:51.000000 buildbot-react-console-view-3.9.1/buildbot_react_console_view.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 16:03:51.149310 buildbot-react-console-view-3.9.1/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1574 2023-09-02 16:00:07.000000 buildbot-react-console-view-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:02.887064 buildbot-react-console-view-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      278 2023-09-02 20:52:02.887064 buildbot-react-console-view-3.9.2/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:02.883064 buildbot-react-console-view-3.9.2/buildbot_react_console_view/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 20:52:02.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      864 2023-09-02 20:48:25.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:02.883064 buildbot-react-console-view-3.9.2/buildbot_react_console_view/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    62416 2023-09-02 20:52:02.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      507 2023-09-02 20:52:02.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view/static/styles.css
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:02.883064 buildbot-react-console-view-3.9.2/buildbot_react_console_view.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      278 2023-09-02 20:52:02.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      444 2023-09-02 20:52:02.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:52:02.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       67 2023-09-02 20:52:02.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       28 2023-09-02 20:52:02.000000 buildbot-react-console-view-3.9.2/buildbot_react_console_view.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 20:52:02.887064 buildbot-react-console-view-3.9.2/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1574 2023-09-02 20:48:25.000000 buildbot-react-console-view-3.9.2/setup.py
```

### Comparing `buildbot-react-console-view-3.9.1/buildbot_react_console_view/__init__.py` & `buildbot-react-console-view-3.9.2/buildbot_react_console_view/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-react-console-view-3.9.1/buildbot_react_console_view/static/scripts.js` & `buildbot-react-console-view-3.9.2/buildbot_react_console_view/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-react-console-view-3.9.1/setup.py` & `buildbot-react-console-view-3.9.2/setup.py`

 * *Files identical despite different names*


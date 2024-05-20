# Comparing `tmp/buildbot_react_wsgi_dashboards-3.11.2.tar.gz` & `tmp/buildbot_react_wsgi_dashboards-3.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot_react_wsgi_dashboards-3.11.2.tar", last modified: Sat May  4 22:43:21 2024, max compression
+gzip compressed data, was "buildbot_react_wsgi_dashboards-3.11.3.tar", last modified: Mon May 20 17:14:23 2024, max compression
```

## Comparing `buildbot_react_wsgi_dashboards-3.11.2.tar` & `buildbot_react_wsgi_dashboards-3.11.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-04 22:43:21.414518 buildbot_react_wsgi_dashboards-3.11.2/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      333 2024-05-04 22:43:21.414518 buildbot_react_wsgi_dashboards-3.11.2/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-04 22:43:21.410518 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        6 2024-05-04 22:43:21.000000 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1730 2024-05-04 22:38:21.000000 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-04 22:43:21.414518 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)  1290143 2024-05-04 22:43:21.000000 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards/static/scripts.js
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-04 22:43:21.414518 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      333 2024-05-04 22:43:21.000000 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      422 2024-05-04 22:43:21.000000 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2024-05-04 22:43:21.000000 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       73 2024-05-04 22:43:21.000000 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       31 2024-05-04 22:43:21.000000 buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2024-05-04 22:43:21.414518 buildbot_react_wsgi_dashboards-3.11.2/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1670 2024-05-04 22:38:21.000000 buildbot_react_wsgi_dashboards-3.11.2/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-20 17:14:23.269998 buildbot_react_wsgi_dashboards-3.11.3/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      333 2024-05-20 17:14:23.269998 buildbot_react_wsgi_dashboards-3.11.3/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-20 17:14:23.265998 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        6 2024-05-20 17:14:23.000000 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1730 2024-05-20 17:08:54.000000 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-20 17:14:23.265998 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)  1290143 2024-05-20 17:14:23.000000 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards/static/scripts.js
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2024-05-20 17:14:23.269998 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      333 2024-05-20 17:14:23.000000 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      422 2024-05-20 17:14:23.000000 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2024-05-20 17:14:23.000000 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       73 2024-05-20 17:14:23.000000 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       31 2024-05-20 17:14:23.000000 buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2024-05-20 17:14:23.269998 buildbot_react_wsgi_dashboards-3.11.3/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1670 2024-05-20 17:08:54.000000 buildbot_react_wsgi_dashboards-3.11.3/setup.py
```

### Comparing `buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards/__init__.py` & `buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot_react_wsgi_dashboards-3.11.2/buildbot_react_wsgi_dashboards/static/scripts.js` & `buildbot_react_wsgi_dashboards-3.11.3/buildbot_react_wsgi_dashboards/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot_react_wsgi_dashboards-3.11.2/setup.py` & `buildbot_react_wsgi_dashboards-3.11.3/setup.py`

 * *Files identical despite different names*


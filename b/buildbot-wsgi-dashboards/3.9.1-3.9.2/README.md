# Comparing `tmp/buildbot-wsgi-dashboards-3.9.1.tar.gz` & `tmp/buildbot-wsgi-dashboards-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-wsgi-dashboards-3.9.1.tar", last modified: Sat Sep  2 16:04:24 2023, max compression
+gzip compressed data, was "buildbot-wsgi-dashboards-3.9.2.tar", last modified: Sat Sep  2 20:52:37 2023, max compression
```

## Comparing `buildbot-wsgi-dashboards-3.9.1.tar` & `buildbot-wsgi-dashboards-3.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:24.981721 buildbot-wsgi-dashboards-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      319 2023-09-02 16:04:24.981721 buildbot-wsgi-dashboards-3.9.1/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:24.981721 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 16:04:24.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1615 2023-09-02 16:00:07.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:24.981721 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2025 2023-09-02 16:04:24.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8307 2023-09-02 16:04:24.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/static/scripts.js.map
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:24.981721 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      319 2023-09-02 16:04:24.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      421 2023-09-02 16:04:24.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:04:24.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       61 2023-09-02 16:04:24.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       25 2023-09-02 16:04:24.000000 buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 16:04:24.981721 buildbot-wsgi-dashboards-3.9.1/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1609 2023-09-02 16:00:07.000000 buildbot-wsgi-dashboards-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.323030 buildbot-wsgi-dashboards-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      319 2023-09-02 20:52:37.323030 buildbot-wsgi-dashboards-3.9.2/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.323030 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 20:52:37.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1615 2023-09-02 20:48:25.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.323030 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2025 2023-09-02 20:52:37.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8307 2023-09-02 20:52:37.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/static/scripts.js.map
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.323030 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      319 2023-09-02 20:52:37.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      421 2023-09-02 20:52:37.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:52:37.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       61 2023-09-02 20:52:37.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       25 2023-09-02 20:52:37.000000 buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 20:52:37.323030 buildbot-wsgi-dashboards-3.9.2/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1609 2023-09-02 20:48:25.000000 buildbot-wsgi-dashboards-3.9.2/setup.py
```

### Comparing `buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/__init__.py` & `buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/static/scripts.js` & `buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-wsgi-dashboards-3.9.1/buildbot_wsgi_dashboards/static/scripts.js.map` & `buildbot-wsgi-dashboards-3.9.2/buildbot_wsgi_dashboards/static/scripts.js.map`

 * *Files identical despite different names*

### Comparing `buildbot-wsgi-dashboards-3.9.1/setup.py` & `buildbot-wsgi-dashboards-3.9.2/setup.py`

 * *Files identical despite different names*


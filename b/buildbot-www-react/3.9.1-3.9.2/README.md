# Comparing `tmp/buildbot-www-react-3.9.1.tar.gz` & `tmp/buildbot-www-react-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-www-react-3.9.1.tar", last modified: Sat Sep  2 16:03:37 2023, max compression
+gzip compressed data, was "buildbot-www-react-3.9.2.tar", last modified: Sat Sep  2 20:51:49 2023, max compression
```

## Comparing `buildbot-www-react-3.9.1.tar` & `buildbot-www-react-3.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:37.597146 buildbot-www-react-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      258 2023-09-02 16:03:37.597146 buildbot-www-react-3.9.1/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:37.597146 buildbot-www-react-3.9.1/buildbot_www_react/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      855 2023-09-02 16:00:07.000000 buildbot-www-react-3.9.1/buildbot_www_react/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:37.597146 buildbot-www-react-3.9.1/buildbot_www_react/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      755 2023-09-02 16:03:36.000000 buildbot-www-react-3.9.1/buildbot_www_react/static/browser-warning-list.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1411 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react/static/browser-warning.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    28827 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react/static/browser-warning.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21460 2023-09-02 16:03:36.000000 buildbot-www-react-3.9.1/buildbot_www_react/static/icon.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1180 2023-09-02 16:03:36.000000 buildbot-www-react-3.9.1/buildbot_www_react/static/icon.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      953 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react/static/index.html
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      393 2023-09-02 16:03:36.000000 buildbot-www-react-3.9.1/buildbot_www_react/static/manifest.json
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       67 2023-09-02 16:03:36.000000 buildbot-www-react-3.9.1/buildbot_www_react/static/robots.txt
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:03:37.597146 buildbot-www-react-3.9.1/buildbot_www_react.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      258 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      655 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       50 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        9 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-09-02 16:03:37.000000 buildbot-www-react-3.9.1/buildbot_www_react.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 16:03:37.597146 buildbot-www-react-3.9.1/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1714 2023-09-02 16:00:07.000000 buildbot-www-react-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:51:49.131078 buildbot-www-react-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      258 2023-09-02 20:51:49.131078 buildbot-www-react-3.9.2/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:51:49.127078 buildbot-www-react-3.9.2/buildbot_www_react/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 20:51:49.000000 buildbot-www-react-3.9.2/buildbot_www_react/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      855 2023-09-02 20:48:25.000000 buildbot-www-react-3.9.2/buildbot_www_react/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:51:49.131078 buildbot-www-react-3.9.2/buildbot_www_react/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      755 2023-09-02 20:51:48.000000 buildbot-www-react-3.9.2/buildbot_www_react/static/browser-warning-list.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1411 2023-09-02 20:51:48.000000 buildbot-www-react-3.9.2/buildbot_www_react/static/browser-warning.css
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    28827 2023-09-02 20:51:48.000000 buildbot-www-react-3.9.2/buildbot_www_react/static/browser-warning.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21460 2023-09-02 20:51:48.000000 buildbot-www-react-3.9.2/buildbot_www_react/static/icon.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1180 2023-09-02 20:51:48.000000 buildbot-www-react-3.9.2/buildbot_www_react/static/icon.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      953 2023-09-02 20:51:48.000000 buildbot-www-react-3.9.2/buildbot_www_react/static/index.html
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      393 2023-09-02 20:51:48.000000 buildbot-www-react-3.9.2/buildbot_www_react/static/manifest.json
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       67 2023-09-02 20:51:48.000000 buildbot-www-react-3.9.2/buildbot_www_react/static/robots.txt
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:51:49.131078 buildbot-www-react-3.9.2/buildbot_www_react.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      258 2023-09-02 20:51:49.000000 buildbot-www-react-3.9.2/buildbot_www_react.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      655 2023-09-02 20:51:49.000000 buildbot-www-react-3.9.2/buildbot_www_react.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:51:49.000000 buildbot-www-react-3.9.2/buildbot_www_react.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       50 2023-09-02 20:51:49.000000 buildbot-www-react-3.9.2/buildbot_www_react.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        9 2023-09-02 20:51:49.000000 buildbot-www-react-3.9.2/buildbot_www_react.egg-info/requires.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-09-02 20:51:49.000000 buildbot-www-react-3.9.2/buildbot_www_react.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 20:51:49.131078 buildbot-www-react-3.9.2/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1714 2023-09-02 20:48:25.000000 buildbot-www-react-3.9.2/setup.py
```

### Comparing `buildbot-www-react-3.9.1/buildbot_www_react/__init__.py` & `buildbot-www-react-3.9.2/buildbot_www_react/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.9.1/buildbot_www_react/static/browser-warning-list.js` & `buildbot-www-react-3.9.2/buildbot_www_react/static/browser-warning-list.js`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.9.1/buildbot_www_react/static/browser-warning.css` & `buildbot-www-react-3.9.2/buildbot_www_react/static/browser-warning.css`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.9.1/buildbot_www_react/static/browser-warning.js` & `buildbot-www-react-3.9.2/buildbot_www_react/static/browser-warning.js`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.9.1/buildbot_www_react/static/icon.png` & `buildbot-www-react-3.9.2/buildbot_www_react/static/icon.png`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.9.1/buildbot_www_react/static/icon.svg` & `buildbot-www-react-3.9.2/buildbot_www_react/static/icon.svg`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.9.1/buildbot_www_react/static/index.html` & `buildbot-www-react-3.9.2/buildbot_www_react/static/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <meta charset="utf-8" />
     <meta name="viewport" content="initial-scale=1, minimum-scale=1, user-scalable=no, maximum-scale=1, width=device-width">
     <meta name="theme-color" content="#000000" />
     <meta name="description" content="Buildbot Web UI"/>
     <link id="bbicon" href="/icon.png" rel="icon">
     <link href="/icon.svg" title="Buildbot" rel="fluid-icon">
     <title>Buildbot</title>
-    <script type="module" crossorigin src="/assets/index-06fa64ba.js"></script>
+    <script type="module" crossorigin src="/assets/index-2bd42961.js"></script>
     <link rel="stylesheet" href="/assets/index-b264164c.css">
   </head>
   <body>
     <div id="outdated"></div>
     <noscript>You need to enable JavaScript to view this website.</noscript>
     <div id="root"></div>
   </body>
```

### Comparing `buildbot-www-react-3.9.1/buildbot_www_react.egg-info/SOURCES.txt` & `buildbot-www-react-3.9.2/buildbot_www_react.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildbot-www-react-3.9.1/setup.py` & `buildbot-www-react-3.9.2/setup.py`

 * *Files identical despite different names*


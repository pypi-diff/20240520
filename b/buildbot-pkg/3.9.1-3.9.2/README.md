# Comparing `tmp/buildbot-pkg-3.9.1.tar.gz` & `tmp/buildbot-pkg-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-pkg-3.9.1.tar", last modified: Sat Sep  2 16:02:33 2023, max compression
+gzip compressed data, was "buildbot-pkg-3.9.2.tar", last modified: Sat Sep  2 20:50:42 2023, max compression
```

## Comparing `buildbot-pkg-3.9.1.tar` & `buildbot-pkg-3.9.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:33.388367 buildbot-pkg-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      251 2023-09-02 16:02:33.388367 buildbot-pkg-3.9.1/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1292 2023-09-02 16:00:07.000000 buildbot-pkg-3.9.1/README
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:02:33.388367 buildbot-pkg-3.9.1/buildbot_pkg.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      251 2023-09-02 16:02:33.000000 buildbot-pkg-3.9.1/buildbot_pkg.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      220 2023-09-02 16:02:33.000000 buildbot-pkg-3.9.1/buildbot_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:02:33.000000 buildbot-pkg-3.9.1/buildbot_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-09-02 16:02:33.000000 buildbot-pkg-3.9.1/buildbot_pkg.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       13 2023-09-02 16:02:33.000000 buildbot-pkg-3.9.1/buildbot_pkg.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8595 2023-09-02 16:00:07.000000 buildbot-pkg-3.9.1/buildbot_pkg.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 16:02:33.388367 buildbot-pkg-3.9.1/setup.cfg
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     1194 2023-09-02 16:00:07.000000 buildbot-pkg-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:42.111142 buildbot-pkg-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      251 2023-09-02 20:50:42.111142 buildbot-pkg-3.9.2/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1292 2023-09-02 20:48:25.000000 buildbot-pkg-3.9.2/README
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:50:42.111142 buildbot-pkg-3.9.2/buildbot_pkg.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      251 2023-09-02 20:50:42.000000 buildbot-pkg-3.9.2/buildbot_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      220 2023-09-02 20:50:42.000000 buildbot-pkg-3.9.2/buildbot_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:50:42.000000 buildbot-pkg-3.9.2/buildbot_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-09-02 20:50:42.000000 buildbot-pkg-3.9.2/buildbot_pkg.egg-info/requires.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       13 2023-09-02 20:50:42.000000 buildbot-pkg-3.9.2/buildbot_pkg.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8595 2023-09-02 20:48:25.000000 buildbot-pkg-3.9.2/buildbot_pkg.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 20:50:42.111142 buildbot-pkg-3.9.2/setup.cfg
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     1194 2023-09-02 20:48:25.000000 buildbot-pkg-3.9.2/setup.py
```

### Comparing `buildbot-pkg-3.9.1/README` & `buildbot-pkg-3.9.2/README`

 * *Files identical despite different names*

### Comparing `buildbot-pkg-3.9.1/buildbot_pkg.py` & `buildbot-pkg-3.9.2/buildbot_pkg.py`

 * *Files identical despite different names*

### Comparing `buildbot-pkg-3.9.1/setup.py` & `buildbot-pkg-3.9.2/setup.py`

 * *Files identical despite different names*


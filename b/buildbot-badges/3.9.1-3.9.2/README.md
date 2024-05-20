# Comparing `tmp/buildbot-badges-3.9.1.tar.gz` & `tmp/buildbot-badges-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot-badges-3.9.1.tar", last modified: Sat Sep  2 16:04:25 2023, max compression
+gzip compressed data, was "buildbot-badges-3.9.2.tar", last modified: Sat Sep  2 20:52:37 2023, max compression
```

## Comparing `buildbot-badges-3.9.1.tar` & `buildbot-badges-3.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:25.357726 buildbot-badges-3.9.1/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      256 2023-09-02 16:04:25.357726 buildbot-badges-3.9.1/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:25.353726 buildbot-badges-3.9.1/buildbot_badges/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 16:04:25.000000 buildbot-badges-3.9.1/buildbot_badges/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5167 2023-09-02 16:00:07.000000 buildbot-badges-3.9.1/buildbot_badges/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:25.357726 buildbot-badges-3.9.1/buildbot_badges/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:00:07.000000 buildbot-badges-3.9.1/buildbot_badges/static/.placeholder
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:25.357726 buildbot-badges-3.9.1/buildbot_badges/templates/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1212 2023-09-02 16:00:07.000000 buildbot-badges-3.9.1/buildbot_badges/templates/badgeio.svg.j2
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      714 2023-09-02 16:00:07.000000 buildbot-badges-3.9.1/buildbot_badges/templates/flat-square.svg.j2
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1480 2023-09-02 16:00:07.000000 buildbot-badges-3.9.1/buildbot_badges/templates/flat.svg.j2
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1574 2023-09-02 16:00:07.000000 buildbot-badges-3.9.1/buildbot_badges/templates/plastic.svg.j2
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 16:04:25.357726 buildbot-badges-3.9.1/buildbot_badges.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      256 2023-09-02 16:04:25.000000 buildbot-badges-3.9.1/buildbot_badges.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      507 2023-09-02 16:04:25.000000 buildbot-badges-3.9.1/buildbot_badges.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 16:04:25.000000 buildbot-badges-3.9.1/buildbot_badges.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       43 2023-09-02 16:04:25.000000 buildbot-badges-3.9.1/buildbot_badges.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       32 2023-09-02 16:04:25.000000 buildbot-badges-3.9.1/buildbot_badges.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       16 2023-09-02 16:04:25.000000 buildbot-badges-3.9.1/buildbot_badges.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 16:04:25.357726 buildbot-badges-3.9.1/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1684 2023-09-02 16:00:07.000000 buildbot-badges-3.9.1/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.711030 buildbot-badges-3.9.2/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      256 2023-09-02 20:52:37.711030 buildbot-badges-3.9.2/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.707030 buildbot-badges-3.9.2/buildbot_badges/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-09-02 20:52:37.000000 buildbot-badges-3.9.2/buildbot_badges/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5167 2023-09-02 20:48:25.000000 buildbot-badges-3.9.2/buildbot_badges/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.707030 buildbot-badges-3.9.2/buildbot_badges/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:48:25.000000 buildbot-badges-3.9.2/buildbot_badges/static/.placeholder
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.711030 buildbot-badges-3.9.2/buildbot_badges/templates/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1212 2023-09-02 20:48:25.000000 buildbot-badges-3.9.2/buildbot_badges/templates/badgeio.svg.j2
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      714 2023-09-02 20:48:25.000000 buildbot-badges-3.9.2/buildbot_badges/templates/flat-square.svg.j2
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1480 2023-09-02 20:48:25.000000 buildbot-badges-3.9.2/buildbot_badges/templates/flat.svg.j2
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1574 2023-09-02 20:48:25.000000 buildbot-badges-3.9.2/buildbot_badges/templates/plastic.svg.j2
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-09-02 20:52:37.707030 buildbot-badges-3.9.2/buildbot_badges.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      256 2023-09-02 20:52:37.000000 buildbot-badges-3.9.2/buildbot_badges.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      507 2023-09-02 20:52:37.000000 buildbot-badges-3.9.2/buildbot_badges.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-09-02 20:52:37.000000 buildbot-badges-3.9.2/buildbot_badges.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       43 2023-09-02 20:52:37.000000 buildbot-badges-3.9.2/buildbot_badges.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       32 2023-09-02 20:52:37.000000 buildbot-badges-3.9.2/buildbot_badges.egg-info/requires.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       16 2023-09-02 20:52:37.000000 buildbot-badges-3.9.2/buildbot_badges.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-09-02 20:52:37.711030 buildbot-badges-3.9.2/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1684 2023-09-02 20:48:25.000000 buildbot-badges-3.9.2/setup.py
```

### Comparing `buildbot-badges-3.9.1/buildbot_badges/__init__.py` & `buildbot-badges-3.9.2/buildbot_badges/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.9.1/buildbot_badges/templates/badgeio.svg.j2` & `buildbot-badges-3.9.2/buildbot_badges/templates/badgeio.svg.j2`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.9.1/buildbot_badges/templates/flat-square.svg.j2` & `buildbot-badges-3.9.2/buildbot_badges/templates/flat-square.svg.j2`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.9.1/buildbot_badges/templates/flat.svg.j2` & `buildbot-badges-3.9.2/buildbot_badges/templates/flat.svg.j2`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.9.1/buildbot_badges/templates/plastic.svg.j2` & `buildbot-badges-3.9.2/buildbot_badges/templates/plastic.svg.j2`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.9.1/setup.py` & `buildbot-badges-3.9.2/setup.py`

 * *Files identical despite different names*


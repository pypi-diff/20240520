# Comparing `tmp/space_exploration_common_lib-0.0.2.tar.gz` & `tmp/space_exploration_common_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_exploration_common_lib-0.0.2.tar", last modified: Mon May 20 18:14:38 2024, max compression
+gzip compressed data, was "space_exploration_common_lib-0.0.3.tar", last modified: Mon May 20 18:18:37 2024, max compression
```

## Comparing `space_exploration_common_lib-0.0.2.tar` & `space_exploration_common_lib-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 18:14:38.072188 space_exploration_common_lib-0.0.2/
--rw-rw-rw-   0        0        0      198 2024-05-20 18:14:38.071190 space_exploration_common_lib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-20 17:41:39.000000 space_exploration_common_lib-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-20 18:14:38.072188 space_exploration_common_lib-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      420 2024-05-20 18:14:29.000000 space_exploration_common_lib-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:14:38.070187 space_exploration_common_lib-0.0.2/space_exploration_common_lib.egg-info/
--rw-rw-rw-   0        0        0      198 2024-05-20 18:14:38.000000 space_exploration_common_lib-0.0.2/space_exploration_common_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      610 2024-05-20 18:14:38.000000 space_exploration_common_lib-0.0.2/space_exploration_common_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 18:14:38.000000 space_exploration_common_lib-0.0.2/space_exploration_common_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-20 18:14:38.000000 space_exploration_common_lib-0.0.2/space_exploration_common_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-20 18:14:38.000000 space_exploration_common_lib-0.0.2/space_exploration_common_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 18:14:38.061665 space_exploration_common_lib-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2024-05-20 17:40:57.000000 space_exploration_common_lib-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:14:38.063267 space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/
--rw-rw-rw-   0        0        0        0 2024-05-20 18:11:49.000000 space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:14:38.065275 space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/model/
--rw-rw-rw-   0        0        0      131 2024-05-20 15:14:54.000000 space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/model/Duration.py
--rw-rw-rw-   0        0        0        0 2024-05-20 17:46:56.000000 space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:14:38.067178 space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/model/mission/
--rw-rw-rw-   0        0        0      620 2024-05-20 16:03:47.000000 space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/model/mission/ProjectMercury.py
--rw-rw-rw-   0        0        0        0 2024-05-20 17:47:10.000000 space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/model/mission/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 18:14:38.069187 space_exploration_common_lib-0.0.2/src/tests/
--rw-rw-rw-   0        0        0        0 2024-05-20 17:41:09.000000 space_exploration_common_lib-0.0.2/src/tests/__init__.py
--rw-rw-rw-   0        0        0      112 2024-05-18 00:22:21.000000 space_exploration_common_lib-0.0.2/src/tests/test_dummy.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:18:37.035383 space_exploration_common_lib-0.0.3/
+-rw-rw-rw-   0        0        0      198 2024-05-20 18:18:37.034383 space_exploration_common_lib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-05-20 17:41:39.000000 space_exploration_common_lib-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 18:18:37.035383 space_exploration_common_lib-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-05-20 18:17:52.000000 space_exploration_common_lib-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:18:37.033383 space_exploration_common_lib-0.0.3/space_exploration_common_lib.egg-info/
+-rw-rw-rw-   0        0        0      198 2024-05-20 18:18:36.000000 space_exploration_common_lib-0.0.3/space_exploration_common_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2024-05-20 18:18:37.000000 space_exploration_common_lib-0.0.3/space_exploration_common_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 18:18:36.000000 space_exploration_common_lib-0.0.3/space_exploration_common_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-20 18:18:36.000000 space_exploration_common_lib-0.0.3/space_exploration_common_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-20 18:18:36.000000 space_exploration_common_lib-0.0.3/space_exploration_common_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 18:18:37.025381 space_exploration_common_lib-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2024-05-20 17:40:57.000000 space_exploration_common_lib-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:18:37.026381 space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/
+-rw-rw-rw-   0        0        0        0 2024-05-20 18:11:49.000000 space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:18:37.028381 space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/model/
+-rw-rw-rw-   0        0        0      131 2024-05-20 15:14:54.000000 space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/model/Duration.py
+-rw-rw-rw-   0        0        0        0 2024-05-20 17:46:56.000000 space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:18:37.030381 space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/model/mission/
+-rw-rw-rw-   0        0        0      620 2024-05-20 16:03:47.000000 space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/model/mission/ProjectMercury.py
+-rw-rw-rw-   0        0        0        0 2024-05-20 17:47:10.000000 space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/model/mission/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:18:37.032385 space_exploration_common_lib-0.0.3/src/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-20 17:41:09.000000 space_exploration_common_lib-0.0.3/src/tests/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-05-18 00:22:21.000000 space_exploration_common_lib-0.0.3/src/tests/test_dummy.py
```

### Comparing `space_exploration_common_lib-0.0.2/space_exploration_common_lib.egg-info/SOURCES.txt` & `space_exploration_common_lib-0.0.3/space_exploration_common_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `space_exploration_common_lib-0.0.2/src/space_exploration_common_lib/model/mission/ProjectMercury.py` & `space_exploration_common_lib-0.0.3/src/space_exploration_common_lib/model/mission/ProjectMercury.py`

 * *Files identical despite different names*


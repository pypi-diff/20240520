# Comparing `tmp/jzai-59.83.48.tar.gz` & `tmp/jzai-59.83.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.48.tar", last modified: Mon May 20 08:35:24 2024, max compression
+gzip compressed data, was "jzai-59.83.49.tar", last modified: Mon May 20 08:36:47 2024, max compression
```

## Comparing `jzai-59.83.48.tar` & `jzai-59.83.49.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:35:24.633446 jzai-59.83.48/
--rw-rw-rw-   0        0        0      275 2024-05-20 08:35:24.632238 jzai-59.83.48/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.48/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 08:35:24.605763 jzai-59.83.48/jzai/
--rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.48/jzai/__init__.py
--rw-rw-rw-   0        0        0     9373 2024-05-20 08:33:38.000000 jzai-59.83.48/jzai/bot.py
--rw-rw-rw-   0        0        0      273 2024-05-20 08:35:14.000000 jzai-59.83.48/jzai/cli.py
--rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.48/jzai/db.py
--rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.48/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:35:24.630692 jzai-59.83.48/jzai.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-20 08:35:24.000000 jzai-59.83.48/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 08:35:24.000000 jzai-59.83.48/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:35:24.000000 jzai-59.83.48/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-20 08:35:24.000000 jzai-59.83.48/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-05-20 08:35:24.000000 jzai-59.83.48/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 08:35:24.000000 jzai-59.83.48/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 08:35:24.634861 jzai-59.83.48/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-20 08:35:20.000000 jzai-59.83.48/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:36:47.660839 jzai-59.83.49/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:36:47.659633 jzai-59.83.49/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.49/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:36:47.640960 jzai-59.83.49/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:34:39.000000 jzai-59.83.49/jzai/__init__.py
+-rw-rw-rw-   0        0        0     9373 2024-05-20 08:33:38.000000 jzai-59.83.49/jzai/bot.py
+-rw-rw-rw-   0        0        0      199 2024-05-20 08:36:28.000000 jzai-59.83.49/jzai/cli.py
+-rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.49/jzai/db.py
+-rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.49/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:36:47.657635 jzai-59.83.49/jzai.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 08:36:47.000000 jzai-59.83.49/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:36:47.660839 jzai-59.83.49/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-20 08:36:45.000000 jzai-59.83.49/setup.py
```

### Comparing `jzai-59.83.48/jzai/bot.py` & `jzai-59.83.49/jzai/bot.py`

 * *Files identical despite different names*

### Comparing `jzai-59.83.48/jzai/db.py` & `jzai-59.83.49/jzai/db.py`

 * *Files identical despite different names*


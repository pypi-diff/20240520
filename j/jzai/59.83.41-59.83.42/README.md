# Comparing `tmp/jzai-59.83.41.tar.gz` & `tmp/jzai-59.83.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.41.tar", last modified: Mon May 20 03:17:44 2024, max compression
+gzip compressed data, was "jzai-59.83.42.tar", last modified: Mon May 20 03:17:51 2024, max compression
```

## Comparing `jzai-59.83.41.tar` & `jzai-59.83.42.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 03:17:44.272604 jzai-59.83.41/
--rw-rw-rw-   0        0        0      226 2024-05-20 03:17:44.268605 jzai-59.83.41/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.41/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 03:17:44.200791 jzai-59.83.41/jzai/
--rw-rw-rw-   0        0        0       58 2024-05-17 02:22:27.000000 jzai-59.83.41/jzai/__init__.py
--rw-rw-rw-   0        0        0     8770 2024-05-20 03:17:35.000000 jzai-59.83.41/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-17 02:23:18.000000 jzai-59.83.41/jzai/cli.py
--rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.41/jzai/db.py
--rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.41/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 03:17:44.265591 jzai-59.83.41/jzai.egg-info/
--rw-rw-rw-   0        0        0      226 2024-05-20 03:17:43.000000 jzai-59.83.41/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 03:17:44.000000 jzai-59.83.41/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 03:17:43.000000 jzai-59.83.41/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-20 03:17:43.000000 jzai-59.83.41/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-20 03:17:43.000000 jzai-59.83.41/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 03:17:43.000000 jzai-59.83.41/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 03:17:44.273604 jzai-59.83.41/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-05-20 03:14:41.000000 jzai-59.83.41/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:17:51.235938 jzai-59.83.42/
+-rw-rw-rw-   0        0        0      226 2024-05-20 03:17:51.233255 jzai-59.83.42/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.42/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 03:17:51.185450 jzai-59.83.42/jzai/
+-rw-rw-rw-   0        0        0       58 2024-05-17 02:22:27.000000 jzai-59.83.42/jzai/__init__.py
+-rw-rw-rw-   0        0        0     8770 2024-05-20 03:17:35.000000 jzai-59.83.42/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-17 02:23:18.000000 jzai-59.83.42/jzai/cli.py
+-rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.42/jzai/db.py
+-rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.42/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:17:51.230842 jzai-59.83.42/jzai.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 03:17:51.000000 jzai-59.83.42/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 03:17:51.235938 jzai-59.83.42/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-20 03:17:48.000000 jzai-59.83.42/setup.py
```

### Comparing `jzai-59.83.41/jzai/bot.py` & `jzai-59.83.42/jzai/bot.py`

 * *Files identical despite different names*

### Comparing `jzai-59.83.41/jzai/db.py` & `jzai-59.83.42/jzai/db.py`

 * *Files identical despite different names*


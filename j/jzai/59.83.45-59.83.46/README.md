# Comparing `tmp/jzai-59.83.45.tar.gz` & `tmp/jzai-59.83.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.45.tar", last modified: Mon May 20 08:26:51 2024, max compression
+gzip compressed data, was "jzai-59.83.46.tar", last modified: Mon May 20 08:29:09 2024, max compression
```

## Comparing `jzai-59.83.45.tar` & `jzai-59.83.46.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:26:51.992477 jzai-59.83.45/
--rw-rw-rw-   0        0        0      275 2024-05-20 08:26:51.991155 jzai-59.83.45/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.45/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 08:26:51.962967 jzai-59.83.45/jzai/
--rw-rw-rw-   0        0        0       26 2024-05-20 08:26:37.000000 jzai-59.83.45/jzai/__init__.py
--rw-rw-rw-   0        0        0     9366 2024-05-20 08:20:05.000000 jzai-59.83.45/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-17 02:23:18.000000 jzai-59.83.45/jzai/cli.py
--rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.45/jzai/db.py
--rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.45/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:26:51.988414 jzai-59.83.45/jzai.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-20 08:26:51.000000 jzai-59.83.45/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 08:26:51.000000 jzai-59.83.45/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:26:51.000000 jzai-59.83.45/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-20 08:26:51.000000 jzai-59.83.45/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-05-20 08:26:51.000000 jzai-59.83.45/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 08:26:51.000000 jzai-59.83.45/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 08:26:51.992477 jzai-59.83.45/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-20 08:26:45.000000 jzai-59.83.45/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:29:09.255979 jzai-59.83.46/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:29:09.254660 jzai-59.83.46/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.46/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:29:09.231903 jzai-59.83.46/jzai/
+-rw-rw-rw-   0        0        0       24 2024-05-20 08:27:39.000000 jzai-59.83.46/jzai/__init__.py
+-rw-rw-rw-   0        0        0     9366 2024-05-20 08:20:05.000000 jzai-59.83.46/jzai/bot.py
+-rw-rw-rw-   0        0        0      266 2024-05-20 08:28:47.000000 jzai-59.83.46/jzai/cli.py
+-rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.46/jzai/db.py
+-rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.46/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:29:09.253199 jzai-59.83.46/jzai.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:29:09.255979 jzai-59.83.46/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-20 08:29:05.000000 jzai-59.83.46/setup.py
```

### Comparing `jzai-59.83.45/jzai/bot.py` & `jzai-59.83.46/jzai/bot.py`

 * *Files identical despite different names*

### Comparing `jzai-59.83.45/jzai/db.py` & `jzai-59.83.46/jzai/db.py`

 * *Files identical despite different names*


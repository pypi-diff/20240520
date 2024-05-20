# Comparing `tmp/mountain_chicken-0.1.5.tar.gz` & `tmp/mountain_chicken-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountain_chicken-0.1.5.tar", last modified: Mon May 20 08:54:53 2024, max compression
+gzip compressed data, was "mountain_chicken-0.1.6.tar", last modified: Mon May 20 09:00:43 2024, max compression
```

## Comparing `mountain_chicken-0.1.5.tar` & `mountain_chicken-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:54:53.387762 mountain_chicken-0.1.5/
--rw-rw-rw-   0        0        0       63 2024-05-20 08:54:53.387262 mountain_chicken-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       29 2024-05-13 15:05:37.000000 mountain_chicken-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 08:54:53.380133 mountain_chicken-0.1.5/mountain_chicken/
--rw-rw-rw-   0        0        0      102 2024-05-20 08:54:12.000000 mountain_chicken-0.1.5/mountain_chicken/__init__.py
--rw-rw-rw-   0        0        0     2542 2024-05-20 08:53:23.000000 mountain_chicken-0.1.5/mountain_chicken/base.py
--rw-rw-rw-   0        0        0      953 2024-05-20 08:52:38.000000 mountain_chicken-0.1.5/mountain_chicken/double_dict.py
--rw-rw-rw-   0        0        0      656 2024-05-20 08:53:35.000000 mountain_chicken-0.1.5/mountain_chicken/mutable_string.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:54:53.386763 mountain_chicken-0.1.5/mountain_chicken.egg-info/
--rw-rw-rw-   0        0        0       63 2024-05-20 08:54:53.000000 mountain_chicken-0.1.5/mountain_chicken.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-05-20 08:54:53.000000 mountain_chicken-0.1.5/mountain_chicken.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:54:53.000000 mountain_chicken-0.1.5/mountain_chicken.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-20 08:54:53.000000 mountain_chicken-0.1.5/mountain_chicken.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 08:54:53.388261 mountain_chicken-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      202 2024-05-20 08:54:20.000000 mountain_chicken-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:00:43.653757 mountain_chicken-0.1.6/
+-rw-rw-rw-   0        0        0       63 2024-05-20 09:00:43.653258 mountain_chicken-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2024-05-13 15:05:37.000000 mountain_chicken-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 09:00:43.645758 mountain_chicken-0.1.6/mountain_chicken/
+-rw-rw-rw-   0        0        0      102 2024-05-20 08:56:55.000000 mountain_chicken-0.1.6/mountain_chicken/__init__.py
+-rw-rw-rw-   0        0        0     2542 2024-05-20 08:53:23.000000 mountain_chicken-0.1.6/mountain_chicken/base.py
+-rw-rw-rw-   0        0        0      953 2024-05-20 08:52:38.000000 mountain_chicken-0.1.6/mountain_chicken/double_dict.py
+-rw-rw-rw-   0        0        0      656 2024-05-20 08:53:35.000000 mountain_chicken-0.1.6/mountain_chicken/mutable_string.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:00:43.652758 mountain_chicken-0.1.6/mountain_chicken.egg-info/
+-rw-rw-rw-   0        0        0       63 2024-05-20 09:00:43.000000 mountain_chicken-0.1.6/mountain_chicken.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-20 09:00:43.000000 mountain_chicken-0.1.6/mountain_chicken.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:00:43.000000 mountain_chicken-0.1.6/mountain_chicken.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 09:00:43.000000 mountain_chicken-0.1.6/mountain_chicken.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 09:00:43.654257 mountain_chicken-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      202 2024-05-20 09:00:22.000000 mountain_chicken-0.1.6/setup.py
```

### Comparing `mountain_chicken-0.1.5/mountain_chicken/base.py` & `mountain_chicken-0.1.6/mountain_chicken/base.py`

 * *Files identical despite different names*

### Comparing `mountain_chicken-0.1.5/mountain_chicken/double_dict.py` & `mountain_chicken-0.1.6/mountain_chicken/double_dict.py`

 * *Files identical despite different names*

### Comparing `mountain_chicken-0.1.5/mountain_chicken/mutable_string.py` & `mountain_chicken-0.1.6/mountain_chicken/mutable_string.py`

 * *Files identical despite different names*


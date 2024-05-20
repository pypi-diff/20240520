# Comparing `tmp/mountain_chicken-0.1.3.tar.gz` & `tmp/mountain_chicken-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountain_chicken-0.1.3.tar", last modified: Sat May 18 17:21:59 2024, max compression
+gzip compressed data, was "mountain_chicken-0.1.4.tar", last modified: Mon May 20 08:46:37 2024, max compression
```

## Comparing `mountain_chicken-0.1.3.tar` & `mountain_chicken-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 17:21:59.261936 mountain_chicken-0.1.3/
--rw-rw-rw-   0        0        0       63 2024-05-18 17:21:59.261436 mountain_chicken-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       29 2024-05-13 15:05:37.000000 mountain_chicken-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 17:21:59.257439 mountain_chicken-0.1.3/mountain_chicken/
--rw-rw-rw-   0        0        0       37 2024-05-16 12:52:50.000000 mountain_chicken-0.1.3/mountain_chicken/__init__.py
--rw-rw-rw-   0        0        0     2580 2024-05-18 17:21:49.000000 mountain_chicken-0.1.3/mountain_chicken/base.py
--rw-rw-rw-   0        0        0      954 2024-05-13 19:08:16.000000 mountain_chicken-0.1.3/mountain_chicken/double_dict.py
--rw-rw-rw-   0        0        0      658 2024-05-16 12:49:31.000000 mountain_chicken-0.1.3/mountain_chicken/mutable_string.py
-drwxrwxrwx   0        0        0        0 2024-05-18 17:21:59.260435 mountain_chicken-0.1.3/mountain_chicken.egg-info/
--rw-rw-rw-   0        0        0       63 2024-05-18 17:21:59.000000 mountain_chicken-0.1.3/mountain_chicken.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-05-18 17:21:59.000000 mountain_chicken-0.1.3/mountain_chicken.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 17:21:59.000000 mountain_chicken-0.1.3/mountain_chicken.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-18 17:21:59.000000 mountain_chicken-0.1.3/mountain_chicken.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 17:21:59.261936 mountain_chicken-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      202 2024-05-18 17:21:48.000000 mountain_chicken-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:46:37.270873 mountain_chicken-0.1.4/
+-rw-rw-rw-   0        0        0       63 2024-05-20 08:46:37.270373 mountain_chicken-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2024-05-13 15:05:37.000000 mountain_chicken-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:46:37.259372 mountain_chicken-0.1.4/mountain_chicken/
+-rw-rw-rw-   0        0        0      104 2024-05-19 20:07:34.000000 mountain_chicken-0.1.4/mountain_chicken/__init__.py
+-rw-rw-rw-   0        0        0     2580 2024-05-18 17:21:49.000000 mountain_chicken-0.1.4/mountain_chicken/base.py
+-rw-rw-rw-   0        0        0      954 2024-05-13 19:08:16.000000 mountain_chicken-0.1.4/mountain_chicken/double_dict.py
+-rw-rw-rw-   0        0        0      658 2024-05-16 12:49:31.000000 mountain_chicken-0.1.4/mountain_chicken/mutable_string.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:46:37.269874 mountain_chicken-0.1.4/mountain_chicken.egg-info/
+-rw-rw-rw-   0        0        0       63 2024-05-20 08:46:37.000000 mountain_chicken-0.1.4/mountain_chicken.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-20 08:46:37.000000 mountain_chicken-0.1.4/mountain_chicken.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:46:37.000000 mountain_chicken-0.1.4/mountain_chicken.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 08:46:37.000000 mountain_chicken-0.1.4/mountain_chicken.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:46:37.270873 mountain_chicken-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      202 2024-05-20 08:46:16.000000 mountain_chicken-0.1.4/setup.py
```

### Comparing `mountain_chicken-0.1.3/mountain_chicken/base.py` & `mountain_chicken-0.1.4/mountain_chicken/base.py`

 * *Files identical despite different names*

### Comparing `mountain_chicken-0.1.3/mountain_chicken/double_dict.py` & `mountain_chicken-0.1.4/mountain_chicken/double_dict.py`

 * *Files identical despite different names*

### Comparing `mountain_chicken-0.1.3/mountain_chicken/mutable_string.py` & `mountain_chicken-0.1.4/mountain_chicken/mutable_string.py`

 * *Files identical despite different names*


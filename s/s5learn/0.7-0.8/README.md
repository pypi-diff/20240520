# Comparing `tmp/s5learn-0.7.tar.gz` & `tmp/s5learn-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5learn-0.7.tar", last modified: Sun May 19 22:37:48 2024, max compression
+gzip compressed data, was "s5learn-0.8.tar", last modified: Sun May 19 22:44:20 2024, max compression
```

## Comparing `s5learn-0.7.tar` & `s5learn-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 22:37:48.476127 s5learn-0.7/
--rw-rw-rw-   0        0        0       52 2024-05-19 22:37:48.476127 s5learn-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 22:37:48.464301 s5learn-0.7/s5learn/
--rw-rw-rw-   0        0        0      396 2024-05-19 22:37:24.000000 s5learn-0.7/s5learn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 22:37:48.476127 s5learn-0.7/s5learn/data/
--rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.7/s5learn/data/example.txt
--rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.7/s5learn/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 22:37:48.476127 s5learn-0.7/s5learn.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-19 22:37:48.000000 s5learn-0.7/s5learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-05-19 22:37:48.000000 s5learn-0.7/s5learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 22:37:48.000000 s5learn-0.7/s5learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 22:37:48.000000 s5learn-0.7/s5learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 22:37:48.476127 s5learn-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1817 2024-05-19 22:37:24.000000 s5learn-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:44:20.641503 s5learn-0.8/
+-rw-rw-rw-   0        0        0       52 2024-05-19 22:44:20.641503 s5learn-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 22:44:20.625879 s5learn-0.8/s5learn/
+-rw-rw-rw-   0        0        0      340 2024-05-19 22:43:52.000000 s5learn-0.8/s5learn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:44:20.641503 s5learn-0.8/s5learn/data/
+-rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.8/s5learn/data/example.txt
+-rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8/s5learn/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:44:20.641503 s5learn-0.8/s5learn.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-19 22:44:20.000000 s5learn-0.8/s5learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-05-19 22:44:20.000000 s5learn-0.8/s5learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 22:44:20.000000 s5learn-0.8/s5learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 22:44:20.000000 s5learn-0.8/s5learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 22:44:20.641503 s5learn-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1817 2024-05-19 22:44:04.000000 s5learn-0.8/setup.py
```

### Comparing `s5learn-0.7/setup.py` & `s5learn-0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='s5learn',
-    version='0.7',
+    version='0.8',
     packages=find_packages(),
     package_data={'': ['data/*.txt']},
 )
 
 
 
 # import setuptools
```


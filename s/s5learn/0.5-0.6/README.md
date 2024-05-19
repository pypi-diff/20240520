# Comparing `tmp/s5learn-0.5.tar.gz` & `tmp/s5learn-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5learn-0.5.tar", last modified: Sun May 19 21:28:51 2024, max compression
+gzip compressed data, was "s5learn-0.6.tar", last modified: Sun May 19 22:20:06 2024, max compression
```

## Comparing `s5learn-0.5.tar` & `s5learn-0.6.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 21:28:51.103974 s5learn-0.5/
--rw-rw-rw-   0        0        0       52 2024-05-19 21:28:51.103974 s5learn-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 21:28:51.088367 s5learn-0.5/s5learn/
--rw-rw-rw-   0        0        0       24 2024-05-19 09:36:27.000000 s5learn-0.5/s5learn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 21:28:51.088367 s5learn-0.5/s5learn/data/
--rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.5/s5learn/data/example.txt
--rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.5/s5learn/main.py
--rw-rw-rw-   0        0        0      197 2024-05-19 20:43:52.000000 s5learn-0.5/s5learn/printtext.py
-drwxrwxrwx   0        0        0        0 2024-05-19 21:28:51.088367 s5learn-0.5/s5learn.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-19 21:28:50.000000 s5learn-0.5/s5learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-19 21:28:50.000000 s5learn-0.5/s5learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 21:28:50.000000 s5learn-0.5/s5learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 21:28:50.000000 s5learn-0.5/s5learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 21:28:51.103974 s5learn-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1817 2024-05-19 21:28:29.000000 s5learn-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:20:06.554152 s5learn-0.6/
+-rw-rw-rw-   0        0        0       52 2024-05-19 22:20:06.546152 s5learn-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 22:20:06.538154 s5learn-0.6/s5learn/
+-rw-rw-rw-   0        0        0      226 2024-05-19 22:19:47.000000 s5learn-0.6/s5learn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:20:06.546152 s5learn-0.6/s5learn/data/
+-rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.6/s5learn/data/example.txt
+-rw-rw-rw-   0        0        0     2753 2024-05-19 22:11:08.000000 s5learn-0.6/s5learn/idp.py
+-rw-rw-rw-   0        0        0     7318 2024-05-19 22:04:34.000000 s5learn-0.6/s5learn/m5.py
+-rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.6/s5learn/main.py
+-rw-rw-rw-   0        0        0     5940 2024-05-19 22:14:34.000000 s5learn-0.6/s5learn/mnv2.py
+-rw-rw-rw-   0        0        0     1394 2024-05-19 22:13:21.000000 s5learn-0.6/s5learn/mnv2_dp.py
+-rw-rw-rw-   0        0        0      979 2024-05-19 22:19:47.000000 s5learn-0.6/s5learn/mnv2_dv.py
+-rw-rw-rw-   0        0        0     2075 2024-05-19 22:06:44.000000 s5learn-0.6/s5learn/ms.py
+-rw-rw-rw-   0        0        0     3935 2024-05-19 22:08:10.000000 s5learn-0.6/s5learn/mv2_train.py
+-rw-rw-rw-   0        0        0     3109 2024-05-19 22:10:02.000000 s5learn-0.6/s5learn/t5.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:20:06.546152 s5learn-0.6/s5learn.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-19 22:20:06.000000 s5learn-0.6/s5learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-19 22:20:06.000000 s5learn-0.6/s5learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 22:20:06.000000 s5learn-0.6/s5learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 22:20:06.000000 s5learn-0.6/s5learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 22:20:06.554152 s5learn-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1817 2024-05-19 22:19:47.000000 s5learn-0.6/setup.py
```

### Comparing `s5learn-0.5/setup.py` & `s5learn-0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='s5learn',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     package_data={'': ['data/*.txt']},
 )
 
 
 
 # import setuptools
```


# Comparing `tmp/s5learn-0.8.tar.gz` & `tmp/s5learn-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5learn-0.8.tar", last modified: Sun May 19 22:44:20 2024, max compression
+gzip compressed data, was "s5learn-0.8.1.tar", last modified: Sun May 19 23:33:43 2024, max compression
```

## Comparing `s5learn-0.8.tar` & `s5learn-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 22:44:20.641503 s5learn-0.8/
--rw-rw-rw-   0        0        0       52 2024-05-19 22:44:20.641503 s5learn-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 22:44:20.625879 s5learn-0.8/s5learn/
--rw-rw-rw-   0        0        0      340 2024-05-19 22:43:52.000000 s5learn-0.8/s5learn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 22:44:20.641503 s5learn-0.8/s5learn/data/
--rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.8/s5learn/data/example.txt
--rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8/s5learn/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 22:44:20.641503 s5learn-0.8/s5learn.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-19 22:44:20.000000 s5learn-0.8/s5learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-05-19 22:44:20.000000 s5learn-0.8/s5learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 22:44:20.000000 s5learn-0.8/s5learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 22:44:20.000000 s5learn-0.8/s5learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 22:44:20.641503 s5learn-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1817 2024-05-19 22:44:04.000000 s5learn-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.092579 s5learn-0.8.1/
+-rw-rw-rw-   0        0        0       54 2024-05-19 23:33:43.092579 s5learn-0.8.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.061331 s5learn-0.8.1/s5learn/
+-rw-rw-rw-   0        0        0       48 2024-05-19 23:33:25.000000 s5learn-0.8.1/s5learn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.076955 s5learn-0.8.1/s5learn/data/
+-rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.8.1/s5learn/data/example.txt
+-rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8.1/s5learn/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.092579 s5learn-0.8.1/s5learn/preprocessing/
+-rw-rw-rw-   0        0        0      200 2024-05-19 23:27:53.000000 s5learn-0.8.1/s5learn/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2753 2024-05-19 22:11:08.000000 s5learn-0.8.1/s5learn/preprocessing/idp.py
+-rw-rw-rw-   0        0        0     7318 2024-05-19 22:04:34.000000 s5learn-0.8.1/s5learn/preprocessing/m5.py
+-rw-rw-rw-   0        0        0     5940 2024-05-19 22:14:34.000000 s5learn-0.8.1/s5learn/preprocessing/mnv2.py
+-rw-rw-rw-   0        0        0     1394 2024-05-19 22:13:21.000000 s5learn-0.8.1/s5learn/preprocessing/mnv2_dp.py
+-rw-rw-rw-   0        0        0      979 2024-05-19 22:19:47.000000 s5learn-0.8.1/s5learn/preprocessing/mnv2_dv.py
+-rw-rw-rw-   0        0        0     2075 2024-05-19 22:06:44.000000 s5learn-0.8.1/s5learn/preprocessing/ms.py
+-rw-rw-rw-   0        0        0     3935 2024-05-19 22:08:10.000000 s5learn-0.8.1/s5learn/preprocessing/mv2_train.py
+-rw-rw-rw-   0        0        0     3109 2024-05-19 22:10:02.000000 s5learn-0.8.1/s5learn/preprocessing/t5.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.092579 s5learn-0.8.1/s5learn.egg-info/
+-rw-rw-rw-   0        0        0       54 2024-05-19 23:33:42.000000 s5learn-0.8.1/s5learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-05-19 23:33:42.000000 s5learn-0.8.1/s5learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 23:33:42.000000 s5learn-0.8.1/s5learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 23:33:42.000000 s5learn-0.8.1/s5learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 23:33:43.092579 s5learn-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1819 2024-05-19 23:31:04.000000 s5learn-0.8.1/setup.py
```

### Comparing `s5learn-0.8/setup.py` & `s5learn-0.8.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='s5learn',
-    version='0.8',
+    version='0.8.1',
     packages=find_packages(),
     package_data={'': ['data/*.txt']},
 )
 
 
 
 # import setuptools
```


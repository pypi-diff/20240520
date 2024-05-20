# Comparing `tmp/s5learn-0.8.1.tar.gz` & `tmp/s5learn-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5learn-0.8.1.tar", last modified: Sun May 19 23:33:43 2024, max compression
+gzip compressed data, was "s5learn-0.8.2.tar", last modified: Sun May 19 23:42:11 2024, max compression
```

## Comparing `s5learn-0.8.1.tar` & `s5learn-0.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.092579 s5learn-0.8.1/
--rw-rw-rw-   0        0        0       54 2024-05-19 23:33:43.092579 s5learn-0.8.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.061331 s5learn-0.8.1/s5learn/
--rw-rw-rw-   0        0        0       48 2024-05-19 23:33:25.000000 s5learn-0.8.1/s5learn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.076955 s5learn-0.8.1/s5learn/data/
--rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.8.1/s5learn/data/example.txt
--rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8.1/s5learn/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.092579 s5learn-0.8.1/s5learn/preprocessing/
--rw-rw-rw-   0        0        0      200 2024-05-19 23:27:53.000000 s5learn-0.8.1/s5learn/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2753 2024-05-19 22:11:08.000000 s5learn-0.8.1/s5learn/preprocessing/idp.py
--rw-rw-rw-   0        0        0     7318 2024-05-19 22:04:34.000000 s5learn-0.8.1/s5learn/preprocessing/m5.py
--rw-rw-rw-   0        0        0     5940 2024-05-19 22:14:34.000000 s5learn-0.8.1/s5learn/preprocessing/mnv2.py
--rw-rw-rw-   0        0        0     1394 2024-05-19 22:13:21.000000 s5learn-0.8.1/s5learn/preprocessing/mnv2_dp.py
--rw-rw-rw-   0        0        0      979 2024-05-19 22:19:47.000000 s5learn-0.8.1/s5learn/preprocessing/mnv2_dv.py
--rw-rw-rw-   0        0        0     2075 2024-05-19 22:06:44.000000 s5learn-0.8.1/s5learn/preprocessing/ms.py
--rw-rw-rw-   0        0        0     3935 2024-05-19 22:08:10.000000 s5learn-0.8.1/s5learn/preprocessing/mv2_train.py
--rw-rw-rw-   0        0        0     3109 2024-05-19 22:10:02.000000 s5learn-0.8.1/s5learn/preprocessing/t5.py
-drwxrwxrwx   0        0        0        0 2024-05-19 23:33:43.092579 s5learn-0.8.1/s5learn.egg-info/
--rw-rw-rw-   0        0        0       54 2024-05-19 23:33:42.000000 s5learn-0.8.1/s5learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-05-19 23:33:42.000000 s5learn-0.8.1/s5learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 23:33:42.000000 s5learn-0.8.1/s5learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 23:33:42.000000 s5learn-0.8.1/s5learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 23:33:43.092579 s5learn-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1819 2024-05-19 23:31:04.000000 s5learn-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:42:11.460450 s5learn-0.8.2/
+-rw-rw-rw-   0        0        0       54 2024-05-19 23:42:11.444824 s5learn-0.8.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 23:42:11.429201 s5learn-0.8.2/s5learn/
+-rw-rw-rw-   0        0        0       28 2024-05-19 23:40:29.000000 s5learn-0.8.2/s5learn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:42:11.429201 s5learn-0.8.2/s5learn/data/
+-rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.8.2/s5learn/data/example.txt
+-rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8.2/s5learn/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:42:11.444824 s5learn-0.8.2/s5learn/preprocessing/
+-rw-rw-rw-   0        0        0      200 2024-05-19 23:27:53.000000 s5learn-0.8.2/s5learn/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2753 2024-05-19 22:11:08.000000 s5learn-0.8.2/s5learn/preprocessing/idp.py
+-rw-rw-rw-   0        0        0     7318 2024-05-19 22:04:34.000000 s5learn-0.8.2/s5learn/preprocessing/m5.py
+-rw-rw-rw-   0        0        0     5940 2024-05-19 22:14:34.000000 s5learn-0.8.2/s5learn/preprocessing/mnv2.py
+-rw-rw-rw-   0        0        0     1394 2024-05-19 22:13:21.000000 s5learn-0.8.2/s5learn/preprocessing/mnv2_dp.py
+-rw-rw-rw-   0        0        0      979 2024-05-19 22:19:47.000000 s5learn-0.8.2/s5learn/preprocessing/mnv2_dv.py
+-rw-rw-rw-   0        0        0     2075 2024-05-19 22:06:44.000000 s5learn-0.8.2/s5learn/preprocessing/ms.py
+-rw-rw-rw-   0        0        0     3935 2024-05-19 22:08:10.000000 s5learn-0.8.2/s5learn/preprocessing/mv2_train.py
+-rw-rw-rw-   0        0        0     3109 2024-05-19 22:10:02.000000 s5learn-0.8.2/s5learn/preprocessing/t5.py
+drwxrwxrwx   0        0        0        0 2024-05-19 23:42:11.444824 s5learn-0.8.2/s5learn.egg-info/
+-rw-rw-rw-   0        0        0       54 2024-05-19 23:42:11.000000 s5learn-0.8.2/s5learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-05-19 23:42:11.000000 s5learn-0.8.2/s5learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 23:42:11.000000 s5learn-0.8.2/s5learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 23:42:11.000000 s5learn-0.8.2/s5learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 23:42:11.460450 s5learn-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1819 2024-05-19 23:40:29.000000 s5learn-0.8.2/setup.py
```

### Comparing `s5learn-0.8.1/s5learn/preprocessing/idp.py` & `s5learn-0.8.2/s5learn/preprocessing/idp.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.1/s5learn/preprocessing/m5.py` & `s5learn-0.8.2/s5learn/preprocessing/m5.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.1/s5learn/preprocessing/mnv2.py` & `s5learn-0.8.2/s5learn/preprocessing/mnv2.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.1/s5learn/preprocessing/mnv2_dp.py` & `s5learn-0.8.2/s5learn/preprocessing/mnv2_dp.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.1/s5learn/preprocessing/mnv2_dv.py` & `s5learn-0.8.2/s5learn/preprocessing/mnv2_dv.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.1/s5learn/preprocessing/ms.py` & `s5learn-0.8.2/s5learn/preprocessing/ms.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.1/s5learn/preprocessing/mv2_train.py` & `s5learn-0.8.2/s5learn/preprocessing/mv2_train.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.1/s5learn/preprocessing/t5.py` & `s5learn-0.8.2/s5learn/preprocessing/t5.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.1/setup.py` & `s5learn-0.8.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='s5learn',
-    version='0.8.1',
+    version='0.8.2',
     packages=find_packages(),
     package_data={'': ['data/*.txt']},
 )
 
 
 
 # import setuptools
```


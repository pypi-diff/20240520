# Comparing `tmp/rdatapp-0.6a0.tar.gz` & `tmp/rdatapp-0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdatapp-0.6a0.tar", last modified: Mon May 20 11:06:22 2024, max compression
+gzip compressed data, was "rdatapp-0.7a0.tar", last modified: Mon May 20 11:49:34 2024, max compression
```

## Comparing `rdatapp-0.6a0.tar` & `rdatapp-0.7a0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:06:22.604677 rdatapp-0.6a0/
--rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-20 11:06:22.604488 rdatapp-0.6a0/PKG-INFO
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:06:22.603396 rdatapp-0.6a0/rdatapp/
--rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.6a0/rdatapp/__init__.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1823 2024-05-20 10:38:30.000000 rdatapp-0.6a0/rdatapp/categorical_encoder.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1404 2024-05-20 10:39:16.000000 rdatapp-0.6a0/rdatapp/data_type_converter.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1474 2024-05-20 10:39:41.000000 rdatapp-0.6a0/rdatapp/datetime_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)      969 2024-05-20 10:42:18.000000 rdatapp-0.6a0/rdatapp/feature_engineer.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     2638 2024-05-20 10:44:02.000000 rdatapp-0.6a0/rdatapp/missing_value_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1155 2024-05-20 10:45:07.000000 rdatapp-0.6a0/rdatapp/outlier_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1464 2024-05-20 10:45:34.000000 rdatapp-0.6a0/rdatapp/scaler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1389 2024-05-20 10:46:15.000000 rdatapp-0.6a0/rdatapp/text_cleaner.py
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:06:22.604247 rdatapp-0.6a0/rdatapp.egg-info/
--rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/PKG-INFO
--rw-r--r--   0 ifozmen    (501) staff       (20)      402 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/SOURCES.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/dependency_links.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       31 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/requires.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/top_level.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-20 11:06:22.604767 rdatapp-0.6a0/setup.cfg
--rw-rw-r--   0 ifozmen    (501) staff       (20)      822 2024-05-20 11:06:15.000000 rdatapp-0.6a0/setup.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:49:34.451567 rdatapp-0.7a0/
+-rw-r--r--   0 ifozmen    (501) staff       (20)     5280 2024-05-20 11:49:34.451389 rdatapp-0.7a0/PKG-INFO
+-rw-r--r--   0 ifozmen    (501) staff       (20)     3914 2024-05-20 11:39:34.000000 rdatapp-0.7a0/README.md
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:49:34.450057 rdatapp-0.7a0/rdatapp/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.7a0/rdatapp/__init__.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1823 2024-05-20 10:38:30.000000 rdatapp-0.7a0/rdatapp/categorical_encoder.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1404 2024-05-20 10:39:16.000000 rdatapp-0.7a0/rdatapp/data_type_converter.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1474 2024-05-20 10:39:41.000000 rdatapp-0.7a0/rdatapp/datetime_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)      969 2024-05-20 10:42:18.000000 rdatapp-0.7a0/rdatapp/feature_engineer.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     2638 2024-05-20 10:44:02.000000 rdatapp-0.7a0/rdatapp/missing_value_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1155 2024-05-20 10:45:07.000000 rdatapp-0.7a0/rdatapp/outlier_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1464 2024-05-20 10:45:34.000000 rdatapp-0.7a0/rdatapp/scaler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1389 2024-05-20 10:46:15.000000 rdatapp-0.7a0/rdatapp/text_cleaner.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:49:34.450984 rdatapp-0.7a0/rdatapp.egg-info/
+-rw-r--r--   0 ifozmen    (501) staff       (20)     5280 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/PKG-INFO
+-rw-r--r--   0 ifozmen    (501) staff       (20)      412 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/SOURCES.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/dependency_links.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       31 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/requires.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-20 11:49:34.000000 rdatapp-0.7a0/rdatapp.egg-info/top_level.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-20 11:49:34.451624 rdatapp-0.7a0/setup.cfg
+-rw-rw-r--   0 ifozmen    (501) staff       (20)     1794 2024-05-20 11:49:24.000000 rdatapp-0.7a0/setup.py
```

### Comparing `rdatapp-0.6a0/rdatapp/__init__.py` & `rdatapp-0.7a0/rdatapp/__init__.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.6a0/rdatapp/categorical_encoder.py` & `rdatapp-0.7a0/rdatapp/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.6a0/rdatapp/data_type_converter.py` & `rdatapp-0.7a0/rdatapp/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.6a0/rdatapp/datetime_handler.py` & `rdatapp-0.7a0/rdatapp/datetime_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.6a0/rdatapp/feature_engineer.py` & `rdatapp-0.7a0/rdatapp/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.6a0/rdatapp/missing_value_handler.py` & `rdatapp-0.7a0/rdatapp/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.6a0/rdatapp/outlier_handler.py` & `rdatapp-0.7a0/rdatapp/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.6a0/rdatapp/scaler.py` & `rdatapp-0.7a0/rdatapp/scaler.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.6a0/rdatapp/text_cleaner.py` & `rdatapp-0.7a0/rdatapp/text_cleaner.py`

 * *Files identical despite different names*


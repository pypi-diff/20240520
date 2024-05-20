# Comparing `tmp/agi_med_metrics-0.0.2.tar.gz` & `tmp/agi_med_metrics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agi_med_metrics-0.0.2.tar", last modified: Tue May 14 10:17:05 2024, max compression
+gzip compressed data, was "agi_med_metrics-0.0.3.tar", last modified: Mon May 20 11:04:45 2024, max compression
```

## Comparing `agi_med_metrics-0.0.2.tar` & `agi_med_metrics-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:17:05.604519 agi_med_metrics-0.0.2/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-14 09:23:43.000000 agi_med_metrics-0.0.2/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      661 2024-05-14 10:17:05.604519 agi_med_metrics-0.0.2/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      146 2024-05-14 09:25:17.000000 agi_med_metrics-0.0.2/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:17:05.604519 agi_med_metrics-0.0.2/agi_med_metrics/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-14 10:16:33.000000 agi_med_metrics-0.0.2/agi_med_metrics/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      425 2024-05-14 09:31:45.000000 agi_med_metrics-0.0.2/agi_med_metrics/errors_cv.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      407 2024-05-14 09:35:54.000000 agi_med_metrics-0.0.2/agi_med_metrics/errors_ml.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      467 2024-05-14 09:35:22.000000 agi_med_metrics-0.0.2/agi_med_metrics/errors_nlp.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:17:05.604519 agi_med_metrics-0.0.2/agi_med_metrics.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      661 2024-05-14 10:17:05.000000 agi_med_metrics-0.0.2/agi_med_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      357 2024-05-14 10:17:05.000000 agi_med_metrics-0.0.2/agi_med_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-14 10:17:05.000000 agi_med_metrics-0.0.2/agi_med_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      203 2024-05-14 10:17:05.000000 agi_med_metrics-0.0.2/agi_med_metrics.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       16 2024-05-14 10:17:05.000000 agi_med_metrics-0.0.2/agi_med_metrics.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      202 2024-05-14 09:37:42.000000 agi_med_metrics-0.0.2/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-14 10:17:05.604519 agi_med_metrics-0.0.2/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      801 2024-05-14 09:43:53.000000 agi_med_metrics-0.0.2/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:44.997841 agi_med_metrics-0.0.3/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-14 09:23:43.000000 agi_med_metrics-0.0.3/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      661 2024-05-20 11:04:44.997841 agi_med_metrics-0.0.3/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      146 2024-05-14 09:25:17.000000 agi_med_metrics-0.0.3/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:44.997841 agi_med_metrics-0.0.3/agi_med_metrics/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-20 10:58:10.000000 agi_med_metrics-0.0.3/agi_med_metrics/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      425 2024-05-14 09:31:45.000000 agi_med_metrics-0.0.3/agi_med_metrics/errors_cv.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      407 2024-05-14 09:35:54.000000 agi_med_metrics-0.0.3/agi_med_metrics/errors_ml.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      859 2024-05-20 10:22:41.000000 agi_med_metrics-0.0.3/agi_med_metrics/errors_nlp.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:44.997841 agi_med_metrics-0.0.3/agi_med_metrics.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      661 2024-05-20 11:04:44.000000 agi_med_metrics-0.0.3/agi_med_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      387 2024-05-20 11:04:44.000000 agi_med_metrics-0.0.3/agi_med_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-20 11:04:44.000000 agi_med_metrics-0.0.3/agi_med_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      203 2024-05-20 11:04:44.000000 agi_med_metrics-0.0.3/agi_med_metrics.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       21 2024-05-20 11:04:44.000000 agi_med_metrics-0.0.3/agi_med_metrics.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      202 2024-05-14 09:37:42.000000 agi_med_metrics-0.0.3/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-20 11:04:44.997841 agi_med_metrics-0.0.3/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      801 2024-05-14 09:43:53.000000 agi_med_metrics-0.0.3/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:04:44.997841 agi_med_metrics-0.0.3/test/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-20 10:22:41.000000 agi_med_metrics-0.0.3/test/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      668 2024-05-20 10:22:41.000000 agi_med_metrics-0.0.3/test/base.py
```

### Comparing `agi_med_metrics-0.0.2/PKG-INFO` & `agi_med_metrics-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agi_med_metrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utils for agi-med team metric calculation
 Author: AGI-MED-TEAM
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: pandas==2.2.0
 Requires-Dist: scikit-learn==1.4.0
 Requires-Dist: scipy==1.12.0
 Requires-Dist: numpy==1.26.4
```

### Comparing `agi_med_metrics-0.0.2/agi_med_metrics.egg-info/PKG-INFO` & `agi_med_metrics-0.0.3/agi_med_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agi_med_metrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utils for agi-med team metric calculation
 Author: AGI-MED-TEAM
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: pandas==2.2.0
 Requires-Dist: scikit-learn==1.4.0
 Requires-Dist: scipy==1.12.0
 Requires-Dist: numpy==1.26.4
```

### Comparing `agi_med_metrics-0.0.2/setup.py` & `agi_med_metrics-0.0.3/setup.py`

 * *Files identical despite different names*


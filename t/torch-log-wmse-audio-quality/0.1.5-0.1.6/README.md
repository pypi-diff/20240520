# Comparing `tmp/torch_log_wmse_audio_quality-0.1.5.tar.gz` & `tmp/torch_log_wmse_audio_quality-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_log_wmse_audio_quality-0.1.5.tar", last modified: Fri May 17 19:10:28 2024, max compression
+gzip compressed data, was "torch_log_wmse_audio_quality-0.1.6.tar", last modified: Mon May 20 21:50:52 2024, max compression
```

## Comparing `torch_log_wmse_audio_quality-0.1.5.tar` & `torch_log_wmse_audio_quality-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:10:28.153313 torch_log_wmse_audio_quality-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-17 19:10:28.153313 torch_log_wmse_audio_quality-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-17 19:10:28.153313 torch_log_wmse_audio_quality-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:10:28.149312 torch_log_wmse_audio_quality-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/tests/test_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:10:28.149312 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    32151 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/filter_ir.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/freq_weighting_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:10:28.153313 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:50:52.169886 torch_log_wmse_audio_quality-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/tests/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32151 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/filter_ir.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/freq_weighting_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/top_level.txt
```

### Comparing `torch_log_wmse_audio_quality-0.1.5/LICENSE` & `torch_log_wmse_audio_quality-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.5/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.5
+Version: 0.1.6
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_log_wmse_audio_quality-0.1.5/README.md` & `torch_log_wmse_audio_quality-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.5/setup.cfg` & `torch_log_wmse_audio_quality-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch-log-wmse-audio-quality
-version = 0.1.5
+version = 0.1.6
 author = Christopher Landschoot
 author_email = crlandschoot@gmail.com
 license = Apache License 2.0
 description = logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/crlandsc/torch-log-wmse-audio-quality
```

### Comparing `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/constants.py` & `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/constants.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/filter_ir.pkl` & `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/filter_ir.pkl`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/metric.py` & `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/metric.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/utils.py` & `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/utils.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.5
+Version: 0.1.6
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/SOURCES.txt` & `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*


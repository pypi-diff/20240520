# Comparing `tmp/htt-0.8.tar.gz` & `tmp/htt-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htt-0.8.tar", max compression
+gzip compressed data, was "htt-0.9.tar", max compression
```

## Comparing `htt-0.8.tar` & `htt-0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-20 03:56:04.979903 htt-0.8/README.md
--rw-r--r--   0        0        0       64 2023-12-19 03:00:23.966998 htt-0.8/htt/__init__.py
--rw-r--r--   0        0        0     8967 2024-03-27 03:05:58.417535 htt-0.8/htt/application.py
--rw-r--r--   0        0        0      495 2024-03-22 00:52:11.954094 htt-0.8/htt/pytest_skip_dev.py
--rw-r--r--   0        0        0     2019 2024-04-19 02:36:25.528905 htt-0.8/htt/segment_timer.py
--rw-r--r--   0        0        0      357 2024-04-19 03:17:33.201294 htt-0.8/pyproject.toml
--rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 htt-0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-20 03:56:04.979903 htt-0.9/README.md
+-rw-r--r--   0        0        0      120 2024-04-19 03:28:19.569647 htt-0.9/htt/__init__.py
+-rw-r--r--   0        0        0     8967 2024-03-27 03:05:58.417535 htt-0.9/htt/application.py
+-rw-r--r--   0        0        0      495 2024-03-22 00:52:11.954094 htt-0.9/htt/pytest_skip_dev.py
+-rw-r--r--   0        0        0     2019 2024-04-19 02:36:25.528905 htt-0.9/htt/segment_timer.py
+-rw-r--r--   0        0        0      357 2024-04-19 03:29:07.338264 htt-0.9/pyproject.toml
+-rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 htt-0.9/PKG-INFO
```

### Comparing `htt-0.8/htt/application.py` & `htt-0.9/htt/application.py`

 * *Files identical despite different names*

### Comparing `htt-0.8/htt/segment_timer.py` & `htt-0.9/htt/segment_timer.py`

 * *Files identical despite different names*


# Comparing `tmp/rix_template-0.0.1.tar.gz` & `tmp/rix_template-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rix_template-0.0.1.tar", last modified: Sun May 19 10:41:19 2024, max compression
+gzip compressed data, was "rix_template-0.0.2.tar", last modified: Sun May 19 15:53:39 2024, max compression
```

## Comparing `rix_template-0.0.1.tar` & `rix_template-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:41:19.536718 rix_template-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 10:41:14.000000 rix_template-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 10:41:14.000000 rix_template-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-19 10:41:19.536718 rix_template-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-19 10:41:14.000000 rix_template-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:41:19.536718 rix_template-0.0.1/rix_template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 10:41:14.000000 rix_template-0.0.1/rix_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:41:19.536718 rix_template-0.0.1/rix_template/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 10:41:14.000000 rix_template-0.0.1/rix_template/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-19 10:41:14.000000 rix_template-0.0.1/rix_template/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-19 10:41:14.000000 rix_template-0.0.1/rix_template/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-19 10:41:14.000000 rix_template-0.0.1/rix_template/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:41:19.536718 rix_template-0.0.1/rix_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-19 10:41:19.000000 rix_template-0.0.1/rix_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-19 10:41:19.000000 rix_template-0.0.1/rix_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 10:41:19.000000 rix_template-0.0.1/rix_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 10:41:19.000000 rix_template-0.0.1/rix_template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 10:41:19.000000 rix_template-0.0.1/rix_template.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 10:41:19.000000 rix_template-0.0.1/rix_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 10:41:19.000000 rix_template-0.0.1/rix_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 10:41:19.536718 rix_template-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-19 10:41:14.000000 rix_template-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:53:39.570357 rix_template-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 15:53:35.000000 rix_template-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 15:53:35.000000 rix_template-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-19 15:53:39.570357 rix_template-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-19 15:53:35.000000 rix_template-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:53:39.570357 rix_template-0.0.2/rix_template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 15:53:35.000000 rix_template-0.0.2/rix_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:53:39.570357 rix_template-0.0.2/rix_template/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 15:53:35.000000 rix_template-0.0.2/rix_template/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-19 15:53:35.000000 rix_template-0.0.2/rix_template/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-19 15:53:35.000000 rix_template-0.0.2/rix_template/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-19 15:53:35.000000 rix_template-0.0.2/rix_template/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:53:39.570357 rix_template-0.0.2/rix_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-19 15:53:39.000000 rix_template-0.0.2/rix_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-19 15:53:39.000000 rix_template-0.0.2/rix_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:53:39.000000 rix_template-0.0.2/rix_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 15:53:39.000000 rix_template-0.0.2/rix_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:53:39.000000 rix_template-0.0.2/rix_template.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 15:53:39.000000 rix_template-0.0.2/rix_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 15:53:39.000000 rix_template-0.0.2/rix_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 15:53:39.570357 rix_template-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-19 15:53:35.000000 rix_template-0.0.2/setup.py
```

### Comparing `rix_template-0.0.1/LICENSE` & `rix_template-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rix_template-0.0.1/LICENSE.md` & `rix_template-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rix_template-0.0.1/PKG-INFO` & `rix_template-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rix_template
-Version: 0.0.1
+Version: 0.0.2
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/Python-Template
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rix_template-0.0.1/README.md` & `rix_template-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rix_template-0.0.1/rix_template/run.py` & `rix_template-0.0.2/rix_template/run.py`

 * *Files identical despite different names*

### Comparing `rix_template-0.0.1/rix_template.egg-info/PKG-INFO` & `rix_template-0.0.2/rix_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rix-template
-Version: 0.0.1
+Version: 0.0.2
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/Python-Template
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rix_template-0.0.1/setup.py` & `rix_template-0.0.2/setup.py`

 * *Files identical despite different names*


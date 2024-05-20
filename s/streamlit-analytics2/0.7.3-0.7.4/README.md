# Comparing `tmp/streamlit_analytics2-0.7.3.tar.gz` & `tmp/streamlit_analytics2-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_analytics2-0.7.3.tar", last modified: Sat May  4 06:03:36 2024, max compression
+gzip compressed data, was "streamlit_analytics2-0.7.4.tar", last modified: Mon May 20 06:02:49 2024, max compression
```

## Comparing `streamlit_analytics2-0.7.3.tar` & `streamlit_analytics2-0.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.724917 streamlit_analytics2-0.7.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/.github/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.724917 streamlit_analytics2-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.724917 streamlit_analytics2-0.7.3/src/streamlit_analytics2/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/firestore.py
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 06:03:36.000000 streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:03:36.728917 streamlit_analytics2-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-04 06:03:00.000000 streamlit_analytics2-0.7.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:02:49.244038 streamlit_analytics2-0.7.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:02:49.240038 streamlit_analytics2-0.7.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/.github/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-20 06:02:49.244038 streamlit_analytics2-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:02:49.244038 streamlit_analytics2-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:02:49.240038 streamlit_analytics2-0.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:02:49.244038 streamlit_analytics2-0.7.4/src/streamlit_analytics2/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:02:49.244038 streamlit_analytics2-0.7.4/src/streamlit_analytics2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-20 06:02:49.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-20 06:02:49.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:02:49.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 06:02:49.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 06:02:49.000000 streamlit_analytics2-0.7.4/src/streamlit_analytics2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:02:49.244038 streamlit_analytics2-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-20 06:02:08.000000 streamlit_analytics2-0.7.4/tests/test_utils.py
```

### Comparing `streamlit_analytics2-0.7.3/.github/README.md` & `streamlit_analytics2-0.7.4/.github/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.3/LICENSE` & `streamlit_analytics2-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.3/PKG-INFO` & `streamlit_analytics2-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_analytics2
-Version: 0.7.3
+Version: 0.7.4
 Summary: Track & visualize user interactions with your streamlit app.
 Author-email: 444B <contact+pypi@444b.me>
 License: MIT License
         
         Copyright (c) 2021 Johannes Rieke
         
         Copyright (c) 2024 444B
```

### Comparing `streamlit_analytics2-0.7.3/pyproject.toml` & `streamlit_analytics2-0.7.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.1.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_analytics2"
-version = "0.7.3"
+version = "0.7.4"
 description = "Track & visualize user interactions with your streamlit app."
 authors = [{ name = "444B", email = "contact+pypi@444b.me" }]
 license = { file = "LICENSE" }
 readme = {file = ".github/README.md", content-type = "text/markdown"}
 keywords = ["streamlit", "analytics", "visualization", "streamlit-analytics", "streamlit-analytics2"]
 classifiers = [
     "Programming Language :: Python :: 3.9",
```

### Comparing `streamlit_analytics2-0.7.3/src/streamlit_analytics2/display.py` & `streamlit_analytics2-0.7.4/src/streamlit_analytics2/display.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.3/src/streamlit_analytics2/firestore.py` & `streamlit_analytics2-0.7.4/src/streamlit_analytics2/firestore.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.3/src/streamlit_analytics2/main.py` & `streamlit_analytics2-0.7.4/src/streamlit_analytics2/main.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.3/src/streamlit_analytics2/utils.py` & `streamlit_analytics2-0.7.4/src/streamlit_analytics2/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_analytics2-0.7.3/src/streamlit_analytics2.egg-info/PKG-INFO` & `streamlit_analytics2-0.7.4/src/streamlit_analytics2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_analytics2
-Version: 0.7.3
+Version: 0.7.4
 Summary: Track & visualize user interactions with your streamlit app.
 Author-email: 444B <contact+pypi@444b.me>
 License: MIT License
         
         Copyright (c) 2021 Johannes Rieke
         
         Copyright (c) 2024 444B
```

### Comparing `streamlit_analytics2-0.7.3/tests/test_utils.py` & `streamlit_analytics2-0.7.4/tests/test_utils.py`

 * *Files identical despite different names*


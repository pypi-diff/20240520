# Comparing `tmp/ndpprep-0.0.3.tar.gz` & `tmp/ndpprep-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndpprep-0.0.3.tar", last modified: Mon May 20 11:28:24 2024, max compression
+gzip compressed data, was "ndpprep-0.0.4.tar", last modified: Mon May 20 11:39:15 2024, max compression
```

## Comparing `ndpprep-0.0.3.tar` & `ndpprep-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:28:24.693322 ndpprep-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-20 11:28:24.693322 ndpprep-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 11:28:20.000000 ndpprep-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-20 11:28:20.000000 ndpprep-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:28:24.693322 ndpprep-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:28:24.689322 ndpprep-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:28:24.693322 ndpprep-0.0.3/src/ndpprep/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:28:20.000000 ndpprep-0.0.3/src/ndpprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 11:28:20.000000 ndpprep-0.0.3/src/ndpprep/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:28:24.693322 ndpprep-0.0.3/src/ndpprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-20 11:28:24.000000 ndpprep-0.0.3/src/ndpprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 11:28:24.000000 ndpprep-0.0.3/src/ndpprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:28:24.000000 ndpprep-0.0.3/src/ndpprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 11:28:24.000000 ndpprep-0.0.3/src/ndpprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 11:28:24.000000 ndpprep-0.0.3/src/ndpprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 11:28:24.000000 ndpprep-0.0.3/src/ndpprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:39:15.839979 ndpprep-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-20 11:39:15.839979 ndpprep-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 11:39:12.000000 ndpprep-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-20 11:39:12.000000 ndpprep-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:39:15.839979 ndpprep-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:39:15.835979 ndpprep-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:39:15.839979 ndpprep-0.0.4/src/ndpprep/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:39:12.000000 ndpprep-0.0.4/src/ndpprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 11:39:12.000000 ndpprep-0.0.4/src/ndpprep/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:39:15.839979 ndpprep-0.0.4/src/ndpprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-20 11:39:15.000000 ndpprep-0.0.4/src/ndpprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 11:39:15.000000 ndpprep-0.0.4/src/ndpprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:39:15.000000 ndpprep-0.0.4/src/ndpprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 11:39:15.000000 ndpprep-0.0.4/src/ndpprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 11:39:15.000000 ndpprep-0.0.4/src/ndpprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 11:39:15.000000 ndpprep-0.0.4/src/ndpprep.egg-info/top_level.txt
```

### Comparing `ndpprep-0.0.3/PKG-INFO` & `ndpprep-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndpprep
-Version: 0.0.3
+Version: 0.0.4
 Summary: A command line tool to prepare high-quality data in Parquet
 Author-email: Mohd Zaid Waqiyuddin Mohd Zulkifli <zaidwaqi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zaidwaqi/ndpprep
 Project-URL: Issues, https://github.com/pypa/zaidwaqi/ndpprep/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ndpprep-0.0.3/pyproject.toml` & `ndpprep-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ndpprep"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Mohd Zaid Waqiyuddin Mohd Zulkifli", email="zaidwaqi@gmail.com" }
 ]
 description = "A command line tool to prepare high-quality data in Parquet"
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.11"
```

### Comparing `ndpprep-0.0.3/src/ndpprep.egg-info/PKG-INFO` & `ndpprep-0.0.4/src/ndpprep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndpprep
-Version: 0.0.3
+Version: 0.0.4
 Summary: A command line tool to prepare high-quality data in Parquet
 Author-email: Mohd Zaid Waqiyuddin Mohd Zulkifli <zaidwaqi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zaidwaqi/ndpprep
 Project-URL: Issues, https://github.com/pypa/zaidwaqi/ndpprep/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


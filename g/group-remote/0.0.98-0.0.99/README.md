# Comparing `tmp/group-remote-0.0.98.tar.gz` & `tmp/group-remote-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group-remote-0.0.98.tar", last modified: Wed Jan 10 13:20:12 2024, max compression
+gzip compressed data, was "group-remote-0.0.99.tar", last modified: Wed Jan 10 14:23:09 2024, max compression
```

## Comparing `group-remote-0.0.98.tar` & `group-remote-0.0.99.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:20:12.355376 group-remote-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-10 13:20:12.355376 group-remote-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-10 13:19:42.000000 group-remote-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:20:12.351376 group-remote-0.0.98/group_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:20:12.355376 group-remote-0.0.98/group_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 13:19:42.000000 group-remote-0.0.98/group_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-01-10 13:19:42.000000 group-remote-0.0.98/group_remote/src/group_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:20:12.355376 group-remote-0.0.98/group_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-10 13:20:12.000000 group-remote-0.0.98/group_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-10 13:20:12.000000 group-remote-0.0.98/group_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 13:20:12.000000 group-remote-0.0.98/group_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-10 13:20:12.000000 group-remote-0.0.98/group_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-10 13:20:12.000000 group-remote-0.0.98/group_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-10 13:19:42.000000 group-remote-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 13:20:12.355376 group-remote-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-10 13:19:42.000000 group-remote-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:23:09.793388 group-remote-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-10 14:23:09.793388 group-remote-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-10 14:22:41.000000 group-remote-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:23:09.789388 group-remote-0.0.99/group_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:23:09.793388 group-remote-0.0.99/group_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 14:22:41.000000 group-remote-0.0.99/group_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-01-10 14:22:41.000000 group-remote-0.0.99/group_remote/src/group_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 14:23:09.793388 group-remote-0.0.99/group_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-10 14:23:09.000000 group-remote-0.0.99/group_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-10 14:23:09.000000 group-remote-0.0.99/group_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 14:23:09.000000 group-remote-0.0.99/group_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-10 14:23:09.000000 group-remote-0.0.99/group_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-10 14:23:09.000000 group-remote-0.0.99/group_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-10 14:22:41.000000 group-remote-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 14:23:09.793388 group-remote-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-10 14:22:41.000000 group-remote-0.0.99/setup.py
```

### Comparing `group-remote-0.0.98/PKG-INFO` & `group-remote-0.0.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-remote
-Version: 0.0.98
+Version: 0.0.99
 Summary: PyPI Package for Circles Group-Remote Python
 Home-page: https://github.com/circles-zone/group-remote-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group-remote-0.0.98/README.md` & `group-remote-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `group-remote-0.0.98/group_remote/src/group_remote.py` & `group-remote-0.0.99/group_remote/src/group_remote.py`

 * *Files identical despite different names*

### Comparing `group-remote-0.0.98/group_remote.egg-info/PKG-INFO` & `group-remote-0.0.99/group_remote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-remote
-Version: 0.0.98
+Version: 0.0.99
 Summary: PyPI Package for Circles Group-Remote Python
 Home-page: https://github.com/circles-zone/group-remote-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group-remote-0.0.98/pyproject.toml` & `group-remote-0.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "group-remote"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.98" # https://pypi.org/project/group-remote i.e. https://pypi.org/project/storage-local/
+version = "0.0.99" # https://pypi.org/project/group-remote i.e. https://pypi.org/project/storage-local/
 description = "group-remote Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `group-remote-0.0.98/setup.py` & `group-remote-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 PACKAGE_NAME = "group-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix).
     # Only lowercase, no underlines.
     name=PACKAGE_NAME,
-    version='0.0.98',  # https://pypi.org/project/group-remote/
+    version='0.0.99',  # https://pypi.org/project/group-remote/
     author="Circles",
     author_email="info@circlez.ai",
     # TODO: Please update the description and delete this line
     description="PyPI Package for Circles Group-Remote Python",
     long_description="PyPI Package for Circles Group-Remote Python",
     long_description_content_type='text/markdown',
     # TODO: Please update the URL below
```


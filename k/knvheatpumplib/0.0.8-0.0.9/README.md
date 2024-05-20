# Comparing `tmp/knvheatpumplib-0.0.8.tar.gz` & `tmp/knvheatpumplib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knvheatpumplib-0.0.8.tar", last modified: Tue Oct 10 10:52:42 2023, max compression
+gzip compressed data, was "knvheatpumplib-0.0.9.tar", last modified: Sun Oct 15 12:51:40 2023, max compression
```

## Comparing `knvheatpumplib-0.0.8.tar` & `knvheatpumplib-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:42.131821 knvheatpumplib-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:42.127821 knvheatpumplib-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:42.127821 knvheatpumplib-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:42.127821 knvheatpumplib-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35142 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-10 10:52:42.131821 knvheatpumplib-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/flake.lock
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/flake.nix
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:42.127821 knvheatpumplib-0.0.8/knvheatpumplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/knvheatpumplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/knvheatpumplib/knvheatpump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/knvheatpumplib/knvparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:42.131821 knvheatpumplib-0.0.8/knvheatpumplib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-10 10:52:42.000000 knvheatpumplib-0.0.8/knvheatpumplib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-10 10:52:42.000000 knvheatpumplib-0.0.8/knvheatpumplib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 10:52:42.000000 knvheatpumplib-0.0.8/knvheatpumplib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-10 10:52:42.000000 knvheatpumplib-0.0.8/knvheatpumplib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-10 10:52:42.131821 knvheatpumplib-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:42.131821 knvheatpumplib-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-10-10 10:52:31.000000 knvheatpumplib-0.0.8/tests/test_knvheatpump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:40.252227 knvheatpumplib-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:40.244227 knvheatpumplib-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:40.248227 knvheatpumplib-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:40.248227 knvheatpumplib-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35142 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-15 12:51:40.252227 knvheatpumplib-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/flake.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/flake.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:40.252227 knvheatpumplib-0.0.9/knvheatpumplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/knvheatpumplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/knvheatpumplib/knvheatpump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/knvheatpumplib/knvparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:40.252227 knvheatpumplib-0.0.9/knvheatpumplib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-15 12:51:40.000000 knvheatpumplib-0.0.9/knvheatpumplib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-15 12:51:40.000000 knvheatpumplib-0.0.9/knvheatpumplib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 12:51:40.000000 knvheatpumplib-0.0.9/knvheatpumplib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-15 12:51:40.000000 knvheatpumplib-0.0.9/knvheatpumplib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 12:51:40.252227 knvheatpumplib-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:40.252227 knvheatpumplib-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2023-10-15 12:51:30.000000 knvheatpumplib-0.0.9/tests/test_knvheatpump.py
```

### Comparing `knvheatpumplib-0.0.8/.github/workflows/pylint.yml` & `knvheatpumplib-0.0.9/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `knvheatpumplib-0.0.8/.github/workflows/python-app.yml` & `knvheatpumplib-0.0.9/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `knvheatpumplib-0.0.8/.github/workflows/python-publish.yml` & `knvheatpumplib-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `knvheatpumplib-0.0.8/.gitignore` & `knvheatpumplib-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `knvheatpumplib-0.0.8/LICENSE.md` & `knvheatpumplib-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `knvheatpumplib-0.0.8/PKG-INFO` & `knvheatpumplib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knvheatpumplib
-Version: 0.0.8
+Version: 0.0.9
 Summary: KNV heatpump Python library
 Author-email: LDprg <lukas_4dr@gmx.at>
 License: GPL-3
 Project-URL: Homepage, https://github.com/LDprg/KNV_heatpump_lib
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `knvheatpumplib-0.0.8/flake.lock` & `knvheatpumplib-0.0.9/flake.lock`

 * *Files identical despite different names*

### Comparing `knvheatpumplib-0.0.8/knvheatpumplib/knvparser.py` & `knvheatpumplib-0.0.9/knvheatpumplib/knvparser.py`

 * *Files identical despite different names*

### Comparing `knvheatpumplib-0.0.8/knvheatpumplib.egg-info/PKG-INFO` & `knvheatpumplib-0.0.9/knvheatpumplib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knvheatpumplib
-Version: 0.0.8
+Version: 0.0.9
 Summary: KNV heatpump Python library
 Author-email: LDprg <lukas_4dr@gmx.at>
 License: GPL-3
 Project-URL: Homepage, https://github.com/LDprg/KNV_heatpump_lib
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `knvheatpumplib-0.0.8/pyproject.toml` & `knvheatpumplib-0.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -28,8 +28,7 @@
 #     "async-timeout",
 #     "asyncio",
 #     "websockets",
 #     "requests",
 #     'importlib-metadata; python_version<"3.8"',
 # ]
 dynamic = ["version"]
-#version = "0.0.7"
```


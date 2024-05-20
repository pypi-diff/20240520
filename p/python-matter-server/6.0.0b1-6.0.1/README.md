# Comparing `tmp/python_matter_server-6.0.0b1.tar.gz` & `tmp/python_matter_server-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_matter_server-6.0.0b1.tar", last modified: Wed May  8 20:06:09 2024, max compression
+gzip compressed data, was "python_matter_server-6.0.1.tar", last modified: Mon May 20 14:54:23 2024, max compression
```

## Comparing `python_matter_server-6.0.0b1.tar` & `python_matter_server-6.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.816553 python_matter_server-6.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-05-08 20:06:09.816553 python_matter_server-6.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.804553 python_matter_server-6.0.0b1/matter_server/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.804553 python_matter_server-6.0.0b1/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29900 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.804553 python_matter_server-6.0.0b1/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/models/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 20:06:06.000000 python_matter_server-6.0.0b1/matter_server/dashboard/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/dashboard/js/
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-08 20:06:06.000000 python_matter_server-6.0.0b1/matter_server/dashboard/js/dialog-box-ztARVrB9.js
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-08 20:06:06.000000 python_matter_server-6.0.0b1/matter_server/dashboard/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)   230455 2024-05-08 20:06:06.000000 python_matter_server-6.0.0b1/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    62667 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.812553 python_matter_server-6.0.0b1/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/custom_web_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-08 20:05:52.000000 python_matter_server-6.0.0b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.812553 python_matter_server-6.0.0b1/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:06:09.816553 python_matter_server-6.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.308885 python_matter_server-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-05-20 14:54:23.308885 python_matter_server-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29900 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/models/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-20 14:54:21.000000 python_matter_server-6.0.1/matter_server/dashboard/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/dashboard/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-20 14:54:21.000000 python_matter_server-6.0.1/matter_server/dashboard/js/dialog-box-ztARVrB9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-20 14:54:21.000000 python_matter_server-6.0.1/matter_server/dashboard/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)   230455 2024-05-20 14:54:21.000000 python_matter_server-6.0.1/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.304885 python_matter_server-6.0.1/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62667 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.304885 python_matter_server-6.0.1/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/custom_web_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-20 14:54:09.000000 python_matter_server-6.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.304885 python_matter_server-6.0.1/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:54:23.308885 python_matter_server-6.0.1/setup.cfg
```

### Comparing `python_matter_server-6.0.0b1/LICENSE` & `python_matter_server-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/PKG-INFO` & `python_matter_server-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 6.0.0b1
+Version: 6.0.1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -15,36 +15,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
 Requires-Dist: orjson
-Requires-Dist: home-assistant-chip-clusters==2024.4.1
+Requires-Dist: home-assistant-chip-clusters==2024.5.0
 Provides-Extra: server
 Requires-Dist: aiohttp==3.9.5; extra == "server"
-Requires-Dist: aiorun==2023.7.2; extra == "server"
+Requires-Dist: aiorun==2024.5.1; extra == "server"
 Requires-Dist: async-timeout==4.0.3; extra == "server"
 Requires-Dist: coloredlogs==15.0.1; extra == "server"
-Requires-Dist: cryptography==42.0.6; extra == "server"
-Requires-Dist: orjson==3.9.15; extra == "server"
+Requires-Dist: cryptography==42.0.7; extra == "server"
+Requires-Dist: orjson==3.10.3; extra == "server"
 Requires-Dist: zeroconf==0.132.2; extra == "server"
-Requires-Dist: home-assistant-chip-core==2024.4.1; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.5.0; extra == "server"
 Provides-Extra: test
 Requires-Dist: codespell==2.2.6; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
-Requires-Dist: pre-commit==3.7.0; extra == "test"
+Requires-Dist: pre-commit==3.7.1; extra == "test"
 Requires-Dist: pre-commit-hooks==4.6.0; extra == "test"
-Requires-Dist: pylint==3.1.0; extra == "test"
-Requires-Dist: pytest==8.2.0; extra == "test"
-Requires-Dist: pytest-asyncio==0.23.6; extra == "test"
+Requires-Dist: pylint==3.2.2; extra == "test"
+Requires-Dist: pytest==8.2.1; extra == "test"
+Requires-Dist: pytest-asyncio==0.23.7; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.4.3; extra == "test"
+Requires-Dist: ruff==0.4.4; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
 as a base and provides both a server and client implementation.
```

### Comparing `python_matter_server-6.0.0b1/README.md` & `python_matter_server-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/client/client.py` & `python_matter_server-6.0.1/matter_server/client/client.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/client/connection.py` & `python_matter_server-6.0.1/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/client/exceptions.py` & `python_matter_server-6.0.1/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/client/models/clusters.py` & `python_matter_server-6.0.1/matter_server/client/models/clusters.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/client/models/device_types.py` & `python_matter_server-6.0.1/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/client/models/node.py` & `python_matter_server-6.0.1/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/common/errors.py` & `python_matter_server-6.0.1/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/common/helpers/api.py` & `python_matter_server-6.0.1/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/common/helpers/json.py` & `python_matter_server-6.0.1/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/common/helpers/util.py` & `python_matter_server-6.0.1/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/common/models.py` & `python_matter_server-6.0.1/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/dashboard/index.html` & `python_matter_server-6.0.1/matter_server/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/dashboard/js/dialog-box-ztARVrB9.js` & `python_matter_server-6.0.1/matter_server/dashboard/js/dialog-box-ztARVrB9.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/dashboard/js/main.js` & `python_matter_server-6.0.1/matter_server/dashboard/js/main.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js` & `python_matter_server-6.0.1/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/__main__.py` & `python_matter_server-6.0.1/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/client_handler.py` & `python_matter_server-6.0.1/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/const.py` & `python_matter_server-6.0.1/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/device_controller.py` & `python_matter_server-6.0.1/matter_server/server/device_controller.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/helpers/attributes.py` & `python_matter_server-6.0.1/matter_server/server/helpers/attributes.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/helpers/custom_web_runner.py` & `python_matter_server-6.0.1/matter_server/server/helpers/custom_web_runner.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/helpers/paa_certificates.py` & `python_matter_server-6.0.1/matter_server/server/helpers/paa_certificates.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
             # Old certificate store version, delete all files
             LOGGER.info("Old PAA root certificate store found, removing certificates.")
             for path in paa_root_cert_dir.iterdir():
                 if not path.is_dir():
                     path.unlink()
         else:
-            paa_root_cert_dir.mkdir()
+            paa_root_cert_dir.mkdir(parents=True)
         return None
 
     last_fetch = await loop.run_in_executor(
         None, _check_paa_root_dir, paa_root_cert_dir, paa_root_cert_dir_version
     )
     if last_fetch and last_fetch > datetime.now(tz=UTC) - timedelta(days=1):
         LOGGER.info("Skip fetching certificates (already fetched within the last 24h).")
```

### Comparing `python_matter_server-6.0.0b1/matter_server/server/helpers/utils.py` & `python_matter_server-6.0.1/matter_server/server/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/server.py` & `python_matter_server-6.0.1/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/stack.py` & `python_matter_server-6.0.1/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/storage.py` & `python_matter_server-6.0.1/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/matter_server/server/vendor_info.py` & `python_matter_server-6.0.1/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b1/pyproject.toml` & `python_matter_server-6.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,48 +18,48 @@
 ]
 dependencies = [
     "aiohttp",
     "aiorun",
     "async-timeout",
     "coloredlogs",
     "orjson",
-    "home-assistant-chip-clusters==2024.4.1",
+    "home-assistant-chip-clusters==2024.5.0",
 ]
 description = "Python Matter WebSocket Server"
 name = "python-matter-server"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "6.0.0b1"
+version = "6.0.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 server = [
     "aiohttp==3.9.5",
-    "aiorun==2023.7.2",
+    "aiorun==2024.5.1",
     "async-timeout==4.0.3",
     "coloredlogs==15.0.1",
-    "cryptography==42.0.6",
-    "orjson==3.9.15",
+    "cryptography==42.0.7",
+    "orjson==3.10.3",
     "zeroconf==0.132.2",
-    "home-assistant-chip-core==2024.4.1",
+    "home-assistant-chip-core==2024.5.0",
 ]
 test = [
     "codespell==2.2.6",
     "isort==5.13.2",
     "mypy==1.10.0",
-    "pre-commit==3.7.0",
+    "pre-commit==3.7.1",
     "pre-commit-hooks==4.6.0",
-    "pylint==3.1.0",
-    "pytest==8.2.0",
-    "pytest-asyncio==0.23.6",
+    "pylint==3.2.2",
+    "pytest==8.2.1",
+    "pytest-asyncio==0.23.7",
     "pytest-aiohttp==1.0.5",
     "pytest-cov==5.0.0",
-    "ruff==0.4.3",
+    "ruff==0.4.4",
     "tomli==2.0.1",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
 
 [tool.codespell]
```

### Comparing `python_matter_server-6.0.0b1/python_matter_server.egg-info/PKG-INFO` & `python_matter_server-6.0.1/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 6.0.0b1
+Version: 6.0.1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -15,36 +15,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
 Requires-Dist: orjson
-Requires-Dist: home-assistant-chip-clusters==2024.4.1
+Requires-Dist: home-assistant-chip-clusters==2024.5.0
 Provides-Extra: server
 Requires-Dist: aiohttp==3.9.5; extra == "server"
-Requires-Dist: aiorun==2023.7.2; extra == "server"
+Requires-Dist: aiorun==2024.5.1; extra == "server"
 Requires-Dist: async-timeout==4.0.3; extra == "server"
 Requires-Dist: coloredlogs==15.0.1; extra == "server"
-Requires-Dist: cryptography==42.0.6; extra == "server"
-Requires-Dist: orjson==3.9.15; extra == "server"
+Requires-Dist: cryptography==42.0.7; extra == "server"
+Requires-Dist: orjson==3.10.3; extra == "server"
 Requires-Dist: zeroconf==0.132.2; extra == "server"
-Requires-Dist: home-assistant-chip-core==2024.4.1; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.5.0; extra == "server"
 Provides-Extra: test
 Requires-Dist: codespell==2.2.6; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
-Requires-Dist: pre-commit==3.7.0; extra == "test"
+Requires-Dist: pre-commit==3.7.1; extra == "test"
 Requires-Dist: pre-commit-hooks==4.6.0; extra == "test"
-Requires-Dist: pylint==3.1.0; extra == "test"
-Requires-Dist: pytest==8.2.0; extra == "test"
-Requires-Dist: pytest-asyncio==0.23.6; extra == "test"
+Requires-Dist: pylint==3.2.2; extra == "test"
+Requires-Dist: pytest==8.2.1; extra == "test"
+Requires-Dist: pytest-asyncio==0.23.7; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.4.3; extra == "test"
+Requires-Dist: ruff==0.4.4; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
 as a base and provides both a server and client implementation.
```

### Comparing `python_matter_server-6.0.0b1/python_matter_server.egg-info/SOURCES.txt` & `python_matter_server-6.0.1/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*


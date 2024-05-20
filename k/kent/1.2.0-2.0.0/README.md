# Comparing `tmp/kent-1.2.0.tar.gz` & `tmp/kent-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kent-1.2.0.tar", last modified: Wed Jan 31 14:27:28 2024, max compression
+gzip compressed data, was "kent-2.0.0.tar", last modified: Mon May 20 01:14:24 2024, max compression
```

## Comparing `kent-1.2.0.tar` & `kent-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-01-31 14:27:28.179886 kent-1.2.0/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      566 2023-09-20 00:52:36.000000 kent-1.2.0/Dockerfile
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2487 2024-01-31 14:27:04.000000 kent-1.2.0/HISTORY.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2022-01-04 19:37:36.000000 kent-1.2.0/LICENSE
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      263 2023-11-06 19:59:19.000000 kent-1.2.0/MANIFEST.in
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      987 2024-01-31 00:38:49.000000 kent-1.2.0/Makefile
--rw-r--r--   0 willkg    (1000) willkg    (1000)     4834 2024-01-31 14:27:28.179886 kent-1.2.0/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     3460 2024-01-31 13:52:59.000000 kent-1.2.0/README.rst
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-01-31 14:27:28.179886 kent-1.2.0/bin/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      823 2022-06-13 13:59:41.000000 kent-1.2.0/bin/kent_submit.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2279 2024-01-31 14:27:04.000000 kent-1.2.0/pyproject.toml
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       38 2024-01-31 14:27:28.179886 kent-1.2.0/setup.cfg
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-01-31 14:27:28.175886 kent-1.2.0/src/
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-01-31 14:27:28.179886 kent-1.2.0/src/kent/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      402 2023-11-06 20:06:10.000000 kent-1.2.0/src/kent/__init__.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     9362 2024-01-31 13:52:59.000000 kent-1.2.0/src/kent/app.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1112 2024-01-31 14:20:14.000000 kent-1.2.0/src/kent/cli_server.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4670 2023-11-06 23:24:24.000000 kent-1.2.0/src/kent/cli_testpost.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-01-31 14:27:28.179886 kent-1.2.0/src/kent/static/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1150 2022-01-04 14:18:49.000000 kent-1.2.0/src/kent/static/favicon.ico
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    72244 2022-06-13 14:01:58.000000 kent-1.2.0/src/kent/static/pico.1.5.3.min.css
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1066 2022-01-01 08:49:10.000000 kent-1.2.0/src/kent/static/pico_LICENSE.md
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       74 2022-06-13 14:01:58.000000 kent-1.2.0/src/kent/static/style.css
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-01-31 14:27:28.179886 kent-1.2.0/src/kent/templates/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4460 2022-06-13 14:01:58.000000 kent-1.2.0/src/kent/templates/index.html
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-01-31 14:27:28.179886 kent-1.2.0/src/kent.egg-info/
--rw-r--r--   0 willkg    (1000) willkg    (1000)     4834 2024-01-31 14:27:28.000000 kent-1.2.0/src/kent.egg-info/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      544 2024-01-31 14:27:28.000000 kent-1.2.0/src/kent.egg-info/SOURCES.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2024-01-31 14:27:28.000000 kent-1.2.0/src/kent.egg-info/dependency_links.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       92 2024-01-31 14:27:28.000000 kent-1.2.0/src/kent.egg-info/entry_points.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       97 2024-01-31 14:27:28.000000 kent-1.2.0/src/kent.egg-info/requires.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)        5 2024-01-31 14:27:28.000000 kent-1.2.0/src/kent.egg-info/top_level.txt
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-01-31 14:27:28.179886 kent-1.2.0/tests/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2963 2023-11-06 19:19:46.000000 kent-1.2.0/tests/test_app.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-05-20 01:14:24.934504 kent-2.0.0/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      566 2023-09-20 00:52:36.000000 kent-2.0.0/Dockerfile
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     3556 2024-05-20 01:13:51.000000 kent-2.0.0/HISTORY.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2022-01-04 19:37:36.000000 kent-2.0.0/LICENSE
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      263 2023-11-06 19:59:19.000000 kent-2.0.0/MANIFEST.in
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      987 2024-01-31 00:38:49.000000 kent-2.0.0/Makefile
+-rw-r--r--   0 willkg    (1000) willkg    (1000)     4828 2024-05-20 01:14:24.934504 kent-2.0.0/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     3462 2024-05-20 01:09:11.000000 kent-2.0.0/README.rst
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-05-20 01:14:24.932504 kent-2.0.0/bin/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      823 2022-06-13 13:59:41.000000 kent-2.0.0/bin/kent_submit.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2259 2024-05-20 01:13:51.000000 kent-2.0.0/pyproject.toml
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       38 2024-05-20 01:14:24.934504 kent-2.0.0/setup.cfg
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-05-20 01:14:24.932504 kent-2.0.0/src/
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-05-20 01:14:24.932504 kent-2.0.0/src/kent/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      402 2023-11-06 20:06:10.000000 kent-2.0.0/src/kent/__init__.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    12481 2024-05-20 01:09:11.000000 kent-2.0.0/src/kent/app.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1112 2024-01-31 14:20:14.000000 kent-2.0.0/src/kent/cli_server.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     4894 2024-05-20 01:09:11.000000 kent-2.0.0/src/kent/cli_testpost.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-05-20 01:14:24.933504 kent-2.0.0/src/kent/static/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1150 2022-01-04 14:18:49.000000 kent-2.0.0/src/kent/static/favicon.ico
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    72244 2022-06-13 14:01:58.000000 kent-2.0.0/src/kent/static/pico.1.5.3.min.css
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1066 2022-01-01 08:49:10.000000 kent-2.0.0/src/kent/static/pico_LICENSE.md
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      184 2024-05-20 01:09:11.000000 kent-2.0.0/src/kent/static/style.css
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-05-20 01:14:24.933504 kent-2.0.0/src/kent/templates/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     6034 2024-05-20 01:09:11.000000 kent-2.0.0/src/kent/templates/index.html
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2800 2024-05-20 01:09:11.000000 kent-2.0.0/src/kent/utils.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-05-20 01:14:24.933504 kent-2.0.0/src/kent.egg-info/
+-rw-r--r--   0 willkg    (1000) willkg    (1000)     4828 2024-05-20 01:14:24.000000 kent-2.0.0/src/kent.egg-info/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      582 2024-05-20 01:14:24.000000 kent-2.0.0/src/kent.egg-info/SOURCES.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2024-05-20 01:14:24.000000 kent-2.0.0/src/kent.egg-info/dependency_links.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       92 2024-05-20 01:14:24.000000 kent-2.0.0/src/kent.egg-info/entry_points.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       89 2024-05-20 01:14:24.000000 kent-2.0.0/src/kent.egg-info/requires.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)        5 2024-05-20 01:14:24.000000 kent-2.0.0/src/kent.egg-info/top_level.txt
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-05-20 01:14:24.933504 kent-2.0.0/tests/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    11554 2024-05-20 01:09:11.000000 kent-2.0.0/tests/test_app.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     7355 2024-05-20 01:09:11.000000 kent-2.0.0/tests/test_utils.py
```

### Comparing `kent-1.2.0/Dockerfile` & `kent-2.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `kent-1.2.0/LICENSE` & `kent-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kent-1.2.0/Makefile` & `kent-2.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `kent-1.2.0/PKG-INFO` & `kent-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kent
-Version: 1.2.0
+Version: 2.0.0
 Summary: Fake Sentry service for debugging and integration tests
 Author: Will Kahn-Greene
 License: MPLv2
 Project-URL: Homepage, https://github.com/willkg/kent/
 Project-URL: Source, https://github.com/willkg/kent/
 Project-URL: Issues, https://github.com/willkg/kent/issues
 Keywords: sentry,integration service,test
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: flask<3,>=2.1.0
+Requires-Dist: flask>3
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sentry-sdk; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -47,15 +47,15 @@
 Goals
 =====
 
 Goals of Kent:
 
 1. make it possible to debug ``before_send`` and ``before_breadcrumb``
    sanitization code when using sentry-sdk
-2. make it possible to debug other sentry error submission payload issues
+2. make it possible to debug other sentry event submission payload issues
 3. make it possible to write integration tests against a fake sentry instance
 
 
 Quick start
 ===========
 
 Installing and running on your local machine
@@ -116,45 +116,45 @@
     $ docker run --init --rm --publish 8000:8000 kent:latest run --host 0.0.0.0 --port 8000
 
 
 Things to know about Kent
 =========================
 
 Kent is the fakest of fake Sentry servers. You can set up a Sentry DSN to point
-to Kent and have your application send errors to it.
+to Kent and have your application send events to it.
 
 Kent is for testing sentry-sdk things. Kent is not for testing Relay.
 
 Kent is a refined fake Sentry service and doesn't like fast food.
 
 Kent will keep track of the last 100 payloads it received in memory. Nothing is
 persisted to disk.
 
-You can access the list of errors and error data with your web browser by going
+You can access the list of events and event data with your web browser by going
 to Kent's index page.
 
 You can also access it with the API. This is most useful for integration tests
-that want to assert things about errors.
+that want to assert things about events.
 
-``GET /api/errorlist/``
-    List of all errors in memory with a unique error id.
+``GET /api/eventlist/``
+    List of all events in memory with a unique event id.
 
-``GET /api/error/ERRORID``
-    Retrieve the payload for a specific error by id.
+``GET /api/event/EVENT_ID``
+    Retrieve the payload for a specific event by id.
 
 ``POST /api/flush/``
-    Flushes the error manager of all errors.
+    Flushes the event manager of all events.
 
-You can use multiple project ids. Kent will keep the errors separate.
+You can use multiple project ids. Kent will keep the events separate.
 
 If you run ``kent-server run`` with the defaults, your DSN is::
 
     http://public@localhost:5000/1    for project id 1
     http://public@localhost:5000/2    for project id 2
-    ...
+    etc.
 
 
 Kent definitely works with:
 
 * Python sentry-sdk client
 * Python raven client (deprecated)
```

### Comparing `kent-1.2.0/README.rst` & `kent-2.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Goals
 =====
 
 Goals of Kent:
 
 1. make it possible to debug ``before_send`` and ``before_breadcrumb``
    sanitization code when using sentry-sdk
-2. make it possible to debug other sentry error submission payload issues
+2. make it possible to debug other sentry event submission payload issues
 3. make it possible to write integration tests against a fake sentry instance
 
 
 Quick start
 ===========
 
 Installing and running on your local machine
@@ -81,45 +81,45 @@
     $ docker run --init --rm --publish 8000:8000 kent:latest run --host 0.0.0.0 --port 8000
 
 
 Things to know about Kent
 =========================
 
 Kent is the fakest of fake Sentry servers. You can set up a Sentry DSN to point
-to Kent and have your application send errors to it.
+to Kent and have your application send events to it.
 
 Kent is for testing sentry-sdk things. Kent is not for testing Relay.
 
 Kent is a refined fake Sentry service and doesn't like fast food.
 
 Kent will keep track of the last 100 payloads it received in memory. Nothing is
 persisted to disk.
 
-You can access the list of errors and error data with your web browser by going
+You can access the list of events and event data with your web browser by going
 to Kent's index page.
 
 You can also access it with the API. This is most useful for integration tests
-that want to assert things about errors.
+that want to assert things about events.
 
-``GET /api/errorlist/``
-    List of all errors in memory with a unique error id.
+``GET /api/eventlist/``
+    List of all events in memory with a unique event id.
 
-``GET /api/error/ERRORID``
-    Retrieve the payload for a specific error by id.
+``GET /api/event/EVENT_ID``
+    Retrieve the payload for a specific event by id.
 
 ``POST /api/flush/``
-    Flushes the error manager of all errors.
+    Flushes the event manager of all events.
 
-You can use multiple project ids. Kent will keep the errors separate.
+You can use multiple project ids. Kent will keep the events separate.
 
 If you run ``kent-server run`` with the defaults, your DSN is::
 
     http://public@localhost:5000/1    for project id 1
     http://public@localhost:5000/2    for project id 2
-    ...
+    etc.
 
 
 Kent definitely works with:
 
 * Python sentry-sdk client
 * Python raven client (deprecated)
```

### Comparing `kent-1.2.0/bin/kent_submit.py` & `kent-2.0.0/bin/kent_submit.py`

 * *Files identical despite different names*

### Comparing `kent-1.2.0/pyproject.toml` & `kent-2.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "kent"
 description = "Fake Sentry service for debugging and integration tests"
-version = "1.2.0"
+version = "2.0.0"
 readme = "README.rst"
 keywords = ["sentry", "integration service", "test"]
 authors = [{name = "Will Kahn-Greene"}]
 license = {text = "MPLv2"}
 requires-python = ">=3.8"
-dependencies = ["flask>=2.1.0,<3"]
+dependencies = ["flask>3"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
@@ -44,26 +44,24 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [tool.ruff]
-# Enable pycodestyle (E), pyflakes (F), and bugbear (B) rules
-select = ["E", "F", "B"]
-
-# Ignore line length violations
 line-length = 88
-ignore = ["E501"]
-
 target-version = "py38"
-
 src = ["src", "tests"]
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint]
+# Enable pycodestyle (E), pyflakes (F), and bugbear (B) rules
+select = ["E", "F", "B"]
+ignore = ["E501"]
+
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
     "ignore:::babel[.*]",
```

### Comparing `kent-1.2.0/src/kent/cli_server.py` & `kent-2.0.0/src/kent/cli_server.py`

 * *Files identical despite different names*

### Comparing `kent-1.2.0/src/kent/cli_testpost.py` & `kent-2.0.0/src/kent/cli_testpost.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import argparse
+from importlib.metadata import version as metadata_version
 import logging
 from urllib.parse import urlparse
 import sys
 
 try:
     import requests
 except ImportError:
@@ -36,14 +37,16 @@
     )
 
     args = parser.parse_args()
 
     logging.basicConfig(level=logging.ERROR)
     init(args.dsn)
 
+    print(f"DSN: {args.dsn}")
+    print(f"Sentry-sdk version: {metadata_version('sentry_sdk')}")
     if args.kind == "message":
         capture_message("test error capture")
         print(f"Message posted to: {args.dsn}")
         return
 
     elif args.kind == "error":
         try:
@@ -65,14 +68,15 @@
         parsed = urlparse(args.dsn)
         report_uri = f"{parsed.scheme}://{parsed.username}@{parsed.netloc}/api{parsed.path}/security/"
 
         data = None
 
         if args.kind == "security_csp_new":
             # Newer browsers send this structure
+            # From: https://w3c.github.io/reporting/#sample-reports
             data = [
                 {
                     "age": 0,
                     "body": {
                         "blockedURL": "https://maps.googleapis.com/maps/api/js",
                         "disposition": "enforce",
                         "documentURL": "https://test.example.com/",
```

### Comparing `kent-1.2.0/src/kent/static/favicon.ico` & `kent-2.0.0/src/kent/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kent-1.2.0/src/kent/static/pico.1.5.3.min.css` & `kent-2.0.0/src/kent/static/pico.1.5.3.min.css`

 * *Files identical despite different names*

### Comparing `kent-1.2.0/src/kent/static/pico_LICENSE.md` & `kent-2.0.0/src/kent/static/pico_LICENSE.md`

 * *Files identical despite different names*

### Comparing `kent-1.2.0/src/kent.egg-info/PKG-INFO` & `kent-2.0.0/src/kent.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kent
-Version: 1.2.0
+Version: 2.0.0
 Summary: Fake Sentry service for debugging and integration tests
 Author: Will Kahn-Greene
 License: MPLv2
 Project-URL: Homepage, https://github.com/willkg/kent/
 Project-URL: Source, https://github.com/willkg/kent/
 Project-URL: Issues, https://github.com/willkg/kent/issues
 Keywords: sentry,integration service,test
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: flask<3,>=2.1.0
+Requires-Dist: flask>3
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sentry-sdk; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -47,15 +47,15 @@
 Goals
 =====
 
 Goals of Kent:
 
 1. make it possible to debug ``before_send`` and ``before_breadcrumb``
    sanitization code when using sentry-sdk
-2. make it possible to debug other sentry error submission payload issues
+2. make it possible to debug other sentry event submission payload issues
 3. make it possible to write integration tests against a fake sentry instance
 
 
 Quick start
 ===========
 
 Installing and running on your local machine
@@ -116,45 +116,45 @@
     $ docker run --init --rm --publish 8000:8000 kent:latest run --host 0.0.0.0 --port 8000
 
 
 Things to know about Kent
 =========================
 
 Kent is the fakest of fake Sentry servers. You can set up a Sentry DSN to point
-to Kent and have your application send errors to it.
+to Kent and have your application send events to it.
 
 Kent is for testing sentry-sdk things. Kent is not for testing Relay.
 
 Kent is a refined fake Sentry service and doesn't like fast food.
 
 Kent will keep track of the last 100 payloads it received in memory. Nothing is
 persisted to disk.
 
-You can access the list of errors and error data with your web browser by going
+You can access the list of events and event data with your web browser by going
 to Kent's index page.
 
 You can also access it with the API. This is most useful for integration tests
-that want to assert things about errors.
+that want to assert things about events.
 
-``GET /api/errorlist/``
-    List of all errors in memory with a unique error id.
+``GET /api/eventlist/``
+    List of all events in memory with a unique event id.
 
-``GET /api/error/ERRORID``
-    Retrieve the payload for a specific error by id.
+``GET /api/event/EVENT_ID``
+    Retrieve the payload for a specific event by id.
 
 ``POST /api/flush/``
-    Flushes the error manager of all errors.
+    Flushes the event manager of all events.
 
-You can use multiple project ids. Kent will keep the errors separate.
+You can use multiple project ids. Kent will keep the events separate.
 
 If you run ``kent-server run`` with the defaults, your DSN is::
 
     http://public@localhost:5000/1    for project id 1
     http://public@localhost:5000/2    for project id 2
-    ...
+    etc.
 
 
 Kent definitely works with:
 
 * Python sentry-sdk client
 * Python raven client (deprecated)
```

### Comparing `kent-1.2.0/src/kent.egg-info/SOURCES.txt` & `kent-2.0.0/src/kent.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 README.rst
 pyproject.toml
 bin/kent_submit.py
 src/kent/__init__.py
 src/kent/app.py
 src/kent/cli_server.py
 src/kent/cli_testpost.py
+src/kent/utils.py
 src/kent.egg-info/PKG-INFO
 src/kent.egg-info/SOURCES.txt
 src/kent.egg-info/dependency_links.txt
 src/kent.egg-info/entry_points.txt
 src/kent.egg-info/requires.txt
 src/kent.egg-info/top_level.txt
 src/kent/static/favicon.ico
 src/kent/static/pico.1.5.3.min.css
 src/kent/static/pico_LICENSE.md
 src/kent/static/style.css
 src/kent/templates/index.html
-tests/test_app.py
+tests/test_app.py
+tests/test_utils.py
```


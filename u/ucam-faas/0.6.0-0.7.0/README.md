# Comparing `tmp/ucam_faas-0.6.0.tar.gz` & `tmp/ucam_faas-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam_faas-0.6.0.tar", max compression
+gzip compressed data, was "ucam_faas-0.7.0.tar", max compression
```

## Comparing `ucam_faas-0.6.0.tar` & `ucam_faas-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3834 2024-04-22 13:48:17.943519 ucam_faas-0.6.0/README.md
--rw-r--r--   0        0        0     3131 2024-05-17 09:51:24.289336 ucam_faas-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7220 2024-05-17 09:40:34.340852 ucam_faas-0.6.0/ucam_faas/__init__.py
--rw-r--r--   0        0        0      106 2024-05-13 16:04:34.383948 ucam_faas-0.6.0/ucam_faas/exceptions.py
--rw-r--r--   0        0        0      581 2024-05-14 20:49:42.585515 ucam_faas-0.6.0/ucam_faas/testing.py
--rw-r--r--   0        0        0        0 2024-05-17 10:36:33.665400 ucam_faas-0.6.0/ucam_faas/tests/__init__.py
--rw-r--r--   0        0        0     2557 2024-05-15 12:27:31.175522 ucam_faas-0.6.0/ucam_faas/tests/test_ucam_faas.py
--rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 ucam_faas-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3834 2024-04-22 13:48:17.943519 ucam_faas-0.7.0/README.md
+-rw-r--r--   0        0        0     3131 2024-05-20 12:40:13.550042 ucam_faas-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3854 2024-05-20 12:28:25.976527 ucam_faas-0.7.0/ucam_faas/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-13 16:04:34.383948 ucam_faas-0.7.0/ucam_faas/exceptions.py
+-rw-r--r--   0        0        0      581 2024-05-14 20:49:42.585515 ucam_faas-0.7.0/ucam_faas/testing.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:25:27.449057 ucam_faas-0.7.0/ucam_faas/tests/__init__.py
+-rw-r--r--   0        0        0     2557 2024-05-15 12:27:31.175522 ucam_faas-0.7.0/ucam_faas/tests/test_ucam_faas.py
+-rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 ucam_faas-0.7.0/PKG-INFO
```

### Comparing `ucam_faas-0.6.0/README.md` & `ucam_faas-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ucam_faas-0.6.0/pyproject.toml` & `ucam_faas-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ucam-faas"
-version = "0.6.0"
+version = "0.7.0"
 description = "Opinionated FaaS support framework extending Google's functions-framework"
 authors = ["University of Cambridge Information Services <devops-wilson@uis.cam.ac.uk>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.developers.cam.ac.uk/uis/devops/ucam-faas-python/ucam-faas"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -76,15 +76,15 @@
 functions-framework = "^3.5.0"
 click = "^8.1.7"
 gunicorn = "^22.0.0"
 flask = "^3.0.3"
 pytest = {version = "^8.1.1", optional = true}
 polyfactory = {version = "^2.16.0", optional = true}
 cloudevents = {extras = ["pydantic"], version = "^1.10.1"}
-ucam-observe = "^0.1.1"
+ucam-observe = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
 tox = "^4.14.2"
 
 [tool.poetry.extras]
```

### Comparing `ucam_faas-0.6.0/ucam_faas/testing.py` & `ucam_faas-0.7.0/ucam_faas/testing.py`

 * *Files identical despite different names*

### Comparing `ucam_faas-0.6.0/ucam_faas/tests/test_ucam_faas.py` & `ucam_faas-0.7.0/ucam_faas/tests/test_ucam_faas.py`

 * *Files identical despite different names*

### Comparing `ucam_faas-0.6.0/PKG-INFO` & `ucam_faas-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam-faas
-Version: 0.6.0
+Version: 0.7.0
 Summary: Opinionated FaaS support framework extending Google's functions-framework
 Home-page: https://gitlab.developers.cam.ac.uk/uis/devops/ucam-faas-python/ucam-faas
 License: MIT
 Author: University of Cambridge Information Services
 Author-email: devops-wilson@uis.cam.ac.uk
 Requires-Python: >=3.9.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,15 @@
 Requires-Dist: flask (>=3.0.3,<4.0.0)
 Requires-Dist: functions-framework (>=3.5.0,<4.0.0)
 Requires-Dist: gunicorn (>=22.0.0,<23.0.0)
 Requires-Dist: polyfactory (>=2.16.0,<3.0.0) ; extra == "testing"
 Requires-Dist: pytest (>=8.1.1,<9.0.0) ; extra == "testing"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
-Requires-Dist: ucam-observe (>=0.1.1,<0.2.0)
+Requires-Dist: ucam-observe (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://gitlab.developers.cam.ac.uk/uis/devops/ucam-faas-python/ucam-faas
 Description-Content-Type: text/markdown
 
 # UCam FaaS Library
 
 This project contains a support library and base Docker image to be used to
 create Function as a Service (FaaS) applications intended to be deployed to a
```


# Comparing `tmp/qase_robotframework-3.0.0b1.tar.gz` & `tmp/qase_robotframework-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_robotframework-3.0.0b1.tar", last modified: Mon May  6 09:41:56 2024, max compression
+gzip compressed data, was "qase_robotframework-3.0.0b2.tar", last modified: Mon May 20 09:23:34 2024, max compression
```

## Comparing `qase_robotframework-3.0.0b1.tar` & `qase_robotframework-3.0.0b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.227186 qase_robotframework-3.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.227186 qase_robotframework-3.0.0b1/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/src/qaseio/robotframework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/src/qaseio/robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/src/qaseio/robotframework/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/src/qaseio/robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/src/qaseio/robotframework/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:34.884266 qase_robotframework-3.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-20 09:23:29.000000 qase_robotframework-3.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-20 09:23:34.884266 qase_robotframework-3.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-20 09:23:29.000000 qase_robotframework-3.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-20 09:23:29.000000 qase_robotframework-3.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:23:34.884266 qase_robotframework-3.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:34.880266 qase_robotframework-3.0.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:34.884266 qase_robotframework-3.0.0b2/src/qase_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-20 09:23:34.000000 qase_robotframework-3.0.0b2/src/qase_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 09:23:34.000000 qase_robotframework-3.0.0b2/src/qase_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:23:34.000000 qase_robotframework-3.0.0b2/src/qase_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 09:23:34.000000 qase_robotframework-3.0.0b2/src/qase_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 09:23:34.000000 qase_robotframework-3.0.0b2/src/qase_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:34.880266 qase_robotframework-3.0.0b2/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:34.884266 qase_robotframework-3.0.0b2/src/qaseio/robotframework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 09:23:29.000000 qase_robotframework-3.0.0b2/src/qaseio/robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-20 09:23:29.000000 qase_robotframework-3.0.0b2/src/qaseio/robotframework/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-20 09:23:29.000000 qase_robotframework-3.0.0b2/src/qaseio/robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 09:23:29.000000 qase_robotframework-3.0.0b2/src/qaseio/robotframework/types.py
```

### Comparing `qase_robotframework-3.0.0b1/LICENSE` & `qase_robotframework-3.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `qase_robotframework-3.0.0b1/PKG-INFO` & `qase_robotframework-3.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-robotframework
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: Qase Robot Framework Plugin
 Author-email: Qase Team <support@qase.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qase_robotframework-3.0.0b1/README.md` & `qase_robotframework-3.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `qase_robotframework-3.0.0b1/pyproject.toml` & `qase_robotframework-3.0.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-robotframework"
-version = "3.0.0b1"
+version = "3.0.0b2"
 description = "Qase Robot Framework Plugin"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Robot Framework",
```

### Comparing `qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/PKG-INFO` & `qase_robotframework-3.0.0b2/src/qase_robotframework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-robotframework
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: Qase Robot Framework Plugin
 Author-email: Qase Team <support@qase.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qase_robotframework-3.0.0b1/src/qaseio/robotframework/listener.py` & `qase_robotframework-3.0.0b2/src/qaseio/robotframework/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import re
 import uuid
 
 from qase.commons import ConfigManager
-from qase.commons.models import Result, Suite, Step
+from qase.commons.models import Result, Suite, Step, Field
 from qase.commons.models.step import StepType, StepGherkinData
 from qase.commons.reporters import QaseCoreReporter
 from qase.commons.models.runtime import Runtime
 
 from .types import STATUSES
 from .models import *
 
@@ -43,34 +43,32 @@
         }
         logger.debug("Starting suite '%s'", name)
 
     def start_test(self, name, attributes: StartTestModel):
         logger.debug("Starting test '%s'", name)
 
         self.runtime.result = Result(title=name, signature=name)
-
+        self.runtime.steps = {}
         case_id = self._extract_ids(attributes.get("tags"))
 
         if case_id:
             self.runtime.result.testops_id = int(case_id)
 
     def end_test(self, name, attributes: EndTestModel):
         logger.debug("Finishing test '%s'", name)
 
         self.runtime.result.execution.complete()
         self.runtime.result.execution.set_status(STATUSES[attributes.get("status")])
         self.runtime.result.execution.stacktrace = attributes.get("message")
         self.runtime.result.add_steps([step for key, step in self.runtime.steps.items()])
 
-        if self.runtime.result.testops_id is None:
-            self.runtime.result.case.title = name
-            self.runtime.result.case.description = attributes.get("doc")
+        self.runtime.result.add_field(Field("description", attributes.get("doc")))
 
-            if self.suite:
-                self.runtime.result.suite = Suite(self.suite.get("title"), self.suite.get("description"))
+        if self.suite:
+            self.runtime.result.suite = Suite(self.suite.get("title"), self.suite.get("description"))
 
         self.reporter.add_result(self.runtime.result)
 
         self.step_uuid = None
 
         logger.info(
             "Finished case result: %s, error: %s",
```

### Comparing `qase_robotframework-3.0.0b1/src/qaseio/robotframework/models.py` & `qase_robotframework-3.0.0b2/src/qaseio/robotframework/models.py`

 * *Files identical despite different names*


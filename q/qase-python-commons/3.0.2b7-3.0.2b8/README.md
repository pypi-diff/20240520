# Comparing `tmp/qase_python_commons-3.0.2b7.tar.gz` & `tmp/qase_python_commons-3.0.2b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_python_commons-3.0.2b7.tar", last modified: Mon May 13 15:28:47 2024, max compression
+gzip compressed data, was "qase_python_commons-3.0.2b8.tar", last modified: Mon May 20 09:23:05 2024, max compression
```

## Comparing `qase_python_commons-3.0.2b7.tar` & `qase_python_commons-3.0.2b8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.410839 qase_python_commons-3.0.2b7/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-13 15:28:47.410839 qase_python_commons-3.0.2b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:28:47.410839 qase_python_commons-3.0.2b7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.402839 qase_python_commons-3.0.2b7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.402839 qase_python_commons-3.0.2b7/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.402839 qase_python_commons-3.0.2b7/src/qase/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/client/
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/client/api_v1_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/client/api_v2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/client/base_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/exceptions/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/profilers/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/profilers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/profilers/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/reporters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/reporters/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/reporters/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/validators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.410839 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.374483 qase_python_commons-3.0.2b8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:23:05.374483 qase_python_commons-3.0.2b8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.362483 qase_python_commons-3.0.2b8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.362483 qase_python_commons-3.0.2b8/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.366483 qase_python_commons-3.0.2b8/src/qase/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.366483 qase_python_commons-3.0.2b8/src/qase/commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/client/api_v1_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/client/api_v2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/client/base_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.366483 qase_python_commons-3.0.2b8/src/qase/commons/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/exceptions/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.366483 qase_python_commons-3.0.2b8/src/qase/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/models/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/src/qase/commons/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/profilers/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/profilers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/profilers/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/src/qase/commons/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/reporters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/reporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/reporters/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/src/qase/commons/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-20 09:22:58.000000 qase_python_commons-3.0.2b8/src/qase/commons/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:23:05.370483 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 09:23:05.000000 qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/top_level.txt
```

### Comparing `qase_python_commons-3.0.2b7/PKG-INFO` & `qase_python_commons-3.0.2b8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b7
+Version: 3.0.2b8
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qase_python_commons-3.0.2b7/pyproject.toml` & `qase_python_commons-3.0.2b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "3.0.2b7"
+version = "3.0.2b8"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/client/api_v1_client.py` & `qase_python_commons-3.0.2b8/src/qase/commons/client/api_v1_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/client/api_v2_client.py` & `qase_python_commons-3.0.2b8/src/qase/commons/client/api_v2_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/client/base_api_client.py` & `qase_python_commons-3.0.2b8/src/qase/commons/client/base_api_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/config.py` & `qase_python_commons-3.0.2b8/src/qase/commons/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                     self._set_config(key[len(env_vars_prefix):].lower().replace('_', '.'), value)
         except Exception as e:
             self.logger.log("Failed to load config from env vars {e}", "error")
 
     def get(self, key, default=None, value_type=None):
         # Use _get_config method to get the value. If None, return default.
         value = self._get_config(key)
-        if value_type and value_type == bool:
+        if value and value_type and value_type == bool:
             return self.parseBool(value)
         return value or default
 
     def validate_config(self):
         if self.validator:
             self.validator.validate(self.config)
```

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/loader.py` & `qase_python_commons-3.0.2b8/src/qase/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/logger.py` & `qase_python_commons-3.0.2b8/src/qase/commons/logger.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/models/attachment.py` & `qase_python_commons-3.0.2b8/src/qase/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/models/result.py` & `qase_python_commons-3.0.2b8/src/qase/commons/models/result.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/models/run.py` & `qase_python_commons-3.0.2b8/src/qase/commons/models/run.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/models/runtime.py` & `qase_python_commons-3.0.2b8/src/qase/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/models/step.py` & `qase_python_commons-3.0.2b8/src/qase/commons/models/step.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/profilers/network.py` & `qase_python_commons-3.0.2b8/src/qase/commons/profilers/network.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/profilers/sleep.py` & `qase_python_commons-3.0.2b8/src/qase/commons/profilers/sleep.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/reporters/core.py` & `qase_python_commons-3.0.2b8/src/qase/commons/reporters/core.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/reporters/report.py` & `qase_python_commons-3.0.2b8/src/qase/commons/reporters/report.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/reporters/testops.py` & `qase_python_commons-3.0.2b8/src/qase/commons/reporters/testops.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.complete_after_run = self.config.get('testops.run.complete', True, bool)
         self.environment = None
 
         self.batch_size = min(2000, max(1, int(self.config.get('testops.batch.size', DEFAULT_BATCH_SIZE))))
         self.send_semaphore = threading.Semaphore(
             self.config.get('testops.batch.threads', 4))  # Semaphore to limit concurrent sends
         self.lock = threading.Lock()
+        self.count_running_threads = 0
 
         environment = self.config.get('environment', None)
         if environment:
             if isinstance(environment, int) or (isinstance(environment, str) and environment.isnumeric()):
                 self.environment = environment
             elif isinstance(environment, str):
                 self.environment = self.client.get_environment(environment, self.project_code)
@@ -76,20 +77,22 @@
             with self.lock:
                 self.processed.extend(results)
         except Exception as e:
             with self.lock:
                 self.logger.log(f"Error at sending results for run {self.run_id}: {e}", "error")
             raise  # Re-raise the exception to be caught by the thread handler
         finally:
+            self.count_running_threads -= 1
             self.send_semaphore.release()  # Release semaphore whether success or exception
 
     def _send_results(self) -> None:
         if self.results:
             # Acquire semaphore before starting the send operation
             self.send_semaphore.acquire()
+            self.count_running_threads += 1
             results_to_send = self.results.copy()
             self.results = []
 
             # Start a new thread for sending results
             send_thread = threading.Thread(target=self._send_results_threaded, args=(results_to_send,))
             send_thread.start()
         else:
@@ -111,14 +114,16 @@
             raise ReporterException("Unable to find given test run.")
         return self.run_id
 
     def complete_run(self) -> None:
         if len(self.results) > 0:
             self._send_results()
         if self.complete_after_run:
+            while self.count_running_threads > 0:
+                pass
             self.client.complete_run(self.project_code, self.run_id)
 
     def complete_worker(self) -> None:
         if len(self.results) > 0:
             self._send_results()
 
     def add_result(self, result: Result) -> None:
```

### Comparing `qase_python_commons-3.0.2b7/src/qase/commons/utils.py` & `qase_python_commons-3.0.2b8/src/qase/commons/utils.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/PKG-INFO` & `qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b7
+Version: 3.0.2b8
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/SOURCES.txt` & `qase_python_commons-3.0.2b8/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*


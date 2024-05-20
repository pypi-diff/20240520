# Comparing `tmp/lambdatest-sdk-utils-1.0.1.tar.gz` & `tmp/lambdatest_sdk_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambdatest-sdk-utils-1.0.1.tar", last modified: Wed Jan 31 18:27:35 2024, max compression
+gzip compressed data, was "lambdatest_sdk_utils-1.0.2.tar", last modified: Mon May 20 14:46:48 2024, max compression
```

## Comparing `lambdatest-sdk-utils-1.0.1.tar` & `lambdatest_sdk_utils-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 18:27:35.616204 lambdatest-sdk-utils-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-31 18:27:35.616204 lambdatest-sdk-utils-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 18:27:35.616204 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-31 18:27:27.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-31 18:27:27.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-31 18:27:27.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-31 18:27:27.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-31 18:27:27.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 18:27:35.616204 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-31 18:27:35.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-01-31 18:27:35.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 18:27:35.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-31 18:27:35.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-31 18:27:35.000000 lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 18:27:35.616204 lambdatest-sdk-utils-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-31 18:27:27.000000 lambdatest-sdk-utils-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:46:48.732546 lambdatest_sdk_utils-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 14:46:48.732546 lambdatest_sdk_utils-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:46:48.728546 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-20 14:46:40.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-20 14:46:40.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-20 14:46:40.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-20 14:46:40.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 14:46:40.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:46:48.732546 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 14:46:48.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-20 14:46:48.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:46:48.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 14:46:48.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 14:46:48.000000 lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:46:48.732546 lambdatest_sdk_utils-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-20 14:46:40.000000 lambdatest_sdk_utils-1.0.2/setup.py
```

### Comparing `lambdatest-sdk-utils-1.0.1/PKG-INFO` & `lambdatest_sdk_utils-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdatest-sdk-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: SDK utils
 Home-page: https://github.com/LambdaTest/lambdatest-python-sdk
 Author: LambdaTest <keys@lambdatest.com>
 License: MIT
 Keywords: lambdatest python selenium sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils/rest.py` & `lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils/rest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from lambdatest_sdk_utils.constants import get_smart_ui_server_address
 from lambdatest_sdk_utils.logger import get_logger
 
-logger = get_logger()
+logger = get_logger('lambdatest_sdk_utils')
 
 def is_smartui_enabled():
     try:
         response = requests.get(f'{get_smart_ui_server_address()}/healthcheck')
         response.raise_for_status()
         return True
     except Exception as e:
```

### Comparing `lambdatest-sdk-utils-1.0.1/lambdatest_sdk_utils.egg-info/PKG-INFO` & `lambdatest_sdk_utils-1.0.2/lambdatest_sdk_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdatest-sdk-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: SDK utils
 Home-page: https://github.com/LambdaTest/lambdatest-python-sdk
 Author: LambdaTest <keys@lambdatest.com>
 License: MIT
 Keywords: lambdatest python selenium sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lambdatest-sdk-utils-1.0.1/setup.py` & `lambdatest_sdk_utils-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import lambdatest_sdk_utils
 
 setup(
     name="lambdatest-sdk-utils",
-    version="1.0.1",
+    version="1.0.2",
     author="LambdaTest <keys@lambdatest.com>",
     description="SDK utils",
     long_description="SDK utils for lambdatest",
     long_description_content_type="text/markdown",
     url="https://github.com/LambdaTest/lambdatest-python-sdk",
     keywords="lambdatest python selenium sdk",
     packages=find_packages(),
```


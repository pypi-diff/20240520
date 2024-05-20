# Comparing `tmp/lambdatest-selenium-driver-1.0.3.tar.gz` & `tmp/lambdatest_selenium_driver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambdatest-selenium-driver-1.0.3.tar", last modified: Tue Feb 13 14:06:01 2024, max compression
+gzip compressed data, was "lambdatest_selenium_driver-1.0.4.tar", last modified: Mon May 20 14:47:38 2024, max compression
```

## Comparing `lambdatest-selenium-driver-1.0.3.tar` & `lambdatest_selenium_driver-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:06:01.085804 lambdatest-selenium-driver-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-02-13 14:06:01.085804 lambdatest-selenium-driver-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:06:01.081804 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-13 14:05:50.000000 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-13 14:05:50.000000 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver/smartui.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-13 14:05:50.000000 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:06:01.081804 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-02-13 14:06:01.000000 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-13 14:06:01.000000 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 14:06:01.000000 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-13 14:06:01.000000 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-13 14:06:01.000000 lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 14:06:01.085804 lambdatest-selenium-driver-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-13 14:05:50.000000 lambdatest-selenium-driver-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:47:38.685344 lambdatest_selenium_driver-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-20 14:47:38.685344 lambdatest_selenium_driver-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:47:38.685344 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 14:47:29.000000 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-20 14:47:29.000000 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver/smartui.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 14:47:29.000000 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:47:38.685344 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-20 14:47:38.000000 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-20 14:47:38.000000 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:47:38.000000 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 14:47:38.000000 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 14:47:38.000000 lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:47:38.685344 lambdatest_selenium_driver-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-20 14:47:29.000000 lambdatest_selenium_driver-1.0.4/setup.py
```

### Comparing `lambdatest-selenium-driver-1.0.3/PKG-INFO` & `lambdatest_selenium_driver-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdatest-selenium-driver
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Selenium SDK for testing with Smart UI
 Home-page: https://github.com/LambdaTest/lambdatest-python-sdk
 Author: LambdaTest <keys@lambdatest.com>
 License: MIT
 Keywords: lambdatest python selenium sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver/smartui.py` & `lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver/smartui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from lambdatest_sdk_utils import is_smartui_enabled,fetch_dom_serializer,post_snapshot
-from lambdatest_sdk_utils import get_pkg_name,setup_logger,get_logger
+from lambdatest_sdk_utils import setup_logger,get_logger
 
 
 def smartui_snapshot(driver, name,options={}):
     # setting up logger
     setup_logger()
-    logger = get_logger()
+    logger = get_logger('lambdatest-selenium-driver')
 
     if not name:
         raise Exception('The `snapshotName` argument is required.')
     if is_smartui_enabled() is False: 
         raise Exception("Cannot find SmartUI server.")
     
     try:
@@ -25,15 +25,15 @@
                 url: document.URL
             }}
             """
         )
 
         # Post the dom to smartui endpoint
         dom['name'] = name
-        res = post_snapshot(dom,get_pkg_name(),options=options)
+        res = post_snapshot(dom,'lambdatest-selenium-driver',options=options)
 
         if res and res.get('data') and res['data'].get('warnings') and len(res['data']['warnings']) != 0:
             for warning in res['data']['warnings']:
                 logger.warn(warning)
 
         logger.info(f'Snapshot captured {name}')
     except Exception as e:
```

### Comparing `lambdatest-selenium-driver-1.0.3/lambdatest_selenium_driver.egg-info/PKG-INFO` & `lambdatest_selenium_driver-1.0.4/lambdatest_selenium_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdatest-selenium-driver
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Selenium SDK for testing with Smart UI
 Home-page: https://github.com/LambdaTest/lambdatest-python-sdk
 Author: LambdaTest <keys@lambdatest.com>
 License: MIT
 Keywords: lambdatest python selenium sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lambdatest-selenium-driver-1.0.3/setup.py` & `lambdatest_selenium_driver-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 cwd = path.abspath(path.dirname(__file__))
 with open(path.join(cwd, 'readme.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="lambdatest-selenium-driver",
-    version="1.0.3",
+    version="1.0.4",
     author="LambdaTest <keys@lambdatest.com>",
     description="Python Selenium SDK for testing with Smart UI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LambdaTest/lambdatest-python-sdk",
     keywords="lambdatest python selenium sdk",
     packages=find_packages(),
```


# Comparing `tmp/ca_vntl_helper-1.1.1.tar.gz` & `tmp/ca_vntl_helper-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ca_vntl_helper-1.1.1.tar", last modified: Mon May 20 07:35:22 2024, max compression
+gzip compressed data, was "ca_vntl_helper-1.1.2.tar", last modified: Mon May 20 07:45:27 2024, max compression
```

## Comparing `ca_vntl_helper-1.1.1.tar` & `ca_vntl_helper-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:35:22.948644 ca_vntl_helper-1.1.1/
--rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.1/LICENSE
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 07:35:22.948402 ca_vntl_helper-1.1.1/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.1/README.md
--rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-20 07:35:20.000000 ca_vntl_helper-1.1.1/pyproject.toml
--rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-20 07:35:22.948694 ca_vntl_helper-1.1.1/setup.cfg
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:35:22.946104 ca_vntl_helper-1.1.1/src/
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:35:22.946744 ca_vntl_helper-1.1.1/src/ca_vntl_helper/
--rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper/__init__.py
--rw-r--r--   0 s19404     (502) staff       (20)     3469 2024-05-20 07:34:39.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper/decorator.py
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:35:22.948123 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 07:35:22.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-20 07:35:22.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/SOURCES.txt
--rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-20 07:35:22.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/dependency_links.txt
--rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-20 07:35:22.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/top_level.txt
--rw-r--r--   0 s19404     (502) staff       (20)     1669 2024-05-20 07:33:54.000000 ca_vntl_helper-1.1.1/src/test.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:45:27.337623 ca_vntl_helper-1.1.2/
+-rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.2/LICENSE
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 07:45:27.337387 ca_vntl_helper-1.1.2/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.2/README.md
+-rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-20 07:42:23.000000 ca_vntl_helper-1.1.2/pyproject.toml
+-rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-20 07:45:27.337687 ca_vntl_helper-1.1.2/setup.cfg
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:45:27.335244 ca_vntl_helper-1.1.2/src/
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:45:27.335895 ca_vntl_helper-1.1.2/src/ca_vntl_helper/
+-rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper/__init__.py
+-rw-r--r--   0 s19404     (502) staff       (20)     3578 2024-05-20 07:41:51.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper/decorator.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:45:27.337133 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 07:45:27.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-20 07:45:27.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-20 07:45:27.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-20 07:45:27.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/top_level.txt
+-rw-r--r--   0 s19404     (502) staff       (20)     1670 2024-05-20 07:37:23.000000 ca_vntl_helper-1.1.2/src/test.py
```

### Comparing `ca_vntl_helper-1.1.1/LICENSE` & `ca_vntl_helper-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.1.1/PKG-INFO` & `ca_vntl_helper-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.1.1
+Version: 1.1.2
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.1.1/README.md` & `ca_vntl_helper-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.1.1/pyproject.toml` & `ca_vntl_helper-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ca-vntl-helper"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Bui Ngoc Huy Van", email="bui_ngoc_huy_van@ca-adv.co.jp" },
 ]
 description = "Some useful functions, classes to help work. Create by Van of Techlab CA team."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ca_vntl_helper-1.1.1/src/ca_vntl_helper/decorator.py` & `ca_vntl_helper-1.1.2/src/ca_vntl_helper/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,17 +47,17 @@
                     message = create_message_detail(error_detail, params)
                 messages += message
             logging.error(messages)
             raise e
     return wrapper
 
 class ErrorTrackerWithCallBacks:
-    def __init__(self, callback_functions=None):
+    def __init__(self, callback_functions=None, is_raise_error=True):
         self.callback_functions = callback_functions
-
+        self.is_raise_error = is_raise_error
     def error_tracking_decorator(self, func):
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except Exception as e:
                 exc = sys.exception()
                 # print(exc.__traceback__)
@@ -76,11 +76,12 @@
                         message = create_message_detail(error_detail, params)
                     messages += message
                 if self.callback_functions:
                     for callback_function in self.callback_functions:
                         callback_function(messages)
                 else:
                     logging.error(messages)
-                raise e
+                if self.is_raise_error:
+                    raise e
 
         return wrapper
```

### Comparing `ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/PKG-INFO` & `ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.1.1
+Version: 1.1.2
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.1.1/src/test.py` & `ca_vntl_helper-1.1.2/src/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 error_tracking_decorator_with_callbacks = error_tracker.error_tracking_decorator
 
 def divide(a, b):
     current_time = datetime.now() - timedelta(10)
     try:
         c = a / b
     except Exception as e:
-        raise e
+        print(e)
     return None
 
 
 
 def second_inner_function(second_inner_a, second_inner_b):
     return divide(second_inner_a, second_inner_b)
```


# Comparing `tmp/ca_vntl_helper-1.1.2.tar.gz` & `tmp/ca_vntl_helper-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ca_vntl_helper-1.1.2.tar", last modified: Mon May 20 07:45:27 2024, max compression
+gzip compressed data, was "ca_vntl_helper-1.1.3.tar", last modified: Mon May 20 09:24:48 2024, max compression
```

## Comparing `ca_vntl_helper-1.1.2.tar` & `ca_vntl_helper-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:45:27.337623 ca_vntl_helper-1.1.2/
--rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.2/LICENSE
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 07:45:27.337387 ca_vntl_helper-1.1.2/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.2/README.md
--rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-20 07:42:23.000000 ca_vntl_helper-1.1.2/pyproject.toml
--rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-20 07:45:27.337687 ca_vntl_helper-1.1.2/setup.cfg
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:45:27.335244 ca_vntl_helper-1.1.2/src/
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:45:27.335895 ca_vntl_helper-1.1.2/src/ca_vntl_helper/
--rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper/__init__.py
--rw-r--r--   0 s19404     (502) staff       (20)     3578 2024-05-20 07:41:51.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper/decorator.py
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:45:27.337133 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 07:45:27.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-20 07:45:27.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/SOURCES.txt
--rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-20 07:45:27.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/dependency_links.txt
--rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-20 07:45:27.000000 ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/top_level.txt
--rw-r--r--   0 s19404     (502) staff       (20)     1670 2024-05-20 07:37:23.000000 ca_vntl_helper-1.1.2/src/test.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 09:24:48.935604 ca_vntl_helper-1.1.3/
+-rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.3/LICENSE
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 09:24:48.935382 ca_vntl_helper-1.1.3/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.3/README.md
+-rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-20 09:24:44.000000 ca_vntl_helper-1.1.3/pyproject.toml
+-rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-20 09:24:48.935658 ca_vntl_helper-1.1.3/setup.cfg
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 09:24:48.933263 ca_vntl_helper-1.1.3/src/
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 09:24:48.933844 ca_vntl_helper-1.1.3/src/ca_vntl_helper/
+-rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.3/src/ca_vntl_helper/__init__.py
+-rw-r--r--   0 s19404     (502) staff       (20)     3748 2024-05-20 09:19:49.000000 ca_vntl_helper-1.1.3/src/ca_vntl_helper/decorator.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 09:24:48.935130 ca_vntl_helper-1.1.3/src/ca_vntl_helper.egg-info/
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 09:24:48.000000 ca_vntl_helper-1.1.3/src/ca_vntl_helper.egg-info/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-20 09:24:48.000000 ca_vntl_helper-1.1.3/src/ca_vntl_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-20 09:24:48.000000 ca_vntl_helper-1.1.3/src/ca_vntl_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-20 09:24:48.000000 ca_vntl_helper-1.1.3/src/ca_vntl_helper.egg-info/top_level.txt
+-rw-r--r--   0 s19404     (502) staff       (20)     1712 2024-05-20 09:20:26.000000 ca_vntl_helper-1.1.3/src/test.py
```

### Comparing `ca_vntl_helper-1.1.2/LICENSE` & `ca_vntl_helper-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.1.2/PKG-INFO` & `ca_vntl_helper-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.1.2
+Version: 1.1.3
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.1.2/README.md` & `ca_vntl_helper-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.1.2/pyproject.toml` & `ca_vntl_helper-1.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ca-vntl-helper"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Bui Ngoc Huy Van", email="bui_ngoc_huy_van@ca-adv.co.jp" },
 ]
 description = "Some useful functions, classes to help work. Create by Van of Techlab CA team."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ca_vntl_helper-1.1.2/src/ca_vntl_helper/decorator.py` & `ca_vntl_helper-1.1.3/src/ca_vntl_helper/decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,16 +55,20 @@
         self.callback_functions = callback_functions
         self.is_raise_error = is_raise_error
     def error_tracking_decorator(self, func):
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except Exception as e:
-                exc = sys.exception()
-                # print(exc.__traceback__)
+                # if python version >= 3.10, use sys.exc_info() instead of sys.exception()
+
+                if sys.version_info >= (3, 10):
+                    _, exc, _ = sys.exc_info()
+                else:
+                    exc = sys.exception()
                 errors_detail = traceback.extract_tb(exc.__traceback__)
                 formatted_lines = traceback.format_exc().splitlines()
                 frames = inspect.trace()
                 messages = f"Error in function {func.__name__} \n"
                 for idx, (frame, error_detail) in enumerate(zip(frames, errors_detail)):
                     if idx == 0:
                         continue
```

### Comparing `ca_vntl_helper-1.1.2/src/ca_vntl_helper.egg-info/PKG-INFO` & `ca_vntl_helper-1.1.3/src/ca_vntl_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.1.2
+Version: 1.1.3
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.1.2/src/test.py` & `ca_vntl_helper-1.1.3/src/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 error_tracking_decorator_with_callbacks = error_tracker.error_tracking_decorator
 
 def divide(a, b):
     current_time = datetime.now() - timedelta(10)
     try:
         c = a / b
     except Exception as e:
-        print(e)
+        raise Exception(f"Error when dividing {a} by {b}")
     return None
 
 
 
 def second_inner_function(second_inner_a, second_inner_b):
     return divide(second_inner_a, second_inner_b)
```


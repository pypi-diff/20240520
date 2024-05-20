# Comparing `tmp/ca_vntl_helper-1.1.0.tar.gz` & `tmp/ca_vntl_helper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ca_vntl_helper-1.1.0.tar", last modified: Mon May 20 03:54:24 2024, max compression
+gzip compressed data, was "ca_vntl_helper-1.1.1.tar", last modified: Mon May 20 07:35:22 2024, max compression
```

## Comparing `ca_vntl_helper-1.1.0.tar` & `ca_vntl_helper-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 03:54:24.742427 ca_vntl_helper-1.1.0/
--rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.0/LICENSE
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 03:54:24.742192 ca_vntl_helper-1.1.0/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.0/README.md
--rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-20 03:54:15.000000 ca_vntl_helper-1.1.0/pyproject.toml
--rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-20 03:54:24.742474 ca_vntl_helper-1.1.0/setup.cfg
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 03:54:24.739925 ca_vntl_helper-1.1.0/src/
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 03:54:24.740507 ca_vntl_helper-1.1.0/src/ca_vntl_helper/
--rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper/__init__.py
--rw-r--r--   0 s19404     (502) staff       (20)     3425 2024-05-20 03:53:36.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper/decorator.py
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 03:54:24.741947 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 03:54:24.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-20 03:54:24.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/SOURCES.txt
--rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-20 03:54:24.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/dependency_links.txt
--rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-20 03:54:24.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/top_level.txt
--rw-r--r--   0 s19404     (502) staff       (20)     1083 2024-05-20 03:22:55.000000 ca_vntl_helper-1.1.0/src/test.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:35:22.948644 ca_vntl_helper-1.1.1/
+-rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.1/LICENSE
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 07:35:22.948402 ca_vntl_helper-1.1.1/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.1/README.md
+-rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-20 07:35:20.000000 ca_vntl_helper-1.1.1/pyproject.toml
+-rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-20 07:35:22.948694 ca_vntl_helper-1.1.1/setup.cfg
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:35:22.946104 ca_vntl_helper-1.1.1/src/
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:35:22.946744 ca_vntl_helper-1.1.1/src/ca_vntl_helper/
+-rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper/__init__.py
+-rw-r--r--   0 s19404     (502) staff       (20)     3469 2024-05-20 07:34:39.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper/decorator.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 07:35:22.948123 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 07:35:22.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-20 07:35:22.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-20 07:35:22.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-20 07:35:22.000000 ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/top_level.txt
+-rw-r--r--   0 s19404     (502) staff       (20)     1669 2024-05-20 07:33:54.000000 ca_vntl_helper-1.1.1/src/test.py
```

### Comparing `ca_vntl_helper-1.1.0/LICENSE` & `ca_vntl_helper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.1.0/PKG-INFO` & `ca_vntl_helper-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.1.0
+Version: 1.1.1
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.1.0/README.md` & `ca_vntl_helper-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.1.0/pyproject.toml` & `ca_vntl_helper-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ca-vntl-helper"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Bui Ngoc Huy Van", email="bui_ngoc_huy_van@ca-adv.co.jp" },
 ]
 description = "Some useful functions, classes to help work. Create by Van of Techlab CA team."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ca_vntl_helper-1.1.0/src/ca_vntl_helper/decorator.py` & `ca_vntl_helper-1.1.1/src/ca_vntl_helper/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                 params = argvalues.locals
                 if idx == len(frames) - 1:
                     message = create_message_detail(error_detail, params, formatted_lines[-1])
                 else:
                     message = create_message_detail(error_detail, params)
                 messages += message
             logging.error(messages)
+            raise e
     return wrapper
 
 class ErrorTrackerWithCallBacks:
     def __init__(self, callback_functions=None):
         self.callback_functions = callback_functions
 
     def error_tracking_decorator(self, func):
@@ -75,10 +76,11 @@
                         message = create_message_detail(error_detail, params)
                     messages += message
                 if self.callback_functions:
                     for callback_function in self.callback_functions:
                         callback_function(messages)
                 else:
                     logging.error(messages)
+                raise e
 
         return wrapper
```

### Comparing `ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/PKG-INFO` & `ca_vntl_helper-1.1.1/src/ca_vntl_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.1.0
+Version: 1.1.1
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

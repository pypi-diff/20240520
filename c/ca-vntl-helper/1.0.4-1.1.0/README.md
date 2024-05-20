# Comparing `tmp/ca_vntl_helper-1.0.4.tar.gz` & `tmp/ca_vntl_helper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ca_vntl_helper-1.0.4.tar", last modified: Tue May 14 13:08:47 2024, max compression
+gzip compressed data, was "ca_vntl_helper-1.1.0.tar", last modified: Mon May 20 03:54:24 2024, max compression
```

## Comparing `ca_vntl_helper-1.0.4.tar` & `ca_vntl_helper-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 13:08:47.048016 ca_vntl_helper-1.0.4/
--rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.0.4/LICENSE
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-14 13:08:47.047789 ca_vntl_helper-1.0.4/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.0.4/README.md
--rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-14 13:08:33.000000 ca_vntl_helper-1.0.4/pyproject.toml
--rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-14 13:08:47.048072 ca_vntl_helper-1.0.4/setup.cfg
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 13:08:47.045470 ca_vntl_helper-1.0.4/src/
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 13:08:47.046165 ca_vntl_helper-1.0.4/src/ca_vntl_helper/
--rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.0.4/src/ca_vntl_helper/__init__.py
--rw-r--r--   0 s19404     (502) staff       (20)     3186 2024-05-14 09:41:02.000000 ca_vntl_helper-1.0.4/src/ca_vntl_helper/decorator.py
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-14 13:08:47.047544 ca_vntl_helper-1.0.4/src/ca_vntl_helper.egg-info/
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-14 13:08:47.000000 ca_vntl_helper-1.0.4/src/ca_vntl_helper.egg-info/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-14 13:08:47.000000 ca_vntl_helper-1.0.4/src/ca_vntl_helper.egg-info/SOURCES.txt
--rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-14 13:08:47.000000 ca_vntl_helper-1.0.4/src/ca_vntl_helper.egg-info/dependency_links.txt
--rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-14 13:08:47.000000 ca_vntl_helper-1.0.4/src/ca_vntl_helper.egg-info/top_level.txt
--rw-r--r--   0 s19404     (502) staff       (20)      993 2024-05-14 12:41:25.000000 ca_vntl_helper-1.0.4/src/test.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 03:54:24.742427 ca_vntl_helper-1.1.0/
+-rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.0/LICENSE
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 03:54:24.742192 ca_vntl_helper-1.1.0/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.0/README.md
+-rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-20 03:54:15.000000 ca_vntl_helper-1.1.0/pyproject.toml
+-rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-20 03:54:24.742474 ca_vntl_helper-1.1.0/setup.cfg
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 03:54:24.739925 ca_vntl_helper-1.1.0/src/
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 03:54:24.740507 ca_vntl_helper-1.1.0/src/ca_vntl_helper/
+-rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper/__init__.py
+-rw-r--r--   0 s19404     (502) staff       (20)     3425 2024-05-20 03:53:36.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper/decorator.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 03:54:24.741947 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 03:54:24.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-20 03:54:24.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-20 03:54:24.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-20 03:54:24.000000 ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/top_level.txt
+-rw-r--r--   0 s19404     (502) staff       (20)     1083 2024-05-20 03:22:55.000000 ca_vntl_helper-1.1.0/src/test.py
```

### Comparing `ca_vntl_helper-1.0.4/LICENSE` & `ca_vntl_helper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.0.4/PKG-INFO` & `ca_vntl_helper-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.0.4
+Version: 1.1.0
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.0.4/README.md` & `ca_vntl_helper-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.0.4/pyproject.toml` & `ca_vntl_helper-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ca-vntl-helper"
-version = "1.0.4"
+version = "1.1.0"
 authors = [
   { name="Bui Ngoc Huy Van", email="bui_ngoc_huy_van@ca-adv.co.jp" },
 ]
 description = "Some useful functions, classes to help work. Create by Van of Techlab CA team."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ca_vntl_helper-1.0.4/src/ca_vntl_helper/decorator.py` & `ca_vntl_helper-1.1.0/src/ca_vntl_helper/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 def create_message_detail(error_detail, params, root_cause=None):
     text_code = linecache.getline(error_detail.filename, error_detail.lineno)
     text_code = text_code.replace("\n", "")
     if root_cause:
         root_cause = f"\t-->ROOT CAUSE: {root_cause} \n"
     else:
         root_cause = ""
+    # check file contain site-packages or pyt
+    if "site-packages" in error_detail.filename:
+        note_message = "site-packages"
+    else:
+        note_message = "your code"
     message = f"===================================================\n" \
               f"Filename: {error_detail.filename},\n" \
               f"Function name: {error_detail.name}, params: {params}\n" \
               f"\t-----\n" \
               f"\tLine: {error_detail.lineno}, {text_code}\n {root_cause}" \
               f"\t-----\n" \
-
+              f"\tNote: This error is from {note_message}\n"
     return message
 
 
 def error_tracking_decorator(func):
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
```

### Comparing `ca_vntl_helper-1.0.4/src/ca_vntl_helper.egg-info/PKG-INFO` & `ca_vntl_helper-1.1.0/src/ca_vntl_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.0.4
+Version: 1.1.0
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.0.4/src/test.py` & `ca_vntl_helper-1.1.0/src/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from ca_vntl_helper import ErrorTrackerWithCallBacks
-
+from datetime import datetime, timedelta
 def send_message_to_slack(message):
     print("Message sent to slack:")
     print(message)
 def save_message_to_logfile_on_s3(message):
     print("Message saved to logfile on S3:")
     print(message)
 
 error_tracker = ErrorTrackerWithCallBacks(callback_functions=[send_message_to_slack, save_message_to_logfile_on_s3])
 
 error_tracking_decorator_with_callbacks = error_tracker.error_tracking_decorator
 
 def divide(a, b):
+    current_time = datetime.now() - timedelta(10)
     return a / b
 
 
 def second_inner_function(second_inner_a, second_inner_b):
     return divide(second_inner_a, second_inner_b)
```


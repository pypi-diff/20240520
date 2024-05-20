# Comparing `tmp/qualystbx-0.7.0.tar.gz` & `tmp/qualystbx-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualystbx-0.7.0.tar", last modified: Sun May 19 12:32:25 2024, max compression
+gzip compressed data, was "qualystbx-0.8.0.tar", last modified: Sun May 19 13:06:51 2024, max compression
```

## Comparing `qualystbx-0.7.0.tar` & `qualystbx-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:32:25.653533 qualystbx-0.7.0/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.7.0/LICENSE.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       20 2024-04-24 16:23:40.000000 qualystbx-0.7.0/MANIFEST.in
--rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-19 12:32:25.653533 qualystbx-0.7.0/PKG-INFO
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.7.0/README.md
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.7.0/license.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      103 2024-01-30 19:38:49.000000 qualystbx-0.7.0/pyproject.toml
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:32:25.649533 qualystbx-0.7.0/qualys_tbx/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.7.0/qualys_tbx/README.md
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       21 2024-05-19 12:32:07.000000 qualystbx-0.7.0/qualys_tbx/__init__.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:32:25.653533 qualystbx-0.7.0/qualys_tbx/qtbx_lib/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-03-28 10:53:29.000000 qualystbx-0.7.0/qualys_tbx/qtbx_lib/__init__.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3599 2024-05-14 05:39:58.000000 qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    17131 2024-05-14 04:00:20.000000 qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     4462 2024-05-18 12:24:25.000000 qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3131 2024-05-14 03:56:41.000000 qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     6824 2024-05-10 03:04:01.000000 qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:32:25.653533 qualystbx-0.7.0/qualys_tbx/qtbx_policy_merge/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-04-02 10:51:14.000000 qualystbx-0.7.0/qualys_tbx/qtbx_policy_merge/__init__.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    24191 2024-05-14 05:59:14.000000 qualystbx-0.7.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     9666 2024-05-19 12:32:06.000000 qualystbx-0.7.0/qualys_tbx/qualystbx.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:32:25.653533 qualystbx-0.7.0/qualystbx.egg-info/
--rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-19 12:32:25.000000 qualystbx-0.7.0/qualystbx.egg-info/PKG-INFO
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      635 2024-05-19 12:32:25.000000 qualystbx-0.7.0/qualystbx.egg-info/SOURCES.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        1 2024-05-19 12:32:25.000000 qualystbx-0.7.0/qualystbx.egg-info/dependency_links.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       56 2024-05-19 12:32:25.000000 qualystbx-0.7.0/qualystbx.egg-info/entry_points.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       11 2024-05-19 12:32:25.000000 qualystbx-0.7.0/qualystbx.egg-info/top_level.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       38 2024-05-19 12:32:25.653533 qualystbx-0.7.0/setup.cfg
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     1835 2024-05-19 12:32:07.000000 qualystbx-0.7.0/setup.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 13:06:51.529802 qualystbx-0.8.0/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.8.0/LICENSE.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       20 2024-04-24 16:23:40.000000 qualystbx-0.8.0/MANIFEST.in
+-rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-19 13:06:51.529802 qualystbx-0.8.0/PKG-INFO
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.8.0/README.md
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.8.0/license.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      103 2024-01-30 19:38:49.000000 qualystbx-0.8.0/pyproject.toml
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 13:06:51.525802 qualystbx-0.8.0/qualys_tbx/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.8.0/qualys_tbx/README.md
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       21 2024-05-19 13:06:15.000000 qualystbx-0.8.0/qualys_tbx/__init__.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 13:06:51.525802 qualystbx-0.8.0/qualys_tbx/qtbx_lib/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-03-28 10:53:29.000000 qualystbx-0.8.0/qualys_tbx/qtbx_lib/__init__.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3599 2024-05-14 05:39:58.000000 qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    17131 2024-05-14 04:00:20.000000 qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     4462 2024-05-18 12:24:25.000000 qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3131 2024-05-14 03:56:41.000000 qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     6824 2024-05-10 03:04:01.000000 qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 13:06:51.525802 qualystbx-0.8.0/qualys_tbx/qtbx_policy_merge/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-04-02 10:51:14.000000 qualystbx-0.8.0/qualys_tbx/qtbx_policy_merge/__init__.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    24191 2024-05-14 05:59:14.000000 qualystbx-0.8.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    10859 2024-05-19 13:06:15.000000 qualystbx-0.8.0/qualys_tbx/qualystbx.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 13:06:51.529802 qualystbx-0.8.0/qualystbx.egg-info/
+-rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-19 13:06:51.000000 qualystbx-0.8.0/qualystbx.egg-info/PKG-INFO
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      635 2024-05-19 13:06:51.000000 qualystbx-0.8.0/qualystbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        1 2024-05-19 13:06:51.000000 qualystbx-0.8.0/qualystbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       56 2024-05-19 13:06:51.000000 qualystbx-0.8.0/qualystbx.egg-info/entry_points.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       11 2024-05-19 13:06:51.000000 qualystbx-0.8.0/qualystbx.egg-info/top_level.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       38 2024-05-19 13:06:51.529802 qualystbx-0.8.0/setup.cfg
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     1835 2024-05-19 13:06:15.000000 qualystbx-0.8.0/setup.py
```

### Comparing `qualystbx-0.7.0/LICENSE.txt` & `qualystbx-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/PKG-INFO` & `qualystbx-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualystbx
-Version: 0.7.0
+Version: 0.8.0
 Summary: Qualys Tool Box - Tools for running various functions in Qualys.
 Home-page: https://pypi.org/project/qualystbx/
 Author: David Gregory
 Author-email: dgregory@qualys.com, dave@davidgregory.com
 License: Apache
 Project-URL: Documentation, https://dg-cafe.github.io/qualystbx/
 Keywords: qualys,qualystoolbox,qualys.com,david gregory,qualystbx,qualysapi
```

### Comparing `qualystbx-0.7.0/README.md` & `qualystbx-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/license.txt` & `qualystbx-0.8.0/license.txt`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/qualys_tbx/README.md` & `qualystbx-0.8.0/qualys_tbx/README.md`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py` & `qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py` & `qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py` & `qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py` & `qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py` & `qualystbx-0.8.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py` & `qualystbx-0.8.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/qualys_tbx/qualystbx.py` & `qualystbx-0.8.0/qualys_tbx/qualystbx.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,39 +45,64 @@
     if tool_selected_to_run in tool_list:
         return tool_selected_to_run
     else:
         print_usage(message=f"Tool Selected is invalid: {tool_selected_to_run}, please select tool from options.")
         sys.exit(1)
 
 
+# def determine_storage_dir():
+#     # Initialize a variable to hold the word following '--execute'
+#     storage_dir = None
+#     # Loop through each argument, stopping before the last to avoid IndexError
+#     for i in range(1, len(sys.argv) - 1):
+#         if sys.argv[i] == '--storage_dir':
+#             if i + 1 < len(sys.argv):
+#                 next_arg = sys.argv[i + 1]
+#                 # Check if the next argument starts with a letter or digit
+#                 if re.match(r"^[a-zA-Z0-9\\:_/-]+$", next_arg):
+#                     storage_dir = next_arg
+#                     break  # Exit the loop after finding and validating '--execute'
+#                 else:
+#                     print_usage(message="--storage_dir not selected. "
+#                                         "Please select a root storage directory. "
+#                                         "e.g.:--storage_dir=C:\\users\myname\Downloads")
+#                     sys.exit(1)
+#             else:
+#                 print_usage(message=f"--storage_dir invalid characters: {storage_dir}, please select another --storage_dir=path and rerun")
+#                 sys.exit(1)
+#     if storage_dir is None:
+#         storage_dir = os.path.expanduser('~')
+#
+#     return storage_dir
+
+
 def determine_storage_dir():
-    # Initialize a variable to hold the word following '--execute'
-    storage_dir = None
+    # Initialize storage_dir with the user's home directory by default
+    storage_dir = os.path.expanduser('~')
+
     # Loop through each argument, stopping before the last to avoid IndexError
     for i in range(1, len(sys.argv) - 1):
         if sys.argv[i] == '--storage_dir':
             if i + 1 < len(sys.argv):
                 next_arg = sys.argv[i + 1]
-                # Check if the next argument starts with a letter or digit
-                if re.match(r"^[a-zA-Z0-9\\:_/-]+$", next_arg):
+                # Check if the next argument is a valid file path
+                if re.match(r"^[a-zA-Z0-9_ /\\:.-]+$", next_arg):
                     storage_dir = next_arg
-                    break  # Exit the loop after finding and validating '--execute'
+                    break  # Exit the loop after finding and validating '--storage_dir'
                 else:
-                    print_usage(message="--storage_dir not selected. "
-                                        "Please select a root storage directory. "
-                                        "e.g.:--storage_dir=C:\\users\myname\Downloads")
-                    sys.exit(1)
+                    print_usage(message="Invalid --storage_dir path. "
+                                        "Please select a valid root storage directory. "
+                                        "e.g.: --storage_dir=C:\\users\\myname\\Downloads or --storage_dir=/home/myname/Downloads")
             else:
-                print_usage(message=f"--storage_dir invalid characters: {storage_dir}, please select another --storage_dir=path and rerun")
-                sys.exit(1)
-    if storage_dir is None:
-        storage_dir = os.path.expanduser('~')
+                print_usage(message=f"--storage_dir argument is missing a value.")
 
+    print(f"Using storage directory: {storage_dir}")
     return storage_dir
 
+
 def determine_log_to_console():
     log_to_console = False
     for i in range(1, len(sys.argv)):
         if sys.argv[i] == '--log_to_console':
             log_to_console = True
     return log_to_console
```

### Comparing `qualystbx-0.7.0/qualystbx.egg-info/PKG-INFO` & `qualystbx-0.8.0/qualystbx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualystbx
-Version: 0.7.0
+Version: 0.8.0
 Summary: Qualys Tool Box - Tools for running various functions in Qualys.
 Home-page: https://pypi.org/project/qualystbx/
 Author: David Gregory
 Author-email: dgregory@qualys.com, dave@davidgregory.com
 License: Apache
 Project-URL: Documentation, https://dg-cafe.github.io/qualystbx/
 Keywords: qualys,qualystoolbox,qualys.com,david gregory,qualystbx,qualysapi
```

### Comparing `qualystbx-0.7.0/qualystbx.egg-info/SOURCES.txt` & `qualystbx-0.8.0/qualystbx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qualystbx-0.7.0/setup.py` & `qualystbx-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 long_description = (here_qualys_tbx / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='qualystbx',
-    version='0.7.0',
+    version='0.8.0',
     packages=find_packages(include=[
         'qualys_tbx',
         'qualys_tbx.qtbx_lib',
         'qualys_tbx.qtbx_policy_merge',
         'qualys_tbx.*',
         'qualys_tbx.qtbx_lib.*',
         'qualys_tbx.qtbx_policy_merge.*',
```


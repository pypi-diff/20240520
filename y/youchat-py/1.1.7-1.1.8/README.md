# Comparing `tmp/youchat-py-1.1.7.tar.gz` & `tmp/youchat_py-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youchat-py-1.1.7.tar", last modified: Sat Sep 16 20:43:54 2023, max compression
+gzip compressed data, was "youchat_py-1.1.8.tar", last modified: Mon May 20 18:55:11 2024, max compression
```

## Comparing `youchat-py-1.1.7.tar` & `youchat_py-1.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:43:54.361486 youchat-py-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-09-16 20:43:44.000000 youchat-py-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2023-09-16 20:43:54.361486 youchat-py-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-09-16 20:43:44.000000 youchat-py-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2023-09-16 20:43:44.000000 youchat-py-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-16 20:43:54.361486 youchat-py-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-09-16 20:43:44.000000 youchat-py-1.1.7/youchat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:43:54.357486 youchat-py-1.1.7/youchat_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2023-09-16 20:43:54.000000 youchat-py-1.1.7/youchat_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-09-16 20:43:54.000000 youchat-py-1.1.7/youchat_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 20:43:54.000000 youchat-py-1.1.7/youchat_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-09-16 20:43:54.000000 youchat-py-1.1.7/youchat_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-16 20:43:54.000000 youchat-py-1.1.7/youchat_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-16 20:43:54.000000 youchat-py-1.1.7/youchat_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:11.886935 youchat_py-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-20 18:55:07.000000 youchat_py-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-20 18:55:11.886935 youchat_py-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-20 18:55:07.000000 youchat_py-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-20 18:55:07.000000 youchat_py-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:55:11.886935 youchat_py-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-20 18:55:07.000000 youchat_py-1.1.8/youchat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:55:11.886935 youchat_py-1.1.8/youchat_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-20 18:55:11.000000 youchat_py-1.1.8/youchat_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-20 18:55:11.000000 youchat_py-1.1.8/youchat_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:55:11.000000 youchat_py-1.1.8/youchat_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 18:55:11.000000 youchat_py-1.1.8/youchat_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 18:55:11.000000 youchat_py-1.1.8/youchat_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 18:55:11.000000 youchat_py-1.1.8/youchat_py.egg-info/top_level.txt
```

### Comparing `youchat-py-1.1.7/LICENSE` & `youchat_py-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `youchat-py-1.1.7/PKG-INFO` & `youchat_py-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youchat-py
-Version: 1.1.7
+Version: 1.1.8
 Summary: Simple communication with YouChat in python.
 License: BSD 2-Clause License
         
         Copyright (c) 2023, Yaroslavik
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -73,18 +73,18 @@
 ## Usage
 ```
 usage: youchat [-h] [-out_type OUT_TYPE] [-timeout TIMEOUT] MESSAGE
 
 positional arguments:
   MESSAGE               Message to YouChat
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -out_type OUT_TYPE, -ot OUT_TYPE
-                        Output type
+                        Output type (json/string)
   -timeout TIMEOUT, -t TIMEOUT
                         Timeout to wait response
 ```
 ### Example 1
 Use in CLI mode
 ```
 youchat hello!
@@ -105,10 +105,12 @@
 ```py
 from youchat import you_message
 
 print( you_message(text='Hello, World!', out_type="string") )
 ```
 **Returns:** `"Hello, World!" is a common phrase used in ...`
 
+## Problems and solutions
+If you often cannot get youchat response - try to update seleniumbase library `pip install -U seleniumbase`
 
 ## Used library
 - seleniumbase
```

### Comparing `youchat-py-1.1.7/README.md` & `youchat_py-1.1.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 ## Usage
 ```
 usage: youchat [-h] [-out_type OUT_TYPE] [-timeout TIMEOUT] MESSAGE
 
 positional arguments:
   MESSAGE               Message to YouChat
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -out_type OUT_TYPE, -ot OUT_TYPE
-                        Output type
+                        Output type (json/string)
   -timeout TIMEOUT, -t TIMEOUT
                         Timeout to wait response
 ```
 ### Example 1
 Use in CLI mode
 ```
 youchat hello!
@@ -47,10 +47,12 @@
 ```py
 from youchat import you_message
 
 print( you_message(text='Hello, World!', out_type="string") )
 ```
 **Returns:** `"Hello, World!" is a common phrase used in ...`
 
+## Problems and solutions
+If you often cannot get youchat response - try to update seleniumbase library `pip install -U seleniumbase`
 
 ## Used library
 - seleniumbase
```

### Comparing `youchat-py-1.1.7/pyproject.toml` & `youchat_py-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "youchat-py"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.7"  # Required
+version = "1.1.8"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Simple communication with YouChat in python."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `youchat-py-1.1.7/youchat.py` & `youchat_py-1.1.8/youchat.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             except Exception:
                 pass
 
             # START Try to easy solve captcha challenge
             try:
                 if sb.assert_element('iframe'):
                     sb.switch_to_frame("iframe")
-                    sb.find_element(".ctp-checkbox-label", timeout=1).click()
+                    sb.find_element(".cb-lb", timeout=1).click()
             except Exception:
                 result['error'] = 'Selenium was detected! Try again later. Captcha not solved automaticly.'
             finally:
                 # Force exit from iframe
                 sb.switch_to_default_content()
 
             if time.time() > timeout_delta:
@@ -65,15 +65,15 @@
                 'error' in result) else result['generated_text']
             return str_res
 
 
 def main_cli():
     parser = argparse.ArgumentParser()
     parser.add_argument('MESSAGE', help="Message to YouChat")
-    parser.add_argument('-out_type', '-ot', help="Output type", default="json")
+    parser.add_argument('-out_type', '-ot', help="Output type (json/string)", default="json")
     parser.add_argument(
         '-timeout', '-t', help="Timeout to wait response", default=20, type=int)
     args = parser.parse_args()
     print(you_message(args.MESSAGE, args.out_type, args.timeout))
 
 
 if __name__ == '__main__':
```

### Comparing `youchat-py-1.1.7/youchat_py.egg-info/PKG-INFO` & `youchat_py-1.1.8/youchat_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youchat-py
-Version: 1.1.7
+Version: 1.1.8
 Summary: Simple communication with YouChat in python.
 License: BSD 2-Clause License
         
         Copyright (c) 2023, Yaroslavik
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -73,18 +73,18 @@
 ## Usage
 ```
 usage: youchat [-h] [-out_type OUT_TYPE] [-timeout TIMEOUT] MESSAGE
 
 positional arguments:
   MESSAGE               Message to YouChat
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -out_type OUT_TYPE, -ot OUT_TYPE
-                        Output type
+                        Output type (json/string)
   -timeout TIMEOUT, -t TIMEOUT
                         Timeout to wait response
 ```
 ### Example 1
 Use in CLI mode
 ```
 youchat hello!
@@ -105,10 +105,12 @@
 ```py
 from youchat import you_message
 
 print( you_message(text='Hello, World!', out_type="string") )
 ```
 **Returns:** `"Hello, World!" is a common phrase used in ...`
 
+## Problems and solutions
+If you often cannot get youchat response - try to update seleniumbase library `pip install -U seleniumbase`
 
 ## Used library
 - seleniumbase
```


# Comparing `tmp/xspace-dl-0.2.1.tar.gz` & `tmp/xspace-dl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.2.1.tar", last modified: Mon May 20 14:14:29 2024, max compression
+gzip compressed data, was "xspace-dl-0.2.2.tar", last modified: Mon May 20 14:21:30 2024, max compression
```

## Comparing `xspace-dl-0.2.1.tar` & `xspace-dl-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:14:29.307877 xspace-dl-0.2.1/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 14:14:29.307676 xspace-dl-0.2.1/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 14:14:29.307924 xspace-dl-0.2.1/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      855 2024-05-20 14:14:13.000000 xspace-dl-0.2.1/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:14:29.306225 xspace-dl-0.2.1/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:11:45.000000 xspace-dl-0.2.1/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7378 2024-05-20 14:13:17.000000 xspace-dl-0.2.1/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6084 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7061 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:14:29.307431 xspace-dl-0.2.1/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:21:30.901268 xspace-dl-0.2.2/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 14:21:30.901008 xspace-dl-0.2.2/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 14:21:30.901387 xspace-dl-0.2.2/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      855 2024-05-20 14:21:27.000000 xspace-dl-0.2.2/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:21:30.897761 xspace-dl-0.2.2/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:11:45.000000 xspace-dl-0.2.2/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7416 2024-05-20 14:20:51.000000 xspace-dl-0.2.2/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6084 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7061 2024-05-20 14:08:08.000000 xspace-dl-0.2.2/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:21:30.900358 xspace-dl-0.2.2/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 14:21:30.000000 xspace-dl-0.2.2/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.2.1/LICENSE` & `xspace-dl-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.1/PKG-INFO` & `xspace-dl-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/rosebabaganoush/xspace-dl
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.1 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.2 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```

### Comparing `xspace-dl-0.2.1/README.md` & `xspace-dl-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.1/pyproject.toml` & `xspace-dl-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.1/setup.py` & `xspace-dl-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',
-    version='0.2.1',
+    version='0.2.2',
     author='Your Name',
     author_email='your.email@example.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rosebabaganoush/xspace-dl',
     packages=find_packages(),
```

### Comparing `xspace-dl-0.2.1/xspace/api.py` & `xspace-dl-0.2.2/xspace/api.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.1/xspace/cookies.py` & `xspace-dl-0.2.2/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.1/xspace/main.py` & `xspace-dl-0.2.2/xspace/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 from xspace.xspace import Xspace
 from xspace.xspace_dl import XspaceDL
 
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_ERROR = 1
 EXIT_CODE_MISUSE = 2
 
+
 def exception_hook(
     _: Type[BaseException],
     exc_value: BaseException,
     _t: TracebackType = None,
 ) -> None:
     """Make Exceptions more legible for the end users"""
+    # Exception type and value
     print(f"\033[31;1;4mError\033[0m: {exc_value}\nRetry with -v to see more details")
 
+
 def space(args: argparse.Namespace) -> int:
     """Manage the twitter space related function"""
     has_input = (
         args.user_url
         or args.input_url
         or args.input_metadata
         or args.from_dynamic_url
@@ -59,15 +62,15 @@
         logging.basicConfig(
             level=logging.DEBUG,
             format="%(asctime)s [%(levelname)s] %(message)s",
             handlers=handlers,
         )
 
     API.init_apis(load_cookies(args.input_cookie_file))
-
+    
     xspace_instance = None
     if args.user_url:
         xspace_instance = Xspace.from_user_avatar(args.user_url)
     elif args.input_metadata:
         xspace_instance = Xspace.from_file(args.input_metadata)
     elif args.input_url:
         xspace_instance = Xspace.from_space_url(args.input_url)
@@ -107,14 +110,15 @@
         except KeyboardInterrupt:
             logging.info("Download Interrupted by user")
         finally:
             if not args.keep_files:
                 xspace_dl.cleanup()
     return EXIT_CODE_SUCCESS
 
+
 def main() -> int:
     """Main function, creates the argument parser"""
     parser = argparse.ArgumentParser(
         description="Script designed to help download twitter spaces"
     )
 
     input_group = parser.add_argument_group("input")
```

### Comparing `xspace-dl-0.2.1/xspace/xspace.py` & `xspace-dl-0.2.2/xspace/xspace.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.1/xspace/xspace_dl.py` & `xspace-dl-0.2.2/xspace/xspace_dl.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.1/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.2.2/xspace_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/rosebabaganoush/xspace-dl
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.1 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.2 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```


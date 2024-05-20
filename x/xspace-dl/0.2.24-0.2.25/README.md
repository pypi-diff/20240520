# Comparing `tmp/xspace-dl-0.2.24.tar.gz` & `tmp/xspace-dl-0.2.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.2.24.tar", last modified: Mon May 20 15:13:47 2024, max compression
+gzip compressed data, was "xspace-dl-0.2.25.tar", last modified: Mon May 20 15:40:45 2024, max compression
```

## Comparing `xspace-dl-0.2.24.tar` & `xspace-dl-0.2.25.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:13:47.288847 xspace-dl-0.2.24/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.24/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:13:47.288673 xspace-dl-0.2.24/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.24/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.24/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 15:13:47.288896 xspace-dl-0.2.24/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 15:13:37.000000 xspace-dl-0.2.24/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:13:47.287287 xspace-dl-0.2.24/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.2.24/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16585 2024-05-20 15:13:19.000000 xspace-dl-0.2.24/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.24/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7335 2024-05-20 15:01:42.000000 xspace-dl-0.2.24/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6059 2024-05-20 15:02:04.000000 xspace-dl-0.2.24/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7062 2024-05-20 15:01:55.000000 xspace-dl-0.2.24/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:13:47.288447 xspace-dl-0.2.24/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:40:45.919843 xspace-dl-0.2.25/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.25/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:40:45.919546 xspace-dl-0.2.25/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.25/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.25/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 15:40:45.919901 xspace-dl-0.2.25/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 15:39:02.000000 xspace-dl-0.2.25/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:40:45.918018 xspace-dl-0.2.25/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.2.25/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16595 2024-05-20 15:36:07.000000 xspace-dl-0.2.25/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      826 2024-05-20 15:38:43.000000 xspace-dl-0.2.25/xspace/chat_extractor.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.25/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     9145 2024-05-20 15:39:59.000000 xspace-dl-0.2.25/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6059 2024-05-20 15:02:04.000000 xspace-dl-0.2.25/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7062 2024-05-20 15:01:55.000000 xspace-dl-0.2.25/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:40:45.919194 xspace-dl-0.2.25/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:40:45.000000 xspace-dl-0.2.25/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      369 2024-05-20 15:40:45.000000 xspace-dl-0.2.25/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 15:40:45.000000 xspace-dl-0.2.25/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 15:40:45.000000 xspace-dl-0.2.25/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 15:40:45.000000 xspace-dl-0.2.25/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 15:40:45.000000 xspace-dl-0.2.25/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.2.24/LICENSE` & `xspace-dl-0.2.25/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.24/PKG-INFO` & `xspace-dl-0.2.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.24
+Version: 0.2.25
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
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.24 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.25 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```

### Comparing `xspace-dl-0.2.24/README.md` & `xspace-dl-0.2.25/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.24/pyproject.toml` & `xspace-dl-0.2.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.24/setup.py` & `xspace-dl-0.2.25/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',
-    version='0.2.24',
+    version='0.2.25',
     author='Your Name',
     author_email='your.email@example.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rosebabaganoush/xspace-dl',
     packages=find_packages(),
```

### Comparing `xspace-dl-0.2.24/xspace/api.py` & `xspace-dl-0.2.25/xspace/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,14 +329,16 @@
         """Retrieve X Space media playlist details by the specified media key.
 
         - media_key: The media key of the X Space.
 
         - return: The media playlist details of the specified media key.
         """
         return super().get(self.join_url("status", media_key))
+    
+    
 
 
 class DummyAPI:
     """Dummy API class used for uninitialized APIs."""
 
     def __init__(self, api_name: str = "API") -> None:
         self.api_name = api_name
```

### Comparing `xspace-dl-0.2.24/xspace/cookies.py` & `xspace-dl-0.2.25/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.24/xspace/main.py` & `xspace-dl-0.2.25/xspace/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from types import TracebackType
 from typing import Optional, Type
 
 from xspace.api import API
 from xspace.cookies import load_cookies
 from xspace.xspace import Xspace
 from xspace.xspace_dl import XspaceDL
+from xspace.chat_extractor import ChatExtractor  # New import
 
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_ERROR = 1
 EXIT_CODE_MISUSE = 2
 
 def exception_hook(
     _: Type[BaseException],
@@ -107,14 +108,58 @@
         except KeyboardInterrupt:
             logging.info("Download Interrupted by user")
         finally:
             if not args.keep_files:
                 xspace_dl.cleanup()
     return EXIT_CODE_SUCCESS
 
+def chat(args: argparse.Namespace) -> int:
+    """Extract chat messages from x space"""
+    if not args.input_url:
+        print("Space URL should be provided")
+        return EXIT_CODE_MISUSE
+
+    if args.log:
+        log_filename = datetime.datetime.now().strftime(
+            ".xspace-chat.%Y-%m-%d_%H-%M-%S_%f.log"
+        )
+        handlers: Optional[list[logging.Handler]] = [
+            logging.FileHandler(log_filename),
+            logging.StreamHandler(),
+        ]
+    else:
+        handlers = None
+
+    if not args.verbose:
+        sys.excepthook = exception_hook
+        logging.basicConfig(
+            level=logging.INFO,
+            format="%(levelname)s: %(message)s",
+            handlers=handlers,
+        )
+    else:
+        logging.basicConfig(
+            level=logging.DEBUG,
+            format="%(asctime)s [%(levelname)s] %(message)s",
+            handlers=handlers,
+        )
+
+    API.init_apis(load_cookies(args.input_cookie_file))
+    
+    xspace_instance = Xspace.from_space_url(args.input_url)
+    media_key = xspace_instance["media_key"]
+    chat_data = API.live_video_stream_api.get_chat_token(media_key)
+    chat_token = chat_data["chatToken"]
+    endpoint = chat_data["endpoint"]
+
+    chat_extractor = ChatExtractor(chat_token, endpoint)
+    chat_extractor.extract()
+    
+    return EXIT_CODE_SUCCESS
+
 def main() -> int:
     """Main function, creates the argument parser"""
     parser = argparse.ArgumentParser(
         description="Script designed to help download x spaces"
     )
 
     input_group = parser.add_argument_group("input")
@@ -210,14 +255,24 @@
     output_group.add_argument(
         "-e",
         "--embed-cover",
         action="store_true",
         help="embed user avatar as cover art",
     )
     parser.set_defaults(func=space)
+    
+    # Add the new chat command
+    chat_group = parser.add_argument_group("chat")
+    chat_group.add_argument(
+        "-i", "--input-url", type=str, metavar="SPACE_URL", help="space url to extract chat"
+    )
+    chat_group.add_argument("-v", "--verbose", action="store_true")
+    chat_group.add_argument("-l", "--log", action="store_true", help="create logfile")
+    chat_group.set_defaults(func=chat)
+
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         return EXIT_CODE_ERROR
     args = parser.parse_args()
     args.func(args)
     return EXIT_CODE_SUCCESS
```

### Comparing `xspace-dl-0.2.24/xspace/xspace.py` & `xspace-dl-0.2.25/xspace/xspace.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.24/xspace/xspace_dl.py` & `xspace-dl-0.2.25/xspace/xspace_dl.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.24/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.2.25/xspace_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.24
+Version: 0.2.25
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
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.24 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.25 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```


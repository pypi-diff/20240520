# Comparing `tmp/xspace-dl-0.3.1.tar.gz` & `tmp/xspace-dl-0.3.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.3.1.tar", last modified: Mon May 20 15:49:56 2024, max compression
+gzip compressed data, was "xspace-dl-0.3.12.tar", last modified: Mon May 20 16:14:00 2024, max compression
```

## Comparing `xspace-dl-0.3.1.tar` & `xspace-dl-0.3.12.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:49:56.788573 xspace-dl-0.3.1/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.3.1/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 15:49:56.788379 xspace-dl-0.3.1/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.3.1/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.3.1/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 15:49:56.788623 xspace-dl-0.3.1/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      855 2024-05-20 15:49:43.000000 xspace-dl-0.3.1/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:49:56.787024 xspace-dl-0.3.1/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.3.1/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16585 2024-05-20 15:49:19.000000 xspace-dl-0.3.1/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.3.1/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7335 2024-05-20 15:48:43.000000 xspace-dl-0.3.1/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6059 2024-05-20 15:49:03.000000 xspace-dl-0.3.1/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7062 2024-05-20 15:49:08.000000 xspace-dl-0.3.1/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:49:56.788130 xspace-dl-0.3.1/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 15:49:56.000000 xspace-dl-0.3.1/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 15:49:56.000000 xspace-dl-0.3.1/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 15:49:56.000000 xspace-dl-0.3.1/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 15:49:56.000000 xspace-dl-0.3.1/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 15:49:56.000000 xspace-dl-0.3.1/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 15:49:56.000000 xspace-dl-0.3.1/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 16:14:00.200373 xspace-dl-0.3.12/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.3.12/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      517 2024-05-20 16:14:00.200180 xspace-dl-0.3.12/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       42 2024-05-20 15:55:56.000000 xspace-dl-0.3.12/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.3.12/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 16:14:00.200435 xspace-dl-0.3.12/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 16:13:55.000000 xspace-dl-0.3.12/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 16:14:00.198876 xspace-dl-0.3.12/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.3.12/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16585 2024-05-20 15:49:19.000000 xspace-dl-0.3.12/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     3977 2024-05-20 16:13:12.000000 xspace-dl-0.3.12/xspace/chat_extractor.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.3.12/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7740 2024-05-20 16:12:37.000000 xspace-dl-0.3.12/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6059 2024-05-20 15:49:03.000000 xspace-dl-0.3.12/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7062 2024-05-20 15:49:08.000000 xspace-dl-0.3.12/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 16:14:00.199933 xspace-dl-0.3.12/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      517 2024-05-20 16:14:00.000000 xspace-dl-0.3.12/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      369 2024-05-20 16:14:00.000000 xspace-dl-0.3.12/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 16:14:00.000000 xspace-dl-0.3.12/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 16:14:00.000000 xspace-dl-0.3.12/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 16:14:00.000000 xspace-dl-0.3.12/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 16:14:00.000000 xspace-dl-0.3.12/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.3.1/LICENSE` & `xspace-dl-0.3.12/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.3.1/pyproject.toml` & `xspace-dl-0.3.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.3.1/setup.py` & `xspace-dl-0.3.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',
-    version='0.3.1',
+    version='0.3.12',
     author='Your Name',
     author_email='your.email@example.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rosebabaganoush/xspace-dl',
     packages=find_packages(),
```

### Comparing `xspace-dl-0.3.1/xspace/api.py` & `xspace-dl-0.3.12/xspace/api.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.3.1/xspace/cookies.py` & `xspace-dl-0.3.12/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.3.1/xspace/main.py` & `xspace-dl-0.3.12/xspace/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from types import TracebackType
 from typing import Optional, Type
 
 from xspace.api import API
 from xspace.cookies import load_cookies
 from xspace.xspace import Xspace
 from xspace.xspace_dl import XspaceDL
+from xspace.chat_extractor import ChatExtractor  # New import for ChatExtractor
 
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_ERROR = 1
 EXIT_CODE_MISUSE = 2
 
 def exception_hook(
     _: Type[BaseException],
@@ -105,14 +106,19 @@
             if args.embed_cover:
                 xspace_dl.embed_cover()
         except KeyboardInterrupt:
             logging.info("Download Interrupted by user")
         finally:
             if not args.keep_files:
                 xspace_dl.cleanup()
+
+    if args.captions_output:
+        chat_extractor = ChatExtractor(args.input_cookie_file, args.captions_output)
+        chat_extractor.get_caption(xspace_instance["id"])
+
     return EXIT_CODE_SUCCESS
 
 def main() -> int:
     """Main function, creates the argument parser"""
     parser = argparse.ArgumentParser(
         description="Script designed to help download x spaces"
     )
@@ -160,17 +166,15 @@
         "--from-master-url",
         type=str,
         metavar="URL",
         help=(
             "use the master url for the processes(useful for ended spaces)\n"
             "example: https://prod-fastly-ap-northeast-1.video.pscp.tv/Transcoding/v1/"
             "hls/YRSsw6_P5xUZHMualK5-ihvePR6o4QmoZVOBGicKvmkL_KB9IQYtxVqm3P_"
-            "vpZ2HnFkoRfar4_uJOjqC8OCo5A/non_transcode/ap-northeast-1/"
-            "periscope-replay-direct-prod-ap-northeast-1-public/"
-            "audio-space/master_playlist.m3u8"
+            "vpZ2HnFkoRfar4_uJOjqC8OCo5A/non_transcode/ap-northeast-1/periscope-replay-direct-prod-ap-northeast-1-public/audio-space/master_playlist.m3u8"
         ),
     )
     input_group.add_argument(
         "-M",
         "--input-metadata",
         type=str,
         metavar="PATH",
@@ -209,15 +213,24 @@
     )
     output_group.add_argument(
         "-e",
         "--embed-cover",
         action="store_true",
         help="embed user avatar as cover art",
     )
+    output_group.add_argument(
+        "-cc",
+        "--captions-output",
+        type=str,
+        metavar="CAPTIONS_OUTPUT",
+        help="output path for captions",
+    )
+
     parser.set_defaults(func=space)
+    
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         return EXIT_CODE_ERROR
     args = parser.parse_args()
     args.func(args)
     return EXIT_CODE_SUCCESS
```

### Comparing `xspace-dl-0.3.1/xspace/xspace.py` & `xspace-dl-0.3.12/xspace/xspace.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.3.1/xspace/xspace_dl.py` & `xspace-dl-0.3.12/xspace/xspace_dl.py`

 * *Files identical despite different names*


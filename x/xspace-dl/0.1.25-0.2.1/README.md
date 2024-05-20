# Comparing `tmp/xspace-dl-0.1.25.tar.gz` & `tmp/xspace-dl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.1.25.tar", last modified: Mon May 20 13:15:38 2024, max compression
+gzip compressed data, was "xspace-dl-0.2.1.tar", last modified: Mon May 20 14:14:29 2024, max compression
```

## Comparing `xspace-dl-0.1.25.tar` & `xspace-dl-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:15:38.958950 xspace-dl-0.1.25/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.25/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 13:15:38.958761 xspace-dl-0.1.25/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4104 2024-05-20 12:44:30.000000 xspace-dl-0.1.25/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1082 2024-05-20 12:44:30.000000 xspace-dl-0.1.25/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 13:15:38.959000 xspace-dl-0.1.25/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      980 2024-05-20 13:15:26.000000 xspace-dl-0.1.25/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:15:38.957403 xspace-dl-0.1.25/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:14:45.000000 xspace-dl-0.1.25/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16813 2024-05-20 12:44:42.000000 xspace-dl-0.1.25/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.25/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7352 2024-05-20 13:01:32.000000 xspace-dl-0.1.25/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6068 2024-05-20 12:48:38.000000 xspace-dl-0.1.25/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7057 2024-05-20 12:44:30.000000 xspace-dl-0.1.25/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 13:15:38.958526 xspace-dl-0.1.25/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4588 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 13:15:38.000000 xspace-dl-0.1.25/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:14:29.307877 xspace-dl-0.2.1/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 14:14:29.307676 xspace-dl-0.2.1/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 14:14:29.307924 xspace-dl-0.2.1/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      855 2024-05-20 14:14:13.000000 xspace-dl-0.2.1/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:14:29.306225 xspace-dl-0.2.1/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:11:45.000000 xspace-dl-0.2.1/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7378 2024-05-20 14:13:17.000000 xspace-dl-0.2.1/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6084 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7061 2024-05-20 14:08:08.000000 xspace-dl-0.2.1/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:14:29.307431 xspace-dl-0.2.1/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6692 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 14:14:29.000000 xspace-dl-0.2.1/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.1.25/LICENSE` & `xspace-dl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.25/pyproject.toml` & `xspace-dl-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-name = "xspace-dl"
+name = "twspace-dl"
 version = "2023.7.24.1"
 description = "The only tool to record Twitter spaces (yet)"
 authors = ["Ryu1845 <ryu@tpgjbo.xyz>"]
 readme = "README.md"
 license = "GPL-2.0-only"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -15,15 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
 mutagen = "^1.46.0"
 
 
 [tool.poetry.scripts]
-xspace_dl = "xspace_dl.__main__:main"
+twspace_dl = "twspace_dl.__main__:main"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 black = "^22.1.0"
 mypy = "^0.940"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
```

### Comparing `xspace-dl-0.1.25/setup.py` & `xspace-dl-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='xspace-dl',  # Updated package name
-    version='0.1.25',  # Increment the version number
-    author='RoseBabaGanoush',
-    author_email='hello@rosebabaganoush.com',
+    name='xspace-dl',
+    version='0.2.1',
+    author='Your Name',
+    author_email='your.email@example.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/RoseBabaganoush/xspace-dl',  # Update with your repository URL
+    url='https://github.com/rosebabaganoush/xspace-dl',
     packages=find_packages(),
     install_requires=[
         'requests',
-        'mutagen',  # Add mutagen to dependencies
+        'mutagen',
     ],
     entry_points={
         'console_scripts': [
-            'xspace-dl=xspace.main:main',  # Adjust as per your CLI entry point
+            'xspace-dl=xspace.main:main',  # Ensure this matches your main entry point
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Operating System :: OS Independent',
     ],
```

### Comparing `xspace-dl-0.1.25/xspace/api.py` & `xspace-dl-0.2.1/xspace/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             raise RuntimeError("API request failed with HTTP error") from e
 
 
 class APIClient:
     """Base API client."""
 
     """Base URL of the API."""
-    _API_URL = "https://x.com/i/api"
+    _API_URL = "https://twitter.com/i/api"
 
     def __init__(self, client: HTTPClient, path: str, cookies: dict[str, str]) -> None:
         """Initialize the API client.
 
         - client: The `HTTPClient` instance to send requests.
         - path: The path to add to the base URL of the API.
         - cookies: The cookies used for making all requests to the API.
@@ -249,17 +249,17 @@
             data = self.profile_spotlights_query(screen_name)
             return data["data"]["user_result_by_screen_name"]["result"]["rest_id"]
 
     def user_id_from_url(self, user_url: str) -> str:
         """Retrieve the numeric user ID (`rest_id`) of the user that the specified profile URL linked to.
 
         Supported URL formats:
-        - https://x.com/<screen_name>
-        - http://x.com/<screen_name>
-        - x.com/<screen_name>
+        - https://twitter.com/<screen_name>
+        - http://twitter.com/<screen_name>
+        - twitter.com/<screen_name>
         and with any number of trailing slashes (`/`).
 
         - user_url: The URL pointing to the profile of the Twitter user.
 
         - return: The numeric user ID (`rest_id`) of the specified user.
 
         - raise RuntimeError: If the specified URL is not a valid Twitter user profile URL.
```

### Comparing `xspace-dl-0.1.25/xspace/cookies.py` & `xspace-dl-0.2.1/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.25/xspace/main.py` & `xspace-dl-0.2.1/xspace/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,45 +5,40 @@
 import logging
 import sys
 from types import TracebackType
 from typing import Optional, Type
 
 from xspace.api import API
 from xspace.cookies import load_cookies
-from xspace.xspace import xspace
-from xspace.xspace_dl import xspaceDL
+from xspace.xspace import Xspace
+from xspace.xspace_dl import XspaceDL
 
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_ERROR = 1
 EXIT_CODE_MISUSE = 2
 
-
 def exception_hook(
     _: Type[BaseException],
     exc_value: BaseException,
     _t: TracebackType = None,
 ) -> None:
     """Make Exceptions more legible for the end users"""
-    # Exception type and value
     print(f"\033[31;1;4mError\033[0m: {exc_value}\nRetry with -v to see more details")
 
-
 def space(args: argparse.Namespace) -> int:
     """Manage the twitter space related function"""
     has_input = (
         args.user_url
         or args.input_url
         or args.input_metadata
         or args.from_dynamic_url
         or args.from_master_url
     )
     if not has_input:
-        print(
-            "Either user url, space url, dynamic url or master url should be provided"
-        )
+        print("Either user url, space url, dynamic url or master url should be provided")
         return EXIT_CODE_MISUSE
 
     if args.log:
         log_filename = datetime.datetime.now().strftime(
             ".xspace-dl.%Y-%m-%d_%H-%M-%S_%f.log"
         )
         handlers: Optional[list[logging.Handler]] = [
@@ -64,39 +59,42 @@
         logging.basicConfig(
             level=logging.DEBUG,
             format="%(asctime)s [%(levelname)s] %(message)s",
             handlers=handlers,
         )
 
     API.init_apis(load_cookies(args.input_cookie_file))
+
+    xspace_instance = None
     if args.user_url:
-        xspace = xspace.from_user_avatar(args.user_url)
+        xspace_instance = Xspace.from_user_avatar(args.user_url)
     elif args.input_metadata:
-        xspace = xspace.from_file(args.input_metadata)
+        xspace_instance = Xspace.from_file(args.input_metadata)
     elif args.input_url:
-        xspace = xspace.from_space_url(args.input_url)
+        xspace_instance = Xspace.from_space_url(args.input_url)
     else:
         logging.warning(
             (
                 "No metadata provided.\n"
                 "The resulting file won't be associated with the original space.\n"
                 "Please consider adding a space url or a metadata file"
             )
         )
-        xspace = xspace({})
-    xspace_dl = xspaceDL(xspace, args.output)
+        xspace_instance = Xspace({})
+
+    xspace_dl = XspaceDL(xspace_instance, args.output)
 
     if args.from_dynamic_url:
         xspace_dl.dyn_url = args.from_dynamic_url
     if args.from_master_url:
         xspace_dl.master_url = args.from_master_url
 
     if args.write_metadata:
         with open(f"{xspace_dl.filename}.json", "w", encoding="utf-8") as metadata_io:
-            json.dump(xspace.source, metadata_io, indent=4)
+            json.dump(xspace_instance.source, metadata_io, indent=4)
     if args.url:
         print(xspace_dl.master_url)
     if args.write_url:
         with open(args.write_url, "a", encoding="utf-8") as url_output:
             url_output.write(f"{xspace_dl.master_url}\n")
     if args.write_playlist:
         xspace_dl.write_playlist()
@@ -109,15 +107,14 @@
         except KeyboardInterrupt:
             logging.info("Download Interrupted by user")
         finally:
             if not args.keep_files:
                 xspace_dl.cleanup()
     return EXIT_CODE_SUCCESS
 
-
 def main() -> int:
     """Main function, creates the argument parser"""
     parser = argparse.ArgumentParser(
         description="Script designed to help download twitter spaces"
     )
 
     input_group = parser.add_argument_group("input")
@@ -220,10 +217,9 @@
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         return EXIT_CODE_ERROR
     args = parser.parse_args()
     args.func(args)
     return EXIT_CODE_SUCCESS
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `xspace-dl-0.1.25/xspace/xspace.py` & `xspace-dl-0.2.1/xspace/xspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 from collections import defaultdict
 from datetime import datetime
 
 from .api import API
 
 
-class xspace(dict):
+class Twspace(dict):
     """Downloader class for twitter spaces"""
 
     def __init__(self, metadata: dict) -> None:
         dict.__init__(
             self,
             {
                 "id": "",
@@ -38,15 +38,15 @@
                 self["creator_id"] = API.graphql_api.user_id(
                     creator_info["screen_name"]
                 )
 
             self.source = metadata
             self.root = root
             self["id"] = root["rest_id"]
-            self["url"] = "https://x.com/i/spaces/" + self["id"]
+            self["url"] = "https://twitter.com/i/spaces/" + self["id"]
             self["title"] = root["title"]
             try:
                 self["start_date"] = datetime.fromtimestamp(
                     int(root["started_at"]) / 1000
                 ).strftime("%Y-%m-%d")
             except ValueError as err:
                 sched_start = datetime.fromtimestamp(
@@ -135,39 +135,39 @@
         actual_format_str = os.path.basename(format_str)
         abs_dir = os.path.dirname(format_str) % self
         basename = self.sterilize_fn(actual_format_str % self)
         return os.path.join(abs_dir, basename)
 
     @classmethod
     def from_space_url(cls, url: str):
-        """Create a xspace instance from a space url"""
+        """Create a Twspace instance from a space url"""
         try:
             space_id = re.findall(r"(?<=spaces/)\w*", url)[0]
         except IndexError as err:
             raise ValueError(
                 (
                     "Input URL is not valid.\n"
-                    "The URL format should 'https://x.com/i/spaces/<space_id>'"
+                    "The URL format should 'https://twitter.com/i/spaces/<space_id>'"
                 )
             ) from err
         return cls(cls._metadata(space_id))
 
     @classmethod
     def from_user_avatar(cls, user_url: str):
-        """Create a xspace instance from a twitter user's ongoing space"""
+        """Create a Twspace instance from a twitter user's ongoing space"""
         user_id = API.graphql_api.user_id_from_url(user_url)
         avatar_content = API.fleets_api.avatar_content(user_id)
         try:
             broadcast_id = avatar_content["users"][user_id]["spaces"]["live_content"][
                 "audiospace"
             ]["broadcast_id"]
         except KeyError as err:
             raise ValueError(
                 "Broadcast ID is not available.\nUser is probably not live"
             ) from err
         return cls(cls._metadata(broadcast_id))
 
     @classmethod
     def from_file(cls, path: str):
-        """Create a xspace instance from a metadata file"""
+        """Create a Twspace instance from a metadata file"""
         with open(path, "r", encoding="utf-8") as metadata_io:
             return cls(json.load(metadata_io))
```

### Comparing `xspace-dl-0.1.25/xspace/xspace_dl.py` & `xspace-dl-0.2.1/xspace/xspace_dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import tempfile
 from functools import cached_property
 from urllib.parse import urlparse
 
 from mutagen.mp4 import MP4, MP4Cover
 
 from .api import API
-from .xspace import xspace
+from .twspace import Twspace
 
 DEFAULT_FNAME_FORMAT = "(%(creator_name)s)%(title)s-%(id)s"
 MP4_COVER_FORMAT_MAP = {"jpg": MP4Cover.FORMAT_JPEG, "png": MP4Cover.FORMAT_PNG}
 
 
-class xspaceDL:
+class TwspaceDL:
     """Downloader class for twitter spaces"""
 
-    def __init__(self, space: xspace, format_str: str) -> None:
+    def __init__(self, space: Twspace, format_str: str) -> None:
         self.space = space
         self.format_str = format_str or DEFAULT_FNAME_FORMAT
         self._tempdir = ""
 
     @cached_property
     def filename(self) -> str:
         """Returns the formatted filename"""
```


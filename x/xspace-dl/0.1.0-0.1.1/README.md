# Comparing `tmp/xspace-dl-0.1.0.tar.gz` & `tmp/xspace-dl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.1.0.tar", last modified: Mon May 20 12:42:03 2024, max compression
+gzip compressed data, was "xspace-dl-0.1.1.tar", last modified: Mon May 20 12:45:51 2024, max compression
```

## Comparing `xspace-dl-0.1.0.tar` & `xspace-dl-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:42:03.960561 xspace-dl-0.1.0/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.0/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4593 2024-05-20 12:42:03.960364 xspace-dl-0.1.0/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4110 2024-05-20 12:31:12.000000 xspace-dl-0.1.0/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 12:27:28.000000 xspace-dl-0.1.0/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 12:42:03.960611 xspace-dl-0.1.0/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      965 2024-05-20 12:41:54.000000 xspace-dl-0.1.0/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:42:03.959077 xspace-dl-0.1.0/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      177 2024-05-20 12:27:28.000000 xspace-dl-0.1.0/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7394 2024-05-20 12:27:28.000000 xspace-dl-0.1.0/xspace/__main__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 12:27:28.000000 xspace-dl-0.1.0/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.0/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6084 2024-05-20 12:27:28.000000 xspace-dl-0.1.0/xspace/twspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7061 2024-05-20 12:27:28.000000 xspace-dl-0.1.0/xspace/twspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:42:03.960139 xspace-dl-0.1.0/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     4593 2024-05-20 12:42:03.000000 xspace-dl-0.1.0/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      350 2024-05-20 12:42:03.000000 xspace-dl-0.1.0/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 12:42:03.000000 xspace-dl-0.1.0/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 12:42:03.000000 xspace-dl-0.1.0/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        9 2024-05-20 12:42:03.000000 xspace-dl-0.1.0/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 12:42:03.000000 xspace-dl-0.1.0/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:45:51.376381 xspace-dl-0.1.1/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 12:27:28.000000 xspace-dl-0.1.1/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4587 2024-05-20 12:45:51.376199 xspace-dl-0.1.1/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4104 2024-05-20 12:44:30.000000 xspace-dl-0.1.1/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1082 2024-05-20 12:44:30.000000 xspace-dl-0.1.1/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 12:45:51.376429 xspace-dl-0.1.1/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      962 2024-05-20 12:45:43.000000 xspace-dl-0.1.1/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:45:51.374961 xspace-dl-0.1.1/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 12:44:30.000000 xspace-dl-0.1.1/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7364 2024-05-20 12:44:30.000000 xspace-dl-0.1.1/xspace/__main__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16813 2024-05-20 12:44:42.000000 xspace-dl-0.1.1/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 12:27:28.000000 xspace-dl-0.1.1/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6068 2024-05-20 12:44:42.000000 xspace-dl-0.1.1/xspace/twspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7057 2024-05-20 12:44:30.000000 xspace-dl-0.1.1/xspace/twspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 12:45:51.375963 xspace-dl-0.1.1/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     4587 2024-05-20 12:45:51.000000 xspace-dl-0.1.1/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      350 2024-05-20 12:45:51.000000 xspace-dl-0.1.1/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 12:45:51.000000 xspace-dl-0.1.1/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 12:45:51.000000 xspace-dl-0.1.1/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        9 2024-05-20 12:45:51.000000 xspace-dl-0.1.1/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 12:45:51.000000 xspace-dl-0.1.1/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.1.0/LICENSE` & `xspace-dl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.0/PKG-INFO` & `xspace-dl-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/RoseBabaganoush/xspace-dl
 Author: RoseBabaGanoush
 Author-email: hello@rosebabaganoush.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 
 Use this if you're not sure.
 
 
 ### From PyPI
 
 ```bash
-pip install twspace-dl
+pip install xspace-dl
 ```
 
 
 
 ## Usage
 
 ```bash
@@ -43,25 +43,25 @@
 
 <details>
 <summary>With binaries</summary>
 
 ### Windows
 
 ```powershell
-.\twspace_dl.exe -i space_url -c COOKIE_FILE
+.\xspace_dl.exe -i space_url -c COOKIE_FILE
 ```
 
 </details>
 
 ## Features
 
 Here's the output of the help option
 
 ```txt
-usage: twspace_dl [-h] [-v] [-s] [-k] [-l] -c COOKIE_FILE
+usage: xspace_dl [-h] [-v] [-s] [-k] [-l] -c COOKIE_FILE
                   [-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-M PATH]
                   [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT] [-e]
 
 Script designed to help download twitter spaces
 
 options:
   -h, --help            show this help message and exit
@@ -128,23 +128,23 @@
 
 Example: `[%(creator_screen_name)s]-%(title)s|%(start_date)s`
 
 ## Known Errors
 
 `Changing ID3 metadata in HLS audio elementary stream is not implemented....`
 
-This is an error in ffmpeg that does not affect twspace_dl at all as far as I know.
+This is an error in ffmpeg that does not affect xspace_dl at all as far as I know.
 
 ## Docker
 
 ### Run once
 
 ```bash
-docker run --rm -v .:/output holoarchivists/twspace-dl -i space_url
+docker run --rm -v .:/output holoarchivists/xspace-dl -i space_url
 ```
 
 ### Run as monitoring service
 
-1. Download the `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named `twspace-dl`.
+1. Download the `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named `xspace-dl`.
 2. Edit `.env` and fill in the Twitter username you want to monitor.
 3. Put a cookies file into the folder and named it `cookies.txt`.
 4. `docker-compose up -d`
```

### Comparing `xspace-dl-0.1.0/README.md` & `xspace-dl-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Use this if you're not sure.
 
 
 ### From PyPI
 
 ```bash
-pip install twspace-dl
+pip install xspace-dl
 ```
 
 
 
 ## Usage
 
 ```bash
@@ -29,25 +29,25 @@
 
 <details>
 <summary>With binaries</summary>
 
 ### Windows
 
 ```powershell
-.\twspace_dl.exe -i space_url -c COOKIE_FILE
+.\xspace_dl.exe -i space_url -c COOKIE_FILE
 ```
 
 </details>
 
 ## Features
 
 Here's the output of the help option
 
 ```txt
-usage: twspace_dl [-h] [-v] [-s] [-k] [-l] -c COOKIE_FILE
+usage: xspace_dl [-h] [-v] [-s] [-k] [-l] -c COOKIE_FILE
                   [-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-M PATH]
                   [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT] [-e]
 
 Script designed to help download twitter spaces
 
 options:
   -h, --help            show this help message and exit
@@ -114,23 +114,23 @@
 
 Example: `[%(creator_screen_name)s]-%(title)s|%(start_date)s`
 
 ## Known Errors
 
 `Changing ID3 metadata in HLS audio elementary stream is not implemented....`
 
-This is an error in ffmpeg that does not affect twspace_dl at all as far as I know.
+This is an error in ffmpeg that does not affect xspace_dl at all as far as I know.
 
 ## Docker
 
 ### Run once
 
 ```bash
-docker run --rm -v .:/output holoarchivists/twspace-dl -i space_url
+docker run --rm -v .:/output holoarchivists/xspace-dl -i space_url
 ```
 
 ### Run as monitoring service
 
-1. Download the `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named `twspace-dl`.
+1. Download the `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named `xspace-dl`.
 2. Edit `.env` and fill in the Twitter username you want to monitor.
 3. Put a cookies file into the folder and named it `cookies.txt`.
 4. `docker-compose up -d`
```

### Comparing `xspace-dl-0.1.0/pyproject.toml` & `xspace-dl-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-name = "twspace-dl"
+name = "xspace-dl"
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
-twspace_dl = "twspace_dl.__main__:main"
+xspace_dl = "xspace_dl.__main__:main"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 black = "^22.1.0"
 mypy = "^0.940"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
```

### Comparing `xspace-dl-0.1.0/setup.py` & `xspace-dl-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',  # Updated package name
-    version='0.1.0',  # Increment the version as needed
+    version='0.1.1',  # Increment the version number
     author='RoseBabaGanoush',
     author_email='hello@rosebabaganoush.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/RoseBabaganoush/xspace-dl',  # Update with your repository URL
     packages=find_packages(),
```

### Comparing `xspace-dl-0.1.0/xspace/__main__.py` & `xspace-dl-0.1.1/xspace/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import datetime
 import json
 import logging
 import sys
 from types import TracebackType
 from typing import Optional, Type
 
-from twspace_dl.api import API
-from twspace_dl.cookies import load_cookies
-from twspace_dl.twspace import Twspace
-from twspace_dl.twspace_dl import TwspaceDL
+from xspace_dl.api import API
+from xspace_dl.cookies import load_cookies
+from xspace_dl.xspace import xspace
+from xspace_dl.xspace_dl import xspaceDL
 
 EXIT_CODE_SUCCESS = 0
 EXIT_CODE_ERROR = 1
 EXIT_CODE_MISUSE = 2
 
 
 def exception_hook(
@@ -40,15 +40,15 @@
         print(
             "Either user url, space url, dynamic url or master url should be provided"
         )
         return EXIT_CODE_MISUSE
 
     if args.log:
         log_filename = datetime.datetime.now().strftime(
-            ".twspace-dl.%Y-%m-%d_%H-%M-%S_%f.log"
+            ".xspace-dl.%Y-%m-%d_%H-%M-%S_%f.log"
         )
         handlers: Optional[list[logging.Handler]] = [
             logging.FileHandler(log_filename),
             logging.StreamHandler(),
         ]
     else:
         handlers = None
@@ -65,56 +65,56 @@
             level=logging.DEBUG,
             format="%(asctime)s [%(levelname)s] %(message)s",
             handlers=handlers,
         )
 
     API.init_apis(load_cookies(args.input_cookie_file))
     if args.user_url:
-        twspace = Twspace.from_user_avatar(args.user_url)
+        xspace = xspace.from_user_avatar(args.user_url)
     elif args.input_metadata:
-        twspace = Twspace.from_file(args.input_metadata)
+        xspace = xspace.from_file(args.input_metadata)
     elif args.input_url:
-        twspace = Twspace.from_space_url(args.input_url)
+        xspace = xspace.from_space_url(args.input_url)
     else:
         logging.warning(
             (
                 "No metadata provided.\n"
                 "The resulting file won't be associated with the original space.\n"
                 "Please consider adding a space url or a metadata file"
             )
         )
-        twspace = Twspace({})
-    twspace_dl = TwspaceDL(twspace, args.output)
+        xspace = xspace({})
+    xspace_dl = xspaceDL(xspace, args.output)
 
     if args.from_dynamic_url:
-        twspace_dl.dyn_url = args.from_dynamic_url
+        xspace_dl.dyn_url = args.from_dynamic_url
     if args.from_master_url:
-        twspace_dl.master_url = args.from_master_url
+        xspace_dl.master_url = args.from_master_url
 
     if args.write_metadata:
-        with open(f"{twspace_dl.filename}.json", "w", encoding="utf-8") as metadata_io:
-            json.dump(twspace.source, metadata_io, indent=4)
+        with open(f"{xspace_dl.filename}.json", "w", encoding="utf-8") as metadata_io:
+            json.dump(xspace.source, metadata_io, indent=4)
     if args.url:
-        print(twspace_dl.master_url)
+        print(xspace_dl.master_url)
     if args.write_url:
         with open(args.write_url, "a", encoding="utf-8") as url_output:
-            url_output.write(f"{twspace_dl.master_url}\n")
+            url_output.write(f"{xspace_dl.master_url}\n")
     if args.write_playlist:
-        twspace_dl.write_playlist()
+        xspace_dl.write_playlist()
 
     if not args.skip_download:
         try:
-            twspace_dl.download()
+            xspace_dl.download()
             if args.embed_cover:
-                twspace_dl.embed_cover()
+                xspace_dl.embed_cover()
         except KeyboardInterrupt:
             logging.info("Download Interrupted by user")
         finally:
             if not args.keep_files:
-                twspace_dl.cleanup()
+                xspace_dl.cleanup()
     return EXIT_CODE_SUCCESS
 
 
 def main() -> int:
     """Main function, creates the argument parser"""
     parser = argparse.ArgumentParser(
         description="Script designed to help download twitter spaces"
```

### Comparing `xspace-dl-0.1.0/xspace/api.py` & `xspace-dl-0.1.1/xspace/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             raise RuntimeError("API request failed with HTTP error") from e
 
 
 class APIClient:
     """Base API client."""
 
     """Base URL of the API."""
-    _API_URL = "https://twitter.com/i/api"
+    _API_URL = "https://x.com/i/api"
 
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
-        - https://twitter.com/<screen_name>
-        - http://twitter.com/<screen_name>
-        - twitter.com/<screen_name>
+        - https://x.com/<screen_name>
+        - http://x.com/<screen_name>
+        - x.com/<screen_name>
         and with any number of trailing slashes (`/`).
 
         - user_url: The URL pointing to the profile of the Twitter user.
 
         - return: The numeric user ID (`rest_id`) of the specified user.
 
         - raise RuntimeError: If the specified URL is not a valid Twitter user profile URL.
```

### Comparing `xspace-dl-0.1.0/xspace/cookies.py` & `xspace-dl-0.1.1/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.1.0/xspace/twspace.py` & `xspace-dl-0.1.1/xspace/twspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 from collections import defaultdict
 from datetime import datetime
 
 from .api import API
 
 
-class Twspace(dict):
+class xspace(dict):
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
-            self["url"] = "https://twitter.com/i/spaces/" + self["id"]
+            self["url"] = "https://x.com/i/spaces/" + self["id"]
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
-        """Create a Twspace instance from a space url"""
+        """Create a xspace instance from a space url"""
         try:
             space_id = re.findall(r"(?<=spaces/)\w*", url)[0]
         except IndexError as err:
             raise ValueError(
                 (
                     "Input URL is not valid.\n"
-                    "The URL format should 'https://twitter.com/i/spaces/<space_id>'"
+                    "The URL format should 'https://x.com/i/spaces/<space_id>'"
                 )
             ) from err
         return cls(cls._metadata(space_id))
 
     @classmethod
     def from_user_avatar(cls, user_url: str):
-        """Create a Twspace instance from a twitter user's ongoing space"""
+        """Create a xspace instance from a twitter user's ongoing space"""
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
-        """Create a Twspace instance from a metadata file"""
+        """Create a xspace instance from a metadata file"""
         with open(path, "r", encoding="utf-8") as metadata_io:
             return cls(json.load(metadata_io))
```

### Comparing `xspace-dl-0.1.0/xspace/twspace_dl.py` & `xspace-dl-0.1.1/xspace/twspace_dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import tempfile
 from functools import cached_property
 from urllib.parse import urlparse
 
 from mutagen.mp4 import MP4, MP4Cover
 
 from .api import API
-from .twspace import Twspace
+from .xspace import xspace
 
 DEFAULT_FNAME_FORMAT = "(%(creator_name)s)%(title)s-%(id)s"
 MP4_COVER_FORMAT_MAP = {"jpg": MP4Cover.FORMAT_JPEG, "png": MP4Cover.FORMAT_PNG}
 
 
-class TwspaceDL:
+class xspaceDL:
     """Downloader class for twitter spaces"""
 
-    def __init__(self, space: Twspace, format_str: str) -> None:
+    def __init__(self, space: xspace, format_str: str) -> None:
         self.space = space
         self.format_str = format_str or DEFAULT_FNAME_FORMAT
         self._tempdir = ""
 
     @cached_property
     def filename(self) -> str:
         """Returns the formatted filename"""
```

### Comparing `xspace-dl-0.1.0/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.1.1/xspace_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/RoseBabaganoush/xspace-dl
 Author: RoseBabaGanoush
 Author-email: hello@rosebabaganoush.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 
 Use this if you're not sure.
 
 
 ### From PyPI
 
 ```bash
-pip install twspace-dl
+pip install xspace-dl
 ```
 
 
 
 ## Usage
 
 ```bash
@@ -43,25 +43,25 @@
 
 <details>
 <summary>With binaries</summary>
 
 ### Windows
 
 ```powershell
-.\twspace_dl.exe -i space_url -c COOKIE_FILE
+.\xspace_dl.exe -i space_url -c COOKIE_FILE
 ```
 
 </details>
 
 ## Features
 
 Here's the output of the help option
 
 ```txt
-usage: twspace_dl [-h] [-v] [-s] [-k] [-l] -c COOKIE_FILE
+usage: xspace_dl [-h] [-v] [-s] [-k] [-l] -c COOKIE_FILE
                   [-i SPACE_URL | -U USER_URL] [-d DYN_URL] [-f URL] [-M PATH]
                   [-o FORMAT_STR] [-m] [-p] [-u] [--write-url URL_OUTPUT] [-e]
 
 Script designed to help download twitter spaces
 
 options:
   -h, --help            show this help message and exit
@@ -128,23 +128,23 @@
 
 Example: `[%(creator_screen_name)s]-%(title)s|%(start_date)s`
 
 ## Known Errors
 
 `Changing ID3 metadata in HLS audio elementary stream is not implemented....`
 
-This is an error in ffmpeg that does not affect twspace_dl at all as far as I know.
+This is an error in ffmpeg that does not affect xspace_dl at all as far as I know.
 
 ## Docker
 
 ### Run once
 
 ```bash
-docker run --rm -v .:/output holoarchivists/twspace-dl -i space_url
+docker run --rm -v .:/output holoarchivists/xspace-dl -i space_url
 ```
 
 ### Run as monitoring service
 
-1. Download the `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named `twspace-dl`.
+1. Download the `docker-compose.yml`, `.env`, `monitor.sh` files and put them in a folder named `xspace-dl`.
 2. Edit `.env` and fill in the Twitter username you want to monitor.
 3. Put a cookies file into the folder and named it `cookies.txt`.
 4. `docker-compose up -d`
```


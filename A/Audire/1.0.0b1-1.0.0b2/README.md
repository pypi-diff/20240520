# Comparing `tmp/audire-1.0.0b1.tar.gz` & `tmp/audire-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audire-1.0.0b1.tar", last modified: Mon May 20 12:23:28 2024, max compression
+gzip compressed data, was "audire-1.0.0b2.tar", last modified: Mon May 20 13:16:01 2024, max compression
```

## Comparing `audire-1.0.0b1.tar` & `audire-1.0.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:23:28.237972 audire-1.0.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:23:28.237972 audire-1.0.0b1/Audire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 12:23:28.000000 audire-1.0.0b1/Audire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 12:23:28.000000 audire-1.0.0b1/Audire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:23:28.000000 audire-1.0.0b1/Audire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 12:23:28.000000 audire-1.0.0b1/Audire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 12:23:28.000000 audire-1.0.0b1/Audire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 12:23:20.000000 audire-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 12:23:28.237972 audire-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-20 12:23:20.000000 audire-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:23:28.237972 audire-1.0.0b1/audire/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-20 12:23:20.000000 audire-1.0.0b1/audire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-20 12:23:20.000000 audire-1.0.0b1/audire/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-20 12:23:20.000000 audire-1.0.0b1/audire/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:23:28.237972 audire-1.0.0b1/audire/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 12:23:20.000000 audire-1.0.0b1/audire/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-20 12:23:20.000000 audire-1.0.0b1/audire/helpers/youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-20 12:23:20.000000 audire-1.0.0b1/audire/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:23:28.237972 audire-1.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-20 12:23:20.000000 audire-1.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:01.215763 audire-1.0.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:01.215763 audire-1.0.0b2/Audire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 13:15:53.000000 audire-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 13:16:01.215763 audire-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-20 13:15:53.000000 audire-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:01.215763 audire-1.0.0b2/audire/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:01.215763 audire-1.0.0b2/audire/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/helpers/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:16:01.215763 audire-1.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-20 13:15:53.000000 audire-1.0.0b2/setup.py
```

### Comparing `audire-1.0.0b1/Audire.egg-info/PKG-INFO` & `audire-1.0.0b2/Audire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Audire
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Package to search and get download links for songs from various platforms asynchronously.
 Home-page: https://github.com/LinuxGuy312/Audire
 Author: Eren
 Author-email: linuxguy312@segfault.net
 License: MIT
 Keywords: songs,song,music,youtube,ytm,Audire,audire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `audire-1.0.0b1/LICENSE` & `audire-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `audire-1.0.0b1/PKG-INFO` & `audire-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Audire
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Package to search and get download links for songs from various platforms asynchronously.
 Home-page: https://github.com/LinuxGuy312/Audire
 Author: Eren
 Author-email: linuxguy312@segfault.net
 License: MIT
 Keywords: songs,song,music,youtube,ytm,Audire,audire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `audire-1.0.0b1/README.md` & `audire-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `audire-1.0.0b1/audire/__init__.py` & `audire-1.0.0b2/audire/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from .main import *
 
-__version__ = "1.0.0b1"
+__version__ = "1.0.0b2"
```

### Comparing `audire-1.0.0b1/audire/dotdict.py` & `audire-1.0.0b2/audire/dotdict.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
+
 class DotDict(dict):
     """
     A class that parses dict into an object that can be accessed with dot notation.
 
     Args:
         dict (dict): The dictionary to convert to a dotdict.
```

### Comparing `audire-1.0.0b1/audire/errors.py` & `audire-1.0.0b2/audire/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
+
 class BaseError(Exception):
     """
     The base class for all errors raised within this package.
 
     Attributes:
         error_message (str, optional): The specific error message.
     """
```

### Comparing `audire-1.0.0b1/audire/helpers/__init__.py` & `audire-1.0.0b2/audire/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `audire-1.0.0b1/audire/helpers/youtube.py` & `audire-1.0.0b2/audire/helpers/youtube.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,18 +53,18 @@
             raise errors.NoResultsFoundError
         result = {"results": resp[:limit]}
         return dotdict.DotDict(result)
 
 
 async def get_download(url: str) -> dotdict.DotDict:
     """
-    Gets Download link for given Video ID.
+    Gets Download link for given URL.
 
     Parameters:
-        video_id (str): Video ID of the song to download
+        url (str): URL of the song to download
 
     Returns:
         DotDict (dotdict): DotDict which you can access with dot notation.
     """
     api = "https://co.wuk.sh/api/json"
     headers = {"accept": "application/json", "content-type": "application/json"}
     payload = {
```

### Comparing `audire-1.0.0b1/audire/main.py` & `audire-1.0.0b2/audire/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,15 @@
     def __init__(self):
         self.platforms = [
             "yt",  # YouTube
             "ytm",  # YouTube Music
         ]
 
     async def search(
-        self, query: str,
-        platform: str = "ytm",
-        limit: int = 10
+        self, query: str, platform: str = "ytm", limit: int = 10
     ) -> dotdict.DotDict:
         """
         Audire Search Function.
 
         Parameters:
             query (str): Query to search.
             platform (str, optional): Platform to search on. Defaults to "ytm" (YouTube Music)
@@ -54,16 +52,19 @@
         Returns:
             DotDict (dotdict): DotDict which you can access with dot notation.
         """
 
         if platform not in self.platforms:
             raise errors.PlatformNotSupportedError
 
-        if platform in ("yt", "ytm"):
-            return await youtube.search(query, platform, limit)
+        if platform == "yt":
+            return await youtube.search(query, False, limit)
+
+        if platform == "ytm":
+            return await youtube.search(query, True, limit)
 
     async def get_download(self, url: str, platform: str) -> dotdict.DotDict:
         """
         Returns An Object.
 
         Parameters:
             url (str): URL of song.
```

### Comparing `audire-1.0.0b1/setup.py` & `audire-1.0.0b2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import os
 import re
 import setuptools
 
 
 def _read(filename, version=False):
-    with open(os.path.join(os.path.dirname(__file__), filename), encoding="utf8") as file:
+    with open(
+        os.path.join(os.path.dirname(__file__), filename), encoding="utf8"
+    ) as file:
         text = file.read()
     if version:
         return re.search(r'__version__ = "(.*?)"', text).group(1)
     return text
 
 
 setuptools.setup(
```


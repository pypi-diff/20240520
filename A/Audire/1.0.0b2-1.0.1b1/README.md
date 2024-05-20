# Comparing `tmp/audire-1.0.0b2.tar.gz` & `tmp/audire-1.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audire-1.0.0b2.tar", last modified: Mon May 20 13:16:01 2024, max compression
+gzip compressed data, was "audire-1.0.1b1.tar", last modified: Mon May 20 13:37:09 2024, max compression
```

## Comparing `audire-1.0.0b2.tar` & `audire-1.0.1b1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:01.215763 audire-1.0.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:01.215763 audire-1.0.0b2/Audire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 13:16:01.000000 audire-1.0.0b2/Audire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 13:15:53.000000 audire-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 13:16:01.215763 audire-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-20 13:15:53.000000 audire-1.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:01.215763 audire-1.0.0b2/audire/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:16:01.215763 audire-1.0.0b2/audire/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/helpers/youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-20 13:15:53.000000 audire-1.0.0b2/audire/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:16:01.215763 audire-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-20 13:15:53.000000 audire-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:37:09.512989 audire-1.0.1b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:37:09.512989 audire-1.0.1b1/Audire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 13:37:09.000000 audire-1.0.1b1/Audire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 13:37:05.000000 audire-1.0.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 13:37:09.512989 audire-1.0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-20 13:37:05.000000 audire-1.0.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:37:09.512989 audire-1.0.1b1/audire/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:37:09.512989 audire-1.0.1b1/audire/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/helpers/soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/helpers/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-20 13:37:05.000000 audire-1.0.1b1/audire/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:37:09.512989 audire-1.0.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-20 13:37:05.000000 audire-1.0.1b1/setup.py
```

### Comparing `audire-1.0.0b2/Audire.egg-info/PKG-INFO` & `audire-1.0.1b1/Audire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Audire
-Version: 1.0.0b2
+Version: 1.0.1b1
 Summary: A Package to search and get download links for songs from various platforms asynchronously.
 Home-page: https://github.com/LinuxGuy312/Audire
 Author: Eren
 Author-email: linuxguy312@segfault.net
 License: MIT
 Keywords: songs,song,music,youtube,ytm,Audire,audire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `audire-1.0.0b2/LICENSE` & `audire-1.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `audire-1.0.0b2/PKG-INFO` & `audire-1.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Audire
-Version: 1.0.0b2
+Version: 1.0.1b1
 Summary: A Package to search and get download links for songs from various platforms asynchronously.
 Home-page: https://github.com/LinuxGuy312/Audire
 Author: Eren
 Author-email: linuxguy312@segfault.net
 License: MIT
 Keywords: songs,song,music,youtube,ytm,Audire,audire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `audire-1.0.0b2/README.md` & `audire-1.0.1b1/README.md`

 * *Files identical despite different names*

### Comparing `audire-1.0.0b2/audire/__init__.py` & `audire-1.0.1b1/audire/helpers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,11 +16,7 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-
-from .main import *
-
-__version__ = "1.0.0b2"
```

### Comparing `audire-1.0.0b2/audire/dotdict.py` & `audire-1.0.1b1/audire/dotdict.py`

 * *Files identical despite different names*

### Comparing `audire-1.0.0b2/audire/errors.py` & `audire-1.0.1b1/audire/errors.py`

 * *Files identical despite different names*

### Comparing `audire-1.0.0b2/audire/helpers/__init__.py` & `audire-1.0.1b1/audire/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,7 +16,11 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
+from .main import *
+
+__version__ = "1.0.1b1"
```

### Comparing `audire-1.0.0b2/audire/helpers/youtube.py` & `audire-1.0.1b1/audire/helpers/youtube.py`

 * *Files identical despite different names*

### Comparing `audire-1.0.0b2/audire/main.py` & `audire-1.0.1b1/audire/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,33 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from audire import dotdict, errors
-from audire.helpers import youtube
+from audire.helpers import (
+    youtube,
+    soundcloud,
+)
 
 
 class Audire:
     """
     Audire class search and get download links for music across various platforms.
 
     Attributes:
         platforms (list): List of supported Platforms.
     """
 
     def __init__(self):
         self.platforms = [
             "yt",  # YouTube
             "ytm",  # YouTube Music
+            "soundcloud",
         ]
 
     async def search(
         self, query: str, platform: str = "ytm", limit: int = 10
     ) -> dotdict.DotDict:
         """
         Audire Search Function.
@@ -58,14 +62,17 @@
 
         if platform == "yt":
             return await youtube.search(query, False, limit)
 
         if platform == "ytm":
             return await youtube.search(query, True, limit)
 
+        if platform == "soundcloud":
+            return None
+
     async def get_download(self, url: str, platform: str) -> dotdict.DotDict:
         """
         Returns An Object.
 
         Parameters:
             url (str): URL of song.
             platform (str): Platform of download.
@@ -75,7 +82,10 @@
         """
 
         if platform not in self.platforms:
             raise errors.PlatformNotSupportedError
 
         if platform in ("yt", "ytm"):
             return await youtube.get_download(url)
+
+        if platform == "soundcloud":
+            return await soundcloud.get_download(url)
```

### Comparing `audire-1.0.0b2/setup.py` & `audire-1.0.1b1/setup.py`

 * *Files identical despite different names*


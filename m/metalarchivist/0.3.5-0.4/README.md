# Comparing `tmp/metalarchivist-0.3.5.tar.gz` & `tmp/metalarchivist-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.3.5.tar", last modified: Thu May 16 15:30:41 2024, max compression
+gzip compressed data, was "metalarchivist-0.4.tar", last modified: Mon May 20 15:15:32 2024, max compression
```

## Comparing `metalarchivist-0.3.5.tar` & `metalarchivist-0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.643391 metalarchivist-0.3.5/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-16 15:30:41.643391 metalarchivist-0.3.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 15:30:41.643391 metalarchivist-0.3.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.634391 metalarchivist-0.3.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.635391 metalarchivist-0.3.5/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.638391 metalarchivist-0.3.5/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.638391 metalarchivist-0.3.5/src/metalarchivist/export/data/
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/export/data/user-agents.json
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     9505 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/export/label.py
--rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.640391 metalarchivist-0.3.5/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7089 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/album.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.640391 metalarchivist-0.3.5/src/metalarchivist/interface/api/
--rw-rw-rw-   0 root         (0) root         (0)     3113 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4836 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/api/page.py
--rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     8109 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/label.py
--rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3645 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.642391 metalarchivist-0.3.5/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-16 15:30:41.000000 metalarchivist-0.3.5/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2024-05-16 15:30:41.000000 metalarchivist-0.3.5/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 15:30:41.000000 metalarchivist-0.3.5/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-16 15:30:41.000000 metalarchivist-0.3.5/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-16 15:30:41.000000 metalarchivist-0.3.5/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 15:30:41.642391 metalarchivist-0.3.5/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10013 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     5407 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/test/test_labels.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-16 15:30:27.000000 metalarchivist-0.3.5/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.888841 metalarchivist-0.4/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-20 15:15:18.000000 metalarchivist-0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      700 2024-05-20 15:15:32.888841 metalarchivist-0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-20 15:15:18.000000 metalarchivist-0.4/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      675 2024-05-20 15:15:18.000000 metalarchivist-0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 15:15:32.889841 metalarchivist-0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.881841 metalarchivist-0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.882841 metalarchivist-0.4/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.884841 metalarchivist-0.4/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.884841 metalarchivist-0.4/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)    10569 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7103 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.886841 metalarchivist-0.4/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9056 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.886841 metalarchivist-0.4/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4836 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     5991 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.888841 metalarchivist-0.4/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      700 2024-05-20 15:15:32.000000 metalarchivist-0.4/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-05-20 15:15:32.000000 metalarchivist-0.4/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 15:15:32.000000 metalarchivist-0.4/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-20 15:15:32.000000 metalarchivist-0.4/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-20 15:15:32.000000 metalarchivist-0.4/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 15:15:32.887841 metalarchivist-0.4/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10205 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     5407 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-20 15:15:18.000000 metalarchivist-0.4/src/test/test_themes.py
```

### Comparing `metalarchivist-0.3.5/LICENSE` & `metalarchivist-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/PKG-INFO` & `metalarchivist-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.3.5
+Version: 0.4
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.3.5/pyproject.toml` & `metalarchivist-0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.3.5"
+version = "0.4"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.3.5/src/metalarchivist/export/album.py` & `metalarchivist-0.4/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/export/band.py` & `metalarchivist-0.4/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/export/data/user-agents.json` & `metalarchivist-0.4/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/export/genre.py` & `metalarchivist-0.4/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/export/label.py` & `metalarchivist-0.4/src/metalarchivist/export/label.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import time
 import string
 import concurrent.futures
 
 import urllib3
 
-from .util import MetalArchives, normalize_keyword_casing, perform_request
+from .util import MetalArchives, normalize_keyword_casing, perform_request, MetalArchivesError
 from ..interface import (LabelProfile, LabelExternalLinks,
                          LabelPage, LabelPages, LabelContainer,
                          LabelRosterPages, LabelRosterPage, 
                          LabelReleasePages, LabelReleasePage)
 
 
-class LabelError(Exception):
-    def __init__(self, status_code, url):
-        self.status_code = status_code
-        self.url = url
-
-    def __repr__(self):
-        return repr(self) + f'<{self.status_code}: {self.url}>'
+class LabelError(MetalArchivesError):
+    ...
 
 
 class Label:
 
     @classmethod
     def get_full_profile(cls, label_url: str, user_agent: str | None = None, wait=3.):
         profile = cls.get_profile(label_url, user_agent=user_agent)
@@ -157,24 +152,24 @@
             
             processed_urls = set()
 
             # don't throw them all in at once
             for segment_start in range(0, profile_urls_len + segment_size, segment_size):
                 segment_end = min(segment_start + segment_size, profile_urls_len)
 
-                band_futures = list()
+                label_futures = list()
                 for url in profile_urls[segment_start:segment_end]:
                     if url not in processed_urls:
                         future = executor.submit(cls.get_profile, url)
-                        band_futures.append(future)
+                        label_futures.append(future)
                         processed_urls.add(url)
                         time.sleep(wait)
 
                 # examine the remains
-                for future in concurrent.futures.as_completed(band_futures):
+                for future in concurrent.futures.as_completed(label_futures):
                     profile = future.result()
                     profiles.append(profile)
 
         return profiles
     
     @classmethod
     def get_external_links(cls, metallum_ids: list[int], segment_size=8, wait=3.) -> list[LabelExternalLinks]:
@@ -189,24 +184,24 @@
             
             processed_urls = set()
 
             # don't throw them all in at once
             for segment_start in range(0, metallum_ids_count + segment_size, segment_size):
                 segment_end = min(segment_start + segment_size, metallum_ids_count)
 
-                band_futures = list()
+                links_futures = list()
                 for url in metallum_ids[segment_start:segment_end]:
                     if url not in processed_urls:
                         future = executor.submit(cls.get_profile_links, url)
-                        band_futures.append(future)
+                        links_futures.append(future)
                         processed_urls.add(url)
                         time.sleep(wait)
 
                 # examine the remains
-                for future in concurrent.futures.as_completed(band_futures):
+                for future in concurrent.futures.as_completed(links_futures):
                     profile = future.result()
                     links.append(profile)
         
         return links
 
     @classmethod
     def get_labels_by_letter(cls, letter: str, echo=0, page_size=500, wait=3.,
@@ -246,7 +241,40 @@
             label_futures = [executor.submit(cls.get_labels_by_letter, letter, echo=echo, page_size=page_size, wait=wait)
                              for letter in letters]
             
             for future in concurrent.futures.as_completed(label_futures):
                 data.append(future.result())
 
         return data.combine()
+
+    @classmethod
+    def get_full_profiles(cls, profile_urls: list[str], segment_size=8, wait=3.) -> list[LabelContainer]:
+
+        profile_urls_len = len(profile_urls)
+        profiles = list()
+        
+        if profile_urls_len == 0:
+            return profiles
+
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            
+            processed_urls = set()
+
+            # don't throw them all in at once
+            for segment_start in range(0, profile_urls_len + segment_size, segment_size):
+                segment_end = min(segment_start + segment_size, profile_urls_len)
+
+                label_futures = list()
+                for url in profile_urls[segment_start:segment_end]:
+                    if url not in processed_urls:
+                        future = executor.submit(cls.get_full_profile, url)
+                        label_futures.append(future)
+                        processed_urls.add(url)
+                        time.sleep(wait)
+
+                # examine the remains
+                for future in concurrent.futures.as_completed(label_futures):
+                    profile = future.result()
+                    profiles.append(profile)
+
+        return profiles
+
```

### Comparing `metalarchivist-0.3.5/src/metalarchivist/export/util.py` & `metalarchivist-0.4/src/metalarchivist/export/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 
 
 class DecodeErrorWarning(UserWarning):
     ...
 
 
 class MetalArchivesError(Exception):
-    def __init__(self, status_code):
+    def __init__(self, status_code, url):
         self.status_code = status_code
+        self.url = url
 
     def __repr__(self):
         return repr(self) + f'<{self.status_code}>'
     
 
 class MetalArchivesInternalError(Exception):
     def __init__(self, **kwargs):
```

### Comparing `metalarchivist-0.3.5/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.4/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/interface/album.py` & `metalarchivist-0.4/src/metalarchivist/interface/album.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
  
 import re
 from datetime import datetime
 from dataclasses import dataclass, field, InitVar, asdict
 
-import lxml.etree
 import lxml.html
+import lxml.etree
+from lxml.etree import ElementBase
 
 from .band import BandLink
 from .genre import Subgenres
+from .api.base import create_key
 
 
 class ParseError(Exception):
     ...
 
 
 def _parse_release_date(release_date) -> str:
@@ -39,30 +41,44 @@
 
     if release_date_parsed is None:
         raise ParseError('unable to parse release date')
 
     return release_date_parsed
 
 
+class AlbumXPath:
+    LABEL_LINK = '//div[@id="album_info"]/dl/dt[text()="Label:"]/following-sibling::dd[1]/a'
+    NAME = './/h1[@class="album_name"]/a/text()'
+    BAND_LINK = './/h2[@class="band_name"]/a'
+    DESCRIPTION_TITLES = '//div[@id="album_info"]/dl/dt/text()'
+    DESCRIPTION_DETAILS = '//div[@id="album_info"]/dl/dd/text()'
+    TRACKLIST = '//div[@id="album_tabs_tracklist"]//tr[@class="even" or @class="odd"]'
+
 @dataclass
 class AlbumLink:
     """ The data within an HTML anchor tag pointing to an album page """
+    html: InitVar[str]
+    
     name: str = field(init=False)
     link: str = field(init=False)
+    metallum_id: int = field(init=False)
+    album_key: str = field(init=False)
     authenticity: str | None = field(init=False, default=None)
 
-    def __init__(self, html: str):
+    def __post_init__(self, html: str):
         fragments = lxml.html.fragments_fromstring(html)
         html_anchor, *remaining_tags = fragments
         
         if remaining_tags and remaining_tags[0].tag == 'span':
             self.authenticity = remaining_tags[0].text.strip()
 
-        self.name = html_anchor.text
-        self.link = html_anchor.attrib['href']
+        self.link = link = html_anchor.attrib['href']
+        self.name = name = html_anchor.text
+        self.metallum_id = metallum_id = int(link.split('/').pop())
+        self.album_key = create_key(metallum_id, name)
 
 
 @dataclass
 class AlbumRelease:    
     band: BandLink
     album: AlbumLink
 
@@ -106,28 +122,31 @@
 
 
 @dataclass
 class AlbumTrack:
     """ A unique track on an album """
     tablerow: InitVar[lxml.etree.ElementBase]
 
-    metallum_id: int = field(init=False)
+    metallum_id: str = field(init=False)
     number: str = field(init=False)
     title: str = field(init=False)
-    length: AlbumTrackLength = field(init=False)
+    length: AlbumTrackLength | None = field(init=False)
     lyrics: str = field(init=False)
+    track_key: str = field(init=False)
 
     def __post_init__(self, tablerow: lxml.etree.ElementBase):
         number, title, length, lyrics = tablerow.xpath('./td')
-        metallum_id = number.xpath('./a').pop().attrib['name']
 
-        self.metallum_id = int(metallum_id)
-        self.title = title.text
+        self.metallum_id = metallum_id = number.xpath('./a').pop().attrib['name']
+        self.title = title = title.text
+
+        self.track_key = create_key(metallum_id, title)
+
         self.number = number.text
-        self.length = AlbumTrackLength(length.text)
+        self.length = AlbumTrackLength(length.text) if length.text else None
         self.lyrics = lyrics.text
 
 
 @dataclass
 class AlbumDescription:
     """ Additional information concerning an album """
     release_type: str | None
@@ -136,49 +155,76 @@
     label: str | None
     media_format: str | None
     version_desc: str | None = field(default=None)
     limitation: str | None = field(default=None)
     reviews: str | None = field(default=None)
 
 
+
+
+@dataclass
+class AlbumLabelLink:
+    """ Rough copy of .label.LabelLink, defined locally to prevent 
+        circular imports between .album and .label 
+    """
+
+    html: InitVar[str]
+
+    name: str = field(init=False)
+    link: str = field(init=False)
+    metallum_id: int = field(init=False)
+    label_key: str = field(init=False)
+
+    def __post_init__(self, html: str):
+        html_anchor = lxml.html.fragment_fromstring(html)
+        self.name = html_anchor.text
+        self.link = link = html_anchor.attrib['href'].split('#').pop(0)
+        self.metallum_id = int(link.split('/').pop())
+        self.label_key = create_key(self.metallum_id, self.name)
+
+    @classmethod
+    def from_element(cls, element: ElementBase):
+        kwargs = dict(method='html', with_tail=False)
+        return cls(lxml.etree.tostring(element, **kwargs))
+
+
 @dataclass
 class AlbumProfile:
     """ An album profile page """
     url: str
     html: InitVar[bytes]
 
     name: str = field(init=False)
     metallum_id: int = field(init=False)
+    album_key: str = field(init=False)
     
     band: BandLink = field(init=False)
+    label: AlbumLabelLink | None = field(init=False)
     tracklist: list[AlbumTrack] = field(init=False)
     description: AlbumDescription = field(init=False)
 
     def __post_init__(self, profile_html):
-        self.metallum_id = int(self.url.split('/')[-1])
-
         profile_document = lxml.html.document_fromstring(profile_html)
+        self.name = name = profile_document.xpath(AlbumXPath.NAME).pop()
+        
+        self.metallum_id = metallum_id = int(self.url.split('/')[-1])
+        
+        self.album_key = create_key(metallum_id, name)
 
-        self.name = profile_document.xpath('.//h1[@class="album_name"]/a/text()').pop()
-
-        band_link = profile_document.xpath('.//h2[@class="band_name"]/a').pop()
+        band_link = profile_document.xpath(AlbumXPath.BAND_LINK).pop()
         band_link_str = lxml.etree.tostring(band_link).decode('utf-8').split('\n')[0]
         self.band = BandLink(band_link_str)
 
-        album_desc_titles_xpath = '//div[@id="album_info"]/dl/dt/text()'
-        album_desc_titles = profile_document.xpath(album_desc_titles_xpath)
-
-        album_desc_detail_xpath = '//div[@id="album_info"]/dl/dd/text()'
-        album_desc_detail = profile_document.xpath(album_desc_detail_xpath)
+        album_desc_titles = profile_document.xpath(AlbumXPath.DESCRIPTION_TITLES)
+        album_desc_detail = profile_document.xpath(AlbumXPath.DESCRIPTION_DETAILS)
 
         self.description = self._parse_description(album_desc_titles, album_desc_detail)
+        self.label = self._parse_label(profile_document)
         
-        album_tracklist_xpath = ('//div[@id="album_tabs_tracklist"]'
-                                 '//tr[@class="even" or @class="odd"]')
-        album_tracklist = profile_document.xpath(album_tracklist_xpath)
+        album_tracklist = profile_document.xpath(AlbumXPath.TRACKLIST)
         self.tracklist = list(map(AlbumTrack, album_tracklist))
 
     @classmethod
     def _parse_description(cls, description_titles, description_details) -> AlbumDescription:
         description = {str(dt).lower(): str(dd).strip() 
                        for dt, dd in zip(description_titles, description_details)}
         
@@ -193,14 +239,24 @@
         # scrub invalid key names
         description = {cls._scrub_key_names(dt): dd
                        for dt, dd in description.items()}
 
         return AlbumDescription(**description)
     
     @staticmethod
+    def _parse_label(profile_document: lxml.etree.ElementBase) -> AlbumLabelLink | None:
+        
+        try:
+            label_anchor = profile_document.xpath(AlbumXPath.LABEL_LINK).pop()
+        except IndexError:
+            return None
+        else:
+            return AlbumLabelLink.from_element(label_anchor)
+
+    @staticmethod
     def _scrub_key_names(key: str) -> str:
         if key == 'type':
             return 'release_type'
 
         if key == 'format':
             return 'media_format'
```

### Comparing `metalarchivist-0.3.5/src/metalarchivist/interface/api/base.py` & `metalarchivist-0.4/src/metalarchivist/interface/api/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,22 @@
 
 from Crypto.Hash import BLAKE2s
 
 
 UNKNOWN = 'Unknown'
 
 
-def create_key(metallum_id: int, name: str) -> str:
-    metallum_id_bytes = struct.pack('>Q', metallum_id)
+def create_key(metallum_id: int | str, name: str) -> str:
+    if isinstance(metallum_id, int):
+        metallum_id_bytes = struct.pack('>Q', metallum_id)
+    elif isinstance(metallum_id, str):
+        metallum_id_bytes = metallum_id.encode('utf-8')
+    else:
+        raise TypeError('metallum_id must be a string or integer')
+
     hash_obj = BLAKE2s.new(data=name.encode('utf-8'), digest_bytes=12, key=metallum_id_bytes)
     return hash_obj.hexdigest()
 
 @dataclass
 class PageDataType(ABC):
     ...
```

### Comparing `metalarchivist-0.3.5/src/metalarchivist/interface/api/page.py` & `metalarchivist-0.4/src/metalarchivist/interface/api/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/interface/band.py` & `metalarchivist-0.4/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/interface/genre.py` & `metalarchivist-0.4/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/interface/label.py` & `metalarchivist-0.4/src/metalarchivist/interface/label.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,9 +241,10 @@
 
     def to_dict(self):
         links = asdict(self.links)
         profile = asdict(self.profile)
         releases = list(map(asdict, self.releases))
         roster = self.roster.to_dict()
 
-        return dict(profile=profile, releases=releases,
+        return dict(label_key=self.profile.label_key,
+                    profile=profile, releases=releases,
                     links=links, roster=roster)
```

### Comparing `metalarchivist-0.3.5/src/metalarchivist/interface/theme.py` & `metalarchivist-0.4/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/metalarchivist/report.py` & `metalarchivist-0.4/src/metalarchivist/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 import string
+from typing import Callable
 from datetime import datetime
 from dataclasses import asdict
 
 from .export import Band, Album, Label
 
-Series = list[str | int | float]
-Record = dict[str, str | float | int | Series]
+Datum = str | int | float | None
+Series = list[Datum]
+Record = dict[str, Datum]
 Dataset = list[Record]
 
 
-def series(from_list, column) -> Series:
-    return [[v for k, v in d.items() if k == column].pop() for d in from_list]
+def series(from_list: list[dict], column: str) -> Series:
+    return [[v for k, v in d.items() if k == column][0] for d in from_list]
 
 
-def select(from_list, column) -> Dataset:
+def select(from_list: list[dict], column: str) -> Dataset:
     return list(map(lambda n: {column: n[column]}, from_list))
 
 
-def expand(from_list, column) -> Dataset:
-    return list(map(lambda n: dict(**n[column]), from_list))
+def expand(from_list: list, column: str) -> Dataset:
+    column_sample: Record = next(filter(lambda n: n[column], from_list))[column]
+    null_dict: Record = {str(k): None for k in column_sample.keys()}
+    return list(map(lambda n: dict(**n[column]) if n[column] else null_dict, from_list))
 
 
-def drop(from_list, *columns) -> Dataset:
+def where(from_list: list, column: str, key: Callable[[Datum], bool]) -> Dataset:
+    return [n for n in from_list if key(n[column])]
+
+
+def drop(from_list: list[dict], *columns: str) -> Dataset:
     return [{k: v for k, v in d.items() if k not in columns} for d in from_list]
 
 
-def rename(from_list, column_map: dict) -> Dataset:
+def rename(from_list: list, column_map: dict) -> Dataset:
     return [{column_map.get(k, k): v for k, v in d.items()} for d in from_list]
 
 
 def join(first_list: Dataset, second_list: Dataset, on_column: str) -> Dataset:
     return [dict(**left, **{k: v for k, v in right.items() if k not in left}) 
             for left in first_list for right in second_list 
             if left[on_column] == right[on_column]]
@@ -39,66 +47,114 @@
     band_profile = Band.get_profiles(profile_urls, wait=wait)
     band_profile = list(map(lambda n: n.to_dict(), band_profile))
     
     band_desc = expand(select(band_profile, 'description'), 'description')
     band_desc = drop(band_desc, 'genre', 'themes', 'lyrical_themes')
 
     band_ids = series(band_profile, 'metallum_id')
-    band_ids = [int(band_id) for band_id in band_ids]
+    band_ids = [int(band_id) for band_id in band_ids if band_id is not None]
     band_links = Band.get_external_links(band_ids, wait=wait)
     band_links = list(map(asdict, band_links))
 
     genres = expand(select(band_profile, 'genres'), 'genres')
     themes = expand(select(band_profile, 'themes'), 'themes')
 
     band_profile = drop(band_profile, 'genres', 'themes',  'description')
     band_profile = join(band_profile, band_links, 'metallum_id')
 
     band_zip = zip(band_profile, band_desc, genres, themes)
 
     return [dict(**bp, **bd, **g, **t) for bp, bd, g, t in band_zip]
 
 
+def get_album_profiles(profile_urls: list[str]) -> Dataset:
+    album_profile = Album.get_profiles(profile_urls)
+    album_profile = list(map(lambda n: n.to_dict(), album_profile))
+    return album_profile
+
+
 def get_albums(range_start: datetime | None = None, range_stop: datetime | None = None, 
                wait=3., retries=3, timeout=3.) -> Dataset:
     if range_start:
         release_page = Album.get_range(range_start, range_stop, wait=wait, retries=retries, 
                                        timeout_cxn=timeout, timeout_read=timeout * 3)
     else:
         release_page = Album.get_upcoming(wait=wait, retries=retries, timeout_cxn=timeout, 
                                           timeout_read=timeout * 3)
 
     release = list(map(asdict, release_page.data))
 
+    band_key = select(expand(select(release, 'band'), 'band'), 'band_key')
+    
     # hoist out the link attributes from each band
     profile_urls = select(expand(select(release, 'band'), 'band'), 'link')
     profile_urls = series(profile_urls, 'link')
     profile_urls = [str(p) for p in profile_urls]
 
     band = get_bands(profile_urls, wait=wait)
 
     album = expand(select(release, 'album'), 'album')
     album = rename(album, dict(name='album', link='album_url'))
 
+    album_url = series(album, 'album_url')
+    album_url = [str(u) for u in album_url]
+    album_profiles = get_album_profiles(album_url)
+    album = join(album, album_profiles, 'album_key')
+    album = drop(album, 'band')
+
+    label_link = select(album, 'label')
+    label_link = expand(label_link, 'label')
+    label_key = select(label_link, 'label_key')
+
+    label_url = where(label_link, 'link', lambda n: n is not None)
+    label_url = series(label_url, 'link')
+    label_url = [str(u) for u in label_url]
+    label = get_label_profiles(label_url)
+    label = rename(label, dict(profile='label_profile',
+                               roster='label_roster',
+                               releases='label_releases'))
+    
     band = rename(band, dict(url='band_url', name='band'))
-    release = drop(release, 'genres', 'band', 'album')
-    profile_urls = [dict(band_url=u) for u in profile_urls]
-    album_zip = zip(album, profile_urls, release)
-
-    album = [dict(**a, **u, **r) for a, u, r in album_zip]
+    release = drop(release, 'genres', 'band', 'album', 'release_type')
+    
+    album = drop(album, 'label')
+    album = zip(album, band_key, label_key, release)
+    album = [dict(**a, **b, **lb, **r) for a, b, lb, r in album]
+    album = join(album, band, 'band_key')
+    album = join(album, label, 'label_key')
 
-    return join(album, band, 'band_url')
+    return album
 
 
 def get_labels() -> Dataset:
     label = Label.get_labels_by_letters(*string.ascii_lowercase, page_size=1000)
     label = map(lambda n: n.label.url, label.data)
     label = map(Label.get_full_profile, label)
     label = map(asdict, label)
     label = list(label)
 
     return label
-        
+
+
+def get_label_profiles(profile_urls: list[str]) -> Dataset:
+    label_container = Label.get_full_profiles(profile_urls)
+    label_container = list(map(lambda n: n.to_dict(), label_container))
+    
+    label_key = select(label_container, 'label_key')
+    label_links = select(label_container, 'links')
+    label_releases = select(label_container, 'releases')
+    label_roster = select(label_container, 'roster')
+    label_profile = select(label_container, 'profile')
+    
+    label_roster = rename(label_roster, dict(current='roster_current', past='roster_past'))
+    label_links = select(label_links, 'links')
+
+    label = zip(label_key, label_profile, label_releases, label_roster, label_links)
+    label = [dict(**key, **profile, **albums, **roster, **links) 
+             for key, profile, albums, roster, links in label]
+
+    return label
+
 
 
 def get_genres():
     ...
```

### Comparing `metalarchivist-0.3.5/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.4/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.3.5
+Version: 0.4
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.3.5/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.4/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/test/test_albums.py` & `metalarchivist-0.4/src/test/test_albums.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,18 @@
             album_band = release['album_url'].split('/')[-3]
             band = release['band_url'].split('/')[-2]
             self.assertIn(band, album_band)
 
         output_path = os.path.join(self.config['unittests']['OUTPUTDIR'], 'test-releases.json')
         json.dump(releases, open(output_path, 'w'))
 
+
+class TestAlbumProfile(unittest.TestCase):
+    metalarchivist, interface, export, config = load_module()
+    
     def test_album_profile(self):
         self.assertIn('Album', dir(self.export))
 
         album = self.export.Album.get_profile('https://www.metal-archives.com/albums/Urfaust/Untergang/1161736')
         self.assertIsNotNone(album)
 
         album_json = album.to_dict()
@@ -241,18 +245,21 @@
 
         self.assertIn('band_key', album_band_link)
 
     def test_album_profiles(self):
 
         self.assertIn('Album', dir(self.export))
 
-        album = self.export.Album.get_profiles(['https://www.metal-archives.com/albums/Urfaust/Untergang/1161736',
-                                                'https://www.metal-archives.com/albums/Furia/Huta_Luna/1166382',
-                                                'https://www.metal-archives.com/albums/Hades_Almighty/...Again_Shall_Be/91367'])
-        self.assertIsNotNone(album)
+        albums = self.export.Album.get_profiles(['https://www.metal-archives.com/albums/Urfaust/Untergang/1161736',
+                                                 'https://www.metal-archives.com/albums/Furia/Huta_Luna/1166382',
+                                                 'https://www.metal-archives.com/albums/Hades_Almighty/...Again_Shall_Be/91367'])
+        self.assertIsNotNone(albums)
+
+        album = albums[0]
+        self.assertEqual(album.name, 'Untergang')
 
     # def test_album_themes(self):
     #     metalarchivist = prepare_submodule(Submodule.MODULE)
     #     self.assertIsNotNone(metalarchivist)
 
     #     interface = prepare_submodule(Submodule.IFACE)
     #     self.assertIsNotNone(interface)
```

### Comparing `metalarchivist-0.3.5/src/test/test_bands.py` & `metalarchivist-0.4/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/test/test_genres.py` & `metalarchivist-0.4/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/test/test_labels.py` & `metalarchivist-0.4/src/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.5/src/test/test_themes.py` & `metalarchivist-0.4/src/test/test_themes.py`

 * *Files identical despite different names*


# Comparing `tmp/tmticket-0.2.8.tar.gz` & `tmp/tmticket-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.8.tar", last modified: Mon May 20 01:43:21 2024, max compression
+gzip compressed data, was "tmticket-0.2.9.tar", last modified: Mon May 20 01:47:39 2024, max compression
```

## Comparing `tmticket-0.2.8.tar` & `tmticket-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:43:21.357041 tmticket-0.2.8/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:43:21.356041 tmticket-0.2.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:43:21.353041 tmticket-0.2.8/pytmtickets/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.8/pytmtickets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5717 2024-05-20 01:41:15.000000 tmticket-0.2.8/pytmtickets/client.py
--rw-r--r--   0 root         (0) root         (0)    17146 2024-05-20 01:32:07.000000 tmticket-0.2.8/pytmtickets/model.py
--rw-r--r--   0 root         (0) root         (0)     4379 2024-05-20 01:01:42.000000 tmticket-0.2.8/pytmtickets/query.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 01:43:21.357041 tmticket-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 01:42:51.000000 tmticket-0.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:43:21.355041 tmticket-0.2.8/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:43:20.000000 tmticket-0.2.8/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 01:43:21.000000 tmticket-0.2.8/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 01:43:20.000000 tmticket-0.2.8/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 01:43:20.000000 tmticket-0.2.8/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 01:43:20.000000 tmticket-0.2.8/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:47:39.512874 tmticket-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:47:39.511874 tmticket-0.2.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:47:39.507874 tmticket-0.2.9/pytmtickets/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.9/pytmtickets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5742 2024-05-20 01:47:10.000000 tmticket-0.2.9/pytmtickets/client.py
+-rw-r--r--   0 root         (0) root         (0)    17156 2024-05-20 01:45:54.000000 tmticket-0.2.9/pytmtickets/model.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2024-05-20 01:01:42.000000 tmticket-0.2.9/pytmtickets/query.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 01:47:39.512874 tmticket-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 01:46:47.000000 tmticket-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:47:39.511874 tmticket-0.2.9/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:47:38.000000 tmticket-0.2.9/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 01:47:39.000000 tmticket-0.2.9/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 01:47:38.000000 tmticket-0.2.9/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 01:47:38.000000 tmticket-0.2.9/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 01:47:38.000000 tmticket-0.2.9/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.8/pytmtickets/client.py` & `tmticket-0.2.9/pytmtickets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import aiohttp
 import logging
-import re
+import re  # Ensure re is imported
 from typing import Any, Dict, Optional
 from .query import AttractionQuery, ClassificationQuery, EventQuery, VenueQuery
 
 log = logging.getLogger(__name__)
 
 class AsyncApiClient:
     """AsyncApiClient is the main wrapper for the Discovery API, updated for asynchronous operation."""
```

### Comparing `tmticket-0.2.8/pytmtickets/model.py` & `tmticket-0.2.9/pytmtickets/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import aiohttp  # Assuming aiohttp is used for async operations
+import re
 
 def _assign_links(obj, json_obj, base_url=None):
     """Assigns `links` attribute to an object from JSON"""
     json_links = json_obj.get('_links')
     if not json_links:
         obj.links = {}
     else:
```

### Comparing `tmticket-0.2.8/pytmtickets/query.py` & `tmticket-0.2.9/pytmtickets/query.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.8/setup.py` & `tmticket-0.2.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.2.8',
+    version='0.2.9',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
 #    long_description=read('README.rst'),
     license='MIT',
     keywords='Ticketmaster',
     url='https://github.com/hokiebrian/pytmtickets',
```


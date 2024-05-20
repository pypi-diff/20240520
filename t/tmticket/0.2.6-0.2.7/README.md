# Comparing `tmp/tmticket-0.2.6.tar.gz` & `tmp/tmticket-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.6.tar", last modified: Mon May 20 01:28:04 2024, max compression
+gzip compressed data, was "tmticket-0.2.7.tar", last modified: Mon May 20 01:38:14 2024, max compression
```

## Comparing `tmticket-0.2.6.tar` & `tmticket-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:28:04.456364 tmticket-0.2.6/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:28:04.455364 tmticket-0.2.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:28:04.452364 tmticket-0.2.6/pytmtickets/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.6/pytmtickets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4992 2024-05-20 01:01:30.000000 tmticket-0.2.6/pytmtickets/client.py
--rw-r--r--   0 root         (0) root         (0)    12153 2024-05-20 01:27:31.000000 tmticket-0.2.6/pytmtickets/model.py
--rw-r--r--   0 root         (0) root         (0)     4379 2024-05-20 01:01:42.000000 tmticket-0.2.6/pytmtickets/query.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 01:28:04.456364 tmticket-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 01:27:40.000000 tmticket-0.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:28:04.455364 tmticket-0.2.6/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:28:03.000000 tmticket-0.2.6/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 01:28:04.000000 tmticket-0.2.6/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 01:28:03.000000 tmticket-0.2.6/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 01:28:03.000000 tmticket-0.2.6/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 01:28:03.000000 tmticket-0.2.6/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:38:14.695029 tmticket-0.2.7/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:38:14.694029 tmticket-0.2.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:38:14.691029 tmticket-0.2.7/pytmtickets/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.7/pytmtickets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2024-05-20 01:36:43.000000 tmticket-0.2.7/pytmtickets/client.py
+-rw-r--r--   0 root         (0) root         (0)    17146 2024-05-20 01:32:07.000000 tmticket-0.2.7/pytmtickets/model.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2024-05-20 01:01:42.000000 tmticket-0.2.7/pytmtickets/query.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 01:38:14.695029 tmticket-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 01:37:09.000000 tmticket-0.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:38:14.693029 tmticket-0.2.7/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:38:14.000000 tmticket-0.2.7/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 01:38:14.000000 tmticket-0.2.7/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 01:38:14.000000 tmticket-0.2.7/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 01:38:14.000000 tmticket-0.2.7/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 01:38:14.000000 tmticket-0.2.7/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.6/pytmtickets/client.py` & `tmticket-0.2.7/pytmtickets/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-"""API client classes"""
 import aiohttp
 import logging
 from typing import Any, Dict, Optional
 from .query import AttractionQuery, ClassificationQuery, EventQuery, VenueQuery
 
 log = logging.getLogger(__name__)
 
@@ -14,15 +13,22 @@
 
     def __init__(self, api_key: str):
         self.__api_key = {'apikey': api_key}
         self.events = EventQuery(api_client=self)
         self.venues = VenueQuery(api_client=self)
         self.attractions = AttractionQuery(api_client=self)
         self.classifications = ClassificationQuery(api_client=self)
+        self.session = None
+
+    async def __aenter__(self):
         self.session = aiohttp.ClientSession()
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self.session.close()
 
     async def search(self, method: str, **kwargs: Any) -> Dict[str, Any]:
         """Generic API request, converted for asynchronous operation"""
         params = {k: v for k, v in kwargs.items() if v is not None}
         url = self.__method_url(method)
         async with self.session.get(url, params={**self.__api_key, **params}) as resp:
             resp.raise_for_status()
@@ -38,15 +44,16 @@
         """Gets a specific href from '_links' object in a response, asynchronously"""
         async with self.session.get(link) as resp:
             resp.raise_for_status()
             return await self._handle_response(resp)
 
     async def close(self) -> None:
         """Close the aiohttp session."""
-        await self.session.close()
+        if self.session:
+            await self.session.close()
 
     @property
     def api_key(self) -> Dict[str, str]:
         return self.__api_key
 
     @api_key.setter
     def api_key(self, api_key: str) -> None:
@@ -131,7 +138,24 @@
             size=page_data.get('size', 0),
             total_elements=page_data.get('totalElements', 0),
             total_pages=page_data.get('totalPages', 0)
         )
 
     def __iter__(self):
         return iter(self.items)
+
+def _assign_links(obj, json_obj, base_url=None):
+    """Assigns `links` attribute to an object from JSON"""
+    json_links = json_obj.get('_links')
+    if not json_links:
+        obj.links = {}
+    else:
+        obj_links = {}
+        for k, v in json_links.items():
+            if 'href' in v:
+                href = re.sub("({.+})", "", v['href'])
+                if base_url:
+                    href = f"{base_url}{href}"
+                obj_links[k] = href
+            else:
+                obj_links[k] = v
+        obj.links = obj_links
```

### Comparing `tmticket-0.2.6/pytmtickets/query.py` & `tmticket-0.2.7/pytmtickets/query.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.6/setup.py` & `tmticket-0.2.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.2.6',
+    version='0.2.7',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
 #    long_description=read('README.rst'),
     license='MIT',
     keywords='Ticketmaster',
     url='https://github.com/hokiebrian/pytmtickets',
```


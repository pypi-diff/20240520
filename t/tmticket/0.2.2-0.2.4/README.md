# Comparing `tmp/tmticket-0.2.2.tar.gz` & `tmp/tmticket-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.2.tar", last modified: Wed May  8 00:06:29 2024, max compression
+gzip compressed data, was "tmticket-0.2.4.tar", last modified: Mon May 20 00:54:36 2024, max compression
```

## Comparing `tmticket-0.2.2.tar` & `tmticket-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.254469 tmticket-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:29.253469 tmticket-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 00:06:29.254469 tmticket-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      968 2024-05-08 00:06:04.000000 tmticket-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.250469 tmticket-0.2.2/tmticket/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5702 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/client.py
--rw-r--r--   0 root         (0) root         (0)    13241 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/model.py
--rw-r--r--   0 root         (0) root         (0)     4525 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.252469 tmticket-0.2.2/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2024-05-08 00:06:29.000000 tmticket-0.2.2/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:54:36.969733 tmticket-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 00:54:36.968733 tmticket-0.2.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:54:36.965733 tmticket-0.2.4/pytmtickets/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.4/pytmtickets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-20 00:44:04.000000 tmticket-0.2.4/pytmtickets/client.py
+-rw-r--r--   0 root         (0) root         (0)    11787 2024-05-20 00:53:18.000000 tmticket-0.2.4/pytmtickets/model.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2024-05-20 00:42:28.000000 tmticket-0.2.4/pytmtickets/query.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 00:54:36.969733 tmticket-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 00:46:58.000000 tmticket-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:54:36.967733 tmticket-0.2.4/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.2/tmticket/query.py` & `tmticket-0.2.4/pytmtickets/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Classes to handle API queries/searches"""
-import aiohttp
+import logging
+from typing import Any, Dict, List, Type, Optional
 from tmticket.model import Venue, Event, Attraction, Classification
 
+log = logging.getLogger(__name__)
+
 class BaseQuery:
     """Base query/parent class for specific search types."""
     attr_map = {
         'start_date_time': 'startDateTime',
         'end_date_time': 'endDateTime',
         'onsale_start_date_time': 'onsaleStartDateTime',
         'onsale_end_date_time': 'onsaleEndDateTime',
@@ -30,105 +33,81 @@
         'page': 'page',
         'size': 'size',
         'locale': 'locale',
         'latlong': 'latlong',
         'radius': 'radius'
     }
 
-    def __init__(self, api_client, method, model):
+    def __init__(self, api_client, method: str, model: Type[Any]):
         self.api_client = api_client
         self.method = method
         self.model = model
 
-    async def __get(self, **kwargs):
-        """Asynchronously sends final request to `ApiClient`"""
-        async with aiohttp.ClientSession() as session:
-            async with session.get(f"{self.api_client.url}/{self.method}", params={**self.api_client.api_key, **kwargs}) as response:
-                return await response.json()
-
-    async def _get(self, keyword=None, entity_id=None, sort=None, include_test=None, page=None, size=None, locale=None, **kwargs):
+    async def _get(self, **kwargs: Any) -> List[Any]:
         """Asynchronously handles basic API search request"""
-        search_args = {
-            'keyword': keyword,
-            'id': entity_id,
-            'sort': sort,
-            'include_test': include_test,
-            'page': page,
-            'size': size,
-            'locale': locale,
-            **kwargs
-        }
-        params = self._search_params(**search_args)
-        return await self.__get(**params)
+        params = self._search_params(**kwargs)
+        url = f"{self.api_client.url}/{self.method}.json"
+        async with self.api_client.session.get(url, params={**self.api_client.api_key, **params}) as response:
+            response.raise_for_status()
+            data = await response.json()
+            return [self.model.from_json(item) for item in data.get('_embedded', {}).get(self.method, [])]
 
-    async def by_id(self, entity_id):
+    async def by_id(self, entity_id: str) -> Any:
         """Asynchronously get a specific object by its ID"""
-        return await self._get(entity_id=entity_id)
+        response = await self._get(id=entity_id)
+        return self.model.from_json(response)
 
-    def _search_params(self, **kwargs):
+    def _search_params(self, **kwargs: Any) -> Dict[str, Any]:
         """Maps parameter names to API-friendly parameters"""
-        kw_map = {}
-        for k, v in kwargs.items():
-            api_key = self.attr_map.get(k)
-            if api_key:
-                kw_map[api_key] = v
-            else:
-                kw_map[k] = v
-        return {k: v for k, v in kw_map.items() if v is not None}
+        return {self.attr_map.get(k, k): v for k, v in kwargs.items() if v is not None}
 
 class AttractionQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'attractions', Attraction)
 
-    async def find(self, **kwargs):
+    async def find(self, **kwargs: Any) -> List[Attraction]:
         return await self._get(**kwargs)
 
 class ClassificationQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'classifications', Classification)
 
+    async def find(self, **kwargs: Any) -> List[Classification]:
+        return await self._get(**kwargs)
 
-    def segment_by_id(self, segment_id):
-        """Return a ``Segment`` matching this ID"""
-        return self.by_id(segment_id).segment
-
-    def genre_by_id(self, genre_id):
-        """Return a ``Genre`` matching this ID"""
-        genre = None
-        resp = self.by_id(genre_id)
-        if resp.segment:
-            for genre in resp.segment.genres:
+    async def segment_by_id(self, segment_id: str) -> Optional[Any]:
+        """Return a `Segment` matching this ID"""
+        classification = await self.by_id(segment_id)
+        return classification.segment if classification else None
+
+    async def genre_by_id(self, genre_id: str) -> Optional[Any]:
+        """Return a `Genre` matching this ID"""
+        classification = await self.by_id(genre_id)
+        if classification and classification.segment:
+            for genre in classification.segment.genres:
                 if genre.id == genre_id:
-                    genre = genre
-        return genre
+                    return genre
+        return None
 
-    def subgenre_by_id(self, subgenre_id):
-        """Return a ``SubGenre`` matching this ID"""
-        subgenre = None
-        segment = self.by_id(subgenre_id).segment
-        if segment:
-            subgenres = [
-                subg for genre in segment.genres
-                for subg in genre.subgenres
-            ]
-            for subg in subgenres:
-                if subg.id == subgenre_id:
-                    subgenre = subg
-        return subgenre
-
-
-    async def find(self, **kwargs):
-        return await self._get(**kwargs)
+    async def subgenre_by_id(self, subgenre_id: str) -> Optional[Any]:
+        """Return a `SubGenre` matching this ID"""
+        classification = await self.by_id(subgenre_id)
+        if classification and classification.segment:
+            for genre in classification.segment.genres:
+                for subgenre in genre.subgenres:
+                    if subgenre.id == subgenre_id:
+                        return subgenre
+        return None
 
 class EventQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'events', Event)
 
-    async def find(self, **kwargs):
+    async def find(self, **kwargs: Any) -> List[Event]:
         return await self._get(**kwargs)
 
 class VenueQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'venues', Venue)
 
-    async def find(self, **kwargs):
+    async def find(self, **kwargs: Any) -> List[Venue]:
         return await self._get(**kwargs)
```


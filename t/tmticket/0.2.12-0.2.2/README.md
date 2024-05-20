# Comparing `tmp/tmticket-0.2.12.tar.gz` & `tmp/tmticket-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.12.tar", last modified: Mon May 20 02:00:24 2024, max compression
+gzip compressed data, was "tmticket-0.2.2.tar", last modified: Wed May  8 00:06:29 2024, max compression
```

## Comparing `tmticket-0.2.12.tar` & `tmticket-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 02:00:24.106735 tmticket-0.2.12/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-20 02:00:24.106735 tmticket-0.2.12/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 02:00:24.103735 tmticket-0.2.12/pytmtickets/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.12/pytmtickets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5717 2024-05-20 01:57:52.000000 tmticket-0.2.12/pytmtickets/client.py
--rw-r--r--   0 root         (0) root         (0)    17156 2024-05-20 01:45:54.000000 tmticket-0.2.12/pytmtickets/model.py
--rw-r--r--   0 root         (0) root         (0)     4379 2024-05-20 01:01:42.000000 tmticket-0.2.12/pytmtickets/query.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 02:00:24.107735 tmticket-0.2.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      522 2024-05-20 02:00:08.000000 tmticket-0.2.12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 02:00:24.105735 tmticket-0.2.12/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-20 02:00:23.000000 tmticket-0.2.12/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 02:00:23.000000 tmticket-0.2.12/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 02:00:23.000000 tmticket-0.2.12/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 02:00:23.000000 tmticket-0.2.12/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 02:00:23.000000 tmticket-0.2.12/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.254469 tmticket-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:29.253469 tmticket-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 00:06:29.254469 tmticket-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2024-05-08 00:06:04.000000 tmticket-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.250469 tmticket-0.2.2/tmticket/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5702 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/model.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.252469 tmticket-0.2.2/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-08 00:06:29.000000 tmticket-0.2.2/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.12/pytmtickets/client.py` & `tmticket-0.2.2/tmticket/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,100 +1,149 @@
+"""API client classes"""
 import aiohttp
+import asyncio
 import logging
-import re
-from typing import Any, Dict, Optional
-from .query import AttractionQuery, ClassificationQuery, EventQuery, VenueQuery
+from collections import namedtuple
+from urllib import parse
+from tmticket.query import AttractionQuery, ClassificationQuery, EventQuery, VenueQuery
+from tmticket.model import Page
 
 log = logging.getLogger(__name__)
+log.setLevel(logging.INFO)
+sh = logging.StreamHandler()
+sh.setLevel(logging.INFO)
+sf = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+sh.setFormatter(sf)
+log.addHandler(sh)
 
-class AsyncApiClient:
-    """AsyncApiClient is the main wrapper for the Discovery API, updated for asynchronous operation."""
 
+class AsyncApiClient:
+    """AsyncApiClient is the main wrapper for the Discovery API, updated for asynchronous operation.
+    
+    Example:    
+    Get the first page result for venues matching keyword 'Tabernacle':
+    
+    ```
+    import ticketpy
+    import asyncio
+    
+    async def main():
+        client = ticketpy.AsyncApiClient("your_api_key")
+        resp = await client.venues.find(keyword="Tabernacle").one()
+        for venue in resp:
+            print(venue.name)
+    if __name__ == "__main__":
+        asyncio.run(main())
+    ```
+    """
     root_url = 'https://app.ticketmaster.com'
     url = 'https://app.ticketmaster.com/discovery/v2'
 
-    def __init__(self, api_key: str):
-        self.__api_key = {'apikey': api_key}
+    def __init__(self, api_key):
+        self.__api_key = None
+        self.api_key = api_key
         self.events = EventQuery(api_client=self)
         self.venues = VenueQuery(api_client=self)
         self.attractions = AttractionQuery(api_client=self)
         self.classifications = ClassificationQuery(api_client=self)
-        self.session = None
+        self.segment_by_id = self.classifications.segment_by_id
+        self.genre_by_id = self.classifications.genre_by_id
+        self.subgenre_by_id = self.classifications.subgenre_by_id
 
-    async def __aenter__(self):
-        self.session = aiohttp.ClientSession()
-        return self
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self.session.close()
-
-    async def search(self, method: str, **kwargs: Any) -> Dict[str, Any]:
+    async def search(self, method, **kwargs):
         """Generic API request, converted for asynchronous operation"""
-        params = {k: v for k, v in kwargs.items() if v is not None}
-        url = self.__method_url(method)
-        async with self.session.get(url, params={**self.__api_key, **params}) as resp:
-            resp.raise_for_status()
-            return await resp.json()
+        kwargs = {k: v for (k, v) in kwargs.items() if v is not None}
+        updates = self.api_key
+
+        for k, v in kwargs.items():
+            if k in ['includeTBA', 'includeTBD', 'includeTest']:
+                updates[k] = self.__yes_no_only(v)
+            elif k in ['size', 'radius', 'marketId']:
+                updates[k] = str(v)
+        kwargs.update(updates)
+
+        urls = {
+            'events': self.__method_url('events'),
+            'venues': self.__method_url('venues'),
+            'attractions': self.__method_url('attractions'),
+            'classifications': self.__method_url('classifications')
+        }
+
+        async with aiohttp.ClientSession() as session:
+            async with session.get(urls[method], params=kwargs) as resp:
+                return await self._handle_response(resp)
 
-    async def _handle_response(self, response: aiohttp.ClientResponse) -> Dict[str, Any]:
+    async def _handle_response(self, response):
         """Handles response, raising ApiException if needed or returning response JSON object asynchronously"""
         if response.status == 200:
             return await response.json()
-        raise ApiException(await response.json())
+        elif response.status == 401:
+            self.__fault(await response.json())
+        elif response.status == 400:
+            self.__error(await response.json())
+        else:
+            self.__unknown_error(await response.json())
 
-    async def get_url(self, link: str) -> Any:
+    async def get_url(self, link):
         """Gets a specific href from '_links' object in a response, asynchronously"""
-        async with self.session.get(link) as resp:
-            resp.raise_for_status()
-            return await self._handle_response(resp)
-
-    async def close(self) -> None:
-        """Close the aiohttp session."""
-        if self.session:
-            await self.session.close()
+        parsed_link = self._parse_link(link)
+        async with aiohttp.ClientSession() as session:
+            async with session.get(parsed_link.url, params=parsed_link.params) as resp:
+                return Page.from_json(await self._handle_response(resp))
 
     @property
-    def api_key(self) -> Dict[str, str]:
+    def api_key(self):
         return self.__api_key
 
     @api_key.setter
-    def api_key(self, api_key: str) -> None:
+    def api_key(self, api_key):
         self.__api_key = {'apikey': api_key}
 
     @staticmethod
-    def __method_url(method: str) -> str:
-        return f"{AsyncApiClient.url}/{method}.json"
+    def __method_url(method):
+        return "{}/{}.json".format(AsyncApiClient.url, method)
+
+    @staticmethod
+    def __yes_no_only(s):
+        s = str(s).lower()
+        if s in ['true', 'yes']:
+            s = 'yes'
+        elif s in ['false', 'no']:
+            s = 'no'
+        return s
+
 
 class ApiException(Exception):
     """Exception thrown for API-related error messages"""
-    def __init__(self, *args: Any) -> None:
+    def __init__(self, *args):
         super().__init__(*args)
 
 class AsyncPagedResponse:
     """Asynchronously iterates through API response pages."""
-    def __init__(self, api_client: AsyncApiClient, response: Dict[str, Any]):
+    def __init__(self, api_client, response):
         self.api_client = api_client
+        self.page = None
         self.page = Page.from_json(response)
 
-    async def limit(self, max_pages: int = 5) -> Any:
+    async def limit(self, max_pages=5):
         """Asynchronously retrieve a number of pages, returning a list of all entities."""
         all_items = []
         counter = 0
         async for pg in self:
             if counter >= max_pages:
                 break
             counter += 1
             all_items.extend(pg)
         return all_items
 
-    async def one(self) -> Any:
+    async def one(self):
         """Asynchronously get items from the first page result."""
         return [i for i in self.page]
 
-    async def maximum(self, max_pages: int = 49) -> Any:
+    async def maximum(self, max_pages=49): # API limits paging depth to (page * size) <= 1000
         """Asynchronously retrieves maximum pages in a result, returning a flat list."""
         all_items = []
         counter = 0
         async for pg in self:
             if counter >= max_pages:
                 break
             counter += 1
@@ -104,59 +153,14 @@
     def __aiter__(self):
         return self._page_iterator()
 
     async def _page_iterator(self):
         current_page = self.page
         yield current_page
         next_url = current_page.links.get('next')
-
+        
         while next_url:
             log.debug(f"Requesting page: {next_url}")
             page_data = await self.api_client.get_url(next_url)
-            next_page = Page.from_json(page_data)
-            yield next_page
-            next_url = next_page.links.get('next')
-
-class Page:
-    """Represents a page in a paged response."""
-    def __init__(self, items: Any, links: Dict[str, str], page: int, size: int, total_elements: int, total_pages: int):
-        self.items = items
-        self.links = links
-        self.page = page
-        self.size = size
-        self.total_elements = total_elements
-        self.total_pages = total_pages
-
-    @staticmethod
-    def from_json(json_data: Dict[str, Any]) -> 'Page':
-        """Creates a `Page` object from JSON data."""
-        items = json_data.get('_embedded', {}).get('events', [])
-        links = json_data.get('_links', {})
-        page_data = json_data.get('page', {})
-        return Page(
-            items=items,
-            links=links,
-            page=page_data.get('number', 0),
-            size=page_data.get('size', 0),
-            total_elements=page_data.get('totalElements', 0),
-            total_pages=page_data.get('totalPages', 0)
-        )
-
-    def __iter__(self):
-        return iter(self.items)
-
-def _assign_links(obj, json_obj, base_url=None):
-    """Assigns `links` attribute to an object from JSON"""
-    json_links = json_obj.get('_links')
-    if not json_links:
-        obj.links = {}
-    else:
-        obj_links = {}
-        for k, v in json_links.items():
-            if 'href' in v:
-                href = re.sub("({.+})", "", v['href'])
-                if base_url:
-                    href = f"{base_url}{href}"
-                obj_links[k] = href
-            else:
-                obj_links[k] = v
-        obj.links = obj_links
+            current_page = Page.from_json(page_data)
+            next_url = current_page.links.get('next')
+            yield current_page
```

### Comparing `tmticket-0.2.12/pytmtickets/model.py` & `tmticket-0.2.2/tmticket/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import aiohttp  # Assuming aiohttp is used for async operations
+"""Models for API objects"""
+from datetime import datetime
 import re
+import aiohttp  # Assuming aiohttp is used for async operations
 
 def _assign_links(obj, json_obj, base_url=None):
     """Assigns `links` attribute to an object from JSON"""
     json_links = json_obj.get('_links')
     if not json_links:
         obj.links = {}
     else:
@@ -49,37 +51,21 @@
         self.status = status
         self.classifications = classifications
         self.links = links
 
     @staticmethod
     def from_json(json_event):
         """Creates an `Event` from API's JSON response"""
-        e = Event(
-            event_id=json_event.get('id'),
-            name=json_event.get('name'),
-            start_date=json_event.get('dates', {}).get('start', {}).get('localDate'),
-            start_time=json_event.get('dates', {}).get('start', {}).get('localTime'),
-            status=json_event.get('dates', {}).get('status', {}).get('code'),
-            classifications=[Classification.from_json(cl) for cl in json_event.get('classifications', [])]
-        )
+        e = Event()
+        e.id = json_event.get('id')
+        e.name = json_event.get('name')
+        # Additional attributes setup
         _assign_links(e, json_event)
         return e
 
-    def to_dict(self):
-        """Convert the Event object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'start_date': self.start_date,
-            'start_time': self.start_time,
-            'status': self.status,
-            'classifications': [cl.to_dict() for cl in self.classifications] if self.classifications else [],
-            'links': self.links,
-        }
-
     async def fetch_additional_details(self):
         """Asynchronously fetch additional event details (hypothetical example)"""
         async with aiohttp.ClientSession() as session:
             async with session.get(self.links['self']) as response:
                 details = await response.json()
                 # Process and update event instance with additional details
 
@@ -139,38 +125,14 @@
         v.state_code = json_venue['state'].get('stateCode')
         v.latitude = json_venue['location'].get('latitude')
         v.longitude = json_venue['location'].get('longitude')
         # Process additional attributes as before
         _assign_links(v, json_venue)
         return v
 
-    def to_dict(self):
-        """Convert the Venue object to a dictionary for serialization"""
-        return {
-            'name': self.name,
-            'id': self.id,
-            'address': self.address,
-            'postal_code': self.postal_code,
-            'city': self.city,
-            'state_code': self.state_code,
-            'latitude': self.latitude,
-            'longitude': self.longitude,
-            'timezone': self.timezone,
-            'url': self.url,
-            'box_office_info': self.box_office_info,
-            'dmas': self.dmas,
-            'markets': self.markets,
-            'general_info': self.general_info,
-            'social': self.social,
-            'images': self.images,
-            'parking_detail': self.parking_detail,
-            'accessible_seating_detail': self.accessible_seating_detail,
-            'links': self.links,
-        }
-
     async def fetch_additional_details(self, api_client):
         """Asynchronously fetch additional venue details.
         
         Args:
             api_client: Instance of an asynchronous API client.
         """
         # Example URL construction, adjust based on your API's design
@@ -205,26 +167,14 @@
         att.test = json_obj.get('test', False)  # Assuming 'test' is a boolean field
         att.images = json_obj.get('images', [])
         classifications = json_obj.get('classifications', [])
         att.classifications = [Classification.from_json(cl) for cl in classifications]
         _assign_links(att, json_obj)
         return att
 
-    def to_dict(self):
-        """Convert the Attraction object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'url': self.url,
-            'classifications': [cl.to_dict() for cl in self.classifications] if self.classifications else [],
-            'images': self.images,
-            'test': self.test,
-            'links': self.links,
-        }
-
     async def fetch_additional_details(self, api_client):
         """Asynchronously fetch additional details for the attraction.
         
         Args:
             api_client: Instance of an asynchronous API client capable of making GET requests.
         """
         details_url = self.links.get('self', '')  # Example, adjust based on actual API design
@@ -233,14 +183,15 @@
                 details_json = await response.json()
                 # Here you would process the details_json to extract and integrate additional details
                 print(details_json)  # Placeholder for actual logic
 
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+
 class Classification:
     """Classification object (segment/genre/sub-genre)"""
     def __init__(self, segment=None, classification_type=None, subtype=None, primary=None, links=None):
         self.segment = segment
         self.type = classification_type
         self.subtype = subtype
         self.primary = primary
@@ -259,24 +210,14 @@
 
         if 'subType' in json_obj:
             cl.subtype = ClassificationSubType(json_obj['subType']['id'], json_obj['subType']['name'])
 
         _assign_links(cl, json_obj)
         return cl
 
-    def to_dict(self):
-        """Convert the Classification object to a dictionary for serialization"""
-        return {
-            'segment': self.segment.to_dict() if self.segment else None,
-            'type': self.type.to_dict() if self.type else None,
-            'subtype': self.subtype.to_dict() if self.subtype else None,
-            'primary': self.primary,
-            'links': self.links,
-        }
-
     def __str__(self):
         return str(self.type)
 
     # Hypothetical async method to fetch additional details
     async def fetch_additional_details(self, api_client):
         """Asynchronously fetch additional classification details."""
         # This method is hypothetical and assumes there's a relevant URL in self.links
@@ -316,74 +257,39 @@
 
         if 'subType' in json_obj:
             ec.subtype = ClassificationSubType(json_obj['subType']['id'], json_obj['subType']['name'])
 
         _assign_links(ec, json_obj)
         return ec
 
-    def to_dict(self):
-        """Convert the EventClassification object to a dictionary for serialization"""
-        return {
-            'genre': self.genre.to_dict() if self.genre else None,
-            'subgenre': self.subgenre.to_dict() if self.subgenre else None,
-            'segment': self.segment.to_dict() if self.segment else None,
-            'type': self.type.to_dict() if self.type else None,
-            'subtype': self.subtype.to_dict() if self.subtype else None,
-            'primary': self.primary,
-            'links': self.links,
-        }
-
     def __str__(self):
         return f"Segment: {self.segment} / Genre: {self.genre} / Subgenre: {self.subgenre} / Type: {self.type} / Subtype: {self.subtype}"
 
+
 class ClassificationType:
     def __init__(self, type_id=None, type_name=None, subtypes=None):
         self.id = type_id
         self.name = type_name
         self.subtypes = subtypes
 
-    @staticmethod
-    def from_json(json_obj):
-        return ClassificationType(
-            type_id=json_obj.get('id'),
-            type_name=json_obj.get('name')
-        )
-
-    def to_dict(self):
-        """Convert the ClassificationType object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# No changes needed here unless dynamic fetching of subtype details becomes necessary
+
 class ClassificationSubType:
     def __init__(self, type_id=None, type_name=None):
         self.id = type_id
         self.name = type_name
 
-    @staticmethod
-    def from_json(json_obj):
-        return ClassificationSubType(
-            type_id=json_obj.get('id'),
-            type_name=json_obj.get('name')
-        )
-
-    def to_dict(self):
-        """Convert the ClassificationSubType object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Similar to ClassificationType, asynchronous behavior might be added for dynamic data fetching
+
 class Segment:
     def __init__(self, segment_id=None, segment_name=None, genres=None, links=None):
         self.id = segment_id
         self.name = segment_name
         self.genres = genres  # Could be a list of Genre instances
         self.links = links
 
@@ -395,26 +301,19 @@
         # Processing embedded genres if available
         if '_embedded' in json_obj:
             genres = json_obj['_embedded'].get('genres', [])
             seg.genres = [Genre.from_json(g) for g in genres]
         _assign_links(seg, json_obj)
         return seg
 
-    def to_dict(self):
-        """Convert the Segment object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'genres': [g.to_dict() for g in self.genres] if self.genres else [],
-            'links': self.links,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Could integrate asynchronous methods if genres require fetching additional details
+
 class Genre:
     def __init__(self, genre_id=None, genre_name=None, subgenres=None, links=None):
         self.id = genre_id
         self.name = genre_name
         self.subgenres = subgenres  # Could be a list of SubGenre instances
         self.links = links
 
@@ -425,43 +324,37 @@
         g.name = json_obj.get('name')
         if '_embedded' in json_obj:
             subgenres = json_obj['_embedded'].get('subgenres', [])
             g.subgenres = [SubGenre.from_json(sg) for sg in subgenres]
         _assign_links(g, json_obj)
         return g
 
-    def to_dict(self):
-        """Convert the Genre object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'subgenres': [sg.to_dict() for sg in self.subgenres] if self.subgenres else [],
-            'links': self.links,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Asynchronous enhancements could be added for dynamic subgenre data fetching
+
 class SubGenre:
     def __init__(self, subgenre_id=None, subgenre_name=None, links=None):
         self.id = subgenre_id
         self.name = subgenre_name
         self.links = links
 
     @staticmethod
     def from_json(json_obj):
         sg = SubGenre()
         sg.id = json_obj['id']
         sg.name = json_obj['name']
         _assign_links(sg, json_obj)
         return sg
 
-    def to_dict(self):
-        """Convert the SubGenre object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'links': self.links,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
+
+# Example async usage to fetch and process event details
+async def main():
+    event = Event.from_json({'id': '123', 'name': 'Sample Event', 'links': {'self': 'http://example.com/event/123'}})
+    await event.fetch_additional_details()
+
+if __name__ == '__main__':
+    import asyncio
+    asyncio.run(main())
```

### Comparing `tmticket-0.2.12/pytmtickets/query.py` & `tmticket-0.2.2/tmticket/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """Classes to handle API queries/searches"""
-import logging
-from typing import Any, Dict, List, Type, Optional
-from .model import Venue, Event, Attraction, Classification
-
-log = logging.getLogger(__name__)
+import aiohttp
+from tmticket.model import Venue, Event, Attraction, Classification
 
 class BaseQuery:
     """Base query/parent class for specific search types."""
     attr_map = {
         'start_date_time': 'startDateTime',
         'end_date_time': 'endDateTime',
         'onsale_start_date_time': 'onsaleStartDateTime',
@@ -33,81 +30,105 @@
         'page': 'page',
         'size': 'size',
         'locale': 'locale',
         'latlong': 'latlong',
         'radius': 'radius'
     }
 
-    def __init__(self, api_client, method: str, model: Type[Any]):
+    def __init__(self, api_client, method, model):
         self.api_client = api_client
         self.method = method
         self.model = model
 
-    async def _get(self, **kwargs: Any) -> List[Any]:
+    async def __get(self, **kwargs):
+        """Asynchronously sends final request to `ApiClient`"""
+        async with aiohttp.ClientSession() as session:
+            async with session.get(f"{self.api_client.url}/{self.method}", params={**self.api_client.api_key, **kwargs}) as response:
+                return await response.json()
+
+    async def _get(self, keyword=None, entity_id=None, sort=None, include_test=None, page=None, size=None, locale=None, **kwargs):
         """Asynchronously handles basic API search request"""
-        params = self._search_params(**kwargs)
-        url = f"{self.api_client.url}/{self.method}.json"
-        async with self.api_client.session.get(url, params={**self.api_client.api_key, **params}) as response:
-            response.raise_for_status()
-            data = await response.json()
-            return [self.model.from_json(item) for item in data.get('_embedded', {}).get(self.method, [])]
+        search_args = {
+            'keyword': keyword,
+            'id': entity_id,
+            'sort': sort,
+            'include_test': include_test,
+            'page': page,
+            'size': size,
+            'locale': locale,
+            **kwargs
+        }
+        params = self._search_params(**search_args)
+        return await self.__get(**params)
 
-    async def by_id(self, entity_id: str) -> Any:
+    async def by_id(self, entity_id):
         """Asynchronously get a specific object by its ID"""
-        response = await self._get(id=entity_id)
-        return self.model.from_json(response)
+        return await self._get(entity_id=entity_id)
 
-    def _search_params(self, **kwargs: Any) -> Dict[str, Any]:
+    def _search_params(self, **kwargs):
         """Maps parameter names to API-friendly parameters"""
-        return {self.attr_map.get(k, k): v for k, v in kwargs.items() if v is not None}
+        kw_map = {}
+        for k, v in kwargs.items():
+            api_key = self.attr_map.get(k)
+            if api_key:
+                kw_map[api_key] = v
+            else:
+                kw_map[k] = v
+        return {k: v for k, v in kw_map.items() if v is not None}
 
 class AttractionQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'attractions', Attraction)
 
-    async def find(self, **kwargs: Any) -> List[Attraction]:
+    async def find(self, **kwargs):
         return await self._get(**kwargs)
 
 class ClassificationQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'classifications', Classification)
 
-    async def find(self, **kwargs: Any) -> List[Classification]:
-        return await self._get(**kwargs)
 
-    async def segment_by_id(self, segment_id: str) -> Optional[Any]:
-        """Return a `Segment` matching this ID"""
-        classification = await self.by_id(segment_id)
-        return classification.segment if classification else None
-
-    async def genre_by_id(self, genre_id: str) -> Optional[Any]:
-        """Return a `Genre` matching this ID"""
-        classification = await self.by_id(genre_id)
-        if classification and classification.segment:
-            for genre in classification.segment.genres:
+    def segment_by_id(self, segment_id):
+        """Return a ``Segment`` matching this ID"""
+        return self.by_id(segment_id).segment
+
+    def genre_by_id(self, genre_id):
+        """Return a ``Genre`` matching this ID"""
+        genre = None
+        resp = self.by_id(genre_id)
+        if resp.segment:
+            for genre in resp.segment.genres:
                 if genre.id == genre_id:
-                    return genre
-        return None
+                    genre = genre
+        return genre
 
-    async def subgenre_by_id(self, subgenre_id: str) -> Optional[Any]:
-        """Return a `SubGenre` matching this ID"""
-        classification = await self.by_id(subgenre_id)
-        if classification and classification.segment:
-            for genre in classification.segment.genres:
-                for subgenre in genre.subgenres:
-                    if subgenre.id == subgenre_id:
-                        return subgenre
-        return None
+    def subgenre_by_id(self, subgenre_id):
+        """Return a ``SubGenre`` matching this ID"""
+        subgenre = None
+        segment = self.by_id(subgenre_id).segment
+        if segment:
+            subgenres = [
+                subg for genre in segment.genres
+                for subg in genre.subgenres
+            ]
+            for subg in subgenres:
+                if subg.id == subgenre_id:
+                    subgenre = subg
+        return subgenre
+
+
+    async def find(self, **kwargs):
+        return await self._get(**kwargs)
 
 class EventQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'events', Event)
 
-    async def find(self, **kwargs: Any) -> List[Event]:
+    async def find(self, **kwargs):
         return await self._get(**kwargs)
 
 class VenueQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'venues', Venue)
 
-    async def find(self, **kwargs: Any) -> List[Venue]:
+    async def find(self, **kwargs):
         return await self._get(**kwargs)
```


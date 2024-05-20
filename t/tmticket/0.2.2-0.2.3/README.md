# Comparing `tmp/tmticket-0.2.2.tar.gz` & `tmp/tmticket-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.2.tar", last modified: Wed May  8 00:06:29 2024, max compression
+gzip compressed data, was "tmticket-0.2.3.tar", last modified: Mon May 20 00:37:33 2024, max compression
```

## Comparing `tmticket-0.2.2.tar` & `tmticket-0.2.3.tar`

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
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:37:33.926352 tmticket-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 00:37:33.926352 tmticket-0.2.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:37:33.923352 tmticket-0.2.3/pytmtickets/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-05 19:05:59.000000 tmticket-0.2.3/pytmtickets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5636 2024-05-20 00:31:41.000000 tmticket-0.2.3/pytmtickets/client.py
+-rw-r--r--   0 root         (0) root         (0)    13934 2024-05-20 00:33:25.000000 tmticket-0.2.3/pytmtickets/model.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2024-05-20 00:34:49.000000 tmticket-0.2.3/pytmtickets/query.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 00:37:33.927352 tmticket-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 00:35:54.000000 tmticket-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:37:33.925352 tmticket-0.2.3/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 00:37:33.000000 tmticket-0.2.3/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 00:37:33.000000 tmticket-0.2.3/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 00:37:33.000000 tmticket-0.2.3/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 00:37:33.000000 tmticket-0.2.3/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 00:37:33.000000 tmticket-0.2.3/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.2/tmticket/client.py` & `tmticket-0.2.3/pytmtickets/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,54 @@
 """API client classes"""
 import aiohttp
-import asyncio
 import logging
-from collections import namedtuple
-from urllib import parse
+from typing import Dict, Any
 from tmticket.query import AttractionQuery, ClassificationQuery, EventQuery, VenueQuery
 from tmticket.model import Page
 
 log = logging.getLogger(__name__)
-log.setLevel(logging.INFO)
-sh = logging.StreamHandler()
-sh.setLevel(logging.INFO)
-sf = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-sh.setFormatter(sf)
-log.addHandler(sh)
-
 
 class AsyncApiClient:
     """AsyncApiClient is the main wrapper for the Discovery API, updated for asynchronous operation.
-    
-    Example:    
+
+    Example:
     Get the first page result for venues matching keyword 'Tabernacle':
-    
+
     ```
     import ticketpy
     import asyncio
-    
+
     async def main():
         client = ticketpy.AsyncApiClient("your_api_key")
         resp = await client.venues.find(keyword="Tabernacle").one()
         for venue in resp:
             print(venue.name)
+
     if __name__ == "__main__":
         asyncio.run(main())
     ```
     """
     root_url = 'https://app.ticketmaster.com'
     url = 'https://app.ticketmaster.com/discovery/v2'
 
-    def __init__(self, api_key):
-        self.__api_key = None
-        self.api_key = api_key
+    def __init__(self, api_key: str):
+        self.__api_key = {'apikey': api_key}
         self.events = EventQuery(api_client=self)
         self.venues = VenueQuery(api_client=self)
         self.attractions = AttractionQuery(api_client=self)
         self.classifications = ClassificationQuery(api_client=self)
         self.segment_by_id = self.classifications.segment_by_id
         self.genre_by_id = self.classifications.genre_by_id
         self.subgenre_by_id = self.classifications.subgenre_by_id
+        self.session = aiohttp.ClientSession()
 
-    async def search(self, method, **kwargs):
+    async def search(self, method: str, **kwargs: Any) -> Dict[str, Any]:
         """Generic API request, converted for asynchronous operation"""
-        kwargs = {k: v for (k, v) in kwargs.items() if v is not None}
-        updates = self.api_key
+        kwargs = {k: v for k, v in kwargs.items() if v is not None}
+        updates = self.__api_key
 
         for k, v in kwargs.items():
             if k in ['includeTBA', 'includeTBD', 'includeTest']:
                 updates[k] = self.__yes_no_only(v)
             elif k in ['size', 'radius', 'marketId']:
                 updates[k] = str(v)
         kwargs.update(updates)
@@ -64,86 +56,86 @@
         urls = {
             'events': self.__method_url('events'),
             'venues': self.__method_url('venues'),
             'attractions': self.__method_url('attractions'),
             'classifications': self.__method_url('classifications')
         }
 
-        async with aiohttp.ClientSession() as session:
-            async with session.get(urls[method], params=kwargs) as resp:
-                return await self._handle_response(resp)
+        async with self.session.get(urls[method], params=kwargs) as resp:
+            return await self._handle_response(resp)
 
-    async def _handle_response(self, response):
+    async def _handle_response(self, response: aiohttp.ClientResponse) -> Dict[str, Any]:
         """Handles response, raising ApiException if needed or returning response JSON object asynchronously"""
         if response.status == 200:
             return await response.json()
         elif response.status == 401:
-            self.__fault(await response.json())
+            raise ApiException(await response.json())
         elif response.status == 400:
-            self.__error(await response.json())
+            raise ApiException(await response.json())
         else:
-            self.__unknown_error(await response.json())
+            raise ApiException(await response.json())
 
-    async def get_url(self, link):
+    async def get_url(self, link: str) -> Page:
         """Gets a specific href from '_links' object in a response, asynchronously"""
         parsed_link = self._parse_link(link)
-        async with aiohttp.ClientSession() as session:
-            async with session.get(parsed_link.url, params=parsed_link.params) as resp:
-                return Page.from_json(await self._handle_response(resp))
+        async with self.session.get(parsed_link.url, params=parsed_link.params) as resp:
+            return Page.from_json(await self._handle_response(resp))
+
+    async def close(self):
+        """Close the aiohttp session."""
+        await self.session.close()
 
     @property
-    def api_key(self):
+    def api_key(self) -> Dict[str, str]:
         return self.__api_key
 
     @api_key.setter
-    def api_key(self, api_key):
+    def api_key(self, api_key: str):
         self.__api_key = {'apikey': api_key}
 
     @staticmethod
-    def __method_url(method):
-        return "{}/{}.json".format(AsyncApiClient.url, method)
+    def __method_url(method: str) -> str:
+        return f"{AsyncApiClient.url}/{method}.json"
 
     @staticmethod
-    def __yes_no_only(s):
+    def __yes_no_only(s: str) -> str:
         s = str(s).lower()
         if s in ['true', 'yes']:
-            s = 'yes'
+            return 'yes'
         elif s in ['false', 'no']:
-            s = 'no'
+            return 'no'
         return s
 
-
 class ApiException(Exception):
     """Exception thrown for API-related error messages"""
     def __init__(self, *args):
         super().__init__(*args)
 
 class AsyncPagedResponse:
     """Asynchronously iterates through API response pages."""
-    def __init__(self, api_client, response):
+    def __init__(self, api_client: AsyncApiClient, response: Dict[str, Any]):
         self.api_client = api_client
-        self.page = None
         self.page = Page.from_json(response)
 
-    async def limit(self, max_pages=5):
+    async def limit(self, max_pages: int = 5) -> list:
         """Asynchronously retrieve a number of pages, returning a list of all entities."""
         all_items = []
         counter = 0
         async for pg in self:
             if counter >= max_pages:
                 break
             counter += 1
             all_items.extend(pg)
         return all_items
 
-    async def one(self):
+    async def one(self) -> list:
         """Asynchronously get items from the first page result."""
         return [i for i in self.page]
 
-    async def maximum(self, max_pages=49): # API limits paging depth to (page * size) <= 1000
+    async def maximum(self, max_pages: int = 49) -> list: # API limits paging depth to (page * size) <= 1000
         """Asynchronously retrieves maximum pages in a result, returning a flat list."""
         all_items = []
         counter = 0
         async for pg in self:
             if counter >= max_pages:
                 break
             counter += 1
@@ -153,14 +145,14 @@
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
             current_page = Page.from_json(page_data)
             next_url = current_page.links.get('next')
             yield current_page
```

### Comparing `tmticket-0.2.2/tmticket/model.py` & `tmticket-0.2.3/pytmtickets/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 """Models for API objects"""
 from datetime import datetime
 import re
-import aiohttp  # Assuming aiohttp is used for async operations
+import aiohttp
+from typing import Dict, Any, List
 
-def _assign_links(obj, json_obj, base_url=None):
+def _assign_links(obj, json_obj: Dict[str, Any], base_url: str = None) -> None:
     """Assigns `links` attribute to an object from JSON"""
     json_links = json_obj.get('_links')
-    if not json_links:
-        obj.links = {}
-    else:
-        obj_links = {}
+    obj.links = {}
+    if json_links:
         for k, v in json_links.items():
             if 'href' in v:
-                href = re.sub("({.+})", "", v['href'])
+                href = re.sub(r"({.+})", "", v['href'])
                 if base_url:
                     href = f"{base_url}{href}"
-                obj_links[k] = href
+                obj.links[k] = href
             else:
-                obj_links[k] = v
-        obj.links = obj_links
+                obj.links[k] = v
 
-class Page(list):
+class Page(List):
     """API response page"""
-    def __init__(self, number=None, size=None, total_elements=None, total_pages=None):
-        super().__init__([])
+    def __init__(self, number: int = None, size: int = None, total_elements: int = None, total_pages: int = None):
+        super().__init__()
         self.number = number
         self.size = size
         self.total_elements = total_elements
         self.total_pages = total_pages
 
     @staticmethod
-    def from_json(json_obj):
+    def from_json(json_obj: Dict[str, Any]) -> 'Page':
         """Instantiate and return a Page(list)"""
         pg = Page()
         pg.number = json_obj['page']['number']
         pg.size = json_obj['page']['size']
         pg.total_pages = json_obj['page']['totalPages']
         pg.total_elements = json_obj['page']['totalElements']
         _assign_links(pg, json_obj)
-        # Assuming implementation for adding items to the page based on 'events', 'venues', etc.
+        # Additional logic for adding items to the page based on 'events', 'venues', etc.
         return pg
 
 class Event:
     """Ticketmaster event"""
-    def __init__(self, event_id=None, name=None, start_date=None, start_time=None, status=None, classifications=None, links=None):
+    def __init__(self, event_id: str = None, name: str = None, start_date: str = None, start_time: str = None,
+                 status: str = None, classifications: List = None, links: Dict[str, Any] = None):
         self.id = event_id
         self.name = name
         self.start_date = start_date
         self.start_time = start_time
         self.status = status
         self.classifications = classifications
         self.links = links
 
     @staticmethod
-    def from_json(json_event):
+    def from_json(json_event: Dict[str, Any]) -> 'Event':
         """Creates an `Event` from API's JSON response"""
-        e = Event()
-        e.id = json_event.get('id')
-        e.name = json_event.get('name')
-        # Additional attributes setup
+        e = Event(
+            event_id=json_event.get('id'),
+            name=json_event.get('name'),
+            # Additional attributes setup
+        )
         _assign_links(e, json_event)
         return e
 
-    async def fetch_additional_details(self):
+    async def fetch_additional_details(self) -> None:
         """Asynchronously fetch additional event details (hypothetical example)"""
         async with aiohttp.ClientSession() as session:
             async with session.get(self.links['self']) as response:
                 details = await response.json()
                 # Process and update event instance with additional details
 
 class Venue:
     """A Ticketmaster venue."""
-    def __init__(self, name=None, address=None, city=None, state_code=None,
-                 postal_code=None, latitude=None, longitude=None,
-                 markets=None, url=None, box_office_info=None,
-                 dmas=None, general_info=None, venue_id=None,
-                 social=None, timezone=None, images=None,
-                 parking_detail=None, accessible_seating_detail=None,
-                 links=None):
+    def __init__(self, name: str = None, address: str = None, city: str = None, state_code: str = None,
+                 postal_code: str = None, latitude: float = None, longitude: float = None,
+                 markets: List = None, url: str = None, box_office_info: Dict = None,
+                 dmas: List = None, general_info: Dict = None, venue_id: str = None,
+                 social: Dict = None, timezone: str = None, images: List = None,
+                 parking_detail: str = None, accessible_seating_detail: str = None,
+                 links: Dict[str, Any] = None):
         self.name = name
         self.id = venue_id
         self.address = address
         self.postal_code = postal_code
         self.city = city
         self.state_code = state_code
         self.latitude = latitude
@@ -95,264 +95,245 @@
         self.social = social
         self.images = images
         self.parking_detail = parking_detail
         self.accessible_seating_detail = accessible_seating_detail
         self.links = links
 
     @property
-    def location(self):
+    def location(self) -> Dict[str, Any]:
         """Location-based data (full address, lat/lon, timezone)"""
         return {
             'address': self.address,
             'postal_code': self.postal_code,
             'city': self.city,
             'state_code': self.state_code,
             'timezone': self.timezone,
             'latitude': self.latitude,
             'longitude': self.longitude
         }
 
     @staticmethod
-    def from_json(json_venue):
+    def from_json(json_venue: Dict[str, Any]) -> 'Venue':
         """Returns a `Venue` object from JSON"""
-        v = Venue()
-        v.id = json_venue.get('id')
-        v.name = json_venue.get('name')
-        v.url = json_venue.get('url')
-        v.postal_code = json_venue.get('postalCode')
-        v.timezone = json_venue.get('timezone')
-        v.address = json_venue['address'].get('line1')
-        v.city = json_venue['city'].get('name')
-        v.state_code = json_venue['state'].get('stateCode')
-        v.latitude = json_venue['location'].get('latitude')
-        v.longitude = json_venue['location'].get('longitude')
-        # Process additional attributes as before
+        v = Venue(
+            name=json_venue.get('name'),
+            venue_id=json_venue.get('id'),
+            url=json_venue.get('url'),
+            postal_code=json_venue.get('postalCode'),
+            timezone=json_venue.get('timezone'),
+            address=json_venue['address'].get('line1') if 'address' in json_venue else None,
+            city=json_venue['city'].get('name') if 'city' in json_venue else None,
+            state_code=json_venue['state'].get('stateCode') if 'state' in json_venue else None,
+            latitude=json_venue['location'].get('latitude') if 'location' in json_venue else None,
+            longitude=json_venue['location'].get('longitude') if 'location' in json_venue else None,
+            # Process additional attributes as before
+        )
         _assign_links(v, json_venue)
         return v
 
-    async def fetch_additional_details(self, api_client):
+    async def fetch_additional_details(self, api_client) -> None:
         """Asynchronously fetch additional venue details.
         
         Args:
             api_client: Instance of an asynchronous API client.
         """
-        # Example URL construction, adjust based on your API's design
         details_url = self.links.get('self', '')  # Assuming 'self' link is detailed info
         if details_url:
             additional_details = await api_client.get(details_url)
             # Process and integrate additional_details into the Venue instance
-            print(additional_details)  # Placeholder for actual processing logic
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.name} at {self.address} in {self.city} {self.state_code}"
 
 class Attraction:
     """Attraction"""
-    def __init__(self, attraction_id=None, attraction_name=None, url=None,
-                 classifications=None, images=None, test=None, links=None):
+    def __init__(self, attraction_id: str = None, attraction_name: str = None, url: str = None,
+                 classifications: List = None, images: List = None, test: bool = None, links: Dict[str, Any] = None):
         self.id = attraction_id
         self.name = attraction_name
         self.url = url
         self.classifications = classifications
         self.images = images
         self.test = test
         self.links = links
 
     @staticmethod
-    def from_json(json_obj):
+    def from_json(json_obj: Dict[str, Any]) -> 'Attraction':
         """Convert JSON object to `Attraction` object"""
-        att = Attraction()
-        att.id = json_obj.get('id')
-        att.name = json_obj.get('name')
-        att.url = json_obj.get('url')
-        att.test = json_obj.get('test', False)  # Assuming 'test' is a boolean field
-        att.images = json_obj.get('images', [])
-        classifications = json_obj.get('classifications', [])
-        att.classifications = [Classification.from_json(cl) for cl in classifications]
+        att = Attraction(
+            attraction_id=json_obj.get('id'),
+            attraction_name=json_obj.get('name'),
+            url=json_obj.get('url'),
+            test=json_obj.get('test', False),  # Assuming 'test' is a boolean field
+            images=json_obj.get('images', []),
+            classifications=[Classification.from_json(cl) for cl in json_obj.get('classifications', [])]
+        )
         _assign_links(att, json_obj)
         return att
 
-    async def fetch_additional_details(self, api_client):
+    async def fetch_additional_details(self, api_client) -> None:
         """Asynchronously fetch additional details for the attraction.
         
         Args:
             api_client: Instance of an asynchronous API client capable of making GET requests.
         """
         details_url = self.links.get('self', '')  # Example, adjust based on actual API design
         if details_url:
             async with api_client.session.get(details_url) as response:
                 details_json = await response.json()
                 # Here you would process the details_json to extract and integrate additional details
-                print(details_json)  # Placeholder for actual logic
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name if self.name is not None else 'Unknown'
 
-
 class Classification:
     """Classification object (segment/genre/sub-genre)"""
-    def __init__(self, segment=None, classification_type=None, subtype=None, primary=None, links=None):
+    def __init__(self, segment: 'Segment' = None, classification_type: 'ClassificationType' = None,
+                 subtype: 'ClassificationSubType' = None, primary: bool = None, links: Dict[str, Any] = None):
         self.segment = segment
         self.type = classification_type
         self.subtype = subtype
         self.primary = primary
         self.links = links
 
     @staticmethod
-    def from_json(json_obj):
-        cl = Classification()
-        cl.primary = json_obj.get('primary')
-
-        if 'segment' in json_obj:
-            cl.segment = Segment.from_json(json_obj['segment'])
-
-        if 'type' in json_obj:
-            cl.type = ClassificationType(json_obj['type']['id'], json_obj['type']['name'])
-
-        if 'subType' in json_obj:
-            cl.subtype = ClassificationSubType(json_obj['subType']['id'], json_obj['subType']['name'])
-
+    def from_json(json_obj: Dict[str, Any]) -> 'Classification':
+        cl = Classification(
+            primary=json_obj.get('primary'),
+            segment=Segment.from_json(json_obj['segment']) if 'segment' in json_obj else None,
+            classification_type=ClassificationType.from_json(json_obj['type']) if 'type' in json_obj else None,
+            subtype=ClassificationSubType.from_json(json_obj['subType']) if 'subType' in json_obj else None
+        )
         _assign_links(cl, json_obj)
         return cl
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.type)
 
-    # Hypothetical async method to fetch additional details
-    async def fetch_additional_details(self, api_client):
+    async def fetch_additional_details(self, api_client) -> None:
         """Asynchronously fetch additional classification details."""
-        # This method is hypothetical and assumes there's a relevant URL in self.links
         details_url = self.links.get('details')  # Assuming 'details' is a key in links
         if details_url:
             async with api_client.session.get(details_url) as response:
                 details_json = await response.json()
                 # Process details_json as needed
 
 class EventClassification:
     """Classification as it's represented in event search results"""
-    def __init__(self, genre=None, subgenre=None, segment=None, classification_type=None, classification_subtype=None, primary=None, links=None):
+    def __init__(self, genre: 'Genre' = None, subgenre: 'SubGenre' = None, segment: 'Segment' = None,
+                 classification_type: 'ClassificationType' = None, classification_subtype: 'ClassificationSubType' = None,
+                 primary: bool = None, links: Dict[str, Any] = None):
         self.genre = genre
         self.subgenre = subgenre
         self.segment = segment
         self.type = classification_type
         self.subtype = classification_subtype
         self.primary = primary
         self.links = links
 
     @staticmethod
-    def from_json(json_obj):
-        ec = EventClassification()
-        ec.primary = json_obj.get('primary')
-
-        if 'segment' in json_obj:
-            ec.segment = Segment.from_json(json_obj['segment'])
-
-        if 'genre' in json_obj:
-            ec.genre = Genre.from_json(json_obj['genre'])
-
-        if 'subGenre' in json_obj:
-            ec.subgenre = SubGenre.from_json(json_obj['subGenre'])
-
-        if 'type' in json_obj:
-            ec.type = ClassificationType(json_obj['type']['id'], json_obj['type']['name'])
-
-        if 'subType' in json_obj:
-            ec.subtype = ClassificationSubType(json_obj['subType']['id'], json_obj['subType']['name'])
-
+    def from_json(json_obj: Dict[str, Any]) -> 'EventClassification':
+        ec = EventClassification(
+            primary=json_obj.get('primary'),
+            segment=Segment.from_json(json_obj['segment']) if 'segment' in json_obj else None,
+            genre=Genre.from_json(json_obj['genre']) if 'genre' in json_obj else None,
+            subgenre=SubGenre.from_json(json_obj['subGenre']) if 'subGenre' in json_obj else None,
+            classification_type=ClassificationType.from_json(json_obj['type']) if 'type' in json_obj else None,
+            classification_subtype=ClassificationSubType.from_json(json_obj['subType']) if 'subType' in json_obj else None
+        )
         _assign_links(ec, json_obj)
         return ec
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Segment: {self.segment} / Genre: {self.genre} / Subgenre: {self.subgenre} / Type: {self.type} / Subtype: {self.subtype}"
 
-
 class ClassificationType:
-    def __init__(self, type_id=None, type_name=None, subtypes=None):
+    def __init__(self, type_id: str = None, type_name: str = None, subtypes: List['ClassificationSubType'] = None):
         self.id = type_id
         self.name = type_name
         self.subtypes = subtypes
 
-    def __str__(self):
-        return self.name if self.name is not None else 'Unknown'
+    @staticmethod
+    def from_json(json_obj: Dict[str, Any]) -> 'ClassificationType':
+        return ClassificationType(
+            type_id=json_obj.get('id'),
+            type_name=json_obj.get('name')
+        )
 
-# No changes needed here unless dynamic fetching of subtype details becomes necessary
+    def __str__(self) -> str:
+        return self.name if self.name is not None else 'Unknown'
 
 class ClassificationSubType:
-    def __init__(self, type_id=None, type_name=None):
+    def __init__(self, type_id: str = None, type_name: str = None):
         self.id = type_id
         self.name = type_name
 
-    def __str__(self):
-        return self.name if self.name is not None else 'Unknown'
+    @staticmethod
+    def from_json(json_obj: Dict[str, Any]) -> 'ClassificationSubType':
+        return ClassificationSubType(
+            type_id=json_obj.get('id'),
+            type_name=json_obj.get('name')
+        )
 
-# Similar to ClassificationType, asynchronous behavior might be added for dynamic data fetching
+    def __str__(self) -> str:
+        return self.name if self.name is not None else 'Unknown'
 
 class Segment:
-    def __init__(self, segment_id=None, segment_name=None, genres=None, links=None):
+    def __init__(self, segment_id: str = None, segment_name: str = None, genres: List['Genre'] = None, links: Dict[str, Any] = None):
         self.id = segment_id
         self.name = segment_name
-        self.genres = genres  # Could be a list of Genre instances
+        self.genres = genres
         self.links = links
 
     @staticmethod
-    def from_json(json_obj):
-        seg = Segment()
-        seg.id = json_obj['id']
-        seg.name = json_obj.get('name')
-        # Processing embedded genres if available
-        if '_embedded' in json_obj:
-            genres = json_obj['_embedded'].get('genres', [])
-            seg.genres = [Genre.from_json(g) for g in genres]
+    def from_json(json_obj: Dict[str, Any]) -> 'Segment':
+        seg = Segment(
+            segment_id=json_obj.get('id'),
+            segment_name=json_obj.get('name'),
+            genres=[Genre.from_json(g) for g in json_obj.get('_embedded', {}).get('genres', [])]
+        )
         _assign_links(seg, json_obj)
         return seg
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name if self.name is not None else 'Unknown'
 
-# Could integrate asynchronous methods if genres require fetching additional details
-
 class Genre:
-    def __init__(self, genre_id=None, genre_name=None, subgenres=None, links=None):
+    def __init__(self, genre_id: str = None, genre_name: str = None, subgenres: List['SubGenre'] = None, links: Dict[str, Any] = None):
         self.id = genre_id
         self.name = genre_name
-        self.subgenres = subgenres  # Could be a list of SubGenre instances
+        self.subgenres = subgenres
         self.links = links
 
     @staticmethod
-    def from_json(json_obj):
-        g = Genre()
-        g.id = json_obj.get('id')
-        g.name = json_obj.get('name')
-        if '_embedded' in json_obj:
-            subgenres = json_obj['_embedded'].get('subgenres', [])
-            g.subgenres = [SubGenre.from_json(sg) for sg in subgenres]
-        _assign_links(g, json_obj)
-        return g
+    def from_json(json_obj: Dict[str, Any]) -> 'Genre':
+        return Genre(
+            genre_id=json_obj.get('id'),
+            genre_name=json_obj.get('name'),
+            subgenres=[SubGenre.from_json(sg) for sg in json_obj.get('_embedded', {}).get('subgenres', [])]
+        )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name if self.name is not None else 'Unknown'
 
-# Asynchronous enhancements could be added for dynamic subgenre data fetching
-
 class SubGenre:
-    def __init__(self, subgenre_id=None, subgenre_name=None, links=None):
+    def __init__(self, subgenre_id: str = None, subgenre_name: str = None, links: Dict[str, Any] = None):
         self.id = subgenre_id
         self.name = subgenre_name
         self.links = links
 
     @staticmethod
-    def from_json(json_obj):
-        sg = SubGenre()
-        sg.id = json_obj['id']
-        sg.name = json_obj['name']
-        _assign_links(sg, json_obj)
-        return sg
+    def from_json(json_obj: Dict[str, Any]) -> 'SubGenre':
+        return SubGenre(
+            subgenre_id=json_obj.get('id'),
+            subgenre_name=json_obj.get('name')
+        )
 
-    def __str__(self):
-        return self.name if self.name is not None else 'Unknown'
+    def __str__(self) -> str:
+        return self.name if self name is not None else 'Unknown'
 
 # Example async usage to fetch and process event details
 async def main():
     event = Event.from_json({'id': '123', 'name': 'Sample Event', 'links': {'self': 'http://example.com/event/123'}})
     await event.fetch_additional_details()
 
 if __name__ == '__main__':
```

### Comparing `tmticket-0.2.2/tmticket/query.py` & `tmticket-0.2.3/pytmtickets/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Classes to handle API queries/searches"""
-import aiohttp
+import logging
+from typing import Any, Dict, Optional
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
@@ -30,105 +33,82 @@
         'page': 'page',
         'size': 'size',
         'locale': 'locale',
         'latlong': 'latlong',
         'radius': 'radius'
     }
 
-    def __init__(self, api_client, method, model):
+    def __init__(self, api_client, method: str, model: Any):
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
+    async def _get(self, **kwargs: Any) -> Dict[str, Any]:
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
+            return await response.json()
 
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
-        return await self._get(**kwargs)
+    async def find(self, **kwargs: Any) -> Any:
+        response = await self._get(**kwargs)
+        return [Attraction.from_json(attraction) for attraction in response.get('_embedded', {}).get('attractions', [])]
 
 class ClassificationQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'classifications', Classification)
 
-
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
-                if genre.id == genre_id:
-                    genre = genre
-        return genre
-
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
+    async def find(self, **kwargs: Any) -> Any:
+        response = await self._get(**kwargs)
+        return [Classification.from_json(classification) for classification in response.get('_embedded', {}).get('classifications', [])]
+
+    async def segment_by_id(self, segment_id: str) -> Any:
+        """Return a `Segment` matching this ID"""
+        classification = await self.by_id(segment_id)
+        return classification.segment
+
+    async def genre_by_id(self, genre_id: str) -> Any:
+        """Return a `Genre` matching this ID"""
+        classification = await self.by_id(genre_id)
+        for genre in classification.segment.genres:
+            if genre.id == genre_id:
+                return genre
+        return None
+
+    async def subgenre_by_id(self, subgenre_id: str) -> Any:
+        """Return a `SubGenre` matching this ID"""
+        classification = await self.by_id(subgenre_id)
+        for genre in classification.segment.genres:
+            for subgenre in genre.subgenres:
+                if subgenre.id == subgenre_id:
+                    return subgenre
+        return None
 
 class EventQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'events', Event)
 
-    async def find(self, **kwargs):
-        return await self._get(**kwargs)
+    async def find(self, **kwargs: Any) -> Any:
+        response = await self._get(**kwargs)
+        return [Event.from_json(event) for event in response.get('_embedded', {}).get('events', [])]
 
 class VenueQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'venues', Venue)
 
-    async def find(self, **kwargs):
-        return await self._get(**kwargs)
+    async def find(self, **kwargs: Any) -> Any:
+        response = await self._get(**kwargs)
+        return [Venue.from_json(venue) for venue in response.get('_embedded', {}).get('venues', [])]
```


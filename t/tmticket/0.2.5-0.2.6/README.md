# Comparing `tmp/tmticket-0.2.5.tar.gz` & `tmp/tmticket-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.5.tar", last modified: Mon May 20 01:03:32 2024, max compression
+gzip compressed data, was "tmticket-0.2.6.tar", last modified: Mon May 20 01:28:04 2024, max compression
```

## Comparing `tmticket-0.2.5.tar` & `tmticket-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:03:32.675587 tmticket-0.2.5/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:03:32.674587 tmticket-0.2.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:03:32.671587 tmticket-0.2.5/pytmtickets/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.5/pytmtickets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4992 2024-05-20 01:01:30.000000 tmticket-0.2.5/pytmtickets/client.py
--rw-r--r--   0 root         (0) root         (0)    11787 2024-05-20 00:53:18.000000 tmticket-0.2.5/pytmtickets/model.py
--rw-r--r--   0 root         (0) root         (0)     4379 2024-05-20 01:01:42.000000 tmticket-0.2.5/pytmtickets/query.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 01:03:32.675587 tmticket-0.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 01:03:11.000000 tmticket-0.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:03:32.674587 tmticket-0.2.5/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:28:04.456364 tmticket-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:28:04.455364 tmticket-0.2.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:28:04.452364 tmticket-0.2.6/pytmtickets/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.6/pytmtickets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2024-05-20 01:01:30.000000 tmticket-0.2.6/pytmtickets/client.py
+-rw-r--r--   0 root         (0) root         (0)    12153 2024-05-20 01:27:31.000000 tmticket-0.2.6/pytmtickets/model.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2024-05-20 01:01:42.000000 tmticket-0.2.6/pytmtickets/query.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 01:28:04.456364 tmticket-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 01:27:40.000000 tmticket-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:28:04.455364 tmticket-0.2.6/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:28:03.000000 tmticket-0.2.6/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 01:28:04.000000 tmticket-0.2.6/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 01:28:03.000000 tmticket-0.2.6/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 01:28:03.000000 tmticket-0.2.6/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 01:28:03.000000 tmticket-0.2.6/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.5/pytmtickets/client.py` & `tmticket-0.2.6/pytmtickets/client.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.5/pytmtickets/model.py` & `tmticket-0.2.6/pytmtickets/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,44 +33,56 @@
         pg.total_pages = json_obj['page']['totalPages']
         pg.total_elements = json_obj['page']['totalElements']
         _assign_links(pg, json_obj)
         return pg
 
 class Event:
     """Ticketmaster event"""
-    def __init__(self, event_id: str = None, name: str = None, start_date: str = None, start_time: str = None,
-                 status: str = None, classifications: List[Any] = None, links: Dict[str, Any] = None):
+    def __init__(self, event_id=None, name=None, start_date=None, start_time=None, status=None, classifications=None, links=None):
         self.id = event_id
         self.name = name
         self.start_date = start_date
         self.start_time = start_time
         self.status = status
         self.classifications = classifications
         self.links = links
 
     @staticmethod
-    def from_json(json_event: Dict[str, Any]) -> 'Event':
+    def from_json(json_event):
         """Creates an `Event` from API's JSON response"""
         e = Event(
             event_id=json_event.get('id'),
             name=json_event.get('name'),
             start_date=json_event.get('dates', {}).get('start', {}).get('localDate'),
             start_time=json_event.get('dates', {}).get('start', {}).get('localTime'),
             status=json_event.get('dates', {}).get('status', {}).get('code'),
             classifications=[Classification.from_json(cl) for cl in json_event.get('classifications', [])]
         )
         _assign_links(e, json_event)
         return e
 
-    async def fetch_additional_details(self, api_client) -> None:
-        """Asynchronously fetch additional event details"""
-        if 'self' in self.links:
-            details_url = self.links['self']
-            additional_details = await api_client.get_url(details_url)
-            # Process and update event instance with additional details
+    def to_dict(self):
+        """Convert the Event object to a dictionary for serialization"""
+        return {
+            'id': self.id,
+            'name': self.name,
+            'start_date': self.start_date,
+            'start_time': self.start_time,
+            'status': self.status,
+            'classifications': [cl.to_dict() for cl in self.classifications] if self.classifications else [],
+            'links': self.links,
+        }
+
+    async def fetch_additional_details(self):
+        """Asynchronously fetch additional event details (hypothetical example)"""
+        async with aiohttp.ClientSession() as session:
+            async with session.get(self.links['self']) as response:
+                details = await response.json()
+                # Process and update event instance with additional details
+
 
 class Venue:
     """A Ticketmaster venue."""
     def __init__(self, name: str = None, address: str = None, city: str = None, state_code: str = None,
                  postal_code: str = None, latitude: float = None, longitude: float = None,
                  markets: List[Any] = None, url: str = None, box_office_info: Dict[str, Any] = None,
                  dmas: List[Any] = None, general_info: Dict[str, Any] = None, venue_id: str = None,
```

### Comparing `tmticket-0.2.5/pytmtickets/query.py` & `tmticket-0.2.6/pytmtickets/query.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.5/setup.py` & `tmticket-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.2.5',
+    version='0.2.6',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
 #    long_description=read('README.rst'),
     license='MIT',
     keywords='Ticketmaster',
     url='https://github.com/hokiebrian/pytmtickets',
```


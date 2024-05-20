# Comparing `tmp/tmticket-0.2.4.tar.gz` & `tmp/tmticket-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.4.tar", last modified: Mon May 20 00:54:36 2024, max compression
+gzip compressed data, was "tmticket-0.2.5.tar", last modified: Mon May 20 01:03:32 2024, max compression
```

## Comparing `tmticket-0.2.4.tar` & `tmticket-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:54:36.969733 tmticket-0.2.4/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 00:54:36.968733 tmticket-0.2.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:54:36.965733 tmticket-0.2.4/pytmtickets/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.4/pytmtickets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5000 2024-05-20 00:44:04.000000 tmticket-0.2.4/pytmtickets/client.py
--rw-r--r--   0 root         (0) root         (0)    11787 2024-05-20 00:53:18.000000 tmticket-0.2.4/pytmtickets/model.py
--rw-r--r--   0 root         (0) root         (0)     4387 2024-05-20 00:42:28.000000 tmticket-0.2.4/pytmtickets/query.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 00:54:36.969733 tmticket-0.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 00:46:58.000000 tmticket-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 00:54:36.967733 tmticket-0.2.4/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 00:54:36.000000 tmticket-0.2.4/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:03:32.675587 tmticket-0.2.5/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:03:32.674587 tmticket-0.2.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:03:32.671587 tmticket-0.2.5/pytmtickets/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 00:42:11.000000 tmticket-0.2.5/pytmtickets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2024-05-20 01:01:30.000000 tmticket-0.2.5/pytmtickets/client.py
+-rw-r--r--   0 root         (0) root         (0)    11787 2024-05-20 00:53:18.000000 tmticket-0.2.5/pytmtickets/model.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2024-05-20 01:01:42.000000 tmticket-0.2.5/pytmtickets/query.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 01:03:32.675587 tmticket-0.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-20 01:03:11.000000 tmticket-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 01:03:32.674587 tmticket-0.2.5/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-20 01:03:32.000000 tmticket-0.2.5/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.4/pytmtickets/client.py` & `tmticket-0.2.5/pytmtickets/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """API client classes"""
 import aiohttp
 import logging
 from typing import Any, Dict, Optional
-from tmticket.query import AttractionQuery, ClassificationQuery, EventQuery, VenueQuery
+from .query import AttractionQuery, ClassificationQuery, EventQuery, VenueQuery
 
 log = logging.getLogger(__name__)
 
 class AsyncApiClient:
     """AsyncApiClient is the main wrapper for the Discovery API, updated for asynchronous operation."""
 
     root_url = 'https://app.ticketmaster.com'
```

### Comparing `tmticket-0.2.4/pytmtickets/model.py` & `tmticket-0.2.5/pytmtickets/model.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.4/pytmtickets/query.py` & `tmticket-0.2.5/pytmtickets/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Classes to handle API queries/searches"""
 import logging
 from typing import Any, Dict, List, Type, Optional
-from tmticket.model import Venue, Event, Attraction, Classification
+from .model import Venue, Event, Attraction, Classification
 
 log = logging.getLogger(__name__)
 
 class BaseQuery:
     """Base query/parent class for specific search types."""
     attr_map = {
         'start_date_time': 'startDateTime',
```

### Comparing `tmticket-0.2.4/setup.py` & `tmticket-0.2.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.2.4',
+    version='0.2.5',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
 #    long_description=read('README.rst'),
     license='MIT',
     keywords='Ticketmaster',
     url='https://github.com/hokiebrian/pytmtickets',
```


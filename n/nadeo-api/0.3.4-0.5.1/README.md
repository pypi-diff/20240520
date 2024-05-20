# Comparing `tmp/nadeo_api-0.3.4.tar.gz` & `tmp/nadeo_api-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadeo_api-0.3.4.tar", last modified: Sun May 19 19:39:14 2024, max compression
+gzip compressed data, was "nadeo_api-0.5.1.tar", last modified: Mon May 20 07:31:53 2024, max compression
```

## Comparing `nadeo_api-0.3.4.tar` & `nadeo_api-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:39:14.118641 nadeo_api-0.3.4/
--rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3675 2024-05-19 19:39:14.118641 nadeo_api-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1695 2024-05-19 19:37:19.000000 nadeo_api-0.3.4/README.md
--rw-rw-rw-   0        0        0      779 2024-05-19 19:38:43.000000 nadeo_api-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-19 19:39:14.119640 nadeo_api-0.3.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-19 19:39:14.087591 nadeo_api-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 19:39:14.102105 nadeo_api-0.3.4/src/nadeo_api/
--rw-rw-rw-   0        0        0     1442 2024-05-19 19:37:37.000000 nadeo_api-0.3.4/src/nadeo_api/__init__.py
--rw-rw-rw-   0        0        0    10109 2024-05-16 23:12:13.000000 nadeo_api-0.3.4/src/nadeo_api/auth.py
--rw-rw-rw-   0        0        0     2053 2024-05-19 19:33:14.000000 nadeo_api-0.3.4/src/nadeo_api/core.py
--rw-rw-rw-   0        0        0     2855 2024-05-18 07:08:54.000000 nadeo_api-0.3.4/src/nadeo_api/live.py
--rw-rw-rw-   0        0        0     1334 2024-05-18 07:08:43.000000 nadeo_api-0.3.4/src/nadeo_api/meet.py
--rw-rw-rw-   0        0        0     2902 2024-05-18 07:08:29.000000 nadeo_api-0.3.4/src/nadeo_api/oauth.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:39:14.117642 nadeo_api-0.3.4/src/nadeo_api.egg-info/
--rw-rw-rw-   0        0        0     3675 2024-05-19 19:39:14.000000 nadeo_api-0.3.4/src/nadeo_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-19 19:39:14.000000 nadeo_api-0.3.4/src/nadeo_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:39:14.000000 nadeo_api-0.3.4/src/nadeo_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 19:39:14.000000 nadeo_api-0.3.4/src/nadeo_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-19 19:39:14.000000 nadeo_api-0.3.4/src/nadeo_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-19 19:39:14.116642 nadeo_api-0.3.4/tests/
--rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.3.4/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:31:53.543398 nadeo_api-0.5.1/
+-rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       16 2024-05-20 07:29:47.000000 nadeo_api-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3735 2024-05-20 07:31:53.542398 nadeo_api-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2024-05-20 06:35:02.000000 nadeo_api-0.5.1/README.md
+-rw-rw-rw-   0        0        0      779 2024-05-20 07:30:27.000000 nadeo_api-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:31:53.543398 nadeo_api-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 07:31:53.503090 nadeo_api-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 07:31:53.528934 nadeo_api-0.5.1/src/nadeo_api/
+-rw-rw-rw-   0        0        0      306 2024-05-20 07:30:32.000000 nadeo_api-0.5.1/src/nadeo_api/__init__.py
+-rw-rw-rw-   0        0        0    10139 2024-05-19 20:49:09.000000 nadeo_api-0.5.1/src/nadeo_api/auth.py
+-rw-rw-rw-   0        0        0     3846 2024-05-20 06:36:35.000000 nadeo_api-0.5.1/src/nadeo_api/core.py
+-rw-rw-rw-   0        0        0     2855 2024-05-18 07:08:54.000000 nadeo_api-0.5.1/src/nadeo_api/live.py
+-rw-rw-rw-   0        0        0     1334 2024-05-18 07:08:43.000000 nadeo_api-0.5.1/src/nadeo_api/meet.py
+-rw-rw-rw-   0        0        0     2902 2024-05-18 07:08:29.000000 nadeo_api-0.5.1/src/nadeo_api/oauth.py
+-rw-rw-rw-   0        0        0     1693 2024-05-20 06:47:56.000000 nadeo_api-0.5.1/src/nadeo_api/util.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:31:53.541398 nadeo_api-0.5.1/src/nadeo_api.egg-info/
+-rw-rw-rw-   0        0        0     3735 2024-05-20 07:31:53.000000 nadeo_api-0.5.1/src/nadeo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-20 07:31:53.000000 nadeo_api-0.5.1/src/nadeo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:31:53.000000 nadeo_api-0.5.1/src/nadeo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 07:31:53.000000 nadeo_api-0.5.1/src/nadeo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-20 07:31:53.000000 nadeo_api-0.5.1/src/nadeo_api.egg-info/top_level.txt
```

### Comparing `nadeo_api-0.3.4/LICENSE.txt` & `nadeo_api-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/PKG-INFO` & `nadeo_api-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.3.4
+Version: 0.5.1
 Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,14 +56,15 @@
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
 ```py
-import nadeo_api        # main module - has some functions not related to endpoints
+import nadeo_api        # main module - functions not related to endpoints
 import nadeo_api.auth   # authentication - required for any endpoint
 import nadeo_api.core   # web services Core endpoints
 import nadeo_api.live   # web services Live endpoints
 import nadeo_api.meet   # web services Meet endpoints
 import nadeo_api.oauth  # OAuth2 endpoints (public API)
+import nadeo_api.util   # unnecessary - use the main module instead
 ```
```

### Comparing `nadeo_api-0.3.4/README.md` & `nadeo_api-0.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
 ```py
-import nadeo_api        # main module - has some functions not related to endpoints
+import nadeo_api        # main module - functions not related to endpoints
 import nadeo_api.auth   # authentication - required for any endpoint
 import nadeo_api.core   # web services Core endpoints
 import nadeo_api.live   # web services Live endpoints
 import nadeo_api.meet   # web services Meet endpoints
 import nadeo_api.oauth  # OAuth2 endpoints (public API)
+import nadeo_api.util   # unnecessary - use the main module instead
 ```
```

### Comparing `nadeo_api-0.3.4/src/nadeo_api/auth.py` & `nadeo_api-0.5.1/src/nadeo_api/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-07
-| Modified: 2024-05-16
+| Modified: 2024-05-19
 
 - Functions for interacting with authentication tokens to use with the API
 - Also contains variables and functions intended for internal use
 '''
 
 from base64 import b64encode, urlsafe_b64decode
 from dataclasses import dataclass
@@ -220,15 +220,15 @@
     agent: str
         - user agent with your program's name and a way to contact you
         - Ubisoft can block your request without this being properly set
         - not required for OAuth2
         - default: `''` (empty)
 
     server_account: bool
-        - whether you're using a dedicated server account instead of a Ubisoft account
+        - whether you're using a dedicated server account (Server usage) instead of a Ubisoft account (Client usage)
         - ignored when using OAuth2
         - default: `False`
     '''
 
     aud_lower: str = audience.lower()
 
     if aud_lower in ('nadeoservices', 'core', 'prod'):
```

### Comparing `nadeo_api-0.3.4/src/nadeo_api/core.py` & `nadeo_api-0.5.1/src/nadeo_api/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-14
-| Modified: 2024-05-18
+| Modified: 2024-05-20
 
 - Functions for interacting with the web services Core API
 '''
 
 from . import auth
+from . import util
 
 
 def get(token: auth.Token, endpoint: str, params: dict = {}) -> dict:
     '''
     - sends a GET request to the Core API
 
     Parameters
@@ -61,14 +62,78 @@
 
     if usage not in ('Client', 'Server'):
         raise ValueError(f'Given usage is invalid: {usage}')
 
     return get(token, 'api/routes', {'usage': usage})
 
 
+def trophies_history(token: auth.Token, account_id: str, count: int, offset: int = 0) -> dict:
+    '''
+    - gets a list of trophy gain history
+    - requires a Ubisoft account (client usage)
+
+    Parameters
+    ----------
+    token: auth.Token
+        - authentication token gotten from `auth.get_token`
+
+    account_id: str
+        - account ID to get data for
+
+    count: int
+        - number of history entries to get
+        - if you set this too high, the request may time out (response 504)
+
+    offset: int
+        - number of history entries to skip, looking backwards from the most recent
+        - default: 0
+
+    Returns
+    -------
+    dict
+        - history entries sorted newest to oldest
+    '''
+
+    if not util.valid_uuid(account_id):
+        raise ValueError(f'Given account ID is invalid: {account_id}')
+
+    if token.server_account:
+        raise ValueError('This endpoint requires a Ubisoft account (client usage)')
+
+    return get(token, f'accounts/{account_id}/trophies', {'offset': offset, 'count': count})
+
+
+def trophies_last_year_summary(token: auth.Token, account_id: str) -> dict:
+    '''
+    - gets a summary of the trophies gained in the last year
+    - requires a Ubisoft account (client usage)
+
+    Parameters
+    ----------
+    token: auth.Token
+        - authentication token gotten from `auth.get_token`
+
+    account_id: str
+        - account ID to get data for
+
+    Returns
+    -------
+    dict
+        - data on given account
+    '''
+
+    if not util.valid_uuid(account_id):
+        raise ValueError(f'Given account ID is invalid: {account_id}')
+
+    if token.server_account:
+        raise ValueError('This endpoint requires a Ubisoft account (client usage)')
+
+    return get(token, f'accounts/{account_id}/trophies/lastYearSummary')
+
+
 def zones(token: auth.Token) -> dict:
     '''
     - gets the valid regions a player may choose from
     - https://webservices.openplanet.dev/core/meta/zones
 
     Parameters
     ----------
```

### Comparing `nadeo_api-0.3.4/src/nadeo_api/live.py` & `nadeo_api-0.5.1/src/nadeo_api/live.py`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/src/nadeo_api/meet.py` & `nadeo_api-0.5.1/src/nadeo_api/meet.py`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/src/nadeo_api/oauth.py` & `nadeo_api-0.5.1/src/nadeo_api/oauth.py`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/src/nadeo_api.egg-info/PKG-INFO` & `nadeo_api-0.5.1/src/nadeo_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.3.4
+Version: 0.5.1
 Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,14 +56,15 @@
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
 ```py
-import nadeo_api        # main module - has some functions not related to endpoints
+import nadeo_api        # main module - functions not related to endpoints
 import nadeo_api.auth   # authentication - required for any endpoint
 import nadeo_api.core   # web services Core endpoints
 import nadeo_api.live   # web services Live endpoints
 import nadeo_api.meet   # web services Meet endpoints
 import nadeo_api.oauth  # OAuth2 endpoints (public API)
+import nadeo_api.util   # unnecessary - use the main module instead
 ```
```


# Comparing `tmp/nadeo_api-0.3.4.tar.gz` & `tmp/nadeo_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadeo_api-0.3.4.tar", last modified: Sun May 19 19:39:14 2024, max compression
+gzip compressed data, was "nadeo_api-0.4.0.tar", last modified: Sun May 19 21:04:23 2024, max compression
```

## Comparing `nadeo_api-0.3.4.tar` & `nadeo_api-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
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
+drwxrwxrwx   0        0        0        0 2024-05-19 21:04:23.413730 nadeo_api-0.4.0/
+-rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3675 2024-05-19 21:04:23.412731 nadeo_api-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1695 2024-05-19 19:37:19.000000 nadeo_api-0.4.0/README.md
+-rw-rw-rw-   0        0        0      779 2024-05-19 21:03:58.000000 nadeo_api-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 21:04:23.413730 nadeo_api-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 21:04:23.364375 nadeo_api-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 21:04:23.390529 nadeo_api-0.4.0/src/nadeo_api/
+-rw-rw-rw-   0        0        0     1439 2024-05-19 21:03:53.000000 nadeo_api-0.4.0/src/nadeo_api/__init__.py
+-rw-rw-rw-   0        0        0    10139 2024-05-19 20:49:09.000000 nadeo_api-0.4.0/src/nadeo_api/auth.py
+-rw-rw-rw-   0        0        0     3603 2024-05-19 20:52:26.000000 nadeo_api-0.4.0/src/nadeo_api/core.py
+-rw-rw-rw-   0        0        0     2855 2024-05-18 07:08:54.000000 nadeo_api-0.4.0/src/nadeo_api/live.py
+-rw-rw-rw-   0        0        0     1334 2024-05-18 07:08:43.000000 nadeo_api-0.4.0/src/nadeo_api/meet.py
+-rw-rw-rw-   0        0        0     2902 2024-05-18 07:08:29.000000 nadeo_api-0.4.0/src/nadeo_api/oauth.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:04:23.411730 nadeo_api-0.4.0/src/nadeo_api.egg-info/
+-rw-rw-rw-   0        0        0     3675 2024-05-19 21:04:23.000000 nadeo_api-0.4.0/src/nadeo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-19 21:04:23.000000 nadeo_api-0.4.0/src/nadeo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 21:04:23.000000 nadeo_api-0.4.0/src/nadeo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 21:04:23.000000 nadeo_api-0.4.0/src/nadeo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 21:04:23.000000 nadeo_api-0.4.0/src/nadeo_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 21:04:23.410732 nadeo_api-0.4.0/tests/
+-rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.4.0/tests/test_auth.py
+-rw-rw-rw-   0        0        0     1230 2024-05-19 20:52:35.000000 nadeo_api-0.4.0/tests/test_core.py
```

### Comparing `nadeo_api-0.3.4/LICENSE.txt` & `nadeo_api-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/PKG-INFO` & `nadeo_api-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.3.4
+Version: 0.4.0
 Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nadeo_api-0.3.4/README.md` & `nadeo_api-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/src/nadeo_api/__init__.py` & `nadeo_api-0.4.0/src/nadeo_api/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,52 +7,52 @@
 - This is the main module - most of what you need is in sub-modules.
 '''
 
 import base64
 import re
 
 
-__version__: tuple = 0, 3, 4
+__version__: tuple = 0, 4.0
 
 
 def account_id_from_login(account_login: str) -> str:
     '''
-    - converts a base64-encoded login to an Ubisoft account ID (UUID)
+    - converts a base64-encoded login to a Ubisoft account ID (UUID)
 
     Parameters
     ----------
     account_login: str
         - base64-encoded login
 
     Returns
     -------
     str
         - account ID
     '''
 
-    if not bool(re.match('^[a-zA-Z0-9\\-_]{22}$', account_login)):
+    if not bool(re.match('^[0-9A-Za-z\\-_]{22}$', account_login)):
         raise ValueError(f'Given account login is invalid: {account_login}')
 
     b: str = bytes.hex(base64.urlsafe_b64decode(f'{account_login}=='))
 
     return f'{b[:8]}-{b[8:12]}-{b[12:16]}-{b[16:20]}-{b[20:]}'
 
 
 def account_login_from_id(account_id: str) -> str:
     '''
-    - converts an Ubisoft account ID (UUID) to a base64-encoded login
+    - converts a Ubisoft account ID (UUID) to a base64-encoded login
 
     Parameters
     ----------
     account_id: str
         - account ID (UUID)
 
     Returns
     -------
     str
         - base64-encoded login
     '''
 
-    if not bool(re.match('^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$', account_id)):
+    if not bool(re.match('^[0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{12}$', account_id)):
         raise ValueError(f'Given account ID is not a valid UUID: {account_id}')
 
     return base64.urlsafe_b64encode(bytes.fromhex(account_id.replace('-', ''))).decode()[:-2]
```

### Comparing `nadeo_api-0.3.4/src/nadeo_api/auth.py` & `nadeo_api-0.4.0/src/nadeo_api/auth.py`

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

### Comparing `nadeo_api-0.3.4/src/nadeo_api/core.py` & `nadeo_api-0.4.0/src/nadeo_api/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-14
-| Modified: 2024-05-18
+| Modified: 2024-05-19
 
 - Functions for interacting with the web services Core API
 '''
 
 from . import auth
 
 
@@ -61,14 +61,72 @@
 
     if usage not in ('Client', 'Server'):
         raise ValueError(f'Given usage is invalid: {usage}')
 
     return get(token, 'api/routes', {'usage': usage})
 
 
+def trophies_history(token: auth.Token, account_id: str, count: int, offset: int = 0) -> dict:
+    '''
+    - gets a list of trophy gain history
+    - requires a Ubisoft account (Client usage)
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
+    if token.server_account:
+        raise ValueError('This endpoint requires a Ubisoft account (Client usage)')
+
+    return get(token, f'accounts/{account_id}/trophies', {'offset': offset, 'count': count})
+
+
+def trophies_last_year_summary(token: auth.Token, account_id: str) -> dict:
+    '''
+    - gets a summary of the trophies gained in the last year
+    - requires a Ubisoft account (Client usage)
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
+    if token.server_account:
+        raise ValueError('This endpoint requires a Ubisoft account (Client usage)')
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

### Comparing `nadeo_api-0.3.4/src/nadeo_api/live.py` & `nadeo_api-0.4.0/src/nadeo_api/live.py`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/src/nadeo_api/meet.py` & `nadeo_api-0.4.0/src/nadeo_api/meet.py`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/src/nadeo_api/oauth.py` & `nadeo_api-0.4.0/src/nadeo_api/oauth.py`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.4/src/nadeo_api.egg-info/PKG-INFO` & `nadeo_api-0.4.0/src/nadeo_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.3.4
+Version: 0.4.0
 Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


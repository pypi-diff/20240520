# Comparing `tmp/scratchcommunication-2.7.2.tar.gz` & `tmp/scratchcommunication-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.7.2.tar", last modified: Wed May  8 13:42:22 2024, max compression
+gzip compressed data, was "scratchcommunication-2.8.1.tar", last modified: Mon May 20 17:28:09 2024, max compression
```

## Comparing `scratchcommunication-2.7.2.tar` & `scratchcommunication-2.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.971186 scratchcommunication-2.7.2/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.123522 scratchcommunication-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-20 17:28:09.123522 scratchcommunication-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.119522 scratchcommunication-2.8.1/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.119522 scratchcommunication-2.8.1/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.123522 scratchcommunication-2.8.1/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 17:28:09.000000 scratchcommunication-2.8.1/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:28:09.123522 scratchcommunication-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:28:09.119522 scratchcommunication-2.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-20 17:28:05.000000 scratchcommunication-2.8.1/tests/test1.py
```

### Comparing `scratchcommunication-2.7.2/LICENSE` & `scratchcommunication-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.2/PKG-INFO` & `scratchcommunication-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.7.2
+Version: 2.8.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,14 +50,15 @@
 For this, you either need a session id or a password.
 
 ## Login using session id
 
 ```python
 import scratchcommunication
 session = scratchcommunication.Session("YOUR_USERNAME", session_id="YOUR_SESSIONID")
+# You can also supply your XToken if it cannot be found using xtoken="YOUR_XTOKEN
 ```
 
 If you log in using your session id, you may not need your to supply your username.
 
 ## Login using password
 
 ```python
```

### Comparing `scratchcommunication-2.7.2/README.md` & `scratchcommunication-2.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 For this, you either need a session id or a password.
 
 ## Login using session id
 
 ```python
 import scratchcommunication
 session = scratchcommunication.Session("YOUR_USERNAME", session_id="YOUR_SESSIONID")
+# You can also supply your XToken if it cannot be found using xtoken="YOUR_XTOKEN
 ```
 
 If you log in using your session id, you may not need your to supply your username.
 
 ## Login using password
 
 ```python
```

### Comparing `scratchcommunication-2.7.2/scratchcommunication/cloud.py` & `scratchcommunication-2.8.1/scratchcommunication/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
 
         def wrapper(func):
             if event in self.events:
                 eventlist = self.events[event]
             else:
                 eventlist = self.events[event] = []
             eventlist.append(func)
-            def dispatcher(data : dict = None, **entries):
+            def dispatcher(data : dict = None, /, **entries):
                 return self.emit_event(event, **data, **entries)
             return dispatcher
 
         return wrapper
 
 
 class TwCloudConnection(CloudConnection):
```

### Comparing `scratchcommunication-2.7.2/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.8.1/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.2/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.8.1/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.2/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.8.1/scratchcommunication/cloudrequests/requests.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.2/scratchcommunication/security.py` & `scratchcommunication-2.8.1/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.2/scratchcommunication/session.py` & `scratchcommunication-2.8.1/scratchcommunication/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,65 +18,71 @@
 CHROMIUM = 4
 EDGE_DEV = 5
 VIVALDI = 6
 ANY = 7
 
 class Session:
     __slots__ = ("session_id", "username", "headers", "cookies", "xtoken", "email", "id", "permissions", "flags", "banned", "session_data", "mute_status", "new_scratcher")
-    def __init__(self, username : str = None, *, session_id : str = None, _login : bool = False):
+    def __init__(self, username : str = None, *, session_id : str = None, xtoken : str = None, _login : bool = False):
         if not _login:
             return
         self.session_id = session_id
         self.username = username
         self.headers = headers
         self.cookies = {
             "scratchcsrftoken" : "a",
             "scratchlanguage" : "en",
             "scratchpolicyseen": "true",
             "scratchsessionsid" : self.session_id,
             "accept": "application/json",
             "Content-Type": "application/json",
         }
-        self._login()
+        self._login(xtoken=xtoken)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
 
     def logout(self):
         for attr in self.__slots__:
             delattr(self, attr)
 
-    def _login(self, *, _session : requests.Session = None):
+    def _login(self, *, xtoken : str = None, _session : requests.Session = None):
         '''
         Don't use this
         '''
         try:
             account = (_session or requests).post("https://scratch.mit.edu/session", headers=self.headers, cookies={
                 "scratchsessionsid": self.session_id,
                 "scratchcsrftoken": "a",
                 "scratchlanguage": "en",
             }).json()
-            self.xtoken = account["user"]["token"]
+            self.supply_xtoken(account["user"]["token"])
             self.username = account["user"]["username"]
-            self.headers["X-Token"] = self.xtoken
             self.email = account["user"]["email"]
             self.id = account["user"]["id"]
             self.permissions = account["permissions"]
             self.flags = account["flags"]
             self.banned = account["user"]["banned"]
             self.session_data = account
             self.new_scratcher = account["permissions"]["new_scratcher"]
             self.mute_status = account["permissions"]["mute_status"]
         except Exception:
             if self.username is None:
                 raise ValueError("No username supplied and there was none found. The username is needed.")
-            warnings.warn("Couldn't find token. Most features will probably still work.")
+            warnings.warn("Couldn't find XToken. Most features will probably still work.")
+            if xtoken:
+                self.supply_xtoken(xtoken)
+                warnings.warn("Got XToken from login data.")
+                
+    def supply_xtoken(self, xtoken):
+        self.xtoken = xtoken
+        self.headers["X-Token"] = xtoken
 
     @classmethod
     def from_browser(cls, browser : Literal[0,1,2,3,4,5,6,7]) -> Self:
         """
         Import cookies from browser to login
         """
         if not browsercookie:
```

### Comparing `scratchcommunication-2.7.2/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.8.1/scratchcommunication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.7.2
+Version: 2.8.1
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,14 +50,15 @@
 For this, you either need a session id or a password.
 
 ## Login using session id
 
 ```python
 import scratchcommunication
 session = scratchcommunication.Session("YOUR_USERNAME", session_id="YOUR_SESSIONID")
+# You can also supply your XToken if it cannot be found using xtoken="YOUR_XTOKEN
 ```
 
 If you log in using your session id, you may not need your to supply your username.
 
 ## Login using password
 
 ```python
```

### Comparing `scratchcommunication-2.7.2/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.8.1/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.2/setup.py` & `scratchcommunication-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.7.2'
+VERSION = '2.8.1'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.7.2/tests/test1.py` & `scratchcommunication-2.8.1/tests/test1.py`

 * *Files identical despite different names*


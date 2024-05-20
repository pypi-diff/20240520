# Comparing `tmp/buzz_client-1.0.3a0.tar.gz` & `tmp/buzz_client-1.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buzz_client-1.0.3a0.tar", max compression
+gzip compressed data, was "buzz_client-1.0.3b0.tar", max compression
```

## Comparing `buzz_client-1.0.3a0.tar` & `buzz_client-1.0.3b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2174 2024-05-16 13:37:23.631928 buzz_client-1.0.3a0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.0.3a0/buzz_client/__init__.py
--rwxr-xr-x   0        0        0     4172 2024-05-17 11:14:24.839316 buzz_client-1.0.3a0/buzz_client/cli.py
--rw-r--r--   0        0        0     2674 2024-05-17 10:30:15.232087 buzz_client-1.0.3a0/buzz_client/client.py
--rw-r--r--   0        0        0      452 2024-05-17 11:14:03.542636 buzz_client-1.0.3a0/pyproject.toml
--rw-r--r--   0        0        0     2821 1970-01-01 00:00:00.000000 buzz_client-1.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0     2174 2024-05-16 13:37:23.631928 buzz_client-1.0.3b0/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.0.3b0/buzz_client/__init__.py
+-rwxr-xr-x   0        0        0     4262 2024-05-20 13:31:49.929211 buzz_client-1.0.3b0/buzz_client/cli.py
+-rw-r--r--   0        0        0     2592 2024-05-20 13:55:38.284805 buzz_client-1.0.3b0/buzz_client/client.py
+-rw-r--r--   0        0        0      452 2024-05-20 13:55:28.866559 buzz_client-1.0.3b0/pyproject.toml
+-rw-r--r--   0        0        0     2821 1970-01-01 00:00:00.000000 buzz_client-1.0.3b0/PKG-INFO
```

### Comparing `buzz_client-1.0.3a0/README.md` & `buzz_client-1.0.3b0/README.md`

 * *Files identical despite different names*

### Comparing `buzz_client-1.0.3a0/buzz_client/cli.py` & `buzz_client-1.0.3b0/buzz_client/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,19 +42,19 @@
 from docopt import docopt
 from buzz_client.client import BuzzClient
 from scriptonite.configuration import Configuration
 from scriptonite.logging import Logger
 
 log = Logger(level="INFO")
 
-VERSION = "1.0.3a"
+VERSION = "1.0.3b"
 
 
 def shutdown(sig, frame):
-    print(f"\nAye, aye! See you...")
+    print("\nAye, aye! See you...")
     sys.exit(0)
 
 
 signal.signal(signal.SIGINT, shutdown)
 
 
 def banner(client):
@@ -86,15 +86,15 @@
     client_configuration.from_mapping(
         dict(api=arguments.get('--api'), token=arguments.get('--token')))
     client_configuration.from_environ(prefix="BUZZ")
 
     client = BuzzClient(client_configuration)
 
     if client.api is None or client.settings.token is None:
-        print(f"\n** Missing values for API URL or TOKEN")
+        print("\n** Missing values for API URL or TOKEN")
         sys.exit(2)
 
     # Check connection
     check = client.check()
     if not check.get('api_ok'):
         print(f"\nERROR: connection to '{client.api}' failed.\n")
         sys.exit(2)
@@ -116,25 +116,28 @@
 
     if arguments.send:
         if arguments.get('<body>'):
             body = [" ".join(arguments.get('<body>'))]  # type: ignore
         else:
             body = []
             for line in sys.stdin:
-                body.append(line.rstrip())
+                body.append(line)
+
+        if len(body) == 0:
+            print("ERROR: refusing to send an empty message\n")
+            sys.exit(2)
 
         r = client.send(notifier=arguments.get('<notifier>'),  # type: ignore
                         title=arguments.get('--title'),  # type: ignore
                         recipient=arguments.get(
             '--recipient'),  # type: ignore
-            body="\n".join(body),
+            body="".join(body),
             severity=arguments.get('--severity'),  # type: ignore
             attach=arguments.get('--attach')  # type: ignore
         )
-        print(
-            f"{r.json().get('detail')} [{r.status_code}]")
+        print(f"{r.json().get('detail')} [{r.status_code}]")
 
         sys.exit(int(not (r)))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `buzz_client-1.0.3a0/buzz_client/client.py` & `buzz_client-1.0.3b0/buzz_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from email.policy import HTTP
 from functools import cached_property
-import re
-from httpx import HTTPError
 import requests
 import logging
 from scriptonite.configuration import Configuration, yaml_load
 from scriptonite.utilities import dictObj
 from scriptonite.logging import Logger
 
 
@@ -27,24 +24,26 @@
         response = requests.get(f"{self.api}{endpoint}",
                                 headers=self.headers)
         return response
 
     def check(self):
         try:
             api_info = self.get('/')
-        except requests.exceptions.ConnectionError:
+        except BaseException as e:
+            print(e)
             return dict(api_ok=False, token_ok=False)
         if api_info.ok:
             api_path = api_info.json().get('api_path')
             token_check = self.get(f"{api_path}/check")
 
             if token_check.ok:
                 return dict(api_ok=True, token_ok=True)
             else:
                 return dict(api_ok=True, token_ok=False)
+        return dict(api_ok=False, token_ok=False)
 
     @cached_property
     def api_info(self) -> dict:
         return self.get('/').json()
 
     @cached_property
     def api_path(self) -> str | None:
@@ -54,15 +53,16 @@
     def api_version(self) -> str | None:
         return self.api_info.get('app_version')
 
     @cached_property
     def notifiers(self):
         response = self.get(f'{self.api_path}/notifiers')
         if response.ok:
-            return self.get(f'{self.api_path}/notifiers').json().get('notifiers')
+            return response.json().get(
+                'notifiers')
         else:
             return []
 
     def send(self, notifier: str,
              recipient: str,
              body: str = "The body",
              title: str = "You got a buzz",
@@ -80,16 +80,16 @@
 
         response = requests.post(
             f"{self.settings.api}{self.api_path}/send/{notifier}",
             data=data,
             files=files,
             headers=self.headers)
 
-        response.raise_for_status()
+        # response.raise_for_status()
         return response
 
 
 if __name__ == "__main__":
     c = Configuration()
-    c.from_file(filename='settings.yaml', load=yaml_load)  # type: ignore
-    c.from_environ(prefix="BC")
+    c.from_environ(prefix="BUZZ")
     bc = BuzzClient(c)
+    bc.check()
```

### Comparing `buzz_client-1.0.3a0/PKG-INFO` & `buzz_client-1.0.3b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buzz-client
-Version: 1.0.3a0
+Version: 1.0.3b0
 Summary: A client for Buzz API
 License: GPL
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: buzz-client Version: 1.0.3a0 Summary: A client for
+Metadata-Version: 2.1 Name: buzz-client Version: 1.0.3b0 Summary: A client for
 Buzz API License: GPL Author: Andrea Mistrali Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: docopt-ng
 (>=0.9.0,<0.10.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
 requests (>=2.31.0,<3.0.0) Requires-Dist: scriptonite (>=1.0.3,<2.0.0)
```


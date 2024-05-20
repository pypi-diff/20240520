# Comparing `tmp/re_ircbot-2.0.8.dev0.tar.gz` & `tmp/re_ircbot-2.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_ircbot-2.0.8.dev0.tar", last modified: Mon May  6 17:05:37 2024, max compression
+gzip compressed data, was "re_ircbot-2.0.9.dev0.tar", last modified: Wed May  8 16:32:20 2024, max compression
```

## Comparing `re_ircbot-2.0.8.dev0.tar` & `re_ircbot-2.0.9.dev0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 17:05:37.962070 re_ircbot-2.0.8.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-06 17:05:37.962070 re_ircbot-2.0.8.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 17:05:37.962070 re_ircbot-2.0.8.dev0/ircbot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54931 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/dcc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5802 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/format.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18557 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1822 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/shortest_prefix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/sqlitedb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/ircbot/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 17:05:37.962070 re_ircbot-2.0.8.dev0/re_ircbot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-06 17:05:37.000000 re_ircbot-2.0.8.dev0/re_ircbot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2024-05-06 17:05:37.000000 re_ircbot-2.0.8.dev0/re_ircbot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-06 17:05:37.000000 re_ircbot-2.0.8.dev0/re_ircbot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-06 17:05:37.000000 re_ircbot-2.0.8.dev0/re_ircbot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-06 17:05:37.000000 re_ircbot-2.0.8.dev0/re_ircbot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-06 17:05:37.962070 re_ircbot-2.0.8.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-06 17:05:30.000000 re_ircbot-2.0.8.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 16:32:20.339513 re_ircbot-2.0.9.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-08 16:32:20.339513 re_ircbot-2.0.9.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 16:32:20.335513 re_ircbot-2.0.9.dev0/ircbot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54907 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/dcc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5802 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/format.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18557 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1822 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/message.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/shortest_prefix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/sqlitedb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/ircbot/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 16:32:20.339513 re_ircbot-2.0.9.dev0/re_ircbot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-08 16:32:20.000000 re_ircbot-2.0.9.dev0/re_ircbot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2024-05-08 16:32:20.000000 re_ircbot-2.0.9.dev0/re_ircbot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-08 16:32:20.000000 re_ircbot-2.0.9.dev0/re_ircbot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-08 16:32:20.000000 re_ircbot-2.0.9.dev0/re_ircbot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-08 16:32:20.000000 re_ircbot-2.0.9.dev0/re_ircbot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-08 16:32:20.339513 re_ircbot-2.0.9.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-08 16:32:13.000000 re_ircbot-2.0.9.dev0/setup.py
```

### Comparing `re_ircbot-2.0.8.dev0/LICENSE` & `re_ircbot-2.0.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/PKG-INFO` & `re_ircbot-2.0.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.8.dev0
+Version: 2.0.9.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.8.dev0/README.md` & `re_ircbot-2.0.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/ircbot/client.py` & `re_ircbot-2.0.9.dev0/ircbot/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,16 @@
         self.reader = reader
         self.writer = writer
 
     async def send_all(self, data: bytes):
         self.writer.write(data)
         await self.writer.drain()
 
-    async def recv(self, n: int = 2048) -> bytes:
-        return await self.reader.read(n)
+    async def recv(self) -> bytes:
+        return await self.reader.readline()
 
     async def aclose(self):
         self.writer.close()
         await self.writer.wait_closed()
 
     def close(self):
         self.writer.close()
@@ -444,21 +444,21 @@
             await asyncio.sleep(self.delay)
         if self.use_sasl:
             import base64
 
             await stream.send_all(("AUTHENTICATE PLAIN").encode())
             sep = "\x00"
             b = base64.b64encode((self.nick + sep + self.nick + sep + self.password).encode("utf8")).decode("utf8")
-            data = (await stream.recv(4096)).decode("utf-8")
+            data = (await stream.recv()).decode("utf-8")
             log("Server SAYS: ", data)
             await stream.send_all(("AUTHENTICATE " + b).encode())
             log("PERFORMING SASL PLAIN AUTH....")
-            data = (await stream.recv(4096)).decode("utf-8")
+            data = (await stream.recv()).decode("utf-8")
             log("Server SAYS: ", data)
-            data = (await stream.recv(4096)).decode("utf-8")
+            data = (await stream.recv()).decode("utf-8")
             log("Server SAYS: ", data)
             await stream.send_all(("CAP END").encode())
 
         self.stream = stream
         if isinstance(self.channels, list):
             for c in self.channels:
                 await self.join(c)
```

### Comparing `re_ircbot-2.0.8.dev0/ircbot/dcc.py` & `re_ircbot-2.0.9.dev0/ircbot/dcc.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/ircbot/format.py` & `re_ircbot-2.0.9.dev0/ircbot/format.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/ircbot/hooks.py` & `re_ircbot-2.0.9.dev0/ircbot/hooks.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/ircbot/message.py` & `re_ircbot-2.0.9.dev0/ircbot/message.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/ircbot/shortest_prefix.py` & `re_ircbot-2.0.9.dev0/ircbot/shortest_prefix.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/ircbot/sqlitedb.py` & `re_ircbot-2.0.9.dev0/ircbot/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/ircbot/utils.py` & `re_ircbot-2.0.9.dev0/ircbot/utils.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.8.dev0/re_ircbot.egg-info/PKG-INFO` & `re_ircbot-2.0.9.dev0/re_ircbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.8.dev0
+Version: 2.0.9.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.8.dev0/setup.py` & `re_ircbot-2.0.9.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import subprocess
 
 import setuptools
 
-VERSION = "2.0.8-dev"
+VERSION = "2.0.9-dev"
 BRANCH = "v2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def requirements():
```


# Comparing `tmp/cnl2feedcrawler-2.1.0.tar.gz` & `tmp/cnl2feedcrawler-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnl2feedcrawler-2.1.0.tar", last modified: Sun May 19 12:23:50 2024, max compression
+gzip compressed data, was "cnl2feedcrawler-2.1.1.tar", last modified: Sun May 19 18:58:53 2024, max compression
```

## Comparing `cnl2feedcrawler-2.1.0.tar` & `cnl2feedcrawler-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.157802 cnl2feedcrawler-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-19 12:23:50.157802 cnl2feedcrawler-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.153802 cnl2feedcrawler-2.1.0/cnl2feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.153802 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.157802 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.153802 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:23:50.157802 cnl2feedcrawler-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:58:53.494111 cnl2feedcrawler-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-19 18:58:53.494111 cnl2feedcrawler-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:58:53.490111 cnl2feedcrawler-2.1.1/cnl2feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:58:53.494111 cnl2feedcrawler-2.1.1/cnl2feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:58:53.494111 cnl2feedcrawler-2.1.1/cnl2feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:58:53.494111 cnl2feedcrawler-2.1.1/cnl2feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-19 18:58:53.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 18:58:53.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:58:53.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 18:58:53.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:58:53.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 18:58:53.000000 cnl2feedcrawler-2.1.1/cnl2feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:58:53.494111 cnl2feedcrawler-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-19 18:58:46.000000 cnl2feedcrawler-2.1.1/setup.py
```

### Comparing `cnl2feedcrawler-2.1.0/LICENSE` & `cnl2feedcrawler-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnl2feedcrawler-2.1.0/PKG-INFO` & `cnl2feedcrawler-2.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,9 @@
-Metadata-Version: 2.1
-Name: cnl2feedcrawler
-Version: 2.1.0
-Summary: Intercept, decrypt and forward CnL to FeedCrawler
-Home-page: https://github.com/rix1337/ClickNLoad2FeedCrawler
-Author: rix1337
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Click'n'Load2FeedCrawler
-Click'n'Load2FeedCrawler fängt Click'n'Load ab, entschlüsselt die Payload und übergibt diese dem FeedCrawler.
+# ClickNLoad2FeedCrawler
+ClickNLoad2FeedCrawler fängt Click'n'Load ab, entschlüsselt die Payload und übergibt diese dem FeedCrawler.
 
 [![PyPI version](https://badge.fury.io/py/cnl2feedcrawler.svg)](https://badge.fury.io/py/cnl2feedcrawler)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/cnl2feedcrawler)](https://img.shields.io/pypi/dm/cnl2feedcrawler)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
 ####  Voraussetzungen
 * Linux basierte Laufzeitumgebung (inkompatibel mit Windows)
@@ -32,21 +17,37 @@
 
 ```pip install -U cnl2feedcrawler```
 
 #### Starten
 
 ```cnl2feedcrawler --url=192.168.1.1:9090``` in der Konsole (Python muss im System-PATH hinterlegt sein)
 
+# Docker
+```
+docker run -d \
+  --name="Python-Template" \
+  -p 9666:9666 \
+  -e 'URL'='192.168.1.1:9090'
+  rix1337/docker-rix-template:latest
+  ```
+
 
 #### Pflichtparameter
 
 | Parameter         | Erläuterung                                                        |
 |-------------------|--------------------------------------------------------------------|
 | ```--url=<URL>``` | Die lokale URL des FeedCrawlers - bspw. `http://192.168.1.1:9090`) |
 
-***
 
-## Credits
 
-* [drwilly](https://github.com/drwilly)
+## Click'n'Load auf Windows umleiten
+
+`netsh interface portproxy add v4tov4 listenport=9666 connectaddress=<Docker Host> connectport=9666 listenaddress=127.0.0.1`
 
+#### Umleitung entfernen:
 
+`netsh interface portproxy delete v4tov4 listenport=9666 listenaddress=127.0.0.1`
+
+
+## Credits
+
+* [drwilly](https://github.com/drwilly)
```

### Comparing `cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/http_requests/request_handler.py` & `cnl2feedcrawler-2.1.1/cnl2feedcrawler/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `cnl2feedcrawler-2.1.0/cnl2feedcrawler/run.py` & `cnl2feedcrawler-2.1.1/cnl2feedcrawler/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             print(output)
         else:
             print(output, file=self.file)
         return output
 
 
 class CNLHandler(http.server.BaseHTTPRequestHandler):
-    http.server.BaseHTTPRequestHandler.server_version = "Click'n'Load2FeedCrawler"
+    http.server.BaseHTTPRequestHandler.server_version = "ClickNLoad2FeedCrawler"
     http.server.BaseHTTPRequestHandler.sys_version = ""
 
     def __init__(self, request, client_address, server):
         self.URL_MAPPING = [
             URLMap("/", get_fn=self.alive),
             URLMap("/jdcheck.js", get_fn=self.jdcheck),
             URLMap("/crossdomain.xml", get_fn=self.crossdomain),
@@ -230,15 +230,15 @@
     return ip
 
 
 def main():
     global feedcrawler_url
 
     print("┌──────────────────────────────────────────────────┐")
-    print(f"  Click'n'Load2FeedCrawler v.{get_version()} von RiX")
+    print(f"  ClickNLoad2FeedCrawler v.{get_version()} von RiX")
     print("  https://github.com/rix1337/ClickNLoad2FeedCrawler")
     print("└──────────────────────────────────────────────────┘")
     local_address = 'http://' + check_ip() + ':' + str(9666)
 
     # Test if NodeJS is available
     try:
         node_version = call(["node", "-v"])
```

### Comparing `cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/PKG-INFO` & `cnl2feedcrawler-2.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cnl2feedcrawler
-Version: 2.1.0
+Version: 2.1.1
 Summary: Intercept, decrypt and forward CnL to FeedCrawler
 Home-page: https://github.com/rix1337/ClickNLoad2FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Click'n'Load2FeedCrawler
-Click'n'Load2FeedCrawler fängt Click'n'Load ab, entschlüsselt die Payload und übergibt diese dem FeedCrawler.
+# ClickNLoad2FeedCrawler
+ClickNLoad2FeedCrawler fängt Click'n'Load ab, entschlüsselt die Payload und übergibt diese dem FeedCrawler.
 
 [![PyPI version](https://badge.fury.io/py/cnl2feedcrawler.svg)](https://badge.fury.io/py/cnl2feedcrawler)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/cnl2feedcrawler)](https://img.shields.io/pypi/dm/cnl2feedcrawler)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
 ####  Voraussetzungen
 * Linux basierte Laufzeitumgebung (inkompatibel mit Windows)
@@ -32,21 +32,39 @@
 
 ```pip install -U cnl2feedcrawler```
 
 #### Starten
 
 ```cnl2feedcrawler --url=192.168.1.1:9090``` in der Konsole (Python muss im System-PATH hinterlegt sein)
 
+# Docker
+```
+docker run -d \
+  --name="Python-Template" \
+  -p 9666:9666 \
+  -e 'URL'='192.168.1.1:9090'
+  rix1337/docker-rix-template:latest
+  ```
+
 
 #### Pflichtparameter
 
 | Parameter         | Erläuterung                                                        |
 |-------------------|--------------------------------------------------------------------|
 | ```--url=<URL>``` | Die lokale URL des FeedCrawlers - bspw. `http://192.168.1.1:9090`) |
 
-***
+
+
+## Click'n'Load auf Windows umleiten
+
+`netsh interface portproxy add v4tov4 listenport=9666 connectaddress=<Docker Host> connectport=9666 listenaddress=127.0.0.1`
+
+#### Umleitung entfernen:
+
+`netsh interface portproxy delete v4tov4 listenport=9666 listenaddress=127.0.0.1`
+
 
 ## Credits
 
 * [drwilly](https://github.com/drwilly)
```

### Comparing `cnl2feedcrawler-2.1.0/setup.py` & `cnl2feedcrawler-2.1.1/setup.py`

 * *Files identical despite different names*


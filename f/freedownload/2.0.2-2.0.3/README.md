# Comparing `tmp/freedownload-2.0.2.tar.gz` & `tmp/freedownload-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freedownload-2.0.2.tar", last modified: Wed May 15 04:17:37 2024, max compression
+gzip compressed data, was "freedownload-2.0.3.tar", last modified: Mon May 20 13:58:01 2024, max compression
```

## Comparing `freedownload-2.0.2.tar` & `freedownload-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 04:17:37.840581 freedownload-2.0.2/
--rw-rw-rw-   0        0        0     1036 2024-05-15 04:17:37.839584 freedownload-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 freedownload-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 04:17:37.809087 freedownload-2.0.2/freedownload/
--rw-rw-rw-   0        0        0     8327 2024-05-15 04:13:48.000000 freedownload-2.0.2/freedownload/__init__.py
--rw-rw-rw-   0        0        0       75 2024-05-15 04:14:52.000000 freedownload-2.0.2/freedownload/version.py
-drwxrwxrwx   0        0        0        0 2024-05-15 04:17:37.838587 freedownload-2.0.2/freedownload.egg-info/
--rw-rw-rw-   0        0        0     1036 2024-05-15 04:17:37.000000 freedownload-2.0.2/freedownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-15 04:17:37.000000 freedownload-2.0.2/freedownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 04:17:37.000000 freedownload-2.0.2/freedownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-15 04:17:37.000000 freedownload-2.0.2/freedownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-15 04:17:37.000000 freedownload-2.0.2/freedownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-05-15 04:17:37.000000 freedownload-2.0.2/freedownload.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-15 04:17:37.840581 freedownload-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1612 2023-12-21 01:53:29.000000 freedownload-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:58:01.414695 freedownload-2.0.3/
+-rw-rw-rw-   0        0        0     1036 2024-05-20 13:58:01.412699 freedownload-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 freedownload-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 13:58:01.372229 freedownload-2.0.3/freedownload/
+-rw-rw-rw-   0        0        0     8308 2024-05-20 13:55:55.000000 freedownload-2.0.3/freedownload/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-20 13:56:54.000000 freedownload-2.0.3/freedownload/version.py
+drwxrwxrwx   0        0        0        0 2024-05-20 13:58:01.410704 freedownload-2.0.3/freedownload.egg-info/
+-rw-rw-rw-   0        0        0     1036 2024-05-20 13:58:01.000000 freedownload-2.0.3/freedownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-20 13:58:01.000000 freedownload-2.0.3/freedownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 13:58:01.000000 freedownload-2.0.3/freedownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-20 13:58:01.000000 freedownload-2.0.3/freedownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 13:58:01.000000 freedownload-2.0.3/freedownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-20 13:58:01.000000 freedownload-2.0.3/freedownload.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-20 13:58:01.414695 freedownload-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1612 2023-12-21 01:53:29.000000 freedownload-2.0.3/setup.py
```

### Comparing `freedownload-2.0.2/PKG-INFO` & `freedownload-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedownload
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python 3 library for short text
 Home-page: https://github.com/hiyabo69/downfree
 Author: Jose
 Author-email: josepalaciosgiraldo91@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `freedownload-2.0.2/README.md` & `freedownload-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `freedownload-2.0.2/freedownload/__init__.py` & `freedownload-2.0.3/freedownload/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,27 +23,27 @@
     cmd = "cls"
 elif sistema_operativo == "Linux":
     cmd = "clear"
 
 def sizeof_fmt(num, suffix='B'):
     for unit in ['','Ki','Mi','Gi','Ti','Pi','Ei','Zi']:
         if abs(num) < 1024.0:
-            return "%3.1f%s%s" % (num, unit, suffix)
+            return "%3.2f%s%s" % (num, unit, suffix)
         num /= 1024.0
     return "%.1f%s%s" % (num, 'Yi', suffix)
 
 def progress(filename, index, total):
-    downloaded_mb = index / (1024 * 1024)
-    total_mb = total / (1024 * 1024)
+    downloaded_mb = sizeof_fmt(index)
+    total_mb = sizeof_fmt(total)
     downloaded_percent = (index / total) * 100
-    progress_bar_length = 15
+    progress_bar_length = 10
     completed_length = int(progress_bar_length * downloaded_percent / 100)
     remaining_length = progress_bar_length - completed_length
 
-    print(f"{Fore.GREEN}{filename} [{completed_length * '●'}{remaining_length * '○'}] {downloaded_mb:.2f}MB / {total_mb:.2f}MB ({downloaded_percent:.2f}%)", end='\r')
+    print(f"{Fore.GREEN}{filename} [{completed_length * '●'}{remaining_length * '○'}] {downloaded_mb}/{total_mb}", end='\r')
 
 def printl(text):
     init()
     print(Fore.GREEN + text,end='\r')
 
 def make_session(dl):
     session = requests.Session()
@@ -148,15 +148,15 @@
                     chunkurl = dl["c"] + "draftfile.php/" + draftid + "/user/draft/" + fileid + "/" + f"{filename.replace(' ','%2520')}-{i}.zip"
                 else:
                     chunkurl = dl['c'].split('^')[0] + chunkur + dl['c'].split('^')[1]
                 resp = session.get(chunkurl, headers=headers, stream=True, verify=False)
                 for chunk in resp.iter_content(chunk_size=8192):
                     chunk_por += len(chunk)
                     f.write(chunk)
-                    progress(f'{filet} ', chunk_por, total_size)
+                    progress(f'{filet}', chunk_por, total_size)
                 l += 1
                 i += 1
             f.close()
             v = ["uoi","m","moodle","evea","ts"]
             if not dl["m"] in v:
                 new_file = str(randint(1000,99999))+filename.replace(".png","") 
                 with open(new_file, "wb") as file:
@@ -192,14 +192,15 @@
         print(Fore.CYAN + 'Pegue una direct Url o escriba "start" para comenzar la descarga de la cola')
         msg = input()
         if msg.lower() == "start":
             if download_queue.empty():
                 print(Fore.RED + "La cola de descarga está vacía. Pegue una URL para agregarla a la cola.")
                 continue
             else:
+                os.system(cmd)
                 print(Fore.GREEN + "Comenzando la descarga de la cola...")
                 print(Fore.RED + "!!! Iniciando Sesión.")
                 result = wait_download(download_queue, ichunk, index, file, session)
                 if result:
                     break
         else:
             url = ast.literal_eval(msg)
```

### Comparing `freedownload-2.0.2/freedownload.egg-info/PKG-INFO` & `freedownload-2.0.3/freedownload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedownload
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python 3 library for short text
 Home-page: https://github.com/hiyabo69/downfree
 Author: Jose
 Author-email: josepalaciosgiraldo91@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `freedownload-2.0.2/setup.py` & `freedownload-2.0.3/setup.py`

 * *Files identical despite different names*


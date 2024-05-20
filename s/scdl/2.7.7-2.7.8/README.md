# Comparing `tmp/scdl-2.7.7.tar.gz` & `tmp/scdl-2.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/scdl/scdl/dist/.tmp-tjy4zj9j/scdl-2.7.7.tar", last modified: Tue Apr 30 17:05:25 2024, max compression
+gzip compressed data, was "/home/runner/work/scdl/scdl/dist/.tmp-z3hlvkhp/scdl-2.7.8.tar", last modified: Mon May 20 17:31:29 2024, max compression
```

## Comparing `scdl-2.7.7.tar` & `scdl-2.7.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:05:25.000000 scdl-2.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 17:05:08.000000 scdl-2.7.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-04-30 17:05:08.000000 scdl-2.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 17:05:08.000000 scdl-2.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-30 17:05:25.000000 scdl-2.7.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4954 2024-04-30 17:05:08.000000 scdl-2.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 17:05:08.000000 scdl-2.7.7/scdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 17:05:08.000000 scdl-2.7.7/scdl/scdl.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    38567 2024-04-30 17:05:08.000000 scdl-2.7.7/scdl/scdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-30 17:05:08.000000 scdl-2.7.7/scdl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 17:05:25.000000 scdl-2.7.7/scdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 17:05:25.000000 scdl-2.7.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-04-30 17:05:08.000000 scdl-2.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:31:29.000000 scdl-2.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-20 17:31:13.000000 scdl-2.7.8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-05-20 17:31:13.000000 scdl-2.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 17:31:13.000000 scdl-2.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-20 17:31:29.000000 scdl-2.7.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4954 2024-05-20 17:31:13.000000 scdl-2.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 17:31:13.000000 scdl-2.7.8/scdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 17:31:13.000000 scdl-2.7.8/scdl/scdl.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38901 2024-05-20 17:31:13.000000 scdl-2.7.8/scdl/scdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-20 17:31:13.000000 scdl-2.7.8/scdl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 17:31:29.000000 scdl-2.7.8/scdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:31:29.000000 scdl-2.7.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-05-20 17:31:13.000000 scdl-2.7.8/setup.py
```

### Comparing `scdl-2.7.7/LICENSE` & `scdl-2.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scdl-2.7.7/PKG-INFO` & `scdl-2.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdl
-Version: 2.7.7
+Version: 2.7.8
 Summary: Download Music from Souncloud
 Home-page: https://github.com/flyingrub/scdl
 Author: FlyinGrub
 Author-email: flyinggrub@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `scdl-2.7.7/README.md` & `scdl-2.7.8/README.md`

 * *Files identical despite different names*

### Comparing `scdl-2.7.7/scdl/scdl.cfg` & `scdl-2.7.8/scdl/scdl.cfg`

 * *Files identical despite different names*

### Comparing `scdl-2.7.7/scdl/scdl.py` & `scdl-2.7.8/scdl/scdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,32 +272,46 @@
     sys.exit(1)
 
 def get_config(config_file: pathlib.Path) -> configparser.ConfigParser:
     """
     Gets config from scdl.cfg
     """
     config = configparser.ConfigParser()
-    
+
     default_config_file = pathlib.Path(__file__).with_name("scdl.cfg")
 
     # load default config first
     config.read_file(open(default_config_file, encoding="UTF-8"))
-    
+
     # load config file if it exists
     if config_file.exists():
         config.read_file(open(config_file, encoding="UTF-8"))
-    
+
     # save config to disk
     config_file.parent.mkdir(parents=True, exist_ok=True)
     with open(config_file, "w", encoding="UTF-8") as f:
         config.write(f)
-        
+
     return config
 
 
+def sanitize_str(filename: str, replacement_char: str = "�", max_length: int = 255):
+    """
+    Sanitizes a string for use as a filename. Does not allow the file to be hidden
+    """
+    if filename.startswith("."):
+        filename = "_" + filename
+    if filename.endswith("."):
+        filename = filename + "_"
+    sanitized = sanitize_filename(
+        filename, replacement_text=replacement_char, max_len=max_length
+    )
+    return sanitized
+
+
 def download_url(client: SoundCloud, **kwargs):
     """
     Detects if a URL is a track or a playlist, and parses the track(s)
     to the track downloader
     """
     url = kwargs.get("l")
     item = client.resolve(url)
@@ -447,15 +461,15 @@
     Downloads a playlist
     """
     if kwargs.get("no_playlist"):
         logger.info("Skipping playlist...")
         return
     playlist_name = playlist.title.encode("utf-8", "ignore")
     playlist_name = playlist_name.decode("utf-8")
-    playlist_name = sanitize_filename(playlist_name)
+    playlist_name = sanitize_str(playlist_name)
     playlist_info = {
                 "author": playlist.user.username,
                 "id": playlist.id,
                 "title": playlist.title
     }
 
     if not kwargs.get("no_playlist_folder"):
@@ -467,19 +481,19 @@
         if kwargs.get("n"):  # Order by creation date and get the n lasts tracks
             playlist.tracks.sort(
                 key=lambda track: track.id, reverse=True
             )
             playlist.tracks = playlist.tracks[: int(kwargs.get("n"))]
             kwargs["playlist_offset"] = 0
         if kwargs.get("sync"):
-                  if os.path.isfile(kwargs.get("sync")):
-                        playlist.tracks = sync(client, playlist, playlist_info, **kwargs)
-                  else:
-                        logger.error(f'Invalid sync archive file {kwargs.get("sync")}')
-                        sys.exit(1)
+            if os.path.isfile(kwargs.get("sync")):
+                playlist.tracks = sync(client, playlist, playlist_info, **kwargs)
+            else:
+                logger.error(f'Invalid sync archive file {kwargs.get("sync")}')
+                sys.exit(1)
 
         tracknumber_digits = len(str(len(playlist.tracks)))
         for counter, track in itertools.islice(enumerate(playlist.tracks, 1), kwargs.get("playlist_offset", 0), None):
             logger.debug(track)
             logger.info(f"Track n°{counter}")
             playlist_info["tracknumber"] = str(counter).zfill(tracknumber_digits)
             if isinstance(track, MiniTrack):
@@ -496,39 +510,38 @@
 def try_utime(path, filetime):
     try:
         os.utime(path, (time.time(), filetime))
     except Exception:
         logger.error("Cannot update utime of file")
 
 def get_filename(track: BasicTrack, original_filename=None, aac=False, playlist_info=None, **kwargs):
-    
+
     username = track.user.username
     title = track.title.encode("utf-8", "ignore").decode("utf-8")
 
     if kwargs.get("addtofile"):
         if username not in title and "-" not in title:
             title = "{0} - {1}".format(username, title)
             logger.debug('Adding "{0}" to filename'.format(username))
 
     timestamp = str(int(track.created_at.timestamp()))
     if kwargs.get("addtimestamp"):
         title = timestamp + "_" + title
-    
+
     if not kwargs.get("addtofile") and not kwargs.get("addtimestamp"):
         if playlist_info:
             title = kwargs.get("playlist_name_format").format(**asdict(track), playlist=playlist_info, timestamp=timestamp)
         else:
             title = kwargs.get("name_format").format(**asdict(track), timestamp=timestamp)
 
     ext = ".m4a" if aac else ".mp3"  # contain aac in m4a to write metadata
     if original_filename is not None:
         original_filename = original_filename.encode("utf-8", "ignore").decode("utf-8")
         ext = os.path.splitext(original_filename)[1]
-    filename = limit_filename_length(title, ext)
-    filename = sanitize_filename(filename)
+    filename = sanitize_str(title + ext)
     return filename
 
 
 def download_original_file(client: SoundCloud, track: BasicTrack, title: str, playlist_info=None, **kwargs):
     logger.info("Downloading the original file.")
 
     # Get the requests stream
```

### Comparing `scdl-2.7.7/scdl/utils.py` & `scdl-2.7.8/scdl/utils.py`

 * *Files identical despite different names*

### Comparing `scdl-2.7.7/scdl.egg-info/PKG-INFO` & `scdl-2.7.8/scdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdl
-Version: 2.7.7
+Version: 2.7.8
 Summary: Download Music from Souncloud
 Home-page: https://github.com/flyingrub/scdl
 Author: FlyinGrub
 Author-email: flyinggrub@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `scdl-2.7.7/setup.py` & `scdl-2.7.8/setup.py`

 * *Files identical despite different names*


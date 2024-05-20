# Comparing `tmp/api_deezer-0.0.1b1.tar.gz` & `tmp/api_deezer-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_deezer-0.0.1b1.tar", max compression
+gzip compressed data, was "api_deezer-0.0.1b2.tar", max compression
```

## Comparing `api_deezer-0.0.1b1.tar` & `api_deezer-0.0.1b2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0       48 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/README.md
--rwxr-xr-x   0        0        0       44 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/__init__.py
--rwxr-xr-x   0        0        0     1830 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/api.py
--rwxr-xr-x   0        0        0     1802 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/decorators/links.py
--rwxr-xr-x   0        0        0      327 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/exceptions/data.py
--rwxr-xr-x   0        0        0      675 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/exceptions/links.py
--rwxr-xr-x   0        0        0        0 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/tests/__init__.py
--rwxr-xr-x   0        0        0       37 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/tests/test.sh
--rwxr-xr-x   0        0        0     1944 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/tests/test_media_types.py
--rwxr-xr-x   0        0        0      169 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/__init__.py
--rwxr-xr-x   0        0        0     1852 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/album.py
--rwxr-xr-x   0        0        0      258 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/artist.py
--rwxr-xr-x   0        0        0     2439 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/chart.py
--rwxr-xr-x   0        0        0      246 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/contributor.py
--rwxr-xr-x   0        0        0      984 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/explicit_content.py
--rwxr-xr-x   0        0        0      101 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/genre.py
--rwxr-xr-x   0        0        0     1504 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/playlist.py
--rwxr-xr-x   0        0        0     1179 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/api_deezer/types/track.py
--rw-r--r--   0        0        0      370 2024-05-19 14:50:40.104152 api_deezer-0.0.1b1/pyproject.toml
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 api_deezer-0.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/README.md
+-rwxr-xr-x   0        0        0       44 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/__init__.py
+-rwxr-xr-x   0        0        0     2969 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/api.py
+-rwxr-xr-x   0        0        0      233 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/exceptions/data.py
+-rwxr-xr-x   0        0        0      487 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/exceptions/links.py
+-rw-r--r--   0        0        0      109 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/py.typed
+-rwxr-xr-x   0        0        0      235 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/__init__.py
+-rwxr-xr-x   0        0        0     1844 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/album.py
+-rwxr-xr-x   0        0        0      407 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/artist.py
+-rwxr-xr-x   0        0        0     2439 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/chart.py
+-rwxr-xr-x   0        0        0      246 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/contributor.py
+-rwxr-xr-x   0        0        0      984 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/explicit_content.py
+-rwxr-xr-x   0        0        0      101 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/genre.py
+-rwxr-xr-x   0        0        0     1504 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/playlist.py
+-rwxr-xr-x   0        0        0     1179 2024-05-20 10:40:17.398403 api_deezer-0.0.1b2/api_deezer/types/track.py
+-rw-r--r--   0        0        0      968 2024-05-20 10:40:17.402403 api_deezer-0.0.1b2/api_deezer/utils.py
+-rw-r--r--   0        0        0      370 2024-05-20 10:40:17.402403 api_deezer-0.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 api_deezer-0.0.1b2/PKG-INFO
```

### Comparing `api_deezer-0.0.1b1/api_deezer/types/album.py` & `api_deezer-0.0.1b2/api_deezer/types/album.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class Artist_Album(BaseModel):
 	id: int
 	name: str
 	picture: str
 	picture_small: str
 	picture_medium: str
 	picture_big: str
-	piOptionalcture_xl: str
+	picture_xl: str
 	type: str
 
 
 class Album_Track_Artist(BaseModel):
 	id: int
 	name: str
 	tracklist: str
```

### Comparing `api_deezer-0.0.1b1/api_deezer/types/chart.py` & `api_deezer-0.0.1b2/api_deezer/types/chart.py`

 * *Files identical despite different names*

### Comparing `api_deezer-0.0.1b1/api_deezer/types/explicit_content.py` & `api_deezer-0.0.1b2/api_deezer/types/explicit_content.py`

 * *Files identical despite different names*

### Comparing `api_deezer-0.0.1b1/api_deezer/types/playlist.py` & `api_deezer-0.0.1b2/api_deezer/types/playlist.py`

 * *Files identical despite different names*

### Comparing `api_deezer-0.0.1b1/api_deezer/types/track.py` & `api_deezer-0.0.1b2/api_deezer/types/track.py`

 * *Files identical despite different names*


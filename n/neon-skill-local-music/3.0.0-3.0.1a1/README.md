# Comparing `tmp/neon-skill-local_music-3.0.0.tar.gz` & `tmp/neon-skill-local_music-3.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-local_music-3.0.0.tar", last modified: Tue Apr  9 23:12:37 2024, max compression
+gzip compressed data, was "neon-skill-local_music-3.0.1a1.tar", last modified: Mon May 20 16:07:42 2024, max compression
```

## Comparing `neon-skill-local_music-3.0.0.tar` & `neon-skill-local_music-3.0.1a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.227141 neon-skill-local_music-3.0.0/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.227141 neon-skill-local_music-3.0.0/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/locale/en-us/vocab/local.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 23:12:37.000000 neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-09 23:12:31.000000 neon-skill-local_music-3.0.0/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-09 23:12:32.000000 neon-skill-local_music-3.0.0/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 23:12:32.000000 neon-skill-local_music-3.0.0/ui/music-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:12:37.231141 neon-skill-local_music-3.0.0/util/
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-09 23:12:32.000000 neon-skill-local_music-3.0.0/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-09 23:12:32.000000 neon-skill-local_music-3.0.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:07:42.243410 neon-skill-local_music-3.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-20 16:07:35.000000 neon-skill-local_music-3.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-20 16:07:42.243410 neon-skill-local_music-3.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-20 16:07:35.000000 neon-skill-local_music-3.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-05-20 16:07:35.000000 neon-skill-local_music-3.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:07:42.239410 neon-skill-local_music-3.0.1a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:07:42.239410 neon-skill-local_music-3.0.1a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:07:42.239410 neon-skill-local_music-3.0.1a1/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 16:07:35.000000 neon-skill-local_music-3.0.1a1/locale/en-us/vocab/local.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:07:42.243410 neon-skill-local_music-3.0.1a1/neon_skill_local_music.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-20 16:07:42.000000 neon-skill-local_music-3.0.1a1/neon_skill_local_music.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 16:07:42.000000 neon-skill-local_music-3.0.1a1/neon_skill_local_music.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:07:42.000000 neon-skill-local_music-3.0.1a1/neon_skill_local_music.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 16:07:42.000000 neon-skill-local_music-3.0.1a1/neon_skill_local_music.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 16:07:42.000000 neon-skill-local_music-3.0.1a1/neon_skill_local_music.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 16:07:42.000000 neon-skill-local_music-3.0.1a1/neon_skill_local_music.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:07:42.243410 neon-skill-local_music-3.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-20 16:07:35.000000 neon-skill-local_music-3.0.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-20 16:07:35.000000 neon-skill-local_music-3.0.1a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:07:42.243410 neon-skill-local_music-3.0.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-20 16:07:36.000000 neon-skill-local_music-3.0.1a1/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:07:42.243410 neon-skill-local_music-3.0.1a1/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 16:07:36.000000 neon-skill-local_music-3.0.1a1/ui/music-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:07:42.243410 neon-skill-local_music-3.0.1a1/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-05-20 16:07:36.000000 neon-skill-local_music-3.0.1a1/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-20 16:07:36.000000 neon-skill-local_music-3.0.1a1/version.py
```

### Comparing `neon-skill-local_music-3.0.0/LICENSE.md` & `neon-skill-local_music-3.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-3.0.0/PKG-INFO` & `neon-skill-local_music-3.0.1a1/neon_skill_local_music.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-skill-local_music
-Version: 3.0.0
+Name: neon-skill-local-music
+Version: 3.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-local_music
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-local_music-3.0.0/README.md` & `neon-skill-local_music-3.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-3.0.0/__init__.py` & `neon-skill-local_music-3.0.1a1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,19 +114,24 @@
         if not results and self.voc_match(phrase, 'local.voc'):
             score = 60
             if media_type == MediaType.MUSIC:
                 score += 20
             else:
                 LOG.debug("No media type requested")
             all_songs = self.music_library.all_songs
+            non_demo = [s for s in all_songs
+                        if not s.path.startswith(self._demo_dir)]
+            if non_demo:
+                LOG.debug("Using non-demo tracks")
+                all_songs = non_demo
             if len(all_songs) > 50:
                 all_songs = sample(self.music_library.all_songs, 50)
             results = self._tracks_to_search_results(all_songs, score)
-            LOG.debug(f"Returning all songs with score={score}")
-        LOG.info(f"Returning {len(results)} results")  # conf 65
+            LOG.info(f"Returning all songs with score={score}")
+        LOG.info(f"Returning {len(results)} results")
         return results
 
     def search_artist(self, phrase, media_type=MediaType.GENERIC) -> List[dict]:
         score = 65
         if media_type == MediaType.MUSIC:
             score += 20
         if self.voc_match(phrase, 'local.voc'):
```

### Comparing `neon-skill-local_music-3.0.0/neon_skill_local_music.egg-info/PKG-INFO` & `neon-skill-local_music-3.0.1a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-skill-local-music
-Version: 3.0.0
+Name: neon-skill-local_music
+Version: 3.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-local_music
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-local_music-3.0.0/setup.py` & `neon-skill-local_music-3.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-3.0.0/skill.json` & `neon-skill-local_music-3.0.1a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-3.0.0/test/test_skill.py` & `neon-skill-local_music-3.0.1a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-local_music-3.0.0/util/__init__.py` & `neon-skill-local_music-3.0.1a1/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                     with open(self._db_file, 'rb') as f:
                         self._songs = pickle.load(f)
             except Exception as e:
                 LOG.exception(e)
                 remove(self._db_file)
 
     @property
-    def all_songs(self):
+    def all_songs(self) -> List[Track]:
         return list(self._songs.values())
 
     def search_songs_for_artist(self, artist: str) -> List[Track]:
         """
         Get all songs by a particular artist
         """
         return [song for song in self._songs.values() if song.artist and
```

### Comparing `neon-skill-local_music-3.0.0/version.py` & `neon-skill-local_music-3.0.1a1/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "3.0.0"
+__version__ = "3.0.1a1"
```


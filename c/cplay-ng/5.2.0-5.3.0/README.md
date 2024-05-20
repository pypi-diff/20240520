# Comparing `tmp/cplay-ng-5.2.0.tar.gz` & `tmp/cplay_ng-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cplay-ng-5.2.0.tar", last modified: Thu Feb  9 22:35:33 2023, max compression
+gzip compressed data, was "cplay_ng-5.3.0.tar", last modified: Mon May 20 21:45:39 2024, max compression
```

## Comparing `cplay-ng-5.2.0.tar` & `cplay_ng-5.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-02-09 22:35:33.379713 cplay-ng-5.2.0/
--rw-r--r--   0 tobias    (1000) tobias    (1000)      485 2019-07-18 07:03:19.000000 cplay-ng-5.2.0/AUTHORS
--rw-r--r--   0 tobias    (1000) tobias    (1000)    18009 2012-10-23 11:10:59.000000 cplay-ng-5.2.0/LICENSE
--rw-r--r--   0 tobias    (1000) tobias    (1000)     1611 2023-02-09 22:35:33.379713 cplay-ng-5.2.0/PKG-INFO
--rw-r--r--   0 tobias    (1000) tobias    (1000)      873 2023-02-09 22:29:10.000000 cplay-ng-5.2.0/README.rst
--rw-r--r--   0 tobias    (1000) tobias    (1000)    23795 2023-02-09 22:31:23.000000 cplay-ng-5.2.0/cplay.py
-drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-02-09 22:35:33.379713 cplay-ng-5.2.0/cplay_ng.egg-info/
--rw-r--r--   0 tobias    (1000) tobias    (1000)     1611 2023-02-09 22:35:33.000000 cplay-ng-5.2.0/cplay_ng.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) tobias    (1000)      207 2023-02-09 22:35:33.000000 cplay-ng-5.2.0/cplay_ng.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)        1 2023-02-09 22:35:33.000000 cplay-ng-5.2.0/cplay_ng.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)       40 2023-02-09 22:35:33.000000 cplay-ng-5.2.0/cplay_ng.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)        6 2023-02-09 22:35:33.000000 cplay-ng-5.2.0/cplay_ng.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)       38 2023-02-09 22:35:33.379713 cplay-ng-5.2.0/setup.cfg
--rw-r--r--   0 tobias    (1000) tobias    (1000)      987 2023-02-09 22:31:31.000000 cplay-ng-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:45:39.168526 cplay_ng-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 21:45:33.000000 cplay_ng-5.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-20 21:45:33.000000 cplay_ng-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-20 21:45:39.168526 cplay_ng-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-20 21:45:33.000000 cplay_ng-5.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24309 2024-05-20 21:45:33.000000 cplay_ng-5.3.0/cplay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:45:39.168526 cplay_ng-5.3.0/cplay_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-20 21:45:39.000000 cplay_ng-5.3.0/cplay_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 21:45:39.000000 cplay_ng-5.3.0/cplay_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:45:39.000000 cplay_ng-5.3.0/cplay_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 21:45:39.000000 cplay_ng-5.3.0/cplay_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 21:45:39.000000 cplay_ng-5.3.0/cplay_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 21:45:33.000000 cplay_ng-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:45:39.168526 cplay_ng-5.3.0/setup.cfg
```

### Comparing `cplay-ng-5.2.0/LICENSE` & `cplay_ng-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cplay-ng-5.2.0/PKG-INFO` & `cplay_ng-5.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: cplay-ng
-Version: 5.2.0
+Version: 5.3.0
 Summary: A simple curses audio player
-Home-page: https://github.com/xi/cplay-ng
-Author: Ulf Betlehem
-Author-email: flu@iki.fi
-Maintainer: Tobias Bengfort
-Maintainer-email: tobias.bengfort@posteo.de
+Author-email: Ulf Betlehem <flu@iki.fi>
+Maintainer-email: Tobias Bengfort <tobias.bengfort@posteo.de>
 License: GPLv2+
+Project-URL: Homepage, https://github.com/xi/cplay-ng
+Keywords: music-player,curses
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Topic :: Multimedia :: Sound/Audio :: Players
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Description
 -----------
 
 ``cplay`` is a minimalist music player with a textual user interface
```

### Comparing `cplay-ng-5.2.0/README.rst` & `cplay_ng-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `cplay-ng-5.2.0/cplay.py` & `cplay_ng-5.3.0/cplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import socket
 import subprocess
 import sys
 import termios
 import time
 from contextlib import contextmanager
 
-__version__ = 'cplay-ng 5.2.0'
+__version__ = 'cplay-ng 5.3.0'
 
 AUDIO_EXTENSIONS = [
     'mp3', 'ogg', 'oga', 'opus', 'flac', 'm4a', 'm4b', 'wav', 'mid', 'wma'
 ]
 
 HELP = """Global
 ------
@@ -74,29 +74,37 @@
     return '%02d:%02d:%02d' % (h, m, s)
 
 
 def str_match(query, s):
     return all(q in s.lower() for q in query.lower().split())
 
 
-def resize(*args):
+def resize(*_args):
     os.write(app.resize_out, b'.')
 
 
 def get_socket(path):
     while True:
         try:
             sock = socket.socket(family=socket.AF_UNIX)
             sock.connect(path)
-            return sock
         except (FileNotFoundError, ConnectionRefusedError):
             time.sleep(0.1)
+        else:
+            return sock
 
 
-@functools.lru_cache()
+@functools.cache
+def get_mpv_version():
+    p = subprocess.run(['mpv', '--version'], stdout=subprocess.PIPE)
+    s = p.stdout.split(b' ', 2)[1].decode()
+    return tuple(int(i) for i in s.split('.'))
+
+
+@functools.lru_cache
 def relpath(path):
     if path.startswith('http'):
         return path
     elif path.startswith(filelist.path):
         return path[len(filelist.path):].lstrip('/')
     else:
         return os.path.relpath(path)
@@ -144,15 +152,15 @@
 
         self.socket_path = '%s/mpv-cplay-%i.sock' % (
             os.getenv('XDG_RUNTIME_DIR', '/tmp'), os.getpid()
         )
         self._proc = subprocess.Popen(
             [
                 'mpv',
-                '--input-ipc-server=%s' % self.socket_path,
+                f'--input-ipc-server={self.socket_path}',
                 '--idle',
                 '--audio-display=no',
                 '--replaygain=track',
             ],
             stdin=subprocess.DEVNULL,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
@@ -208,19 +216,26 @@
 
     def _play(self):
         if not self.path:
             self.is_playing = False
             return
         self.is_playing = True
         self._playing += 1
-        self._ipc('loadfile', self.path, 'replace', 'start=%i' % self.position)
+        if get_mpv_version() > (0, 38, 0):
+            self._ipc('loadfile', self.path, 'replace', 0, 'start=%i' % self.position)
+        else:
+            self._ipc('loadfile', self.path, 'replace', 'start=%i' % self.position)
 
     def play(self, path):
-        self.path = path
-        self.position = 0
+        if path and (m := re.match(r'^(http.*)#t=([0-9]+)$', path)):
+            self.path = m[1]
+            self.position = float(m[2])
+        else:
+            self.path = path
+            self.position = 0
         self.length = 0
         self._seek_step = 0
         self._play()
 
     def toggle(self):
         if self.is_playing:
             self.stop()
@@ -330,21 +345,21 @@
         items = self.items[self.position:self.position + self.rows]
         for i, item in enumerate(items):
             attr = 0
             if self.position + i == self.cursor:
                 attr |= curses.A_REVERSE
             if self.position + i == self.active:
                 attr |= curses.A_BOLD
-            item = self.format_item(item)
-            item = space_between('  ' + item, '', app.cols)
-            yield (item, attr)
-        for i in range(max(0, self.rows - len(items))):
+            s_item = self.format_item(item)
+            s_item = space_between('  ' + s_item, '', app.cols)
+            yield (s_item, attr)
+        for _i in range(max(0, self.rows - len(items))):
             yield ''
 
-    def process_key(self, key):
+    def process_key(self, key):  # noqa: C901
         if key in [curses.KEY_DOWN, 'j']:
             self.move_cursor(1)
         elif key in [curses.KEY_UP, 'k']:
             self.move_cursor(-1)
         elif key in [curses.KEY_NPAGE, 'J']:
             self.move_cursor(self.rows - 2)
         elif key in [curses.KEY_PPAGE, 'K']:
@@ -394,28 +409,26 @@
 
     def get_title(self):
         title = 'Filelist: %s/' % self.path.rstrip('/')
         if self.rsearch_str:
             title += 'search "%s"/' % self.rsearch_str
         return title
 
-    @functools.lru_cache()
     def format_item(self, item):
         s = super().format_item(item)
         ext = get_ext(item)
         if not (ext in AUDIO_EXTENSIONS or ext == 'm3u'):
             s += '/'
         return s
 
     def set_path(self, path, prev=None):
         if path != self.path:
             self.path = path
             os.chdir(path)
             relpath.cache_clear()
-            self.format_item.cache_clear()
             self.search_cache = []
         self.all_items = []
         self.rsearch_str = ''
 
         for p, ext, is_dir in listdir(path):
             if is_dir or ext == 'm3u' or ext in AUDIO_EXTENSIONS:
                 self.all_items.append(p)
@@ -456,36 +469,35 @@
                     self.items.append(path)
         else:
             self.items = self.all_items
 
         self.rsearch_str = query
         self.set_cursor(self.cursor)
 
+    def activate(self, item):
+        ext = item.rsplit('.', 1)[-1]
+        if os.path.isdir(item):
+            self.set_path(item)
+        elif ext in AUDIO_EXTENSIONS:
+            playlist.active = -1
+            player.play(item)
+        elif ext == 'm3u':
+            playlist.load(item)
+            app.toggle_tabs()
+
     def process_key(self, key):
         if key == 'a':
-            if not self.items:
-                return True
-            if playlist.add(self.items[self.cursor]):
+            if self.items and playlist.add(self.items[self.cursor]):
                 self.move_cursor(1)
         elif key == 's':
             app.input.start('search: ', on_input=self.filter)
             self.filter(self.rsearch_str)
         elif key == '\n':
-            if not self.items:
-                return True
-            item = self.items[self.cursor]
-            ext = item.rsplit('.', 1)[-1]
-            if os.path.isdir(item):
-                self.set_path(item)
-            elif ext in AUDIO_EXTENSIONS:
-                playlist.active = -1
-                player.play(item)
-            elif ext == 'm3u':
-                playlist.load(item)
-                app.toggle_tabs()
+            if self.items:
+                self.activate(self.items[self.cursor])
         elif key == curses.KEY_BACKSPACE:
             if self.rsearch_str:
                 self.set_path(self.path)
             else:
                 self.set_path(os.path.dirname(self.path), prev=self.path)
         else:
             return super().process_key(key)
@@ -586,33 +598,33 @@
         try:
             return self.items[self.active]
         except IndexError:
             self.active = -1
 
     def add_dir(self, path):
         count = 0
-        for p, ext, is_dir in listdir(path):
+        for p, _ext, _is_dir in listdir(path):
             count += self.add(p, recursive=True)
         return count
 
     def add_playlist(self, path):
         count = 0
         dirname = os.path.dirname(path)
         with open(path, errors='replace') as fh:
-            for line in fh:
-                line = line.strip()
+            for _line in fh:
+                line = _line.strip()
                 if not line or line[0] == '#':
                     continue
                 if not re.match(r'^(/|https?://)', line):
                     line = os.path.join(dirname, line)
                 self.items.append(line)
                 count += 1
         return count
 
-    def add(self, path, recursive=False):
+    def add(self, path, *, recursive=False):
         ext = path.rsplit('.', 1)[-1]
         if os.path.isdir(path):
             return self.add_dir(path)
         elif ext == 'm3u' and not recursive:
             return self.add_playlist(path)
         elif ext in AUDIO_EXTENSIONS:
             self.items.append(path)
@@ -629,18 +641,18 @@
     def write(self, path):
         try:
             with open(path, 'w') as fh:
                 for item in self.items:
                     fh.write('%s\n' % item)
                 self.path = path
                 self.items_written = self.items.copy()
-        except IOError:
+        except OSError:
             pass
 
-    def process_key(self, key):
+    def process_key(self, key):  # noqa: C901
         if key == 'm':
             self.move_item(1)
         elif key == 'M':
             self.move_item(-1)
         elif key == 'd':
             self.remove_item()
         elif key == 'D':
@@ -720,43 +732,44 @@
         elif self.tab == helplist:
             status = __version__
         elif player.is_playing:
             status = 'Playing %s' % player.get_title()
         else:
             status = ''
 
-        counter = '%s / %s' % (
+        counter = ' / '.join([
             format_time(player.position),
             format_time(player.length),
-        )
+        ])
         yield space_between(status, counter, self.cols)
 
-    def render(self, force=False):
+    def render(self, *, force=False):
         lines = list(self._render())
         try:
             for i, line in enumerate(lines):
                 if (
                     not force
                     and len(self.old_lines) > i
                     and line == self.old_lines[i]
                 ):
                     continue
                 screen.move(i, 0)
                 screen.clrtoeol()
                 if isinstance(line, str):
-                    line = (line, 0)
-                screen.insstr(i, 0, *line)
+                    screen.insstr(i, 0, line, 0)
+                else:
+                    screen.insstr(i, 0, *line)
             # make sure cursor is in a meaningful position for a11y
             screen.move(self.tab.cursor - self.tab.position + 2, 0)
             screen.refresh()
         except curses.error:
             pass
         self.old_lines = lines
 
-    def process_key(self, key):
+    def process_key(self, key):  # noqa: C901
         if self.input.process_key(key):
             pass
         elif self.tab.process_key(key):
             pass
         elif key in ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']:
             player.set_volume(int(key, 10) * 11)
         elif key == curses.KEY_RIGHT:
@@ -786,15 +799,15 @@
             sel.register(self.resize_in, selectors.EVENT_READ)
             sel.register(player.socket, selectors.EVENT_READ)
 
             while True:
                 player.finish_seek()
 
                 timeout = 0.5 if player.is_playing else None
-                for key, mask in sel.select(timeout):
+                for key, _mask in sel.select(timeout):
                     if key.fileobj is self.resize_in:
                         os.read(self.resize_in, 8)
                         self.on_resize()
                         self.render(force=True)
                     elif key.fileobj is sys.stdin:
                         self.process_key(screen.get_wch())
                     elif key.fileobj is player.socket:
@@ -812,18 +825,18 @@
 helplist = HelpList()
 app = Application()
 
 screen = curses.initscr()
 
 
 def main():
-    screen.keypad(True)
+    screen.keypad(True)  # noqa: FBT003
     curses.cbreak()
     curses.noecho()
-    curses.meta(True)
+    curses.meta(True)  # noqa: FBT003
     curses.curs_set(0)
 
     signal.signal(signal.SIGWINCH, resize)
 
     try:
         with enable_ctrl_keys():
             app.run()
```

### Comparing `cplay-ng-5.2.0/cplay_ng.egg-info/PKG-INFO` & `cplay_ng-5.3.0/cplay_ng.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: cplay-ng
-Version: 5.2.0
+Version: 5.3.0
 Summary: A simple curses audio player
-Home-page: https://github.com/xi/cplay-ng
-Author: Ulf Betlehem
-Author-email: flu@iki.fi
-Maintainer: Tobias Bengfort
-Maintainer-email: tobias.bengfort@posteo.de
+Author-email: Ulf Betlehem <flu@iki.fi>
+Maintainer-email: Tobias Bengfort <tobias.bengfort@posteo.de>
 License: GPLv2+
+Project-URL: Homepage, https://github.com/xi/cplay-ng
+Keywords: music-player,curses
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Topic :: Multimedia :: Sound/Audio :: Players
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Description
 -----------
 
 ``cplay`` is a minimalist music player with a textual user interface
```


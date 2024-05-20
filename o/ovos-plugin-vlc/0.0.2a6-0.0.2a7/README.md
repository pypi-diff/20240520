# Comparing `tmp/ovos_plugin_vlc-0.0.2a6-py3-none-any.whl.zip` & `tmp/ovos_plugin_vlc-0.0.2a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7846 bytes, number of entries: 8
--rw-r--r--  2.0 unx     5875 b- defN 24-May-11 03:25 ovos_plugin_vlc/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 24-May-11 03:25 ovos_plugin_vlc/version.py
--rw-r--r--  2.0 unx    11349 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/LICENSE
--rw-r--r--  2.0 unx      348 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/WHEEL
--rw-r--r--  2.0 unx      147 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      708 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/RECORD
-8 files, 18712 bytes uncompressed, 6592 bytes compressed:  64.8%
+Zip file size: 7868 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-20 04:38 ovos_plugin_vlc/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-May-20 04:38 ovos_plugin_vlc/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 24-May-20 04:38 ovos_plugin_vlc-0.0.2a7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      348 b- defN 24-May-20 04:38 ovos_plugin_vlc-0.0.2a7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 04:38 ovos_plugin_vlc-0.0.2a7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      147 b- defN 24-May-20 04:38 ovos_plugin_vlc-0.0.2a7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-May-20 04:38 ovos_plugin_vlc-0.0.2a7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      708 b- defN 24-May-20 04:38 ovos_plugin_vlc-0.0.2a7.dist-info/RECORD
+8 files, 18763 bytes uncompressed, 6614 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_plugin_vlc/__init__.py
 Comment: 
 
 Filename: ovos_plugin_vlc/version.py
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a6.dist-info/LICENSE
+Filename: ovos_plugin_vlc-0.0.2a7.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a6.dist-info/METADATA
+Filename: ovos_plugin_vlc-0.0.2a7.dist-info/METADATA
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a6.dist-info/WHEEL
+Filename: ovos_plugin_vlc-0.0.2a7.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a6.dist-info/entry_points.txt
+Filename: ovos_plugin_vlc-0.0.2a7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a6.dist-info/top_level.txt
+Filename: ovos_plugin_vlc-0.0.2a7.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a6.dist-info/RECORD
+Filename: ovos_plugin_vlc-0.0.2a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_plugin_vlc/__init__.py

```diff
@@ -23,18 +23,17 @@
                                      self.queue_ended, 0)
         self.vlc_events.event_attach(vlc.EventType.MediaPlayerEncounteredError,
                                      self.handle_vlc_error, None)
 
         self.config = config
         self.bus = bus
         self.name = name
-        self.normal_volume = None
+        self.normal_volume = 100
         self.low_volume = self.config.get('low_volume', 30)
         self._playback_time = 0
-        self.player.audio_set_volume(100)
         self._last_sync = 0
 
     ###################
     # vlc internals
     def handle_vlc_error(self, data, other):
         self.ocp_error()
 
@@ -100,18 +99,19 @@
         self.player.set_pause(1)
 
     def resume(self):
         """ Resume paused playback. """
         self.player.set_pause(0)
 
     def lower_volume(self):
+        self.normal_volume = self.player.audio_get_volume()  # remember volume
         self.player.audio_set_volume(self.low_volume)
 
     def restore_volume(self):
-        self.player.audio_set_volume(100)
+        self.player.audio_set_volume(self.normal_volume)
 
     def track_info(self):
         """ Extract info of current track. """
         ret = {}
         t = self.player.get_media()
         if t:
             ret['album'] = t.get_meta(vlc.Meta.Album)
```

## ovos_plugin_vlc/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 2
-VERSION_ALPHA = 6
+VERSION_ALPHA = 7
 # END_VERSION_BLOCK
```

## Comparing `ovos_plugin_vlc-0.0.2a6.dist-info/LICENSE` & `ovos_plugin_vlc-0.0.2a7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_plugin_vlc-0.0.2a6.dist-info/RECORD` & `ovos_plugin_vlc-0.0.2a7.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ovos_plugin_vlc/__init__.py,sha256=mvECoadIeiSEbhnvMbbuIB5k2O3ZrhXbPaY9KMAGssI,5875
-ovos_plugin_vlc/version.py,sha256=di5Z7K6nH7UaPd1uj2qxhcT0JK5MyN10xTqgznSb2b4,177
-ovos_plugin_vlc-0.0.2a6.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_plugin_vlc-0.0.2a6.dist-info/METADATA,sha256=ySqWC204tpwQy38AePv7SU_EhceQIXmJz1m_3devzj4,348
-ovos_plugin_vlc-0.0.2a6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ovos_plugin_vlc-0.0.2a6.dist-info/entry_points.txt,sha256=yyfZ-8jm_iKva1qJ1CfxkKRNgPnUeP6gveK1UiWx6eE,147
-ovos_plugin_vlc-0.0.2a6.dist-info/top_level.txt,sha256=Eh9jwKJdrdwsCh7iQkzQqn69pbD1-EkVK3Ud1mTDxxU,16
-ovos_plugin_vlc-0.0.2a6.dist-info/RECORD,,
+ovos_plugin_vlc/__init__.py,sha256=3zwYnkteb218j65unmmfwiyRhBsf1ODWYiL7JdexTSE,5926
+ovos_plugin_vlc/version.py,sha256=nzY0vok5lo9ShBsSEyRIdOa2hpDX9Spl94J4BX1dI9Y,177
+ovos_plugin_vlc-0.0.2a7.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_plugin_vlc-0.0.2a7.dist-info/METADATA,sha256=6I7AasQolQ_8efmtflynDzL1OD9Bpoj3U-romLSgN_4,348
+ovos_plugin_vlc-0.0.2a7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ovos_plugin_vlc-0.0.2a7.dist-info/entry_points.txt,sha256=yyfZ-8jm_iKva1qJ1CfxkKRNgPnUeP6gveK1UiWx6eE,147
+ovos_plugin_vlc-0.0.2a7.dist-info/top_level.txt,sha256=Eh9jwKJdrdwsCh7iQkzQqn69pbD1-EkVK3Ud1mTDxxU,16
+ovos_plugin_vlc-0.0.2a7.dist-info/RECORD,,
```


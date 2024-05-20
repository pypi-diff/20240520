# Comparing `tmp/gamdl-2.2.3.tar.gz` & `tmp/gamdl-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.2.3.tar` & `gamdl-2.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       17 2024-05-09 23:19:48.259539 gamdl-2.2.3/.github/FUNDING.yml
--rw-r--r--   0        0        0     1137 2024-05-09 23:19:48.259539 gamdl-2.2.3/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-05-09 23:19:48.259539 gamdl-2.2.3/.gitignore
--rw-r--r--   0        0        0    12216 2024-05-09 23:19:48.259539 gamdl-2.2.3/README.md
--rw-r--r--   0        0        0       22 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/__main__.py
--rw-r--r--   0        0        0     8853 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26865 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/cli.py
--rw-r--r--   0        0        0     5570 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/constants.py
--rw-r--r--   0        0        0    16263 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader.py
--rw-r--r--   0        0        0    10263 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2202 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader_post.py
--rw-r--r--   0        0        0    14146 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader_song.py
--rw-r--r--   0        0        0     4016 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      797 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-05-09 23:19:48.259539 gamdl-2.2.3/gamdl/models.py
--rw-r--r--   0        0        0      593 2024-05-09 23:19:48.259539 gamdl-2.2.3/pyproject.toml
--rw-r--r--   0        0        0       56 2024-05-09 23:19:48.259539 gamdl-2.2.3/requirements.txt
--rw-r--r--   0        0        0    12724 1970-01-01 00:00:00.000000 gamdl-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-05-20 18:54:11.800668 gamdl-2.2.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1137 2024-05-20 18:54:11.800668 gamdl-2.2.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-05-20 18:54:11.800668 gamdl-2.2.4/.gitignore
+-rw-r--r--   0        0        0    12354 2024-05-20 18:54:11.800668 gamdl-2.2.4/README.md
+-rw-r--r--   0        0        0       22 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/__main__.py
+-rw-r--r--   0        0        0     8791 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    27001 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/cli.py
+-rw-r--r--   0        0        0     5570 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/constants.py
+-rw-r--r--   0        0        0    16263 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader.py
+-rw-r--r--   0        0        0    10340 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2294 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    14146 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     4016 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      797 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-05-20 18:54:11.800668 gamdl-2.2.4/gamdl/models.py
+-rw-r--r--   0        0        0      576 2024-05-20 18:54:11.804668 gamdl-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-05-20 18:54:11.804668 gamdl-2.2.4/requirements.txt
+-rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 gamdl-2.2.4/PKG-INFO
```

### Comparing `gamdl-2.2.3/.github/workflows/main.yml` & `gamdl-2.2.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.3/README.md` & `gamdl-2.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Glomatico's Apple Music Downloader
-A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts.
+A Python CLI app for downloading Apple Music songs/music videos/posts.
 
 **Discord Server:** https://discord.gg/aBjMEZ9tnq
 
 ## Features
 * Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
 * Download music videos up to 4K
 * Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
 * Highly customizable
 * Use artist links to download all of their albums or music videos
 
 ## Prerequisites
 * Python 3.8 or higher
-* The cookies file of your Apple Music account (requires an active subscription)
+* The cookies file of your Apple Music browser session (requires an active subscription)
     * You can get your cookies by using one of the following extensions on your browser of choice at the Apple Music website with your account signed in:
         * Firefox: https://addons.mozilla.org/addon/export-cookies-txt
         * Chromium based browsers: https://chrome.google.com/webstore/detail/gdocmgbfkjnnpapoeobnolbbkoibbcif
 * FFmpeg on your system PATH
     * Older versions of FFmpeg may not work.
     * Up to date binaries can be obtained from the links below:
         * Windows: https://github.com/AnimMouse/ffmpeg-stable-autobuild/releases
@@ -49,16 +49,22 @@
     gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1624945511"
     ```
 * Choose which albums or music videos to download from an artist
     ```bash
     gamdl "https://music.apple.com/us/artist/rick-astley/669771"
     ```
 
+### Interactive prompt controls
+* Arrow keys - Move selection
+* Space - Toggle selection
+* Ctrl + A - Select all
+* Enter - Confirm selection
+
 ## Configuration
-You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
+gamdl can be configured by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
 | Command line argument / Config file key                         | Description                                                                  | Default value                                |
 | --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
 | `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
 | `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
 | `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
 | `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs separated by newlines. | `false`                                      |
 | `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                                      |
@@ -67,15 +73,15 @@
 | `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
 | `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
 | `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
 | `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                                      |
 | `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Apple Music`                              |
 | `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
 | `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
-| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8dl-RE`                                |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                                |
 | `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                                 |
 | `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
 | `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                                     |
 | `--download-mode` / `download_mode`                             | Download mode.                                                               | `ytdlp`                                      |
 | `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                                     |
 | `--cover-format` / `cover_format`                               | Cover format.                                                                | `jpg`                                        |
 | `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.                        | `{album_artist}/{album}`                     |
@@ -181,13 +187,13 @@
 
 ### Synced lyrics formats
 The following synced lyrics formats are available:
 * `lrc`
 * `srt`
 * `ttml`
     * Native format for Apple Music synced lyrics.
-    * Highly unsupported by media players.
+    * Highly unsupported by most media players.
   
 ### Cover formats
 The following cover formats are available:
 * `jpg`
 * `png`
```

### Comparing `gamdl-2.2.3/gamdl/apple_music_api.py` & `gamdl-2.2.4/gamdl/apple_music_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,21 +165,20 @@
         )
         self._check_amp_api_response(response)
         return response.json()["data"][0]
 
     def get_playlist(
         self,
         playlist_id: str,
-        is_library: bool = False,
         limit_tracks: int = 300,
         extend: str = "extendedAssetUrls",
         fetch_all: bool = True,
     ) -> dict:
         response = self.session.get(
-            f"{self.AMP_API_URL}/v1/{'me' if is_library else 'catalog'}/{self.storefront}/playlists/{playlist_id}",
+            f"{self.AMP_API_URL}/v1/catalog/{self.storefront}/playlists/{playlist_id}",
             params={
                 "extend": extend,
                 "limit[tracks]": limit_tracks,
             },
         )
         self._check_amp_api_response(response)
         playlist = response.json()["data"][0]
```

### Comparing `gamdl-2.2.3/gamdl/cli.py` & `gamdl-2.2.4/gamdl/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,38 +521,40 @@
                             logger.debug("Getting decryption key")
                             decryption_key = downloader.get_decryption_key(
                                 stream_info.pssh, track["id"]
                             )
                         encrypted_path = downloader_song.get_encrypted_path(track["id"])
                         decrypted_path = downloader_song.get_decrypted_path(track["id"])
                         remuxed_path = downloader_song.get_remuxed_path(track["id"])
-                        logger.debug(f"Downloading to {encrypted_path}")
+                        logger.debug(f'Downloading to "{encrypted_path}"')
                         downloader.download(encrypted_path, stream_info.stream_url)
                         if codec_song in LEGACY_CODECS:
-                            logger.debug(f"Remuxing/Decrypting to {remuxed_path}")
+                            logger.debug(
+                                f'Decrypting/Remuxing to "{decrypted_path}"/"{remuxed_path}"'
+                            )
                             downloader_song_legacy.remux(
                                 encrypted_path,
                                 decrypted_path,
                                 remuxed_path,
                                 decryption_key,
                             )
                         else:
-                            logger.debug(f"Decrypting to {decrypted_path}")
+                            logger.debug(f'Decrypting to "{decrypted_path}"')
                             downloader_song.decrypt(
                                 encrypted_path, decrypted_path, decryption_key
                             )
-                            logger.debug(f"Remuxing to {final_path}")
+                            logger.debug(f'Remuxing to "{final_path}"')
                             downloader_song.remux(
                                 decrypted_path,
                                 remuxed_path,
                                 stream_info.codec,
                             )
                         logger.debug("Applying tags")
                         downloader.apply_tags(remuxed_path, tags, cover_url)
-                        logger.debug(f"Moving to {final_path}")
+                        logger.debug(f'Moving to "{final_path}"')
                         downloader.move_to_output_path(remuxed_path, final_path)
                     if no_synced_lyrics or not lyrics.synced:
                         pass
                     elif lyrics_synced_path.exists() and not overwrite:
                         logger.debug(
                             f'Synced lyrics already exists at "{lyrics_synced_path}", skipping'
                         )
@@ -624,73 +626,73 @@
                         )
                         decrypted_path_audio = (
                             downloader_music_video.get_decrypted_path_audio(track["id"])
                         )
                         remuxed_path = downloader_music_video.get_remuxed_path(
                             track["id"]
                         )
-                        logger.debug(f"Downloading video to {encrypted_path_video}")
+                        logger.debug(f'Downloading video to "{encrypted_path_video}"')
                         downloader.download(
                             encrypted_path_video, stream_info_video.stream_url
                         )
-                        logger.debug(f"Downloading audio to {encrypted_path_audio}")
+                        logger.debug(f'Downloading audio to "{encrypted_path_audio}"')
                         downloader.download(
                             encrypted_path_audio, stream_info_audio.stream_url
                         )
-                        logger.debug(f"Decrypting video to {decrypted_path_video}")
+                        logger.debug(f'Decrypting video to "{decrypted_path_video}"')
                         downloader_music_video.decrypt(
                             encrypted_path_video,
                             decryption_key_video,
                             decrypted_path_video,
                         )
-                        logger.debug(f"Decrypting audio to {decrypted_path_audio}")
+                        logger.debug(f'Decrypting audio to "{decrypted_path_audio}"')
                         downloader_music_video.decrypt(
                             encrypted_path_audio,
                             decryption_key_audio,
                             decrypted_path_audio,
                         )
-                        logger.debug(f"Remuxing to {remuxed_path}")
+                        logger.debug(f'Remuxing to "{remuxed_path}"')
                         downloader_music_video.remux(
                             decrypted_path_video,
                             decrypted_path_audio,
                             remuxed_path,
                             stream_info_video.codec,
                             stream_info_audio.codec,
                         )
                         logger.debug("Applying tags")
                         downloader.apply_tags(remuxed_path, tags, cover_url)
-                        logger.debug(f"Moving to {final_path}")
+                        logger.debug(f'Moving to "{final_path}"')
                         downloader.move_to_output_path(remuxed_path, final_path)
                     if not save_cover:
                         pass
                     elif cover_path.exists() and not overwrite:
                         logger.debug(
                             f'Cover already exists at "{cover_path}", skipping'
                         )
                     else:
                         logger.debug(f'Saving cover to "{cover_path}"')
                         downloader.save_cover(cover_path, cover_url)
                 elif track["type"] == "uploaded-videos":
                     stream_url = downloader_post.get_stream_url(track)
                     tags = downloader_post.get_tags(track)
-                    temp_path = downloader_post.get_temp_path(track["id"])
+                    post_temp_path = downloader_post.get_post_temp_path(track["id"])
                     final_path = downloader.get_final_path(tags, ".m4v")
                     cover_path = downloader_music_video.get_cover_path(final_path)
                     cover_url = downloader.get_cover_url(track)
                     if final_path.exists() and not overwrite:
                         logger.warning(
                             f'({queue_progress}) Post video already exists at "{final_path}", skipping'
                         )
                     else:
-                        logger.debug(f"Downloading to {final_path}")
-                        downloader.download_ytdlp(temp_path, stream_url)
+                        logger.debug(f'Downloading to "{post_temp_path}"')
+                        downloader.download_ytdlp(post_temp_path, stream_url)
                         logger.debug("Applying tags")
-                        downloader.apply_tags(temp_path, tags, cover_url)
-                        logger.debug(f"Moving to {final_path}")
-                        downloader.move_to_output_path(temp_path, final_path)
+                        downloader.apply_tags(post_temp_path, tags, cover_url)
+                        logger.debug(f'Moving to "{final_path}"')
+                        downloader.move_to_output_path(post_temp_path, final_path)
                     if not save_cover:
                         pass
                     elif cover_path.exists() and not overwrite:
                         logger.debug(
                             f'Cover already exists at "{cover_path}", skipping'
                         )
                     else:
```

### Comparing `gamdl-2.2.3/gamdl/constants.py` & `gamdl-2.2.4/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.3/gamdl/downloader.py` & `gamdl-2.2.4/gamdl/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def __init__(
         self,
         apple_music_api: AppleMusicApi,
         itunes_api: ItunesApi,
         output_path: Path = Path("./Apple Music"),
         temp_path: Path = Path("./temp"),
         wvd_path: Path = None,
-        nm3u8dlre_path: str = "N_m3u8dl-RE",
+        nm3u8dlre_path: str = "N_m3u8DL-RE",
         mp4decrypt_path: str = "mp4decrypt",
         ffmpeg_path: str = "ffmpeg",
         mp4box_path: str = "MP4Box",
         download_mode: DownloadMode = DownloadMode.YTDLP,
         remux_mode: RemuxMode = RemuxMode.FFMPEG,
         cover_format: CoverFormat = CoverFormat.JPG,
         template_folder_album: str = "{album_artist}/{album}",
```

### Comparing `gamdl-2.2.3/gamdl/downloader_music_video.py` & `gamdl-2.2.4/gamdl/downloader_music_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import re
 import subprocess
 import urllib.parse
 from pathlib import Path
 
 import m3u8
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
@@ -163,14 +162,15 @@
             "artist": metadata_itunes[0]["artistName"],
             "artist_id": int(metadata_itunes[0]["artistId"]),
             "copyright": itunes_page.get("copyright"),
             "date": self.downloader.sanitize_date(metadata_itunes[0]["releaseDate"]),
             "genre": metadata_itunes[0]["primaryGenreName"],
             "genre_id": int(itunes_page["genres"][0]["genreId"]),
             "media_type": 6,
+            "storefront": int(self.downloader.itunes_api.storefront_id.split("-")[0]),
             "title": metadata_itunes[0]["trackCensoredName"],
             "title_id": int(metadata["id"]),
         }
         if metadata_itunes[0]["trackExplicitness"] == "notExplicit":
             tags["rating"] = 0
         elif metadata_itunes[0]["trackExplicitness"] == "explicit":
             tags["rating"] = 1
```

### Comparing `gamdl-2.2.3/gamdl/downloader_post.py` & `gamdl-2.2.4/gamdl/downloader_post.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,11 +63,12 @@
     def get_tags(self, metadata: dict) -> list:
         attributes = metadata["attributes"]
         return {
             "artist": attributes["artistName"],
             "date": self.downloader.sanitize_date(attributes["uploadDate"]),
             "title": attributes["name"],
             "title_id": int(metadata["id"]),
+            "storefront": int(self.downloader.itunes_api.storefront_id.split("-")[0]),
         }
 
-    def get_temp_path(self, track_id: str) -> Path:
+    def get_post_temp_path(self, track_id: str) -> Path:
         return self.downloader.temp_path / f"{track_id}_temp.m4v"
```

### Comparing `gamdl-2.2.3/gamdl/downloader_song.py` & `gamdl-2.2.4/gamdl/downloader_song.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.3/gamdl/downloader_song_legacy.py` & `gamdl-2.2.4/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.3/gamdl/enums.py` & `gamdl-2.2.4/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.3/gamdl/hardcoded_wvd.py` & `gamdl-2.2.4/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.3/gamdl/itunes_api.py` & `gamdl-2.2.4/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2.3/pyproject.toml` & `gamdl-2.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gamdl"
-description = "A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts."
+description = "A Python CLI app for downloading Apple Music songs/music videos/posts."
 requires-python = ">=3.8"
 authors = [{ name = "glomatico" }]
 dependencies = [
     "ciso8601",
     "click",
     "inquirerpy",
     "m3u8",
```

### Comparing `gamdl-2.2.3/PKG-INFO` & `gamdl-2.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.2.3
-Summary: A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts.
+Version: 2.2.4
+Summary: A Python CLI app for downloading Apple Music songs/music videos/posts.
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: inquirerpy
 Requires-Dist: m3u8
 Requires-Dist: pywidevine
 Requires-Dist: pyyaml
 Requires-Dist: yt-dlp
 Project-URL: homepage, https://github.com/glomatico/gamdl
 Project-URL: repository, https://github.com/glomatico/gamdl
 
 # Glomatico's Apple Music Downloader
-A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts.
+A Python CLI app for downloading Apple Music songs/music videos/posts.
 
 **Discord Server:** https://discord.gg/aBjMEZ9tnq
 
 ## Features
 * Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
 * Download music videos up to 4K
 * Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
 * Highly customizable
 * Use artist links to download all of their albums or music videos
 
 ## Prerequisites
 * Python 3.8 or higher
-* The cookies file of your Apple Music account (requires an active subscription)
+* The cookies file of your Apple Music browser session (requires an active subscription)
     * You can get your cookies by using one of the following extensions on your browser of choice at the Apple Music website with your account signed in:
         * Firefox: https://addons.mozilla.org/addon/export-cookies-txt
         * Chromium based browsers: https://chrome.google.com/webstore/detail/gdocmgbfkjnnpapoeobnolbbkoibbcif
 * FFmpeg on your system PATH
     * Older versions of FFmpeg may not work.
     * Up to date binaries can be obtained from the links below:
         * Windows: https://github.com/AnimMouse/ffmpeg-stable-autobuild/releases
@@ -66,16 +66,22 @@
     gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1624945511"
     ```
 * Choose which albums or music videos to download from an artist
     ```bash
     gamdl "https://music.apple.com/us/artist/rick-astley/669771"
     ```
 
+### Interactive prompt controls
+* Arrow keys - Move selection
+* Space - Toggle selection
+* Ctrl + A - Select all
+* Enter - Confirm selection
+
 ## Configuration
-You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
+gamdl can be configured by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
 | Command line argument / Config file key                         | Description                                                                  | Default value                                |
 | --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
 | `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
 | `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
 | `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
 | `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs separated by newlines. | `false`                                      |
 | `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                                      |
@@ -84,15 +90,15 @@
 | `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
 | `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
 | `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
 | `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                                      |
 | `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Apple Music`                              |
 | `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
 | `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
-| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8dl-RE`                                |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                                |
 | `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                                 |
 | `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
 | `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                                     |
 | `--download-mode` / `download_mode`                             | Download mode.                                                               | `ytdlp`                                      |
 | `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                                     |
 | `--cover-format` / `cover_format`                               | Cover format.                                                                | `jpg`                                        |
 | `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.                        | `{album_artist}/{album}`                     |
@@ -198,14 +204,14 @@
 
 ### Synced lyrics formats
 The following synced lyrics formats are available:
 * `lrc`
 * `srt`
 * `ttml`
     * Native format for Apple Music synced lyrics.
-    * Highly unsupported by media players.
+    * Highly unsupported by most media players.
   
 ### Cover formats
 The following cover formats are available:
 * `jpg`
 * `png`
```


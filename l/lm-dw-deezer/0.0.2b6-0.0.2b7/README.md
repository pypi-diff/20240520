# Comparing `tmp/lm_dw_deezer-0.0.2b6.tar.gz` & `tmp/lm_dw_deezer-0.0.2b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_dw_deezer-0.0.2b6.tar", max compression
+gzip compressed data, was "lm_dw_deezer-0.0.2b7.tar", max compression
```

## Comparing `lm_dw_deezer-0.0.2b6.tar` & `lm_dw_deezer-0.0.2b7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rwxr-xr-x   0        0        0      490 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/README.md
--rwxr-xr-x   0        0        0      195 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/__init__.py
--rwxr-xr-x   0        0        0      161 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/compressions/__init__.py
--rwxr-xr-x   0        0        0      404 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/compressions/gzip.py
--rwxr-xr-x   0        0        0      411 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/compressions/utils.py
--rwxr-xr-x   0        0        0     1058 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/compressions/zip.py
--rwxr-xr-x   0        0        0      856 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/compressions/zstd.py
--rwxr-xr-x   0        0        0      386 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/__init__.py
--rwxr-xr-x   0        0        0     2025 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/conf.py
--rwxr-xr-x   0        0        0     1027 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/enums.py
--rwxr-xr-x   0        0        0       98 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/image.py
--rwxr-xr-x   0        0        0      350 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/thread_func.py
--rwxr-xr-x   0        0        0      613 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/utils.py
--rw-r--r--   0        0        0       94 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/utils_infos.py
--rwxr-xr-x   0        0        0       73 2024-05-19 14:48:46.142499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/decrypt/__init__.py
--rwxr-xr-x   0        0        0     1331 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/decrypt/decryptor.py
--rwxr-xr-x   0        0        0     1355 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/decrypt/utils.py
--rw-r--r--   0        0        0      316 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/decrypt/utils_infos.py
--rwxr-xr-x   0        0        0     4424 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw.py
--rwxr-xr-x   0        0        0      170 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/__init__.py
--rwxr-xr-x   0        0        0     1816 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/album.py
--rwxr-xr-x   0        0        0     2223 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/dws.py
--rwxr-xr-x   0        0        0     1923 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/playlist.py
--rw-r--r--   0        0        0     1217 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/track.py
--rwxr-xr-x   0        0        0     1489 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/utils.py
--rw-r--r--   0        0        0       60 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/utils_infos.py
--rwxr-xr-x   0        0        0     5120 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_utils.py
--rwxr-xr-x   0        0        0      111 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/exceptions/__init__.py
--rwxr-xr-x   0        0        0      240 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/exceptions/no_be.py
--rwxr-xr-x   0        0        0      252 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/exceptions/no_stream_data.py
--rwxr-xr-x   0        0        0     8904 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/exes/cli.py
--rwxr-xr-x   0        0        0      648 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/exes/data_utils.py
--rwxr-xr-x   0        0        0     1165 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/exes/read_browsers_cookies.py
--rwxr-xr-x   0        0        0     1500 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/exes/utils.py
--rwxr-xr-x   0        0        0      238 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/generators/__init__.py
--rwxr-xr-x   0        0        0      743 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/generators/album.py
--rwxr-xr-x   0        0        0      778 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/generators/playlist.py
--rwxr-xr-x   0        0        0      743 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/generators/track.py
--rwxr-xr-x   0        0        0        0 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/graphql/__init__.py
--rwxr-xr-x   0        0        0     1502 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/graphql/queries.py
--rwxr-xr-x   0        0        0     1518 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/graphql/types.py
--rwxr-xr-x   0        0        0       78 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/logger/__init__.py
--rwxr-xr-x   0        0        0      386 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/logger/decorators.py
--rwxr-xr-x   0        0        0      165 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/logger/enums.py
--rwxr-xr-x   0        0        0     1637 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/logger/log.py
--rwxr-xr-x   0        0        0     1092 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/medjays/__init__.py
--rwxr-xr-x   0        0        0      109 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/py.typed
--rwxr-xr-x   0        0        0       68 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/__init__.py
--rwxr-xr-x   0        0        0      838 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/helpers.py
--rwxr-xr-x   0        0        0     3421 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/tag_flac.py
--rwxr-xr-x   0        0        0     4609 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/tag_mp3.py
--rwxr-xr-x   0        0        0     2710 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/tag_track.py
--rwxr-xr-x   0        0        0      118 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/utils_infos.py
--rwxr-xr-x   0        0        0      234 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/__init__.py
--rwxr-xr-x   0        0        0    71135 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/data_utils.py
--rwxr-xr-x   0        0        0     2525 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/dw_album.py
--rwxr-xr-x   0        0        0     2641 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/dw_playlist.py
--rwxr-xr-x   0        0        0      619 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/dw_track.py
--rw-r--r--   0        0        0      106 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/enums.py
--rwxr-xr-x   0        0        0      393 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/pipe_ext/__init__.py
--rwxr-xr-x   0        0        0      362 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/pipe_ext/album.py
--rwxr-xr-x   0        0        0      368 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/pipe_ext/bases.py
--rwxr-xr-x   0        0        0     1753 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/pipe_ext/playlist.py
--rwxr-xr-x   0        0        0      106 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/pipe_ext/track.py
--rwxr-xr-x   0        0        0      285 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/pipe_ext/tracks.py
--rwxr-xr-x   0        0        0      198 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/track_out.py
--rwxr-xr-x   0        0        0      581 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/utils.py
--rw-r--r--   0        0        0      683 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/utils_image.py
--rwxr-xr-x   0        0        0     1406 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/lm_dw_deezer/utils.py
--rwxr-xr-x   0        0        0      826 2024-05-19 14:48:46.146499 lm_dw_deezer-0.0.2b6/pyproject.toml
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 lm_dw_deezer-0.0.2b6/PKG-INFO
+-rwxr-xr-x   0        0        0      490 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/README.md
+-rwxr-xr-x   0        0        0      195 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/__init__.py
+-rwxr-xr-x   0        0        0      161 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/compressions/__init__.py
+-rwxr-xr-x   0        0        0      404 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/compressions/gzip.py
+-rwxr-xr-x   0        0        0      411 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/compressions/utils.py
+-rwxr-xr-x   0        0        0     1058 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/compressions/zip.py
+-rwxr-xr-x   0        0        0      856 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/compressions/zstd.py
+-rwxr-xr-x   0        0        0      386 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/__init__.py
+-rwxr-xr-x   0        0        0     2025 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/conf.py
+-rwxr-xr-x   0        0        0     1027 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/enums.py
+-rwxr-xr-x   0        0        0       98 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/image.py
+-rwxr-xr-x   0        0        0      350 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/thread_func.py
+-rwxr-xr-x   0        0        0      613 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/utils.py
+-rw-r--r--   0        0        0       94 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/utils_infos.py
+-rwxr-xr-x   0        0        0       73 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/decrypt/__init__.py
+-rwxr-xr-x   0        0        0     1331 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/decrypt/decryptor.py
+-rwxr-xr-x   0        0        0     1355 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/decrypt/utils.py
+-rw-r--r--   0        0        0      316 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/decrypt/utils_infos.py
+-rwxr-xr-x   0        0        0     4424 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw.py
+-rwxr-xr-x   0        0        0      170 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/__init__.py
+-rwxr-xr-x   0        0        0     1816 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/album.py
+-rwxr-xr-x   0        0        0     2223 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/dws.py
+-rwxr-xr-x   0        0        0     1923 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/playlist.py
+-rw-r--r--   0        0        0     1217 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/track.py
+-rwxr-xr-x   0        0        0     1489 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/utils.py
+-rw-r--r--   0        0        0       60 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/utils_infos.py
+-rwxr-xr-x   0        0        0     5120 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_utils.py
+-rwxr-xr-x   0        0        0      111 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/exceptions/__init__.py
+-rwxr-xr-x   0        0        0      240 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/exceptions/no_be.py
+-rwxr-xr-x   0        0        0      252 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/exceptions/no_stream_data.py
+-rwxr-xr-x   0        0        0     8904 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/exes/cli.py
+-rwxr-xr-x   0        0        0      648 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/exes/data_utils.py
+-rwxr-xr-x   0        0        0     1165 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/exes/read_browsers_cookies.py
+-rwxr-xr-x   0        0        0     1500 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/exes/utils.py
+-rwxr-xr-x   0        0        0      238 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/generators/__init__.py
+-rwxr-xr-x   0        0        0      743 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/generators/album.py
+-rwxr-xr-x   0        0        0      778 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/generators/playlist.py
+-rwxr-xr-x   0        0        0      743 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/generators/track.py
+-rwxr-xr-x   0        0        0        0 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/graphql/__init__.py
+-rwxr-xr-x   0        0        0     1502 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/graphql/queries.py
+-rwxr-xr-x   0        0        0     1518 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/graphql/types.py
+-rwxr-xr-x   0        0        0       78 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/logger/__init__.py
+-rwxr-xr-x   0        0        0      386 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/logger/decorators.py
+-rwxr-xr-x   0        0        0      165 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/logger/enums.py
+-rwxr-xr-x   0        0        0     1637 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/logger/log.py
+-rwxr-xr-x   0        0        0     1092 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/medjays/__init__.py
+-rwxr-xr-x   0        0        0      109 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/py.typed
+-rwxr-xr-x   0        0        0       68 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/__init__.py
+-rwxr-xr-x   0        0        0      838 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/helpers.py
+-rwxr-xr-x   0        0        0     3421 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/tag_flac.py
+-rwxr-xr-x   0        0        0     4609 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/tag_mp3.py
+-rwxr-xr-x   0        0        0     2710 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/tag_track.py
+-rwxr-xr-x   0        0        0      118 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/utils_infos.py
+-rwxr-xr-x   0        0        0      234 2024-05-19 15:41:01.018102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/__init__.py
+-rwxr-xr-x   0        0        0    71135 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/data_utils.py
+-rwxr-xr-x   0        0        0     2490 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/dw_album.py
+-rwxr-xr-x   0        0        0     2606 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/dw_playlist.py
+-rwxr-xr-x   0        0        0      619 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/dw_track.py
+-rw-r--r--   0        0        0      106 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/enums.py
+-rwxr-xr-x   0        0        0      393 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/pipe_ext/__init__.py
+-rwxr-xr-x   0        0        0      362 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/pipe_ext/album.py
+-rwxr-xr-x   0        0        0      368 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/pipe_ext/bases.py
+-rwxr-xr-x   0        0        0     1753 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/pipe_ext/playlist.py
+-rwxr-xr-x   0        0        0      106 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/pipe_ext/track.py
+-rwxr-xr-x   0        0        0      285 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/pipe_ext/tracks.py
+-rwxr-xr-x   0        0        0      198 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/track_out.py
+-rwxr-xr-x   0        0        0      581 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/utils.py
+-rw-r--r--   0        0        0      683 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/utils_image.py
+-rwxr-xr-x   0        0        0     1406 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/lm_dw_deezer/utils.py
+-rwxr-xr-x   0        0        0      826 2024-05-19 15:41:01.022102 lm_dw_deezer-0.0.2b7/pyproject.toml
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 lm_dw_deezer-0.0.2b7/PKG-INFO
```

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/compressions/zip.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/compressions/zip.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/compressions/zstd.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/compressions/zstd.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/conf.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/conf.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/enums.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/enums.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/config/utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/config/utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/decrypt/decryptor.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/decrypt/decryptor.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/decrypt/utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/decrypt/utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/album.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/album.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/dws.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/dws.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/playlist.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/playlist.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/track.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/track.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_helpers/utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/dw_utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/dw_utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/exes/cli.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/exes/cli.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/exes/data_utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/exes/data_utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/exes/read_browsers_cookies.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/exes/read_browsers_cookies.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/exes/utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/exes/utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/generators/album.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/generators/album.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/generators/playlist.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/generators/playlist.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/generators/track.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/generators/track.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/graphql/queries.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/graphql/queries.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/graphql/types.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/graphql/types.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/logger/log.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/logger/log.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/medjays/__init__.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/medjays/__init__.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/helpers.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/helpers.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/tag_flac.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/tag_flac.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/tag_mp3.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/tag_mp3.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/tagger/tag_track.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/tagger/tag_track.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/data_utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/data_utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/dw_album.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/dw_album.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,14 @@
 
 	def download_undownloaded_thread(self, thread_func: Thread_Func) -> None:
 		threads: list[DW_Medjay] = []
 		event = Event()
 		workers = thread_func.WORKERS
 
 		for track in self.get_undownloaded():
-			self.statuses[track]['helper']
-
 			if workers == 0:
 				wait_threads(threads)
 
 				if event.is_set():
 					break
 
 				workers = thread_func.WORKERS
```

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/dw_playlist.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/dw_playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,14 @@
 
 	def download_undownloaded_thread(self, thread_func: Thread_Func) -> None:
 		threads: list[DW_Medjay] = []
 		event = Event()
 		workers = thread_func.WORKERS
 
 		for track in self.get_undownloaded():
-			self.statuses[track]['helper']
-
 			if workers == 0:
 				wait_threads(threads)
 
 				if event.is_set():
 					break
 
 				workers = thread_func.WORKERS
```

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/dw_track.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/dw_track.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/pipe_ext/playlist.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/pipe_ext/playlist.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/types/utils_image.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/types/utils_image.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/lm_dw_deezer/utils.py` & `lm_dw_deezer-0.0.2b7/lm_dw_deezer/utils.py`

 * *Files identical despite different names*

### Comparing `lm_dw_deezer-0.0.2b6/pyproject.toml` & `lm_dw_deezer-0.0.2b7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lm-dw-deezer"
-version = "0.0.2b06"
+version = "0.0.2b07"
 description = "Liberum Melodian Library for making easy tracks downloading from Deezer"
 authors = ["An0nimia <an0nimia@protonmail.com>"]
 license = "CC BY 4.0"
 readme = "README.md"
 repository = "https://github.com/An0nimia/lm_dw_deezer"
```

### Comparing `lm_dw_deezer-0.0.2b6/PKG-INFO` & `lm_dw_deezer-0.0.2b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-dw-deezer
-Version: 0.0.2b6
+Version: 0.0.2b7
 Summary: Liberum Melodian Library for making easy tracks downloading from Deezer
 Home-page: https://github.com/An0nimia/lm_dw_deezer
 License: CC BY 4.0
 Author: An0nimia
 Author-email: an0nimia@protonmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
```


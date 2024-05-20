# Comparing `tmp/api_deezer_full-0.0.1b36.tar.gz` & `tmp/api_deezer_full-0.0.1b37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_deezer_full-0.0.1b36.tar", max compression
+gzip compressed data, was "api_deezer_full-0.0.1b37.tar", max compression
```

## Comparing `api_deezer_full-0.0.1b36.tar` & `api_deezer_full-0.0.1b37.tar`

### file list

```diff
@@ -1,65 +1,61 @@
--rwxr-xr-x   0        0        0       48 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/README.md
--rwxr-xr-x   0        0        0      200 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/README.md
--rwxr-xr-x   0        0        0      195 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/__init__.py
--rwxr-xr-x   0        0        0       47 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/__init__.py
--rwxr-xr-x   0        0        0     4632 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/api.py
--rwxr-xr-x   0        0        0      104 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/decorators/__init__.py
--rwxr-xr-x   0        0        0     3049 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/decorators/link.py
--rwxr-xr-x   0        0        0      535 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/decorators/login.py
--rwxr-xr-x   0        0        0       65 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/exceptions/__init__.py
--rwxr-xr-x   0        0        0      197 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/exceptions/arl_invalid.py
--rwxr-xr-x   0        0        0        0 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/exceptions/data_exceded.py
--rwxr-xr-x   0        0        0      447 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/exceptions/track_404.py
--rwxr-xr-x   0        0        0      389 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/__init__.py
--rwxr-xr-x   0        0        0      360 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/album.py
--rwxr-xr-x   0        0        0      507 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/artist.py
--rwxr-xr-x   0        0        0      668 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/contributor.py
--rwxr-xr-x   0        0        0      388 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/playlist.py
--rw-r--r--   0        0        0      142 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/search/__init__.py
--rw-r--r--   0        0        0      468 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/search/album.py
--rw-r--r--   0        0        0      435 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/search/artist.py
--rw-r--r--   0        0        0     1366 2024-03-10 13:58:25.808476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/search/playlist.py
--rw-r--r--   0        0        0      982 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/search/search.py
--rwxr-xr-x   0        0        0     2927 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/track.py
--rwxr-xr-x   0        0        0       60 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/gw/types/user.py
--rwxr-xr-x   0        0        0       53 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/__init__.py
--rwxr-xr-x   0        0        0     2475 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/api.py
--rwxr-xr-x   0        0        0       92 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/exceptions/__init__.py
--rwxr-xr-x   0        0        0      416 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/exceptions/insufficient_rights.py
--rwxr-xr-x   0        0        0      160 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/types/__init__.py
--rwxr-xr-x   0        0        0       89 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/types/aliases.py
--rwxr-xr-x   0        0        0       68 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/types/cipher.py
--rwxr-xr-x   0        0        0      513 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/types/media.py
--rwxr-xr-x   0        0        0      151 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/types/medias.py
--rwxr-xr-x   0        0        0       82 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/media/types/source.py
--rw-r--r--   0        0        0       54 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/mobile/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/mobile/api.py
--rw-r--r--   0        0        0        0 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/mobile/exceptions/__init__.py
--rw-r--r--   0        0        0      360 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/mobile/exceptions/bad_credentials.py
--rw-r--r--   0        0        0      325 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/mobile/utils.py
--rwxr-xr-x   0        0        0       51 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/__init__.py
--rwxr-xr-x   0        0        0     3242 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/api.py
--rwxr-xr-x   0        0        0       96 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/decorators/__init__.py
--rwxr-xr-x   0        0        0     2602 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/decorators/link.py
--rwxr-xr-x   0        0        0      548 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/decorators/login.py
--rwxr-xr-x   0        0        0        0 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/exceptions/__init__.py
--rwxr-xr-x   0        0        0        0 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/exceptions/data_exceded.py
--rwxr-xr-x   0        0        0      447 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/exceptions/track_404.py
--rwxr-xr-x   0        0        0        0 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/grapql/__init__.py
--rwxr-xr-x   0        0        0     2166 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/grapql/queries.py
--rwxr-xr-x   0        0        0     5056 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/grapql/types.py
--rwxr-xr-x   0        0        0      567 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/__init__.py
--rwxr-xr-x   0        0        0      362 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/album.py
--rwxr-xr-x   0        0        0      260 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/artist.py
--rwxr-xr-x   0        0        0     1771 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/bases.py
--rwxr-xr-x   0        0        0      323 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/contributor.py
--rwxr-xr-x   0        0        0       72 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/cover.py
--rwxr-xr-x   0        0        0      192 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/disk_info.py
--rwxr-xr-x   0        0        0      335 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/lyrics.py
--rwxr-xr-x   0        0        0     1101 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/media.py
--rwxr-xr-x   0        0        0      454 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/media_rights.py
--rwxr-xr-x   0        0        0     1360 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/playlist.py
--rwxr-xr-x   0        0        0       92 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/track.py
--rwxr-xr-x   0        0        0        0 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/api_deezer_full/py.typed
--rwxr-xr-x   0        0        0      398 2024-03-10 13:58:25.812476 api_deezer_full-0.0.1b36/pyproject.toml
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 api_deezer_full-0.0.1b36/PKG-INFO
+-rwxr-xr-x   0        0        0       48 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/README.md
+-rwxr-xr-x   0        0        0      200 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/README.md
+-rwxr-xr-x   0        0        0      195 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/__init__.py
+-rwxr-xr-x   0        0        0       50 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/__init__.py
+-rwxr-xr-x   0        0        0     4744 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/api.py
+-rwxr-xr-x   0        0        0       61 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/decorators/__init__.py
+-rwxr-xr-x   0        0        0      535 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/decorators/login.py
+-rwxr-xr-x   0        0        0       65 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/exceptions/__init__.py
+-rwxr-xr-x   0        0        0      197 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/exceptions/arl_invalid.py
+-rwxr-xr-x   0        0        0        0 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/exceptions/data_exceded.py
+-rwxr-xr-x   0        0        0      246 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/exceptions/track_404.py
+-rwxr-xr-x   0        0        0      389 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/__init__.py
+-rwxr-xr-x   0        0        0      351 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/album.py
+-rwxr-xr-x   0        0        0      507 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/artist.py
+-rwxr-xr-x   0        0        0      668 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/contributor.py
+-rwxr-xr-x   0        0        0      379 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/playlist.py
+-rw-r--r--   0        0        0      142 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/search/__init__.py
+-rw-r--r--   0        0        0      468 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/search/album.py
+-rw-r--r--   0        0        0      435 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/search/artist.py
+-rw-r--r--   0        0        0     1366 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/search/playlist.py
+-rw-r--r--   0        0        0      982 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/search/search.py
+-rwxr-xr-x   0        0        0     2927 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/track.py
+-rwxr-xr-x   0        0        0       60 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/types/user.py
+-rw-r--r--   0        0        0      765 2024-05-20 14:17:48.717461 api_deezer_full-0.0.1b37/api_deezer_full/gw/utils.py
+-rwxr-xr-x   0        0        0       53 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/__init__.py
+-rwxr-xr-x   0        0        0     2475 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/api.py
+-rwxr-xr-x   0        0        0       92 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/exceptions/__init__.py
+-rwxr-xr-x   0        0        0      416 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/exceptions/insufficient_rights.py
+-rwxr-xr-x   0        0        0      160 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/types/__init__.py
+-rwxr-xr-x   0        0        0       89 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/types/aliases.py
+-rwxr-xr-x   0        0        0       68 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/types/cipher.py
+-rwxr-xr-x   0        0        0      513 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/types/media.py
+-rwxr-xr-x   0        0        0      151 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/types/medias.py
+-rwxr-xr-x   0        0        0       82 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/media/types/source.py
+-rw-r--r--   0        0        0       54 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/mobile/__init__.py
+-rw-r--r--   0        0        0     2395 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/mobile/api.py
+-rw-r--r--   0        0        0        0 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/mobile/exceptions/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/mobile/exceptions/bad_credentials.py
+-rw-r--r--   0        0        0      325 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/mobile/utils.py
+-rwxr-xr-x   0        0        0       51 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/__init__.py
+-rwxr-xr-x   0        0        0     3236 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/api.py
+-rwxr-xr-x   0        0        0       62 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/decorators/__init__.py
+-rwxr-xr-x   0        0        0      548 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/decorators/login.py
+-rwxr-xr-x   0        0        0        0 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/grapql/__init__.py
+-rwxr-xr-x   0        0        0     2166 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/grapql/queries.py
+-rwxr-xr-x   0        0        0     5056 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/grapql/types.py
+-rwxr-xr-x   0        0        0      567 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/__init__.py
+-rwxr-xr-x   0        0        0      362 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/album.py
+-rwxr-xr-x   0        0        0      260 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/artist.py
+-rwxr-xr-x   0        0        0     1771 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/bases.py
+-rwxr-xr-x   0        0        0      323 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/contributor.py
+-rwxr-xr-x   0        0        0       72 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/cover.py
+-rwxr-xr-x   0        0        0      192 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/disk_info.py
+-rwxr-xr-x   0        0        0      335 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/lyrics.py
+-rwxr-xr-x   0        0        0     1101 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/media.py
+-rwxr-xr-x   0        0        0      454 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/media_rights.py
+-rwxr-xr-x   0        0        0     1360 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/playlist.py
+-rwxr-xr-x   0        0        0       92 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/track.py
+-rwxr-xr-x   0        0        0        0 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/api_deezer_full/py.typed
+-rwxr-xr-x   0        0        0      398 2024-05-20 14:17:48.721461 api_deezer_full-0.0.1b37/pyproject.toml
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 api_deezer_full-0.0.1b37/PKG-INFO
```

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/gw/api.py` & `api_deezer_full-0.0.1b37/api_deezer_full/gw/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 from requests import Session
 
 from datetime import datetime
 
 from json import dump as JSON_dump
 
+from .utils import check_errors
+from .decorators import check_login
 from .exceptions import Arl_Invalid
 
 from .types import (
 	Track, Album, User,
 	Playlist, Search
 )
 
-from .decorators import (
-	check_link, check_login
-)
-
 
 # https://e-cdn-files.dzcdn.net/cache/js/app-web.bb0399eb33362d783b36.js
 
 
 class API_GW:
 	__API_URL = 'https://www.deezer.com/ajax/gw-light.php' #?method=deezer.getUserData&input=3&api_version=1.0&api_token=&cid=465385533
 
@@ -64,20 +62,23 @@
 
 		resp = self._session.post(
 			url = self.__API_URL,
 			params = params,
 			json = json_data
 		).json()
 
+		check_errors(params, json_data)
+
 		return resp
 
 
-	@check_link(method = 'deezer.getUserData')
 	def gw_get_user_data_JSON(self) -> dict[str, Any]:
-		...
+		method = 'deezer.getUserData'
+
+		return self.gw_make_req(method)
 
 
 	def gw_get_user_data(self) -> User:
 		raise NotImplementedError('Sorry obj serialization at the moment sucks')
 		res = self.gw_get_user_data_JSON()
 
 
@@ -100,142 +101,147 @@
 		self.exp_license_token: datetime = datetime.fromtimestamp(
 			int(
 				user_data_json['USER']['OPTIONS']['expiration_timestamp']
 			)
 		)
 
 
-	def gw_get_track_lyric(self, id_track: int) -> dict[str, Any]:
+	def gw_get_track_lyric(self, id_track: int | str) -> dict[str, Any]:
 		method = 'song.getLyrics'
 
 		params = {
 			'SNG_ID': id_track
 		}
 
 		return self.gw_make_req(method, params)
 
 
-	@check_link(method = 'song.getData', type_media = 'track')
-	def gw_get_track_JSON(self, id_track: str) -> dict[str, Any]:
+	def gw_get_track_JSON(self, id_track: int | str) -> dict[str, Any]:
+		method = 'song.getData'
+
 		params = {
 			'SNG_ID': id_track
 		}
 
-		return params
+		return self.gw_make_req(method, params)
 
 
-	def gw_get_track(self, link: str) -> Track:
-		res = self.gw_get_track_JSON(link)
+	def gw_get_track(self, id_track: int | str) -> Track:
+		res = self.gw_get_track_JSON(id_track)
 
 		return Track.model_validate(res['results'])
 
 
-	def gw_get_tracks(self, id_tracks: list[int]) -> dict[str, Any]:
+	def gw_get_tracks(self, id_tracks: list[int | str]) -> dict[str, Any]:
 		method = 'song.getListData'
 
 		params = {
 			'sng_ids': id_tracks
 		}
 
 		return self.gw_make_req(method, params)
 
 
-	@check_link(method = 'song.getListByAlbum', type_media = 'album')
 	def gw_get_album_JSON(
 		self,
-		id_album: str,
+		id_album: int | str,
 		nb: int = -1,
 		start: int = 0
 	) -> dict[str, Any]:
 
+		method = 'song.getListByAlbum'
+
 		params = {
 			'alb_id': id_album,
 			'nb': nb,
 			'start': start
 		}
 
-		return params
+		return self.gw_make_req(method, params)
 
 
 	def gw_get_album(
 		self,
-		id_album: str,
+		id_album: int | str,
 		nb: int = -1,
 		start: int = 0
 	) -> Album:
 		res = self.gw_get_album_JSON(id_album, nb, start)
 
 		return Album.model_validate(res['results'])
 
 
-	@check_link(method = 'playlist.getSongs', type_media = 'playlist')
 	def gw_get_playlist_JSON(
 		self,
-		id_playlist: str,
+		id_playlist: int | str,
 		nb: int = -1,
 		start: int = 0
 	) -> dict[str, Any]:
 
+		method = 'playlist.getSongs'
+
 		params = {
 			'playlist_id': id_playlist,
 			'nb': nb,
 			'start': start
 		}
 
-		return params
+		return self.gw_make_req(method, params)
 
 
 	def gw_get_playlist(
 		self,
-		id_playlist: str,
+		id_playlist: int | str,
 		nb: int = -1,
 		start: int = 0
 	) -> Playlist:
 
 		res = self.gw_get_playlist_JSON(id_playlist, nb, start)
 
 		return Playlist.model_validate(res['results'])
 
 
-	@check_link(method = 'deezer.pageAlbum', type_media = 'album')
 	def gw_get_page_album_JSON(
 		self,
-		id_album: str,
+		id_album: int | str,
 		lang: str = 'en'
 	) -> dict[str, Any]:
 
+		method = 'deezer.pageAlbum'
+
 		params = {
 			'alb_id': id_album,
 			'lang': lang
 		}
 
-		return params
+		return self.gw_make_req(method, params)
 
 
-	@check_link(method = 'deezer.pageSearch')
 	def gw_search_JSON(
 		self,
 		query: str,
 		start: int = 0,
 		artist_suggest: bool = True,
 		nb: int = 40,
 		suggest: bool = True,
 		top_tracks: bool = True
 	) -> dict[str, Any]:
 
+		method = 'deezer.pageSearch'
+
 		params = {
 			'query': query,
 			'start': start,
 			'nb': nb,
 			'suggest' :suggest,
 			'artist_suggest': artist_suggest,
 			'top_tracks': top_tracks
 		}
 
-		return params
+		return self.gw_make_req(method, params)
 
 
 	def gw_search(
 		self,
 		query: str,
 		start: int = 0,
 		artist_suggest: bool = True,
```

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/gw/decorators/login.py` & `api_deezer_full-0.0.1b37/api_deezer_full/gw/decorators/login.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/gw/types/contributor.py` & `api_deezer_full-0.0.1b37/api_deezer_full/gw/types/contributor.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/gw/types/search/playlist.py` & `api_deezer_full-0.0.1b37/api_deezer_full/gw/types/search/playlist.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/gw/types/search/search.py` & `api_deezer_full-0.0.1b37/api_deezer_full/gw/types/search/search.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/gw/types/track.py` & `api_deezer_full-0.0.1b37/api_deezer_full/gw/types/track.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/media/api.py` & `api_deezer_full-0.0.1b37/api_deezer_full/media/api.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/media/types/media.py` & `api_deezer_full-0.0.1b37/api_deezer_full/media/types/media.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/mobile/api.py` & `api_deezer_full-0.0.1b37/api_deezer_full/mobile/api.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/pipe/api.py` & `api_deezer_full-0.0.1b37/api_deezer_full/pipe/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,18 @@
+from jwt import decode #pyright: ignore [reportUnknownVariableType]
 from typing import Any
-
 from requests import Session
 
-from jwt import decode
-
 from ..gw import API_GW
 
-from .decorators import (
-	check_link, check_login
-)
-
 from .grapql import queries
 from .grapql.types import get_introspection
 
+from .decorators import check_login
+
 from .types import (
 	Track, Album,
 	Lyrics, Playlist
 )
 
 
 class API_PIPE(API_GW):
@@ -60,15 +56,14 @@
 		}
 
 		res = self.pipe_make_req(params)
 
 		self.write_log(res, 'introspection.json')
 
 
-	@check_link(type_media = 'track')
 	def pipe_get_track_JSON(self, id_track: str) -> dict[str, Any]:
 		'''
 
 		Function for getting Track's infos in JSON format
 
 		'''
 
@@ -77,51 +72,54 @@
 
 	def pipe_get_track(self, link: str) -> Track:
 		res = self.pipe_get_track_JSON(link)
 
 		return Track.model_validate(res['data']['track'])
 
 
-	@check_link(type_media = 'album')
 	def pipe_get_album_JSON(self, id_album: str) -> dict[str, Any]:
 		'''
 
 		Function for getting Album's infos in JSON format
 
 		'''
 
-		return queries.get_album_query(id_album)
+		params = queries.get_album_query(id_album)
+
+		return self.pipe_make_req(params)
 
 
 	def pipe_get_album(self, link: str) -> Album:
 		res = self.pipe_get_album_JSON(link)
 
 		return Album.model_validate(res['data']['album'])
 
 
-	@check_link(type_media = 'playlist')
 	def pipe_get_playlist_JSON(self, id_playlist: str) -> dict[str, Any]:
 		'''
 
 		Function for getting Playlist's infos in JSON format
 
 		'''
 
-		return queries.get_playlist_query(id_playlist)
+		params = queries.get_playlist_query(id_playlist)
+
+		return self.pipe_make_req(params)
 
 
 	def pipe_get_playlist(self, link: str) -> Playlist:
 		res = self.pipe_get_playlist_JSON(link)
 		
 		return Playlist.model_validate(res['data']['playlist'])
 
 
-	@check_link(type_media = 'track_lyric')
 	def pipe_get_track_lyric_JSON(self, id_track: str) -> dict[str, Any]:
-		return queries.get_track_lyric_query(id_track)
+		params = queries.get_track_lyric_query(id_track)
+
+		return self.pipe_make_req(params)
 
 
 	def pipe_get_track_lyric(self, id_track: str) -> Lyrics:
 		res = self.pipe_get_track_lyric_JSON(id_track)
 
 		return Lyrics.model_validate(res['data']['track']['lyrics'])
```

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/pipe/decorators/login.py` & `api_deezer_full-0.0.1b37/api_deezer_full/pipe/decorators/login.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/pipe/grapql/queries.py` & `api_deezer_full-0.0.1b37/api_deezer_full/pipe/grapql/queries.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/pipe/grapql/types.py` & `api_deezer_full-0.0.1b37/api_deezer_full/pipe/grapql/types.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/__init__.py` & `api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/__init__.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/bases.py` & `api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/bases.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/media.py` & `api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/media.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/api_deezer_full/pipe/types/playlist.py` & `api_deezer_full-0.0.1b37/api_deezer_full/pipe/types/playlist.py`

 * *Files identical despite different names*

### Comparing `api_deezer_full-0.0.1b36/PKG-INFO` & `api_deezer_full-0.0.1b37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-deezer-full
-Version: 0.0.1b36
+Version: 0.0.1b37
 Summary: Wrapper for all 'hidden' deezer APIs
 License: CC BY 4.0
 Author: An0nimia
 Author-email: an0nimia@protonmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


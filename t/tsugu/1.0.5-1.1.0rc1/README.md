# Comparing `tmp/tsugu-1.0.5.tar.gz` & `tmp/tsugu-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-1.0.5.tar", last modified: Thu May 16 00:32:40 2024, max compression
+gzip compressed data, was "tsugu-1.1.0rc1.tar", last modified: Mon May 20 19:00:58 2024, max compression
```

## Comparing `tsugu-1.0.5.tar` & `tsugu-1.1.0rc1.tar`

### file list

```diff
@@ -1,97 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.401273 tsugu-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-16 00:32:32.000000 tsugu-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-16 00:32:40.401273 tsugu-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-16 00:32:32.000000 tsugu-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:32:40.401273 tsugu-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-16 00:32:32.000000 tsugu-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.389273 tsugu-1.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-16 00:32:32.000000 tsugu-1.0.5/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.389273 tsugu-1.0.5/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.389273 tsugu-1.0.5/tsugu/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.389273 tsugu-1.0.5/tsugu/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.389273 tsugu-1.0.5/tsugu/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.393273 tsugu-1.0.5/tsugu/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.393273 tsugu-1.0.5/tsugu/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.393273 tsugu-1.0.5/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.389273 tsugu-1.0.5/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-16 00:32:40.000000 tsugu-1.0.5/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-16 00:32:40.000000 tsugu-1.0.5/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:32:40.000000 tsugu-1.0.5/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 00:32:40.000000 tsugu-1.0.5/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 00:32:40.000000 tsugu-1.0.5/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.397273 tsugu-1.0.5/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.397273 tsugu-1.0.5/tsugu_async/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.397273 tsugu-1.0.5/tsugu_async/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.397273 tsugu-1.0.5/tsugu_async/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.397273 tsugu-1.0.5/tsugu_async/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.401273 tsugu-1.0.5/tsugu_async/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:32:40.401273 tsugu-1.0.5/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-16 00:32:32.000000 tsugu-1.0.5/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.832085 tsugu-1.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-20 19:00:58.828085 tsugu-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:00:58.832085 tsugu-1.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/tsugu/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/tsugu/router/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.820085 tsugu-1.1.0rc1/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 19:00:58.000000 tsugu-1.1.0rc1/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu_async/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.824085 tsugu-1.1.0rc1/tsugu_async/router/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.828085 tsugu-1.1.0rc1/tsugu_async/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.828085 tsugu-1.1.0rc1/tsugu_async/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:58.828085 tsugu-1.1.0rc1/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-20 19:00:49.000000 tsugu-1.1.0rc1/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-1.0.5/LICENSE` & `tsugu-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.5/PKG-INFO` & `tsugu-1.1.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.0.5
+Version: 1.1.0rc1
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -33,16 +33,17 @@
         
         
         ```shell
         pip install tsugu
         ```
         
         
-        > Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
+        > API Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
         
+        > Command matching by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
         ***
         
         ## handler
         
         - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
@@ -81,18 +82,18 @@
         
         
         ## 配置
         
         
         > 随意更改配置项可能会导致不可预知的错误。
         
-        ### tsugu_api settings
+        ### tsugu_api_core settings
         
         ```py
-        from tsugu_api import settings
+        from tsugu_api_core import settings
         
         settings.timeout = 10
         '''
         请求超时时间
         '''
         
         settings.proxy = ''
@@ -136,62 +137,49 @@
         '''
         是否压缩返回数据，压缩可减少返回数据大小。
         默认为 True，即压缩返回数据。若不压缩返回数据，可将此项设置为 False。
         '''
         
         ```
         
-        ```py
-        from tsugu_api_async import settings
-        ...
-        ```
-        
         ### tsugu_async config
         
         ```py
         from tsugu import config
         
-        config.prefix = ['/', '']
-        '''
-        命令前缀
-        最后一个参数如果不是空字符串，则只有在命令前缀符合时才会触发命令。
-        '''
         
-        config.allow_gap_less = True
+        config.compact = True
         '''
         是否允许命令与参数之间没有空格
         '''
         
-        config.get_remote_user_data_max_retry = 3
+        config.remote_data_max_retry = 3
         '''
         获取远程用户数据最大重试次数
         '''
         
-        config.token_name = "Tsugu"
+        config.bandori_station_token_name = "Tsugu"
         '''
         bandori station token
         '''
         config.bandori_station_token = "ZtV4EX2K9Onb"
         '''
         bandori station token
         '''
         
-        config.ban_gacha_simulate_group_data = []
+        config.disable_gacha_simulate_group_ids = []
         '''
         需要关闭模拟抽卡的群
         '''
-        
-        config.commands = ...
-        
-        config.user_commands = ...
         ```
         
         ```py
         from tsugu_async import config
         ...
+        # 与上面相同
         ```
         
         
         
         ***
         
          <details>
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.0.5 Summary: Tsugu Python Frontend
-Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
-Author-email: zjr2992@outlook.com License: MIT Description:
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc1 Summary: Tsugu Python
+Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
+kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
-- `handler` ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
-```python import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id
-å¹³å° é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x',
-user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
-',i) if isinstance(i, str) else None print(f"[å¾ç]") if isinstance(i, bytes)
-else None ``` ```python import tsugu_async ... ``` >
-å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º
-`user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã ## handler_raw
-å¦æä½ æ¹ä¾¿ä½¿ç¨ base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
+--- ```shell pip install tsugu ``` > API Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
+matching by _A_l_c_o_n_n_a *** ## handler - `handler`
+ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
+import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
+é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
+platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
+str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
+```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
+`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
+å¯ä»¥å¡«å `red`ã ## handler_raw å¦æä½ æ¹ä¾¿ä½¿ç¨
+base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
 åç«¯æ¬èº«è¿åæ­¤æ°æ®ç»æï¼è¿ä¸ªæ¹æ³å¯ä»¥èçä¸å¿è¦çå¼éã
 ```python import tsugu for i in tsugu.handler_raw(message='æ¥å¡ ars 1x',
 user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
 ',i) if i['type'] == 'text' else None print(f"[å¾ç]") if i['type'] ==
 'base64' else None ``` ```python import tsugu_async ... ``` ## éç½® >
-éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api
-settings ```py from tsugu_api import settings settings.timeout = 10 '''
+éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api_core
+settings ```py from tsugu_api_core import settings settings.timeout = 10 '''
 è¯·æ±è¶æ¶æ¶é´ ''' settings.proxy = '' ''' ä»£çå°å '''
 settings.backend_url = 'http://tsugubot.com:8080' ''' åç«¯å°å é»è®¤ä¸º
 Tsugu å®æ¹åç«¯ï¼è¥æèªå»ºåç«¯æå¡å¨å¯è¿è¡ä¿®æ¹ã '''
 settings.backend_proxy = True ''' æ¯å¦ä½¿ç¨åç«¯ä»£ç
 å½è®¾ç½®ä»£çå°ååå¯ä¿®æ¹æ­¤é¡¹ä»¥å³å®æ¯å¦ä½¿ç¨ä»£çã é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨åç«¯ä»£çãè¥ä½¿ç¨ä»£çæ¶åç«¯æå¡å¨æ æ³è®¿é®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.userdata_backend_url = 'http://tsugubot.com:8080' '''
@@ -37,26 +38,21 @@
 Falseã ''' settings.use_easy_bg = True '''
 æ¯å¦ä½¿ç¨ç®æèæ¯ï¼ä½¿ç¨å¯å¨éä½èæ¯è´¨éçåæä¸å å¿«ååºéåº¦ã
 é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨ç®æèæ¯ãè¥ä¸ä½¿ç¨ç®æèæ¯ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.compress = True '''
 æ¯å¦åç¼©è¿åæ°æ®ï¼åç¼©å¯åå°è¿åæ°æ®å¤§å°ã é»è®¤ä¸º
 Trueï¼å³åç¼©è¿åæ°æ®ãè¥ä¸åç¼©è¿åæ°æ®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
-Falseã ''' ``` ```py from tsugu_api_async import settings ... ``` ###
-tsugu_async config ```py from tsugu import config config.prefix = ['/', ''] '''
-å½ä»¤åç¼
-æåä¸ä¸ªåæ°å¦æä¸æ¯ç©ºå­ç¬¦ä¸²ï¼ååªæå¨å½ä»¤åç¼ç¬¦åæ¶æä¼è§¦åå½ä»¤ã
-''' config.allow_gap_less = True '''
-æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
-config.get_remote_user_data_max_retry = 3 '''
-è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ° ''' config.token_name = "Tsugu" '''
-bandori station token ''' config.bandori_station_token = "ZtV4EX2K9Onb" '''
-bandori station token ''' config.ban_gacha_simulate_group_data = [] '''
-éè¦å³é­æ¨¡ææ½å¡çç¾¤ ''' config.commands = ... config.user_commands =
-... ``` ```py from tsugu_async import config ... ``` *** ?å?®?¢?æ???ð???±?æ???å?¯?¼
-((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+Falseã ''' ``` ### tsugu_async config ```py from tsugu import config
+config.compact = True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
+config.remote_data_max_retry = 3 ''' è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ°
+''' config.bandori_station_token_name = "Tsugu" ''' bandori station token '''
+config.bandori_station_token = "ZtV4EX2K9Onb" ''' bandori station token '''
+config.disable_gacha_simulate_group_ids = [] ''' éè¦å³é­æ¨¡ææ½å¡çç¾¤
+''' ``` ```py from tsugu_async import config ... # ä¸ä¸é¢ç¸å ``` ***
+?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
 qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ --- Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-1.0.5/README.md` & `tsugu-1.1.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 
 
 ```shell
 pip install tsugu
 ```
 
 
-> Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
+> API Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
 
+> Command matching by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
 ***
 
 ## handler
 
 - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
 
 ```python
@@ -73,18 +74,18 @@
 
 
 ## 配置
 
 
 > 随意更改配置项可能会导致不可预知的错误。
 
-### tsugu_api settings
+### tsugu_api_core settings
 
 ```py
-from tsugu_api import settings
+from tsugu_api_core import settings
 
 settings.timeout = 10
 '''
 请求超时时间
 '''
 
 settings.proxy = ''
@@ -128,62 +129,49 @@
 '''
 是否压缩返回数据，压缩可减少返回数据大小。
 默认为 True，即压缩返回数据。若不压缩返回数据，可将此项设置为 False。
 '''
 
 ```
 
-```py
-from tsugu_api_async import settings
-...
-```
-
 ### tsugu_async config
 
 ```py
 from tsugu import config
 
-config.prefix = ['/', '']
-'''
-命令前缀
-最后一个参数如果不是空字符串，则只有在命令前缀符合时才会触发命令。
-'''
 
-config.allow_gap_less = True
+config.compact = True
 '''
 是否允许命令与参数之间没有空格
 '''
 
-config.get_remote_user_data_max_retry = 3
+config.remote_data_max_retry = 3
 '''
 获取远程用户数据最大重试次数
 '''
 
-config.token_name = "Tsugu"
+config.bandori_station_token_name = "Tsugu"
 '''
 bandori station token
 '''
 config.bandori_station_token = "ZtV4EX2K9Onb"
 '''
 bandori station token
 '''
 
-config.ban_gacha_simulate_group_data = []
+config.disable_gacha_simulate_group_ids = []
 '''
 需要关闭模拟抽卡的群
 '''
-
-config.commands = ...
-
-config.user_commands = ...
 ```
 
 ```py
 from tsugu_async import config
 ...
+# 与上面相同
 ```
 
 
 
 ***
 
  <details>
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
-- `handler` ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
-```python import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id
-å¹³å° é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x',
-user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
-',i) if isinstance(i, str) else None print(f"[å¾ç]") if isinstance(i, bytes)
-else None ``` ```python import tsugu_async ... ``` >
-å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º
-`user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã ## handler_raw
-å¦æä½ æ¹ä¾¿ä½¿ç¨ base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
+--- ```shell pip install tsugu ``` > API Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
+matching by _A_l_c_o_n_n_a *** ## handler - `handler`
+ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
+import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
+é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
+platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
+str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
+```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
+`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
+å¯ä»¥å¡«å `red`ã ## handler_raw å¦æä½ æ¹ä¾¿ä½¿ç¨
+base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
 åç«¯æ¬èº«è¿åæ­¤æ°æ®ç»æï¼è¿ä¸ªæ¹æ³å¯ä»¥èçä¸å¿è¦çå¼éã
 ```python import tsugu for i in tsugu.handler_raw(message='æ¥å¡ ars 1x',
 user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
 ',i) if i['type'] == 'text' else None print(f"[å¾ç]") if i['type'] ==
 'base64' else None ``` ```python import tsugu_async ... ``` ## éç½® >
-éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api
-settings ```py from tsugu_api import settings settings.timeout = 10 '''
+éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api_core
+settings ```py from tsugu_api_core import settings settings.timeout = 10 '''
 è¯·æ±è¶æ¶æ¶é´ ''' settings.proxy = '' ''' ä»£çå°å '''
 settings.backend_url = 'http://tsugubot.com:8080' ''' åç«¯å°å é»è®¤ä¸º
 Tsugu å®æ¹åç«¯ï¼è¥æèªå»ºåç«¯æå¡å¨å¯è¿è¡ä¿®æ¹ã '''
 settings.backend_proxy = True ''' æ¯å¦ä½¿ç¨åç«¯ä»£ç
 å½è®¾ç½®ä»£çå°ååå¯ä¿®æ¹æ­¤é¡¹ä»¥å³å®æ¯å¦ä½¿ç¨ä»£çã é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨åç«¯ä»£çãè¥ä½¿ç¨ä»£çæ¶åç«¯æå¡å¨æ æ³è®¿é®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.userdata_backend_url = 'http://tsugubot.com:8080' '''
@@ -34,23 +35,18 @@
 Falseã ''' settings.use_easy_bg = True '''
 æ¯å¦ä½¿ç¨ç®æèæ¯ï¼ä½¿ç¨å¯å¨éä½èæ¯è´¨éçåæä¸å å¿«ååºéåº¦ã
 é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨ç®æèæ¯ãè¥ä¸ä½¿ç¨ç®æèæ¯ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.compress = True '''
 æ¯å¦åç¼©è¿åæ°æ®ï¼åç¼©å¯åå°è¿åæ°æ®å¤§å°ã é»è®¤ä¸º
 Trueï¼å³åç¼©è¿åæ°æ®ãè¥ä¸åç¼©è¿åæ°æ®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
-Falseã ''' ``` ```py from tsugu_api_async import settings ... ``` ###
-tsugu_async config ```py from tsugu import config config.prefix = ['/', ''] '''
-å½ä»¤åç¼
-æåä¸ä¸ªåæ°å¦æä¸æ¯ç©ºå­ç¬¦ä¸²ï¼ååªæå¨å½ä»¤åç¼ç¬¦åæ¶æä¼è§¦åå½ä»¤ã
-''' config.allow_gap_less = True '''
-æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
-config.get_remote_user_data_max_retry = 3 '''
-è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ° ''' config.token_name = "Tsugu" '''
-bandori station token ''' config.bandori_station_token = "ZtV4EX2K9Onb" '''
-bandori station token ''' config.ban_gacha_simulate_group_data = [] '''
-éè¦å³é­æ¨¡ææ½å¡çç¾¤ ''' config.commands = ... config.user_commands =
-... ``` ```py from tsugu_async import config ... ``` *** ?å?®?¢?æ???ð???±?æ???å?¯?¼
-((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+Falseã ''' ``` ### tsugu_async config ```py from tsugu import config
+config.compact = True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
+config.remote_data_max_retry = 3 ''' è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ°
+''' config.bandori_station_token_name = "Tsugu" ''' bandori station token '''
+config.bandori_station_token = "ZtV4EX2K9Onb" ''' bandori station token '''
+config.disable_gacha_simulate_group_ids = [] ''' éè¦å³é­æ¨¡ææ½å¡çç¾¤
+''' ``` ```py from tsugu_async import config ... # ä¸ä¸é¢ç¸å ``` ***
+?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
 qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ ---
```

### Comparing `tsugu-1.0.5/setup.py` & `tsugu-1.1.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='1.0.5',
+    version='1.1.0-rc1',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
-    packages=find_packages(),
+    packages=find_packages(exclude=('test','test*')),
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
             "loguru",
-            "tsugu-api-python>=1.1.2"
+            "tsugu-api-python==1.2.0",
+            "arclet-alconna",
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-1.0.5/test/test_async.py` & `tsugu-1.1.0rc1/test/test_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 
         # tsugu.database('./user_data.db')
         # tsugu_async.config.reload_from_json('./config.json')
         # from tsugu_api_async import settings
         # settings.backend_url = 'http://127.0.0.1:8010'
         from tsugu_api_async import settings
 
-        settings.backend_url = 'http://124.221.153.148:3000'
+        # settings.backend_url = 'http://124.221.153.148:3000'
         # settings.userdata_backend_url = 'http://127.0.0.1:3001'
 
-        msg1 = await tsugu_async.handler('查玩家', '1528593481', 'red', '666808414')
+        msg1 = await tsugu_async.handler('查活动 蓝 ag', '1528593481', 'red', '666808414')
         await show_back_msg(msg1)
 
         # msg2 = await tsugu_async.handler('ycm', '1528593481', 'red', '666808414')
         # await show_back_msg(msg2)
 
         # msg3 = await tsugu_async.handler('12324 测q1试', '1528593481', 'red', '666808414')
         # await show_back_msg(msg3)
```

### Comparing `tsugu-1.0.5/tsugu/handler.py` & `tsugu-1.1.0rc1/tsugu/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import base64
 from typing import List, Union, Dict
 
 from .utils import *
 from loguru import logger
 from . import router
 
+
 def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
     :param message: 用户消息
     :param user_id: 用户ID
```

### Comparing `tsugu-1.0.5/tsugu/router/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc1/tsugu_async/router/remote/change_server_mode.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,42 @@
-from ...utils import text_response, User
+from ...utils import text_response, User, server_name_2_server_id
+import tsugu_api_async
 from ...config import config
-from ...command_matcher import MC
-from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
-from tsugu_api._typing import _ServerId
-import tsugu_api
-
-
-def handler(user: User, res: MC, platform: str, channel_id: str):
-    if not res.args or len(res.args) < 2:
-        return text_response('请输入正确的格式：验证绑定 你的玩家ID(数字) 服务器名(字母缩写)')
-    player_id = int(res.args[0])
-    server_pre = server_name_2_server_id(res.args[1])
-    if not server_exists(server_pre):
-        return text_response('未找到服务器，请输入正确的服务器名')
-    user.server_mode = server_pre
-
-    r = tsugu_api.bind_player_verification(platform, user.user_id, user.server_mode, player_id, True)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    return text_response(f'绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
+from tsugu_api_core._typing import _ServerName
 
+alc = Alconna(
+        ["主服务器", "设置主服务器"],
+    Args["serverName#服务器名", _ServerName],
+        meta=CommandMeta(
+            compact=config.compact, description="主服务器",
+            usage="将指定的服务器设置为你的主服务器。",
+            example="""主服务器 cn : 将国服设置为主服务器。"""
 
+        )
+    )
+
+
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        r = await tsugu_api_async.change_user_data(platform, user.user_id, {'server_mode': server_name_2_server_id(res.serverName)})
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('主服务器已设置为 ' + res.serverName)
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
+
+#
+# def handler(user: User, res: MC, platform: str, channel_id: str):
+#     if res.args:
+#         server_mode = server_name_2_server_id(res.args[0])
+#         if not server_exists(server_mode):
+#             return text_response('未找到服务器，请输入正确的服务器名')
+#         update: _Update = {'server_mode': server_mode, }
+#         if r := tsugu_api.change_user_data(platform, user.user_id, update):
+#             if r.get('status') == 'success':
+#                 return text_response('主服务器已设置为 ' + server_id_2_server_name(server_mode))
+#             return text_response(r.get('data'))
+#
```

### Comparing `tsugu-1.0.5/tsugu/router/remote/change_default_server.py` & `tsugu-1.1.0rc1/tsugu/router/remote/switch_car_forwarding_off.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,26 @@
-from ...config import config
-from ...utils import text_response, User
-from ...command_matcher import MC
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api
-from ...utils import server_exists, server_names_2_server_ids
-from tsugu_api._typing import _Update
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+
+
+alc = Alconna(
+        ["关闭车牌转发", "关闭个人车牌转发"],
+        meta=CommandMeta(
+            compact=config.compact, description="关闭车牌转发",)
+    )
+
+
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
 
+    if res.matched:
+        update = {'car': False, }
+        r = tsugu_api.change_user_data(platform, user.user_id, update)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('关闭车牌转发成功！')
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
 
-def handler(user: User, res: MC, platform: str, channel_id: str):
-    default_server = server_names_2_server_ids(res.args)
-    if not default_server:
-        return text_response('未找到服务器，请输入正确的服务器名')
-    change_data: _Update = {'default_server': default_server}
-    r = tsugu_api.change_user_data(platform, user.user_id, change_data)
-    if r.get('status') == 'success':
-        return text_response(f'默认服务器已设置为 {", ".join(res.args)}')
-    return text_response(r.get('data'))
```

### Comparing `tsugu-1.0.5/tsugu/router/remote/player_status.py` & `tsugu-1.1.0rc1/tsugu/router/remote/player_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,77 @@
-from ...config import config
-from ...utils import text_response, User
-from ...command_matcher import MC
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api
-from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
-from tsugu_api._typing import _ServerId, _Update
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from tsugu_api_core._typing import _ServerName
 
 
-def handler(user: User, res: MC, platform: str, channel_id: str):
-    # 无参数
-    if not res.args:
-        # 默认情况1: 优先当前服务器
-        for i in user.game_ids:
-            if i.get("server") == user.server_mode:
-                player_id = str(i.get("game_id"))
-                server = int(i.get("server"))
-                text = f'已查找默认服务器 {server_id_2_server_name(server)} 的记录'
-                msg = tsugu_api.search_player(int(player_id), server) + text_response(text)
-                return msg
-        else:
-            # 默认情况2: 优先第一个记录
-            if len(user.game_ids) > 0:
-                player_id = str(user.game_ids[0].get("game_id"))
-                server = int(user.game_ids[0].get("server"))
-                text = f'已查找第一个记录 {player_id}'
-                msg = tsugu_api.search_player(int(player_id), server) + text_response(text)
-                return msg
-            else:
-                return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
-
-    # 查询指定服务器的玩家状态
-    server: _ServerId = server_name_2_server_id(res.args[0])
-    if server_exists(server):
-        for i in user.game_ids:
-            if i.get("server") == server:
-                player_id = str(i.get("game_id"))
-                text = f'已查找指定服务器 {server_id_2_server_name(server)} 的记录'
-                msg = tsugu_api.search_player(int(player_id), server) + text_response(text)
-                return msg
+alc = Alconna(
+        ["玩家状态"],
+        Args["serverName", _ServerName.__args__, None]["serverIndex", int, None],
+        meta=CommandMeta(
+            compact=config.compact, description="查询自己的玩家状态",
+            usage='根据关键词或活动ID查询活动信息',
+            example='''玩家状态 :返回玩家状态(优先当前服务器下第一条记录)
+玩家状态 1 :返回绑定的第一条记录的状态
+玩家状态 jp :返回绑定的cn服务器的记录的状态'''
+        )
+    )
+
+
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        if res.serverName:
+            return _case_server(user, res.serverName)
+        elif res.serverIndex:
+            return _case_index(user, res.serverIndex)
         else:
-            return text_response(
-                f'未在 {len(user.game_ids)} 条记录中找到 {server_id_2_server_name(server)} 的记录')
+            return _case_default(user)
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
+
+
+
+def _utils_search_player_by_game_id(game_id, additional_text=""):
+    player_id = str(game_id.get("game_id"))
+    server = int(game_id.get("server"))
+    response = tsugu_api.search_player(int(player_id), server)
+    return response + text_response(additional_text)
+
+
+def _case_default(user: User):
+    # 优先当前服务器
+    for game_id in user.game_ids:
+        if game_id.get("server") == user.server_mode:
+            text = f'已查找默认服务器 {server_id_2_server_name(user.server_mode)} 的记录。'
+            return _utils_search_player_by_game_id(game_id, text)
+    # 兜底逻辑：使用第一个记录
+    if user.game_ids:
+        game_id = user.game_ids[0]
+        text = f'已查找第一个记录。'
+        return _utils_search_player_by_game_id(game_id, text)
+    return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
+
+
+def _case_server(user: User, server_name: str):
+    server_id = server_name_2_server_id(server_name)
+    # 服务器不存在
+    if not server_exists(server_id):
+        return text_response(f'服务器 {server_name} 不存在。')
+    # 查找记录
+    for game_id in user.game_ids:
+        if game_id.get("server") == server_id:
+            # 找到记录
+            return _utils_search_player_by_game_id(game_id)
+    # 未找到记录
+    return text_response(f'未在记录中找到服务器 {server_name} 的记录。')
+
+
+def _case_index(user: User, index: int):
+    if index > len(user.game_ids) or index < 1:
+        return text_response(f'未找到记录 {index}。')
+    return _utils_search_player_by_game_id(user.game_ids[index - 1])
 
-    # 查询指定记录顺序的玩家状态
-    if res.args[0].isdigit():
-        if int(res.args[0]) > len(user.game_ids) or int(res.args[0]) < 1:
-            return text_response(f'未找到记录 {res.args[0]}')
-        player_id = str(user.game_ids[int(res.args[0]) - 1].get("game_id"))
-        server = int(user.game_ids[int(res.args[0]) - 1].get("server"))
-        text = f'已查找第 {res.args[0]} 条记录'
-        msg = tsugu_api.search_player(int(player_id), server) + text_response(text)
-        return msg
 
-    return text_response('请确保输入是 服务器名(字母缩写) 或者 记录(数字)')
```

### Comparing `tsugu-1.0.5/tsugu/router/remote/unbind_player.py` & `tsugu-1.1.0rc1/tsugu/router/remote/bind_player_verification_off.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,52 @@
-from ...config import config
-from ...utils import text_response, User
-from ...command_matcher import MC
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api
-from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
-from tsugu_api._typing import _ServerId
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from tsugu_api_core._typing import _ServerName
 
 
-def mask_data(game_id: str):
-    game_id = str(game_id)
-    if len(game_id) < 6:
-        return game_id[:3] + '*' * (len(game_id) - 3)
-    elif len(game_id) < 3:
-        return '*' * len(game_id)
-    else:
-        game_id = game_id[:3] + '*' * (len(game_id) - 6) + game_id[-3:]
-    return game_id
-
-
-def handler(user: User, res: MC, platform: str, channel_id: str):
-    bind_record = '\n'.join(
-        [f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in
-         enumerate(user.game_ids)])
-    if not res.args:
-        return text_response(f'请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n{bind_record}')
-
-    if not res.args[0].isdigit():
-        return text_response(f'请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n{bind_record}')
-
-    if int(res.args[0]) > len(user.game_ids):
-        return text_response(f'未找到记录 {res.args[0]}，当前的绑定记录如下:\n{bind_record}')
-
-    server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
-    r = tsugu_api.bind_player_request(platform, user.user_id, server_mode, False)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    # 如果是200
-    return text_response(
-        f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.args[0]}\n来完成本次身份验证''')
+alc = Alconna(
+        ["验证解绑"],
+    Args["index#要解绑的绑定编号", int],
+        meta=CommandMeta(
+            compact=config.compact, description="验证解绑",
+            usage="验证解绑 记录编号(数字)",
+            example="验证解绑 1 : 解绑第一个记录"
+        ),
+    )
+
+
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        if len(user.game_ids) < int(res.index):
+            return text_response('未找到记录')
+        player_id = user.game_ids[int(res.index) - 1].get("game_id")
+        server_mode = user.game_ids[int(res.index) - 1].get("server")
+        r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('解绑成功！')
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
+
+
+# def handler(user: User, res: MC, platform: str, channel_id: str):
+#     if not res.args or len(res.args) > 1:
+#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
+#     if not res.args[0].isdigit():
+#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
+#     if int(res.text) <= 0:
+#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)，编号从1开始')
+#     if len(user.game_ids) < int(res.text):
+#         return text_response('未找到记录')
+#     player_id = user.game_ids[int(res.args[0]) - 1].get("game_id")
+#     server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
+#     r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
+#     if r.get('status') != 'success':
+#         return text_response(r.get('data'))
+#     return text_response('解绑成功！')
+#
+#
```

### Comparing `tsugu-1.0.5/tsugu/utils/__init__.py` & `tsugu-1.1.0rc1/tsugu/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,70 +2,84 @@
 from typing import List
 
 from ..config import config
 import tsugu_api
 from loguru import logger
 import time
 
-from tsugu_api._typing import _ServerId
+from tsugu_api_core._typing import _ServerId
 
 
-class User:
-    def __init__(self, user_id: str, platform: str, server_mode: _ServerId, default_server: List[_ServerId], car: bool, server_list: list, game_ids: list, verify_code: str):
-        self.user_id: str = user_id
-        self.platform: str = platform
-        self.server_mode: _ServerId = server_mode
-        self.default_server: List[_ServerId] = default_server
-        self.car: bool = car
-        self.server_list: list = server_list
-        self.game_ids = game_ids
-        self.verify_code = verify_code
+_i_s = {0: "jp", 1: "en", 2: "tw", 3: "cn", 4: "kr"}
+_s_i = {"jp": 0, "en": 1, "tw": 2, "cn": 3, "kr": 4}
 
 
 def text_response(string):
-    return [{"type": "string", "string": string}]
+    return [{"type": "string", "string": str(string)}]
 
 
 def server_names_2_server_ids(server_name: List[str]) -> List[_ServerId]:
-    return [config._s_i[code] for code in server_name]
+    return [_s_i[code] for code in server_name]
 
 
 def server_name_2_server_id(server_name: str) -> _ServerId:
-    return config._s_i[server_name] if server_name in config._s_i else None
+    return _s_i[server_name] if server_name in _s_i else None
 
 
 def server_ids_2_server_names(index: List[_ServerId]) -> List[str]:
-    return [config._i_s[code] for code in index]
+    return [_i_s[code] for code in index]
 
 
 def server_id_2_server_name(index: _ServerId) -> str:
-    return config._i_s[index] if index in config._i_s else None
+    return _i_s[index] if index in _i_s else None
 
 
 def server_exists(server):
     if server or server == 0:
         return True
     if not server:
         return False
     return False
 
 
+class User:
+    def __init__(self, user_id: str, platform: str, server_mode: _ServerId, default_server: List[_ServerId], car: bool, server_list: list, game_ids: list, verify_code: str):
+        self.user_id: str = user_id
+        self.platform: str = platform
+        self.server_mode: _ServerId = server_mode
+        self.default_server: List[_ServerId] = default_server
+        self.car: bool = car
+        self.server_list: list = server_list
+        self.game_ids = game_ids
+        self.verify_code = verify_code
+
+
 def get_user(user_id: str, platform: str) -> User:
-    for i in range(0, config.get_remote_user_data_max_retry):
+    '''
+    获取用户数据
+    多次尝试获取用户数据
+    兼容旧版用户数据
+
+    :param user_id:
+    :param platform:
+    :return:
+    '''
+    for i in range(0, config.remote_data_max_retry):
         try:
             user_data_res = tsugu_api.get_user_data(platform, user_id)
             if user_data_res.get('status') == 'failed':
                 return text_response(user_data_res.get('data'))
             break
         except Exception as e:
             logger.error(f'Error: {e}')
-            time.sleep(0.5)
+            time.sleep(0.8)
             continue
     else:
         raise Exception('获取用户数据失败')
+
     # 获取用户数据失败
     if user_data_res.get('status') == 'failed':
         return text_response(user_data_res.get('data'))
     # 构建用户对象
     user_data = user_data_res.get('data')
 
     if user_data.get('game_ids') is None:
@@ -75,16 +89,14 @@
             if user_data.get('server_list')[i]['playerId'] != 0:
                 new_game_id = {"game_id": user_data.get('server_list')[i]['playerId'], "server": i}
                 user_data['game_ids'].append(new_game_id)
         verify_code_all = []
         for i in range(0, 5):
             if user_data.get('server_list')[i].get('verifyCode') is not None:
                 verify_code_all.append(i)
-        # 有一说一，下面这行没有实际意义
-        user_data['verify_code'] = '或'.join([str(user_data.get('server_list')[i].get('verifyCode')) for i in verify_code_all]) if len(verify_code_all) > 1 else verify_code_all[0] if verify_code_all else ''
 
     user = User(user_id=user_id,
                 platform=platform,
                 server_mode=user_data.get('server_mode'),
                 default_server=user_data.get('default_server'),
                 car=user_data.get('car'),
                 server_list=user_data.get('server_list', None),
```

### Comparing `tsugu-1.0.5/tsugu.egg-info/PKG-INFO` & `tsugu-1.1.0rc1/tsugu.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.0.5
+Version: 1.1.0rc1
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
@@ -33,16 +33,17 @@
         
         
         ```shell
         pip install tsugu
         ```
         
         
-        > Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
+        > API Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
         
+        > Command matching by <a href="https://github.com/ArcletProject/Alconna">Alconna</a>
         ***
         
         ## handler
         
         - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
@@ -81,18 +82,18 @@
         
         
         ## 配置
         
         
         > 随意更改配置项可能会导致不可预知的错误。
         
-        ### tsugu_api settings
+        ### tsugu_api_core settings
         
         ```py
-        from tsugu_api import settings
+        from tsugu_api_core import settings
         
         settings.timeout = 10
         '''
         请求超时时间
         '''
         
         settings.proxy = ''
@@ -136,62 +137,49 @@
         '''
         是否压缩返回数据，压缩可减少返回数据大小。
         默认为 True，即压缩返回数据。若不压缩返回数据，可将此项设置为 False。
         '''
         
         ```
         
-        ```py
-        from tsugu_api_async import settings
-        ...
-        ```
-        
         ### tsugu_async config
         
         ```py
         from tsugu import config
         
-        config.prefix = ['/', '']
-        '''
-        命令前缀
-        最后一个参数如果不是空字符串，则只有在命令前缀符合时才会触发命令。
-        '''
         
-        config.allow_gap_less = True
+        config.compact = True
         '''
         是否允许命令与参数之间没有空格
         '''
         
-        config.get_remote_user_data_max_retry = 3
+        config.remote_data_max_retry = 3
         '''
         获取远程用户数据最大重试次数
         '''
         
-        config.token_name = "Tsugu"
+        config.bandori_station_token_name = "Tsugu"
         '''
         bandori station token
         '''
         config.bandori_station_token = "ZtV4EX2K9Onb"
         '''
         bandori station token
         '''
         
-        config.ban_gacha_simulate_group_data = []
+        config.disable_gacha_simulate_group_ids = []
         '''
         需要关闭模拟抽卡的群
         '''
-        
-        config.commands = ...
-        
-        config.user_commands = ...
         ```
         
         ```py
         from tsugu_async import config
         ...
+        # 与上面相同
         ```
         
         
         
         ***
         
          <details>
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.0.5 Summary: Tsugu Python Frontend
-Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
-Author-email: zjr2992@outlook.com License: MIT Description:
+Metadata-Version: 2.1 Name: tsugu Version: 1.1.0rc1 Summary: Tsugu Python
+Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
+kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
---- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
-- `handler` ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
-```python import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id
-å¹³å° é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x',
-user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
-',i) if isinstance(i, str) else None print(f"[å¾ç]") if isinstance(i, bytes)
-else None ``` ```python import tsugu_async ... ``` >
-å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º
-`user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã ## handler_raw
-å¦æä½ æ¹ä¾¿ä½¿ç¨ base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
+--- ```shell pip install tsugu ``` > API Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n > Command
+matching by _A_l_c_o_n_n_a *** ## handler - `handler`
+ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ: ```python
+import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å°
+é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481',
+platform='red', channel_id='666808414'): print('ææ¬: ',i) if isinstance(i,
+str) else None print(f"[å¾ç]") if isinstance(i, bytes) else None ```
+```python import tsugu_async ... ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
+`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
+å¯ä»¥å¡«å `red`ã ## handler_raw å¦æä½ æ¹ä¾¿ä½¿ç¨
+base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
 åç«¯æ¬èº«è¿åæ­¤æ°æ®ç»æï¼è¿ä¸ªæ¹æ³å¯ä»¥èçä¸å¿è¦çå¼éã
 ```python import tsugu for i in tsugu.handler_raw(message='æ¥å¡ ars 1x',
 user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
 ',i) if i['type'] == 'text' else None print(f"[å¾ç]") if i['type'] ==
 'base64' else None ``` ```python import tsugu_async ... ``` ## éç½® >
-éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api
-settings ```py from tsugu_api import settings settings.timeout = 10 '''
+éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api_core
+settings ```py from tsugu_api_core import settings settings.timeout = 10 '''
 è¯·æ±è¶æ¶æ¶é´ ''' settings.proxy = '' ''' ä»£çå°å '''
 settings.backend_url = 'http://tsugubot.com:8080' ''' åç«¯å°å é»è®¤ä¸º
 Tsugu å®æ¹åç«¯ï¼è¥æèªå»ºåç«¯æå¡å¨å¯è¿è¡ä¿®æ¹ã '''
 settings.backend_proxy = True ''' æ¯å¦ä½¿ç¨åç«¯ä»£ç
 å½è®¾ç½®ä»£çå°ååå¯ä¿®æ¹æ­¤é¡¹ä»¥å³å®æ¯å¦ä½¿ç¨ä»£çã é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨åç«¯ä»£çãè¥ä½¿ç¨ä»£çæ¶åç«¯æå¡å¨æ æ³è®¿é®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.userdata_backend_url = 'http://tsugubot.com:8080' '''
@@ -37,26 +38,21 @@
 Falseã ''' settings.use_easy_bg = True '''
 æ¯å¦ä½¿ç¨ç®æèæ¯ï¼ä½¿ç¨å¯å¨éä½èæ¯è´¨éçåæä¸å å¿«ååºéåº¦ã
 é»è®¤ä¸º
 Trueï¼å³ä½¿ç¨ç®æèæ¯ãè¥ä¸ä½¿ç¨ç®æèæ¯ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
 Falseã ''' settings.compress = True '''
 æ¯å¦åç¼©è¿åæ°æ®ï¼åç¼©å¯åå°è¿åæ°æ®å¤§å°ã é»è®¤ä¸º
 Trueï¼å³åç¼©è¿åæ°æ®ãè¥ä¸åç¼©è¿åæ°æ®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
-Falseã ''' ``` ```py from tsugu_api_async import settings ... ``` ###
-tsugu_async config ```py from tsugu import config config.prefix = ['/', ''] '''
-å½ä»¤åç¼
-æåä¸ä¸ªåæ°å¦æä¸æ¯ç©ºå­ç¬¦ä¸²ï¼ååªæå¨å½ä»¤åç¼ç¬¦åæ¶æä¼è§¦åå½ä»¤ã
-''' config.allow_gap_less = True '''
-æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
-config.get_remote_user_data_max_retry = 3 '''
-è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ° ''' config.token_name = "Tsugu" '''
-bandori station token ''' config.bandori_station_token = "ZtV4EX2K9Onb" '''
-bandori station token ''' config.ban_gacha_simulate_group_data = [] '''
-éè¦å³é­æ¨¡ææ½å¡çç¾¤ ''' config.commands = ... config.user_commands =
-... ``` ```py from tsugu_async import config ... ``` *** ?å?®?¢?æ???ð???±?æ???å?¯?¼
-((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+Falseã ''' ``` ### tsugu_async config ```py from tsugu import config
+config.compact = True ''' æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
+config.remote_data_max_retry = 3 ''' è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ°
+''' config.bandori_station_token_name = "Tsugu" ''' bandori station token '''
+config.bandori_station_token = "ZtV4EX2K9Onb" ''' bandori station token '''
+config.disable_gacha_simulate_group_ids = [] ''' éè¦å³é­æ¨¡ææ½å¡çç¾¤
+''' ``` ```py from tsugu_async import config ... # ä¸ä¸é¢ç¸å ``` ***
+?å?®?¢?æ???ð???±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
 qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ --- Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-1.0.5/tsugu.egg-info/SOURCES.txt` & `tsugu-1.1.0rc1/tsugu.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 tsugu/config.py
 tsugu/handler.py
 tsugu.egg-info/PKG-INFO
 tsugu.egg-info/SOURCES.txt
 tsugu.egg-info/dependency_links.txt
 tsugu.egg-info/requires.txt
 tsugu.egg-info/top_level.txt
-tsugu/command_matcher/__init__.py
 tsugu/router/__init__.py
 tsugu/router/bandoristation/__init__.py
 tsugu/router/bandoristation/rooms_forward.py
 tsugu/router/bandoristation/ycm.py
 tsugu/router/remote/__init__.py
 tsugu/router/remote/bind_player.py
 tsugu/router/remote/bind_player_verification_off.py
@@ -26,30 +25,28 @@
 tsugu/router/remote/switch_car_forwarding_on.py
 tsugu/router/remote/unbind_player.py
 tsugu/router/universal/__init__.py
 tsugu/router/universal/event_stage.py
 tsugu/router/universal/gacha_simulate.py
 tsugu/router/universal/get_card_illustration.py
 tsugu/router/universal/lsycx.py
-tsugu/router/universal/room_list.py
 tsugu/router/universal/search_card.py
 tsugu/router/universal/search_character.py
 tsugu/router/universal/search_event.py
 tsugu/router/universal/search_gacha.py
 tsugu/router/universal/search_player.py
 tsugu/router/universal/search_song.py
 tsugu/router/universal/song_chart.py
 tsugu/router/universal/song_meta.py
 tsugu/router/universal/ycx.py
 tsugu/router/universal/ycx_all.py
 tsugu/utils/__init__.py
 tsugu_async/__init__.py
 tsugu_async/config.py
 tsugu_async/handler.py
-tsugu_async/command_matcher/__init__.py
 tsugu_async/router/__init__.py
 tsugu_async/router/bandoristation/__init__.py
 tsugu_async/router/bandoristation/rooms_forward.py
 tsugu_async/router/bandoristation/ycm.py
 tsugu_async/router/remote/__init__.py
 tsugu_async/router/remote/bind_player.py
 tsugu_async/router/remote/bind_player_verification_off.py
```

### Comparing `tsugu-1.0.5/tsugu_async/handler.py` & `tsugu-1.1.0rc1/tsugu_async/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Union, Dict
 
 from .utils import *
 from loguru import logger
 from tsugu_api import settings
 from . import router
 
+
 async def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
     :param message: 用户消息
     :param user_id: 用户ID
```

### Comparing `tsugu-1.0.5/tsugu_async/router/remote/bind_player.py` & `tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,30 @@
-from ...config import config
-from ...utils import text_response, User
-from ...command_matcher import MC
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api_async
-from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar, AllParam
+from tsugu_api_core._typing import _ServerName
+
+
+alc = Alconna(
+        ["绑定玩家"],
+    Args["args;?", AllParam],
+    meta=CommandMeta(
+            compact=config.compact, description="绑定玩家",
+            usage="只需发送‘绑定玩家’。",
+        ),
+    )
+
 
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
 
-async def handler(user: User, res: MC, platform: str, channel_id: str):
-    # 获取绑定请求
-    r = await tsugu_api_async.bind_player_request(platform, user.user_id, user.server_mode, True)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    return text_response(
-        f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字母缩写)\n例如：验证绑定 114****514 cn''')
+    if res.matched:
+        r = await tsugu_api_async.bind_player_request(platform, user.user_id, user.server_mode, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response(
+            f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字母缩写)\n例如：验证绑定 114****514 cn''')
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
```

### Comparing `tsugu-1.0.5/tsugu_async/router/remote/bind_player_verification_off.py` & `tsugu-1.1.0rc1/tsugu_async/router/remote/bind_player_verification_off.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,52 @@
-from ...utils import text_response, User
-from ...command_matcher import MC
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api_async
-from ...utils import server_exists, server_name_2_server_id
-from loguru import logger
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from tsugu_api_core._typing import _ServerName
 
 
-async def handler(user: User, res: MC, platform: str, channel_id: str):
-    if not res.args or len(res.args) > 1:
-        return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
-    if not res.args[0].isdigit():
-        return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
-    if int(res.text) <= 0:
-        return text_response('请输入正确的格式：验证解绑 记录编号(数字)，编号从1开始')
-    if len(user.game_ids) < int(res.text):
-        return text_response('未找到记录')
-    player_id = user.game_ids[int(res.args[0]) - 1].get("game_id")
-    server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
-    r = await tsugu_api_async.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    return text_response('解绑成功！')
+alc = Alconna(
+        ["验证解绑"],
+    Args["index#要解绑的绑定编号", int],
+        meta=CommandMeta(
+            compact=config.compact, description="验证解绑",
+            usage="验证解绑 记录编号(数字)",
+            example="验证解绑 1 : 解绑第一个记录"
+        ),
+    )
 
 
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        if len(user.game_ids) < int(res.index):
+            return text_response('未找到记录')
+        player_id = user.game_ids[int(res.index) - 1].get("game_id")
+        server_mode = user.game_ids[int(res.index) - 1].get("server")
+        r = await tsugu_api_async.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('解绑成功！')
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
+
+
+# def handler(user: User, res: MC, platform: str, channel_id: str):
+#     if not res.args or len(res.args) > 1:
+#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
+#     if not res.args[0].isdigit():
+#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
+#     if int(res.text) <= 0:
+#         return text_response('请输入正确的格式：验证解绑 记录编号(数字)，编号从1开始')
+#     if len(user.game_ids) < int(res.text):
+#         return text_response('未找到记录')
+#     player_id = user.game_ids[int(res.args[0]) - 1].get("game_id")
+#     server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
+#     r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
+#     if r.get('status') != 'success':
+#         return text_response(r.get('data'))
+#     return text_response('解绑成功！')
+#
+#
```

### Comparing `tsugu-1.0.5/tsugu_async/router/remote/bind_player_verification_on.py` & `tsugu-1.1.0rc1/tsugu/router/remote/bind_player_verification_on.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
+import tsugu_api
 from ...config import config
-from ...utils import text_response, User
-from ...command_matcher import MC
-import tsugu_api_async
-from ...utils import server_exists, server_name_2_server_id
-
-
-async def handler(user: User, res: MC, platform: str, channel_id: str):
-    if not res.args or len(res.args) < 2:
-        return text_response('请输入正确的格式：验证绑定 你的玩家ID(数字) 服务器名(字母缩写)')
-    player_id = int(res.args[0])
-    server_pre = server_name_2_server_id(res.args[1])
-    if not server_exists(server_pre):
-        return text_response('未找到服务器，请输入正确的服务器名')
-    user.server_mode = server_pre
-
-    r = await tsugu_api_async.bind_player_verification(platform, user.user_id, user.server_mode, player_id, True)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    return text_response(f'绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
-
-
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from tsugu_api_core._typing import _ServerName
 
+alc = Alconna(
+        ["验证绑定"],
+    Args["playerID#你的玩家ID(数字)", int]["serverName#服务器名(字母缩写)", _ServerName],
+        meta=CommandMeta(
+            compact=config.compact, description="验证绑定",)
+    )
+
+
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        server = server_name_2_server_id(res.serverName)
+        r = tsugu_api.bind_player_verification(platform, user.user_id, server, res.playerID, True)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response('绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
```

### Comparing `tsugu-1.0.5/tsugu_async/router/remote/change_server_mode.py` & `tsugu-1.1.0rc1/tsugu/router/remote/change_server_mode.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,42 @@
-from ...utils import text_response, User
-from ...command_matcher import MC
-import tsugu_api_async
-from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
-from tsugu_api._typing import _ServerId, _Update
-import typing
-
-
-async def handler(user: User, res: MC, platform: str, channel_id: str):
-    if res.args:
-        server_mode = server_name_2_server_id(res.args[0])
-        if not server_exists(server_mode):
-            return text_response('未找到服务器，请输入正确的服务器名')
-        update: _Update = {'server_mode': server_mode, }
-        r = await tsugu_api_async.change_user_data(platform, user.user_id, update)
-        if r:
-            if r.get('status') == 'success':
-                return text_response('主服务器已设置为 ' + server_id_2_server_name(server_mode))
+from ...utils import text_response, User, server_name_2_server_id
+import tsugu_api
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager, MultiVar
+from tsugu_api_core._typing import _ServerName
+
+alc = Alconna(
+        ["主服务器", "设置主服务器"],
+    Args["serverName#服务器名", _ServerName],
+        meta=CommandMeta(
+            compact=config.compact, description="主服务器",
+            usage="将指定的服务器设置为你的主服务器。",
+            example="""主服务器 cn : 将国服设置为主服务器。"""
+
+        )
+    )
+
+
+def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        r = tsugu_api.change_user_data(platform, user.user_id, {'server_mode': server_name_2_server_id(res.serverName)})
+        if r.get('status') != 'success':
             return text_response(r.get('data'))
+        return text_response('主服务器已设置为 ' + res.serverName)
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
 
+#
+# def handler(user: User, res: MC, platform: str, channel_id: str):
+#     if res.args:
+#         server_mode = server_name_2_server_id(res.args[0])
+#         if not server_exists(server_mode):
+#             return text_response('未找到服务器，请输入正确的服务器名')
+#         update: _Update = {'server_mode': server_mode, }
+#         if r := tsugu_api.change_user_data(platform, user.user_id, update):
+#             if r.get('status') == 'success':
+#                 return text_response('主服务器已设置为 ' + server_id_2_server_name(server_mode))
+#             return text_response(r.get('data'))
+#
```

### Comparing `tsugu-1.0.5/tsugu_async/router/remote/unbind_player.py` & `tsugu-1.1.0rc1/tsugu_async/router/remote/unbind_player.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,50 @@
-from ...utils import text_response, User
-from ...command_matcher import MC
+from ...utils import text_response, User, server_id_2_server_name, server_name_2_server_id, server_exists
 import tsugu_api_async
-from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from tsugu_api_core._typing import _ServerName
+
+
+alc = Alconna(
+        ["解除绑定"],
+    Args["index#要解绑的绑定编号", int, None],
+        meta=CommandMeta(
+            compact=config.compact, description="解除绑定",
+            usage="验证解绑 记录编号(数字)",
+            example="验证解绑 1 : 解绑第一个记录"
+        ),
+    )
+
+
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        if not res.index:
+            bind_record = '\n'.join([f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in enumerate(user.game_ids)])
+            return text_response('请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n' + bind_record)
+
+        if len(user.game_ids) < int(res.index):
+            return text_response('未找到记录')
+
+        server_mode = user.game_ids[int(res.index) - 1].get("server")
+
+        r = await tsugu_api_async.bind_player_request(platform, user.user_id, server_mode, False)
+        if r.get('status') != 'success':
+            return text_response(r.get('data'))
+        return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.index}\n来完成本次身份验证''')
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
 
 
 def mask_data(game_id: str):
     game_id = str(game_id)
     if len(game_id) < 6:
         return game_id[:3] + '*' * (len(game_id) - 3)
     elif len(game_id) < 3:
         return '*' * len(game_id)
     else:
         game_id = game_id[:3] + '*' * (len(game_id) - 6) + game_id[-3:]
     return game_id
 
-
-async def handler(user: User, res: MC, platform: str, channel_id: str):
-    bind_record = '\n'.join(
-        [f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in
-         enumerate(user.game_ids)])
-    if not res.args:
-        return text_response(f'请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n{bind_record}')
-
-    if not res.args[0].isdigit():
-        return text_response(f'请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n{bind_record}')
-
-    if int(res.args[0]) > len(user.game_ids):
-        return text_response(f'未找到记录 {res.args[0]}，当前的绑定记录如下:\n{bind_record}')
-
-    server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
-    r = await tsugu_api_async.bind_player_request(platform, user.user_id, server_mode, False)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    # 如果是200
-    return text_response(
-        f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.args[0]}\n来完成本次身份验证''')
-
-
```

### Comparing `tsugu-1.0.5/tsugu_async/router/universal/event_stage.py` & `tsugu-1.1.0rc1/tsugu_async/router/universal/search_gacha.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from ...config import config
-from ...utils import text_response, User, server_exists
-from ...command_matcher import MC
+from ...utils import text_response, User
 import tsugu_api_async
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+
+
+alc = Alconna(
+        ["查卡池"],
+        Args["gachaId#可以通过查活动、查卡等获取", str],
+        meta=CommandMeta(
+            compact=config.compact, description="查卡池",
+            usage='根据卡池ID查询卡池信息',
+        )
+    )
+
 
-async def handler(user: User, res: MC, platform: str, channel_id: str):
-    if res.args:
-        #     最后一个参数
-        # if server_exists(name_2_index(res.args[-1])):
-        #     user.server_mode = name_2_index(res.args[-1])
-        event_id_pre: str = res.args[0]
-        # if event_id_pre.isdigit():
-        #     event_id = int(event_id_pre)
-        #     return tsugu_api.event_stage(user.server_mode, event_id=event_id, meta=False)
-        if res.text == '-m':
-            return await tsugu_api_async.event_stage(user.server_mode, meta=True)
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
 
-    return await tsugu_api_async.event_stage(user.server_mode, meta=False)
+    if res.matched:
+        return await tsugu_api_async.search_gacha(user.default_server, res.gachaId)
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
```

### Comparing `tsugu-1.0.5/tsugu_async/router/universal/ycx_all.py` & `tsugu-1.1.0rc1/tsugu_async/router/universal/song_meta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,31 @@
-from ...config import config
-from ...utils import text_response, User, server_exists, server_name_2_server_id
-from ...command_matcher import MC
+from ...utils import text_response, User, server_name_2_server_id
 import tsugu_api_async
+from ...config import config
+from arclet.alconna import Alconna, Option, Subcommand, Args, CommandMeta, Empty, Namespace, namespace, command_manager
+from tsugu_api_core._typing import _ServerName
 
 
-async def handler(user: User, res: MC, platform: str, channel_id: str):
-    # 无参数
-    if not res.args:
-        return await tsugu_api_async.ycx_all(user.server_mode)
-
-    # 一个参数
-    if len(res.args) == 1:
-        # 两个参数都是数字
-        if res.args[0].isdigit():
-            if res.args[0].isdigit():
-                event_id: int = int(res.args[0])
-            else:
-                return text_response('请输入正确的活动ID')
-            return await tsugu_api_async.ycx_all(user.server_mode, event_id)
-        elif server_exists(server_pre := server_name_2_server_id(res.args[0])):
-            user.server_mode = server_pre
-            return await tsugu_api_async.ycx_all(user.server_mode)
-        else:
-            return text_response('请输入正确的活动ID或服务器名称字母简写')
+alc = Alconna(
+        ["查询分数表", '查分数表', '查询分数榜', '查分数榜'],
+        Args["serverName;?#省略服务器名时，默认从你当前的主服务器查询。", _ServerName.__args__],
+        meta=CommandMeta(
+            compact=config.compact, description="查询分数表",
+            usage='查询指定服务器的歌曲分数表。',
+            example='''查询分数表 cn :返回国服的歌曲分数表'''
+        )
+    )
 
-    if len(res.args) == 2:
-        # 两个参数是 event_id server_mode
-        if res.args[0].isdigit():
-            event_id: int = int(res.args[0])
-        else:
-            return text_response('第一个参数请输入正确的活动ID')
-        if server_exists(server_pre := server_name_2_server_id(res.args[1])):
-            user.server_mode = server_pre
-            return await tsugu_api_async.ycx_all(user.server_mode, event_id)
+
+async def handler(message: str, user: User, platform: str, channel_id: str):
+    res = alc.parse(message)
+
+    if res.matched:
+        if res.serverName:
+            server = server_name_2_server_id(res.serverName)
         else:
-            return text_response('第二个参数请输入正确的服务器名称字母简写')
+            server = user.server_mode
+        return await tsugu_api_async.song_meta(user.default_server, server)
+    elif res.head_matched:
+        return text_response(res.error_info)
+    return None
 
-    return text_response('参数过多(<=2)')
```

### Comparing `tsugu-1.0.5/tsugu_async/utils/__init__.py` & `tsugu-1.1.0rc1/tsugu_async/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,107 @@
 import typing
 from typing import List
 
 from ..config import config
-
-from tsugu_api._typing import _ServerId
 import tsugu_api_async
-import time
 from loguru import logger
-import asyncio
-from typing import Optional
+import time
 
+from tsugu_api_core._typing import _ServerId
 
-class User:
-    def __init__(self, user_id: str, platform: str, server_mode: _ServerId, default_server: List[_ServerId], car: bool, server_list: list, game_ids: list, verify_code: str):
-        self.user_id: str = user_id
-        self.platform: str = platform
-        self.server_mode: _ServerId = server_mode
-        self.default_server: List[_ServerId] = default_server
-        self.car: bool = car
-        self.server_list: list = server_list
-        self.game_ids = game_ids
-        self.verify_code = verify_code
+
+_i_s = {0: "jp", 1: "en", 2: "tw", 3: "cn", 4: "kr"}
+_s_i = {"jp": 0, "en": 1, "tw": 2, "cn": 3, "kr": 4}
 
 
 def text_response(string):
-    return [{"type": "string", "string": string}]
+    return [{"type": "string", "string": str(string)}]
 
 
 def server_names_2_server_ids(server_name: List[str]) -> List[_ServerId]:
-    return [config._s_i[code] for code in server_name]
+    return [_s_i[code] for code in server_name]
 
 
 def server_name_2_server_id(server_name: str) -> _ServerId:
-    return config._s_i[server_name] if server_name in config._s_i else None
+    return _s_i[server_name] if server_name in _s_i else None
 
 
 def server_ids_2_server_names(index: List[_ServerId]) -> List[str]:
-    return [config._i_s[code] for code in index]
+    return [_i_s[code] for code in index]
 
 
 def server_id_2_server_name(index: _ServerId) -> str:
-    return config._i_s[index] if index in config._i_s else None
+    return _i_s[index] if index in _i_s else None
 
 
 def server_exists(server):
     if server or server == 0:
         return True
     if not server:
         return False
     return False
 
 
-async def get_user(user_id: str, platform: str) -> Optional[User]:
-    for i in range(0, config.get_remote_user_data_max_retry):
+class User:
+    def __init__(self, user_id: str, platform: str, server_mode: _ServerId, default_server: List[_ServerId], car: bool, server_list: list, game_ids: list, verify_code: str):
+        self.user_id: str = user_id
+        self.platform: str = platform
+        self.server_mode: _ServerId = server_mode
+        self.default_server: List[_ServerId] = default_server
+        self.car: bool = car
+        self.server_list: list = server_list
+        self.game_ids = game_ids
+        self.verify_code = verify_code
+
+
+async def get_user(user_id: str, platform: str) -> User:
+    '''
+    获取用户数据
+    多次尝试获取用户数据
+    兼容旧版用户数据
+
+    :param user_id:
+    :param platform:
+    :return:
+    '''
+    for i in range(0, config.remote_data_max_retry):
         try:
             user_data_res = await tsugu_api_async.get_user_data(platform, user_id)
             if user_data_res.get('status') == 'failed':
-                return None
+                return text_response(user_data_res.get('data'))
             break
         except Exception as e:
             logger.error(f'Error: {e}')
-            time.sleep(0.5)
+            time.sleep(0.8)
             continue
     else:
-        return None
+        raise Exception('获取用户数据失败')
 
-    # 旧数据兼容
+    # 获取用户数据失败
+    if user_data_res.get('status') == 'failed':
+        return text_response(user_data_res.get('data'))
+    # 构建用户对象
     user_data = user_data_res.get('data')
+
     if user_data.get('game_ids') is None:
 
         user_data['game_ids'] = []
         for i in range(0, 5):
-            if user_data.get('server_list')[i]['playerId'] != 0:  # type: ignore
-                new_game_id = {"game_id": user_data.get('server_list')[i]['playerId'], "server": i}  # type: ignore
-                user_data['game_ids'].append(new_game_id)  # type: ignore
+            if user_data.get('server_list')[i]['playerId'] != 0:
+                new_game_id = {"game_id": user_data.get('server_list')[i]['playerId'], "server": i}
+                user_data['game_ids'].append(new_game_id)
         verify_code_all = []
         for i in range(0, 5):
             if user_data.get('server_list')[i].get('verifyCode') is not None:
                 verify_code_all.append(i)
-        # 有一说一，下面这行没有实际意义
-        user_data['verify_code'] = '或'.join(
-            [str(user_data.get('server_list')[i].get('verifyCode')) for i in verify_code_all]) if len(
-            verify_code_all) > 1 else verify_code_all[0] if verify_code_all else ''
 
-    # 构建用户对象
     user = User(user_id=user_id,
                 platform=platform,
-                server_mode=user_data.get('server_mode'),  # type: ignore
-                default_server=user_data.get('default_server'),  # type: ignore
-                car=user_data.get('car'),  # type: ignore
-                server_list=user_data.get('server_list', None),  # type: ignore
-                game_ids=user_data.get('game_ids', []),  # type: ignore
-                verify_code=user_data.get('verify_code'))  # type: ignore
+                server_mode=user_data.get('server_mode'),
+                default_server=user_data.get('default_server'),
+                car=user_data.get('car'),
+                server_list=user_data.get('server_list', None),
+                game_ids=user_data.get('game_ids', []),
+                verify_code=user_data.get('verify_code'))
     return user
 
 
-
```


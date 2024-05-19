# Comparing `tmp/tautulli-4.2.1.2140b0.tar.gz` & `tmp/tautulli-4.2.2.2140b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tautulli-4.2.1.2140b0.tar", last modified: Mon May 13 01:38:06 2024, max compression
+gzip compressed data, was "tautulli-4.2.2.2140b0.tar", last modified: Sun May 19 22:58:40 2024, max compression
```

## Comparing `tautulli-4.2.1.2140b0.tar` & `tautulli-4.2.2.2140b0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.975376 tautulli-4.2.1.2140b0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-13 01:38:06.975376 tautulli-4.2.1.2140b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 01:38:06.979376 tautulli-4.2.1.2140b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-13 01:37:42.000000 tautulli-4.2.1.2140b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.959376 tautulli-4.2.1.2140b0/tautulli/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/API_VERSIONS.json
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/PYTHON_VERSIONS.json
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.963376 tautulli-4.2.1.2140b0/tautulli/api/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    97885 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/api/json_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    67947 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/api/object_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.963376 tautulli-4.2.1.2140b0/tautulli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/exceptions/api_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/exceptions/base_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/exceptions/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/exceptions/json_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.963376 tautulli-4.2.1.2140b0/tautulli/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/internal/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.975376 tautulli-4.2.1.2140b0/tautulli/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/children_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/collections_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/date_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/export_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/exports_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/geo_ip_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/get_plays_or_stream_types_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/home_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/item_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/item_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/libraries_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/library_media_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/library_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/library_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/library_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/new_rating_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/newsletter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/newsletter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/newsletter_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/newsletter_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/notification_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/notifier_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/notifier_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/notifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/old_rating_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/playlists_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/plex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/pms_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/recently_added.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/registered_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/search_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/server_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/server_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/server_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/server_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/server_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/servers_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    30292 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/stream_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/synced_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/tautulli_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/update_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/user_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/user_logins.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/user_player_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/user_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/usernames.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/users_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/models/whois_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.975376 tautulli-4.2.1.2140b0/tautulli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/tools/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.975376 tautulli-4.2.1.2140b0/tautulli/tools/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/tools/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tautulli/tools/webhooks/discord.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.975376 tautulli-4.2.1.2140b0/tautulli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-13 01:38:06.000000 tautulli-4.2.1.2140b0/tautulli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 01:38:06.000000 tautulli-4.2.1.2140b0/tautulli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 01:38:06.000000 tautulli-4.2.1.2140b0/tautulli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 01:38:06.000000 tautulli-4.2.1.2140b0/tautulli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 01:38:06.000000 tautulli-4.2.1.2140b0/tautulli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:38:06.975376 tautulli-4.2.1.2140b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tests/test_json_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tests/test_object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 01:37:41.000000 tautulli-4.2.1.2140b0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.169218 tautulli-4.2.2.2140b0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-19 22:58:40.169218 tautulli-4.2.2.2140b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-19 22:58:40.173218 tautulli-4.2.2.2140b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-19 22:58:18.000000 tautulli-4.2.2.2140b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.153218 tautulli-4.2.2.2140b0/tautulli/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/API_VERSIONS.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/PYTHON_VERSIONS.json
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.157218 tautulli-4.2.2.2140b0/tautulli/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97885 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/api/json_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67947 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/api/object_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.157218 tautulli-4.2.2.2140b0/tautulli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/exceptions/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/exceptions/base_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/exceptions/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/exceptions/json_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.157218 tautulli-4.2.2.2140b0/tautulli/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/internal/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.169218 tautulli-4.2.2.2140b0/tautulli/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/children_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/collections_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/export_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/exports_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/geo_ip_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/get_plays_or_stream_types_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/home_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/item_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/item_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/libraries_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/library_media_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/library_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/library_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/library_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/new_rating_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/newsletter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/newsletter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/newsletter_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/newsletter_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/notification_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/notifier_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/notifier_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/old_rating_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/playlists_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/plex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/pms_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/recently_added.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/registered_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/search_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/server_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/server_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/server_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/servers_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30292 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/synced_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/tautulli_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/update_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/user_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/user_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/user_player_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/user_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/usernames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/users_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/models/whois_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.169218 tautulli-4.2.2.2140b0/tautulli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/tools/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.169218 tautulli-4.2.2.2140b0/tautulli/tools/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/tools/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tautulli/tools/webhooks/discord.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.169218 tautulli-4.2.2.2140b0/tautulli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-19 22:58:40.000000 tautulli-4.2.2.2140b0/tautulli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-19 22:58:40.000000 tautulli-4.2.2.2140b0/tautulli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:58:40.000000 tautulli-4.2.2.2140b0/tautulli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-19 22:58:40.000000 tautulli-4.2.2.2140b0/tautulli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 22:58:40.000000 tautulli-4.2.2.2140b0/tautulli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:58:40.169218 tautulli-4.2.2.2140b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tests/test_json_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tests/test_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-19 22:58:17.000000 tautulli-4.2.2.2140b0/tests/test_utils.py
```

### Comparing `tautulli-4.2.1.2140b0/LICENSE` & `tautulli-4.2.2.2140b0/LICENSE`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/PKG-INFO` & `tautulli-4.2.2.2140b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tautulli
-Version: 4.2.1.2140b0
+Version: 4.2.2.2140b0
 Summary: A complete Python client for Tautulli's API
 Home-page: https://github.com/nwithan8/pytulli
-Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/4.2.1.2140b0.tar.gz
+Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/4.2.2.2140b0.tar.gz
 Author: Nate Harris
 Author-email: n8gr8gbln@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: Tautulli,API,client,Plex,PMS,Plex Media Server,media,server,JSON
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tautulli-4.2.1.2140b0/README.md` & `tautulli-4.2.2.2140b0/README.md`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/setup.py` & `tautulli-4.2.2.2140b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 from typing import List
 
 import setuptools
 
-__version__ = '4.2.1.2140b0'
+__version__ = '4.2.2.2140b0'
 
 __title__ = "tautulli"
 __author__ = 'Nate Harris'
 __author_email__ = 'n8gr8gbln@gmail.com'
 __github_username__ = "nwithan8"
 __github_repo__ = "pytulli"
 __copyright__ = "Copyright © 2024 - Nate Harris"
```

### Comparing `tautulli-4.2.1.2140b0/tautulli/api/json_api.py` & `tautulli-4.2.2.2140b0/tautulli/api/json_api.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/api/object_api.py` & `tautulli-4.2.2.2140b0/tautulli/api/object_api.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/exceptions/http_exception.py` & `tautulli-4.2.2.2140b0/tautulli/exceptions/http_exception.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/exceptions/json_exception.py` & `tautulli-4.2.2.2140b0/tautulli/exceptions/json_exception.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/internal/decorators.py` & `tautulli-4.2.2.2140b0/tautulli/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/internal/static.py` & `tautulli-4.2.2.2140b0/tautulli/internal/static.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/internal/utils.py` & `tautulli-4.2.2.2140b0/tautulli/internal/utils.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/__init__.py` & `tautulli-4.2.2.2140b0/tautulli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/activity.py` & `tautulli-4.2.2.2140b0/tautulli/models/activity.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/children_metadata.py` & `tautulli-4.2.2.2140b0/tautulli/models/children_metadata.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/collections_table.py` & `tautulli-4.2.2.2140b0/tautulli/models/collections_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/docs.py` & `tautulli-4.2.2.2140b0/tautulli/models/docs.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/export_fields.py` & `tautulli-4.2.2.2140b0/tautulli/models/export_fields.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/exports_table.py` & `tautulli-4.2.2.2140b0/tautulli/models/exports_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/geo_ip_lookup.py` & `tautulli-4.2.2.2140b0/tautulli/models/geo_ip_lookup.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/history.py` & `tautulli-4.2.2.2140b0/tautulli/models/history.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/home_stats.py` & `tautulli-4.2.2.2140b0/tautulli/models/home_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/libraries.py` & `tautulli-4.2.2.2140b0/tautulli/models/libraries.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/libraries_table.py` & `tautulli-4.2.2.2140b0/tautulli/models/libraries_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/library.py` & `tautulli-4.2.2.2140b0/tautulli/models/library.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/library_media_info.py` & `tautulli-4.2.2.2140b0/tautulli/models/library_media_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/metadata.py` & `tautulli-4.2.2.2140b0/tautulli/models/metadata.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/newsletter_config.py` & `tautulli-4.2.2.2140b0/tautulli/models/newsletter_config.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/newsletter_log.py` & `tautulli-4.2.2.2140b0/tautulli/models/newsletter_log.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/notification_log.py` & `tautulli-4.2.2.2140b0/tautulli/models/notification_log.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/notifier_config.py` & `tautulli-4.2.2.2140b0/tautulli/models/notifier_config.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/parser.py` & `tautulli-4.2.2.2140b0/tautulli/models/parser.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/playlists_table.py` & `tautulli-4.2.2.2140b0/tautulli/models/playlists_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/pms_update.py` & `tautulli-4.2.2.2140b0/tautulli/models/pms_update.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/recently_added.py` & `tautulli-4.2.2.2140b0/tautulli/models/recently_added.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/registered_device.py` & `tautulli-4.2.2.2140b0/tautulli/models/registered_device.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/search_results.py` & `tautulli-4.2.2.2140b0/tautulli/models/search_results.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/server_info.py` & `tautulli-4.2.2.2140b0/tautulli/models/server_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/server_list.py` & `tautulli-4.2.2.2140b0/tautulli/models/server_list.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/settings.py` & `tautulli-4.2.2.2140b0/tautulli/models/settings.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/stream_data.py` & `tautulli-4.2.2.2140b0/tautulli/models/stream_data.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/synced_items.py` & `tautulli-4.2.2.2140b0/tautulli/models/synced_items.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/tautulli_info.py` & `tautulli-4.2.2.2140b0/tautulli/models/tautulli_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/user.py` & `tautulli-4.2.2.2140b0/tautulli/models/user.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/user_ips.py` & `tautulli-4.2.2.2140b0/tautulli/models/user_ips.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/user_logins.py` & `tautulli-4.2.2.2140b0/tautulli/models/user_logins.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/users.py` & `tautulli-4.2.2.2140b0/tautulli/models/users.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/users_table.py` & `tautulli-4.2.2.2140b0/tautulli/models/users_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/models/whois_lookup.py` & `tautulli-4.2.2.2140b0/tautulli/models/whois_lookup.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/tools/api_helper.py` & `tautulli-4.2.2.2140b0/tautulli/tools/api_helper.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/tools/utils.py` & `tautulli-4.2.2.2140b0/tautulli/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli/tools/webhooks/discord.py` & `tautulli-4.2.2.2140b0/tautulli/tools/webhooks/discord.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tautulli.egg-info/PKG-INFO` & `tautulli-4.2.2.2140b0/tautulli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tautulli
-Version: 4.2.1.2140b0
+Version: 4.2.2.2140b0
 Summary: A complete Python client for Tautulli's API
 Home-page: https://github.com/nwithan8/pytulli
-Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/4.2.1.2140b0.tar.gz
+Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/4.2.2.2140b0.tar.gz
 Author: Nate Harris
 Author-email: n8gr8gbln@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: Tautulli,API,client,Plex,PMS,Plex Media Server,media,server,JSON
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tautulli-4.2.1.2140b0/tautulli.egg-info/SOURCES.txt` & `tautulli-4.2.2.2140b0/tautulli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tests/test_json_api.py` & `tautulli-4.2.2.2140b0/tests/test_json_api.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tests/test_object_api.py` & `tautulli-4.2.2.2140b0/tests/test_object_api.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.2.1.2140b0/tests/test_shortcuts.py` & `tautulli-4.2.2.2140b0/tests/test_shortcuts.py`

 * *Files identical despite different names*


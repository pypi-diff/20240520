# Comparing `tmp/feedcrawler-19.1.0.tar.gz` & `tmp/feedcrawler-19.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedcrawler-19.1.0.tar", last modified: Sat Apr 13 11:00:03 2024, max compression
+gzip compressed data, was "feedcrawler-19.2.0.tar", last modified: Sun May 19 11:45:42 2024, max compression
```

## Comparing `feedcrawler-19.1.0.tar` & `feedcrawler-19.2.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.670682 feedcrawler-19.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-13 11:00:03.670682 feedcrawler-19.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     6823 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.658681 feedcrawler-19.1.0/feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.658681 feedcrawler-19.1.0/feedcrawler/external_sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.658681 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44484 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.662681 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
--rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.662681 feedcrawler-19.1.0/feedcrawler/external_sites/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/metadata/imdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.662681 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.662681 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.662681 feedcrawler-19.1.0/feedcrawler/external_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42961 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_tools/myjd_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_tools/ombi_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_tools/overseerr_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/external_tools/plex_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.662681 feedcrawler-19.1.0/feedcrawler/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15005 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/jobs/feed_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    20746 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/jobs/package_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.666682 feedcrawler-19.1.0/feedcrawler/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23773 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.666682 feedcrawler-19.1.0/feedcrawler/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    44221 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/myjd_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/url_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.666682 feedcrawler-19.1.0/feedcrawler/web_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.658681 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.666682 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.670682 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    91095 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-Bix6I8bK.js
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@meforma-Cn7fFUfm.js
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@meforma-D0j6vHqc.css
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-WhmJkuoZ.js
--rw-r--r--   0 runner    (1001) docker     (127)    66277 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-DxhzX8GC.js
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-C2nz7ynZ.js
--rw-r--r--   0 runner    (1001) docker     (127)    29744 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-Cm0UX6qg.js
--rw-r--r--   0 runner    (1001) docker     (127)   231929 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-DUEfxN0n.css
--rw-r--r--   0 runner    (1001) docker     (127)    60814 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-DZKer8Tf.js
--rw-r--r--   0 runner    (1001) docker     (127)   176032 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-BOrJxbIo.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130396 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-BtvjY1KL.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    79729 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-Cb-KCKU4.css
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-BAhsgUwW.css
--rw-r--r--   0 runner    (1001) docker     (127)   147441 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-C4FFZX5g.js
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-LriLsbSV.css
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-l0sNRNKZ.js
--rw-r--r--   0 runner    (1001) docker     (127)    22928 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-Dqxmm31T.js
--rw-r--r--   0 runner    (1001) docker     (127)    51640 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-jXauJNZF.js
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-C5iuhTWR.js
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-C8dxsqXw.js
--rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    84539 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/feedcrawler/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:00:03.658681 feedcrawler-19.1.0/feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 11:00:03.000000 feedcrawler-19.1.0/feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 11:00:03.670682 feedcrawler-19.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-13 10:59:45.000000 feedcrawler-19.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.811183 feedcrawler-19.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-19 11:45:42.811183 feedcrawler-19.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7975 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.799183 feedcrawler-19.2.0/feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.799183 feedcrawler-19.2.0/feedcrawler/external_sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.799183 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44484 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.799183 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.803182 feedcrawler-19.2.0/feedcrawler/external_sites/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/metadata/imdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.803182 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.803182 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.803182 feedcrawler-19.2.0/feedcrawler/external_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42961 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_tools/myjd_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_tools/ombi_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_tools/overseerr_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/external_tools/plex_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.803182 feedcrawler-19.2.0/feedcrawler/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15005 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/jobs/feed_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20746 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/jobs/package_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.807182 feedcrawler-19.2.0/feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23773 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.807182 feedcrawler-19.2.0/feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44221 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/myjd_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/url_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.807182 feedcrawler-19.2.0/feedcrawler/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.795183 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.807182 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.811183 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    91095 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-Bix6I8bK.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@meforma-Cn7fFUfm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@meforma-D0j6vHqc.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-WhmJkuoZ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    66277 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-DxhzX8GC.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-C2nz7ynZ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29744 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-Cm0UX6qg.js
+-rw-r--r--   0 runner    (1001) docker     (127)   231929 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-DUEfxN0n.css
+-rw-r--r--   0 runner    (1001) docker     (127)    60814 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-DZKer8Tf.js
+-rw-r--r--   0 runner    (1001) docker     (127)   176032 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-BOrJxbIo.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130396 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-BtvjY1KL.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    79729 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-Cb-KCKU4.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-BAhsgUwW.css
+-rw-r--r--   0 runner    (1001) docker     (127)   147441 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-C4FFZX5g.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-LriLsbSV.css
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-l0sNRNKZ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22928 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-Dqxmm31T.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51640 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-jXauJNZF.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-C5iuhTWR.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-C8dxsqXw.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    84539 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/feedcrawler/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:45:42.799183 feedcrawler-19.2.0/feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 11:45:42.000000 feedcrawler-19.2.0/feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:45:42.811183 feedcrawler-19.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-19 11:45:23.000000 feedcrawler-19.2.0/setup.py
```

### Comparing `feedcrawler-19.1.0/LICENSE.md` & `feedcrawler-19.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/PKG-INFO` & `feedcrawler-19.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: feedcrawler
-Version: 19.1.0
-Summary: Automate downloads using predefined sites and the My JDownloader API
-Home-page: https://github.com/rix1337/FeedCrawler
-Author: rix1337
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # FeedCrawler
 
 <img src="https://raw.githubusercontent.com/rix1337/FeedCrawler/main/feedcrawler/web_interface/vuejs_frontend/public/favicon.ico" data-canonical-src="https://raw.githubusercontent.com/rix1337/FeedCrawler/main/feedcrawler/web_interface/vuejs_frontend/public/favicon.ico" width="64" height="64" />
 
 FeedCrawler automatisiert bequem das Hinzufügen von Links für den JDownloader.
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rix1337/FeedCrawler/CreateRelease.yml?branch=main)](https://github.com/rix1337/FeedCrawler/actions/workflows/CreateRelease.yml)
@@ -69,22 +54,50 @@
 
 ### Start
 
 ```feedcrawler``` in der Konsole (Python muss im System-PATH hinterlegt sein)
 
 ### [Docker Image](https://hub.docker.com/r/rix1337/docker-feedcrawler/)
 
+```
+docker run -d \
+  --name="FeedCrawler" \
+  -p port:9090 \
+  -v /path/to/config/:/config:rw \
+  -e USER=NUTZERNAME \ 
+  -e PASS=PASSWORT \
+  -e DEVICE=GERÄTENAME \
+  -e DELAY=30 \
+  -e LOGLEVEL=[INFO/DEBUG/WARNING/ERROR/CRITICAL/NOTSET] \
+  --log-opt max-size=50m \
+  rix1337/docker-feedcrawler
+  ```
+
 * Der Betrieb als Docker-Container empfiehlt sich als Standardinstallation - vor allem für NAS-Systeme, Homeserver und
   sonstige Geräte die dauerhaft und möglichst wartungsfrei (headless) betrieben werden sollen.
 * Bei jedem Release wird ein getaggtes Image erstellt. Damit kann man auf der Wunschversion verbleiben oder im Falle
   eines Bugs zu einer stabilen Version zurück kehren.
 * Um immer auf dem aktuellen Stand zu sein, einfach das mit `latest` getaggte Image nutzen.
 * Für UNRAID-Server kann das Image direkt über die Community Applications bezogen und der Container so eingerichtet
   werden.
 
+##### Optionale Parameter
+ - `-e USER` (ab dem ersten Start, sofern unverändert)
+ - `-e PASS` (ab dem ersten Start, sofern unverändert)
+ - `-e DEVICE` (immer, sofern nur ein Gerät im MyJD-Konto vorhanden ist, sonst ab dem ersten Start, sofern unverändert)
+ - `-e DELAY` (immer, sofern der erste Suchlauf nach Start nicht um diese ganze Zahl in Sekunden verzögert werden soll)
+
+##### Spezifische Version nutzen
+
+Das Image `rix1377/docker-feedcrawler` wird standardmäßig auf das `:latest`-Tag aufgelöst. Dieses wird mit jedem Release auf die neue Version aktualisiert. Mit jedem Release wird ebenfalls eine getaggte Version des Images erzeugt. Auf letztere kann man wechseln, um beispielsweise bei Fehlern in der neuen Version auf einen funktionierenden Stand zurück zu kehren.
+
+Beispiel:
+
+`docker pull rix1337/docker-feedcrawler:13.0.3`
+
 ### Windows Build
 
 * Jedem [Release](https://github.com/rix1337/FeedCrawler/releases) wird eine selbstständig unter Windows lauffähige
   Version des FeedCrawlers beigefügt.
 * Hierfür müssen weder Python, noch die Zusatzpakete installiert werden.
 * Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
 
@@ -117,9 +130,7 @@
 
 Es empfiehlt sich, zusätzlich einen Reverse-Proxy mit HTTPs-Zertifikat,
 bspw. [kostenlos von letsencrypt](https://letsencrypt.org/), zu verwenden.
 
 ## Credits
 
 * [mmarquezs](https://github.com/mmarquezs/) (My JDownloader-API für Python)
-
-
```

### Comparing `feedcrawler-19.1.0/README.md` & `feedcrawler-19.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: feedcrawler
+Version: 19.2.0
+Summary: Automate downloads using predefined sites and the My JDownloader API
+Home-page: https://github.com/rix1337/FeedCrawler
+Author: rix1337
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # FeedCrawler
 
 <img src="https://raw.githubusercontent.com/rix1337/FeedCrawler/main/feedcrawler/web_interface/vuejs_frontend/public/favicon.ico" data-canonical-src="https://raw.githubusercontent.com/rix1337/FeedCrawler/main/feedcrawler/web_interface/vuejs_frontend/public/favicon.ico" width="64" height="64" />
 
 FeedCrawler automatisiert bequem das Hinzufügen von Links für den JDownloader.
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rix1337/FeedCrawler/CreateRelease.yml?branch=main)](https://github.com/rix1337/FeedCrawler/actions/workflows/CreateRelease.yml)
@@ -54,22 +69,50 @@
 
 ### Start
 
 ```feedcrawler``` in der Konsole (Python muss im System-PATH hinterlegt sein)
 
 ### [Docker Image](https://hub.docker.com/r/rix1337/docker-feedcrawler/)
 
+```
+docker run -d \
+  --name="FeedCrawler" \
+  -p port:9090 \
+  -v /path/to/config/:/config:rw \
+  -e USER=NUTZERNAME \ 
+  -e PASS=PASSWORT \
+  -e DEVICE=GERÄTENAME \
+  -e DELAY=30 \
+  -e LOGLEVEL=[INFO/DEBUG/WARNING/ERROR/CRITICAL/NOTSET] \
+  --log-opt max-size=50m \
+  rix1337/docker-feedcrawler
+  ```
+
 * Der Betrieb als Docker-Container empfiehlt sich als Standardinstallation - vor allem für NAS-Systeme, Homeserver und
   sonstige Geräte die dauerhaft und möglichst wartungsfrei (headless) betrieben werden sollen.
 * Bei jedem Release wird ein getaggtes Image erstellt. Damit kann man auf der Wunschversion verbleiben oder im Falle
   eines Bugs zu einer stabilen Version zurück kehren.
 * Um immer auf dem aktuellen Stand zu sein, einfach das mit `latest` getaggte Image nutzen.
 * Für UNRAID-Server kann das Image direkt über die Community Applications bezogen und der Container so eingerichtet
   werden.
 
+##### Optionale Parameter
+ - `-e USER` (ab dem ersten Start, sofern unverändert)
+ - `-e PASS` (ab dem ersten Start, sofern unverändert)
+ - `-e DEVICE` (immer, sofern nur ein Gerät im MyJD-Konto vorhanden ist, sonst ab dem ersten Start, sofern unverändert)
+ - `-e DELAY` (immer, sofern der erste Suchlauf nach Start nicht um diese ganze Zahl in Sekunden verzögert werden soll)
+
+##### Spezifische Version nutzen
+
+Das Image `rix1377/docker-feedcrawler` wird standardmäßig auf das `:latest`-Tag aufgelöst. Dieses wird mit jedem Release auf die neue Version aktualisiert. Mit jedem Release wird ebenfalls eine getaggte Version des Images erzeugt. Auf letztere kann man wechseln, um beispielsweise bei Fehlern in der neuen Version auf einen funktionierenden Stand zurück zu kehren.
+
+Beispiel:
+
+`docker pull rix1337/docker-feedcrawler:13.0.3`
+
 ### Windows Build
 
 * Jedem [Release](https://github.com/rix1337/FeedCrawler/releases) wird eine selbstständig unter Windows lauffähige
   Version des FeedCrawlers beigefügt.
 * Hierfür müssen weder Python, noch die Zusatzpakete installiert werden.
 * Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
 
@@ -102,7 +145,9 @@
 
 Es empfiehlt sich, zusätzlich einen Reverse-Proxy mit HTTPs-Zertifikat,
 bspw. [kostenlos von letsencrypt](https://letsencrypt.org/), zu verwenden.
 
 ## Credits
 
 * [mmarquezs](https://github.com/mmarquezs/) (My JDownloader-API für Python)
+
+
```

### Comparing `feedcrawler-19.1.0/feedcrawler/crawler.py` & `feedcrawler-19.2.0/feedcrawler/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from feedcrawler.providers.myjd_connection import set_device_from_config, get_if_one_device, myjd_input
 from feedcrawler.providers.sqlite_database import FeedDb, remove_redundant_db_tables
 from feedcrawler.web_interface.web_server import web_server
 
 version = "v." + version.get_version()
 
 
-def start_feedcrawler():
+def main():
     with multiprocessing.Manager() as manager:
         shared_state_dict = manager.dict()
         shared_state_lock = manager.Lock()
         shared_state.set_state(shared_state_dict, shared_state_lock)
 
         parser = argparse.ArgumentParser()
         parser.add_argument("--log-level", help="Legt fest, wie genau geloggt wird (INFO, DEBUG)")
@@ -241,8 +241,8 @@
         else:
             feed_crawler(shared_state_dict, shared_state_lock)
             process_web_server.terminate()
             sys.exit(0)
 
 
 if __name__ == "__main__":
-    start_feedcrawler()
+    main()
```

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/content_all.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/content_shows.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/shared.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_by.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_dw.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_ff.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_ff.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_fx.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_hw.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_nk.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_nx.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_all_ww.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_all_ww.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/metadata/imdb.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/metadata/imdb.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/content_all.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/content_shows.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/shared.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_by.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_dw.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_fx.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_hw.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_nk.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_sites/web_search/sites/content_all_nx.py` & `feedcrawler-19.2.0/feedcrawler/external_sites/web_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_tools/myjd_api.py` & `feedcrawler-19.2.0/feedcrawler/external_tools/myjd_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_tools/ombi_api.py` & `feedcrawler-19.2.0/feedcrawler/external_tools/ombi_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_tools/overseerr_api.py` & `feedcrawler-19.2.0/feedcrawler/external_tools/overseerr_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/external_tools/plex_api.py` & `feedcrawler-19.2.0/feedcrawler/external_tools/plex_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/jobs/feed_search.py` & `feedcrawler-19.2.0/feedcrawler/jobs/feed_search.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/jobs/package_watcher.py` & `feedcrawler-19.2.0/feedcrawler/jobs/package_watcher.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/common_functions.py` & `feedcrawler-19.2.0/feedcrawler/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/config.py` & `feedcrawler-19.2.0/feedcrawler/providers/config.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/gui.py` & `feedcrawler-19.2.0/feedcrawler/providers/gui.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/http_requests/cache_handler.py` & `feedcrawler-19.2.0/feedcrawler/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/http_requests/cloudflare_handlers.py` & `feedcrawler-19.2.0/feedcrawler/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/http_requests/request_handler.py` & `feedcrawler-19.2.0/feedcrawler/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/myjd_connection.py` & `feedcrawler-19.2.0/feedcrawler/providers/myjd_connection.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/notifications.py` & `feedcrawler-19.2.0/feedcrawler/providers/notifications.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/shared_state.py` & `feedcrawler-19.2.0/feedcrawler/providers/shared_state.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/sqlite_database.py` & `feedcrawler-19.2.0/feedcrawler/providers/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/url_functions.py` & `feedcrawler-19.2.0/feedcrawler/providers/url_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/providers/version.py` & `feedcrawler-19.2.0/feedcrawler/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "19.1.0"
+    return "19.2.0"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-Bix6I8bK.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-Bix6I8bK.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@meforma-Cn7fFUfm.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@meforma-Cn7fFUfm.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@meforma-D0j6vHqc.css` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@meforma-D0j6vHqc.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-WhmJkuoZ.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-WhmJkuoZ.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-DxhzX8GC.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-DxhzX8GC.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-C2nz7ynZ.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-C2nz7ynZ.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-Cm0UX6qg.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-Cm0UX6qg.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-DUEfxN0n.css` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-DUEfxN0n.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-DZKer8Tf.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-DZKer8Tf.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-BOrJxbIo.woff` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-BOrJxbIo.woff`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-BtvjY1KL.woff2` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-BtvjY1KL.woff2`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-Cb-KCKU4.css` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-Cb-KCKU4.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-BAhsgUwW.css` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-BAhsgUwW.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-C4FFZX5g.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-C4FFZX5g.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-LriLsbSV.css` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-LriLsbSV.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-Dqxmm31T.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-Dqxmm31T.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-jXauJNZF.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-jXauJNZF.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-C5iuhTWR.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-C5iuhTWR.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-C8dxsqXw.js` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-C8dxsqXw.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/vuejs_frontend/dist/index.html` & `feedcrawler-19.2.0/feedcrawler/web_interface/vuejs_frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler/web_interface/web_server.py` & `feedcrawler-19.2.0/feedcrawler/web_interface/web_server.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-19.1.0/feedcrawler.egg-info/PKG-INFO` & `feedcrawler-19.2.0/feedcrawler.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 19.1.0
+Version: 19.2.0
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -69,22 +69,50 @@
 
 ### Start
 
 ```feedcrawler``` in der Konsole (Python muss im System-PATH hinterlegt sein)
 
 ### [Docker Image](https://hub.docker.com/r/rix1337/docker-feedcrawler/)
 
+```
+docker run -d \
+  --name="FeedCrawler" \
+  -p port:9090 \
+  -v /path/to/config/:/config:rw \
+  -e USER=NUTZERNAME \ 
+  -e PASS=PASSWORT \
+  -e DEVICE=GERÄTENAME \
+  -e DELAY=30 \
+  -e LOGLEVEL=[INFO/DEBUG/WARNING/ERROR/CRITICAL/NOTSET] \
+  --log-opt max-size=50m \
+  rix1337/docker-feedcrawler
+  ```
+
 * Der Betrieb als Docker-Container empfiehlt sich als Standardinstallation - vor allem für NAS-Systeme, Homeserver und
   sonstige Geräte die dauerhaft und möglichst wartungsfrei (headless) betrieben werden sollen.
 * Bei jedem Release wird ein getaggtes Image erstellt. Damit kann man auf der Wunschversion verbleiben oder im Falle
   eines Bugs zu einer stabilen Version zurück kehren.
 * Um immer auf dem aktuellen Stand zu sein, einfach das mit `latest` getaggte Image nutzen.
 * Für UNRAID-Server kann das Image direkt über die Community Applications bezogen und der Container so eingerichtet
   werden.
 
+##### Optionale Parameter
+ - `-e USER` (ab dem ersten Start, sofern unverändert)
+ - `-e PASS` (ab dem ersten Start, sofern unverändert)
+ - `-e DEVICE` (immer, sofern nur ein Gerät im MyJD-Konto vorhanden ist, sonst ab dem ersten Start, sofern unverändert)
+ - `-e DELAY` (immer, sofern der erste Suchlauf nach Start nicht um diese ganze Zahl in Sekunden verzögert werden soll)
+
+##### Spezifische Version nutzen
+
+Das Image `rix1377/docker-feedcrawler` wird standardmäßig auf das `:latest`-Tag aufgelöst. Dieses wird mit jedem Release auf die neue Version aktualisiert. Mit jedem Release wird ebenfalls eine getaggte Version des Images erzeugt. Auf letztere kann man wechseln, um beispielsweise bei Fehlern in der neuen Version auf einen funktionierenden Stand zurück zu kehren.
+
+Beispiel:
+
+`docker pull rix1337/docker-feedcrawler:13.0.3`
+
 ### Windows Build
 
 * Jedem [Release](https://github.com/rix1337/FeedCrawler/releases) wird eine selbstständig unter Windows lauffähige
   Version des FeedCrawlers beigefügt.
 * Hierfür müssen weder Python, noch die Zusatzpakete installiert werden.
 * Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
```

### Comparing `feedcrawler-19.1.0/feedcrawler.egg-info/SOURCES.txt` & `feedcrawler-19.2.0/feedcrawler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE.md
 MANIFEST.in
 README.md
 setup.py
 feedcrawler/__init__.py
-feedcrawler/crawler.py
+feedcrawler/run.py
 feedcrawler.egg-info/PKG-INFO
 feedcrawler.egg-info/SOURCES.txt
 feedcrawler.egg-info/dependency_links.txt
 feedcrawler.egg-info/entry_points.txt
 feedcrawler.egg-info/not-zip-safe
 feedcrawler.egg-info/requires.txt
 feedcrawler.egg-info/top_level.txt
```

### Comparing `feedcrawler-19.1.0/setup.py` & `feedcrawler-19.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,11 +34,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'feedcrawler = feedcrawler.crawler:start_feedcrawler',
+            'feedcrawler = feedcrawler.run:main',
         ],
     },
 )
```


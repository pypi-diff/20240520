# Comparing `tmp/bricks-py-0.0.8.tar.gz` & `tmp/bricks-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bricks-py-0.0.8.tar", last modified: Tue Dec 12 11:15:08 2023, max compression
+gzip compressed data, was "bricks-py-0.0.9.tar", last modified: Wed Dec 13 14:43:58 2023, max compression
```

## Comparing `bricks-py-0.0.8.tar` & `bricks-py-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.174039 bricks-py-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-12 11:15:08.174039 bricks-py-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-12 11:14:58.000000 bricks-py-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.166040 bricks-py-0.0.8/bricks/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.166040 bricks-py-0.0.8/bricks/client/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.166040 bricks-py-0.0.8/bricks/core/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11462 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/core/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/core/genesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/core/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.166040 bricks-py-0.0.8/bricks/db/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/db/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)    17131 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/db/redis_.py
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/db/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.166040 bricks-py-0.0.8/bricks/downloader/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/downloader/cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/downloader/curl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/downloader/genesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/downloader/go_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/downloader/requests_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.170040 bricks-py-0.0.8/bricks/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12749 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.170040 bricks-py-0.0.8/bricks/lib/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/queues/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/queues/genesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/queues/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    24307 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/queues/redis_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/queues/smart.py
--rw-r--r--   0 runner    (1001) docker     (127)     9745 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/lib/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.170040 bricks-py-0.0.8/bricks/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/plugins/make_seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/plugins/on_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/plugins/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/plugins/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.170040 bricks-py-0.0.8/bricks/spider/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/spider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27902 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/spider/air.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/spider/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/spider/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.174039 bricks-py-0.0.8/bricks/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/csv_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.174039 bricks-py-0.0.8/bricks/utils/fake/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26522 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/fake/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/pandora.py
--rw-r--r--   0 runner    (1001) docker     (127)    17265 2023-12-12 11:14:58.000000 bricks-py-0.0.8/bricks/utils/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.174039 bricks-py-0.0.8/bricks_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-12 11:15:08.000000 bricks-py-0.0.8/bricks_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2023-12-12 11:15:08.000000 bricks-py-0.0.8/bricks_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 11:15:08.000000 bricks-py-0.0.8/bricks_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-12 11:15:08.000000 bricks-py-0.0.8/bricks_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-12 11:15:08.000000 bricks-py-0.0.8/bricks_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:15:08.174039 bricks-py-0.0.8/demos/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-12 11:14:58.000000 bricks-py-0.0.8/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2023-12-12 11:14:58.000000 bricks-py-0.0.8/demos/air_spider_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-12 11:14:58.000000 bricks-py-0.0.8/demos/dispatcher_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2023-12-12 11:14:58.000000 bricks-py-0.0.8/demos/form_spider_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2023-12-12 11:14:58.000000 bricks-py-0.0.8/demos/template_spider_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 11:15:08.174039 bricks-py-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-12 11:14:58.000000 bricks-py-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.737047 bricks-py-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-13 14:43:58.737047 bricks-py-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-12-13 14:43:48.000000 bricks-py-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.729047 bricks-py-0.0.9/bricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.729047 bricks-py-0.0.9/bricks/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.729047 bricks-py-0.0.9/bricks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/core/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/core/genesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/core/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.729047 bricks-py-0.0.9/bricks/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/db/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17131 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/db/redis_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/db/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.733047 bricks-py-0.0.9/bricks/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/downloader/cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11254 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/downloader/curl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/downloader/go_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/downloader/playwright_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/downloader/requests_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.733047 bricks-py-0.0.9/bricks/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13155 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.733047 bricks-py-0.0.9/bricks/lib/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/queues/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/queues/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24299 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/queues/redis_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/queues/smart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/lib/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.733047 bricks-py-0.0.9/bricks/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/plugins/make_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/plugins/on_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/plugins/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/plugins/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.737047 bricks-py-0.0.9/bricks/spider/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/spider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28279 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/spider/air.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/spider/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/spider/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.737047 bricks-py-0.0.9/bricks/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/csv_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.737047 bricks-py-0.0.9/bricks/utils/fake/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26522 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/fake/user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/pandora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17265 2023-12-13 14:43:48.000000 bricks-py-0.0.9/bricks/utils/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.737047 bricks-py-0.0.9/bricks_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-13 14:43:58.000000 bricks-py-0.0.9/bricks_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2023-12-13 14:43:58.000000 bricks-py-0.0.9/bricks_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 14:43:58.000000 bricks-py-0.0.9/bricks_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-13 14:43:58.000000 bricks-py-0.0.9/bricks_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-13 14:43:58.000000 bricks-py-0.0.9/bricks_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 14:43:58.737047 bricks-py-0.0.9/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-13 14:43:48.000000 bricks-py-0.0.9/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2023-12-13 14:43:48.000000 bricks-py-0.0.9/demos/air_spider_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-12-13 14:43:48.000000 bricks-py-0.0.9/demos/dispatcher_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2023-12-13 14:43:48.000000 bricks-py-0.0.9/demos/form_spider_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-13 14:43:48.000000 bricks-py-0.0.9/demos/form_spider_demo2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-12-13 14:43:48.000000 bricks-py-0.0.9/demos/template_spider_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 14:43:58.737047 bricks-py-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-13 14:43:48.000000 bricks-py-0.0.9/setup.py
```

### Comparing `bricks-py-0.0.8/bricks/core/context.py` & `bricks-py-0.0.9/bricks/core/context.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/core/dispatch.py` & `bricks-py-0.0.9/bricks/core/dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,20 +349,20 @@
 
     @property
     def running(self):
         return self.max_workers - self._remain_workers._value + self.tasks.qsize()  # noqa
 
     def run(self):
         async def main():
+            self.loop = asyncio.get_event_loop()
             self._shutdown = asyncio.Event()
             self._running.set()
             await self._shutdown.wait()
             self._set_env()
 
-        asyncio.set_event_loop(self.loop)
         asyncio.run(main())
 
     def stop(self):
         self.loop.call_soon_threadsafe(self._shutdown.set)
         self.stop_worker(*self.workers.keys())
         # note: It must be called this way, otherwise the thread is unsafe and the write over there cannot be closed
```

### Comparing `bricks-py-0.0.8/bricks/core/events.py` & `bricks-py-0.0.9/bricks/core/events.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/core/genesis.py` & `bricks-py-0.0.9/bricks/core/genesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023-11-15 12:49
 # @Author  : Kem
 # @Desc    :
 import functools
 import time
-from typing import Union, Literal, Callable
+from typing import Union, Literal, Callable, List
 
 from loguru import logger
 
 from bricks.core import signals, dispatch
-from bricks.core.events import EventManager, Task
 from bricks.core.context import Flow, Context
+from bricks.core.events import EventManager, Task, Register
 from bricks.state import const
 from bricks.utils import pandora
 from bricks.utils.scheduler import BaseTrigger, Scheduler
 
 
 class MetaClass(type):
 
@@ -92,14 +92,15 @@
         :param scheduler:
         :param task_name:
         :param args:
         :param kwargs:
         :param callback:
         :return:
         """
+
         def job():
             self.run(task_name=task_name, args=args, kwargs=kwargs)
             callback and pandora.invoke(callback, namespace={"spider": self}, annotations={type(self): self})
 
         form: Union[Literal['cron', 'date', 'interval'], BaseTrigger] = scheduler.pop("form")
         exprs: str = scheduler.pop("exprs")
         scheduler_ = Scheduler()
@@ -174,15 +175,15 @@
     Context = Flow
 
     def __init__(self, **kwargs) -> None:
         for k, v in kwargs.items():
             self.set(k, v, nx=True)
 
         self.dispatcher = dispatch.Dispatcher(max_workers=self.get("concurrency", 1))
-        self.plugins = []
+        self.plugins: List[Register] = []
 
     def on_consume(self, context: Flow):
         context.next.root == self.on_consume and context.flow()
 
         while True:
             context: Flow = context.produce()
             if context is None: return
```

### Comparing `bricks-py-0.0.8/bricks/core/signals.py` & `bricks-py-0.0.9/bricks/core/signals.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/db/mongo.py` & `bricks-py-0.0.9/bricks/db/mongo.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/db/redis_.py` & `bricks-py-0.0.9/bricks/db/redis_.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/db/sqlite.py` & `bricks-py-0.0.9/bricks/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/downloader/cffi.py` & `bricks-py-0.0.9/bricks/downloader/cffi.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 import copy
 import urllib.parse
 from typing import Union
 
 from curl_cffi import requests
 
-from bricks.downloader import genesis
+from bricks.downloader import AbstractDownloader
 from bricks.lib.cookies import Cookies
 from bricks.lib.request import Request
 from bricks.lib.response import Response
 
 
-class Downloader(genesis.Downloader):
+class Downloader(AbstractDownloader):
     """
     对 cffi 进行的一层包装, 类似 requests, tls 与浏览器保持一致
     兼容 Windows / Mac / Linux
 
 
     """
```

### Comparing `bricks-py-0.0.8/bricks/downloader/curl.py` & `bricks-py-0.0.9/bricks/downloader/curl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import copy
 import io
 import os
 import random
 import urllib.parse
 from typing import Union
 
-from bricks.downloader import genesis
+from bricks.downloader import AbstractDownloader
 from bricks.lib.cookies import Cookies
 from bricks.lib.request import Request
 from bricks.lib.response import Response
 from bricks.utils import pandora
 
 pandora.require("pycurl")
 
-import pycurl
-import certifi
-import six
+import pycurl  # noqa: E402
+import certifi  # noqa: E402
+import six  # noqa: E402
 
 
-class Downloader(genesis.Downloader):
+class Downloader(AbstractDownloader):
     """
     对 pycurl 进行的一层包装, pycurl 太难装了, 不推荐用
 
 
     """
 
     def __init__(
@@ -319,9 +319,9 @@
             pass
 
         return options
 
 
 if __name__ == '__main__':
     downloader = Downloader()
-    res = downloader.fetch({"url": "https://www.baidu.com"})
-    print(res.cookies)
+    resp = downloader.fetch({"url": "https://www.baidu.com"})
+    print(resp.cookies)
```

### Comparing `bricks-py-0.0.8/bricks/downloader/genesis.py` & `bricks-py-0.0.9/bricks/downloader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from loguru import logger
 
 from bricks.core import genesis
 from bricks.lib.request import Request
 from bricks.lib.response import Response
 
 
-class Downloader(metaclass=genesis.MetaClass):
+class AbstractDownloader(metaclass=genesis.MetaClass):
 
     def fetch(self, request: Union[Request, dict]) -> Response:
         """
         发送请求以获得一个响应
 
         :param request: 请求或包含请求参数的字典
         :return:
```

### Comparing `bricks-py-0.0.8/bricks/downloader/go_requests.py` & `bricks-py-0.0.9/bricks/downloader/go_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from __future__ import absolute_import
 
 import copy
 import urllib.parse
 import warnings
 from typing import Union
 
-from bricks.downloader import genesis
+from bricks.downloader import AbstractDownloader
 from bricks.lib.cookies import Cookies
 from bricks.lib.request import Request
 from bricks.lib.response import Response
 from bricks.utils import pandora
 
 warnings.filterwarnings("ignore")
 pandora.require("requests-go")
 
-import requests_go
+import requests_go  # noqa: E402
 
 
-class Downloader(genesis.Downloader):
+class Downloader(AbstractDownloader):
     """
     对 requests-go 进行的一层包装, 支持手动设置 tls
     兼容 Windows / Mac / Linux
 
 
     """
 
@@ -96,9 +96,9 @@
                 res.request = request
 
                 return res
 
 
 if __name__ == '__main__':
     downloader = Downloader()
-    res = downloader.fetch({"url": "https://www.baidu.com"})
-    print(res)
+    resp = downloader.fetch({"url": "https://www.baidu.com"})
+    print(resp)
```

### Comparing `bricks-py-0.0.8/bricks/downloader/requests_.py` & `bricks-py-0.0.9/bricks/downloader/requests_.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 import copy
 import http.client
 import urllib.parse
 import warnings
 from typing import Union
 
-from bricks.downloader import genesis
+from bricks.downloader import AbstractDownloader
 from bricks.lib.cookies import Cookies
 from bricks.lib.request import Request
 from bricks.lib.response import Response
 from bricks.utils import pandora
 
 warnings.filterwarnings("ignore")
 # 设置 requests 最大的响应头的长度 为 1000
 http.client._MAXHEADERS = 1000
 
 pandora.require("requests")
 
-import requests
+import requests  # noqa: E402
 
 
-class Downloader(genesis.Downloader):
+class Downloader(AbstractDownloader):
     """
     对 requests 进行的一层包装
     兼容 Windows / Mac / Linux
 
 
     """
```

### Comparing `bricks-py-0.0.8/bricks/lib/cookies.py` & `bricks-py-0.0.9/bricks/lib/cookies.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,15 +175,18 @@
 
         return f"<Cookies[{cookies_repr}]>"
 
     @classmethod
     def by_jar(cls, jar):
         cookies = cls()
         for cookie in jar:
-            cookies.set(name=cookie.name, value=cookie.value, domain=cookie.domain, path=cookie.path)
+            if isinstance(cookie, dict):
+                cookies.set(name=cookie["name"], value=cookie["value"], domain=cookie.get('domain'), path=cookie.get('path'))
+            else:
+                cookies.set(name=cookie.name, value=cookie.value, domain=cookie.domain, path=cookie.path)
         return cookies
 
     def load(self, set_cookie_string: str):
         simple_cookie = SimpleCookie()
         simple_cookie.load(set_cookie_string)
         # 遍历解析后的 SimpleCookie 来创建 Cookie 对象并添加到 CookieJar
         for key, morsel in simple_cookie.items():
```

### Comparing `bricks-py-0.0.8/bricks/lib/counter.py` & `bricks-py-0.0.9/bricks/lib/counter.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/lib/extractors.py` & `bricks-py-0.0.9/bricks/lib/extractors.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/lib/headers.py` & `bricks-py-0.0.9/bricks/lib/headers.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/lib/items.py` & `bricks-py-0.0.9/bricks/lib/items.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/lib/nodes.py` & `bricks-py-0.0.9/bricks/lib/nodes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,111 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023-11-20 21:26
 # @Author  : Kem
 # @Desc    :
 import copy
 import dataclasses
 import re
-from typing import Any, Union, Callable, Optional
+from typing import Any, Union, Callable, Optional, Literal
 
 from bricks.utils import pandora
 
 FORMAT_REGEX = re.compile(r'{(\w+)(?::(\w+))?}')
 
 
 @dataclasses.dataclass
 class RenderNode:
+    errors: Literal["fix", "raise", "ignore"] = "fix"
+    adapters: dict = dataclasses.field(default_factory=lambda: {
+        "int": int,
+        int: int,
+        "str": str,
+        str: str,
+        "float": float,
+        float: float,
+        "json": pandora.json_or_eval,
+        list: pandora.json_or_eval,
+        dict: pandora.json_or_eval,
+    })
 
-    @classmethod
-    def format(cls, value, base: dict, errors: str = "raise"):
+    def format(self, value, base: dict):
         if isinstance(value, str):
             while True:
                 try:
                     return value.format(**base)
                 except ValueError:
 
                     placeholders = FORMAT_REGEX.findall(value)
                     # 有多个, 那最终肯定还是字符串
                     convert_value = len(placeholders) == 1
                     for placeholder, type_str in placeholders:
 
                         if placeholder not in base:
-                            if errors == 'raise':
+                            if self.errors == 'raise':
                                 raise ValueError(f"Missing key in base: {placeholder}")
-                            elif errors == 'ignore':
+                            elif self.errors == 'ignore':
                                 return value
                             else:
                                 base.setdefault(placeholder, "")
 
                         placeholder_value = base[placeholder]
                         if type_str:
-                            placeholder_value = cls.convert(placeholder_value, type_str)
+                            placeholder_value = self.run_adapter(placeholder_value, type_str, base=base)
                             value = value.replace(f"{{{placeholder}:{type_str}}}", str(placeholder_value))
                         else:
                             value = value.replace(f"{{{placeholder}}}", str(placeholder_value))
 
                         if convert_value:
-                            value = cls.convert(value, type(placeholder_value))
+                            value = self.run_adapter(value, type(placeholder_value), base=base)
 
                     return value
 
                 except KeyError as e:
-                    if errors == "raise":
+                    if self.errors == "raise":
                         raise ValueError(f"Missing key in base: {e}")
 
-                    elif errors == 'ignore':
+                    elif self.errors == 'ignore':
                         return value
 
                     else:
                         base.setdefault(e.args[0], "")
 
         elif isinstance(value, list):
-            return [cls.format(item, base, errors=errors) for item in value]
+            return [self.format(item, base) for item in value]
         elif isinstance(value, dict):
-            return {k: cls.format(v, base, errors=errors) for k, v in value.items()}
+            return {k: self.format(v, base) for k, v in value.items()}
         elif dataclasses.is_dataclass(value):
             return value.render(base)
         return value
 
-    @staticmethod
-    def convert(value, type_str):
-        maps = {
-            "int": {
-                "action": int,
-                "default": 0
-            },
-            int: {
-                "action": int,
-                "default": 0
-            },
-            "str": {
-                "action": str,
-                "default": ""
-            },
-            str: {
-                "action": str,
-                "default": ""
-            },
-            "float": {
-                "action": str,
-                "default": 0.0
-            },
-            float: {
-                "action": str,
-                "default": 0.0
-            },
-            "json": {
-                "action": pandora.json_or_eval,
-                "default": None
-            },
-            list: {
-                "action": pandora.json_or_eval,
-                "default": None
-            },
-            dict: {
-                "action": pandora.json_or_eval,
-                "default": None
-            },
-        }
-        if type_str in maps:
-            try:
-                return maps[type_str]['action'](value)
-            except ValueError:
-                return maps[type_str]['default']
-        else:
-            return value
-
-    def render(self, base: dict):
+    def render(self, base: dict = None):
         # 创建一个新的实例，避免修改原始实例
+        base = base or {}
         node = copy.deepcopy(self)
         for field in dataclasses.fields(self):
             value = getattr(node, field.name)
-            new_value = self.format(value, base, errors=getattr(self, "strict", "fix"))
+            new_value = self.format(value, base)
             setattr(node, field.name, new_value)
         return node
 
+    def register_adapter(self, form: Any, action: Callable):
+        self.adapters[form] = action
+
+    def run_adapter(self, value, form: Any, base: dict = None):
+        print(value)
+        if form in self.adapters:
+            adapter = self.adapters[form]
+            try:
+                assert callable(adapter), f"Invalid adapter action: {adapter}"
+                return pandora.invoke(adapter, args=[value], namespace=base)
+            except (ValueError, AssertionError):
+                return value
+        else:
+            return value
+
 
 @dataclasses.dataclass
 class LinkNode:
     root: Callable = None
     prev: Optional['LinkNode'] = None
     callback: Optional[Callable] = None
```

### Comparing `bricks-py-0.0.8/bricks/lib/proxies.py` & `bricks-py-0.0.9/bricks/lib/proxies.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import json
 import math
 import queue
 import re
 import threading
 import time
 import urllib.parse
-from typing import Optional, Callable
+from typing import Optional, Callable, Type
 
 from loguru import logger
 
 from bricks.db.redis_ import Redis
 from bricks.downloader import cffi
 from bricks.utils import pandora
 
@@ -28,14 +28,17 @@
     r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'  # ...or ip
     r'(?::\d+)?'  # optional port
     r'(?:/?|[/?]\S+)$', re.IGNORECASE
 )
 
 
 class MetaClass(type):
+    _instances = {}
+    _lock = threading.Lock()
+
     def __new__(cls, name, bases, dct):  # noqa
         def wrapper(raw_method):
             def inner(self, *args, **kwargs):
                 self: BaseProxy
                 proxy = raw_method(self, *args, **kwargs)
                 proxy.proxy = self.fmt(proxy=proxy.proxy)
                 proxy.auth = self.auth
@@ -47,14 +50,21 @@
             return inner
 
         # 在这里可以修改类的定义
         dct['get'] = wrapper(dct['get'])
         # 创建并返回新的类
         return super(MetaClass, cls).__new__(cls, name, bases, dct)
 
+    def __call__(cls, *args, **kwargs):
+        with cls._lock:
+            if cls not in cls._instances:
+                instance = super().__call__(*args, **kwargs)
+                cls._instances[cls] = instance
+        return cls._instances[cls]
+
 
 class Proxy:
     def __init__(
             self,
             proxy: Optional[str] = None,
             auth: Optional[Callable] = None,
             recover: Optional[Callable] = ...,
@@ -144,14 +154,18 @@
 
         # scheme://username:password@proxy:port
         elif parsed.username and parsed.password:
             proxy = f'{self.scheme}://{parsed.username}:{parsed.password}@{parsed.hostname}"{parsed.port}'
 
         return proxy
 
+    @classmethod
+    def build(cls, **options):
+        return pandora.invoke(cls, kwargs=options)
+
 
 class ApiProxy(BaseProxy):
     def __init__(
             self,
             key,
             scheme: str = "http",
             username: Optional[str] = None,
@@ -318,20 +332,22 @@
 
         :param configs: 获取代理的配置 -> {"ref": "指向代理类", ... 这些其他的都是实例化类的参数}
         :param timeout: 获取代理的超时时间, timeout 为 None 代表一直等待, 超时会直接使用空代理
         :return:
         """
         with self._context:
             for config in configs:
-                config["ref"] = pandora.load_objects(config["ref"])
+                ref = config["ref"] = pandora.load_objects(config["ref"])
+                ref: Type[BaseProxy]
+
                 rkey = self.get_rkey(config)
 
                 if not hasattr(self._local, rkey):
                     if rkey not in self.container:
-                        self.container[rkey] = pandora.invoke(config["ref"], kwargs=config)
+                        self.container[rkey] = ref.build(**config)
 
                     # 获取代理模型
                     ins: BaseProxy = self.container[rkey]
                     try:
                         proxy = ins.get(timeout=timeout)
                     except TimeoutError:
                         proxy = Proxy()
@@ -420,9 +436,8 @@
             self._context = threading.Lock()
 
 
 manager = Manager()
 
 if __name__ == '__main__':
     p = CustomProxy("127.0.0.1:7890")
-    print(p.get())
     print(pandora.prepare(CustomProxy))
```

### Comparing `bricks-py-0.0.8/bricks/lib/queues/cache.py` & `bricks-py-0.0.9/bricks/lib/queues/cache.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/lib/queues/genesis.py` & `bricks-py-0.0.9/bricks/lib/queues/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # -*- coding: utf-8 -*-
+# @Time    : 2023-12-11 13:14
+# @Author  : Kem
+# @Desc    :
+# -*- coding: utf-8 -*-
 # @Time    : 2023-12-11 13:15
 # @Author  : Kem
 # @Desc    :
 import copy
 import functools
 import json
 import time
@@ -256,7 +260,13 @@
         def inner(name, *values, **kwargs):
             return func(name, *[i.fingerprint if isinstance(i, Item) else i for i in values], **kwargs)
 
         return inner
 
     def command(self, name: str, order: dict):
         raise NotImplementedError
+
+
+# 必须在最后导入, 不然会出现循环导入
+from bricks.lib.queues.smart import SmartQueue  # noqa: E402
+from bricks.lib.queues.redis_ import RedisQueue  # noqa: E402
+from bricks.lib.queues.local import LocalQueue  # noqa: E402
```

### Comparing `bricks-py-0.0.8/bricks/lib/queues/local.py` & `bricks-py-0.0.9/bricks/lib/queues/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import threading
 import time
 from collections import defaultdict
 
 from loguru import logger
 
-from bricks.lib.queues.genesis import TaskQueue, Item
+from bricks.lib.queues import TaskQueue, Item
 from bricks.lib.queues.smart import SmartQueue
 from bricks.utils import pandora
 
 
 class LocalQueue(TaskQueue):
 
     def __init__(self) -> None:
```

### Comparing `bricks-py-0.0.8/bricks/lib/queues/redis_.py` & `bricks-py-0.0.9/bricks/lib/queues/redis_.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 import time
 
 from loguru import logger
 
 from bricks import state
 from bricks.db.redis_ import Redis
-from bricks.lib.queues.genesis import TaskQueue
+from bricks.lib.queues import TaskQueue
 from bricks.utils import pandora
 
 
 class RedisQueue(TaskQueue):
     subscribe = True
 
     def __init__(self, host='127.0.0.1', password=None, port=6379, database=0, genre="set", **kwargs):
```

### Comparing `bricks-py-0.0.8/bricks/lib/queues/smart.py` & `bricks-py-0.0.9/bricks/lib/queues/smart.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/lib/request.py` & `bricks-py-0.0.9/bricks/lib/request.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/lib/response.py` & `bricks-py-0.0.9/bricks/lib/response.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/lib/variable.py` & `bricks-py-0.0.9/bricks/lib/variable.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/plugins/make_seeds.py` & `bricks-py-0.0.9/bricks/plugins/make_seeds.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/plugins/on_request.py` & `bricks-py-0.0.9/bricks/plugins/on_request.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/plugins/scripts.py` & `bricks-py-0.0.9/bricks/plugins/scripts.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/plugins/storage.py` & `bricks-py-0.0.9/bricks/plugins/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,15 +99,16 @@
     """
 
     row_keys = row_keys or []
 
     # 仅支持 set, list, string
     assert key_type in ["set", "list", "string"], ValueError(f'不支持的存储类型-{key_type}')
     # 当存储类型不为 string 时, path 不能为空且类型必须与预期一致
-    assert (path and conn.type(path) in [key_type, 'none']) or key_type == 'string', f'存储类型错误, 已存在-{path}:{conn.type(path)}, 存储类型-{key_type}'
+    assert (path and conn.type(path) in [key_type,
+                                         'none']) or key_type == 'string', f'存储类型错误, 已存在-{path}:{conn.type(path)}, 存储类型-{key_type}'
     # 当存储类型为 string 时, row_keys 不能为空
     assert row_keys or key_type != 'string', ValueError(f'存储类型为 string 时必须存在 row_keys')
 
     def generate_key(_row):
         key = splice.join([str(_row.get(key, "")) for key in row_keys])
         return key
 
@@ -125,19 +126,7 @@
             for key in iterable(path):
                 conn.expire(key, ttl)
 
     if row_keys:
         for row in items:
             row['$key'] = generate_key(row)
     write(items)
-
-
-if __name__ == '__main__':
-    from no_views.conn import redis
-    to_redis(
-        path="5",
-        conn=redis,
-        items=[{"a": 1, "b": 2}, {"a": 2, "b": 3}],
-        key_type="string",
-        row_keys=["a", "b"],
-        # ttl=60
-    )
```

### Comparing `bricks-py-0.0.8/bricks/spider/air.py` & `bricks-py-0.0.9/bricks/spider/air.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023-11-15 14:09
 # @Author  : Kem
 # @Desc    :
+import collections
 import datetime
 import functools
 import inspect
 import math
 import queue
 import re
 import time
@@ -13,15 +14,15 @@
 
 from loguru import logger
 
 from bricks import state
 from bricks.core import dispatch, signals, events
 from bricks.core.context import Flow
 from bricks.core.genesis import Pangu
-from bricks.downloader import genesis, cffi
+from bricks.downloader import cffi, AbstractDownloader
 from bricks.lib.counter import FastWriteCounter
 from bricks.lib.items import Items
 from bricks.lib.proxies import manager
 from bricks.lib.queues import TaskQueue, LocalQueue, Item
 from bricks.lib.request import Request
 from bricks.lib.response import Response
 from bricks.plugins import on_request
@@ -67,33 +68,43 @@
         self.flow({"next": self.target.on_retry})
 
     def failure(self, shutdown=False):
         ret = self.task_queue.remove(self.queue_name, self.seeds, backup='failure') if self.seeds else None
         shutdown and self.flow({"next": None})
         return ret
 
-    def submit(self, obj: Union[Request, Item, dict], call_later=False) -> "Context":
+    def submit(self, obj: Union[Request, Item, dict], call_later=False, attrs: dict = None) -> List["Context"]:
         """
         专门为新请求分支封装的方法, 会自动将请求放入队列
         传入的对象可以是新的种子 / 新的 request
 
+        :param attrs:
         :param obj:
         :param call_later: 是否延迟调用, 如果延迟调用, 就是将种子放到当前队列, 等待其他机器获取消费, 否则
         :return:
         """
-        assert obj.__class__ in [Request, Item, dict], f"不支持的类型: {obj.__class__}"
-        if obj.__class__ in [Item, dict]:
-            if call_later:
-                self.task_queue.put(self.queue_name, obj)
-                return self
+        ret = []
+        attrs = attrs or {}
+        group = collections.defaultdict(list)
+        for o in obj:
+            assert o.__class__ in [Request, Item, dict], TypeError(f"不支持的类型: {o.__class__}")
+            group[o.__class__].append(o)
+
+        for cls, objs in group.items():
+            if cls in [Item, dict]:
+                if call_later:
+                    self.task_queue.put(self.queue_name, *objs)
+                else:
+                    self.task_queue.put(self.queue_name, *objs, qtypes="temp")
+                    ret.extend([self.branch({"seeds": o, "next": self.target.on_seeds, **attrs}) for o in objs])
             else:
-                self.task_queue.put(self.queue_name, obj, qtypes="temp")
-                return self.branch({"seeds": obj, "next": self.target.on_seeds})
+                ret.extend([self.branch({"request": o, "next": self.target.on_request, **attrs}) for o in objs ])
+
         else:
-            return self.branch({"request": obj, "next": self.target.on_request})
+            return ret
 
     def clear_proxy(self):
         manager.clear_proxy(self.request.proxy or self.target.proxy)
         self.request.proxies = None
 
     error = failure
 
@@ -136,15 +147,15 @@
 class Spider(Pangu):
     Context = Context
     InitContext = InitContext
 
     def __init__(
             self,
             concurrency: Optional[int] = 1,
-            downloader: Optional[Union[str, genesis.Downloader]] = None,
+            downloader: Optional[Union[str, AbstractDownloader]] = None,
             task_queue: Optional[TaskQueue] = None,
             queue_name: Optional[str] = "",
             proxy: Optional[dict] = None,
             forever: Optional[bool] = False,
             **kwargs
     ) -> None:
```

### Comparing `bricks-py-0.0.8/bricks/spider/form.py` & `bricks-py-0.0.9/bricks/spider/form.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023-11-18 10:47
 # @Author  : Kem
 # @Desc    :
+import collections
 import copy
 import inspect
 from dataclasses import dataclass
 from typing import Optional, Union, List, Dict, Callable
 
 from loguru import logger
 
@@ -26,63 +27,81 @@
         super().__init__(target, form, **kwargs)
         self.signpost: SignPost = kwargs.get("signpost") or SignPost()
 
     def retry(self):
         super().retry()
         self.signpost.action = "retry"
 
-    def submit(self, obj: Union[Request, Item, dict], call_later=False, signpost: SignPost = None) -> "Context":
-        assert obj.__class__ in [Request, Item, dict], f"不支持的类型: {obj.__class__}"
-        if obj.__class__ in [Item, dict]:
-            signpost = SignPost(cursor=Post(self.signpost.download.value)) if signpost is None else signpost
-
-            if call_later:
-                self.task_queue.put(self.queue_name, obj)
-                return self
+    def submit(self, *obj: Union[Item, dict, Request], call_later=False, attrs: dict = None) -> List["Context"]:
+        ret = []
+        attrs = attrs or {}
+        group = collections.defaultdict(list)
+        for o in obj:
+            assert o.__class__ in [Request, Item, dict], TypeError(f"不支持的类型: {o.__class__}")
+            group[o.__class__].append(o)
+
+        for cls, objs in group.items():
+
+            if cls in [Item, dict]:
+                # 将游标指向上一个下载节点
+                signpost = SignPost(cursor=Post(self.signpost.download.value))
+
+                if call_later:
+                    self.task_queue.put(self.queue_name, *objs)
+
+                else:
+                    self.task_queue.put(self.queue_name, *objs, qtypes="temp")
+                    # 交给 on flow 进行流程分配: on_flow -> make_request -> on_request
+                    ret.extend([
+                        self.branch({"seeds": o, "signpost": signpost, "next": self.target.on_flow, **attrs})
+                        for o in objs
+                    ])
+
             else:
-                self.task_queue.put(self.queue_name, obj, qtypes="temp")
-                return self.branch({
-                    "seeds": obj,
-                    "signpost": signpost
-                })
+                # 将游标指向下载节点后一个
+                signpost = SignPost(cursor=Post(self.signpost.download.value + 1))
+
+                # 自己进行流程分配: on_flow (省去) -> make_request (省去) -> on_request, 所以直接是 on_request
+                ret.extend([
+                    self.branch({"request": o, "signpost": signpost, "next": self.target.on_request, **attrs})
+                    for o in objs
+                ])
+
         else:
-            signpost = signpost or SignPost()
-            return self.branch({"request": obj, "next": self.target.on_request, "signpost": signpost})
+            return ret
 
 
 class Task(_events.Task, RenderNode):
     ...
 
 
 @dataclass
 class Layout(RenderNode):
     rename: dict = None
     show: dict = None
     factory: dict = None
     default: dict = None
-    strict: str = "fix"
 
 
 @dataclass
 class Download(RenderNode):
-    url: str
+    url: str = ...
     params: Optional[dict] = None
     method: str = 'GET'
     body: Union[str, dict] = None
     headers: Union[Header, dict] = None
     cookies: Dict[str, str] = None
     options: dict = None
     timeout: int = ...
     allow_redirects: bool = True
     proxies: Optional[str] = None
     proxy: Optional[dict] = None
     status_codes: Optional[dict] = ...
     retry: int = 0
     max_retry: int = 5
-    strict: str = "fix"
 
     def to_request(self) -> Request:
         return Request(
             url=self.url,
             params=self.params,
             method=self.method,
             body=self.body,
@@ -94,43 +113,40 @@
             proxies=self.proxies,
             proxy=self.proxy,
             status_codes=self.status_codes,
             retry=self.retry,
             max_retry=self.max_retry
         )
 
-    def to_response(self, spider: "Spider" = None) -> Response:
-        return convert.req2resp(self.to_request(), spider)
+    def to_response(self, options: dict = None) -> Response:
+        return convert.req2resp(self.to_request(), options)
 
 
 @dataclass
 class Parse(RenderNode):
-    func: Union[str, Callable]
+    func: Union[str, Callable] = ...
     args: Optional[list] = None
     kwargs: Optional[dict] = None
-    strict: str = "fix"
     layout: Optional[Layout] = None
 
 
 @dataclass
 class Pipeline(RenderNode):
-    func: Union[str, Callable]
+    func: Union[str, Callable] = ...
     args: Optional[list] = None
     kwargs: Optional[dict] = None
-    strict: str = "fix"
     success: bool = False
     layout: Optional[Layout] = None
 
 
 @dataclass
 class Init(RenderNode):
-    func: Union[str, Callable]
+    func: Union[str, Callable] = ...
     args: Optional[list] = None
     kwargs: Optional[dict] = None
-    strict: str = "fix"
     layout: Optional[Layout] = None
 
 
 @dataclass
 class Config:
     spider: List[Union[Download, Parse, Task, Pipeline]] = None
     init: Optional[List[Init]] = None
@@ -140,14 +156,16 @@
 class Spider(air.Spider):
     Context = Context
 
     @property
     def flows(self):
         return {
             self.on_consume: self.on_flow,
+            # run spider 拿到种子后 -> self.on_seeds, 此时 signpost 都是 0
+            # 那么直接交给 on_flow 进行分配
             self.on_seeds: self.on_flow,
             self.make_request: self.on_request,
             self.on_request: self.on_flow,
             self.on_retry: self.on_flow,
             self.on_response: self.on_flow,
             self.on_pipeline: self.on_flow,
         }
@@ -393,10 +411,11 @@
         super().install()
 
         for form, events in (self.config.events or {}).items():
             self.use(form, *events)
 
 
 if __name__ == '__main__':
-    down = Download(url="http://www.baidu.com")
-    resp = down.to_response()
-    print(resp.text)
+    down = Download(url="http://www.baidu.com", params={"skus": '{sku:allsku}'})
+    down.register_adapter("allsku", lambda has_sku, miss_sku: has_sku + miss_sku)
+    rendered = down.render({"has_sku": [1, 2, 3], "miss_sku": [4, 5, 6]})
+    print(rendered.params)
```

### Comparing `bricks-py-0.0.8/bricks/spider/template.py` & `bricks-py-0.0.9/bricks/spider/template.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/state.py` & `bricks-py-0.0.9/bricks/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "VERSION",
 )
 
 # 当前 机器 ID
 MACHINE_ID = hashlib.sha256(uuid.UUID(int=uuid.getnode()).hex[-12:].encode()).hexdigest()
 
 # 当前框架版本
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 # 全局变量
 G = variable.VariableG()
 # 线程变量
 T = variable.VariableT()
```

### Comparing `bricks-py-0.0.8/bricks/utils/arrow.py` & `bricks-py-0.0.9/bricks/utils/arrow.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/utils/codes.py` & `bricks-py-0.0.9/bricks/utils/codes.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/utils/convert.py` & `bricks-py-0.0.9/bricks/utils/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,37 +10,54 @@
 from bricks.lib.items import Items
 from bricks.lib.request import Request
 from bricks.lib.response import Response
 from bricks.spider.air import Spider
 from bricks.utils import pandora
 
 
-def curl2resp(curl_cmd: str, spider: Spider = None) -> Response:
+def curl2resp(curl_cmd: str, options: dict = None) -> Response:
     """
     curl 转响应
 
     :param curl_cmd:
-    :param spider:
+    :param options:
     :return:
     """
     request = Request.from_curl(curl_cmd)
-    return req2resp(request, spider)
+    return req2resp(request, options)
 
 
-def req2resp(request: Request, spider: Spider = None) -> Response:
+def req2resp(request: Request, options: dict = None) -> Response:
     """
     请求转响应
 
     :param request:
-    :param spider:
+    :param options:
     :return:
     """
     dispatcher = contextlib.nullcontext()
-    if not spider:
-        spider = Spider()
+    options = options or {}
+    plugins: Union[dict, type(...), None] = options.pop("plugins", ...)
+
+    spider = Spider(**options)
+
+    # 不需要任何插件
+    if not plugins:
+        for plugin in spider.plugins:
+            plugin.unregister()
+
+    # 使用默认插件
+    elif plugins is ...:
+        pass
+
+    else:
+        for plugin in spider.plugins:
+            plugin.unregister()
+        for form, plugin in plugins:
+            spider.use(form, *pandora.iterable(plugin))
 
     if inspect.iscoroutinefunction(spider.downloader.fetch):
         dispatcher = spider.dispatcher
 
     with dispatcher:
         context = spider.make_context(
             request=request,
@@ -96,18 +113,18 @@
         return _obj
 
     if isinstance(obj, (dict, list)):
         obj = json.dumps(obj)
         encoding = "utf-8"
     else:
         encoding = None
-    resp = Response(content=ensure_bytes(obj), encoding=encoding)
+    res = Response(content=ensure_bytes(obj), encoding=encoding)
 
     return resp2items(
-        response=resp,
+        response=res,
         engine=engine,
         rules=rules,
         rename=rename,
         default=default,
         factory=factory,
         show=show
     )
@@ -129,9 +146,9 @@
   -H 'Sec-Fetch-Site: same-origin' \
   -H 'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36 Edg/118.0.2088.57' \
   -H 'X-Requested-With: XMLHttpRequest' \
   -H 'sec-ch-ua: "Chromium";v="118", "Microsoft Edge";v="118", "Not=A?Brand";v="99"' \
   -H 'sec-ch-ua-mobile: ?0' \
   -H 'sec-ch-ua-platform: "macOS"' \
   --compressed"""
-    resp = curl2resp(cmd)
+    resp = curl2resp(cmd, options={"proxy": {"ref": "bricks.lib.proxies.CustomProxy", "key": "127.0.0.1:7890"}})
     print(resp.text)
```

### Comparing `bricks-py-0.0.8/bricks/utils/csv_.py` & `bricks-py-0.0.9/bricks/utils/csv_.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/utils/fake/user_agent.py` & `bricks-py-0.0.9/bricks/utils/fake/user_agent.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/utils/pandora.py` & `bricks-py-0.0.9/bricks/utils/pandora.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks/utils/scheduler.py` & `bricks-py-0.0.9/bricks/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/bricks_py.egg-info/SOURCES.txt` & `bricks-py-0.0.9/bricks_py.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,31 +12,30 @@
 bricks/db/__init__.py
 bricks/db/mongo.py
 bricks/db/redis_.py
 bricks/db/sqlite.py
 bricks/downloader/__init__.py
 bricks/downloader/cffi.py
 bricks/downloader/curl.py
-bricks/downloader/genesis.py
 bricks/downloader/go_requests.py
+bricks/downloader/playwright_.py
 bricks/downloader/requests_.py
 bricks/lib/__init__.py
 bricks/lib/cookies.py
 bricks/lib/counter.py
 bricks/lib/extractors.py
 bricks/lib/headers.py
 bricks/lib/items.py
 bricks/lib/nodes.py
 bricks/lib/proxies.py
 bricks/lib/request.py
 bricks/lib/response.py
 bricks/lib/variable.py
 bricks/lib/queues/__init__.py
 bricks/lib/queues/cache.py
-bricks/lib/queues/genesis.py
 bricks/lib/queues/local.py
 bricks/lib/queues/redis_.py
 bricks/lib/queues/smart.py
 bricks/plugins/__init__.py
 bricks/plugins/make_seeds.py
 bricks/plugins/on_request.py
 bricks/plugins/scripts.py
@@ -59,8 +58,9 @@
 bricks_py.egg-info/dependency_links.txt
 bricks_py.egg-info/requires.txt
 bricks_py.egg-info/top_level.txt
 demos/__init__.py
 demos/air_spider_demo.py
 demos/dispatcher_test.py
 demos/form_spider_demo.py
+demos/form_spider_demo2.py
 demos/template_spider_demo.py
```

### Comparing `bricks-py-0.0.8/demos/air_spider_demo.py` & `bricks-py-0.0.9/demos/air_spider_demo.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/demos/dispatcher_test.py` & `bricks-py-0.0.9/demos/dispatcher_test.py`

 * *Files identical despite different names*

### Comparing `bricks-py-0.0.8/demos/form_spider_demo.py` & `bricks-py-0.0.9/demos/form_spider_demo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from bricks import const
+from bricks.core import signals
 from bricks.db.mongo import Mongo
 from bricks.db.sqlite import Sqlite
-from bricks.lib.queues import RedisQueue
 from bricks.plugins import scripts
 from bricks.spider import form
 
 sqlite = Sqlite("test")
 sqlite.create_table("user_info", structure={
     "userId": int,
     "roomId": int,
@@ -18,15 +19,15 @@
 
 class MySpider(form.Spider):
 
     @property
     def config(self) -> form.Config:
         return form.Config(
             init=[
-                form.Init(func=lambda: ({"page": i} for i in range(100)))
+                form.Init(func=lambda: {"page": 1})
             ],
             spider=[
                 form.Download(
                     url="https://fx1.service.kugou.com/mfanxing-home/h5/cdn/room/index/list_v2",
                     params={
                         "page": "{page}",
                         "cid": 6000
@@ -55,62 +56,65 @@
                                 "startTime": "startTime",
                                 "kugouId": "kugouId",
                                 "status": "status",
                             }
                         }
                     }
                 ),
-                form.Task(
-                    func=scripts.turn_page,
-                    kwargs={
-                        "match": [
-                            "context.response.get('data.hasNextPage') == 1"
-                        ],
-                        "call_later": True
-                    }
-                ),
-                form.Task(
-                    func=scripts.inject,
-                    kwargs={
-                        "flows": [
-                            "context = Context.get_context()",
-                            "logger.debug(context.seeds)"
-                        ]
-                    }
-                ),
-                # form.Pipeline(
-                #     func="bricks.plugins.storage.to_sqlite",
-                #     kwargs={
-                #         "conn": sqlite,
-                #         "path": "user_info"
-                #     },
-                #     success=True
-                # )
 
-                # form.Pipeline(
-                #     func="bricks.plugins.storage.to_mongo",
+                # form.Task(
+                #     func=scripts.turn_page,
                 #     kwargs={
-                #         "conn": mongo,
-                #         "path": "user_info",
-                #         "database": "live",
-                #         "row_keys": ['userId']
-                #     },
-                #     success=True
-                # )
+                #         "match": [
+                #             # "print(context.response.get('data.hasNextPage'))",
+                #             "context.response.get('data.hasNextPage') == 1"
+                #         ],
+                #         # "call_later": True
+                #     }
+                # ),
 
                 form.Pipeline(
-                    func=lambda context: print(context.items),
-                    success=True
+                    func=self.my_pipline,
+                    # success=True
                 )
-            ]
+            ],
+            events={
+                const.BEFORE_PIPELINE: [
+                    form.Task(
+                        func=scripts.turn_page,
+                        kwargs={
+                            "match": [
+                                # "print(context.response.get('data.hasNextPage'))",
+                                "context.response.get('data.hasNextPage') == 1"
+                            ],
+                            # "call_later": True
+                        }
+                    ),
+
+                ]
+            }
         )
 
+    def my_pipline(self, context: form.Context):
+        print(context.items)
+        raise signals.Success
+
+    # def tu(self, context: form.Context):
+    #     if context.response.get('data.hasNextPage') == 1:
+    #         download: form.Download = context.obtain('download')
+    #         seeds = {"page": context.seeds["page"] + 1}
+    #         req = download.render(seeds).to_request()
+    #         context.submit(req, attrs={"seeds": seeds})
+
 
 if __name__ == '__main__':
+    from bricks.downloader import playwright_
+
     spider = MySpider(
+        downloader=playwright_.Downloader(),
         # task_queue=RedisQueue()
     )
     # 使用调度器运行
     # spider.launch({"form": "interval", "exprs": "seconds=1"})
     # # 单次运行
     spider.run()
     # # survey 运行 -> 可以获取到执行的 Context
```

### Comparing `bricks-py-0.0.8/demos/template_spider_demo.py` & `bricks-py-0.0.9/demos/template_spider_demo.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,43 +3,35 @@
 # @Author  : Kem
 # @Desc    :
 import time
 
 from bricks import const
 from bricks.core import signals
 from bricks.lib.queues import RedisQueue
-from bricks.plugins.make_seeds import by_redis
 from bricks.spider import template
 from bricks.spider.template import Config
-from no_views.conn import redis, redis_config
 
 
 class Spider(template.Spider):
 
     def __init__(self, **kwargs):
 
         super().__init__(**kwargs)
 
     @property
     def config(self) -> Config:
         return Config(
             init=[
                 template.Init(
-                    func=by_redis,
+                    func=lambda: {"page": 1},
                     layout=template.Layout(
                         factory={
                             "time": lambda: time.time()
                         }
                     ),
-                    kwargs={
-                        "path": "test",
-                        "key_type": "test",
-                        "conn": redis,
-                        # "batch_size": 1000
-                    }
 
                 )
             ],
             events={
                 const.AFTER_REQUEST: [
                     template.Task(func=self.is_success),
                 ],
@@ -110,14 +102,12 @@
         if context.response.get('code') != 0:
             # 重试信号
             raise signals.Retry
 
 
 if __name__ == '__main__':
     spider = Spider(
-        task_queue=RedisQueue(
-            **redis_config
-        )
+        task_queue=RedisQueue()
     )
     spider.run(
         task_name='init',
     )
```

### Comparing `bricks-py-0.0.8/setup.py` & `bricks-py-0.0.9/setup.py`

 * *Files identical despite different names*


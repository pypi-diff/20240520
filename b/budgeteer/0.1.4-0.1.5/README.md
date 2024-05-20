# Comparing `tmp/budgeteer-0.1.4.tar.gz` & `tmp/budgeteer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgeteer-0.1.4.tar", last modified: Sun May 19 13:04:29 2024, max compression
+gzip compressed data, was "budgeteer-0.1.5.tar", last modified: Mon May 20 10:41:31 2024, max compression
```

## Comparing `budgeteer-0.1.4.tar` & `budgeteer-0.1.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.022253 budgeteer-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 13:04:03.000000 budgeteer-0.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-19 13:04:03.000000 budgeteer-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-19 13:04:29.022253 budgeteer-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-19 13:04:03.000000 budgeteer-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.014253 budgeteer-0.1.4/budgeteer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.018252 budgeteer-0.1.4/budgeteer/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.018252 budgeteer-0.1.4/budgeteer/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.018252 budgeteer-0.1.4/budgeteer/web_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.014253 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.018252 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.022253 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    85787 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
--rw-r--r--   0 runner    (1001) docker     (127)    64371 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
--rw-r--r--   0 runner    (1001) docker     (127)    28960 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
--rw-r--r--   0 runner    (1001) docker     (127)   231964 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
--rw-r--r--   0 runner    (1001) docker     (127)    60654 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
--rw-r--r--   0 runner    (1001) docker     (127)   164360 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (127)    76081 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
--rw-r--r--   0 runner    (1001) docker     (127)   121340 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    24455 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js
--rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
--rw-r--r--   0 runner    (1001) docker     (127)    51150 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
--rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
--rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-05-19 13:04:03.000000 budgeteer-0.1.4/budgeteer/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:04:29.014253 budgeteer-0.1.4/budgeteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-19 13:04:29.000000 budgeteer-0.1.4/budgeteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 13:04:28.000000 budgeteer-0.1.4/budgeteer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:04:29.022253 budgeteer-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-19 13:04:03.000000 budgeteer-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.886628 budgeteer-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 10:41:09.000000 budgeteer-0.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 10:41:09.000000 budgeteer-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-20 10:41:31.886628 budgeteer-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-20 10:41:09.000000 budgeteer-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.878628 budgeteer-0.1.5/budgeteer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.882628 budgeteer-0.1.5/budgeteer/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.882628 budgeteer-0.1.5/budgeteer/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.882628 budgeteer-0.1.5/budgeteer/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.878628 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.882628 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.886628 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    85787 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    64371 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28960 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
+-rw-r--r--   0 runner    (1001) docker     (127)   231964 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
+-rw-r--r--   0 runner    (1001) docker     (127)    60654 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   164360 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76081 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121340 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    24455 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51150 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-05-20 10:41:09.000000 budgeteer-0.1.5/budgeteer/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:41:31.882628 budgeteer-0.1.5/budgeteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 10:41:31.000000 budgeteer-0.1.5/budgeteer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:41:31.886628 budgeteer-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-20 10:41:09.000000 budgeteer-0.1.5/setup.py
```

### Comparing `budgeteer-0.1.4/LICENSE.md` & `budgeteer-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/PKG-INFO` & `budgeteer-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgeteer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Einfacher Überblick über das eigene Budget
 Home-page: https://github.com/rix1337/BudgeTeer
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `budgeteer-0.1.4/README.md` & `budgeteer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/providers/common_functions.py` & `budgeteer-0.1.5/budgeteer/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/providers/config.py` & `budgeteer-0.1.5/budgeteer/providers/config.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/providers/http_requests/cache_handler.py` & `budgeteer-0.1.5/budgeteer/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/providers/http_requests/cloudflare_handlers.py` & `budgeteer-0.1.5/budgeteer/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/providers/http_requests/request_handler.py` & `budgeteer-0.1.5/budgeteer/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/providers/shared_state.py` & `budgeteer-0.1.5/budgeteer/providers/shared_state.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/providers/sqlite_database.py` & `budgeteer-0.1.5/budgeteer/providers/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/providers/version.py` & `budgeteer-0.1.5/budgeteer/providers/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "0.1.4"
+    return "0.1.5"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `budgeteer-0.1.4/budgeteer/run.py` & `budgeteer-0.1.5/budgeteer/run.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/vuejs_frontend/dist/index.html` & `budgeteer-0.1.5/budgeteer/web_interface/vuejs_frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer/web_interface/web_server.py` & `budgeteer-0.1.5/budgeteer/web_interface/web_server.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/budgeteer.egg-info/PKG-INFO` & `budgeteer-0.1.5/budgeteer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgeteer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Einfacher Überblick über das eigene Budget
 Home-page: https://github.com/rix1337/BudgeTeer
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `budgeteer-0.1.4/budgeteer.egg-info/SOURCES.txt` & `budgeteer-0.1.5/budgeteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.4/setup.py` & `budgeteer-0.1.5/setup.py`

 * *Files identical despite different names*


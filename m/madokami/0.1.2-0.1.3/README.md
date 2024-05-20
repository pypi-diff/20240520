# Comparing `tmp/madokami-0.1.2.tar.gz` & `tmp/madokami-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madokami-0.1.2.tar", max compression
+gzip compressed data, was "madokami-0.1.3.tar", max compression
```

## Comparing `madokami-0.1.2.tar` & `madokami-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       26 2024-05-18 20:36:30.412937 madokami-0.1.2/README.md
--rw-r--r--   0        0        0      160 2024-04-21 19:50:38.326411 madokami-0.1.2/madokami/__init__.py
--rw-r--r--   0        0        0      602 2024-05-18 07:22:56.118748 madokami-0.1.2/madokami/api/__init__.py
--rw-r--r--   0        0        0      525 2024-05-18 07:23:24.607036 madokami-0.1.2/madokami/api/app.py
--rw-r--r--   0        0        0     4074 2024-05-18 01:58:36.106403 madokami-0.1.2/madokami/api/downloads.py
--rw-r--r--   0        0        0     1171 2024-05-13 02:49:57.491222 madokami-0.1.2/madokami/api/engines.py
--rw-r--r--   0        0        0      517 2024-05-17 02:48:25.866035 madokami-0.1.2/madokami/api/logs.py
--rw-r--r--   0        0        0     2189 2024-04-30 05:00:11.850809 madokami-0.1.2/madokami/api/media.py
--rw-r--r--   0        0        0     3015 2024-05-18 07:01:02.388989 madokami-0.1.2/madokami/api/models.py
--rw-r--r--   0        0        0     1948 2024-05-12 13:33:26.276521 madokami-0.1.2/madokami/api/plugins.py
--rw-r--r--   0        0        0     1496 2024-05-17 23:53:16.295962 madokami-0.1.2/madokami/api/register.py
--rw-r--r--   0        0        0     2627 2024-05-18 06:58:58.825707 madokami-0.1.2/madokami/api/scheduler.py
--rw-r--r--   0        0        0     1957 2024-05-15 16:19:59.207775 madokami-0.1.2/madokami/api/settings.py
--rw-r--r--   0        0        0     3021 2024-05-17 04:28:28.426201 madokami-0.1.2/madokami/api/subscribe.py
--rw-r--r--   0        0        0        0 2024-04-29 01:48:06.182046 madokami-0.1.2/madokami/api/utils.py
--rw-r--r--   0        0        0      215 2024-04-21 19:50:38.330738 madokami-0.1.2/madokami/app.py
--rw-r--r--   0        0        0     1088 2024-05-18 18:47:45.951393 madokami-0.1.2/madokami/config.py
--rw-r--r--   0        0        0     7854 2024-05-18 06:56:28.905698 madokami-0.1.2/madokami/crud.py
--rw-r--r--   0        0        0      748 2024-04-18 18:55:51.445120 madokami-0.1.2/madokami/db.py
--rw-r--r--   0        0        0       58 2024-04-19 16:00:57.987815 madokami-0.1.2/madokami/drivers/__init__.py
--rw-r--r--   0        0        0     1143 2024-05-18 22:04:37.489617 madokami-0.1.2/madokami/drivers/app.py
--rw-r--r--   0        0        0      691 2024-05-18 22:07:18.555001 madokami-0.1.2/madokami/drivers/deps.py
--rw-r--r--   0        0        0     1150 2024-04-19 15:58:56.300037 madokami-0.1.2/madokami/drivers/hooks.py
--rw-r--r--   0        0        0     3317 2024-05-18 07:22:56.125901 madokami-0.1.2/madokami/drivers/madokami.py
--rw-r--r--   0        0        0      276 2024-04-21 20:05:51.108606 madokami-0.1.2/madokami/drivers/router.py
--rw-r--r--   0        0        0        0 2024-04-17 21:56:18.236636 madokami-0.1.2/madokami/internal/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-17 04:02:26.686931 madokami-0.1.2/madokami/internal/core_config.py
--rw-r--r--   0        0        0        0 2024-04-29 09:24:55.711542 madokami-0.1.2/madokami/internal/default_plugins/__init__.py
--rw-r--r--   0        0        0     2103 2024-04-29 09:27:02.804424 madokami-0.1.2/madokami/internal/default_plugins/bangumi_requester.py
--rw-r--r--   0        0        0     7983 2024-05-18 08:17:58.567517 madokami-0.1.2/madokami/internal/default_plugins/default_downloader.py
--rw-r--r--   0        0        0     1220 2024-05-18 15:15:17.837703 madokami-0.1.2/madokami/internal/default_plugins/default_requester.py
--rw-r--r--   0        0        0     1569 2024-04-29 03:28:47.980966 madokami-0.1.2/madokami/internal/downloader.py
--rw-r--r--   0        0        0     2337 2024-05-16 22:38:56.274073 madokami-0.1.2/madokami/internal/models.py
--rw-r--r--   0        0        0     2204 2024-04-29 01:40:43.791427 madokami-0.1.2/madokami/internal/scheduler.py
--rw-r--r--   0        0        0     1828 2024-05-18 18:22:06.475757 madokami-0.1.2/madokami/internal/settings.py
--rw-r--r--   0        0        0     1273 2024-04-29 10:33:18.819150 madokami-0.1.2/madokami/internal/utils.py
--rw-r--r--   0        0        0     2870 2024-05-17 02:50:28.680331 madokami-0.1.2/madokami/log.py
--rw-r--r--   0        0        0     2248 2024-04-29 09:11:41.963790 madokami-0.1.2/madokami/models.py
--rw-r--r--   0        0        0      102 2024-04-19 07:04:58.251852 madokami-0.1.2/madokami/plugin/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 20:56:49.430527 madokami-0.1.2/madokami/plugin/backend/__init__.py
--rw-r--r--   0        0        0      396 2024-04-19 00:44:26.847710 madokami-0.1.2/madokami/plugin/backend/downloader.py
--rw-r--r--   0        0        0      637 2024-04-28 05:02:24.433471 madokami-0.1.2/madokami/plugin/backend/engine.py
--rw-r--r--   0        0        0      430 2024-05-12 22:55:06.238039 madokami-0.1.2/madokami/plugin/backend/models.py
--rw-r--r--   0        0        0      271 2024-04-18 05:26:07.664373 madokami-0.1.2/madokami/plugin/backend/parser.py
--rw-r--r--   0        0        0      312 2024-04-19 01:53:23.037566 madokami-0.1.2/madokami/plugin/backend/requester.py
--rw-r--r--   0        0        0      730 2024-05-12 22:51:26.981727 madokami-0.1.2/madokami/plugin/basic_plugin.py
--rw-r--r--   0        0        0      609 2024-04-28 13:11:05.653144 madokami-0.1.2/madokami/plugin/engine_register.py
--rw-r--r--   0        0        0      950 2024-04-19 15:58:56.303370 madokami-0.1.2/madokami/plugin/hooks.py
--rw-r--r--   0        0        0     8522 2024-05-16 22:38:56.271309 madokami-0.1.2/madokami/plugin/manager.py
--rw-r--r--   0        0        0      104 2024-05-11 22:42:57.785966 madokami-0.1.2/madokami/plugin/models.py
--rw-r--r--   0        0        0     1326 2024-05-16 22:34:17.155970 madokami-0.1.2/madokami/plugin/settings_register.py
--rw-r--r--   0        0        0      537 2024-05-11 22:42:57.803098 madokami-0.1.2/madokami/plugin/subscription.py
--rw-r--r--   0        0        0      441 2024-05-11 22:42:57.810307 madokami-0.1.2/madokami/plugin/subscription_regiser.py
--rw-r--r--   0        0        0      348 2024-04-19 17:11:26.334662 madokami-0.1.2/madokami/util.py
--rw-r--r--   0        0        0      548 2024-05-18 22:11:31.824891 madokami-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 madokami-0.1.2/setup.py
--rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 madokami-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-18 20:36:30.412937 madokami-0.1.3/README.md
+-rw-r--r--   0        0        0      160 2024-04-21 19:50:38.326411 madokami-0.1.3/madokami/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-18 07:22:56.118748 madokami-0.1.3/madokami/api/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-18 07:23:24.607036 madokami-0.1.3/madokami/api/app.py
+-rw-r--r--   0        0        0     4074 2024-05-18 01:58:36.106403 madokami-0.1.3/madokami/api/downloads.py
+-rw-r--r--   0        0        0     1171 2024-05-13 02:49:57.491222 madokami-0.1.3/madokami/api/engines.py
+-rw-r--r--   0        0        0      517 2024-05-17 02:48:25.866035 madokami-0.1.3/madokami/api/logs.py
+-rw-r--r--   0        0        0     2189 2024-04-30 05:00:11.850809 madokami-0.1.3/madokami/api/media.py
+-rw-r--r--   0        0        0     3015 2024-05-18 07:01:02.388989 madokami-0.1.3/madokami/api/models.py
+-rw-r--r--   0        0        0     1948 2024-05-12 13:33:26.276521 madokami-0.1.3/madokami/api/plugins.py
+-rw-r--r--   0        0        0     1496 2024-05-17 23:53:16.295962 madokami-0.1.3/madokami/api/register.py
+-rw-r--r--   0        0        0     2627 2024-05-18 06:58:58.825707 madokami-0.1.3/madokami/api/scheduler.py
+-rw-r--r--   0        0        0     1957 2024-05-15 16:19:59.207775 madokami-0.1.3/madokami/api/settings.py
+-rw-r--r--   0        0        0     3021 2024-05-17 04:28:28.426201 madokami-0.1.3/madokami/api/subscribe.py
+-rw-r--r--   0        0        0        0 2024-04-29 01:48:06.182046 madokami-0.1.3/madokami/api/utils.py
+-rw-r--r--   0        0        0      215 2024-04-21 19:50:38.330738 madokami-0.1.3/madokami/app.py
+-rw-r--r--   0        0        0     1088 2024-05-18 18:47:45.951393 madokami-0.1.3/madokami/config.py
+-rw-r--r--   0        0        0     7854 2024-05-18 06:56:28.905698 madokami-0.1.3/madokami/crud.py
+-rw-r--r--   0        0        0      748 2024-04-18 18:55:51.445120 madokami-0.1.3/madokami/db.py
+-rw-r--r--   0        0        0       58 2024-04-19 16:00:57.987815 madokami-0.1.3/madokami/drivers/__init__.py
+-rw-r--r--   0        0        0     1143 2024-05-18 22:04:37.489617 madokami-0.1.3/madokami/drivers/app.py
+-rw-r--r--   0        0        0      691 2024-05-18 22:07:18.555001 madokami-0.1.3/madokami/drivers/deps.py
+-rw-r--r--   0        0        0     1150 2024-04-19 15:58:56.300037 madokami-0.1.3/madokami/drivers/hooks.py
+-rw-r--r--   0        0        0     3317 2024-05-18 07:22:56.125901 madokami-0.1.3/madokami/drivers/madokami.py
+-rw-r--r--   0        0        0      276 2024-04-21 20:05:51.108606 madokami-0.1.3/madokami/drivers/router.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:56:18.236636 madokami-0.1.3/madokami/internal/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-17 04:02:26.686931 madokami-0.1.3/madokami/internal/core_config.py
+-rw-r--r--   0        0        0        0 2024-04-29 09:24:55.711542 madokami-0.1.3/madokami/internal/default_plugins/__init__.py
+-rw-r--r--   0        0        0     2103 2024-04-29 09:27:02.804424 madokami-0.1.3/madokami/internal/default_plugins/bangumi_requester.py
+-rw-r--r--   0        0        0     7991 2024-05-19 06:50:53.366405 madokami-0.1.3/madokami/internal/default_plugins/default_downloader.py
+-rw-r--r--   0        0        0     1220 2024-05-18 15:15:17.837703 madokami-0.1.3/madokami/internal/default_plugins/default_requester.py
+-rw-r--r--   0        0        0     1569 2024-04-29 03:28:47.980966 madokami-0.1.3/madokami/internal/downloader.py
+-rw-r--r--   0        0        0     2337 2024-05-16 22:38:56.274073 madokami-0.1.3/madokami/internal/models.py
+-rw-r--r--   0        0        0     2204 2024-04-29 01:40:43.791427 madokami-0.1.3/madokami/internal/scheduler.py
+-rw-r--r--   0        0        0     1881 2024-05-19 06:50:53.369340 madokami-0.1.3/madokami/internal/settings.py
+-rw-r--r--   0        0        0     1273 2024-04-29 10:33:18.819150 madokami-0.1.3/madokami/internal/utils.py
+-rw-r--r--   0        0        0     2870 2024-05-17 02:50:28.680331 madokami-0.1.3/madokami/log.py
+-rw-r--r--   0        0        0     2248 2024-04-29 09:11:41.963790 madokami-0.1.3/madokami/models.py
+-rw-r--r--   0        0        0      102 2024-04-19 07:04:58.251852 madokami-0.1.3/madokami/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:56:49.430527 madokami-0.1.3/madokami/plugin/backend/__init__.py
+-rw-r--r--   0        0        0      396 2024-04-19 00:44:26.847710 madokami-0.1.3/madokami/plugin/backend/downloader.py
+-rw-r--r--   0        0        0      637 2024-04-28 05:02:24.433471 madokami-0.1.3/madokami/plugin/backend/engine.py
+-rw-r--r--   0        0        0      430 2024-05-12 22:55:06.238039 madokami-0.1.3/madokami/plugin/backend/models.py
+-rw-r--r--   0        0        0      271 2024-04-18 05:26:07.664373 madokami-0.1.3/madokami/plugin/backend/parser.py
+-rw-r--r--   0        0        0      312 2024-04-19 01:53:23.037566 madokami-0.1.3/madokami/plugin/backend/requester.py
+-rw-r--r--   0        0        0      730 2024-05-12 22:51:26.981727 madokami-0.1.3/madokami/plugin/basic_plugin.py
+-rw-r--r--   0        0        0      609 2024-04-28 13:11:05.653144 madokami-0.1.3/madokami/plugin/engine_register.py
+-rw-r--r--   0        0        0      950 2024-04-19 15:58:56.303370 madokami-0.1.3/madokami/plugin/hooks.py
+-rw-r--r--   0        0        0     8522 2024-05-16 22:38:56.271309 madokami-0.1.3/madokami/plugin/manager.py
+-rw-r--r--   0        0        0      104 2024-05-11 22:42:57.785966 madokami-0.1.3/madokami/plugin/models.py
+-rw-r--r--   0        0        0     1326 2024-05-16 22:34:17.155970 madokami-0.1.3/madokami/plugin/settings_register.py
+-rw-r--r--   0        0        0      537 2024-05-11 22:42:57.803098 madokami-0.1.3/madokami/plugin/subscription.py
+-rw-r--r--   0        0        0      441 2024-05-11 22:42:57.810307 madokami-0.1.3/madokami/plugin/subscription_regiser.py
+-rw-r--r--   0        0        0      348 2024-04-19 17:11:26.334662 madokami-0.1.3/madokami/util.py
+-rw-r--r--   0        0        0      548 2024-05-19 14:49:52.049441 madokami-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 madokami-0.1.3/setup.py
+-rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 madokami-0.1.3/PKG-INFO
```

### Comparing `madokami-0.1.2/madokami/api/__init__.py` & `madokami-0.1.3/madokami/api/__init__.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/app.py` & `madokami-0.1.3/madokami/api/app.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/downloads.py` & `madokami-0.1.3/madokami/api/downloads.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/engines.py` & `madokami-0.1.3/madokami/api/engines.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/logs.py` & `madokami-0.1.3/madokami/api/logs.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/media.py` & `madokami-0.1.3/madokami/api/media.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/models.py` & `madokami-0.1.3/madokami/api/models.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/plugins.py` & `madokami-0.1.3/madokami/api/plugins.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/register.py` & `madokami-0.1.3/madokami/api/register.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/scheduler.py` & `madokami-0.1.3/madokami/api/scheduler.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/settings.py` & `madokami-0.1.3/madokami/api/settings.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/api/subscribe.py` & `madokami-0.1.3/madokami/api/subscribe.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/config.py` & `madokami-0.1.3/madokami/config.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/crud.py` & `madokami-0.1.3/madokami/crud.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/db.py` & `madokami-0.1.3/madokami/db.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/drivers/app.py` & `madokami-0.1.3/madokami/drivers/app.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/drivers/deps.py` & `madokami-0.1.3/madokami/drivers/deps.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/drivers/hooks.py` & `madokami-0.1.3/madokami/drivers/hooks.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/drivers/madokami.py` & `madokami-0.1.3/madokami/drivers/madokami.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/internal/core_config.py` & `madokami-0.1.3/madokami/internal/core_config.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/internal/default_plugins/bangumi_requester.py` & `madokami-0.1.3/madokami/internal/default_plugins/bangumi_requester.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/internal/default_plugins/default_downloader.py` & `madokami-0.1.3/madokami/internal/default_plugins/default_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 class DefaultAria2Downloader(Downloader):
 
     def __init__(self):
         self._status = "Initialized"
         aria2_host = get_config('madokami.config.aria2_host', default='http://localhost')
         aria2_port = get_config('madokami.config.aria2_port', default='6800')
-        aria2_secret = get_config('madokami.config.aria2_secret', default='')
+        aria2_secret = get_config('madokami.config.aria2_secret', default='MADOKAMI')
         if aria2_host is None or aria2_port is None or aria2_secret is None:
             raise ValueError('Aria2 configuration is not set')
         client = aria2p.Client(
             host=aria2_host,
             port=int(aria2_port),
             secret=aria2_secret
         )
```

### Comparing `madokami-0.1.2/madokami/internal/default_plugins/default_requester.py` & `madokami-0.1.3/madokami/internal/default_plugins/default_requester.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/internal/downloader.py` & `madokami-0.1.3/madokami/internal/downloader.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/internal/models.py` & `madokami-0.1.3/madokami/internal/models.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/internal/scheduler.py` & `madokami-0.1.3/madokami/internal/scheduler.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/internal/settings.py` & `madokami-0.1.3/madokami/internal/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,28 +15,28 @@
         'name': '缓存路径',
         'description': '为Madokami设置缓存路径',
         'default': './data/cache'
     },
     {
         'key': 'madokami.config.aria2_host',
         'name': 'Aria2 地址',
-        'description': '为下载器指定Aria2地址',
+        'description': '为下载器指定Aria2地址 (重启生效)',
         'default': 'http://localhost'
     },
     {
         'key': 'madokami.config.aria2_port',
         'name': 'Aria2 端口',
-        'description': '为下载器指定Aria2端口',
+        'description': '为下载器指定Aria2端口 (重启生效)',
         'default': 6800
     },
     {
         'key': 'madokami.config.aria2_secret',
         'name': 'Aria2 密钥',
-        'description': '为下载器指定PRC密钥',
-        'default': ''
+        'description': '为下载器指定PRC密钥 (重启生效)',
+        'default': 'MADOKAMI'
     },
     {
         'key': 'madokami.config.bangumi_token',
         'name': 'Bangumi秘钥',
         'description': '用于Bangumi API请求的秘钥，请勿滥用',
         'default': '8jkdHoKPLrOuI3WN8Xv5BLMp0MgAZ5Dk7KXP2i4j'
     }
```

### Comparing `madokami-0.1.2/madokami/internal/utils.py` & `madokami-0.1.3/madokami/internal/utils.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/log.py` & `madokami-0.1.3/madokami/log.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/models.py` & `madokami-0.1.3/madokami/models.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/plugin/backend/engine.py` & `madokami-0.1.3/madokami/plugin/backend/engine.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/plugin/basic_plugin.py` & `madokami-0.1.3/madokami/plugin/basic_plugin.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/plugin/engine_register.py` & `madokami-0.1.3/madokami/plugin/engine_register.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/plugin/hooks.py` & `madokami-0.1.3/madokami/plugin/hooks.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/plugin/manager.py` & `madokami-0.1.3/madokami/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/plugin/settings_register.py` & `madokami-0.1.3/madokami/plugin/settings_register.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/madokami/plugin/subscription.py` & `madokami-0.1.3/madokami/plugin/subscription.py`

 * *Files identical despite different names*

### Comparing `madokami-0.1.2/pyproject.toml` & `madokami-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "madokami"
-version = "0.1.2"
+version = "0.1.3"
 description = "A core library for madokami"
 authors = ["Hongpei Zheng <summerkirakira@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.110.1"
```

### Comparing `madokami-0.1.2/setup.py` & `madokami-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'requests>=2.31.0,<3.0.0',
  'sqlalchemy>=2.0.29,<3.0.0',
  'sqlmodel>=0.0.16,<0.0.17',
  'uvicorn>=0.29.0,<0.30.0']
 
 setup_kwargs = {
     'name': 'madokami',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A core library for madokami',
     'long_description': 'Madokami项目的核心库',
     'author': 'Hongpei Zheng',
     'author_email': 'summerkirakira@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `madokami-0.1.2/PKG-INFO` & `madokami-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madokami
-Version: 0.1.2
+Version: 0.1.3
 Summary: A core library for madokami
 Author: Hongpei Zheng
 Author-email: summerkirakira@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


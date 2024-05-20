# Comparing `tmp/mrkutil-1.3.6.tar.gz` & `tmp/mrkutil-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrkutil-1.3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mrkutil-1.3.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mrkutil-1.3.6.tar` & `mrkutil-1.3.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       91 2024-04-10 18:38:36.896155 mrkutil-1.3.6/.flake8
--rw-r--r--   0        0        0     1800 2024-04-10 13:44:48.196615 mrkutil-1.3.6/.gitignore
--rw-r--r--   0        0        0      366 2024-04-10 18:38:32.560123 mrkutil-1.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2024-04-10 13:44:48.196615 mrkutil-1.3.6/LICENSE
--rw-r--r--   0        0        0     3057 2024-04-11 06:14:47.021960 mrkutil-1.3.6/README.md
--rw-r--r--   0        0        0      113 2024-05-10 05:30:31.272029 mrkutil-1.3.6/mrkutil/__init__.py
--rw-r--r--   0        0        0       72 2024-04-10 13:44:48.196615 mrkutil-1.3.6/mrkutil/base/__init__.py
--rw-r--r--   0        0        0     1748 2024-04-10 19:00:33.746768 mrkutil-1.3.6/mrkutil/base/base_handler.py
--rw-r--r--   0        0        0       94 2024-04-29 09:23:03.607864 mrkutil-1.3.6/mrkutil/cache/__init__.py
--rw-r--r--   0        0        0     5275 2024-05-10 05:30:19.239832 mrkutil-1.3.6/mrkutil/cache/base_redis.py
--rw-r--r--   0        0        0      262 2024-04-24 12:44:29.700772 mrkutil-1.3.6/mrkutil/communication/__init__.py
--rw-r--r--   0        0        0     1462 2024-04-24 11:50:42.829911 mrkutil-1.3.6/mrkutil/communication/call_service.py
--rw-r--r--   0        0        0     3162 2024-04-24 14:31:17.548693 mrkutil-1.3.6/mrkutil/communication/listen.py
--rw-r--r--   0        0        0     1375 2024-04-24 12:37:29.267696 mrkutil-1.3.6/mrkutil/communication/trigger_service.py
--rw-r--r--   0        0        0      154 2024-04-10 13:44:48.196615 mrkutil-1.3.6/mrkutil/logging/__init__.py
--rw-r--r--   0        0        0     2681 2024-04-10 19:05:36.249709 mrkutil-1.3.6/mrkutil/logging/logging_config.py
--rw-r--r--   0        0        0     1831 2024-04-10 19:05:53.713880 mrkutil-1.3.6/mrkutil/logging/logging_formatter.py
--rw-r--r--   0        0        0       82 2024-05-09 15:50:48.203270 mrkutil-1.3.6/mrkutil/pagination/__init__.py
--rw-r--r--   0        0        0      805 2024-04-10 19:06:55.098484 mrkutil-1.3.6/mrkutil/pagination/dependency.py
--rw-r--r--   0        0        0     1692 2024-04-10 19:12:12.205642 mrkutil-1.3.6/mrkutil/pagination/mongoengine.py
--rw-r--r--   0        0        0     3051 2024-05-09 17:18:46.497731 mrkutil-1.3.6/mrkutil/pagination/sqlalchemy.py
--rw-r--r--   0        0        0       77 2024-04-10 18:53:14.101683 mrkutil-1.3.6/mrkutil/responses/__init__.py
--rw-r--r--   0        0        0     3225 2024-04-12 08:51:40.055110 mrkutil-1.3.6/mrkutil/responses/response_helper.py
--rw-r--r--   0        0        0      256 2024-04-10 18:53:21.969785 mrkutil-1.3.6/mrkutil/utilities.py
--rw-r--r--   0        0        0      822 2024-04-24 12:36:34.647032 mrkutil-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mrkutil-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-10 18:38:36.896155 mrkutil-1.3.7/.flake8
+-rw-r--r--   0        0        0     1800 2024-04-10 13:44:48.196615 mrkutil-1.3.7/.gitignore
+-rw-r--r--   0        0        0      366 2024-04-10 18:38:32.560123 mrkutil-1.3.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2024-04-10 13:44:48.196615 mrkutil-1.3.7/LICENSE
+-rw-r--r--   0        0        0     3057 2024-04-11 06:14:47.021960 mrkutil-1.3.7/README.md
+-rw-r--r--   0        0        0      113 2024-05-20 20:08:12.753407 mrkutil-1.3.7/mrkutil/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-10 13:44:48.196615 mrkutil-1.3.7/mrkutil/base/__init__.py
+-rw-r--r--   0        0        0     1748 2024-04-10 19:00:33.746768 mrkutil-1.3.7/mrkutil/base/base_handler.py
+-rw-r--r--   0        0        0       94 2024-04-29 09:23:03.607864 mrkutil-1.3.7/mrkutil/cache/__init__.py
+-rw-r--r--   0        0        0     5277 2024-05-20 20:06:54.992462 mrkutil-1.3.7/mrkutil/cache/base_redis.py
+-rw-r--r--   0        0        0      262 2024-04-24 12:44:29.700772 mrkutil-1.3.7/mrkutil/communication/__init__.py
+-rw-r--r--   0        0        0     1462 2024-04-24 11:50:42.829911 mrkutil-1.3.7/mrkutil/communication/call_service.py
+-rw-r--r--   0        0        0     3162 2024-04-24 14:31:17.548693 mrkutil-1.3.7/mrkutil/communication/listen.py
+-rw-r--r--   0        0        0     1375 2024-04-24 12:37:29.267696 mrkutil-1.3.7/mrkutil/communication/trigger_service.py
+-rw-r--r--   0        0        0      154 2024-04-10 13:44:48.196615 mrkutil-1.3.7/mrkutil/logging/__init__.py
+-rw-r--r--   0        0        0     2681 2024-04-10 19:05:36.249709 mrkutil-1.3.7/mrkutil/logging/logging_config.py
+-rw-r--r--   0        0        0     1831 2024-04-10 19:05:53.713880 mrkutil-1.3.7/mrkutil/logging/logging_formatter.py
+-rw-r--r--   0        0        0       82 2024-05-09 15:50:48.203270 mrkutil-1.3.7/mrkutil/pagination/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-10 19:06:55.098484 mrkutil-1.3.7/mrkutil/pagination/dependency.py
+-rw-r--r--   0        0        0     1692 2024-04-10 19:12:12.205642 mrkutil-1.3.7/mrkutil/pagination/mongoengine.py
+-rw-r--r--   0        0        0     3066 2024-05-20 18:24:46.326210 mrkutil-1.3.7/mrkutil/pagination/sqlalchemy.py
+-rw-r--r--   0        0        0       77 2024-04-10 18:53:14.101683 mrkutil-1.3.7/mrkutil/responses/__init__.py
+-rw-r--r--   0        0        0     3225 2024-04-12 08:51:40.055110 mrkutil-1.3.7/mrkutil/responses/response_helper.py
+-rw-r--r--   0        0        0      256 2024-04-10 18:53:21.969785 mrkutil-1.3.7/mrkutil/utilities.py
+-rw-r--r--   0        0        0      822 2024-04-24 12:36:34.647032 mrkutil-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mrkutil-1.3.7/PKG-INFO
```

### Comparing `mrkutil-1.3.6/.gitignore` & `mrkutil-1.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/LICENSE` & `mrkutil-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/README.md` & `mrkutil-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/base/base_handler.py` & `mrkutil-1.3.7/mrkutil/base/base_handler.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/cache/base_redis.py` & `mrkutil-1.3.7/mrkutil/cache/base_redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,17 @@
     def __del__(self):
         # Close connection when this object is destroyed
         import asyncio
 
         try:
             loop = asyncio.get_event_loop()
             if loop.is_running():
-                loop.create_task(self.server.close())
+                loop.create_task(self.server.aclose())
             else:
-                loop.run_until_complete(self.server.close())
+                loop.run_until_complete(self.server.aclose())
         except Exception:
             pass
 
     async def _setData(self, key, data):
         if self._cache_timeout:
             await self.server.set(key, data, self._cache_timeout)
         else:
```

### Comparing `mrkutil-1.3.6/mrkutil/communication/call_service.py` & `mrkutil-1.3.7/mrkutil/communication/call_service.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/communication/listen.py` & `mrkutil-1.3.7/mrkutil/communication/listen.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/communication/trigger_service.py` & `mrkutil-1.3.7/mrkutil/communication/trigger_service.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/logging/logging_config.py` & `mrkutil-1.3.7/mrkutil/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/logging/logging_formatter.py` & `mrkutil-1.3.7/mrkutil/logging/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/pagination/dependency.py` & `mrkutil-1.3.7/mrkutil/pagination/dependency.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/pagination/mongoengine.py` & `mrkutil-1.3.7/mrkutil/pagination/mongoengine.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/mrkutil/pagination/sqlalchemy.py` & `mrkutil-1.3.7/mrkutil/pagination/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 def _sort_by(query: Select, direction: Optional[str], sort_by: Optional[str]) -> Select:
     """
     Sorts query by a specific column in ascending or descending order,
     after verifying that the column exists.
     """
     if sort_by:
-        columns = [column.key for column in inspect(query).c]
+        columns = [column.key for column in inspect(query).selected_columns]
         if sort_by not in columns:
             sort_by = None
 
     if sort_by and direction == "desc":
         query = query.order_by(desc(sort_by))
     elif sort_by and direction == "asc":
         query = query.order_by(asc(sort_by))
```

### Comparing `mrkutil-1.3.6/mrkutil/responses/response_helper.py` & `mrkutil-1.3.7/mrkutil/responses/response_helper.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/pyproject.toml` & `mrkutil-1.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mrkutil-1.3.6/PKG-INFO` & `mrkutil-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrkutil
-Version: 1.3.6
+Version: 1.3.7
 Summary: Python package containing common functions for python service based architecture.
 Author-email: Nebojsa Mrkic <mrkic.nebojsa@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: RabbitMQPubSub>=1.1.1
 Requires-Dist: redis>=4.3 ; extra == "extras"
 Requires-Dist: sqlalchemy>=1.4 ; extra == "extras"
```


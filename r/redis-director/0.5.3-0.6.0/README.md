# Comparing `tmp/redis_director-0.5.3.tar.gz` & `tmp/redis_director-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_director-0.5.3.tar", max compression
+gzip compressed data, was "redis_director-0.6.0.tar", max compression
```

## Comparing `redis_director-0.5.3.tar` & `redis_director-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2113 2024-05-16 08:23:46.385495 redis_director-0.5.3/README.md
--rw-r--r--   0        0        0      320 2024-05-16 08:23:38.733336 redis_director-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      131 2024-05-16 07:14:20.616944 redis_director-0.5.3/redis_director/__init__.py
--rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.5.3/redis_director/constants.py
--rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.5.3/redis_director/handler.py
--rw-r--r--   0        0        0     2342 2024-05-16 07:46:49.594320 redis_director-0.5.3/redis_director/publisher.py
--rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.5.3/redis_director/subscriber.py
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 redis_director-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     2113 2024-05-16 08:23:46.385495 redis_director-0.6.0/README.md
+-rw-r--r--   0        0        0      320 2024-05-20 00:58:50.092792 redis_director-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      266 2024-05-20 00:59:00.829045 redis_director-0.6.0/redis_director/__init__.py
+-rw-r--r--   0        0        0      760 2024-05-20 00:58:27.508256 redis_director-0.6.0/redis_director/callback.py
+-rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.6.0/redis_director/constants.py
+-rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.6.0/redis_director/handler.py
+-rw-r--r--   0        0        0     4154 2024-05-20 00:55:55.652461 redis_director-0.6.0/redis_director/publisher.py
+-rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.6.0/redis_director/subscriber.py
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 redis_director-0.6.0/PKG-INFO
```

### Comparing `redis_director-0.5.3/README.md` & `redis_director-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `redis_director-0.5.3/redis_director/constants.py` & `redis_director-0.6.0/redis_director/constants.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.5.3/redis_director/subscriber.py` & `redis_director-0.6.0/redis_director/subscriber.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.5.3/PKG-INFO` & `redis_director-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-director
-Version: 0.5.3
+Version: 0.6.0
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


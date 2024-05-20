# Comparing `tmp/redis_director-0.6.0.tar.gz` & `tmp/redis_director-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_director-0.6.0.tar", max compression
+gzip compressed data, was "redis_director-0.6.1.tar", max compression
```

## Comparing `redis_director-0.6.0.tar` & `redis_director-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2113 2024-05-16 08:23:46.385495 redis_director-0.6.0/README.md
--rw-r--r--   0        0        0      320 2024-05-20 00:58:50.092792 redis_director-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      266 2024-05-20 00:59:00.829045 redis_director-0.6.0/redis_director/__init__.py
--rw-r--r--   0        0        0      760 2024-05-20 00:58:27.508256 redis_director-0.6.0/redis_director/callback.py
--rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.6.0/redis_director/constants.py
--rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.6.0/redis_director/handler.py
--rw-r--r--   0        0        0     4154 2024-05-20 00:55:55.652461 redis_director-0.6.0/redis_director/publisher.py
--rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.6.0/redis_director/subscriber.py
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 redis_director-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2113 2024-05-16 08:23:46.385495 redis_director-0.6.1/README.md
+-rw-r--r--   0        0        0      320 2024-05-20 01:21:10.031688 redis_director-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      266 2024-05-20 00:59:00.829045 redis_director-0.6.1/redis_director/__init__.py
+-rw-r--r--   0        0        0      760 2024-05-20 00:58:27.508256 redis_director-0.6.1/redis_director/callback.py
+-rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.6.1/redis_director/constants.py
+-rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.6.1/redis_director/handler.py
+-rw-r--r--   0        0        0     4186 2024-05-20 01:06:02.504705 redis_director-0.6.1/redis_director/publisher.py
+-rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.6.1/redis_director/subscriber.py
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 redis_director-0.6.1/PKG-INFO
```

### Comparing `redis_director-0.6.0/README.md` & `redis_director-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `redis_director-0.6.0/redis_director/callback.py` & `redis_director-0.6.1/redis_director/callback.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.6.0/redis_director/constants.py` & `redis_director-0.6.1/redis_director/constants.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.6.0/redis_director/publisher.py` & `redis_director-0.6.1/redis_director/publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 from typing import Any, Callable, Dict, Iterable, List
 from fun_things.math import weighted_distribution
 from redis import Redis
 
-from redis_director.callback import (
-    generic_sadd_callback,
-    generic_spop_callback,
-)
-
 from .subscriber import Subscriber
 
 
 class Publisher:
     def __init__(
         self,
         redis: Redis,
@@ -35,14 +30,19 @@
 
         self.__redis = redis
         self.__score_key: str = score_key
         self.__queue_key: str = queue_key
         self.__add_payloads_callback = add_payloads_callback
         self.__pop_payloads_callback = pop_payloads_callback
 
+        from redis_director.callback import (
+            generic_sadd_callback,
+            generic_spop_callback,
+        )
+
         if add_payloads_callback == None:
             self.__add_payloads_callback = generic_sadd_callback
 
         if pop_payloads_callback == None:
             self.__pop_payloads_callback = generic_spop_callback
 
     @property
```

### Comparing `redis_director-0.6.0/redis_director/subscriber.py` & `redis_director-0.6.1/redis_director/subscriber.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.6.0/PKG-INFO` & `redis_director-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-director
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


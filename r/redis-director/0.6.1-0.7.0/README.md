# Comparing `tmp/redis_director-0.6.1.tar.gz` & `tmp/redis_director-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_director-0.6.1.tar", max compression
+gzip compressed data, was "redis_director-0.7.0.tar", max compression
```

## Comparing `redis_director-0.6.1.tar` & `redis_director-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2113 2024-05-16 08:23:46.385495 redis_director-0.6.1/README.md
--rw-r--r--   0        0        0      320 2024-05-20 01:21:10.031688 redis_director-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      266 2024-05-20 00:59:00.829045 redis_director-0.6.1/redis_director/__init__.py
--rw-r--r--   0        0        0      760 2024-05-20 00:58:27.508256 redis_director-0.6.1/redis_director/callback.py
--rw-r--r--   0        0        0      568 2024-05-16 07:42:23.997303 redis_director-0.6.1/redis_director/constants.py
--rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.6.1/redis_director/handler.py
--rw-r--r--   0        0        0     4186 2024-05-20 01:06:02.504705 redis_director-0.6.1/redis_director/publisher.py
--rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.6.1/redis_director/subscriber.py
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 redis_director-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2113 2024-05-16 08:23:46.385495 redis_director-0.7.0/README.md
+-rw-r--r--   0        0        0      320 2024-05-20 01:43:21.231551 redis_director-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      297 2024-05-20 01:40:49.544799 redis_director-0.7.0/redis_director/__init__.py
+-rw-r--r--   0        0        0     1037 2024-05-20 01:40:41.096614 redis_director-0.7.0/redis_director/callback.py
+-rw-r--r--   0        0        0      808 2024-05-20 01:34:28.055535 redis_director-0.7.0/redis_director/constants.py
+-rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.7.0/redis_director/handler.py
+-rw-r--r--   0        0        0     4178 2024-05-20 01:43:04.091290 redis_director-0.7.0/redis_director/publisher.py
+-rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.7.0/redis_director/subscriber.py
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 redis_director-0.7.0/PKG-INFO
```

### Comparing `redis_director-0.6.1/README.md` & `redis_director-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `redis_director-0.6.1/redis_director/callback.py` & `redis_director-0.7.0/redis_director/callback.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Iterable
 
+from redis_director.constants import SRANDPOP_LUA_SCRIPT
 from redis_director.publisher import Publisher
 
 
 def generic_sadd_callback(
     publisher: Publisher,
     payloads: Iterable[str],
 ):
@@ -37,7 +38,19 @@
     publisher: Publisher,
     batch_size: int,
 ):
     return publisher.redis.lpop(
         publisher.queue_key,
         batch_size,
     )
+
+
+def generic_srandpop_callback(
+    publisher: Publisher,
+    batch_size: int,
+):
+    publisher.redis.eval(
+        SRANDPOP_LUA_SCRIPT,
+        1,
+        publisher.queue_key,
+        batch_size,  # type: ignore
+    )
```

### Comparing `redis_director-0.6.1/redis_director/constants.py` & `redis_director-0.7.0/redis_director/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,7 +23,21 @@
 
 end
 
 redis.call('zadd', key, newScore, member)
 
 return newScore
 """
+
+# srandmember + spop
+SRANDPOP_LUA_SCRIPT = """
+local key = KEYS[1]
+local batchSize = ARGV[1]
+
+local items = redis.call('SRANDMEMBER', key, batchSize)
+
+for i, name in ipairs(items) do
+    redis.call('SREM', key, name)
+end
+
+return items
+"""
```

### Comparing `redis_director-0.6.1/redis_director/publisher.py` & `redis_director-0.7.0/redis_director/publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, Iterable, List
+from typing import Any, Callable, Dict, Iterable
 from fun_things.math import weighted_distribution
 from redis import Redis
 
 from .subscriber import Subscriber
 
 
 class Publisher:
@@ -10,44 +10,44 @@
         self,
         redis: Redis,
         score_key: str,
         queue_key: str,
         add_payloads_callback: Callable[
             [
                 "Publisher",
-                Iterable[str],
+                Iterable,
             ],
             None,
         ] = None,  # type: ignore
         pop_payloads_callback: Callable[
             [
                 "Publisher",
                 int,
             ],
-            List[str],
+            list,
         ] = None,  # type: ignore
     ):
         self.__subscribers: Dict[str, Subscriber] = {}
 
         self.__redis = redis
         self.__score_key: str = score_key
         self.__queue_key: str = queue_key
         self.__add_payloads_callback = add_payloads_callback
         self.__pop_payloads_callback = pop_payloads_callback
 
         from redis_director.callback import (
             generic_sadd_callback,
-            generic_spop_callback,
+            generic_srandpop_callback,
         )
 
         if add_payloads_callback == None:
             self.__add_payloads_callback = generic_sadd_callback
 
         if pop_payloads_callback == None:
-            self.__pop_payloads_callback = generic_spop_callback
+            self.__pop_payloads_callback = generic_srandpop_callback
 
     @property
     def redis(self):
         return self.__redis
 
     @property
     def score_key(self):
```

### Comparing `redis_director-0.6.1/redis_director/subscriber.py` & `redis_director-0.7.0/redis_director/subscriber.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.6.1/PKG-INFO` & `redis_director-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-director
-Version: 0.6.1
+Version: 0.7.0
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


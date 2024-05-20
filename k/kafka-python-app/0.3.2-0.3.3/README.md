# Comparing `tmp/kafka_python_app-0.3.2.tar.gz` & `tmp/kafka_python_app-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_python_app-0.3.2.tar", last modified: Wed Jan 10 01:04:04 2024, max compression
+gzip compressed data, was "kafka_python_app-0.3.3.tar", last modified: Mon May 20 20:31:16 2024, max compression
```

## Comparing `kafka_python_app-0.3.2.tar` & `kafka_python_app-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2024-01-10 01:04:04.095795 kafka_python_app-0.3.2/
--rw-rw-r--   0 doc       (1000) doc       (1000)     1070 2022-04-11 01:45:36.000000 kafka_python_app-0.3.2/LICENSE.md
--rw-r--r--   0 doc       (1000) doc       (1000)    13890 2024-01-10 01:04:04.095795 kafka_python_app-0.3.2/PKG-INFO
--rw-rw-r--   0 doc       (1000) doc       (1000)    13370 2024-01-06 23:18:15.000000 kafka_python_app-0.3.2/README.md
-drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2024-01-10 01:04:04.091795 kafka_python_app-0.3.2/kafka_python_app/
--rw-rw-r--   0 doc       (1000) doc       (1000)      723 2022-04-11 01:26:35.000000 kafka_python_app-0.3.2/kafka_python_app/__init__.py
--rw-rw-r--   0 doc       (1000) doc       (1000)    25899 2024-01-10 00:08:23.000000 kafka_python_app-0.3.2/kafka_python_app/app.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     4681 2024-01-10 01:00:13.000000 kafka_python_app-0.3.2/kafka_python_app/connector.py
-drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2024-01-10 01:04:04.095795 kafka_python_app-0.3.2/kafka_python_app.egg-info/
--rw-r--r--   0 doc       (1000) doc       (1000)    13890 2024-01-10 01:04:04.000000 kafka_python_app-0.3.2/kafka_python_app.egg-info/PKG-INFO
--rw-rw-r--   0 doc       (1000) doc       (1000)      716 2024-01-10 01:04:04.000000 kafka_python_app-0.3.2/kafka_python_app.egg-info/SOURCES.txt
--rw-rw-r--   0 doc       (1000) doc       (1000)        1 2024-01-10 01:04:04.000000 kafka_python_app-0.3.2/kafka_python_app.egg-info/dependency_links.txt
--rw-rw-r--   0 doc       (1000) doc       (1000)       55 2024-01-10 01:04:04.000000 kafka_python_app-0.3.2/kafka_python_app.egg-info/requires.txt
--rw-rw-r--   0 doc       (1000) doc       (1000)       17 2024-01-10 01:04:04.000000 kafka_python_app-0.3.2/kafka_python_app.egg-info/top_level.txt
--rw-rw-r--   0 doc       (1000) doc       (1000)       38 2024-01-10 01:04:04.095795 kafka_python_app-0.3.2/setup.cfg
--rw-rw-r--   0 doc       (1000) doc       (1000)      846 2024-01-10 00:08:23.000000 kafka_python_app-0.3.2/setup.py
-drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2024-01-10 01:04:04.095795 kafka_python_app-0.3.2/tests/
--rw-rw-r--   0 doc       (1000) doc       (1000)     4432 2024-01-10 00:35:13.000000 kafka_python_app-0.3.2/tests/test_kafka_app.py
--rw-rw-r--   0 doc       (1000) doc       (1000)    14301 2024-01-10 00:37:33.000000 kafka_python_app-0.3.2/tests/test_kafka_app_emit_with_response.py
--rw-rw-r--   0 doc       (1000) doc       (1000)    15028 2024-01-10 00:39:34.000000 kafka_python_app-0.3.2/tests/test_kafka_app_emit_with_response_custom_pipe.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     4495 2024-01-10 00:44:54.000000 kafka_python_app-0.3.2/tests/test_kafka_app_event_topic_filter.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     4359 2023-03-11 01:51:45.000000 kafka_python_app-0.3.2/tests/test_kafka_app_msg_key_as_event.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     6936 2024-01-10 00:44:54.000000 kafka_python_app-0.3.2/tests/test_kafka_app_pipelines.py
--rw-rw-r--   0 doc       (1000) doc       (1000)    16847 2024-01-10 00:44:54.000000 kafka_python_app-0.3.2/tests/test_kafka_app_pipelines_pipe_events.py
--rw-rw-r--   0 doc       (1000) doc       (1000)    20197 2024-01-10 00:46:49.000000 kafka_python_app-0.3.2/tests/test_kafka_app_pipelines_pipe_events_custom_pipe.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     4431 2024-01-10 00:47:46.000000 kafka_python_app-0.3.2/tests/test_kafka_app_raw_msg.py
--rw-rw-r--   0 doc       (1000) doc       (1000)     3124 2024-01-10 01:00:13.000000 kafka_python_app-0.3.2/tests/test_kafka_listener.py
+drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2024-05-20 20:31:16.678861 kafka_python_app-0.3.3/
+-rw-rw-r--   0 doc       (1000) doc       (1000)     1070 2022-04-11 01:45:36.000000 kafka_python_app-0.3.3/LICENSE.md
+-rw-r--r--   0 doc       (1000) doc       (1000)    13890 2024-05-20 20:31:16.678861 kafka_python_app-0.3.3/PKG-INFO
+-rw-rw-r--   0 doc       (1000) doc       (1000)    13370 2024-01-06 23:18:15.000000 kafka_python_app-0.3.3/README.md
+drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2024-05-20 20:31:16.674861 kafka_python_app-0.3.3/kafka_python_app/
+-rw-rw-r--   0 doc       (1000) doc       (1000)      723 2022-04-11 01:26:35.000000 kafka_python_app-0.3.3/kafka_python_app/__init__.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)    25834 2024-05-20 02:25:58.000000 kafka_python_app-0.3.3/kafka_python_app/app.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4681 2024-01-10 01:00:13.000000 kafka_python_app-0.3.3/kafka_python_app/connector.py
+drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2024-05-20 20:31:16.678861 kafka_python_app-0.3.3/kafka_python_app.egg-info/
+-rw-r--r--   0 doc       (1000) doc       (1000)    13890 2024-05-20 20:31:16.000000 kafka_python_app-0.3.3/kafka_python_app.egg-info/PKG-INFO
+-rw-rw-r--   0 doc       (1000) doc       (1000)      777 2024-05-20 20:31:16.000000 kafka_python_app-0.3.3/kafka_python_app.egg-info/SOURCES.txt
+-rw-rw-r--   0 doc       (1000) doc       (1000)        1 2024-05-20 20:31:16.000000 kafka_python_app-0.3.3/kafka_python_app.egg-info/dependency_links.txt
+-rw-rw-r--   0 doc       (1000) doc       (1000)       55 2024-05-20 20:31:16.000000 kafka_python_app-0.3.3/kafka_python_app.egg-info/requires.txt
+-rw-rw-r--   0 doc       (1000) doc       (1000)       17 2024-05-20 20:31:16.000000 kafka_python_app-0.3.3/kafka_python_app.egg-info/top_level.txt
+-rw-rw-r--   0 doc       (1000) doc       (1000)       38 2024-05-20 20:31:16.678861 kafka_python_app-0.3.3/setup.cfg
+-rw-rw-r--   0 doc       (1000) doc       (1000)      846 2024-05-20 20:20:43.000000 kafka_python_app-0.3.3/setup.py
+drwxrwxr-x   0 doc       (1000) doc       (1000)        0 2024-05-20 20:31:16.678861 kafka_python_app-0.3.3/tests/
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4432 2024-01-10 00:35:13.000000 kafka_python_app-0.3.3/tests/test_kafka_app.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)    14301 2024-05-19 23:41:20.000000 kafka_python_app-0.3.3/tests/test_kafka_app_emit_with_response.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     5253 2024-05-20 20:16:32.000000 kafka_python_app-0.3.3/tests/test_kafka_app_emit_with_response_bulk_multireplica.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)    15028 2024-01-10 00:39:34.000000 kafka_python_app-0.3.3/tests/test_kafka_app_emit_with_response_custom_pipe.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4495 2024-01-10 00:44:54.000000 kafka_python_app-0.3.3/tests/test_kafka_app_event_topic_filter.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4359 2023-03-11 01:51:45.000000 kafka_python_app-0.3.3/tests/test_kafka_app_msg_key_as_event.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     6936 2024-01-10 00:44:54.000000 kafka_python_app-0.3.3/tests/test_kafka_app_pipelines.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)    16847 2024-01-10 00:44:54.000000 kafka_python_app-0.3.3/tests/test_kafka_app_pipelines_pipe_events.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)    20197 2024-01-10 00:46:49.000000 kafka_python_app-0.3.3/tests/test_kafka_app_pipelines_pipe_events_custom_pipe.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     4431 2024-01-10 00:47:46.000000 kafka_python_app-0.3.3/tests/test_kafka_app_raw_msg.py
+-rw-rw-r--   0 doc       (1000) doc       (1000)     3124 2024-01-10 01:00:13.000000 kafka_python_app-0.3.3/tests/test_kafka_listener.py
```

### Comparing `kafka_python_app-0.3.2/LICENSE.md` & `kafka_python_app-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/PKG-INFO` & `kafka_python_app-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka_python_app
-Version: 0.3.2
+Version: 0.3.3
 Summary: kafka application endpoint
 Home-page: https://github.com/doctor3030/kafka-python-app.git
 Author: Dmitry Amanov
 Author-email: dmitry.amanov@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kafka_python_app-0.3.2/README.md` & `kafka_python_app-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/kafka_python_app/__init__.py` & `kafka_python_app-0.3.3/kafka_python_app/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/kafka_python_app/app.py` & `kafka_python_app-0.3.3/kafka_python_app/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import hashlib
 import time
 import asyncio
 from collections import deque
 from kafka_python_app.connector import ListenerConfig, KafkaConnector, ConsumerRecord, ProducerRecord
 
 
-def _get_event_id_hash(event_id: str, service_id: str):
-    _id = '.'.join([service_id, event_id])
-    return hashlib.sha256(_id.encode('utf-8')).hexdigest()
+def _get_event_id_hash(event_id: str):
+    # _id = '.'.join([service_id, event_id])
+    return hashlib.sha256(event_id.encode('utf-8')).hexdigest()
 
 
 class TransactionPipeWithReturnOptions(pydantic.BaseModel):
     response_event_name: str
     response_from_topic: str
     cache_client: Any
     return_event_timeout: int
@@ -223,15 +223,15 @@
         )
 
         if not event_id:
             raise RuntimeError('Pipe event failed')
 
         time_up = time.time()
         while True:
-            response = cache_client.get(_get_event_id_hash(event_id, app_id))
+            response = cache_client.get(_get_event_id_hash(event_id))
             if response is not None:
                 response_msg = json.loads(response.decode('utf-8'))
                 logger.info(
                     f'--------> PIPE RESPONSE RECEIVED (message pipeline {pipeline_name}): '
                     f'name: {options.with_response_options.response_event_name}; '
                     f'event_id: {event_id}')
                 return response_msg
@@ -474,15 +474,15 @@
             headers = dict((x, y.decode('utf-8')) for x, y in kwargs.get('headers'))
 
             if logger:
                 logger.info(
                     f'--------> CACHING PIPE RESPONSE: name: {event_name}; event_id: {headers["event_id"]}')
 
             cache_client.set(
-                name=_get_event_id_hash(headers['event_id'], self.app_id),
+                name=_get_event_id_hash(headers['event_id']),
                 value=json.dumps(message).encode('utf-8'),
                 ex=30
             )
             return message
         except Exception as e:
             err_msg = f'_cache_pipe_response => Exception: type: {sys.exc_info()[0]}; ' \
                       f'line#: {sys.exc_info()[2].tb_lineno}; ' \
@@ -546,16 +546,15 @@
                 f'to: {topic}; '
                 f'event_id: {event_id}')
 
             self.emit(topic, message)
 
             time_up = time.time()
             while True:
-                response = self.config.emit_with_response_options.cache_client.get(
-                    _get_event_id_hash(event_id, self.app_id))
+                response = self.config.emit_with_response_options.cache_client.get(_get_event_id_hash(event_id))
                 if response is not None:
                     return json.loads(response.decode('utf-8')), None
                 else:
                     if time.time() - time_up < self.config.emit_with_response_options.return_event_timeout:
                         await asyncio.sleep(0.001)
                     else:
                         raise TimeoutError(f'Emit event with response timeout: '
```

### Comparing `kafka_python_app-0.3.2/kafka_python_app/connector.py` & `kafka_python_app-0.3.3/kafka_python_app/connector.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/kafka_python_app.egg-info/PKG-INFO` & `kafka_python_app-0.3.3/kafka_python_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka_python_app
-Version: 0.3.2
+Version: 0.3.3
 Summary: kafka application endpoint
 Home-page: https://github.com/doctor3030/kafka-python-app.git
 Author: Dmitry Amanov
 Author-email: dmitry.amanov@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kafka_python_app-0.3.2/kafka_python_app.egg-info/SOURCES.txt` & `kafka_python_app-0.3.3/kafka_python_app.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 kafka_python_app.egg-info/PKG-INFO
 kafka_python_app.egg-info/SOURCES.txt
 kafka_python_app.egg-info/dependency_links.txt
 kafka_python_app.egg-info/requires.txt
 kafka_python_app.egg-info/top_level.txt
 tests/test_kafka_app.py
 tests/test_kafka_app_emit_with_response.py
+tests/test_kafka_app_emit_with_response_bulk_multireplica.py
 tests/test_kafka_app_emit_with_response_custom_pipe.py
 tests/test_kafka_app_event_topic_filter.py
 tests/test_kafka_app_msg_key_as_event.py
 tests/test_kafka_app_pipelines.py
 tests/test_kafka_app_pipelines_pipe_events.py
 tests/test_kafka_app_pipelines_pipe_events_custom_pipe.py
 tests/test_kafka_app_raw_msg.py
```

### Comparing `kafka_python_app-0.3.2/setup.py` & `kafka_python_app-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ROOOT = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (ROOOT / "README.md").read_text()
 
 setup(
     name='kafka_python_app',
-    version="0.3.2",
+    version="0.3.3",
     author="Dmitry Amanov",
     author_email="dmitry.amanov@gmail.com",
     description="kafka application endpoint",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/doctor3030/kafka-python-app.git",
     license="MIT",
```

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app.py` & `kafka_python_app-0.3.3/tests/test_kafka_app.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app_emit_with_response.py` & `kafka_python_app-0.3.3/tests/test_kafka_app_emit_with_response.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app_emit_with_response_custom_pipe.py` & `kafka_python_app-0.3.3/tests/test_kafka_app_emit_with_response_custom_pipe.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app_event_topic_filter.py` & `kafka_python_app-0.3.3/tests/test_kafka_app_event_topic_filter.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app_msg_key_as_event.py` & `kafka_python_app-0.3.3/tests/test_kafka_app_msg_key_as_event.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app_pipelines.py` & `kafka_python_app-0.3.3/tests/test_kafka_app_pipelines.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app_pipelines_pipe_events.py` & `kafka_python_app-0.3.3/tests/test_kafka_app_pipelines_pipe_events.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app_pipelines_pipe_events_custom_pipe.py` & `kafka_python_app-0.3.3/tests/test_kafka_app_pipelines_pipe_events_custom_pipe.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_app_raw_msg.py` & `kafka_python_app-0.3.3/tests/test_kafka_app_raw_msg.py`

 * *Files identical despite different names*

### Comparing `kafka_python_app-0.3.2/tests/test_kafka_listener.py` & `kafka_python_app-0.3.3/tests/test_kafka_listener.py`

 * *Files identical despite different names*


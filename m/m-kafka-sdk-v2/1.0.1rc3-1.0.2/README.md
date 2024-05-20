# Comparing `tmp/m-kafka-sdk-v2-1.0.1rc3.tar.gz` & `tmp/m_kafka_sdk_v2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-kafka-sdk-v2-1.0.1rc3.tar", last modified: Wed Mar 20 03:33:15 2024, max compression
+gzip compressed data, was "m_kafka_sdk_v2-1.0.2.tar", last modified: Mon May 20 11:23:35 2024, max compression
```

## Comparing `m-kafka-sdk-v2-1.0.1rc3.tar` & `m_kafka_sdk_v2-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.241295 m-kafka-sdk-v2-1.0.1rc3/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-03-20 03:33:15.240295 m-kafka-sdk-v2-1.0.1rc3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     5881 2024-03-20 03:04:15.000000 m-kafka-sdk-v2-1.0.1rc3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.238295 m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-03-20 03:33:15.000000 m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      871 2024-03-20 03:33:15.000000 m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 03:33:15.000000 m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-20 03:33:15.000000 m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       75 2024-03-20 03:33:15.000000 m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-20 03:33:15.000000 m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.214294 m-kafka-sdk-v2-1.0.1rc3/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.227295 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.228294 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/
--rw-r--r--   0 root         (0) root         (0)     1594 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.232295 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/
--rw-r--r--   0 root         (0) root         (0)     1326 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8847 2024-03-20 03:04:15.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/batch_consumer_manager.py
--rwxr-xr-x   0 root         (0) root         (0)     8054 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/ensure_kafka_topic.py
--rw-r--r--   0 root         (0) root         (0)    11806 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/kafka_consumer_manager.py
--rw-r--r--   0 root         (0) root         (0)     1736 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/kafka_producer_manager.py
--rw-r--r--   0 root         (0) root         (0)     3074 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/redisbloom_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.233295 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.236295 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/models/mongo/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/models/mongo/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6321 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/models/mongo/base_model.py
--rw-r--r--   0 root         (0) root         (0)      447 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/models/mongo/requeue_consumer_model.py
--rw-r--r--   0 root         (0) root         (0)      103 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 03:33:15.242295 m-kafka-sdk-v2-1.0.1rc3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9294 2024-03-20 03:33:14.000000 m-kafka-sdk-v2-1.0.1rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 03:33:15.238295 m-kafka-sdk-v2-1.0.1rc3/test/
--rw-r--r--   0 root         (0) root         (0)      655 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/test/test_consumer.py
--rw-r--r--   0 root         (0) root         (0)      829 2024-02-15 03:33:30.000000 m-kafka-sdk-v2-1.0.1rc3/test/test_singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.936139 m_kafka_sdk_v2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     6911 2024-05-20 11:23:35.935140 m_kafka_sdk_v2-1.0.2/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     5956 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.934139 m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6911 2024-05-20 11:23:35.000000 m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      871 2024-05-20 11:23:35.000000 m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 11:23:35.000000 m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-20 11:23:35.000000 m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-20 11:23:35.000000 m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-20 11:23:35.000000 m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.898139 m_kafka_sdk_v2-1.0.2/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.923139 m_kafka_sdk_v2-1.0.2/mobio/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.923139 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/
+-rw-r--r--   0 root         (0) root         (0)     1594 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.928139 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/
+-rw-r--r--   0 root         (0) root         (0)     1326 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8847 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/batch_consumer_manager.py
+-rwxr-xr-x   0 root         (0) root         (0)     8054 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/ensure_kafka_topic.py
+-rw-r--r--   0 root         (0) root         (0)    11806 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/kafka_consumer_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/kafka_producer_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/redisbloom_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.929139 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.931139 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/models/mongo/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/models/mongo/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6321 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/models/mongo/base_model.py
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/models/mongo/requeue_consumer_model.py
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 11:23:35.936139 m_kafka_sdk_v2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9286 2024-05-20 11:23:35.000000 m_kafka_sdk_v2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 11:23:35.933139 m_kafka_sdk_v2-1.0.2/test/
+-rw-r--r--   0 root         (0) root         (0)      655 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/test/test_consumer.py
+-rw-r--r--   0 root         (0) root         (0)      829 2024-05-20 11:07:05.000000 m_kafka_sdk_v2-1.0.2/test/test_singleton.py
```

### Comparing `m-kafka-sdk-v2-1.0.1rc3/PKG-INFO` & `m_kafka_sdk_v2-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-kafka-sdk-v2
-Version: 1.0.1rc3
+Version: 1.0.2
 Summary: Mobio Kafka SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,kafka,m-kafka
@@ -121,14 +121,17 @@
     client_mongo = MongoClient(url_connection, connect=False)
 
     TestConsumer(topic_name="test", group_id="test", client_mongo=client_mongo, retryable=True, lst_subscribe_topic=['test', 'test1'], retry_topic='test1', enable_bloom=True, auto_commit=True)
 ```
 
 # change logs
 
+* 1.0.2 (2024-05-20)
+  * Build 1.0.1-rc3 thành 1.0.2, không sửa logic
+
 * 1.0.1-rc3 (2024-03-20)
   * Batch consume message
     * Bỏ log "no offset to commit"
     * Sử dụng redisbloom<=0.4.0 do redisbloom==0.4.1 bắt buộc redis==3.5.3
 
 * 1.0.1-rc2 (2024-03-01)
   * Batch consume message
```

### Comparing `m-kafka-sdk-v2-1.0.1rc3/README.md` & `m_kafka_sdk_v2-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,17 @@
     client_mongo = MongoClient(url_connection, connect=False)
 
     TestConsumer(topic_name="test", group_id="test", client_mongo=client_mongo, retryable=True, lst_subscribe_topic=['test', 'test1'], retry_topic='test1', enable_bloom=True, auto_commit=True)
 ```
 
 # change logs
 
+* 1.0.2 (2024-05-20)
+  * Build 1.0.1-rc3 thành 1.0.2, không sửa logic
+
 * 1.0.1-rc3 (2024-03-20)
   * Batch consume message
     * Bỏ log "no offset to commit"
     * Sử dụng redisbloom<=0.4.0 do redisbloom==0.4.1 bắt buộc redis==3.5.3
 
 * 1.0.1-rc2 (2024-03-01)
   * Batch consume message
```

### Comparing `m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/PKG-INFO` & `m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-kafka-sdk-v2
-Version: 1.0.1rc3
+Version: 1.0.2
 Summary: Mobio Kafka SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,kafka,m-kafka
@@ -121,14 +121,17 @@
     client_mongo = MongoClient(url_connection, connect=False)
 
     TestConsumer(topic_name="test", group_id="test", client_mongo=client_mongo, retryable=True, lst_subscribe_topic=['test', 'test1'], retry_topic='test1', enable_bloom=True, auto_commit=True)
 ```
 
 # change logs
 
+* 1.0.2 (2024-05-20)
+  * Build 1.0.1-rc3 thành 1.0.2, không sửa logic
+
 * 1.0.1-rc3 (2024-03-20)
   * Batch consume message
     * Bỏ log "no offset to commit"
     * Sử dụng redisbloom<=0.4.0 do redisbloom==0.4.1 bắt buộc redis==3.5.3
 
 * 1.0.1-rc2 (2024-03-01)
   * Batch consume message
```

### Comparing `m-kafka-sdk-v2-1.0.1rc3/m_kafka_sdk_v2.egg-info/SOURCES.txt` & `m_kafka_sdk_v2-1.0.2/m_kafka_sdk_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/__init__.py` & `m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/__init__.py` & `m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/batch_consumer_manager.py` & `m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/batch_consumer_manager.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/ensure_kafka_topic.py` & `m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/ensure_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/kafka_consumer_manager.py` & `m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/kafka_consumer_manager.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/kafka_producer_manager.py` & `m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/kafka_producer_manager.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/helpers/redisbloom_client.py` & `m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/helpers/redisbloom_client.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/mobio/libs/kafka_lib/models/mongo/base_model.py` & `m_kafka_sdk_v2-1.0.2/mobio/libs/kafka_lib/models/mongo/base_model.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/setup.py` & `m_kafka_sdk_v2-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         :return:
         """
         requirements = ["requests>=2.25.1", "confluent-kafka>=1.7.0", "redisbloom<=0.4.0", "m-singleton>=0.3"]
         return requirements
 
 
 version_dev='0.1.5'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
-version_prod='1.0.1-rc3'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_prod='1.0.2'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode = ''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -48,15 +48,15 @@
     name="m-kafka-sdk-v2" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1-rc3',  # Required, Phần này cũng không được format file.
+    version='1.0.2',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Kafka SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `m-kafka-sdk-v2-1.0.1rc3/test/test_consumer.py` & `m_kafka_sdk_v2-1.0.2/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-1.0.1rc3/test/test_singleton.py` & `m_kafka_sdk_v2-1.0.2/test/test_singleton.py`

 * *Files identical despite different names*


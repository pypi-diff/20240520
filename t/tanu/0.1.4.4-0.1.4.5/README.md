# Comparing `tmp/tanu-0.1.4.4.tar.gz` & `tmp/tanu-0.1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tanu-0.1.4.4.tar", last modified: Wed May 15 08:48:44 2024, max compression
+gzip compressed data, was "tanu-0.1.4.5.tar", last modified: Mon May 20 10:11:57 2024, max compression
```

## Comparing `tanu-0.1.4.4.tar` & `tanu-0.1.4.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 08:48:44.970086 tanu-0.1.4.4/
--rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.4.4/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.4.4/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-15 08:48:44.970018 tanu-0.1.4.4/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.4.4/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.4.4/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      720 2024-05-15 08:48:44.970325 tanu-0.1.4.4/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.4.4/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 08:48:44.967658 tanu-0.1.4.4/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 08:48:44.968754 tanu-0.1.4.4/src/tanu/
--rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.4.4/src/tanu/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    18523 2024-05-15 08:48:13.000000 tanu-0.1.4.4/src/tanu/tanu.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 08:48:44.969629 tanu-0.1.4.4/src/tanu/utils/
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.4.4/src/tanu/utils/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.4.4/src/tanu/utils/object_encoder_decoder.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 08:48:44.969794 tanu-0.1.4.4/src/tanu.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-15 08:48:44.000000 tanu-0.1.4.4/src/tanu.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-15 08:48:44.000000 tanu-0.1.4.4/src/tanu.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-15 08:48:44.000000 tanu-0.1.4.4/src/tanu.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       47 2024-05-15 08:48:44.000000 tanu-0.1.4.4/src/tanu.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-15 08:48:44.000000 tanu-0.1.4.4/src/tanu.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-20 10:11:57.724592 tanu-0.1.4.5/
+-rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.4.5/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.4.5/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-20 10:11:57.724530 tanu-0.1.4.5/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.4.5/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.4.5/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      720 2024-05-20 10:11:57.724837 tanu-0.1.4.5/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.4.5/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-20 10:11:57.721605 tanu-0.1.4.5/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-20 10:11:57.723219 tanu-0.1.4.5/src/tanu/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.4.5/src/tanu/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    18603 2024-05-20 10:11:43.000000 tanu-0.1.4.5/src/tanu/tanu.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-20 10:11:57.724039 tanu-0.1.4.5/src/tanu/utils/
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.4.5/src/tanu/utils/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.4.5/src/tanu/utils/object_encoder_decoder.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-20 10:11:57.724317 tanu-0.1.4.5/src/tanu.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-20 10:11:57.000000 tanu-0.1.4.5/src/tanu.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-20 10:11:57.000000 tanu-0.1.4.5/src/tanu.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-20 10:11:57.000000 tanu-0.1.4.5/src/tanu.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       47 2024-05-20 10:11:57.000000 tanu-0.1.4.5/src/tanu.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-20 10:11:57.000000 tanu-0.1.4.5/src/tanu.egg-info/top_level.txt
```

### Comparing `tanu-0.1.4.4/LICENSE.txt` & `tanu-0.1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tanu-0.1.4.4/PKG-INFO` & `tanu-0.1.4.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tanu-0.1.4.4/setup.cfg` & `tanu-0.1.4.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tanu
-version = 0.1.4.4
+version = 0.1.4.5
 author = chocolate-icecream
 description = Message passing between Python programs via RabbitMQ.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `tanu-0.1.4.4/src/tanu/tanu.py` & `tanu-0.1.4.5/src/tanu/tanu.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         """Continuously consume results from the result queue."""
         connection = pika.BlockingConnection(pika.ConnectionParameters(host=self.host, port=self.port))
         channel = connection.channel()
         channel.queue_declare(queue=self.result_queue_name)
         channel.basic_consume(queue=self.result_queue_name, auto_ack=True, on_message_callback=self.on_result_received)
         try:
             channel.start_consuming()
-        except pika.exceptions.StreamLostError:
+        except (pika.exceptions.StreamLostError, pika.exceptions.AMQPHeartbeatTimeout):
             logger.warning(f"Stream Loss Error while consuming queue '{self.result_queue_name}'")
             t = threading.Thread(target=self.start_consumer)
             t.daemon = True
             t.start()
 
 
     def on_result_received(self, ch, method, properties, body):
@@ -344,15 +344,15 @@
             channel.basic_qos(prefetch_count=1)
             channel.basic_consume(queue=queue_name, on_message_callback=self._call_command)
             logger.info(f"{self.name} starts running...")
             try:
                 channel.start_consuming()
             except KeyboardInterrupt:
                 break
-            except pika.exceptions.StreamLostError:
+            except (pika.exceptions.StreamLostError, pika.exceptions.AMQPHeartbeatTimeout):
                 logger.warning(f"Stream Lost Error while consuming queue {queue_name}")
                 pass
             
 
     def _call_command(self, ch_req, method, properties, body):
         """Process incoming command requests."""
         try:
```

### Comparing `tanu-0.1.4.4/src/tanu/utils/object_encoder_decoder.py` & `tanu-0.1.4.5/src/tanu/utils/object_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `tanu-0.1.4.4/src/tanu.egg-info/PKG-INFO` & `tanu-0.1.4.5/src/tanu.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```


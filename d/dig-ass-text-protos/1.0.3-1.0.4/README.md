# Comparing `tmp/dig_ass_text_protos-1.0.3.tar.gz` & `tmp/dig_ass_text_protos-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_text_protos-1.0.3.tar", last modified: Tue May 14 10:02:43 2024, max compression
+gzip compressed data, was "dig_ass_text_protos-1.0.4.tar", last modified: Mon May 20 11:51:59 2024, max compression
```

## Comparing `dig_ass_text_protos-1.0.3.tar` & `dig_ass_text_protos-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:43.846191 dig_ass_text_protos-1.0.3/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.3/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      371 2024-05-14 10:02:43.846191 dig_ass_text_protos-1.0.3/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-1.0.3/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:43.846191 dig_ass_text_protos-1.0.3/dig_ass_text_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2764 2024-05-14 10:02:42.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos/DigitalAssistantText_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2470 2024-05-14 10:02:42.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-05-14 10:02:42.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-14 10:01:31.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1551 2024-05-13 14:05:20.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:43.846191 dig_ass_text_protos-1.0.3/dig_ass_text_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      371 2024-05-14 10:02:43.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-05-14 10:02:43.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-14 10:02:43.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-14 10:02:43.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-14 10:02:43.000000 dig_ass_text_protos-1.0.3/dig_ass_text_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-14 10:00:02.000000 dig_ass_text_protos-1.0.3/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-14 10:02:43.846191 dig_ass_text_protos-1.0.3/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.3/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:59.371254 dig_ass_text_protos-1.0.4/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.4/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      371 2024-05-20 11:51:59.371254 dig_ass_text_protos-1.0.4/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-1.0.4/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:59.371254 dig_ass_text_protos-1.0.4/dig_ass_text_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2764 2024-05-20 11:51:57.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos/DigitalAssistantText_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2470 2024-05-20 11:51:57.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-05-20 11:51:57.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-20 11:50:51.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1551 2024-05-13 14:05:20.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:59.371254 dig_ass_text_protos-1.0.4/dig_ass_text_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      371 2024-05-20 11:51:59.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-05-20 11:51:59.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-20 11:51:59.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-20 11:51:59.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-20 11:51:59.000000 dig_ass_text_protos-1.0.4/dig_ass_text_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-20 11:47:49.000000 dig_ass_text_protos-1.0.4/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-20 11:51:59.371254 dig_ass_text_protos-1.0.4/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.4/setup.py
```

### Comparing `dig_ass_text_protos-1.0.3/dig_ass_text_protos/DigitalAssistantText_pb2.py` & `dig_ass_text_protos-1.0.4/dig_ass_text_protos/DigitalAssistantText_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.3/dig_ass_text_protos/DigitalAssistantText_pb2.pyi` & `dig_ass_text_protos-1.0.4/dig_ass_text_protos/DigitalAssistantText_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.3/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py` & `dig_ass_text_protos-1.0.4/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.3/dig_ass_text_protos/client.py` & `dig_ass_text_protos-1.0.4/dig_ass_text_protos/client.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.3/dig_ass_text_protos.egg-info/SOURCES.txt` & `dig_ass_text_protos-1.0.4/dig_ass_text_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.3/setup.py` & `dig_ass_text_protos-1.0.4/setup.py`

 * *Files identical despite different names*


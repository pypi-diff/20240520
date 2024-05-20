# Comparing `tmp/dig_ass_ep_protos-1.0.2.tar.gz` & `tmp/dig_ass_ep_protos-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ep_protos-1.0.2.tar", last modified: Tue May 14 10:02:11 2024, max compression
+gzip compressed data, was "dig_ass_ep_protos-1.0.3.tar", last modified: Mon May 20 11:51:43 2024, max compression
```

## Comparing `dig_ass_ep_protos-1.0.2.tar` & `dig_ass_ep_protos-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:11.253859 dig_ass_ep_protos-1.0.2/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-1.0.2/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      367 2024-05-14 10:02:11.253859 dig_ass_ep_protos-1.0.2/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-1.0.2/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:11.253859 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2205 2024-05-14 10:02:09.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1559 2024-05-14 10:02:09.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-05-14 10:02:09.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-14 10:01:31.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1153 2024-05-13 14:05:24.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:11.253859 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      367 2024-05-14 10:02:11.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-05-14 10:02:11.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-14 10:02:11.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-14 10:02:11.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-05-14 10:02:11.000000 dig_ass_ep_protos-1.0.2/dig_ass_ep_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-14 10:00:02.000000 dig_ass_ep_protos-1.0.2/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-14 10:02:11.253859 dig_ass_ep_protos-1.0.2/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.2/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:43.714928 dig_ass_ep_protos-1.0.3/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-1.0.3/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      367 2024-05-20 11:51:43.714928 dig_ass_ep_protos-1.0.3/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-1.0.3/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:43.714928 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2205 2024-05-20 11:51:42.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1559 2024-05-20 11:51:42.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-05-20 11:51:42.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-20 11:50:51.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1153 2024-05-13 14:05:24.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:43.714928 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      367 2024-05-20 11:51:43.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-05-20 11:51:43.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-20 11:51:43.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-20 11:51:43.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-05-20 11:51:43.000000 dig_ass_ep_protos-1.0.3/dig_ass_ep_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-20 11:47:49.000000 dig_ass_ep_protos-1.0.3/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-20 11:51:43.714928 dig_ass_ep_protos-1.0.3/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.3/setup.py
```

### Comparing `dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py` & `dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi` & `dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py` & `dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-1.0.2/dig_ass_ep_protos/client.py` & `dig_ass_ep_protos-1.0.3/dig_ass_ep_protos/client.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-1.0.2/setup.py` & `dig_ass_ep_protos-1.0.3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/dig_ass_ocr_protos-0.0.7.tar.gz` & `tmp/dig_ass_ocr_protos-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ocr_protos-0.0.7.tar", last modified: Tue May 14 10:02:22 2024, max compression
+gzip compressed data, was "dig_ass_ocr_protos-0.0.8.tar", last modified: Mon May 20 11:51:51 2024, max compression
```

## Comparing `dig_ass_ocr_protos-0.0.7.tar` & `dig_ass_ocr_protos-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:22.601974 dig_ass_ocr_protos-0.0.7/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.7/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      369 2024-05-14 10:02:22.601974 dig_ass_ocr_protos-0.0.7/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.7/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:22.597974 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1686 2024-05-14 10:02:21.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-05-14 10:02:21.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2914 2024-05-14 10:02:21.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-14 10:01:31.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      676 2024-05-13 14:05:52.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-14 10:02:22.601974 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      369 2024-05-14 10:02:22.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-05-14 10:02:22.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-14 10:02:22.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-14 10:02:22.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-14 10:02:22.000000 dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-14 10:00:02.000000 dig_ass_ocr_protos-0.0.7/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-14 10:02:22.601974 dig_ass_ocr_protos-0.0.7/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.7/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:51.359087 dig_ass_ocr_protos-0.0.8/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.8/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      369 2024-05-20 11:51:51.359087 dig_ass_ocr_protos-0.0.8/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.8/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:51.359087 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1686 2024-05-20 11:51:49.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-05-20 11:51:49.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2914 2024-05-20 11:51:49.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-20 11:50:51.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      676 2024-05-13 14:05:52.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-20 11:51:51.359087 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      369 2024-05-20 11:51:51.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-05-20 11:51:51.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-20 11:51:51.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-20 11:51:51.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-20 11:51:51.000000 dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-20 11:47:49.000000 dig_ass_ocr_protos-0.0.8/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-20 11:51:51.359087 dig_ass_ocr_protos-0.0.8/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-05-02 11:09:19.000000 dig_ass_ocr_protos-0.0.8/setup.py
```

### Comparing `dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py` & `dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi` & `dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py` & `dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.7/dig_ass_ocr_protos/client.py` & `dig_ass_ocr_protos-0.0.8/dig_ass_ocr_protos/client.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.7/setup.py` & `dig_ass_ocr_protos-0.0.8/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/nightingalejsonadapter-3.1.0.tar.gz` & `tmp/nightingalejsonadapter-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nightingalejsonadapter-3.1.0.tar", last modified: Mon May 20 19:18:51 2024, max compression
+gzip compressed data, was "nightingalejsonadapter-3.2.0.tar", last modified: Mon May 20 20:17:43 2024, max compression
```

## Comparing `nightingalejsonadapter-3.1.0.tar` & `nightingalejsonadapter-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 19:18:51.310287 nightingalejsonadapter-3.1.0/
--rw-rw-rw-   0        0        0      280 2024-05-20 19:18:51.310287 nightingalejsonadapter-3.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 19:18:51.302286 nightingalejsonadapter-3.1.0/nightingalejsonadapter/
--rw-rw-rw-   0        0        0        0 2024-05-03 01:38:22.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/__init__.py
--rw-rw-rw-   0        0        0      481 2024-05-03 01:38:22.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/intervention_adapter.py
--rw-rw-rw-   0        0        0      740 2024-05-03 14:52:50.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/patient_info_adapter.py
--rw-rw-rw-   0        0        0      455 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/trigger_adapter.py
--rw-rw-rw-   0        0        0      533 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/uuid_generator.py
--rw-rw-rw-   0        0        0      809 2024-05-20 09:22:44.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/vital_kafka_adapter.py
--rw-rw-rw-   0        0        0      629 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/vitals_adapter.py
--rw-rw-rw-   0        0        0     1885 2024-05-20 19:15:09.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter/vitals_response.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:18:51.309287 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/
--rw-rw-rw-   0        0        0      280 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-20 19:18:51.000000 nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 19:18:51.311287 nightingalejsonadapter-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0      797 2024-05-20 10:39:06.000000 nightingalejsonadapter-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:17:43.267597 nightingalejsonadapter-3.2.0/
+-rw-rw-rw-   0        0        0      280 2024-05-20 20:17:43.266596 nightingalejsonadapter-3.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 20:17:43.230567 nightingalejsonadapter-3.2.0/nightingalejsonadapter/
+-rw-rw-rw-   0        0        0        0 2024-05-03 01:38:22.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter/__init__.py
+-rw-rw-rw-   0        0        0      481 2024-05-03 01:38:22.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter/intervention_adapter.py
+-rw-rw-rw-   0        0        0      740 2024-05-03 14:52:50.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter/patient_info_adapter.py
+-rw-rw-rw-   0        0        0      455 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter/trigger_adapter.py
+-rw-rw-rw-   0        0        0      533 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter/uuid_generator.py
+-rw-rw-rw-   0        0        0      809 2024-05-20 09:22:44.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter/vital_kafka_adapter.py
+-rw-rw-rw-   0        0        0      629 2024-05-03 01:38:23.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter/vitals_adapter.py
+-rw-rw-rw-   0        0        0     1900 2024-05-20 20:10:03.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter/vitals_response.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:17:43.264603 nightingalejsonadapter-3.2.0/nightingalejsonadapter.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-20 20:17:42.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2024-05-20 20:17:43.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 20:17:42.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 20:17:42.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-20 20:17:42.000000 nightingalejsonadapter-3.2.0/nightingalejsonadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 20:17:43.268594 nightingalejsonadapter-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      797 2024-05-20 20:10:22.000000 nightingalejsonadapter-3.2.0/setup.py
```

### Comparing `nightingalejsonadapter-3.1.0/nightingalejsonadapter/patient_info_adapter.py` & `nightingalejsonadapter-3.2.0/nightingalejsonadapter/patient_info_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-3.1.0/nightingalejsonadapter/uuid_generator.py` & `nightingalejsonadapter-3.2.0/nightingalejsonadapter/uuid_generator.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-3.1.0/nightingalejsonadapter/vital_kafka_adapter.py` & `nightingalejsonadapter-3.2.0/nightingalejsonadapter/vital_kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-3.1.0/nightingalejsonadapter/vitals_adapter.py` & `nightingalejsonadapter-3.2.0/nightingalejsonadapter/vitals_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-3.1.0/nightingalejsonadapter/vitals_response.py` & `nightingalejsonadapter-3.2.0/nightingalejsonadapter/vitals_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,13 +53,13 @@
     predictionTimeDeltaMinutes: int
     victimId: str
     procedureMessageCount: int
     procedureMessages: List[ProcedureMessage]
     predictions: List[Prediction]
     
     @field_serializer('timestamp')
-    def timestamp_serializer(self, timestamp: datetime, _info):
+    def serialize_timestamp(self, timestamp: datetime, _info):
         return timestamp.isoformat().replace('+00:00', '') + 'Z'
     
     @field_serializer('lastMeasurementTimestamp')
-    def timestamp_serializer(self, lastMeasurementTimestamp: datetime, _info):
+    def serialize_last_measurement_timestamp(self, lastMeasurementTimestamp: datetime, _info):
         return lastMeasurementTimestamp.isoformat().replace('+00:00', '') + 'Z'
```

### Comparing `nightingalejsonadapter-3.1.0/nightingalejsonadapter.egg-info/SOURCES.txt` & `nightingalejsonadapter-3.2.0/nightingalejsonadapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-3.1.0/setup.py` & `nightingalejsonadapter-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '3.1.0' 
+VERSION = '3.2.0' 
 DESCRIPTION = 'JSON adapter'
 LONG_DESCRIPTION = 'JSON adapters and validators for Nightingale Communication and Integration'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="nightingalejsonadapter",
```


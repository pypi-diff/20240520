# Comparing `tmp/ebb_events-0.3.3.tar.gz` & `tmp/ebb_events-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_events-0.3.3.tar", max compression
+gzip compressed data, was "ebb_events-0.3.4.tar", max compression
```

## Comparing `ebb_events-0.3.3.tar` & `ebb_events-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.3/LICENSE
--rw-r--r--   0        0        0     8842 2024-05-14 16:56:47.897263 ebb_events-0.3.3/README.md
--rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.3/ebb_events/__init__.py
--rw-r--r--   0        0        0     8886 2024-05-15 20:31:26.930793 ebb_events-0.3.3/ebb_events/builders/event_builder.py
--rw-r--r--   0        0        0    10777 2024-05-17 17:46:46.038249 ebb_events-0.3.3/ebb_events/consumers/event_consumer.py
--rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.3/ebb_events/enums.py
--rw-r--r--   0        0        0      414 2024-05-10 21:40:45.943826 ebb_events-0.3.3/ebb_events/event_payload_utils.py
--rw-r--r--   0        0        0     2668 2024-05-13 20:48:51.509330 ebb_events-0.3.3/ebb_events/event_schema.py
--rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.3/ebb_events/exceptions.py
--rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.3/ebb_events/field_constants.py
--rw-r--r--   0        0        0      571 2024-05-17 17:46:46.038517 ebb_events-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 ebb_events-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.4/LICENSE
+-rw-r--r--   0        0        0     9163 2024-05-20 19:44:17.149941 ebb_events-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.4/ebb_events/__init__.py
+-rw-r--r--   0        0        0     8886 2024-05-15 20:31:26.930793 ebb_events-0.3.4/ebb_events/builders/event_builder.py
+-rw-r--r--   0        0        0    10777 2024-05-17 17:46:46.038249 ebb_events-0.3.4/ebb_events/consumers/event_consumer.py
+-rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.4/ebb_events/enums.py
+-rw-r--r--   0        0        0      875 2024-05-20 19:44:17.150314 ebb_events-0.3.4/ebb_events/event_payload_utils.py
+-rw-r--r--   0        0        0     3194 2024-05-20 19:44:17.150658 ebb_events-0.3.4/ebb_events/event_schema.py
+-rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.4/ebb_events/exceptions.py
+-rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.4/ebb_events/field_constants.py
+-rw-r--r--   0        0        0      571 2024-05-20 19:44:17.150966 ebb_events-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9661 1970-01-01 00:00:00.000000 ebb_events-0.3.4/PKG-INFO
```

### Comparing `ebb_events-0.3.3/LICENSE` & `ebb_events-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.3/README.md` & `ebb_events-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,16 @@
         "value": ____,
         "units": str
     },
     ...
 }
 ```
 
+To confirm that your message follow this structure, you can utilize the following utility helper which returns `True` for valid date event messages, and returns a dictionary of field validation errors for invalid messages: `ebb_events.event_payload_utils.validate_data_event_payload_message(payload_message=my_message)`
+
 ### EventEnvelope Class:
 The EventEnvelope class is used to consolidate all of the pieces of aa event payload and build the expected structure for a user so that users don't have to worry about constructing the properly formatted topic or payload. The `EventEnvelope` class expects to be provided with certain fields that are then used to build the topic and payload via class methods. These methods handle all the validation and formatting needed to ensure that your events follow the ebb-events standards.
 
 Required fields: `organization`, `system_id`, `event_type`, `subsystem_id`, `device_id`
 Useful methods: `EventEnvelope().build_event_topic()`, `EventEnvelope().build_event_payload()`
 
 # Event Consumer:
```

### Comparing `ebb_events-0.3.3/ebb_events/builders/event_builder.py` & `ebb_events-0.3.4/ebb_events/builders/event_builder.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.3/ebb_events/consumers/event_consumer.py` & `ebb_events-0.3.4/ebb_events/consumers/event_consumer.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.3/ebb_events/event_schema.py` & `ebb_events-0.3.4/ebb_events/event_schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 from marshmallow import Schema, fields, validate
 
 from ebb_events.enums import EventType
-from ebb_events.event_payload_utils import remove_nones_helper
 
 
 TOPIC_MAX_LENGTH = 50
 TOPIC_REGEX = r"^[a-z0-9-]+$"
 SOURCE_REGEX = r"^([a-z0-9-]+\/){4}[a-z0-9-]+$"
 SOURCE_MAX_LENGTH = 256
 
 
+def remove_nones_helper(data):
+    """
+    Recursive helper returns the parameter dictionary with None key:values removed
+    from top level and all nested dictionaries
+    """
+    if isinstance(data, dict):
+        return {
+            key: remove_nones_helper(value)
+            for key, value in data.items()
+            if value is not None and remove_nones_helper(value) is not None
+        }
+    return data
+
+
 class EventEnvelopeSchema(Schema):
     """Schema for EventEnvelope class to validate fields follow requirements"""
 
     organization = fields.Str(
         validate=[
             validate.Length(max=TOPIC_MAX_LENGTH),
             validate.Regexp(regex=TOPIC_REGEX),
@@ -51,18 +64,18 @@
     that id as a string value e.g. (str(id))
     """
 
     def _serialize(self, value, attr, obj, **kwargs):
         return str(value)
 
 
-class DictConditionallyRemoveInvalid(fields.Dict):
+class DictConditionallyRemoveNone(fields.Dict):
     """
     Class for EventPayloadSchema data field to conditionally
-    remove invalid fields: None, NaN
+    remove None fields
     """
 
     def _serialize(self, value, attr, obj, **kwargs):
         remove_nones = self.context.get("remove_nones", False)
         if remove_nones:
             # Filter out None values from the dictionary for top and second levels
             filtered_dict = remove_nones_helper(value)
@@ -86,8 +99,15 @@
     )
     type = fields.Str(
         required=True,
         validate=[
             validate.OneOf([e.value for e in EventType]),
         ],
     )
-    data = DictConditionallyRemoveInvalid(required=True)
+    data = DictConditionallyRemoveNone(required=True)
+
+
+class DataSchema(Schema):
+    """Schema for event data entries to check expected structure"""
+
+    value = fields.Float(required=True)
+    units = fields.Str(required=False, allow_none=True)
```

### Comparing `ebb_events-0.3.3/pyproject.toml` & `ebb_events-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-events"
-version = "0.3.3"
+version = "0.3.4"
 description = "Package for building and standardizing MQTT event messages."
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 marshmallow = "^3.21.1"
```

### Comparing `ebb_events-0.3.3/PKG-INFO` & `ebb_events-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-events
-Version: 0.3.3
+Version: 0.3.4
 Summary: Package for building and standardizing MQTT event messages.
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -116,14 +116,16 @@
         "value": ____,
         "units": str
     },
     ...
 }
 ```
 
+To confirm that your message follow this structure, you can utilize the following utility helper which returns `True` for valid date event messages, and returns a dictionary of field validation errors for invalid messages: `ebb_events.event_payload_utils.validate_data_event_payload_message(payload_message=my_message)`
+
 ### EventEnvelope Class:
 The EventEnvelope class is used to consolidate all of the pieces of aa event payload and build the expected structure for a user so that users don't have to worry about constructing the properly formatted topic or payload. The `EventEnvelope` class expects to be provided with certain fields that are then used to build the topic and payload via class methods. These methods handle all the validation and formatting needed to ensure that your events follow the ebb-events standards.
 
 Required fields: `organization`, `system_id`, `event_type`, `subsystem_id`, `device_id`
 Useful methods: `EventEnvelope().build_event_topic()`, `EventEnvelope().build_event_payload()`
 
 # Event Consumer:
```


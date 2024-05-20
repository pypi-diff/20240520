# Comparing `tmp/Serializer_Deserializer-1.6.tar.gz` & `tmp/Serializer_Deserializer-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Serializer_Deserializer-1.6.tar", last modified: Thu May 16 12:02:08 2024, max compression
+gzip compressed data, was "Serializer_Deserializer-1.7.tar", last modified: Mon May 20 18:32:33 2024, max compression
```

## Comparing `Serializer_Deserializer-1.6.tar` & `Serializer_Deserializer-1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:02:08.973003 Serializer_Deserializer-1.6/
--rw-rw-rw-   0        0        0      167 2024-05-16 12:02:08.973003 Serializer_Deserializer-1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 12:02:08.957294 Serializer_Deserializer-1.6/SerializerDeserializerModels/
--rw-rw-rw-   0        0        0     2639 2024-05-02 10:13:27.000000 Serializer_Deserializer-1.6/SerializerDeserializerModels/SerializerDeserializerModels.py
--rw-rw-rw-   0        0        0        0 2024-04-22 14:17:22.000000 Serializer_Deserializer-1.6/SerializerDeserializerModels/__init__.py
--rw-rw-rw-   0        0        0     2144 2024-05-16 12:01:55.000000 Serializer_Deserializer-1.6/SerializerDeserializerModels/models.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:02:08.973003 Serializer_Deserializer-1.6/Serializer_Deserializer.egg-info/
--rw-rw-rw-   0        0        0      167 2024-05-16 12:02:08.000000 Serializer_Deserializer-1.6/Serializer_Deserializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-05-16 12:02:08.000000 Serializer_Deserializer-1.6/Serializer_Deserializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:02:08.000000 Serializer_Deserializer-1.6/Serializer_Deserializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 14:27:54.000000 Serializer_Deserializer-1.6/Serializer_Deserializer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2024-05-16 12:02:08.000000 Serializer_Deserializer-1.6/Serializer_Deserializer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:02:08.973003 Serializer_Deserializer-1.6/setup.cfg
--rw-rw-rw-   0        0        0      291 2024-05-16 12:02:07.000000 Serializer_Deserializer-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:32:33.223631 Serializer_Deserializer-1.7/
+-rw-rw-rw-   0        0        0      167 2024-05-20 18:32:33.223631 Serializer_Deserializer-1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 18:32:33.215632 Serializer_Deserializer-1.7/SerializerDeserializerModels/
+-rw-rw-rw-   0        0        0     2639 2024-05-20 18:31:10.000000 Serializer_Deserializer-1.7/SerializerDeserializerModels/SerializerDeserializerModels.py
+-rw-rw-rw-   0        0        0        0 2024-04-22 14:17:22.000000 Serializer_Deserializer-1.7/SerializerDeserializerModels/__init__.py
+-rw-rw-rw-   0        0        0     2144 2024-05-16 12:01:55.000000 Serializer_Deserializer-1.7/SerializerDeserializerModels/models.py
+drwxrwxrwx   0        0        0        0 2024-05-20 18:32:33.222631 Serializer_Deserializer-1.7/Serializer_Deserializer.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-05-20 18:32:33.000000 Serializer_Deserializer-1.7/Serializer_Deserializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-20 18:32:33.000000 Serializer_Deserializer-1.7/Serializer_Deserializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 18:32:33.000000 Serializer_Deserializer-1.7/Serializer_Deserializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 14:27:54.000000 Serializer_Deserializer-1.7/Serializer_Deserializer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       29 2024-05-20 18:32:33.000000 Serializer_Deserializer-1.7/Serializer_Deserializer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 18:32:33.224630 Serializer_Deserializer-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      291 2024-05-20 18:32:29.000000 Serializer_Deserializer-1.7/setup.py
```

### Comparing `Serializer_Deserializer-1.6/SerializerDeserializerModels/SerializerDeserializerModels.py` & `Serializer_Deserializer-1.7/SerializerDeserializerModels/SerializerDeserializerModels.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     @staticmethod
     def message_to_json(message):
         return {
             'ID': message.id,
             'FROM': message.from_user,
             'TO': message.to_user,
             'GROUP': message.group,
-            'CREATE_AT': message.created_at.strftime("%I:%M"),
+            'CREATE_AT': message.created_at.strftime("%H:%M"),
             'CONTENT': message.content
         }
 
     @staticmethod
     def json_to_message(message_dict):
         message = Message(id=message_dict.get('ID', None), from_user=message_dict.get('FROM', None),
                     to_user=message_dict.get('TO', None), group=message_dict.get('GROUP', None),
```

### Comparing `Serializer_Deserializer-1.6/SerializerDeserializerModels/models.py` & `Serializer_Deserializer-1.7/SerializerDeserializerModels/models.py`

 * *Files identical despite different names*


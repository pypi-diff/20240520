# Comparing `tmp/talus-1.0.0rc5.tar.gz` & `tmp/talus-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talus-1.0.0rc5.tar", last modified: Fri May 17 21:40:12 2024, max compression
+gzip compressed data, was "talus-1.0.0rc6.tar", last modified: Mon May 20 18:15:24 2024, max compression
```

## Comparing `talus-1.0.0rc5.tar` & `talus-1.0.0rc6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-17 21:40:00.000000 talus-1.0.0rc5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-17 21:40:00.000000 talus-1.0.0rc5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-17 21:40:00.000000 talus-1.0.0rc5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-17 21:40:00.000000 talus-1.0.0rc5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-17 21:40:12.355312 talus-1.0.0rc5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-17 21:40:00.000000 talus-1.0.0rc5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-17 21:40:00.000000 talus-1.0.0rc5/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-17 21:40:00.000000 talus-1.0.0rc5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-17 21:40:12.355312 talus-1.0.0rc5/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.351312 talus-1.0.0rc5/talus/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/consumer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/talus/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/binding.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     2393 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     4703 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/talus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4660 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/talus/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_binding.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3935 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7784 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_processor.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/test_producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/talus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-17 21:40:00.000000 talus-1.0.0rc5/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-20 18:15:11.000000 talus-1.0.0rc6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-20 18:15:11.000000 talus-1.0.0rc6/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-20 18:15:11.000000 talus-1.0.0rc6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-20 18:15:11.000000 talus-1.0.0rc6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-20 18:15:24.281118 talus-1.0.0rc6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-20 18:15:11.000000 talus-1.0.0rc6/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-20 18:15:11.000000 talus-1.0.0rc6/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-20 18:15:11.000000 talus-1.0.0rc6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 18:15:24.281118 talus-1.0.0rc6/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.277118 talus-1.0.0rc6/talus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/consumer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/talus/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/binding.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4703 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/talus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/talus/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_binding.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/test_producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/talus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-20 18:15:23.000000 talus-1.0.0rc6/talus.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-20 18:15:11.000000 talus-1.0.0rc6/tox.ini
```

### Comparing `talus-1.0.0rc5/.gitignore` & `talus-1.0.0rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/.pre-commit-config.yaml` & `talus-1.0.0rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/LICENSE` & `talus-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/PKG-INFO` & `talus-1.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc5/README.rst` & `talus-1.0.0rc6/README.rst`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/bitbucket-pipelines.yml` & `talus-1.0.0rc6/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/pyproject.toml` & `talus-1.0.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/base.py` & `talus-1.0.0rc6/talus/base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/consumer.py` & `talus-1.0.0rc6/talus/consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/models/binding.py` & `talus-1.0.0rc6/talus/models/binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/models/connection_parameters.py` & `talus-1.0.0rc6/talus/models/connection_parameters.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/models/message.py` & `talus-1.0.0rc6/talus/models/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class MessageBodyBase(BaseModel):
     """
     Base class for message schemas which can be used to validate message bodies.
     """
 
     model_config = ConfigDict(extra="allow")
 
-    conversation_id: str = Field(default_factory=lambda: uuid.uuid4().hex, alias="conversationId")
+    conversationId: str = Field(default_factory=lambda: uuid.uuid4().hex)
 
 
 class MessageBase:
     """
     Base class for messages establishing a common interface for use by DurableConnections
     """
```

### Comparing `talus-1.0.0rc5/talus/models/processor.py` & `talus-1.0.0rc6/talus/models/processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/models/retryer.py` & `talus-1.0.0rc6/talus/models/retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/producer.py` & `talus-1.0.0rc6/talus/producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/tests/conftest.py` & `talus-1.0.0rc6/talus/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 @pytest.fixture(params=["no-conversation-id", "conversation-id"])
 def message_data(request, message_data_schema_cls) -> dict[str, str]:
     result = message_data_schema_cls(key=uuid4().hex).model_dump()
     match request.param:
         case "no-conversation-id":
-            result.pop("conversation_id")
+            result.pop("conversationId")
             return result
         case "conversation-id":
             return result
         case _:
             raise NotImplementedError("message data parameter not implemented")
```

### Comparing `talus-1.0.0rc5/talus/tests/models/test_binding.py` & `talus-1.0.0rc6/talus/tests/models/test_binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/tests/models/test_message.py` & `talus-1.0.0rc6/talus/tests/models/test_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,33 +13,27 @@
 
 def test_consume_message_model_valid(
     method, properties, body, routing_key, headers, delivery_tag, message_data
 ):
     """
     :given: A ConsumeMessage class
     :when: A new instance is created with default args
-    :then: The instance body has a conversation_id and other properties are set
+    :then: The instance body has a conversationId and other properties are set
     """
     # given/when
     message = ConsumeMessageBase(method=method, properties=properties, body=body)
     # then
-    assert message.body.conversation_id is not None
+    assert message.body.conversationId is not None
     assert message.method == method
     assert message.properties == properties
     assert message.routing_key == routing_key
     assert message.headers == headers
     assert message.delivery_tag == delivery_tag
     assert (
-        message.body.model_dump()
-        == {"conversation_id": message.body.conversation_id} | message_data
-    )
-    serialized_message_dict = json.loads(message.body.model_dump_json(by_alias=True))
-    assert serialized_message_dict["conversationId"] == message.body.conversation_id
-    assert (
-        serialized_message_dict == {"conversationId": message.body.conversation_id} | message_data
+        message.body.model_dump() == {"conversationId": message.body.conversationId} | message_data
     )
 
 
 class ExampleMessageBody(MessageBodyBase):
     required_str: str
     required_int: int
 
@@ -68,32 +62,26 @@
         ConsumableMessage(method=method, properties=properties, body=invalid_body)
 
 
 def test_publish_message_model(routing_key, headers, body, message_data, publish_message_cls):
     """
     :given: A PublishMessage class
     :when: A new instance is created
-    :then: The instance body has a conversation_id and other properties are set
+    :then: The instance body has a conversationId and other properties are set
     """
     # given/when
     message = publish_message_cls(body=body)
     # then
-    assert message.body.conversation_id is not None
+    assert message.body.conversationId is not None
     assert message.routing_key == routing_key
     assert message.headers == headers
     assert isinstance(message.properties, pika.spec.BasicProperties)
     assert message.properties.headers == headers
     assert (
-        message.body.model_dump()
-        == {"conversation_id": message.body.conversation_id} | message_data
-    )
-    serialized_message_dict = json.loads(message.body.model_dump_json(by_alias=True))
-    assert serialized_message_dict["conversationId"] == message.body.conversation_id
-    assert (
-        serialized_message_dict == {"conversationId": message.body.conversation_id} | message_data
+        message.body.model_dump() == {"conversationId": message.body.conversationId} | message_data
     )
 
 
 class PublishMessage(PublishMessageBase):
     message_body_cls = ExampleMessageBody
     routing_key = "test.m"
```

### Comparing `talus-1.0.0rc5/talus/tests/models/test_processor.py` & `talus-1.0.0rc6/talus/tests/models/test_processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/tests/models/test_queue.py` & `talus-1.0.0rc6/talus/tests/models/test_queue.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/tests/models/test_retryer.py` & `talus-1.0.0rc6/talus/tests/models/test_retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/tests/test_base.py` & `talus-1.0.0rc6/talus/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/tests/test_consumer.py` & `talus-1.0.0rc6/talus/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus/tests/test_producer.py` & `talus-1.0.0rc6/talus/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/talus.egg-info/PKG-INFO` & `talus-1.0.0rc6/talus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc5/talus.egg-info/SOURCES.txt` & `talus-1.0.0rc6/talus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc5/tox.ini` & `talus-1.0.0rc6/tox.ini`

 * *Files identical despite different names*


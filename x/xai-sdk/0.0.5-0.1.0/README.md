# Comparing `tmp/xai_sdk-0.0.5.tar.gz` & `tmp/xai_sdk-0.1.0.tar.gz`

## Comparing `xai_sdk-0.0.5.tar` & `xai_sdk-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/Makefile
--rwxr-xr-x   0        0        0     1703 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/create_bindings.sh
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/__about__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/__init__.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/chat.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/client.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/files.py
--rw-r--r--   0        0        0    22409 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/grok.py
--rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/ide.py
--rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/sampler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/__init__.py
--rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2.py
--rw-r--r--   0        0        0    12809 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2.pyi
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2_grpc.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2.pyi
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2_grpc.py
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2.py
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2.pyi
--rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2_grpc.py
--rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2.py
--rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2.pyi
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2_grpc.py
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2.pyi
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2_grpc.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/x_entities_pb2.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/x_entities_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/x_entities_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/README.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 xai_sdk-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/Makefile
+-rwxr-xr-x   0        0        0     1703 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/create_bindings.sh
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/__about__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/__init__.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/chat.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/client.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/files.py
+-rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/grok.py
+-rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/ide.py
+-rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/sampler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/__init__.py
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/chat_pb2.py
+-rw-r--r--   0        0        0    13089 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/chat_pb2.pyi
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/chat_pb2_grpc.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/files_pb2.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/files_pb2.pyi
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/files_pb2_grpc.py
+-rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/prod_search_pb2.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/prod_search_pb2.pyi
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/prod_search_pb2_grpc.py
+-rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/sampler_public_pb2.py
+-rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/sampler_public_pb2.pyi
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/sampler_public_pb2_grpc.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/stateless_chat_pb2.py
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/stateless_chat_pb2.pyi
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/stateless_chat_pb2_grpc.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/x_entities_pb2.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/x_entities_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/x_entities_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/google/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/google/api/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/google/api/http_pb2.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/src/xai_sdk/proto/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/README.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 xai_sdk-0.1.0/PKG-INFO
```

### Comparing `xai_sdk-0.0.5/Makefile` & `xai_sdk-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/create_bindings.sh` & `xai_sdk-0.1.0/create_bindings.sh`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/__init__.py` & `xai_sdk-0.1.0/src/xai_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/chat.py` & `xai_sdk-0.1.0/src/xai_sdk/chat.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/client.py` & `xai_sdk-0.1.0/src/xai_sdk/client.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/files.py` & `xai_sdk-0.1.0/src/xai_sdk/files.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/grok.py` & `xai_sdk-0.1.0/src/xai_sdk/grok.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,33 +79,29 @@
 
     def __init__(
         self,
         stub: chat_pb2_grpc.ChatStub,
         model_name: str,
         fun_mode: bool,
         conversation_id: Optional[str],
-        dev_only_use_grok: bool = True,
     ):
         """Initializes a new instance of the `Conversation` class.
 
         Args:
             stub: gRPC stub used to communicate with the xAI API.
             model_name: Name of the model to use for this conversation.
             fun_mode: True if fun mode shall be enabled for this conversation.
             conversation_id: ID of this conversation. If no ID was provided, a new conversation is
                 created when the first API call is issued.
-            dev_only_use_grok: By setting this to `False`, the conversation is with the raw model
-                instead of with Grok. This means there is no support for searching or fun mode.
         """
         self._stub = stub
         self._model_name = model_name
         self._fun_mode = fun_mode
         self._conversation_id: Optional[str] = conversation_id
         self._conversation: Optional[chat_pb2.Conversation] = None
-        self._use_grok = dev_only_use_grok
 
         # True if this conversation was deleted.
         self._deleted = False
 
         # A mapping from response IDs to the respective response objects.
         self._responses: dict[str, "Response"] = {}
 
@@ -273,15 +269,14 @@
                 # Start sampling from Grok.
                 response = self._stub.AddResponse(
                     chat_pb2.AddResponseRequest(
                         conversation_id=self._conversation_id,
                         message=user_message,
                         model_name=self._model_name,
                         parent_response_id=self._leaf_response_id or "",
-                        use_grok=self._use_grok,
                         system_prompt_name="fun" if self._fun_mode else "",
                     )
                 )
 
                 # Unroll the responses and emit the tokens.
                 async for msg in response:
                     if msg.HasField("user_response"):
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/ide.py` & `xai_sdk-0.1.0/src/xai_sdk/ide.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/sampler.py` & `xai_sdk-0.1.0/src/xai_sdk/sampler.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/chat_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: chat.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,20 +15,21 @@
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import sampler_public_pb2 as sampler__public__pb2
 from . import prod_search_pb2 as prod__search__pb2
 from . import x_entities_pb2 as x__entities__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nchat.proto\x12\nprompt_ide\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x14sampler_public.proto\x1a\x11prod_search.proto\x1a\x10x_entities.proto\"I\n\x19RegenerateResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x13\n\x0bresponse_id\x18\x02 \x01(\t\"7\n\x19\x43reateConversationRequest\x12\x1a\n\x12system_prompt_name\x18\x01 \x01(\t\"1\n\x16GetConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\"4\n\x19\x44\x65leteConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\"L\n\x19ListConversationsResponse\x12/\n\rconversations\x18\x01 \x03(\x0b\x32\x18.prompt_ide.Conversation\"I\n\x14GenerateTitleRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x18\n\x10leaf_response_id\x18\x02 \x01(\t\"*\n\x15GenerateTitleResponse\x12\x11\n\tnew_title\x18\x01 \x01(\t\"p\n\x17\x41\x64\x64ModelResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0f\n\x07partial\x18\x03 \x01(\x08\x12\x1a\n\x12parent_response_id\x18\x04 \x01(\t\"T\n\x19UpdateConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07starred\x18\x03 \x01(\x08\"\x89\x01\n\rSearchContext\x12\x18\n\x10web_search_query\x18\x01 \x01(\t\x12\x1c\n\x14web_formatted_chunks\x18\x02 \x01(\t\x12\x16\n\x0ex_search_query\x18\x03 \x01(\t\x12\x1a\n\x12x_formatted_chunks\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\t\"\xc8\x01\n\x10ResponseDebugLog\x12\x1a\n\x12system_prompt_name\x18\x01 \x01(\t\x12\x16\n\x0e\x64isable_search\x18\x02 \x01(\x08\x12\x11\n\tweb_query\x18\x03 \x01(\t\x12\x0f\n\x07x_query\x18\x04 \x01(\t\x12\x13\n\x0bimage_query\x18\x05 \x01(\t\x12\x0e\n\x06prompt\x18\x07 \x01(\t\x12\x31\n\x0esearch_context\x18\x08 \x01(\x0b\x32\x19.prompt_ide.SearchContextJ\x04\x08\x06\x10\x07\"\x83\x03\n\x12\x41\x64\x64ResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x1a\n\x12parent_response_id\x18\x05 \x01(\t\x12\x1a\n\x12system_prompt_name\x18\x07 \x01(\t\x12\x16\n\x0e\x64isable_search\x18\x08 \x01(\x08\x12\x1f\n\x17\x65nable_image_generation\x18\t \x01(\x08\x12\x12\n\nforce_rust\x18\n \x01(\x08\x12:\n\x17injected_search_context\x18\x0b \x01(\x0b\x32\x19.prompt_ide.SearchContext\x12\x18\n\x0btemperature\x18\x0c \x01(\x02H\x00\x88\x01\x01\x12\x11\n\x04seed\x18\r \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x14ignore_time_location\x18\x0e \x01(\x08\x42\x0e\n\x0c_temperatureB\x07\n\x05_seedJ\x04\x08\x04\x10\x05J\x04\x08\x06\x10\x07\"\xbd\x03\n\x13\x41\x64\x64ResponseResponse\x12-\n\ruser_response\x18\x01 \x01(\x0b\x32\x14.prompt_ide.ResponseH\x00\x12\x31\n\x05token\x18\x02 \x01(\x0b\x32 .prompt_ide.SampleTokensResponseH\x00\x12.\n\x0emodel_response\x18\x03 \x01(\x0b\x32\x14.prompt_ide.ResponseH\x00\x12/\n\x0cquery_action\x18\x04 \x01(\x0b\x32\x17.prompt_ide.QueryActionH\x00\x12H\n\x19image_generation_response\x18\x05 \x01(\x0b\x32#.prompt_ide.ImageGenerationResponseH\x00\x12\x36\n\x10x_search_results\x18\x06 \x01(\x0b\x32\x1a.prompt_ide.XSearchResultsH\x00\x12U\n cached_image_generation_response\x18\x07 \x01(\x0b\x32).prompt_ide.CachedImageGenerationResponseH\x00\x42\n\n\x08response\"*\n\x0bQueryAction\x12\r\n\x05query\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x8a\x02\n\x0c\x43onversation\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07starred\x18\x06 \x01(\x08\x12/\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodify_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\tresponses\x18\x05 \x03(\x0b\x32\x14.prompt_ide.Response\x12\x1f\n\x12system_prompt_name\x18\x07 \x01(\tH\x00\x88\x01\x01\x42\x15\n\x13_system_prompt_name\"\xe6\x02\n\x08Response\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0e\n\x06sender\x18\x03 \x01(\t\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12parent_response_id\x18\x05 \x01(\t\x12\x0e\n\x06manual\x18\x06 \x01(\x08\x12\x0f\n\x07partial\x18\x07 \x01(\x08\x12\x0e\n\x06shared\x18\x08 \x01(\x08\x12\r\n\x05query\x18\t \x01(\t\x12\x12\n\nquery_type\x18\n \x01(\t\x12\x11\n\txpost_ids\x18\x0b \x03(\t\x12!\n\x06xposts\x18\x0c \x03(\x0b\x32\x11.prompt_ide.XPost\x12\x1c\n\x14generated_image_urls\x18\r \x03(\t\x12/\n\tdebug_log\x18\x0e \x01(\x0b\x32\x1c.prompt_ide.ResponseDebugLog\"N\n\x17ImageGenerationResponse\x12\x1d\n\x15generated_image_bytes\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\"2\n\x1d\x43\x61\x63hedImageGenerationResponse\x12\x11\n\timage_url\x18\x01 \x01(\t\"H\n\x18ShareConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x13\n\x0bresponse_id\x18\x02 \x01(\t\".\n\x19ShareConversationResponse\x12\x11\n\tshared_id\x18\x01 \x01(\t2\x99\x06\n\x04\x43hat\x12W\n\x12\x43reateConversation\x12%.prompt_ide.CreateConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12Q\n\x0fGetConversation\x12\".prompt_ide.GetConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12T\n\x11ListConversations\x12\x16.google.protobuf.Empty\x1a%.prompt_ide.ListConversationsResponse\"\x00\x12R\n\x0b\x41\x64\x64Response\x12\x1e.prompt_ide.AddResponseRequest\x1a\x1f.prompt_ide.AddResponseResponse\"\x00\x30\x01\x12U\n\x12\x44\x65leteConversation\x12%.prompt_ide.DeleteConversationRequest\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\rGenerateTitle\x12 .prompt_ide.GenerateTitleRequest\x1a!.prompt_ide.GenerateTitleResponse\"\x00\x12W\n\x12UpdateConversation\x12%.prompt_ide.UpdateConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12O\n\x10\x41\x64\x64ModelResponse\x12#.prompt_ide.AddModelResponseRequest\x1a\x14.prompt_ide.Response\"\x00\x12\x62\n\x11ShareConversation\x12$.prompt_ide.ShareConversationRequest\x1a%.prompt_ide.ShareConversationResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nchat.proto\x12\nprompt_ide\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x14sampler_public.proto\x1a\x11prod_search.proto\x1a\x10x_entities.proto\"I\n\x19RegenerateResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x13\n\x0bresponse_id\x18\x02 \x01(\t\"7\n\x19\x43reateConversationRequest\x12\x1a\n\x12system_prompt_name\x18\x01 \x01(\t\"1\n\x16GetConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\"4\n\x19\x44\x65leteConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\"L\n\x19ListConversationsResponse\x12/\n\rconversations\x18\x01 \x03(\x0b\x32\x18.prompt_ide.Conversation\"I\n\x14GenerateTitleRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x18\n\x10leaf_response_id\x18\x02 \x01(\t\"*\n\x15GenerateTitleResponse\x12\x11\n\tnew_title\x18\x01 \x01(\t\"p\n\x17\x41\x64\x64ModelResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0f\n\x07partial\x18\x03 \x01(\x08\x12\x1a\n\x12parent_response_id\x18\x04 \x01(\t\"T\n\x19UpdateConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07starred\x18\x03 \x01(\x08\"\x89\x01\n\rSearchContext\x12\x18\n\x10web_search_query\x18\x01 \x01(\t\x12\x1c\n\x14web_formatted_chunks\x18\x02 \x01(\t\x12\x16\n\x0ex_search_query\x18\x03 \x01(\t\x12\x1a\n\x12x_formatted_chunks\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\t\"\xc8\x01\n\x10ResponseDebugLog\x12\x1a\n\x12system_prompt_name\x18\x01 \x01(\t\x12\x16\n\x0e\x64isable_search\x18\x02 \x01(\x08\x12\x11\n\tweb_query\x18\x03 \x01(\t\x12\x0f\n\x07x_query\x18\x04 \x01(\t\x12\x13\n\x0bimage_query\x18\x05 \x01(\t\x12\x0e\n\x06prompt\x18\x07 \x01(\t\x12\x31\n\x0esearch_context\x18\x08 \x01(\x0b\x32\x19.prompt_ide.SearchContextJ\x04\x08\x06\x10\x07\"\xb3\x01\n\x11\x41\x64\x64itionalOptions\x12:\n\x17injected_search_context\x18\x01 \x01(\x0b\x32\x19.prompt_ide.SearchContext\x12\x18\n\x0btemperature\x18\x02 \x01(\x02H\x00\x88\x01\x01\x12\x11\n\x04seed\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x14ignore_time_location\x18\x04 \x01(\x08\x42\x0e\n\x0c_temperatureB\x07\n\x05_seed\"\xb6\x02\n\x12\x41\x64\x64ResponseRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x1a\n\x12parent_response_id\x18\x05 \x01(\t\x12\x1a\n\x12system_prompt_name\x18\x07 \x01(\t\x12\x16\n\x0e\x64isable_search\x18\x08 \x01(\x08\x12\x1f\n\x17\x65nable_image_generation\x18\t \x01(\x08\x12\x12\n\nforce_rust\x18\n \x01(\x08\x12\x39\n\x12\x61\x64\x64itional_options\x18\x0f \x01(\x0b\x32\x1d.prompt_ide.AdditionalOptionsJ\x04\x08\x04\x10\x05J\x04\x08\x06\x10\x07J\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\r\x10\x0eJ\x04\x08\x0e\x10\x0f\"\xbd\x03\n\x13\x41\x64\x64ResponseResponse\x12-\n\ruser_response\x18\x01 \x01(\x0b\x32\x14.prompt_ide.ResponseH\x00\x12\x31\n\x05token\x18\x02 \x01(\x0b\x32 .prompt_ide.SampleTokensResponseH\x00\x12.\n\x0emodel_response\x18\x03 \x01(\x0b\x32\x14.prompt_ide.ResponseH\x00\x12/\n\x0cquery_action\x18\x04 \x01(\x0b\x32\x17.prompt_ide.QueryActionH\x00\x12H\n\x19image_generation_response\x18\x05 \x01(\x0b\x32#.prompt_ide.ImageGenerationResponseH\x00\x12\x36\n\x10x_search_results\x18\x06 \x01(\x0b\x32\x1a.prompt_ide.XSearchResultsH\x00\x12U\n cached_image_generation_response\x18\x07 \x01(\x0b\x32).prompt_ide.CachedImageGenerationResponseH\x00\x42\n\n\x08response\"*\n\x0bQueryAction\x12\r\n\x05query\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x8a\x02\n\x0c\x43onversation\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07starred\x18\x06 \x01(\x08\x12/\n\x0b\x63reate_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0bmodify_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\tresponses\x18\x05 \x03(\x0b\x32\x14.prompt_ide.Response\x12\x1f\n\x12system_prompt_name\x18\x07 \x01(\tH\x00\x88\x01\x01\x42\x15\n\x13_system_prompt_name\"\xe6\x02\n\x08Response\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0e\n\x06sender\x18\x03 \x01(\t\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12parent_response_id\x18\x05 \x01(\t\x12\x0e\n\x06manual\x18\x06 \x01(\x08\x12\x0f\n\x07partial\x18\x07 \x01(\x08\x12\x0e\n\x06shared\x18\x08 \x01(\x08\x12\r\n\x05query\x18\t \x01(\t\x12\x12\n\nquery_type\x18\n \x01(\t\x12\x11\n\txpost_ids\x18\x0b \x03(\t\x12!\n\x06xposts\x18\x0c \x03(\x0b\x32\x11.prompt_ide.XPost\x12\x1c\n\x14generated_image_urls\x18\r \x03(\t\x12/\n\tdebug_log\x18\x0e \x01(\x0b\x32\x1c.prompt_ide.ResponseDebugLog\"N\n\x17ImageGenerationResponse\x12\x1d\n\x15generated_image_bytes\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\"2\n\x1d\x43\x61\x63hedImageGenerationResponse\x12\x11\n\timage_url\x18\x01 \x01(\t\"H\n\x18ShareConversationRequest\x12\x17\n\x0f\x63onversation_id\x18\x01 \x01(\t\x12\x13\n\x0bresponse_id\x18\x02 \x01(\t\".\n\x19ShareConversationResponse\x12\x11\n\tshared_id\x18\x01 \x01(\t2\x99\x06\n\x04\x43hat\x12W\n\x12\x43reateConversation\x12%.prompt_ide.CreateConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12Q\n\x0fGetConversation\x12\".prompt_ide.GetConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12T\n\x11ListConversations\x12\x16.google.protobuf.Empty\x1a%.prompt_ide.ListConversationsResponse\"\x00\x12R\n\x0b\x41\x64\x64Response\x12\x1e.prompt_ide.AddResponseRequest\x1a\x1f.prompt_ide.AddResponseResponse\"\x00\x30\x01\x12U\n\x12\x44\x65leteConversation\x12%.prompt_ide.DeleteConversationRequest\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\rGenerateTitle\x12 .prompt_ide.GenerateTitleRequest\x1a!.prompt_ide.GenerateTitleResponse\"\x00\x12W\n\x12UpdateConversation\x12%.prompt_ide.UpdateConversationRequest\x1a\x18.prompt_ide.Conversation\"\x00\x12O\n\x10\x41\x64\x64ModelResponse\x12#.prompt_ide.AddModelResponseRequest\x1a\x14.prompt_ide.Response\"\x00\x12\x62\n\x11ShareConversation\x12$.prompt_ide.ShareConversationRequest\x1a%.prompt_ide.ShareConversationResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'chat_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
+
   DESCRIPTOR._options = None
   _globals['_REGENERATERESPONSEREQUEST']._serialized_start=147
   _globals['_REGENERATERESPONSEREQUEST']._serialized_end=220
   _globals['_CREATECONVERSATIONREQUEST']._serialized_start=222
   _globals['_CREATECONVERSATIONREQUEST']._serialized_end=277
   _globals['_GETCONVERSATIONREQUEST']._serialized_start=279
   _globals['_GETCONVERSATIONREQUEST']._serialized_end=328
@@ -45,28 +45,30 @@
   _globals['_ADDMODELRESPONSEREQUEST']._serialized_end=693
   _globals['_UPDATECONVERSATIONREQUEST']._serialized_start=695
   _globals['_UPDATECONVERSATIONREQUEST']._serialized_end=779
   _globals['_SEARCHCONTEXT']._serialized_start=782
   _globals['_SEARCHCONTEXT']._serialized_end=919
   _globals['_RESPONSEDEBUGLOG']._serialized_start=922
   _globals['_RESPONSEDEBUGLOG']._serialized_end=1122
-  _globals['_ADDRESPONSEREQUEST']._serialized_start=1125
-  _globals['_ADDRESPONSEREQUEST']._serialized_end=1512
-  _globals['_ADDRESPONSERESPONSE']._serialized_start=1515
-  _globals['_ADDRESPONSERESPONSE']._serialized_end=1960
-  _globals['_QUERYACTION']._serialized_start=1962
-  _globals['_QUERYACTION']._serialized_end=2004
-  _globals['_CONVERSATION']._serialized_start=2007
-  _globals['_CONVERSATION']._serialized_end=2273
-  _globals['_RESPONSE']._serialized_start=2276
-  _globals['_RESPONSE']._serialized_end=2634
-  _globals['_IMAGEGENERATIONRESPONSE']._serialized_start=2636
-  _globals['_IMAGEGENERATIONRESPONSE']._serialized_end=2714
-  _globals['_CACHEDIMAGEGENERATIONRESPONSE']._serialized_start=2716
-  _globals['_CACHEDIMAGEGENERATIONRESPONSE']._serialized_end=2766
-  _globals['_SHARECONVERSATIONREQUEST']._serialized_start=2768
-  _globals['_SHARECONVERSATIONREQUEST']._serialized_end=2840
-  _globals['_SHARECONVERSATIONRESPONSE']._serialized_start=2842
-  _globals['_SHARECONVERSATIONRESPONSE']._serialized_end=2888
-  _globals['_CHAT']._serialized_start=2891
-  _globals['_CHAT']._serialized_end=3684
+  _globals['_ADDITIONALOPTIONS']._serialized_start=1125
+  _globals['_ADDITIONALOPTIONS']._serialized_end=1304
+  _globals['_ADDRESPONSEREQUEST']._serialized_start=1307
+  _globals['_ADDRESPONSEREQUEST']._serialized_end=1617
+  _globals['_ADDRESPONSERESPONSE']._serialized_start=1620
+  _globals['_ADDRESPONSERESPONSE']._serialized_end=2065
+  _globals['_QUERYACTION']._serialized_start=2067
+  _globals['_QUERYACTION']._serialized_end=2109
+  _globals['_CONVERSATION']._serialized_start=2112
+  _globals['_CONVERSATION']._serialized_end=2378
+  _globals['_RESPONSE']._serialized_start=2381
+  _globals['_RESPONSE']._serialized_end=2739
+  _globals['_IMAGEGENERATIONRESPONSE']._serialized_start=2741
+  _globals['_IMAGEGENERATIONRESPONSE']._serialized_end=2819
+  _globals['_CACHEDIMAGEGENERATIONRESPONSE']._serialized_start=2821
+  _globals['_CACHEDIMAGEGENERATIONRESPONSE']._serialized_end=2871
+  _globals['_SHARECONVERSATIONREQUEST']._serialized_start=2873
+  _globals['_SHARECONVERSATIONREQUEST']._serialized_end=2945
+  _globals['_SHARECONVERSATIONRESPONSE']._serialized_start=2947
+  _globals['_SHARECONVERSATIONRESPONSE']._serialized_end=2993
+  _globals['_CHAT']._serialized_start=2996
+  _globals['_CHAT']._serialized_end=3789
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2.pyi` & `xai_sdk-0.1.0/src/xai_sdk/proto/chat_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,97 +7,97 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class RegenerateResponseRequest(_message.Message):
-    __slots__ = ("conversation_id", "response_id")
+    __slots__ = ["conversation_id", "response_id"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_ID_FIELD_NUMBER: _ClassVar[int]
     conversation_id: str
     response_id: str
     def __init__(self, conversation_id: _Optional[str] = ..., response_id: _Optional[str] = ...) -> None: ...
 
 class CreateConversationRequest(_message.Message):
-    __slots__ = ("system_prompt_name",)
+    __slots__ = ["system_prompt_name"]
     SYSTEM_PROMPT_NAME_FIELD_NUMBER: _ClassVar[int]
     system_prompt_name: str
     def __init__(self, system_prompt_name: _Optional[str] = ...) -> None: ...
 
 class GetConversationRequest(_message.Message):
-    __slots__ = ("conversation_id",)
+    __slots__ = ["conversation_id"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     conversation_id: str
     def __init__(self, conversation_id: _Optional[str] = ...) -> None: ...
 
 class DeleteConversationRequest(_message.Message):
-    __slots__ = ("conversation_id",)
+    __slots__ = ["conversation_id"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     conversation_id: str
     def __init__(self, conversation_id: _Optional[str] = ...) -> None: ...
 
 class ListConversationsResponse(_message.Message):
-    __slots__ = ("conversations",)
+    __slots__ = ["conversations"]
     CONVERSATIONS_FIELD_NUMBER: _ClassVar[int]
     conversations: _containers.RepeatedCompositeFieldContainer[Conversation]
     def __init__(self, conversations: _Optional[_Iterable[_Union[Conversation, _Mapping]]] = ...) -> None: ...
 
 class GenerateTitleRequest(_message.Message):
-    __slots__ = ("conversation_id", "leaf_response_id")
+    __slots__ = ["conversation_id", "leaf_response_id"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     LEAF_RESPONSE_ID_FIELD_NUMBER: _ClassVar[int]
     conversation_id: str
     leaf_response_id: str
     def __init__(self, conversation_id: _Optional[str] = ..., leaf_response_id: _Optional[str] = ...) -> None: ...
 
 class GenerateTitleResponse(_message.Message):
-    __slots__ = ("new_title",)
+    __slots__ = ["new_title"]
     NEW_TITLE_FIELD_NUMBER: _ClassVar[int]
     new_title: str
     def __init__(self, new_title: _Optional[str] = ...) -> None: ...
 
 class AddModelResponseRequest(_message.Message):
-    __slots__ = ("conversation_id", "message", "partial", "parent_response_id")
+    __slots__ = ["conversation_id", "message", "partial", "parent_response_id"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     PARTIAL_FIELD_NUMBER: _ClassVar[int]
     PARENT_RESPONSE_ID_FIELD_NUMBER: _ClassVar[int]
     conversation_id: str
     message: str
     partial: bool
     parent_response_id: str
     def __init__(self, conversation_id: _Optional[str] = ..., message: _Optional[str] = ..., partial: bool = ..., parent_response_id: _Optional[str] = ...) -> None: ...
 
 class UpdateConversationRequest(_message.Message):
-    __slots__ = ("conversation_id", "title", "starred")
+    __slots__ = ["conversation_id", "title", "starred"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     TITLE_FIELD_NUMBER: _ClassVar[int]
     STARRED_FIELD_NUMBER: _ClassVar[int]
     conversation_id: str
     title: str
     starred: bool
     def __init__(self, conversation_id: _Optional[str] = ..., title: _Optional[str] = ..., starred: bool = ...) -> None: ...
 
 class SearchContext(_message.Message):
-    __slots__ = ("web_search_query", "web_formatted_chunks", "x_search_query", "x_formatted_chunks", "date")
+    __slots__ = ["web_search_query", "web_formatted_chunks", "x_search_query", "x_formatted_chunks", "date"]
     WEB_SEARCH_QUERY_FIELD_NUMBER: _ClassVar[int]
     WEB_FORMATTED_CHUNKS_FIELD_NUMBER: _ClassVar[int]
     X_SEARCH_QUERY_FIELD_NUMBER: _ClassVar[int]
     X_FORMATTED_CHUNKS_FIELD_NUMBER: _ClassVar[int]
     DATE_FIELD_NUMBER: _ClassVar[int]
     web_search_query: str
     web_formatted_chunks: str
     x_search_query: str
     x_formatted_chunks: str
     date: str
     def __init__(self, web_search_query: _Optional[str] = ..., web_formatted_chunks: _Optional[str] = ..., x_search_query: _Optional[str] = ..., x_formatted_chunks: _Optional[str] = ..., date: _Optional[str] = ...) -> None: ...
 
 class ResponseDebugLog(_message.Message):
-    __slots__ = ("system_prompt_name", "disable_search", "web_query", "x_query", "image_query", "prompt", "search_context")
+    __slots__ = ["system_prompt_name", "disable_search", "web_query", "x_query", "image_query", "prompt", "search_context"]
     SYSTEM_PROMPT_NAME_FIELD_NUMBER: _ClassVar[int]
     DISABLE_SEARCH_FIELD_NUMBER: _ClassVar[int]
     WEB_QUERY_FIELD_NUMBER: _ClassVar[int]
     X_QUERY_FIELD_NUMBER: _ClassVar[int]
     IMAGE_QUERY_FIELD_NUMBER: _ClassVar[int]
     PROMPT_FIELD_NUMBER: _ClassVar[int]
     SEARCH_CONTEXT_FIELD_NUMBER: _ClassVar[int]
@@ -106,44 +106,50 @@
     web_query: str
     x_query: str
     image_query: str
     prompt: str
     search_context: SearchContext
     def __init__(self, system_prompt_name: _Optional[str] = ..., disable_search: bool = ..., web_query: _Optional[str] = ..., x_query: _Optional[str] = ..., image_query: _Optional[str] = ..., prompt: _Optional[str] = ..., search_context: _Optional[_Union[SearchContext, _Mapping]] = ...) -> None: ...
 
+class AdditionalOptions(_message.Message):
+    __slots__ = ["injected_search_context", "temperature", "seed", "ignore_time_location"]
+    INJECTED_SEARCH_CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
+    SEED_FIELD_NUMBER: _ClassVar[int]
+    IGNORE_TIME_LOCATION_FIELD_NUMBER: _ClassVar[int]
+    injected_search_context: SearchContext
+    temperature: float
+    seed: int
+    ignore_time_location: bool
+    def __init__(self, injected_search_context: _Optional[_Union[SearchContext, _Mapping]] = ..., temperature: _Optional[float] = ..., seed: _Optional[int] = ..., ignore_time_location: bool = ...) -> None: ...
+
 class AddResponseRequest(_message.Message):
-    __slots__ = ("conversation_id", "message", "model_name", "parent_response_id", "system_prompt_name", "disable_search", "enable_image_generation", "force_rust", "injected_search_context", "temperature", "seed", "ignore_time_location")
+    __slots__ = ["conversation_id", "message", "model_name", "parent_response_id", "system_prompt_name", "disable_search", "enable_image_generation", "force_rust", "additional_options"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     PARENT_RESPONSE_ID_FIELD_NUMBER: _ClassVar[int]
     SYSTEM_PROMPT_NAME_FIELD_NUMBER: _ClassVar[int]
     DISABLE_SEARCH_FIELD_NUMBER: _ClassVar[int]
     ENABLE_IMAGE_GENERATION_FIELD_NUMBER: _ClassVar[int]
     FORCE_RUST_FIELD_NUMBER: _ClassVar[int]
-    INJECTED_SEARCH_CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
-    SEED_FIELD_NUMBER: _ClassVar[int]
-    IGNORE_TIME_LOCATION_FIELD_NUMBER: _ClassVar[int]
+    ADDITIONAL_OPTIONS_FIELD_NUMBER: _ClassVar[int]
     conversation_id: str
     message: str
     model_name: str
     parent_response_id: str
     system_prompt_name: str
     disable_search: bool
     enable_image_generation: bool
     force_rust: bool
-    injected_search_context: SearchContext
-    temperature: float
-    seed: int
-    ignore_time_location: bool
-    def __init__(self, conversation_id: _Optional[str] = ..., message: _Optional[str] = ..., model_name: _Optional[str] = ..., parent_response_id: _Optional[str] = ..., system_prompt_name: _Optional[str] = ..., disable_search: bool = ..., enable_image_generation: bool = ..., force_rust: bool = ..., injected_search_context: _Optional[_Union[SearchContext, _Mapping]] = ..., temperature: _Optional[float] = ..., seed: _Optional[int] = ..., ignore_time_location: bool = ...) -> None: ...
+    additional_options: AdditionalOptions
+    def __init__(self, conversation_id: _Optional[str] = ..., message: _Optional[str] = ..., model_name: _Optional[str] = ..., parent_response_id: _Optional[str] = ..., system_prompt_name: _Optional[str] = ..., disable_search: bool = ..., enable_image_generation: bool = ..., force_rust: bool = ..., additional_options: _Optional[_Union[AdditionalOptions, _Mapping]] = ...) -> None: ...
 
 class AddResponseResponse(_message.Message):
-    __slots__ = ("user_response", "token", "model_response", "query_action", "image_generation_response", "x_search_results", "cached_image_generation_response")
+    __slots__ = ["user_response", "token", "model_response", "query_action", "image_generation_response", "x_search_results", "cached_image_generation_response"]
     USER_RESPONSE_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     MODEL_RESPONSE_FIELD_NUMBER: _ClassVar[int]
     QUERY_ACTION_FIELD_NUMBER: _ClassVar[int]
     IMAGE_GENERATION_RESPONSE_FIELD_NUMBER: _ClassVar[int]
     X_SEARCH_RESULTS_FIELD_NUMBER: _ClassVar[int]
     CACHED_IMAGE_GENERATION_RESPONSE_FIELD_NUMBER: _ClassVar[int]
@@ -153,23 +159,23 @@
     query_action: QueryAction
     image_generation_response: ImageGenerationResponse
     x_search_results: _prod_search_pb2.XSearchResults
     cached_image_generation_response: CachedImageGenerationResponse
     def __init__(self, user_response: _Optional[_Union[Response, _Mapping]] = ..., token: _Optional[_Union[_sampler_public_pb2.SampleTokensResponse, _Mapping]] = ..., model_response: _Optional[_Union[Response, _Mapping]] = ..., query_action: _Optional[_Union[QueryAction, _Mapping]] = ..., image_generation_response: _Optional[_Union[ImageGenerationResponse, _Mapping]] = ..., x_search_results: _Optional[_Union[_prod_search_pb2.XSearchResults, _Mapping]] = ..., cached_image_generation_response: _Optional[_Union[CachedImageGenerationResponse, _Mapping]] = ...) -> None: ...
 
 class QueryAction(_message.Message):
-    __slots__ = ("query", "type")
+    __slots__ = ["query", "type"]
     QUERY_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     query: str
     type: str
     def __init__(self, query: _Optional[str] = ..., type: _Optional[str] = ...) -> None: ...
 
 class Conversation(_message.Message):
-    __slots__ = ("conversation_id", "title", "starred", "create_time", "modify_time", "responses", "system_prompt_name")
+    __slots__ = ["conversation_id", "title", "starred", "create_time", "modify_time", "responses", "system_prompt_name"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     TITLE_FIELD_NUMBER: _ClassVar[int]
     STARRED_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
     RESPONSES_FIELD_NUMBER: _ClassVar[int]
     SYSTEM_PROMPT_NAME_FIELD_NUMBER: _ClassVar[int]
@@ -179,15 +185,15 @@
     create_time: _timestamp_pb2.Timestamp
     modify_time: _timestamp_pb2.Timestamp
     responses: _containers.RepeatedCompositeFieldContainer[Response]
     system_prompt_name: str
     def __init__(self, conversation_id: _Optional[str] = ..., title: _Optional[str] = ..., starred: bool = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., modify_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., responses: _Optional[_Iterable[_Union[Response, _Mapping]]] = ..., system_prompt_name: _Optional[str] = ...) -> None: ...
 
 class Response(_message.Message):
-    __slots__ = ("response_id", "message", "sender", "create_time", "parent_response_id", "manual", "partial", "shared", "query", "query_type", "xpost_ids", "xposts", "generated_image_urls", "debug_log")
+    __slots__ = ["response_id", "message", "sender", "create_time", "parent_response_id", "manual", "partial", "shared", "query", "query_type", "xpost_ids", "xposts", "generated_image_urls", "debug_log"]
     RESPONSE_ID_FIELD_NUMBER: _ClassVar[int]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     SENDER_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     PARENT_RESPONSE_ID_FIELD_NUMBER: _ClassVar[int]
     MANUAL_FIELD_NUMBER: _ClassVar[int]
     PARTIAL_FIELD_NUMBER: _ClassVar[int]
@@ -211,33 +217,33 @@
     xpost_ids: _containers.RepeatedScalarFieldContainer[str]
     xposts: _containers.RepeatedCompositeFieldContainer[_x_entities_pb2.XPost]
     generated_image_urls: _containers.RepeatedScalarFieldContainer[str]
     debug_log: ResponseDebugLog
     def __init__(self, response_id: _Optional[str] = ..., message: _Optional[str] = ..., sender: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., parent_response_id: _Optional[str] = ..., manual: bool = ..., partial: bool = ..., shared: bool = ..., query: _Optional[str] = ..., query_type: _Optional[str] = ..., xpost_ids: _Optional[_Iterable[str]] = ..., xposts: _Optional[_Iterable[_Union[_x_entities_pb2.XPost, _Mapping]]] = ..., generated_image_urls: _Optional[_Iterable[str]] = ..., debug_log: _Optional[_Union[ResponseDebugLog, _Mapping]] = ...) -> None: ...
 
 class ImageGenerationResponse(_message.Message):
-    __slots__ = ("generated_image_bytes", "content_type")
+    __slots__ = ["generated_image_bytes", "content_type"]
     GENERATED_IMAGE_BYTES_FIELD_NUMBER: _ClassVar[int]
     CONTENT_TYPE_FIELD_NUMBER: _ClassVar[int]
     generated_image_bytes: bytes
     content_type: str
     def __init__(self, generated_image_bytes: _Optional[bytes] = ..., content_type: _Optional[str] = ...) -> None: ...
 
 class CachedImageGenerationResponse(_message.Message):
-    __slots__ = ("image_url",)
+    __slots__ = ["image_url"]
     IMAGE_URL_FIELD_NUMBER: _ClassVar[int]
     image_url: str
     def __init__(self, image_url: _Optional[str] = ...) -> None: ...
 
 class ShareConversationRequest(_message.Message):
-    __slots__ = ("conversation_id", "response_id")
+    __slots__ = ["conversation_id", "response_id"]
     CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_ID_FIELD_NUMBER: _ClassVar[int]
     conversation_id: str
     response_id: str
     def __init__(self, conversation_id: _Optional[str] = ..., response_id: _Optional[str] = ...) -> None: ...
 
 class ShareConversationResponse(_message.Message):
-    __slots__ = ("shared_id",)
+    __slots__ = ["shared_id"]
     SHARED_ID_FIELD_NUMBER: _ClassVar[int]
     shared_id: str
     def __init__(self, shared_id: _Optional[str] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/chat_pb2_grpc.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/files_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: files.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -19,14 +18,15 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0b\x66iles.proto\x12\nprompt_ide\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"]\n\x11UploadFileRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\x0c\x12\x11\n\tmime_type\x18\x03 \x01(\t\x12\x11\n\toverwrite\x18\x04 \x01(\x08\"y\n\x0c\x46ileMetadata\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x12\n\nsize_bytes\x18\x02 \x01(\x05\x12\x11\n\tmime_type\x18\x03 \x01(\t\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x11RenameFileRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x15\n\rnew_file_name\x18\x02 \x01(\t\"(\n\x13\x44ownloadFileRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t\"I\n\nFileObject\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.prompt_ide.FileMetadata\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\x0c\"s\n\x11ListFilesResponse\x12\x14\n\x0cstorage_used\x18\x01 \x01(\x05\x12\x1f\n\x17storage_available_total\x18\x02 \x01(\x05\x12\'\n\x05\x66iles\x18\x03 \x03(\x0b\x32\x18.prompt_ide.FileMetadata\"&\n\x11\x44\x65leteFileRequest\x12\x11\n\tfile_name\x18\x01 \x01(\t2\xf0\x02\n\x04\x46ile\x12G\n\nUploadFile\x12\x1d.prompt_ide.UploadFileRequest\x1a\x18.prompt_ide.FileMetadata\"\x00\x12I\n\x0c\x44ownloadFile\x12\x1f.prompt_ide.DownloadFileRequest\x1a\x16.prompt_ide.FileObject\"\x00\x12\x44\n\tListFiles\x12\x16.google.protobuf.Empty\x1a\x1d.prompt_ide.ListFilesResponse\"\x00\x12G\n\nRenameFile\x12\x1d.prompt_ide.RenameFileRequest\x1a\x18.prompt_ide.FileMetadata\"\x00\x12\x45\n\nDeleteFile\x12\x1d.prompt_ide.DeleteFileRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'files_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
+
   DESCRIPTOR._options = None
   _globals['_UPLOADFILEREQUEST']._serialized_start=89
   _globals['_UPLOADFILEREQUEST']._serialized_end=182
   _globals['_FILEMETADATA']._serialized_start=184
   _globals['_FILEMETADATA']._serialized_end=305
   _globals['_RENAMEFILEREQUEST']._serialized_start=307
   _globals['_RENAMEFILEREQUEST']._serialized_end=368
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2.pyi` & `xai_sdk-0.1.0/src/xai_sdk/proto/files_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,67 +4,67 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class UploadFileRequest(_message.Message):
-    __slots__ = ("file_name", "content", "mime_type", "overwrite")
+    __slots__ = ["file_name", "content", "mime_type", "overwrite"]
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
     OVERWRITE_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     content: bytes
     mime_type: str
     overwrite: bool
     def __init__(self, file_name: _Optional[str] = ..., content: _Optional[bytes] = ..., mime_type: _Optional[str] = ..., overwrite: bool = ...) -> None: ...
 
 class FileMetadata(_message.Message):
-    __slots__ = ("file_name", "size_bytes", "mime_type", "create_time")
+    __slots__ = ["file_name", "size_bytes", "mime_type", "create_time"]
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     SIZE_BYTES_FIELD_NUMBER: _ClassVar[int]
     MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     size_bytes: int
     mime_type: str
     create_time: _timestamp_pb2.Timestamp
     def __init__(self, file_name: _Optional[str] = ..., size_bytes: _Optional[int] = ..., mime_type: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class RenameFileRequest(_message.Message):
-    __slots__ = ("file_name", "new_file_name")
+    __slots__ = ["file_name", "new_file_name"]
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     NEW_FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     new_file_name: str
     def __init__(self, file_name: _Optional[str] = ..., new_file_name: _Optional[str] = ...) -> None: ...
 
 class DownloadFileRequest(_message.Message):
-    __slots__ = ("file_name",)
+    __slots__ = ["file_name"]
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     def __init__(self, file_name: _Optional[str] = ...) -> None: ...
 
 class FileObject(_message.Message):
-    __slots__ = ("metadata", "content")
+    __slots__ = ["metadata", "content"]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     metadata: FileMetadata
     content: bytes
     def __init__(self, metadata: _Optional[_Union[FileMetadata, _Mapping]] = ..., content: _Optional[bytes] = ...) -> None: ...
 
 class ListFilesResponse(_message.Message):
-    __slots__ = ("storage_used", "storage_available_total", "files")
+    __slots__ = ["storage_used", "storage_available_total", "files"]
     STORAGE_USED_FIELD_NUMBER: _ClassVar[int]
     STORAGE_AVAILABLE_TOTAL_FIELD_NUMBER: _ClassVar[int]
     FILES_FIELD_NUMBER: _ClassVar[int]
     storage_used: int
     storage_available_total: int
     files: _containers.RepeatedCompositeFieldContainer[FileMetadata]
     def __init__(self, storage_used: _Optional[int] = ..., storage_available_total: _Optional[int] = ..., files: _Optional[_Iterable[_Union[FileMetadata, _Mapping]]] = ...) -> None: ...
 
 class DeleteFileRequest(_message.Message):
-    __slots__ = ("file_name",)
+    __slots__ = ["file_name"]
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     file_name: str
     def __init__(self, file_name: _Optional[str] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/files_pb2_grpc.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/files_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/prod_search_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prod_search.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -20,14 +19,15 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11prod_search.proto\x12\nprompt_ide\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x10x_entities.proto\";\n\x18GetXCuratedTrendsRequest\x12\r\n\x05limit\x18\x01 \x01(\x05\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\"E\n\x19GetXCuratedTrendsResponse\x12(\n\x06trends\x18\x01 \x03(\x0b\x32\x18.prompt_ide.XTrendResult\"\"\n\x14GetXTrendByIdRequest\x12\n\n\x02id\x18\x01 \x01(\t\"@\n\x15GetXTrendByIdResponse\x12\'\n\x05trend\x18\x01 \x01(\x0b\x32\x18.prompt_ide.XTrendResult\"\xb2\x01\n\rSearchRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x15\n\rforce_refresh\x18\x02 \x01(\x08\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x0e\n\x06prompt\x18\x04 \x01(\t\x12\x11\n\tsearch_id\x18\x05 \x01(\t\x12\x17\n\x0f\x62\x61\x63kend_address\x18\x06 \x01(\t\x12\x12\n\nforce_rust\x18\x07 \x01(\x08\x12\x17\n\x0fimage_generator\x18\x08 \x01(\t\"\xe1\x02\n\x0eSearchResponse\x12\x36\n\x10x_search_results\x18\x01 \x01(\x0b\x32\x1a.prompt_ide.XSearchResultsH\x00\x12:\n\x12web_search_results\x18\x02 \x01(\x0b\x32\x1c.prompt_ide.WebSearchResultsH\x00\x12\x0e\n\x04text\x18\x03 \x01(\tH\x00\x12\x46\n\x18image_generation_results\x18\x04 \x01(\x0b\x32\".prompt_ide.ImageGenerationResultsH\x00\x12\x34\n\x0fx_trend_results\x18\x05 \x01(\x0b\x32\x19.prompt_ide.XTrendResultsH\x00\x12\x13\n\tsearch_id\x18\x06 \x01(\tH\x00\x12-\n\x05\x64\x65\x62ug\x18\x07 \x01(\x0b\x32\x1c.prompt_ide.DebugInformationH\x00\x42\t\n\x07payload\"4\n\x0eXSearchResults\x12\"\n\x07results\x18\x01 \x03(\x0b\x32\x11.prompt_ide.XPost\":\n\rXTrendResults\x12)\n\x07results\x18\x01 \x03(\x0b\x32\x18.prompt_ide.XTrendResult\"\xe6\x01\n\x0fWebSearchResult\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0f\n\x07preview\x18\x04 \x01(\t\x12\x1a\n\x12search_engine_text\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x11\n\tsite_name\x18\x07 \x01(\t\x12\x16\n\x0emetadata_title\x18\x08 \x01(\t\x12\x0f\n\x07\x63reator\x18\t \x01(\t\x12\r\n\x05image\x18\n \x01(\t\x12\x0f\n\x07\x66\x61vicon\x18\x0b \x01(\t\x12\x13\n\x0b\x63itation_id\x18\x0c \x01(\tJ\x04\x08\x03\x10\x04\"@\n\x10WebSearchResults\x12,\n\x07results\x18\x01 \x03(\x0b\x32\x1b.prompt_ide.WebSearchResult\":\n\x15ImageGenerationResult\x12\x11\n\timage_url\x18\x01 \x01(\t\x12\x0e\n\x06prompt\x18\x02 \x01(\t\"e\n\x16ImageGenerationResults\x12\x32\n\x07results\x18\x01 \x03(\x0b\x32!.prompt_ide.ImageGenerationResult\x12\x17\n\x0fimage_generator\x18\x02 \x01(\t\"F\n\x1fGetMostRecentSearchQueryRequest\x12\r\n\x05limit\x18\x01 \x01(\x05\x12\x14\n\x0cquery_prefix\x18\x02 \x01(\t\"/\n\x0bSearchQuery\x12\x11\n\tsearch_id\x18\x01 \x01(\t\x12\r\n\x05query\x18\x02 \x01(\t\"?\n\x13SearchQueryResponse\x12(\n\x07queries\x18\x01 \x03(\x0b\x32\x17.prompt_ide.SearchQuery\"-\n\x18\x44\x65leteSearchQueryRequest\x12\x11\n\tsearch_id\x18\x01 \x01(\t\"%\n\x14\x43ompleteQueryRequest\x12\r\n\x05query\x18\x01 \x01(\t\"&\n\x15\x43ompleteQueryResponse\x12\r\n\x05query\x18\x01 \x01(\t\"P\n\x19SummarizeWebResultRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x17\n\x0f\x62\x61\x63kend_address\x18\x03 \x01(\t\",\n\x1aSummarizeWebResultResponse\x12\x0e\n\x06\x61nswer\x18\x01 \x01(\t\"h\n\x17WebsiteDebugInformation\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08raw_html\x18\x02 \x01(\t\x12\x13\n\x0bparsed_text\x18\x03 \x01(\t\x12\x19\n\x11summarized_chunks\x18\x04 \x03(\t\"i\n\x10\x44\x65\x62ugInformation\x12\x1e\n\x16\x66ormatted_model_prompt\x18\x01 \x01(\t\x12\x35\n\x08websites\x18\x02 \x03(\x0b\x32#.prompt_ide.WebsiteDebugInformation2\x8b\x05\n\x06Search\x12\x43\n\x06Search\x12\x19.prompt_ide.SearchRequest\x1a\x1a.prompt_ide.SearchResponse\"\x00\x30\x01\x12j\n\x18GetMostRecentSearchQuery\x12+.prompt_ide.GetMostRecentSearchQueryRequest\x1a\x1f.prompt_ide.SearchQueryResponse\"\x00\x12S\n\x11\x44\x65leteSearchQuery\x12$.prompt_ide.DeleteSearchQueryRequest\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\rCompleteQuery\x12 .prompt_ide.CompleteQueryRequest\x1a!.prompt_ide.CompleteQueryResponse\"\x00\x12g\n\x12SummarizeWebResult\x12%.prompt_ide.SummarizeWebResultRequest\x1a&.prompt_ide.SummarizeWebResultResponse\"\x00\x30\x01\x12\x62\n\x11GetXCuratedTrends\x12$.prompt_ide.GetXCuratedTrendsRequest\x1a%.prompt_ide.GetXCuratedTrendsResponse\"\x00\x12V\n\rGetXTrendById\x12 .prompt_ide.GetXTrendByIdRequest\x1a!.prompt_ide.GetXTrendByIdResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prod_search_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
+
   DESCRIPTOR._options = None
   _globals['_GETXCURATEDTRENDSREQUEST']._serialized_start=113
   _globals['_GETXCURATEDTRENDSREQUEST']._serialized_end=172
   _globals['_GETXCURATEDTRENDSRESPONSE']._serialized_start=174
   _globals['_GETXCURATEDTRENDSRESPONSE']._serialized_end=243
   _globals['_GETXTRENDBYIDREQUEST']._serialized_start=245
   _globals['_GETXTRENDBYIDREQUEST']._serialized_end=279
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2.pyi` & `xai_sdk-0.1.0/src/xai_sdk/proto/prod_search_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class GetXCuratedTrendsRequest(_message.Message):
-    __slots__ = ("limit", "category")
+    __slots__ = ["limit", "category"]
     LIMIT_FIELD_NUMBER: _ClassVar[int]
     CATEGORY_FIELD_NUMBER: _ClassVar[int]
     limit: int
     category: str
     def __init__(self, limit: _Optional[int] = ..., category: _Optional[str] = ...) -> None: ...
 
 class GetXCuratedTrendsResponse(_message.Message):
-    __slots__ = ("trends",)
+    __slots__ = ["trends"]
     TRENDS_FIELD_NUMBER: _ClassVar[int]
     trends: _containers.RepeatedCompositeFieldContainer[_x_entities_pb2.XTrendResult]
     def __init__(self, trends: _Optional[_Iterable[_Union[_x_entities_pb2.XTrendResult, _Mapping]]] = ...) -> None: ...
 
 class GetXTrendByIdRequest(_message.Message):
-    __slots__ = ("id",)
+    __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: str
     def __init__(self, id: _Optional[str] = ...) -> None: ...
 
 class GetXTrendByIdResponse(_message.Message):
-    __slots__ = ("trend",)
+    __slots__ = ["trend"]
     TREND_FIELD_NUMBER: _ClassVar[int]
     trend: _x_entities_pb2.XTrendResult
     def __init__(self, trend: _Optional[_Union[_x_entities_pb2.XTrendResult, _Mapping]] = ...) -> None: ...
 
 class SearchRequest(_message.Message):
-    __slots__ = ("query", "force_refresh", "model_name", "prompt", "search_id", "backend_address", "force_rust", "image_generator")
+    __slots__ = ["query", "force_refresh", "model_name", "prompt", "search_id", "backend_address", "force_rust", "image_generator"]
     QUERY_FIELD_NUMBER: _ClassVar[int]
     FORCE_REFRESH_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     PROMPT_FIELD_NUMBER: _ClassVar[int]
     SEARCH_ID_FIELD_NUMBER: _ClassVar[int]
     BACKEND_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     FORCE_RUST_FIELD_NUMBER: _ClassVar[int]
@@ -51,15 +51,15 @@
     search_id: str
     backend_address: str
     force_rust: bool
     image_generator: str
     def __init__(self, query: _Optional[str] = ..., force_refresh: bool = ..., model_name: _Optional[str] = ..., prompt: _Optional[str] = ..., search_id: _Optional[str] = ..., backend_address: _Optional[str] = ..., force_rust: bool = ..., image_generator: _Optional[str] = ...) -> None: ...
 
 class SearchResponse(_message.Message):
-    __slots__ = ("x_search_results", "web_search_results", "text", "image_generation_results", "x_trend_results", "search_id", "debug")
+    __slots__ = ["x_search_results", "web_search_results", "text", "image_generation_results", "x_trend_results", "search_id", "debug"]
     X_SEARCH_RESULTS_FIELD_NUMBER: _ClassVar[int]
     WEB_SEARCH_RESULTS_FIELD_NUMBER: _ClassVar[int]
     TEXT_FIELD_NUMBER: _ClassVar[int]
     IMAGE_GENERATION_RESULTS_FIELD_NUMBER: _ClassVar[int]
     X_TREND_RESULTS_FIELD_NUMBER: _ClassVar[int]
     SEARCH_ID_FIELD_NUMBER: _ClassVar[int]
     DEBUG_FIELD_NUMBER: _ClassVar[int]
@@ -69,27 +69,27 @@
     image_generation_results: ImageGenerationResults
     x_trend_results: XTrendResults
     search_id: str
     debug: DebugInformation
     def __init__(self, x_search_results: _Optional[_Union[XSearchResults, _Mapping]] = ..., web_search_results: _Optional[_Union[WebSearchResults, _Mapping]] = ..., text: _Optional[str] = ..., image_generation_results: _Optional[_Union[ImageGenerationResults, _Mapping]] = ..., x_trend_results: _Optional[_Union[XTrendResults, _Mapping]] = ..., search_id: _Optional[str] = ..., debug: _Optional[_Union[DebugInformation, _Mapping]] = ...) -> None: ...
 
 class XSearchResults(_message.Message):
-    __slots__ = ("results",)
+    __slots__ = ["results"]
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     results: _containers.RepeatedCompositeFieldContainer[_x_entities_pb2.XPost]
     def __init__(self, results: _Optional[_Iterable[_Union[_x_entities_pb2.XPost, _Mapping]]] = ...) -> None: ...
 
 class XTrendResults(_message.Message):
-    __slots__ = ("results",)
+    __slots__ = ["results"]
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     results: _containers.RepeatedCompositeFieldContainer[_x_entities_pb2.XTrendResult]
     def __init__(self, results: _Optional[_Iterable[_Union[_x_entities_pb2.XTrendResult, _Mapping]]] = ...) -> None: ...
 
 class WebSearchResult(_message.Message):
-    __slots__ = ("url", "title", "preview", "search_engine_text", "description", "site_name", "metadata_title", "creator", "image", "favicon", "citation_id")
+    __slots__ = ["url", "title", "preview", "search_engine_text", "description", "site_name", "metadata_title", "creator", "image", "favicon", "citation_id"]
     URL_FIELD_NUMBER: _ClassVar[int]
     TITLE_FIELD_NUMBER: _ClassVar[int]
     PREVIEW_FIELD_NUMBER: _ClassVar[int]
     SEARCH_ENGINE_TEXT_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     SITE_NAME_FIELD_NUMBER: _ClassVar[int]
     METADATA_TITLE_FIELD_NUMBER: _ClassVar[int]
@@ -107,103 +107,103 @@
     creator: str
     image: str
     favicon: str
     citation_id: str
     def __init__(self, url: _Optional[str] = ..., title: _Optional[str] = ..., preview: _Optional[str] = ..., search_engine_text: _Optional[str] = ..., description: _Optional[str] = ..., site_name: _Optional[str] = ..., metadata_title: _Optional[str] = ..., creator: _Optional[str] = ..., image: _Optional[str] = ..., favicon: _Optional[str] = ..., citation_id: _Optional[str] = ...) -> None: ...
 
 class WebSearchResults(_message.Message):
-    __slots__ = ("results",)
+    __slots__ = ["results"]
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     results: _containers.RepeatedCompositeFieldContainer[WebSearchResult]
     def __init__(self, results: _Optional[_Iterable[_Union[WebSearchResult, _Mapping]]] = ...) -> None: ...
 
 class ImageGenerationResult(_message.Message):
-    __slots__ = ("image_url", "prompt")
+    __slots__ = ["image_url", "prompt"]
     IMAGE_URL_FIELD_NUMBER: _ClassVar[int]
     PROMPT_FIELD_NUMBER: _ClassVar[int]
     image_url: str
     prompt: str
     def __init__(self, image_url: _Optional[str] = ..., prompt: _Optional[str] = ...) -> None: ...
 
 class ImageGenerationResults(_message.Message):
-    __slots__ = ("results", "image_generator")
+    __slots__ = ["results", "image_generator"]
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     IMAGE_GENERATOR_FIELD_NUMBER: _ClassVar[int]
     results: _containers.RepeatedCompositeFieldContainer[ImageGenerationResult]
     image_generator: str
     def __init__(self, results: _Optional[_Iterable[_Union[ImageGenerationResult, _Mapping]]] = ..., image_generator: _Optional[str] = ...) -> None: ...
 
 class GetMostRecentSearchQueryRequest(_message.Message):
-    __slots__ = ("limit", "query_prefix")
+    __slots__ = ["limit", "query_prefix"]
     LIMIT_FIELD_NUMBER: _ClassVar[int]
     QUERY_PREFIX_FIELD_NUMBER: _ClassVar[int]
     limit: int
     query_prefix: str
     def __init__(self, limit: _Optional[int] = ..., query_prefix: _Optional[str] = ...) -> None: ...
 
 class SearchQuery(_message.Message):
-    __slots__ = ("search_id", "query")
+    __slots__ = ["search_id", "query"]
     SEARCH_ID_FIELD_NUMBER: _ClassVar[int]
     QUERY_FIELD_NUMBER: _ClassVar[int]
     search_id: str
     query: str
     def __init__(self, search_id: _Optional[str] = ..., query: _Optional[str] = ...) -> None: ...
 
 class SearchQueryResponse(_message.Message):
-    __slots__ = ("queries",)
+    __slots__ = ["queries"]
     QUERIES_FIELD_NUMBER: _ClassVar[int]
     queries: _containers.RepeatedCompositeFieldContainer[SearchQuery]
     def __init__(self, queries: _Optional[_Iterable[_Union[SearchQuery, _Mapping]]] = ...) -> None: ...
 
 class DeleteSearchQueryRequest(_message.Message):
-    __slots__ = ("search_id",)
+    __slots__ = ["search_id"]
     SEARCH_ID_FIELD_NUMBER: _ClassVar[int]
     search_id: str
     def __init__(self, search_id: _Optional[str] = ...) -> None: ...
 
 class CompleteQueryRequest(_message.Message):
-    __slots__ = ("query",)
+    __slots__ = ["query"]
     QUERY_FIELD_NUMBER: _ClassVar[int]
     query: str
     def __init__(self, query: _Optional[str] = ...) -> None: ...
 
 class CompleteQueryResponse(_message.Message):
-    __slots__ = ("query",)
+    __slots__ = ["query"]
     QUERY_FIELD_NUMBER: _ClassVar[int]
     query: str
     def __init__(self, query: _Optional[str] = ...) -> None: ...
 
 class SummarizeWebResultRequest(_message.Message):
-    __slots__ = ("query", "url", "backend_address")
+    __slots__ = ["query", "url", "backend_address"]
     QUERY_FIELD_NUMBER: _ClassVar[int]
     URL_FIELD_NUMBER: _ClassVar[int]
     BACKEND_ADDRESS_FIELD_NUMBER: _ClassVar[int]
     query: str
     url: str
     backend_address: str
     def __init__(self, query: _Optional[str] = ..., url: _Optional[str] = ..., backend_address: _Optional[str] = ...) -> None: ...
 
 class SummarizeWebResultResponse(_message.Message):
-    __slots__ = ("answer",)
+    __slots__ = ["answer"]
     ANSWER_FIELD_NUMBER: _ClassVar[int]
     answer: str
     def __init__(self, answer: _Optional[str] = ...) -> None: ...
 
 class WebsiteDebugInformation(_message.Message):
-    __slots__ = ("url", "raw_html", "parsed_text", "summarized_chunks")
+    __slots__ = ["url", "raw_html", "parsed_text", "summarized_chunks"]
     URL_FIELD_NUMBER: _ClassVar[int]
     RAW_HTML_FIELD_NUMBER: _ClassVar[int]
     PARSED_TEXT_FIELD_NUMBER: _ClassVar[int]
     SUMMARIZED_CHUNKS_FIELD_NUMBER: _ClassVar[int]
     url: str
     raw_html: str
     parsed_text: str
     summarized_chunks: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, url: _Optional[str] = ..., raw_html: _Optional[str] = ..., parsed_text: _Optional[str] = ..., summarized_chunks: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class DebugInformation(_message.Message):
-    __slots__ = ("formatted_model_prompt", "websites")
+    __slots__ = ["formatted_model_prompt", "websites"]
     FORMATTED_MODEL_PROMPT_FIELD_NUMBER: _ClassVar[int]
     WEBSITES_FIELD_NUMBER: _ClassVar[int]
     formatted_model_prompt: str
     websites: _containers.RepeatedCompositeFieldContainer[WebsiteDebugInformation]
     def __init__(self, formatted_model_prompt: _Optional[str] = ..., websites: _Optional[_Iterable[_Union[WebsiteDebugInformation, _Mapping]]] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/prod_search_pb2_grpc.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/prod_search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/sampler_public_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: sampler_public.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -20,28 +19,29 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14sampler_public.proto\x12\nprompt_ide\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xba\x01\n\x13SampleTokensRequest\x12\x12\n\x06prompt\x18\x01 \x03(\rB\x02\x18\x01\x12\'\n\x06inputs\x18\x07 \x03(\x0b\x32\x17.prompt_ide.PromptInput\x12,\n\x08settings\x18\x02 \x01(\x0b\x32\x1a.prompt_ide.SampleSettings\x12\x18\n\x10return_attention\x18\x04 \x01(\x08\x12\x12\n\nmodel_name\x18\x05 \x01(\tJ\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07\"\x82\x01\n\x0bPromptInput\x12\x0e\n\x04text\x18\x01 \x01(\tH\x00\x12\x15\n\x0bimage_bytes\x18\x02 \x01(\x0cH\x00\x12\x16\n\x0cimage_base64\x18\x03 \x01(\tH\x00\x12)\n\ttoken_ids\x18\x04 \x01(\x0b\x32\x14.prompt_ide.TokenIdsH\x00\x42\t\n\x07payload\"\x1a\n\x08TokenIds\x12\x0e\n\x06tokens\x18\x01 \x03(\r\"\xac\x01\n\x14SampleTokensResponse\x12\"\n\x05token\x18\x01 \x01(\x0b\x32\x11.prompt_ide.TokenH\x00\x12)\n\x06\x62udget\x18\x02 \x01(\x0b\x32\x17.prompt_ide.TokenBudgetH\x00\x12\x33\n\x0btransaction\x18\x04 \x01(\x0b\x32\x1c.prompt_ide.TokenTransactionH\x00\x42\n\n\x08responseJ\x04\x08\x03\x10\x04\"\x8a\x01\n\x1eTokenizeAndSampleTokensRequest\x12\x0c\n\x04text\x18\x01 \x01(\t\x12,\n\x08settings\x18\x02 \x01(\x0b\x32\x1a.prompt_ide.SampleSettings\x12\x18\n\x10return_attention\x18\x04 \x01(\x08\x12\x12\n\nmodel_name\x18\x05 \x01(\t\"\xe9\x01\n\x0eSampleSettings\x12\x0f\n\x07max_len\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x02\x12\x11\n\tnucleus_p\x18\x03 \x01(\x02\x12\x13\n\x0bstop_tokens\x18\x04 \x03(\t\x12\x14\n\x0cstop_strings\x18\x07 \x03(\t\x12\x10\n\x08rng_seed\x18\x05 \x01(\x04\x12.\n\x0e\x61llowed_tokens\x18\x06 \x03(\x0b\x32\x16.prompt_ide.InputToken\x12\x31\n\x11\x64isallowed_tokens\x18\x08 \x03(\x0b\x32\x16.prompt_ide.InputToken\"A\n\nInputToken\x12\x16\n\x0cstring_token\x18\x01 \x01(\tH\x00\x12\x12\n\x08token_id\x18\x02 \x01(\rH\x00\x42\x07\n\x05token\"\xca\x01\n\x05Token\x12&\n\x0b\x66inal_logit\x18\x01 \x01(\x0b\x32\x11.prompt_ide.Logit\x12 \n\x05top_k\x18\x04 \x03(\x0b\x32\x11.prompt_ide.Logit\x12\x11\n\tattention\x18\x05 \x03(\x02\x12/\n\ntoken_type\x18\x03 \x01(\x0e\x32\x1b.prompt_ide.Token.TokenType\"-\n\tTokenType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04USER\x10\x01\x12\t\n\x05MODEL\x10\x02J\x04\x08\x02\x10\x03\"=\n\x05Logit\x12\x10\n\x08token_id\x18\x01 \x01(\r\x12\x14\n\x0cstring_token\x18\x02 \x01(\t\x12\x0c\n\x04prob\x18\x03 \x01(\x02\"3\n\x0fTokenizeRequest\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\"5\n\x10TokenizeResponse\x12!\n\x06tokens\x18\x01 \x03(\x0b\x32\x11.prompt_ide.Token\"N\n\x18ListTransactionsResponse\x12\x32\n\x0ctransactions\x18\x01 \x03(\x0b\x32\x1c.prompt_ide.TokenTransaction\"\xee\x01\n\x10TokenTransaction\x12\x19\n\x11num_prompt_tokens\x18\x01 \x01(\x05\x12\x1c\n\x14num_generated_tokens\x18\x02 \x01(\x05\x12\x17\n\x0f\x63ost_multiplier\x18\x03 \x01(\x05\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10transaction_type\x18\x05 \x01(\t\x12\x16\n\x0etransaction_id\x18\x06 \x01(\t\x12\x12\n\nmodel_name\x18\x07 \x01(\t\x12\x11\n\tconfirmed\x18\x08 \x01(\x08\"1\n\x15GetTokenBudgetRequest\x12\x18\n\x10transaction_type\x18\x01 \x01(\t\"g\n\x0bTokenBudget\x12\x13\n\x0btoken_limit\x18\x01 \x01(\x05\x12\x14\n\x0ctokens_spent\x18\x02 \x01(\x05\x12\x15\n\rrequest_limit\x18\x03 \x01(\x05\x12\x16\n\x0erequests_spent\x18\x04 \x01(\x05\x32\xf9\x04\n\x07Sampler\x12{\n\x0cSampleTokens\x12\x1f.prompt_ide.SampleTokensRequest\x1a .prompt_ide.SampleTokensResponse\"&\x82\xd3\xe4\x93\x02 \"\x1b/rest/sampler/sample-tokens:\x01*0\x01\x12h\n\x08Tokenize\x12\x1b.prompt_ide.TokenizeRequest\x1a\x1c.prompt_ide.TokenizeResponse\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/rest/sampler/tokenize:\x01*\x12\x9e\x01\n\x17TokenizeAndSampleTokens\x12*.prompt_ide.TokenizeAndSampleTokensRequest\x1a .prompt_ide.SampleTokensResponse\"3\x82\xd3\xe4\x93\x02-\"(/rest/sampler/tokenize-and-sample-tokens:\x01*0\x01\x12t\n\x10ListTransactions\x12\x16.google.protobuf.Empty\x1a$.prompt_ide.ListTransactionsResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/rest/sampler/transactions\x12p\n\x0eGetTokenBudget\x12!.prompt_ide.GetTokenBudgetRequest\x1a\x17.prompt_ide.TokenBudget\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/rest/sampler/token-budgetB\x1cZ\x1ax.ai/prompt_ide;prompt_ideb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sampler_public_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'Z\032x.ai/prompt_ide;prompt_ide'
-  _globals['_SAMPLETOKENSREQUEST'].fields_by_name['prompt']._options = None
-  _globals['_SAMPLETOKENSREQUEST'].fields_by_name['prompt']._serialized_options = b'\030\001'
-  _globals['_SAMPLER'].methods_by_name['SampleTokens']._options = None
-  _globals['_SAMPLER'].methods_by_name['SampleTokens']._serialized_options = b'\202\323\344\223\002 \"\033/rest/sampler/sample-tokens:\001*'
-  _globals['_SAMPLER'].methods_by_name['Tokenize']._options = None
-  _globals['_SAMPLER'].methods_by_name['Tokenize']._serialized_options = b'\202\323\344\223\002\033\"\026/rest/sampler/tokenize:\001*'
-  _globals['_SAMPLER'].methods_by_name['TokenizeAndSampleTokens']._options = None
-  _globals['_SAMPLER'].methods_by_name['TokenizeAndSampleTokens']._serialized_options = b'\202\323\344\223\002-\"(/rest/sampler/tokenize-and-sample-tokens:\001*'
-  _globals['_SAMPLER'].methods_by_name['ListTransactions']._options = None
-  _globals['_SAMPLER'].methods_by_name['ListTransactions']._serialized_options = b'\202\323\344\223\002\034\022\032/rest/sampler/transactions'
-  _globals['_SAMPLER'].methods_by_name['GetTokenBudget']._options = None
-  _globals['_SAMPLER'].methods_by_name['GetTokenBudget']._serialized_options = b'\202\323\344\223\002\034\022\032/rest/sampler/token-budget'
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'Z\032x.ai/prompt_ide;prompt_ide'
+  _SAMPLETOKENSREQUEST.fields_by_name['prompt']._options = None
+  _SAMPLETOKENSREQUEST.fields_by_name['prompt']._serialized_options = b'\030\001'
+  _SAMPLER.methods_by_name['SampleTokens']._options = None
+  _SAMPLER.methods_by_name['SampleTokens']._serialized_options = b'\202\323\344\223\002 \"\033/rest/sampler/sample-tokens:\001*'
+  _SAMPLER.methods_by_name['Tokenize']._options = None
+  _SAMPLER.methods_by_name['Tokenize']._serialized_options = b'\202\323\344\223\002\033\"\026/rest/sampler/tokenize:\001*'
+  _SAMPLER.methods_by_name['TokenizeAndSampleTokens']._options = None
+  _SAMPLER.methods_by_name['TokenizeAndSampleTokens']._serialized_options = b'\202\323\344\223\002-\"(/rest/sampler/tokenize-and-sample-tokens:\001*'
+  _SAMPLER.methods_by_name['ListTransactions']._options = None
+  _SAMPLER.methods_by_name['ListTransactions']._serialized_options = b'\202\323\344\223\002\034\022\032/rest/sampler/transactions'
+  _SAMPLER.methods_by_name['GetTokenBudget']._options = None
+  _SAMPLER.methods_by_name['GetTokenBudget']._serialized_options = b'\202\323\344\223\002\034\022\032/rest/sampler/token-budget'
   _globals['_SAMPLETOKENSREQUEST']._serialized_start=129
   _globals['_SAMPLETOKENSREQUEST']._serialized_end=315
   _globals['_PROMPTINPUT']._serialized_start=318
   _globals['_PROMPTINPUT']._serialized_end=448
   _globals['_TOKENIDS']._serialized_start=450
   _globals['_TOKENIDS']._serialized_end=476
   _globals['_SAMPLETOKENSRESPONSE']._serialized_start=479
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2.pyi` & `xai_sdk-0.1.0/src/xai_sdk/proto/sampler_public_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -6,69 +6,69 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class SampleTokensRequest(_message.Message):
-    __slots__ = ("prompt", "inputs", "settings", "return_attention", "model_name")
+    __slots__ = ["prompt", "inputs", "settings", "return_attention", "model_name"]
     PROMPT_FIELD_NUMBER: _ClassVar[int]
     INPUTS_FIELD_NUMBER: _ClassVar[int]
     SETTINGS_FIELD_NUMBER: _ClassVar[int]
     RETURN_ATTENTION_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     prompt: _containers.RepeatedScalarFieldContainer[int]
     inputs: _containers.RepeatedCompositeFieldContainer[PromptInput]
     settings: SampleSettings
     return_attention: bool
     model_name: str
     def __init__(self, prompt: _Optional[_Iterable[int]] = ..., inputs: _Optional[_Iterable[_Union[PromptInput, _Mapping]]] = ..., settings: _Optional[_Union[SampleSettings, _Mapping]] = ..., return_attention: bool = ..., model_name: _Optional[str] = ...) -> None: ...
 
 class PromptInput(_message.Message):
-    __slots__ = ("text", "image_bytes", "image_base64", "token_ids")
+    __slots__ = ["text", "image_bytes", "image_base64", "token_ids"]
     TEXT_FIELD_NUMBER: _ClassVar[int]
     IMAGE_BYTES_FIELD_NUMBER: _ClassVar[int]
     IMAGE_BASE64_FIELD_NUMBER: _ClassVar[int]
     TOKEN_IDS_FIELD_NUMBER: _ClassVar[int]
     text: str
     image_bytes: bytes
     image_base64: str
     token_ids: TokenIds
     def __init__(self, text: _Optional[str] = ..., image_bytes: _Optional[bytes] = ..., image_base64: _Optional[str] = ..., token_ids: _Optional[_Union[TokenIds, _Mapping]] = ...) -> None: ...
 
 class TokenIds(_message.Message):
-    __slots__ = ("tokens",)
+    __slots__ = ["tokens"]
     TOKENS_FIELD_NUMBER: _ClassVar[int]
     tokens: _containers.RepeatedScalarFieldContainer[int]
     def __init__(self, tokens: _Optional[_Iterable[int]] = ...) -> None: ...
 
 class SampleTokensResponse(_message.Message):
-    __slots__ = ("token", "budget", "transaction")
+    __slots__ = ["token", "budget", "transaction"]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     BUDGET_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_FIELD_NUMBER: _ClassVar[int]
     token: Token
     budget: TokenBudget
     transaction: TokenTransaction
     def __init__(self, token: _Optional[_Union[Token, _Mapping]] = ..., budget: _Optional[_Union[TokenBudget, _Mapping]] = ..., transaction: _Optional[_Union[TokenTransaction, _Mapping]] = ...) -> None: ...
 
 class TokenizeAndSampleTokensRequest(_message.Message):
-    __slots__ = ("text", "settings", "return_attention", "model_name")
+    __slots__ = ["text", "settings", "return_attention", "model_name"]
     TEXT_FIELD_NUMBER: _ClassVar[int]
     SETTINGS_FIELD_NUMBER: _ClassVar[int]
     RETURN_ATTENTION_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     text: str
     settings: SampleSettings
     return_attention: bool
     model_name: str
     def __init__(self, text: _Optional[str] = ..., settings: _Optional[_Union[SampleSettings, _Mapping]] = ..., return_attention: bool = ..., model_name: _Optional[str] = ...) -> None: ...
 
 class SampleSettings(_message.Message):
-    __slots__ = ("max_len", "temperature", "nucleus_p", "stop_tokens", "stop_strings", "rng_seed", "allowed_tokens", "disallowed_tokens")
+    __slots__ = ["max_len", "temperature", "nucleus_p", "stop_tokens", "stop_strings", "rng_seed", "allowed_tokens", "disallowed_tokens"]
     MAX_LEN_FIELD_NUMBER: _ClassVar[int]
     TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
     NUCLEUS_P_FIELD_NUMBER: _ClassVar[int]
     STOP_TOKENS_FIELD_NUMBER: _ClassVar[int]
     STOP_STRINGS_FIELD_NUMBER: _ClassVar[int]
     RNG_SEED_FIELD_NUMBER: _ClassVar[int]
     ALLOWED_TOKENS_FIELD_NUMBER: _ClassVar[int]
@@ -80,25 +80,25 @@
     stop_strings: _containers.RepeatedScalarFieldContainer[str]
     rng_seed: int
     allowed_tokens: _containers.RepeatedCompositeFieldContainer[InputToken]
     disallowed_tokens: _containers.RepeatedCompositeFieldContainer[InputToken]
     def __init__(self, max_len: _Optional[int] = ..., temperature: _Optional[float] = ..., nucleus_p: _Optional[float] = ..., stop_tokens: _Optional[_Iterable[str]] = ..., stop_strings: _Optional[_Iterable[str]] = ..., rng_seed: _Optional[int] = ..., allowed_tokens: _Optional[_Iterable[_Union[InputToken, _Mapping]]] = ..., disallowed_tokens: _Optional[_Iterable[_Union[InputToken, _Mapping]]] = ...) -> None: ...
 
 class InputToken(_message.Message):
-    __slots__ = ("string_token", "token_id")
+    __slots__ = ["string_token", "token_id"]
     STRING_TOKEN_FIELD_NUMBER: _ClassVar[int]
     TOKEN_ID_FIELD_NUMBER: _ClassVar[int]
     string_token: str
     token_id: int
     def __init__(self, string_token: _Optional[str] = ..., token_id: _Optional[int] = ...) -> None: ...
 
 class Token(_message.Message):
-    __slots__ = ("final_logit", "top_k", "attention", "token_type")
+    __slots__ = ["final_logit", "top_k", "attention", "token_type"]
     class TokenType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = ()
+        __slots__ = []
         UNKNOWN: _ClassVar[Token.TokenType]
         USER: _ClassVar[Token.TokenType]
         MODEL: _ClassVar[Token.TokenType]
     UNKNOWN: Token.TokenType
     USER: Token.TokenType
     MODEL: Token.TokenType
     FINAL_LOGIT_FIELD_NUMBER: _ClassVar[int]
@@ -108,45 +108,45 @@
     final_logit: Logit
     top_k: _containers.RepeatedCompositeFieldContainer[Logit]
     attention: _containers.RepeatedScalarFieldContainer[float]
     token_type: Token.TokenType
     def __init__(self, final_logit: _Optional[_Union[Logit, _Mapping]] = ..., top_k: _Optional[_Iterable[_Union[Logit, _Mapping]]] = ..., attention: _Optional[_Iterable[float]] = ..., token_type: _Optional[_Union[Token.TokenType, str]] = ...) -> None: ...
 
 class Logit(_message.Message):
-    __slots__ = ("token_id", "string_token", "prob")
+    __slots__ = ["token_id", "string_token", "prob"]
     TOKEN_ID_FIELD_NUMBER: _ClassVar[int]
     STRING_TOKEN_FIELD_NUMBER: _ClassVar[int]
     PROB_FIELD_NUMBER: _ClassVar[int]
     token_id: int
     string_token: str
     prob: float
     def __init__(self, token_id: _Optional[int] = ..., string_token: _Optional[str] = ..., prob: _Optional[float] = ...) -> None: ...
 
 class TokenizeRequest(_message.Message):
-    __slots__ = ("text", "model_name")
+    __slots__ = ["text", "model_name"]
     TEXT_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     text: str
     model_name: str
     def __init__(self, text: _Optional[str] = ..., model_name: _Optional[str] = ...) -> None: ...
 
 class TokenizeResponse(_message.Message):
-    __slots__ = ("tokens",)
+    __slots__ = ["tokens"]
     TOKENS_FIELD_NUMBER: _ClassVar[int]
     tokens: _containers.RepeatedCompositeFieldContainer[Token]
     def __init__(self, tokens: _Optional[_Iterable[_Union[Token, _Mapping]]] = ...) -> None: ...
 
 class ListTransactionsResponse(_message.Message):
-    __slots__ = ("transactions",)
+    __slots__ = ["transactions"]
     TRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
     transactions: _containers.RepeatedCompositeFieldContainer[TokenTransaction]
     def __init__(self, transactions: _Optional[_Iterable[_Union[TokenTransaction, _Mapping]]] = ...) -> None: ...
 
 class TokenTransaction(_message.Message):
-    __slots__ = ("num_prompt_tokens", "num_generated_tokens", "cost_multiplier", "create_time", "transaction_type", "transaction_id", "model_name", "confirmed")
+    __slots__ = ["num_prompt_tokens", "num_generated_tokens", "cost_multiplier", "create_time", "transaction_type", "transaction_id", "model_name", "confirmed"]
     NUM_PROMPT_TOKENS_FIELD_NUMBER: _ClassVar[int]
     NUM_GENERATED_TOKENS_FIELD_NUMBER: _ClassVar[int]
     COST_MULTIPLIER_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_TYPE_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_ID_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
@@ -158,21 +158,21 @@
     transaction_type: str
     transaction_id: str
     model_name: str
     confirmed: bool
     def __init__(self, num_prompt_tokens: _Optional[int] = ..., num_generated_tokens: _Optional[int] = ..., cost_multiplier: _Optional[int] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., transaction_type: _Optional[str] = ..., transaction_id: _Optional[str] = ..., model_name: _Optional[str] = ..., confirmed: bool = ...) -> None: ...
 
 class GetTokenBudgetRequest(_message.Message):
-    __slots__ = ("transaction_type",)
+    __slots__ = ["transaction_type"]
     TRANSACTION_TYPE_FIELD_NUMBER: _ClassVar[int]
     transaction_type: str
     def __init__(self, transaction_type: _Optional[str] = ...) -> None: ...
 
 class TokenBudget(_message.Message):
-    __slots__ = ("token_limit", "tokens_spent", "request_limit", "requests_spent")
+    __slots__ = ["token_limit", "tokens_spent", "request_limit", "requests_spent"]
     TOKEN_LIMIT_FIELD_NUMBER: _ClassVar[int]
     TOKENS_SPENT_FIELD_NUMBER: _ClassVar[int]
     REQUEST_LIMIT_FIELD_NUMBER: _ClassVar[int]
     REQUESTS_SPENT_FIELD_NUMBER: _ClassVar[int]
     token_limit: int
     tokens_spent: int
     request_limit: int
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/sampler_public_pb2_grpc.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/sampler_public_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/stateless_chat_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: stateless_chat.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -19,22 +18,23 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14stateless_chat.proto\x12\nprompt_ide\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\"\xb0\x02\n\x15StatelessConversation\x12!\n\x19stateless_conversation_id\x18\x05 \x01(\t\x12\x30\n\tresponses\x18\x01 \x03(\x0b\x32\x1d.prompt_ide.StatelessResponse\x12\x1a\n\x12system_prompt_name\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08username\x18\x04 \x01(\t\x12\x1f\n\x17\x65xpose_username_to_grok\x18\x06 \x01(\x08\x12\x16\n\x0e\x64isable_search\x18\x07 \x01(\x08\x12\x1f\n\x17\x65nable_image_generation\x18\x08 \x01(\x08\x12\x12\n\nmodel_name\x18\t \x01(\t\x12\x18\n\x10x_posts_as_field\x18\n \x01(\x08\"\x99\x02\n\x11StatelessResponse\x12\x34\n\x06sender\x18\x01 \x01(\x0e\x32$.prompt_ide.StatelessResponse.Sender\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05query\x18\x03 \x01(\t\x12\x12\n\nquery_type\x18\x05 \x01(\t\x12:\n\x10image_attachment\x18\x06 \x01(\x0b\x32\x1b.prompt_ide.ImageAttachmentH\x00\x88\x01\x01\x12\x12\n\nx_post_ids\x18\x07 \x03(\t\"/\n\x06Sender\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05HUMAN\x10\x01\x12\r\n\tASSISTANT\x10\x02\x42\x13\n\x11_image_attachmentJ\x04\x08\x04\x10\x05\"<\n\x0fImageAttachment\x12\x13\n\x0bimage_bytes\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\":\n DeleteLoggedConversationsRequest\x12\x16\n\x0e\x61\x63\x63ounting_key\x18\x01 \x01(\t2\xa8\x03\n\rStatelessChat\x12\x7f\n\x0b\x41\x64\x64Response\x12!.prompt_ide.StatelessConversation\x1a\x1d.prompt_ide.StatelessResponse\",\x82\xd3\xe4\x93\x02&\"!/rest/stateless-chat/add-response:\x01*0\x01\x12\x7f\n\x0fLogForDebugging\x12!.prompt_ide.StatelessConversation\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+\"&/rest/stateless-chat/log-for-debugging:\x01*\x12\x94\x01\n\x19\x44\x65leteLoggedConversations\x12,.prompt_ide.DeleteLoggedConversationsRequest\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+*)/rest/stateless-chat/logged-conversationsB\x1cZ\x1ax.ai/prompt_ide;prompt_ideb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stateless_chat_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'Z\032x.ai/prompt_ide;prompt_ide'
-  _globals['_STATELESSCHAT'].methods_by_name['AddResponse']._options = None
-  _globals['_STATELESSCHAT'].methods_by_name['AddResponse']._serialized_options = b'\202\323\344\223\002&\"!/rest/stateless-chat/add-response:\001*'
-  _globals['_STATELESSCHAT'].methods_by_name['LogForDebugging']._options = None
-  _globals['_STATELESSCHAT'].methods_by_name['LogForDebugging']._serialized_options = b'\202\323\344\223\002+\"&/rest/stateless-chat/log-for-debugging:\001*'
-  _globals['_STATELESSCHAT'].methods_by_name['DeleteLoggedConversations']._options = None
-  _globals['_STATELESSCHAT'].methods_by_name['DeleteLoggedConversations']._serialized_options = b'\202\323\344\223\002+*)/rest/stateless-chat/logged-conversations'
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'Z\032x.ai/prompt_ide;prompt_ide'
+  _STATELESSCHAT.methods_by_name['AddResponse']._options = None
+  _STATELESSCHAT.methods_by_name['AddResponse']._serialized_options = b'\202\323\344\223\002&\"!/rest/stateless-chat/add-response:\001*'
+  _STATELESSCHAT.methods_by_name['LogForDebugging']._options = None
+  _STATELESSCHAT.methods_by_name['LogForDebugging']._serialized_options = b'\202\323\344\223\002+\"&/rest/stateless-chat/log-for-debugging:\001*'
+  _STATELESSCHAT.methods_by_name['DeleteLoggedConversations']._options = None
+  _STATELESSCHAT.methods_by_name['DeleteLoggedConversations']._serialized_options = b'\202\323\344\223\002+*)/rest/stateless-chat/logged-conversations'
   _globals['_STATELESSCONVERSATION']._serialized_start=96
   _globals['_STATELESSCONVERSATION']._serialized_end=400
   _globals['_STATELESSRESPONSE']._serialized_start=403
   _globals['_STATELESSRESPONSE']._serialized_end=684
   _globals['_STATELESSRESPONSE_SENDER']._serialized_start=610
   _globals['_STATELESSRESPONSE_SENDER']._serialized_end=657
   _globals['_IMAGEATTACHMENT']._serialized_start=686
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2.pyi` & `xai_sdk-0.1.0/src/xai_sdk/proto/stateless_chat_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class StatelessConversation(_message.Message):
-    __slots__ = ("stateless_conversation_id", "responses", "system_prompt_name", "name", "username", "expose_username_to_grok", "disable_search", "enable_image_generation", "model_name", "x_posts_as_field")
+    __slots__ = ["stateless_conversation_id", "responses", "system_prompt_name", "name", "username", "expose_username_to_grok", "disable_search", "enable_image_generation", "model_name", "x_posts_as_field"]
     STATELESS_CONVERSATION_ID_FIELD_NUMBER: _ClassVar[int]
     RESPONSES_FIELD_NUMBER: _ClassVar[int]
     SYSTEM_PROMPT_NAME_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     USERNAME_FIELD_NUMBER: _ClassVar[int]
     EXPOSE_USERNAME_TO_GROK_FIELD_NUMBER: _ClassVar[int]
     DISABLE_SEARCH_FIELD_NUMBER: _ClassVar[int]
@@ -29,17 +29,17 @@
     disable_search: bool
     enable_image_generation: bool
     model_name: str
     x_posts_as_field: bool
     def __init__(self, stateless_conversation_id: _Optional[str] = ..., responses: _Optional[_Iterable[_Union[StatelessResponse, _Mapping]]] = ..., system_prompt_name: _Optional[str] = ..., name: _Optional[str] = ..., username: _Optional[str] = ..., expose_username_to_grok: bool = ..., disable_search: bool = ..., enable_image_generation: bool = ..., model_name: _Optional[str] = ..., x_posts_as_field: bool = ...) -> None: ...
 
 class StatelessResponse(_message.Message):
-    __slots__ = ("sender", "message", "query", "query_type", "image_attachment", "x_post_ids")
+    __slots__ = ["sender", "message", "query", "query_type", "image_attachment", "x_post_ids"]
     class Sender(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = ()
+        __slots__ = []
         UNKNOWN: _ClassVar[StatelessResponse.Sender]
         HUMAN: _ClassVar[StatelessResponse.Sender]
         ASSISTANT: _ClassVar[StatelessResponse.Sender]
     UNKNOWN: StatelessResponse.Sender
     HUMAN: StatelessResponse.Sender
     ASSISTANT: StatelessResponse.Sender
     SENDER_FIELD_NUMBER: _ClassVar[int]
@@ -53,19 +53,19 @@
     query: str
     query_type: str
     image_attachment: ImageAttachment
     x_post_ids: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, sender: _Optional[_Union[StatelessResponse.Sender, str]] = ..., message: _Optional[str] = ..., query: _Optional[str] = ..., query_type: _Optional[str] = ..., image_attachment: _Optional[_Union[ImageAttachment, _Mapping]] = ..., x_post_ids: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class ImageAttachment(_message.Message):
-    __slots__ = ("image_bytes", "content_type")
+    __slots__ = ["image_bytes", "content_type"]
     IMAGE_BYTES_FIELD_NUMBER: _ClassVar[int]
     CONTENT_TYPE_FIELD_NUMBER: _ClassVar[int]
     image_bytes: bytes
     content_type: str
     def __init__(self, image_bytes: _Optional[bytes] = ..., content_type: _Optional[str] = ...) -> None: ...
 
 class DeleteLoggedConversationsRequest(_message.Message):
-    __slots__ = ("accounting_key",)
+    __slots__ = ["accounting_key"]
     ACCOUNTING_KEY_FIELD_NUMBER: _ClassVar[int]
     accounting_key: str
     def __init__(self, accounting_key: _Optional[str] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/stateless_chat_pb2_grpc.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/stateless_chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/x_entities_pb2.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/x_entities_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: x_entities.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -18,14 +17,15 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10x_entities.proto\x12\nprompt_ide\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd0\x02\n\x05XPost\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04text\x18\x03 \x01(\t\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11profile_image_url\x18\x05 \x01(\t\x12\x0f\n\x07post_id\x18\x06 \x01(\t\x12\x13\n\x0b\x63itation_id\x18\x08 \x01(\t\x12!\n\x06parent\x18\t \x01(\x0b\x32\x11.prompt_ide.XPost\x12\x1b\n\x0eparent_post_id\x18\n \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rquote_post_id\x18\x0b \x01(\tH\x01\x88\x01\x01\x12 \n\x05quote\x18\x0c \x01(\x0b\x32\x11.prompt_ide.XPostB\x11\n\x0f_parent_post_idB\x10\n\x0e_quote_post_idJ\x04\x08\x07\x10\x08\"\x87\x02\n\nXTrendPost\x12\x15\n\rauthor_handle\x18\x01 \x01(\t\x12\x13\n\x0b\x61uthor_name\x18\x02 \x01(\t\x12\x15\n\rauthor_avatar\x18\x03 \x01(\t\x12\x19\n\x11\x61uthor_nfollowers\x18\x04 \x01(\x05\x12\x0f\n\x07rest_id\x18\x05 \x01(\t\x12\x10\n\x08nreplies\x18\x06 \x01(\x05\x12\x0c\n\x04text\x18\x07 \x01(\t\x12\x12\n\ncreated_ts\x18\x08 \x01(\x03\x12\x10\n\x08nreposts\x18\t \x01(\x05\x12\x0c\n\x04imgs\x18\n \x03(\t\x12\x0c\n\x04vids\x18\x0b \x03(\t\x12(\n\x04\x63\x61rd\x18\x0c \x01(\x0b\x32\x1a.prompt_ide.XTrendPostCard\"\x96\x01\n\x0cXTrendResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04hook\x18\x02 \x01(\t\x12\x0f\n\x07summary\x18\x03 \x01(\t\x12\x0f\n\x07rest_id\x18\x04 \x01(\t\x12%\n\x05posts\x18\x05 \x03(\x0b\x32\x16.prompt_ide.XTrendPost\x12\x11\n\tthumbnail\x18\x06 \x01(\t\x12\x0e\n\x06header\x18\x07 \x01(\t\"*\n\x0eXTrendPostCard\x12\x0b\n\x03img\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'x_entities_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
+
   DESCRIPTOR._options = None
   _globals['_XPOST']._serialized_start=66
   _globals['_XPOST']._serialized_end=402
   _globals['_XTRENDPOST']._serialized_start=405
   _globals['_XTRENDPOST']._serialized_end=668
   _globals['_XTRENDRESULT']._serialized_start=671
   _globals['_XTRENDRESULT']._serialized_end=821
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/x_entities_pb2.pyi` & `xai_sdk-0.1.0/src/xai_sdk/proto/x_entities_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class XPost(_message.Message):
-    __slots__ = ("username", "name", "text", "create_time", "profile_image_url", "post_id", "citation_id", "parent", "parent_post_id", "quote_post_id", "quote")
+    __slots__ = ["username", "name", "text", "create_time", "profile_image_url", "post_id", "citation_id", "parent", "parent_post_id", "quote_post_id", "quote"]
     USERNAME_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     TEXT_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     PROFILE_IMAGE_URL_FIELD_NUMBER: _ClassVar[int]
     POST_ID_FIELD_NUMBER: _ClassVar[int]
     CITATION_ID_FIELD_NUMBER: _ClassVar[int]
@@ -29,15 +29,15 @@
     parent: XPost
     parent_post_id: str
     quote_post_id: str
     quote: XPost
     def __init__(self, username: _Optional[str] = ..., name: _Optional[str] = ..., text: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., profile_image_url: _Optional[str] = ..., post_id: _Optional[str] = ..., citation_id: _Optional[str] = ..., parent: _Optional[_Union[XPost, _Mapping]] = ..., parent_post_id: _Optional[str] = ..., quote_post_id: _Optional[str] = ..., quote: _Optional[_Union[XPost, _Mapping]] = ...) -> None: ...
 
 class XTrendPost(_message.Message):
-    __slots__ = ("author_handle", "author_name", "author_avatar", "author_nfollowers", "rest_id", "nreplies", "text", "created_ts", "nreposts", "imgs", "vids", "card")
+    __slots__ = ["author_handle", "author_name", "author_avatar", "author_nfollowers", "rest_id", "nreplies", "text", "created_ts", "nreposts", "imgs", "vids", "card"]
     AUTHOR_HANDLE_FIELD_NUMBER: _ClassVar[int]
     AUTHOR_NAME_FIELD_NUMBER: _ClassVar[int]
     AUTHOR_AVATAR_FIELD_NUMBER: _ClassVar[int]
     AUTHOR_NFOLLOWERS_FIELD_NUMBER: _ClassVar[int]
     REST_ID_FIELD_NUMBER: _ClassVar[int]
     NREPLIES_FIELD_NUMBER: _ClassVar[int]
     TEXT_FIELD_NUMBER: _ClassVar[int]
@@ -57,15 +57,15 @@
     nreposts: int
     imgs: _containers.RepeatedScalarFieldContainer[str]
     vids: _containers.RepeatedScalarFieldContainer[str]
     card: XTrendPostCard
     def __init__(self, author_handle: _Optional[str] = ..., author_name: _Optional[str] = ..., author_avatar: _Optional[str] = ..., author_nfollowers: _Optional[int] = ..., rest_id: _Optional[str] = ..., nreplies: _Optional[int] = ..., text: _Optional[str] = ..., created_ts: _Optional[int] = ..., nreposts: _Optional[int] = ..., imgs: _Optional[_Iterable[str]] = ..., vids: _Optional[_Iterable[str]] = ..., card: _Optional[_Union[XTrendPostCard, _Mapping]] = ...) -> None: ...
 
 class XTrendResult(_message.Message):
-    __slots__ = ("name", "hook", "summary", "rest_id", "posts", "thumbnail", "header")
+    __slots__ = ["name", "hook", "summary", "rest_id", "posts", "thumbnail", "header"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     HOOK_FIELD_NUMBER: _ClassVar[int]
     SUMMARY_FIELD_NUMBER: _ClassVar[int]
     REST_ID_FIELD_NUMBER: _ClassVar[int]
     POSTS_FIELD_NUMBER: _ClassVar[int]
     THUMBNAIL_FIELD_NUMBER: _ClassVar[int]
     HEADER_FIELD_NUMBER: _ClassVar[int]
@@ -75,13 +75,13 @@
     rest_id: str
     posts: _containers.RepeatedCompositeFieldContainer[XTrendPost]
     thumbnail: str
     header: str
     def __init__(self, name: _Optional[str] = ..., hook: _Optional[str] = ..., summary: _Optional[str] = ..., rest_id: _Optional[str] = ..., posts: _Optional[_Iterable[_Union[XTrendPost, _Mapping]]] = ..., thumbnail: _Optional[str] = ..., header: _Optional[str] = ...) -> None: ...
 
 class XTrendPostCard(_message.Message):
-    __slots__ = ("img", "url")
+    __slots__ = ["img", "url"]
     IMG_FIELD_NUMBER: _ClassVar[int]
     URL_FIELD_NUMBER: _ClassVar[int]
     img: str
     url: str
     def __init__(self, img: _Optional[str] = ..., url: _Optional[str] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/google/api/annotations_pb2.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/google/api/annotations_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/annotations.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -19,10 +18,12 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cgoogle/api/annotations.proto\x12\ngoogle.api\x1a\x15google/api/http.proto\x1a google/protobuf/descriptor.proto:E\n\x04http\x12\x1e.google.protobuf.MethodOptions\x18\xb0\xca\xbc\" \x01(\x0b\x32\x14.google.api.HttpRuleBn\n\x0e\x63om.google.apiB\x10\x41nnotationsProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.annotations_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.google.apiB\020AnnotationsProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
+  google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(http)
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\020AnnotationsProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\242\002\004GAPI'
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2.py` & `xai_sdk-0.1.0/src/xai_sdk/proto/google/api/http_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # fmt: off
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: google/api/http.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,16 +16,17 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15google/api/http.proto\x12\ngoogle.api\"+\n\x04Http\x12#\n\x05rules\x18\x01 \x03(\x0b\x32\x14.google.api.HttpRule\"\xea\x01\n\x08HttpRule\x12\x10\n\x08selector\x18\x01 \x01(\t\x12\r\n\x03get\x18\x02 \x01(\tH\x00\x12\r\n\x03put\x18\x03 \x01(\tH\x00\x12\x0e\n\x04post\x18\x04 \x01(\tH\x00\x12\x10\n\x06\x64\x65lete\x18\x05 \x01(\tH\x00\x12\x0f\n\x05patch\x18\x06 \x01(\tH\x00\x12/\n\x06\x63ustom\x18\x08 \x01(\x0b\x32\x1d.google.api.CustomHttpPatternH\x00\x12\x0c\n\x04\x62ody\x18\x07 \x01(\t\x12\x31\n\x13\x61\x64\x64itional_bindings\x18\x0b \x03(\x0b\x32\x14.google.api.HttpRuleB\t\n\x07pattern\"/\n\x11\x43ustomHttpPattern\x12\x0c\n\x04kind\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\tBj\n\x0e\x63om.google.apiB\tHttpProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xf8\x01\x01\xa2\x02\x04GAPIb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'google.api.http_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.google.apiB\tHttpProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\370\001\001\242\002\004GAPI'
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n\016com.google.apiB\tHttpProtoP\001ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\370\001\001\242\002\004GAPI'
   _globals['_HTTP']._serialized_start=37
   _globals['_HTTP']._serialized_end=80
   _globals['_HTTPRULE']._serialized_start=83
   _globals['_HTTPRULE']._serialized_end=317
   _globals['_CUSTOMHTTPPATTERN']._serialized_start=319
   _globals['_CUSTOMHTTPPATTERN']._serialized_end=366
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xai_sdk-0.0.5/src/xai_sdk/proto/google/api/http_pb2.pyi` & `xai_sdk-0.1.0/src/xai_sdk/proto/google/api/http_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Http(_message.Message):
-    __slots__ = ("rules",)
+    __slots__ = ["rules"]
     RULES_FIELD_NUMBER: _ClassVar[int]
     rules: _containers.RepeatedCompositeFieldContainer[HttpRule]
     def __init__(self, rules: _Optional[_Iterable[_Union[HttpRule, _Mapping]]] = ...) -> None: ...
 
 class HttpRule(_message.Message):
-    __slots__ = ("selector", "get", "put", "post", "delete", "patch", "custom", "body", "additional_bindings")
+    __slots__ = ["selector", "get", "put", "post", "delete", "patch", "custom", "body", "additional_bindings"]
     SELECTOR_FIELD_NUMBER: _ClassVar[int]
     GET_FIELD_NUMBER: _ClassVar[int]
     PUT_FIELD_NUMBER: _ClassVar[int]
     POST_FIELD_NUMBER: _ClassVar[int]
     DELETE_FIELD_NUMBER: _ClassVar[int]
     PATCH_FIELD_NUMBER: _ClassVar[int]
     CUSTOM_FIELD_NUMBER: _ClassVar[int]
@@ -30,13 +30,13 @@
     patch: str
     custom: CustomHttpPattern
     body: str
     additional_bindings: _containers.RepeatedCompositeFieldContainer[HttpRule]
     def __init__(self, selector: _Optional[str] = ..., get: _Optional[str] = ..., put: _Optional[str] = ..., post: _Optional[str] = ..., delete: _Optional[str] = ..., patch: _Optional[str] = ..., custom: _Optional[_Union[CustomHttpPattern, _Mapping]] = ..., body: _Optional[str] = ..., additional_bindings: _Optional[_Iterable[_Union[HttpRule, _Mapping]]] = ...) -> None: ...
 
 class CustomHttpPattern(_message.Message):
-    __slots__ = ("kind", "path")
+    __slots__ = ["kind", "path"]
     KIND_FIELD_NUMBER: _ClassVar[int]
     PATH_FIELD_NUMBER: _ClassVar[int]
     kind: str
     path: str
     def __init__(self, kind: _Optional[str] = ..., path: _Optional[str] = ...) -> None: ...
```

### Comparing `xai_sdk-0.0.5/.gitignore` & `xai_sdk-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/LICENSE.txt` & `xai_sdk-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/pyproject.toml` & `xai_sdk-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.0.5/PKG-INFO` & `xai_sdk-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: xai-sdk
-Version: 0.0.5
+Version: 0.1.0
 Project-URL: Documentation, https://x.ai/api/sdk.html
 Author-email: Toby Pohlen <pohlen@x.ai>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```


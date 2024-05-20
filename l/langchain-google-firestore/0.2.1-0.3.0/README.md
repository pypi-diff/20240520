# Comparing `tmp/langchain_google_firestore-0.2.1-py3-none-any.whl.zip` & `tmp/langchain_google_firestore-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 22185 bytes, number of entries: 13
--rw-r--r--  2.0 unx      920 b- defN 24-May-01 21:10 langchain_google_firestore/__init__.py
--rw-r--r--  2.0 unx     2942 b- defN 24-May-01 21:10 langchain_google_firestore/chat_message_history.py
--rw-r--r--  2.0 unx     1309 b- defN 24-May-01 21:10 langchain_google_firestore/common.py
--rw-r--r--  2.0 unx     4703 b- defN 24-May-01 21:10 langchain_google_firestore/document_converter.py
--rw-r--r--  2.0 unx     8090 b- defN 24-May-01 21:10 langchain_google_firestore/document_loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-May-01 21:10 langchain_google_firestore/py.typed
--rw-r--r--  2.0 unx    12399 b- defN 24-May-01 21:10 langchain_google_firestore/vectorstores.py
--rw-r--r--  2.0 unx      597 b- defN 24-May-01 21:10 langchain_google_firestore/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-May-01 21:12 langchain_google_firestore-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    19331 b- defN 24-May-01 21:12 langchain_google_firestore-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-01 21:12 langchain_google_firestore-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 24-May-01 21:12 langchain_google_firestore-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1266 b- defN 24-May-01 21:12 langchain_google_firestore-0.2.1.dist-info/RECORD
-13 files, 63034 bytes uncompressed, 20005 bytes compressed:  68.3%
+Zip file size: 22304 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      920 b- defN 24-May-20 20:21 langchain_google_firestore/__init__.py
+-rw-r--r--  2.0 unx     3430 b- defN 24-May-20 20:21 langchain_google_firestore/chat_message_history.py
+-rw-r--r--  2.0 unx     1309 b- defN 24-May-20 20:21 langchain_google_firestore/common.py
+-rw-r--r--  2.0 unx     4703 b- defN 24-May-20 20:21 langchain_google_firestore/document_converter.py
+-rw-r--r--  2.0 unx     8090 b- defN 24-May-20 20:21 langchain_google_firestore/document_loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-20 20:21 langchain_google_firestore/py.typed
+-rw-r--r--  2.0 unx    12399 b- defN 24-May-20 20:21 langchain_google_firestore/vectorstores.py
+-rw-r--r--  2.0 unx      597 b- defN 24-May-20 20:21 langchain_google_firestore/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-20 20:23 langchain_google_firestore-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    19383 b- defN 24-May-20 20:23 langchain_google_firestore-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 20:23 langchain_google_firestore-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 24-May-20 20:23 langchain_google_firestore-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1266 b- defN 24-May-20 20:23 langchain_google_firestore-0.3.0.dist-info/RECORD
+13 files, 63574 bytes uncompressed, 20124 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: langchain_google_firestore/vectorstores.py
 Comment: 
 
 Filename: langchain_google_firestore/version.py
 Comment: 
 
-Filename: langchain_google_firestore-0.2.1.dist-info/LICENSE
+Filename: langchain_google_firestore-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_firestore-0.2.1.dist-info/METADATA
+Filename: langchain_google_firestore-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_firestore-0.2.1.dist-info/WHEEL
+Filename: langchain_google_firestore-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_firestore-0.2.1.dist-info/top_level.txt
+Filename: langchain_google_firestore-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_firestore-0.2.1.dist-info/RECORD
+Filename: langchain_google_firestore-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_firestore/chat_message_history.py

```diff
@@ -33,48 +33,61 @@
 
 class FirestoreChatMessageHistory(BaseChatMessageHistory):
     def __init__(
         self,
         session_id: str,
         collection: str = DEFAULT_COLLECTION,
         client: Optional[Client] = None,
+        encode_message: bool = True,
     ) -> None:
         """Chat Message History for Google Cloud Firestore.
 
         Args:
             session_id: Arbitrary key that is used to store the messages of a single
                 chat session. This is the document_path of a document.
             collection: The single `/`-delimited path to a Firestore collection.
             client: Client for interacting with the Google Cloud Firestore API.
+            encode_message: Encode the message when storing into Firestore.
         """
+        self.encode_message = encode_message
         self.client = client_with_user_agent(USER_AGENT, client)
         self.session_id = session_id
         self.doc_ref = self.client.collection(collection).document(session_id)
         self.messages: List[BaseMessage] = []
         self._load_messages()
 
     def _load_messages(self) -> None:
         doc = self.doc_ref.get()
         if doc.exists:
             data_messages = doc.to_dict()
             if "messages" in data_messages:
-                self.messages = decode_messages(data_messages["messages"])
+                self.messages = convert_messages_to_langchain(
+                    self.encode_message, data_messages["messages"]
+                )
 
     def add_message(self, message: BaseMessage) -> None:
         self.messages.append(message)
         self._upsert_messages()
 
     def _upsert_messages(self) -> None:
-        self.doc_ref.set({"messages": encode_messages(self.messages)})
+        if self.encode_message:
+            self.doc_ref.set({"messages": encode_messages(self.messages)})
+        else:
+            self.doc_ref.set({"messages": [m.json() for m in self.messages]})
 
     def clear(self) -> None:
         self.messages = []
         self.doc_ref.delete()
 
 
 def encode_messages(messages: List[BaseMessage]) -> List[bytes]:
     return [str.encode(m.json()) for m in messages]
 
 
-def decode_messages(messages: List[bytes]) -> List[BaseMessage]:
-    dict_messages = [json.loads(m.decode()) for m in messages]
+def convert_messages_to_langchain(
+    is_encoded: bool, messages: List[bytes]
+) -> List[BaseMessage]:
+    if is_encoded:
+        dict_messages = [json.loads(m.decode()) for m in messages]
+    else:
+        dict_messages = [json.loads(m) for m in messages]
     return messages_from_dict([{"type": m["type"], "data": m} for m in dict_messages])
```

## langchain_google_firestore/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
```

## Comparing `langchain_google_firestore-0.2.1.dist-info/LICENSE` & `langchain_google_firestore-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_firestore-0.2.1.dist-info/METADATA` & `langchain_google_firestore-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-firestore
-Version: 0.2.1
+Version: 0.3.0
 Summary: LangChain integrations for Google Cloud Firestore
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -228,14 +228,15 @@
 Requires-Dist: more-itertools <11.0.0,>=10.2.0
 Provides-Extra: test
 Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
 Requires-Dist: mypy ==1.10.0 ; extra == 'test'
 Requires-Dist: pytest-asyncio ==0.23.6 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
+Requires-Dist: pytest-cov ==5.0.0 ; extra == 'test'
 
 Firestore for LangChain
 =======================
 
 |preview| |pypi| |versions|
 
 - `Client Library Documentation`_
@@ -316,15 +317,15 @@
     store = FirestoreVectorStore(
         collection="VectorStore",
         embedding=embedding
     )
 
 See the full `Vector Store`_ tutorial.
 
-.. _`Vector Store`: https://github.com/googleapis/langchain-google-firestore-python/blob/main/docs/vector_store.ipynb
+.. _`Vector Store`: https://github.com/googleapis/langchain-google-firestore-python/blob/main/docs/vectorstores.ipynb
 
 Document Loader Usage
 ~~~~~~~~~~~~~~~~~~~~~
 
 Use a document loader to load data as LangChain ``Document``\ s.
 
 .. code-block:: python
```

## Comparing `langchain_google_firestore-0.2.1.dist-info/RECORD` & `langchain_google_firestore-0.3.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 langchain_google_firestore/__init__.py,sha256=y0T6tgQjKQ4mJ9LqMVPfzc0bVbI-Kmp9UbtccFbJqDI,920
-langchain_google_firestore/chat_message_history.py,sha256=Iv5tesPp85ZPl4HqCBMY0yaXXCjP8_r_9mk5BGAO9lE,2942
+langchain_google_firestore/chat_message_history.py,sha256=S_immNp0ufj6AL6kKXRnf-g7shN3lWaT1qXmYMcCqNo,3430
 langchain_google_firestore/common.py,sha256=y4b-mP3Le3GbdS8pCMIf7sy5VcSftvkTFjGDcmPxE5E,1309
 langchain_google_firestore/document_converter.py,sha256=KFDvyKzA3CaYkXiMV0F_YloEtiKf708S16ZYOJwsp04,4703
 langchain_google_firestore/document_loader.py,sha256=CguEq_9IpWS9ojhKWx0d_1S0J1vA01moswZgF-XNea4,8090
 langchain_google_firestore/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 langchain_google_firestore/vectorstores.py,sha256=rinOn5RyK4oM6O56EIzOpw1OjAq0UxT2UMzceIP0r6c,12399
-langchain_google_firestore/version.py,sha256=lal6j0-2qdxqYCLjy1FcTVeiboHQADADWfCBuVKcU3k,597
-langchain_google_firestore-0.2.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_firestore-0.2.1.dist-info/METADATA,sha256=qda_uY3iAFMTUjLYhqf4CYb_awOalaonqYgiwfmGty0,19331
-langchain_google_firestore-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_firestore-0.2.1.dist-info/top_level.txt,sha256=DE7TPex7qLfJ4mR_QyJoCq4IQEoS-uF1NoUlWlaEf-8,27
-langchain_google_firestore-0.2.1.dist-info/RECORD,,
+langchain_google_firestore/version.py,sha256=Bt9xmJb_aic5hHSb19XJI5LMnotdGjBnwcYbbCI4jfo,597
+langchain_google_firestore-0.3.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_firestore-0.3.0.dist-info/METADATA,sha256=Y34DHf-yXXmVgkL8ckoI1Lu4zTgxcsL8loarVrl4WfE,19383
+langchain_google_firestore-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_firestore-0.3.0.dist-info/top_level.txt,sha256=DE7TPex7qLfJ4mR_QyJoCq4IQEoS-uF1NoUlWlaEf-8,27
+langchain_google_firestore-0.3.0.dist-info/RECORD,,
```


# Comparing `tmp/conva_ai-0.1.0.tar.gz` & `tmp/conva_ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conva_ai-0.1.0.tar", last modified: Mon May 13 15:08:36 2024, max compression
+gzip compressed data, was "conva_ai-0.1.1.tar", last modified: Mon May 20 10:34:32 2024, max compression
```

## Comparing `conva_ai-0.1.0.tar` & `conva_ai-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-13 15:08:36.063070 conva_ai-0.1.0/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3650 2024-05-13 15:08:36.062804 conva_ai-0.1.0/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     2844 2024-05-13 15:07:54.000000 conva_ai-0.1.0/README.md
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-13 15:08:36.061287 conva_ai-0.1.0/conva_ai/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-20 05:49:43.000000 conva_ai-0.1.0/conva_ai/__init__.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      677 2024-05-13 15:07:54.000000 conva_ai-0.1.0/conva_ai/base.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     4015 2024-05-13 15:07:54.000000 conva_ai-0.1.0/conva_ai/client.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      604 2024-04-25 13:45:56.000000 conva_ai-0.1.0/conva_ai/response.py
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-13 15:08:36.062471 conva_ai-0.1.0/conva_ai.egg-info/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3650 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/SOURCES.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/dependency_links.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      193 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/requires.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/top_level.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      652 2024-05-13 15:07:54.000000 conva_ai-0.1.0/pyproject.toml
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      571 2024-04-23 09:58:39.000000 conva_ai-0.1.0/requirements.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-05-13 15:08:36.063138 conva_ai-0.1.0/setup.cfg
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-20 10:34:32.493361 conva_ai-0.1.1/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3963 2024-05-20 10:34:32.493102 conva_ai-0.1.1/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3157 2024-05-20 10:34:17.000000 conva_ai-0.1.1/README.md
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-20 10:34:32.491480 conva_ai-0.1.1/conva_ai/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-20 05:49:43.000000 conva_ai-0.1.1/conva_ai/__init__.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      677 2024-05-15 11:46:24.000000 conva_ai-0.1.1/conva_ai/base.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     4015 2024-05-15 11:46:24.000000 conva_ai-0.1.1/conva_ai/client.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      604 2024-04-25 13:45:56.000000 conva_ai-0.1.1/conva_ai/response.py
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-20 10:34:32.492805 conva_ai-0.1.1/conva_ai.egg-info/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3963 2024-05-20 10:34:32.000000 conva_ai-0.1.1/conva_ai.egg-info/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-05-20 10:34:32.000000 conva_ai-0.1.1/conva_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-05-20 10:34:32.000000 conva_ai-0.1.1/conva_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      193 2024-05-20 10:34:32.000000 conva_ai-0.1.1/conva_ai.egg-info/requires.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-05-20 10:34:32.000000 conva_ai-0.1.1/conva_ai.egg-info/top_level.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      652 2024-05-20 10:34:17.000000 conva_ai-0.1.1/pyproject.toml
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      571 2024-04-23 09:58:39.000000 conva_ai-0.1.1/requirements.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-05-20 10:34:32.493418 conva_ai-0.1.1/setup.cfg
```

### Comparing `conva_ai-0.1.0/PKG-INFO` & `conva_ai-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: conva_ai
-Version: 0.1.0
-Summary: Python SDK for using Conva AI co-pilots
-Author-email: Slang Labs <support@slanglabs.in>
-Project-URL: Homepage, http://www.slanglabs.in
-Project-URL: Documentation, https://docs.slanglabs.in/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Requires-Dist: annotated-types==0.6.0
-Requires-Dist: certifi==2024.2.2
-Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: idna==3.7
-Requires-Dist: pydantic==2.7.0
-Requires-Dist: pydantic-core==2.18.1
-Requires-Dist: requests==2.31.0
-Requires-Dist: sseclient-py==1.8.0
-Requires-Dist: typing-extensions==4.11.0
-Requires-Dist: urllib3==2.2.1
-
 # Python Library for Conva AI
 
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
@@ -32,22 +9,52 @@
 import asyncio
 from conva_ai import AsyncConvaAI
 client = AsyncConvaAI(
     assistant_id="<YOUR_ASSISTANT_ID>", 
     assistant_version="<YOUR_ASSISTANT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
-async def generate(client: AsyncConvaAI, query: str, stream: bool):
-    response = client.invoke_capability(query, stream=stream)
+async def generate_with_capability_group(client: AsyncConvaAI, query: str, capability_group: str = "default", stream: bool = "True"):
+  if stream:
+    response = await client.invoke_capability_group_stream(query, capability_group=capability_group)
     out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
     return out
+  else:
+    response = await client.invoke_capability_group(query, capability_group=capability_group)
+    return response.model_dump_json(indent=4)
 
-final_response = asyncio.run(generate(client, "how are you", True))
+final_response = asyncio.run(generate_with_capability_group(client, "how are you", stream=True))
+print(final_response)
+```
+
+The above snippet of code is used for invoking a capability group. 
+
+Similarly, a particular capability can be invoked by
+```
+import asyncio
+from conva_ai import AsyncConvaAI
+client = AsyncConvaAI(
+    assistant_id="<YOUR_ASSISTANT_ID>", 
+    assistant_version="<YOUR_ASSISTANT_VERSION>", 
+    api_key="<YOUR_API_KEY>"
+)
+async def generate_with_capability_name(client: AsyncConvaAI, query: str, capability_name: str, stream: bool):
+  if stream:
+    response = await client.invoke_capability_stream(query, capability_name=capability_name)
+    out = ""
+    async for res in response:
+        out = res.model_dump_json(indent=4)
+    return out
+  else:
+    response = await client.invoke_capability(query, capability_name=capability_name)
+    return response.model_dump_json(indent=4)
+
+final_response = asyncio.run(generate_with_capability_name(client, "buy 10 shares", "order_management", True))
 print(final_response)
 ```
 
 You can try out the co-pilot on [Google Colab](https://colab.research.google.com/drive/1WtbARTRQ9wCvztrAQuEhQUvwImhtPZXd#scrollTo=ZSVBQsOelgfv)
 
 If you want to get the response as dictionary, then replace
 ```
@@ -88,40 +95,10 @@
 ```
 
 ### 3. Debugging responses
 
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
-import asyncio
-from conva_ai.client import AsyncConvaAI
-
-client = AsyncConvaAI(
-        assistant_id="<YOUR_ASSISTANT_ID>", 
-        assistant_version="<YOUR_ASSISTANT_VERSION>", 
-        api_key="<YOUR_API_KEY>"
-    )
-
-async def generate(client: AsyncConvaAI, query: str, stream: bool):
-    response = client.invoke_capability(query, stream=stream)
-    out=""
-    async for res in response:
-        out = res
-    return out
-
-final_response = asyncio.run(generate("how are you", True))
-print(final_response.reason)
-```
-
-### How to use capability groups
-
-Capability Groups are used to control the list of Capabilities that Co pilot will have access. 
-You can make use of the capability group while using the `invoke_capability` method
-
-```
-async def generate(client: AsyncConvaAI, query: str, stream: bool):
-    response = client.invoke_capability(query, stream=stream, capability_group="<CAPABILITY_GROUP_NAME>")
-    out=""
-    async for res in response:
-        out = res
-    return out
-```
+final_response_dict = json.loads(final_response)
+print(final_response_dict["reason"])
+```
```

### Comparing `conva_ai-0.1.0/conva_ai/base.py` & `conva_ai-0.1.1/conva_ai/base.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.1.0/conva_ai/client.py` & `conva_ai-0.1.1/conva_ai/client.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.1.0/conva_ai/response.py` & `conva_ai-0.1.1/conva_ai/response.py`

 * *Files identical despite different names*

### Comparing `conva_ai-0.1.0/conva_ai.egg-info/PKG-INFO` & `conva_ai-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,22 +32,52 @@
 import asyncio
 from conva_ai import AsyncConvaAI
 client = AsyncConvaAI(
     assistant_id="<YOUR_ASSISTANT_ID>", 
     assistant_version="<YOUR_ASSISTANT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
-async def generate(client: AsyncConvaAI, query: str, stream: bool):
-    response = client.invoke_capability(query, stream=stream)
+async def generate_with_capability_group(client: AsyncConvaAI, query: str, capability_group: str = "default", stream: bool = "True"):
+  if stream:
+    response = await client.invoke_capability_group_stream(query, capability_group=capability_group)
     out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
     return out
+  else:
+    response = await client.invoke_capability_group(query, capability_group=capability_group)
+    return response.model_dump_json(indent=4)
 
-final_response = asyncio.run(generate(client, "how are you", True))
+final_response = asyncio.run(generate_with_capability_group(client, "how are you", stream=True))
+print(final_response)
+```
+
+The above snippet of code is used for invoking a capability group. 
+
+Similarly, a particular capability can be invoked by
+```
+import asyncio
+from conva_ai import AsyncConvaAI
+client = AsyncConvaAI(
+    assistant_id="<YOUR_ASSISTANT_ID>", 
+    assistant_version="<YOUR_ASSISTANT_VERSION>", 
+    api_key="<YOUR_API_KEY>"
+)
+async def generate_with_capability_name(client: AsyncConvaAI, query: str, capability_name: str, stream: bool):
+  if stream:
+    response = await client.invoke_capability_stream(query, capability_name=capability_name)
+    out = ""
+    async for res in response:
+        out = res.model_dump_json(indent=4)
+    return out
+  else:
+    response = await client.invoke_capability(query, capability_name=capability_name)
+    return response.model_dump_json(indent=4)
+
+final_response = asyncio.run(generate_with_capability_name(client, "buy 10 shares", "order_management", True))
 print(final_response)
 ```
 
 You can try out the co-pilot on [Google Colab](https://colab.research.google.com/drive/1WtbARTRQ9wCvztrAQuEhQUvwImhtPZXd#scrollTo=ZSVBQsOelgfv)
 
 If you want to get the response as dictionary, then replace
 ```
@@ -88,40 +118,10 @@
 ```
 
 ### 3. Debugging responses
 
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
-import asyncio
-from conva_ai.client import AsyncConvaAI
-
-client = AsyncConvaAI(
-        assistant_id="<YOUR_ASSISTANT_ID>", 
-        assistant_version="<YOUR_ASSISTANT_VERSION>", 
-        api_key="<YOUR_API_KEY>"
-    )
-
-async def generate(client: AsyncConvaAI, query: str, stream: bool):
-    response = client.invoke_capability(query, stream=stream)
-    out=""
-    async for res in response:
-        out = res
-    return out
-
-final_response = asyncio.run(generate("how are you", True))
-print(final_response.reason)
-```
-
-### How to use capability groups
-
-Capability Groups are used to control the list of Capabilities that Co pilot will have access. 
-You can make use of the capability group while using the `invoke_capability` method
-
-```
-async def generate(client: AsyncConvaAI, query: str, stream: bool):
-    response = client.invoke_capability(query, stream=stream, capability_group="<CAPABILITY_GROUP_NAME>")
-    out=""
-    async for res in response:
-        out = res
-    return out
+final_response_dict = json.loads(final_response)
+print(final_response_dict["reason"])
 ```
```

### Comparing `conva_ai-0.1.0/pyproject.toml` & `conva_ai-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "conva_ai"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Slang Labs", email="support@slanglabs.in" },
 ]
 dynamic = ["dependencies"]
 description = "Python SDK for using Conva AI co-pilots"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `conva_ai-0.1.0/requirements.txt` & `conva_ai-0.1.1/requirements.txt`

 * *Files identical despite different names*


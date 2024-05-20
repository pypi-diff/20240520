# Comparing `tmp/llm_taxi-0.2.1.tar.gz` & `tmp/llm_taxi-0.3.1.tar.gz`

## Comparing `llm_taxi-0.2.1.tar` & `llm_taxi-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,44 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/.python-version
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/pyrightconfig.json
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/requirements-dev.lock
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/requirements.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/__init__.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/cli.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/conversation.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/factory.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/__init__.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/anthropic.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/base.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/dashscope.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/deepinfra.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/deepseek.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/google.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/groq.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/mistral.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/openai.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/openrouter.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/perplexity.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/src/llm_taxi/llms/together.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/tests/test_llm.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 llm_taxi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/.python-version
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/pyrightconfig.json
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/requirements-dev.lock
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/requirements.lock
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/cli.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/conversation.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/factory.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/anthropic.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/base.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/dashscope.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/deepinfra.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/deepseek.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/google.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/groq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/mistral.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/openai.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/openrouter.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/perplexity.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/clients/together.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/__init__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/base.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/google.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/mistral.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/embeddings/openai.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/anthropic.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/base.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/dashscope.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/deepinfra.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/deepseek.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/google.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/groq.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/mistral.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/openai.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/openrouter.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/perplexity.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/src/llm_taxi/llms/together.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/tests/test_llm.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 llm_taxi-0.3.1/PKG-INFO
```

### Comparing `llm_taxi-0.2.1/requirements-dev.lock` & `llm_taxi-0.3.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.2.1/requirements.lock` & `llm_taxi-0.3.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.2.1/src/llm_taxi/cli.py` & `llm_taxi-0.3.1/src/llm_taxi/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 
 async def async_main():
     args = parse_args()
 
     call_kwargs = {
         "max_tokens": args.max_tokens,
     }
-    model = llm(model=args.model, call_kwargs=call_kwargs)
+    try:
+        model = llm(model=args.model, call_kwargs=call_kwargs)
+    except KeyError as e:
+        print(f"Error: {e}")
+        sys.exit(1)
 
     while True:
         try:
             user_input = input("> ").strip()
         except (KeyboardInterrupt, EOFError):
             sys.exit(0)
 
@@ -37,15 +41,14 @@
             Message(
                 role=Role.User,
                 content=user_input,
             ),
         ]
         response = await model.streaming_response(messages=messages)
 
-        print(f"({args.model}): ", end="", flush=True)
         async for chunk in response:
             print(chunk, end="", flush=True)
         print("\n")
 
 
 def main():
     asyncio.run(async_main())
```

### Comparing `llm_taxi-0.2.1/src/llm_taxi/llms/__init__.py` & `llm_taxi-0.3.1/src/llm_taxi/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.2.1/src/llm_taxi/llms/anthropic.py` & `llm_taxi-0.3.1/src/llm_taxi/llms/anthropic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from collections.abc import AsyncGenerator
-from typing import Any, ClassVar, Literal, cast
+from typing import Any, Literal, cast
 
-from anthropic import AsyncAnthropic
 from anthropic._types import NOT_GIVEN, NotGiven
 from anthropic.types import MessageParam
 
+from llm_taxi.clients.anthropic import Anthropic as AnthropicClient
 from llm_taxi.conversation import Message, Role
 from llm_taxi.llms.base import LLM
 
 
-class Anthropic(LLM):
-    env_vars: ClassVar[dict[str, str]] = {
-        "api_key": "ANTHROPIC_API_KEY",
-    }
-
-    def _init_client(self, **kwargs) -> Any:
-        return AsyncAnthropic(**kwargs)
-
+class Anthropic(AnthropicClient, LLM):
     def _convert_messages(self, messages: list[Message]) -> list[Any]:
         return [
             MessageParam(
                 role=cast(Literal["user", "assistant"], message.role.value),
                 content=message.content,
             )
             for message in messages
```

### Comparing `llm_taxi-0.2.1/src/llm_taxi/llms/google.py` & `llm_taxi-0.3.1/src/llm_taxi/llms/google.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,17 @@
 import itertools
 from collections.abc import AsyncGenerator
-from typing import Any, ClassVar
+from typing import Any
 
+from llm_taxi.clients.google import Google as GoogleClient
 from llm_taxi.conversation import Message, Role
-from llm_taxi.llms import LLM
+from llm_taxi.llms.base import LLM
 
 
-class Google(LLM):
-    env_vars: ClassVar[dict[str, str]] = {
-        "api_key": "GOOGLE_API_KEY",
-    }
-
-    def __init__(
-        self,
-        *,
-        model: str,
-        api_key: str,
-        base_url: str | None = None,
-        call_kwargs: dict | None = None,
-        **client_kwargs,
-    ) -> None:
-        super().__init__(
-            model=model,
-            api_key=api_key,
-            base_url=base_url,
-            call_kwargs=call_kwargs,
-            **client_kwargs,
-        )
-
-        from google import generativeai as genai
-
-        genai.configure(api_key=api_key, **client_kwargs)
-
-        self._call_kwargs.pop("model", None)
-
-    def _init_client(self, **kwargs) -> Any:
-        from google import generativeai as genai
-
-        return genai.GenerativeModel(self.model, **kwargs)
-
+class Google(GoogleClient, LLM):
     def _convert_messages(self, messages: list[Message]) -> list[Any]:
         role_mappping = {
             Role.System: "user",
             Role.User: "user",
             Role.Assistant: "model",
         }
         groups = itertools.groupby(
```

### Comparing `llm_taxi-0.2.1/src/llm_taxi/llms/groq.py` & `llm_taxi-0.3.1/src/llm_taxi/llms/groq.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-from typing import Any, ClassVar
+from typing import Any
 
-from groq import AsyncGroq
 from groq.types.chat.completion_create_params import Message as GroqMessage
 
+from llm_taxi.clients.groq import Groq as GroqClient
 from llm_taxi.conversation import Message
 from llm_taxi.llms.openai import OpenAI
 
 
-class Groq(OpenAI):
-    env_vars: ClassVar[dict[str, str]] = {
-        "api_key": "GROQ_API_KEY",
-    }
-
-    def _init_client(self, **kwargs) -> Any:
-        return AsyncGroq(**kwargs)
-
+class Groq(GroqClient, OpenAI):
     def _convert_messages(self, messages: list[Message]) -> list[Any]:
         return [
             GroqMessage(
                 role=message.role.value,
                 content=message.content,
             )
             for message in messages
```

### Comparing `llm_taxi-0.2.1/src/llm_taxi/llms/mistral.py` & `llm_taxi-0.3.1/src/llm_taxi/llms/openai.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 from collections.abc import AsyncGenerator
-from typing import Any, ClassVar
-
-from mistralai.async_client import MistralAsyncClient
-from mistralai.models.chat_completion import ChatMessage
+from typing import Any
 
+from llm_taxi.clients.openai import OpenAI as OpenAIClient
 from llm_taxi.conversation import Message
-from llm_taxi.llms.openai import OpenAI
-
+from llm_taxi.llms.base import LLM
 
-class Mistral(OpenAI):
-    env_vars: ClassVar[dict[str, str]] = {
-        "api_key": "MISTRAL_API_KEY",
-    }
 
-    def _init_client(self, **kwargs) -> Any:
-        kwargs.pop("base_url", None)
+async def streaming_response(response: Any) -> AsyncGenerator:
+    async for chunk in response:
+        if content := chunk.choices[0].delta.content:
+            yield content
 
-        return MistralAsyncClient(**kwargs)
-
-    def _convert_messages(self, messages: list[Message]) -> list[Any]:
-        return [ChatMessage(role=x.role.value, content=x.content) for x in messages]
 
+class OpenAI(OpenAIClient, LLM):
     async def streaming_response(
         self,
         messages: list[Message],
         **kwargs,
     ) -> AsyncGenerator:
         messages = self._convert_messages(messages)
 
-        response = self.client.chat_stream(
+        response = await self.client.chat.completions.create(
             messages=messages,
+            stream=True,
             **self._get_call_kwargs(**kwargs),
         )
 
-        return self._streaming_response(response)
+        return streaming_response(response)
 
     async def response(self, messages: list[Message], **kwargs) -> str:
         messages = self._convert_messages(messages)
 
-        response = await self.client.chat(
+        response = await self.client.chat.completions.create(
             messages=messages,
             **self._get_call_kwargs(**kwargs),
         )
 
-        return response.choices[0].message.content
+        if content := response.choices[0].message.content:
+            return content
+
+        return ""
```

### Comparing `llm_taxi-0.2.1/pyproject.toml` & `llm_taxi-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-taxi"
-version = "0.2.1"
+version = "0.3.1"
 description = "Call LLM as easily as calling a taxi."
 authors = [{ name = "Yevgnen Koh", email = "wherejoystarts@gmail.com" }]
 dependencies = [
     "openai>=1.28.1",
     "pydantic>=2.7.1",
     "google-generativeai>=0.5.2",
     "together>=1.1.5",
```


# Comparing `tmp/arena_client-0.2.0.tar.gz` & `tmp/arena_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena_client-0.2.0.tar", max compression
+gzip compressed data, was "arena_client-0.2.1.tar", max compression
```

## Comparing `arena_client-0.2.0.tar` & `arena_client-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      570 2024-05-17 11:59:03.499076 arena_client-0.2.0/README.md
--rw-r--r--   0        0        0     1330 2024-05-17 11:59:03.499076 arena_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      154 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/__init__.py
--rw-r--r--   0        0        0    12669 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/client.py
--rw-r--r--   0        0        0     1018 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/__init__.py
--rw-r--r--   0        0        0     3988 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/anthropic.py
--rw-r--r--   0        0        0     4364 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/chat_completion.py
--rw-r--r--   0        0        0      281 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/evaluation.py
--rw-r--r--   0        0        0     2393 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/mistral.py
--rw-r--r--   0        0        0     1882 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/openai.py
--rw-r--r--   0        0        0      204 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/settings.py
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 arena_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      570 2024-05-20 10:18:49.495750 arena_client-0.2.1/README.md
+-rw-r--r--   0        0        0     1348 2024-05-20 10:18:49.495750 arena_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      154 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/__init__.py
+-rw-r--r--   0        0        0    12669 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/client.py
+-rw-r--r--   0        0        0     1018 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/__init__.py
+-rw-r--r--   0        0        0     4009 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/anthropic.py
+-rw-r--r--   0        0        0     4364 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/chat_completion.py
+-rw-r--r--   0        0        0      281 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/evaluation.py
+-rw-r--r--   0        0        0     2287 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/mistral.py
+-rw-r--r--   0        0        0     1444 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/openai.py
+-rw-r--r--   0        0        0      204 2024-05-20 10:18:49.495750 arena_client-0.2.1/src/arena/models/settings.py
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 arena_client-0.2.1/PKG-INFO
```

### Comparing `arena_client-0.2.0/README.md` & `arena_client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.0/pyproject.toml` & `arena_client-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arena-client"
-version = "0.2.0"
+version = "0.2.1"
 description = "A client to use arena AI"
 authors = ["Nicolas Grislain <ng@sarus.tech>"]
 license = "Apache-2"
 readme = "README.md"
 packages = [{from = "src", include = "arena"}]
 
 [tool.poetry.dependencies]
@@ -17,14 +17,15 @@
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.10.0"
 pytest = "^8.1.1"
 ruff = "^0.2.2"
 python-dotenv = "^1.0.1"
 rich = "^13.7.1"
+faker = "^25.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py311"
```

### Comparing `arena_client-0.2.0/src/arena/client.py` & `arena_client-0.2.1/src/arena/client.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.0/src/arena/models/__init__.py` & `arena_client-0.2.1/src/arena/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.0/src/arena/models/anthropic.py` & `arena_client-0.2.1/src/arena/models/anthropic.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 from arena import models
 from arena.models import Function, ChatCompletionToolParam, Message, ResponseFormat, TopLogprob, TokenLogprob, ChoiceLogprobs, Choice
 """
 ChatCompletionCreate -> anthropic MessageCreateParams -> anthropic Message -> ChatCompletion
 """
 
+MODELS = ("claude-3-opus-20240229", "claude-3-sonnet-20240229", "claude-3-haiku-20240307", "claude-2.1", "claude-2.0", "claude-instant-1.2")
+
+
 class Metadata(BaseModel):
     user_id: str
 
 
 class FunctionDefinition(BaseModel):
     name: str
     description: str | None = None
@@ -22,15 +25,15 @@
     """
     Maps to:
     https://github.com/anthropics/anthropic-sdk-python/blob/main/src/anthropic/types/message_create_params.py#L13
     https://docs.anthropic.com/claude/reference/messages_post
     """
     max_tokens: int = 1
     messages: Sequence[Message]
-    model: str | Literal["claude-3-opus-20240229", "claude-3-sonnet-20240229", "claude-3-haiku-20240307", "claude-2.1", "claude-2.0", "claude-instant-1.2"]
+    model: str | Literal[*MODELS]
     metadata: Metadata | None = None
     stop_sequences: Sequence[str] | None = None
     system: str | None = None
     temperature: float | None = None
     tools: Sequence[FunctionDefinition] | None = None
     top_p: float | None = None
     top_k: int | None = None
```

### Comparing `arena_client-0.2.0/src/arena/models/chat_completion.py` & `arena_client-0.2.1/src/arena/models/chat_completion.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.2.0/src/arena/models/mistral.py` & `arena_client-0.2.1/src/arena/models/mistral.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 from arena import models
 from arena.models import Function, FunctionDefinition, ChatCompletionToolParam, Message, ResponseFormat, TopLogprob, TokenLogprob, ChoiceLogprobs, Choice, CompletionUsage
 
 """
 models.ChatCompletionCreate -> ChatCompletionCreate -> ChatCompletion -> models.ChatCompletion
 """
 
+MODELS = ("mistral-large-latest", "mistral-medium", "mistral-medium-latest", "mistral-small", "mistral-small-latest", "mistral-tiny", "open-mistral-7b", "open-mixtral-8x7b")
+
+
 class ChatCompletionRequest(BaseModel):
     """
     Maps to:
     https://github.com/mistralai/client-python/blob/main/src/mistralai/client.py#L153
     https://github.com/mistralai/client-python/blob/main/src/mistralai/models/chat_completion.py
     https://docs.mistral.ai/api/#operation/createChatCompletion
     """
     messages: Sequence[Message]
-    model: str | Literal["mistral-embed", "mistral-large-2402", "mistral-large-latest", "mistral-medium", "mistral-medium-2312", "mistral-medium-latest", "mistral-small", "mistral-small-2312", "mistral-small-2402", "mistral-small-latest", "mistral-tiny", "mistral-tiny-2312", "open-mistral-7b", "open-mixtral-8x7b"]
+    model: str | Literal[*MODELS]
     max_tokens: int | None = None
     response_format: ResponseFormat | None = None
     safe_prompt: bool | None = None
     random_seed: int | None = None
     temperature: float | None = None
     tool_choice: Literal["none", "auto", "any"] | None = None
     tools: Sequence[ChatCompletionToolParam] | None = None
```

### Comparing `arena_client-0.2.0/src/arena/models/openai.py` & `arena_client-0.2.1/src/arena/models/openai.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,22 @@
 from typing import Mapping, Sequence, Literal, Any
 
 from pydantic import BaseModel
 
 from arena import models
 from arena.models import Function, FunctionDefinition, ChatCompletionToolParam, Message, ResponseFormat, TopLogprob, TokenLogprob, ChoiceLogprobs, Choice, CompletionUsage
 
+MODELS = ("gpt-4o", "gpt-4-turbo", "gpt-4", "gpt-3.5-turbo", "gpt-3.5-turbo-16k")
 
 class ChatCompletionRequest(models.ChatCompletionRequest):
     """
     https://github.com/openai/openai-python/blob/main/src/openai/types/chat/completion_create_params.py#L24
     https://platform.openai.com/docs/api-reference/chat
     """
-    model: str | Literal[
-        "gpt-4-turbo",
-        "gpt-4-turbo-2024-04-09",
-        "gpt-4-0125-preview",
-        "gpt-4-turbo-preview",
-        "gpt-4-1106-preview",
-        "gpt-4-vision-preview",
-        "gpt-4",
-        "gpt-4-0314",
-        "gpt-4-0613",
-        "gpt-4-32k",
-        "gpt-4-32k-0314",
-        "gpt-4-32k-0613",
-        "gpt-3.5-turbo",
-        "gpt-3.5-turbo-16k",
-        "gpt-3.5-turbo-0301",
-        "gpt-3.5-turbo-0613",
-        "gpt-3.5-turbo-1106",
-        "gpt-3.5-turbo-0125",
-        "gpt-3.5-turbo-16k-0613",
-    ]
+    model: str | Literal[*MODELS]
 
     @classmethod
     def from_chat_completion_request(cls, ccc: models.ChatCompletionRequest) -> "ChatCompletionRequest":
         return ChatCompletionRequest.model_validate(ccc.model_dump(exclude=["lm_config"]))
 
     def to_dict(self) -> Mapping[str, Any]:
         return self.model_dump(exclude_none=True)
```

### Comparing `arena_client-0.2.0/PKG-INFO` & `arena_client-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: A client to use arena AI
 License: Apache-2
 Author: Nicolas Grislain
 Author-email: ng@sarus.tech
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


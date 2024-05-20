# Comparing `tmp/unisender_go_api-0.2.0.tar.gz` & `tmp/unisender_go_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisender_go_api-0.2.0.tar", max compression
+gzip compressed data, was "unisender_go_api-0.3.0.tar", max compression
```

## Comparing `unisender_go_api-0.2.0.tar` & `unisender_go_api-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3959 2024-05-14 15:46:59.342756 unisender_go_api-0.2.0/README.md
--rw-r--r--   0        0        0      647 2024-05-14 15:56:30.189781 unisender_go_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      368 2024-05-14 15:22:42.792246 unisender_go_api-0.2.0/unisender_go_api/__init__.py
--rw-r--r--   0        0        0     4172 2024-05-14 15:28:20.231823 unisender_go_api-0.2.0/unisender_go_api/api_methods.py
--rw-r--r--   0        0        0    13047 2024-05-14 15:57:59.984882 unisender_go_api-0.2.0/unisender_go_api/api_types.py
--rw-r--r--   0        0        0     1684 2024-05-14 11:33:21.539085 unisender_go_api-0.2.0/unisender_go_api/clients.py
--rw-r--r--   0        0        0     3562 2024-05-14 13:30:24.516530 unisender_go_api-0.2.0/unisender_go_api/exceptions.py
--rw-r--r--   0        0        0     4733 1970-01-01 00:00:00.000000 unisender_go_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3959 2024-05-14 15:46:59.342756 unisender_go_api-0.3.0/README.md
+-rw-r--r--   0        0        0      647 2024-05-20 06:25:31.849489 unisender_go_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      371 2024-05-20 06:17:35.658525 unisender_go_api-0.3.0/unisender_go_api/__init__.py
+-rw-r--r--   0        0        0     4175 2024-05-20 06:17:22.516544 unisender_go_api-0.3.0/unisender_go_api/_api_methods.py
+-rw-r--r--   0        0        0    12917 2024-05-20 06:20:58.962323 unisender_go_api-0.3.0/unisender_go_api/_api_types.py
+-rw-r--r--   0        0        0     1684 2024-05-20 06:16:49.582010 unisender_go_api-0.3.0/unisender_go_api/_clients.py
+-rw-r--r--   0        0        0     3600 2024-05-20 06:18:51.897548 unisender_go_api-0.3.0/unisender_go_api/_exceptions.py
+-rw-r--r--   0        0        0     4733 1970-01-01 00:00:00.000000 unisender_go_api-0.3.0/PKG-INFO
```

### Comparing `unisender_go_api-0.2.0/README.md` & `unisender_go_api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `unisender_go_api-0.2.0/pyproject.toml` & `unisender_go_api-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unisender-go-api"
-version = "0.2.0"
+version = "0.3.0"
 description = "Thin wrapper for the Unisender Go API"
 authors = [
     "Evgeny Evseev <pelid80@gmail.com>",
 ]
 license = "GNU GPLv3"
 readme = "README.md"
 repository = "https://gitlab.dvmn.org/dvmn-open-source-dev-tools/unisender-go-api"
```

### Comparing `unisender_go_api-0.2.0/unisender_go_api/api_methods.py` & `unisender_go_api-0.3.0/unisender_go_api/_api_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import Counter
 from typing import Literal
 from urllib.parse import urljoin
 
 import httpx
-from pydantic import BaseModel, Field, validator, ValidationError, Extra
+from pydantic import BaseModel, Extra, Field, ValidationError, validator
 
-from .exceptions import raise_for_status, SyncClientSetupError, ResponseFormatError
-from .clients import SyncClient
-from .api_types import Message, Tag
+from ._api_types import Message, Tag
+from ._clients import SyncClient
+from ._exceptions import raise_for_status, ResponseFormatError, SyncClientSetupError
 
 
 def post_as_json(request_payload: BaseModel, api_method: str) -> httpx.Response:
     """Send a request to the Unisender Go API synchronously using a JSON payload."""
     client = SyncClient.default_client.get(None)
 
     if not client:
```

### Comparing `unisender_go_api-0.2.0/unisender_go_api/api_types.py` & `unisender_go_api-0.3.0/unisender_go_api/_api_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Literal, Union, Any, cast
+from typing import Any, cast, Literal, Union
 
 from pydantic import (
     BaseModel,
-    ConstrainedStr,
+    conint,
+    constr,
     ConstrainedInt,
+    ConstrainedStr,
     EmailStr,
     Field,
-    conint,
-    constr,
-    validator,
     root_validator,
-    StrictStr,
+    StrictBool,
     StrictFloat,
     StrictInt,
-    StrictBool,
+    StrictStr,
+    validator,
 )
 
 IntFlag: ConstrainedInt = conint(ge=0, le=1)
 
 
 AttachmentType: ConstrainedStr = constr(min_length=1, strip_whitespace=True, to_lower=True)
 AttachmentName: ConstrainedStr = constr(min_length=1, strip_whitespace=True)
@@ -35,17 +35,14 @@
     )
     content: str = Field(
         max_length=9786710,
         description='Содержимое файла в base64 https://en.wikipedia.org/wiki/Base64. Максимальный размер '
                     'файла 7Mб (9786710 байт в base64).',
     )
 
-    class Config:
-        allow_population_by_field_name = True
-
     @validator('name')
     @classmethod
     def validate_name(cls, v: str) -> str:
         if '/' in v:
             raise ValueError(f'Symbol `/` is prohibited to use inside attachment name: {v!r}.')
 
         return v
@@ -67,17 +64,14 @@
     )
     content: str = Field(
         max_length=9786710,
         description='Содержимое файла в base64 https://en.wikipedia.org/wiki/Base64. Максимальный размер '
                     'файла 7Mб (9786710 байт в base64).',
     )
 
-    class Config:
-        allow_population_by_field_name = True
-
 
 SubstitutionName: ConstrainedStr = constr(regex=r'^[a-zA-Z][a-zA-Z0-9\_]*$', strict=True)
 SubstitutionValue = Union[StrictStr | StrictFloat | StrictInt | StrictBool | None, 'Substitutions']
 
 
 class Substitutions(BaseModel):
     __root__: dict[SubstitutionName, SubstitutionValue]
```

### Comparing `unisender_go_api-0.2.0/unisender_go_api/clients.py` & `unisender_go_api-0.3.0/unisender_go_api/_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextlib import asynccontextmanager, contextmanager, AsyncExitStack  # noqa F401
 from contextvars import ContextVar, Token
-from dataclasses import dataclass, KW_ONLY, field
+from dataclasses import dataclass, field, KW_ONLY
 from typing import AsyncGenerator, ClassVar, Generator, Type, TypeVar  # noqa F401
 
 import httpx
 
 DEFAULT_UNISENDER_GO_API_ROOT_URL = 'https://go1.unisender.ru/ru/transactional/api/'
 
 SyncClientType = TypeVar('SyncClientType', bound='SyncClient')
```

### Comparing `unisender_go_api-0.2.0/unisender_go_api/exceptions.py` & `unisender_go_api-0.3.0/unisender_go_api/_exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import ABC
-from contextlib import suppress, contextmanager
 from collections.abc import Generator
-from typing import TYPE_CHECKING, Optional
+from contextlib import contextmanager, suppress
+from typing import Optional, TYPE_CHECKING
 
-from pydantic import ValidationError
 import httpx
+from pydantic import ValidationError
 
 if TYPE_CHECKING:
-    from .api_methods import ErrorResponse
+    from ._api_methods import ErrorResponse
 
 
 class UnisenderGoError(Exception, ABC):
     pass
 
 
 @UnisenderGoError.register
@@ -42,25 +42,26 @@
 
     def __init__(
         self,
         *,
         request: httpx.Request,
         response: httpx.Response,
     ) -> None:
-        from .api_methods import ErrorResponse
+        from ._api_methods import ErrorResponse
 
         self.response_payload = None
         with suppress(ValidationError):
             self.response_payload = ErrorResponse.parse_raw(response.content)
 
+        payload = self.response_payload
         message_template_lines = [
-            "Error code={payload.code!r} message={payload.message!r};" if self.response_payload else None,
             "Error occured on {request.method} {request.url}",
-            "Response HTTP status is {response.status_code} {response.reason_phrase}",
-            "Response payload: {response.text}",
+            "HTTP status code: {response.status_code} {response.reason_phrase}",
+            "Unisender Go API error: code={payload.code!r} message={payload.message!r};" if payload else None,
+            "Response payload: {response.text!r}",
             'For more information check: https://godocs.unisender.ru/web-api-ref#api-errors',
         ]
         message_template = '\n'.join(line for line in message_template_lines if line)
 
         message = message_template.format(
             payload=self.response_payload,
             request=request,
@@ -81,16 +82,16 @@
         request: httpx.Request,
         response: httpx.Response,
     ):
         self.request = request
         self.response = response
         exception_message = (
             f"Error occured on {request.method} {request.url}\n"
-            f"Response HTTP status is {response.status_code} {response.reason_phrase}\n"
-            f"Response payload: {response.text}"
+            f"HTTP status code: {response.status_code} {response.reason_phrase}\n"
+            f"Response payload: {response.text!r}"
         )
         super().__init__(exception_message)
 
     @classmethod
     @contextmanager
     def reraise_from(
         cls,
```

### Comparing `unisender_go_api-0.2.0/PKG-INFO` & `unisender_go_api-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisender-go-api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Thin wrapper for the Unisender Go API
 Home-page: https://pypi.org/project/unisender-go-api/
 License: GNU GPLv3
 Keywords: unisender,api,httpx,wrapper,asyncio
 Author: Evgeny Evseev
 Author-email: pelid80@gmail.com
 Requires-Python: >=3.10,<4.0
```


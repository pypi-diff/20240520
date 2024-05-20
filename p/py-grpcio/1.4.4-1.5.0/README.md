# Comparing `tmp/py_grpcio-1.4.4.tar.gz` & `tmp/py_grpcio-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grpcio-1.4.4.tar", max compression
+gzip compressed data, was "py_grpcio-1.5.0.tar", max compression
```

## Comparing `py_grpcio-1.4.4.tar` & `py_grpcio-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/LICENSE
--rw-r--r--   0        0        0     4581 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/README.md
--rw-r--r--   0        0        0      307 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/__init__.py
--rw-r--r--   0        0        0       60 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/__meta__.py
--rw-r--r--   0        0        0      796 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/exceptions.py
--rw-r--r--   0        0        0     1961 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/interceptor.py
--rw-r--r--   0        0        0     5102 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/method.py
--rw-r--r--   0        0        0     1148 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/middleware.py
--rw-r--r--   0        0        0     5588 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/models.py
--rw-r--r--   0        0        0      114 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/proto/__init__.py
--rw-r--r--   0        0        0      483 2024-05-16 22:24:26.765816 py_grpcio-1.4.4/py_grpcio/proto/enums.py
--rw-r--r--   0        0        0     3882 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/proto/parser.py
--rw-r--r--   0        0        0      686 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/proto/templates/service.proto.template
--rw-r--r--   0        0        0     1921 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/server.py
--rw-r--r--   0        0        0      924 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/service.py
--rw-r--r--   0        0        0     2727 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/service_meta.py
--rw-r--r--   0        0        0      582 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/py_grpcio/utils.py
--rw-r--r--   0        0        0      573 2024-05-16 22:24:26.769816 py_grpcio-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-20 21:54:18.980897 py_grpcio-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4581 2024-05-20 21:54:18.980897 py_grpcio-1.5.0/README.md
+-rw-r--r--   0        0        0      307 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/__meta__.py
+-rw-r--r--   0        0        0      796 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/exceptions.py
+-rw-r--r--   0        0        0     1961 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/interceptor.py
+-rw-r--r--   0        0        0     5102 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/method.py
+-rw-r--r--   0        0        0     1148 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/middleware.py
+-rw-r--r--   0        0        0     5588 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/models.py
+-rw-r--r--   0        0        0      114 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/proto/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/proto/enums.py
+-rw-r--r--   0        0        0     3882 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/proto/parser.py
+-rw-r--r--   0        0        0      686 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/proto/templates/service.proto.template
+-rw-r--r--   0        0        0     2798 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/server.py
+-rw-r--r--   0        0        0      924 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/service.py
+-rw-r--r--   0        0        0     2727 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/service_meta.py
+-rw-r--r--   0        0        0      582 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/py_grpcio/utils.py
+-rw-r--r--   0        0        0      573 2024-05-20 21:54:18.984897 py_grpcio-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.5.0/PKG-INFO
```

### Comparing `py_grpcio-1.4.4/LICENSE` & `py_grpcio-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/README.md` & `py_grpcio-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/exceptions.py` & `py_grpcio-1.5.0/py_grpcio/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/interceptor.py` & `py_grpcio-1.5.0/py_grpcio/interceptor.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/method.py` & `py_grpcio-1.5.0/py_grpcio/method.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/middleware.py` & `py_grpcio-1.5.0/py_grpcio/middleware.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/models.py` & `py_grpcio-1.5.0/py_grpcio/models.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/proto/parser.py` & `py_grpcio-1.5.0/py_grpcio/proto/parser.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/proto/templates/service.proto.template` & `py_grpcio-1.5.0/py_grpcio/proto/templates/service.proto.template`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/server.py` & `py_grpcio-1.5.0/py_grpcio/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-from typing import Type
 from pathlib import Path
+
 from types import ModuleType
+from typing import Type, ParamSpec, Callable, Awaitable
 
 from asyncio import AbstractEventLoop, get_event_loop
 
+from loguru import logger
+
 from grpc.aio import server
 from grpc.aio._server import Server  # noqa: _server
 
 from py_grpcio.service import BaseService
 from py_grpcio.middleware import BaseMiddleware
 from py_grpcio.interceptor import ServerInterceptor
 
+ServerParam: ParamSpec = ParamSpec('ServerParam')
+
+LifespanFunc: Type[Callable[[ServerParam], Awaitable[None]]] = Callable[[ServerParam], Awaitable[None]]
+
 
 class BaseServer:
     def __init__(
         self: 'BaseServer',
         port: int = 50051,
         proto_dir: Path = Path('proto'),
-        middlewares: set[Type[BaseMiddleware]] | None = None
+        middlewares: set[Type[BaseMiddleware]] | None = None,
+        on_startup: LifespanFunc | None = None,
+        on_shutdown: LifespanFunc | None = None
     ):
         self.port: int = port
         self.proto_dir: Path = proto_dir
         self.proto_dir.mkdir(exist_ok=True)
 
         self.loop: AbstractEventLoop = get_event_loop()
 
@@ -30,24 +39,36 @@
 
         self.services: dict[str, Type[BaseService]] = {}
 
         self.__protos: dict[str, ModuleType] = {}
         self.__services: dict[str, ModuleType] = {}
         self.middlewares: set[Type[BaseMiddleware]] = middlewares or set()
 
-    def add_service(self: 'BaseServer', service: Type[BaseService]):
+        self.on_startup: LifespanFunc | None = on_startup
+        self.on_shutdown: LifespanFunc | None = on_shutdown
+
+    def add_service(self: 'BaseServer', service: Type[BaseService]) -> None:
         self.services[service.name]: Type[BaseService] = service
         service.set_middlewares(middlewares=self.middlewares)
         service.init_protos_and_services(proto_dir=self.proto_dir)
         self.__protos[service.name], self.__services[service.name] = service.protos, service.services
         getattr(service.services, f'add_{service.name}Servicer_to_server')(servicer=service, server=self.server)
 
     async def start_server(self: 'BaseServer') -> None:
         await self.server.start()
+        logger.info('Server has been launched!')
         await self.server.wait_for_termination()
 
     def run(self: 'BaseServer') -> None:
-        self.server.add_insecure_port(f'[::]:{self.port}')
+        self.server.add_insecure_port(address=f'[::]:{self.port}')
         try:
-            self.loop.run_until_complete(self.start_server())
+            logger.info('Server starts up...')
+            if self.on_startup:
+                self.loop.run_until_complete(future=self.on_startup(server=self))
+            self.loop.run_until_complete(future=self.start_server())
+        except KeyboardInterrupt:
+            ...
         finally:
+            if self.on_shutdown:
+                self.loop.run_until_complete(future=self.on_shutdown(server=self))
+            logger.info('Server is stopped!')
             self.loop.stop()
```

### Comparing `py_grpcio-1.4.4/py_grpcio/service.py` & `py_grpcio-1.5.0/py_grpcio/service.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/service_meta.py` & `py_grpcio-1.5.0/py_grpcio/service_meta.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/py_grpcio/utils.py` & `py_grpcio-1.5.0/py_grpcio/utils.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.4/pyproject.toml` & `py_grpcio-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-grpcio"
-version = "1.4.4"
+version = "1.5.0"
 description = "gRPC with autogen by Pydantic models"
 authors = ["Yurii <ykolibroda@lytvynov-production.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "py_grpcio" },
 ]
```

### Comparing `py_grpcio-1.4.4/PKG-INFO` & `py_grpcio-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grpcio
-Version: 1.4.4
+Version: 1.5.0
 Summary: gRPC with autogen by Pydantic models
 License: MIT
 Author: Yurii
 Author-email: ykolibroda@lytvynov-production.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/fastapi_resources-0.4.9.tar.gz` & `tmp/fastapi_resources-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_resources-0.4.9.tar", max compression
+gzip compressed data, was "fastapi_resources-0.5.0.tar", max compression
```

## Comparing `fastapi_resources-0.4.9.tar` & `fastapi_resources-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2022-10-05 19:53:19.150339 fastapi_resources-0.4.9/fastapi_resources/__init__.py
--rw-r--r--   0        0        0       26 2023-11-09 18:16:44.991887 fastapi_resources-0.4.9/fastapi_resources/resources/__init__.py
--rw-r--r--   0        0        0     4979 2023-11-12 01:59:25.551967 fastapi_resources-0.4.9/fastapi_resources/resources/base_resource.py
--rw-r--r--   0        0        0       25 2023-11-09 18:16:44.992339 fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8203 2023-11-12 01:23:46.162326 fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/base.py
--rw-r--r--   0        0        0       36 2023-11-09 18:16:44.992745 fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/exceptions.py
--rw-r--r--   0        0        0     7409 2023-11-29 17:25:22.767364 fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/mixins.py
--rw-r--r--   0        0        0      553 2023-11-09 18:16:44.993163 fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/paginators.py
--rw-r--r--   0        0        0      777 2023-11-09 18:16:44.993327 fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/resources.py
--rw-r--r--   0        0        0     2405 2023-11-09 18:16:44.993495 fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/types.py
--rw-r--r--   0        0        0     1881 2023-11-29 17:08:00.200960 fastapi_resources-0.4.9/fastapi_resources/resources/types.py
--rw-r--r--   0        0        0       91 2022-10-05 19:53:19.151384 fastapi_resources-0.4.9/fastapi_resources/routers/__init__.py
--rw-r--r--   0        0        0    12820 2023-11-29 17:11:49.706472 fastapi_resources-0.4.9/fastapi_resources/routers/base_router.py
--rw-r--r--   0        0        0      859 2023-01-04 21:47:54.786676 fastapi_resources-0.4.9/fastapi_resources/routers/decorators.py
--rw-r--r--   0        0        0       51 2022-10-12 22:33:19.044947 fastapi_resources-0.4.9/fastapi_resources/routers/json_api_router/__init__.py
--rw-r--r--   0        0        0    16901 2023-11-29 17:10:39.599358 fastapi_resources-0.4.9/fastapi_resources/routers/json_api_router/json_api_router.py
--rw-r--r--   0        0        0     2341 2023-11-23 17:39:00.279502 fastapi_resources-0.4.9/fastapi_resources/routers/json_api_router/types.py
--rw-r--r--   0        0        0        0 2022-10-05 19:53:19.152483 fastapi_resources-0.4.9/fastapi_resources/types.py
--rw-r--r--   0        0        0      650 2023-11-30 18:22:54.168440 fastapi_resources-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 fastapi_resources-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-05 19:53:19.150339 fastapi_resources-0.5.0/fastapi_resources/__init__.py
+-rw-r--r--   0        0        0       26 2023-11-09 18:16:44.991887 fastapi_resources-0.5.0/fastapi_resources/resources/__init__.py
+-rw-r--r--   0        0        0     4979 2023-11-12 01:59:25.551967 fastapi_resources-0.5.0/fastapi_resources/resources/base_resource.py
+-rw-r--r--   0        0        0       25 2023-11-09 18:16:44.992339 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8203 2023-11-12 01:23:46.162326 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/base.py
+-rw-r--r--   0        0        0       36 2023-11-09 18:16:44.992745 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/exceptions.py
+-rw-r--r--   0        0        0     7440 2024-02-29 19:45:06.485617 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0      553 2023-11-09 18:16:44.993163 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/paginators.py
+-rw-r--r--   0        0        0      777 2023-11-09 18:16:44.993327 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/resources.py
+-rw-r--r--   0        0        0     2405 2023-11-09 18:16:44.993495 fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1881 2023-11-29 17:08:00.200960 fastapi_resources-0.5.0/fastapi_resources/resources/types.py
+-rw-r--r--   0        0        0       91 2022-10-05 19:53:19.151384 fastapi_resources-0.5.0/fastapi_resources/routers/__init__.py
+-rw-r--r--   0        0        0    13551 2024-05-19 23:19:50.957345 fastapi_resources-0.5.0/fastapi_resources/routers/base_router.py
+-rw-r--r--   0        0        0      897 2024-05-19 23:15:26.291112 fastapi_resources-0.5.0/fastapi_resources/routers/decorators.py
+-rw-r--r--   0        0        0       51 2022-10-12 22:33:19.044947 fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/__init__.py
+-rw-r--r--   0        0        0    17118 2023-12-10 21:30:56.451631 fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/json_api_router.py
+-rw-r--r--   0        0        0     2341 2023-11-23 17:39:00.279502 fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/types.py
+-rw-r--r--   0        0        0        0 2022-10-05 19:53:19.152483 fastapi_resources-0.5.0/fastapi_resources/types.py
+-rw-r--r--   0        0        0      630 2024-05-19 23:20:37.765483 fastapi_resources-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 fastapi_resources-0.5.0/PKG-INFO
```

### Comparing `fastapi_resources-0.4.9/fastapi_resources/resources/base_resource.py` & `fastapi_resources-0.5.0/fastapi_resources/resources/base_resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/base.py` & `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/mixins.py` & `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,16 @@
         row = self.get_object(id=id)
 
         self.session.delete(row)
         self.session.commit()
 
         return {"ok": True}
 
+
+class DeleteAllResourceMixin:
     def delete_all(self: types.SQLAlchemyResourceProtocol[types.TDb]):
         where = self.get_where()
 
         self.session.execute(delete(self.Db).where(*where))
         self.session.commit()
 
         return [], None, 0
```

### Comparing `fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/paginators.py` & `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/paginators.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/resources.py` & `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/resources.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.4.9/fastapi_resources/resources/sqlalchemy/types.py` & `fastapi_resources-0.5.0/fastapi_resources/resources/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.4.9/fastapi_resources/resources/types.py` & `fastapi_resources-0.5.0/fastapi_resources/resources/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.4.9/fastapi_resources/routers/base_router.py` & `fastapi_resources-0.5.0/fastapi_resources/routers/base_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 TResource = TypeVar("TResource", bound=ResourceProtocol)
 
 
 @runtime_checkable
 class Action(Protocol):
     detail: bool
-    methods: decorators.methods
+    methods: list[decorators.methods]
     kwargs: dict[str, Any]
 
     def __call__(self):
         ...
 
 
 class ResourceRoute(APIRoute):
@@ -190,15 +190,18 @@
 
     def _link_actions(self):
         resource_class = self.resource_class
 
         for action in inspect.getmembers(object=self):
             name, func = action
 
-            if not isinstance(func, Action):
+            # NOTE: This used to use `runtime_checkable` and `isinstance`, but it broke
+            # in 3.12. Python's docs advises to use hasattr anyway, so here we are.
+            is_action = hasattr(func, "detail") and hasattr(func, "methods")
+            if not is_action:
                 continue
 
             for method in func.methods:
                 route_method = getattr(self, method)
                 response_model = (
                     self.ReadResponseModel if func.detail else self.ListResponseModel
                 )
@@ -296,30 +299,54 @@
 
     async def perform_delete_all(self, request: Request, resource: TResource):
         if not resource.delete_all:
             raise NotImplementedError("Resource.delete_all not implemented")
 
         return await self._await_if_necessary(resource.delete_all())
 
-    async def _retrieve(self, *, id: Union[int, str], request: Request):
+    async def _retrieve(
+        self,
+        *,
+        id: Union[int, str],
+        request: Request,
+        background_tasks: BackgroundTasks,
+    ):
         resource = self.get_resource(request=request)
         if not resource.retrieve:
             raise NotImplementedError("Resource.retrieve not implemented")
 
-        row = resource.retrieve(id=id)
+        try:
+            row = resource.retrieve(id=id)
+        finally:
+            self._process_tasks(
+                background_tasks=background_tasks,
+                resource=resource,
+            )
+
         res = self.build_response(rows=row, resource=resource, request=request)
         return res
 
-    async def _list(self, *, request: Request):
+    async def _list(
+        self,
+        *,
+        request: Request,
+        background_tasks: BackgroundTasks,
+    ):
         resource = self.get_resource(request=request)
         if not resource.list:
             raise NotImplementedError("Resource.list not implemented")
 
         # Next and count are ignored in the base router
-        rows, next, count = resource.list()
+        try:
+            rows, next, count = resource.list()
+        finally:
+            self._process_tasks(
+                background_tasks=background_tasks,
+                resource=resource,
+            )
 
         return self.build_response(
             rows=rows, resource=resource, request=request, count=count, next=next
         )
 
     def _process_tasks(self, background_tasks: BackgroundTasks, resource: TResource):
         for task in resource.tasks:
```

### Comparing `fastapi_resources-0.4.9/fastapi_resources/routers/decorators.py` & `fastapi_resources-0.5.0/fastapi_resources/routers/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import functools
 from typing import Callable, Literal
 
 methods = Literal["post", "get", "patch", "delete"]
 
 
-def action(detail: bool, methods: list[methods] = ["get"], **kwargs):
+def action(detail: bool, methods: list[methods] | None = None, **kwargs):
+    methods = methods or ["get"]
+
     def action_decorator(func: Callable):
         func.detail = detail
         func.methods = methods
         func.kwargs = kwargs
 
         @functools.wraps(func)
         def wrapped(*args, **kwargs):
```

### Comparing `fastapi_resources-0.4.9/fastapi_resources/routers/json_api_router/json_api_router.py` & `fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/json_api_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,19 +477,28 @@
 
     async def _retrieve(
         self,
         *,
         id: Union[int, str],
         request: Request,
         include: Optional[str] = include_query,
+        background_tasks: BackgroundTasks,
     ):
-        return await super()._retrieve(id=id, request=request)
+        return await super()._retrieve(
+            id=id, request=request, background_tasks=background_tasks
+        )
 
-    async def _list(self, *, request: Request, include: Optional[str] = include_query):
-        return await super()._list(request=request)
+    async def _list(
+        self,
+        *,
+        request: Request,
+        include: Optional[str] = include_query,
+        background_tasks: BackgroundTasks,
+    ):
+        return await super()._list(request=request, background_tasks=background_tasks)
 
     async def _create(
         self,
         *,
         create: base_router.TCreatePayload,
         request: Request,
         include: Optional[str] = include_query,
```

### Comparing `fastapi_resources-0.4.9/fastapi_resources/routers/json_api_router/types.py` & `fastapi_resources-0.5.0/fastapi_resources/routers/json_api_router/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.4.9/pyproject.toml` & `fastapi_resources-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "fastapi-resources"
-version = "0.4.9"
+version = "0.5.0"
 description = ""
 authors = ["Ben Davis <ben@bencdavis.com>"]
 packages = [
     { include = "fastapi_resources" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-fastapi = "^0.104.0"
-sqlalchemy = "2.0.23"
+python = "^3.12"
+fastapi = "^0.111.0"
+sqlalchemy = "^2.0.30"
 pydantic = "^2.0.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-requests = "^2.26.0"
+pytest = "^8.2.1"
 pytest-clarity = "^1.0.1"
 pytest-watcher = "^0.2.1"
 debugpy = "^1.6.2"
 
 [tool.poetry.group.dev.dependencies]
 dirty-equals = "^0.5.0"
-uvicorn = {extras = ["standard"], version = "^0.15.0"}
-httpx = "^0.24.1"
+uvicorn = {extras = ["standard"], version = "^0.29.0"}
+httpx = "^0.27.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```


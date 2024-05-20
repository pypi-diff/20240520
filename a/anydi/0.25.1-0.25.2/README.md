# Comparing `tmp/anydi-0.25.1.tar.gz` & `tmp/anydi-0.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.25.1.tar", max compression
+gzip compressed data, was "anydi-0.25.2.tar", max compression
```

## Comparing `anydi-0.25.1.tar` & `anydi-0.25.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.1/LICENSE
--rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.25.1/README.md
--rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.25.1/anydi/__init__.py
--rw-r--r--   0        0        0    27996 2024-05-09 08:20:34.172615 anydi-0.25.1/anydi/_container.py
--rw-r--r--   0        0        0    10215 2024-05-08 12:47:28.300076 anydi-0.25.1/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.1/anydi/_logger.py
--rw-r--r--   0        0        0     3675 2024-05-08 08:27:43.981700 anydi-0.25.1/anydi/_module.py
--rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.25.1/anydi/_scanner.py
--rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.25.1/anydi/_types.py
--rw-r--r--   0        0        0     3692 2024-05-08 13:39:48.511132 anydi-0.25.1/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.1/anydi/ext/__init__.py
--rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.25.1/anydi/ext/django/__init__.py
--rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.25.1/anydi/ext/django/_container.py
--rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.25.1/anydi/ext/django/_settings.py
--rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.25.1/anydi/ext/django/_utils.py
--rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.25.1/anydi/ext/django/apps.py
--rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.25.1/anydi/ext/django/middleware.py
--rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.25.1/anydi/ext/django/ninja/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.25.1/anydi/ext/django/ninja/_operation.py
--rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.25.1/anydi/ext/django/ninja/_signature.py
--rw-r--r--   0        0        0     5305 2024-05-08 08:36:20.513818 anydi-0.25.1/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     3999 2024-05-08 06:51:25.864651 anydi-0.25.1/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.1/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.1/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.1/anydi/py.typed
--rw-r--r--   0        0        0     3107 2024-05-09 08:27:56.198682 anydi-0.25.1/pyproject.toml
--rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 anydi-0.25.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.2/LICENSE
+-rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.25.2/README.md
+-rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.25.2/anydi/__init__.py
+-rw-r--r--   0        0        0    27996 2024-05-09 08:20:34.172615 anydi-0.25.2/anydi/_container.py
+-rw-r--r--   0        0        0    10215 2024-05-08 12:47:28.300076 anydi-0.25.2/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.2/anydi/_logger.py
+-rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.25.2/anydi/_module.py
+-rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.25.2/anydi/_scanner.py
+-rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.25.2/anydi/_types.py
+-rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.25.2/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.2/anydi/ext/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.25.2/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.25.2/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.25.2/anydi/ext/django/_settings.py
+-rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.25.2/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.25.2/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.25.2/anydi/ext/django/middleware.py
+-rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.25.2/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.25.2/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.25.2/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     5305 2024-05-08 08:36:20.513818 anydi-0.25.2/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     4043 2024-05-20 11:14:22.992471 anydi-0.25.2/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.2/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.2/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.2/anydi/py.typed
+-rw-r--r--   0        0        0     3107 2024-05-20 11:14:36.707323 anydi-0.25.2/pyproject.toml
+-rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 anydi-0.25.2/PKG-INFO
```

### Comparing `anydi-0.25.1/LICENSE` & `anydi-0.25.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/README.md` & `anydi-0.25.2/README.md`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/__init__.py` & `anydi-0.25.2/anydi/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/_container.py` & `anydi-0.25.2/anydi/_container.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/_context.py` & `anydi-0.25.2/anydi/_context.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/_module.py` & `anydi-0.25.2/anydi/_module.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/_scanner.py` & `anydi-0.25.2/anydi/_scanner.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/_types.py` & `anydi-0.25.2/anydi/_types.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/_utils.py` & `anydi-0.25.2/anydi/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import builtins
 import functools
 import inspect
 import sys
 from typing import Any, AsyncIterator, Callable, ForwardRef, Iterator, TypeVar, cast
 
-from typing_extensions import Annotated, ParamSpec, get_origin
+from typing_extensions import ParamSpec, get_args, get_origin
 
 try:
     import anyio  # noqa
 except ImportError:
     anyio = None  # type: ignore[assignment]
 
 
@@ -29,72 +29,84 @@
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 def get_full_qualname(obj: Any) -> str:
     """Get the fully qualified name of an object."""
-    origin = get_origin(obj)
-    if origin is Annotated:
-        metadata = ", ".join(
-            [
-                f'"{arg}"' if isinstance(arg, str) else str(arg)
-                for arg in obj.__metadata__
-            ]
-        )
-        return f"Annotated[{get_full_qualname(obj.__args__[0])}, {metadata}]]"
-
     qualname = getattr(obj, "__qualname__", None)
-    module_name = getattr(obj, "__module__", None)
+    module = getattr(obj, "__module__", None)
+
     if qualname is None:
         qualname = type(obj).__qualname__
 
-    if module_name is None:
-        module_name = type(obj).__module__
+    if module is None:
+        module = type(obj).__module__
 
-    if module_name == builtins.__name__:
+    if module == builtins.__name__:
         return qualname
-    return f"{module_name}.{qualname}"
+
+    origin = get_origin(obj)
+
+    if origin:
+        args = ", ".join(
+            get_full_qualname(arg) if not isinstance(arg, str) else f'"{arg}"'
+            for arg in get_args(obj)
+        )
+        return f"{get_full_qualname(origin)}[{args}]"
+
+    return f"{module}.{qualname}"
 
 
 def is_builtin_type(tp: type[Any]) -> bool:
     """Check if the given type is a built-in type."""
     return tp.__module__ == builtins.__name__
 
 
-def make_forwardref(annotation: str, globalns: dict[str, Any]) -> Any:
-    """Create a forward reference from a string annotation."""
-    forward_ref = ForwardRef(annotation)
-    return evaluate_forwardref(forward_ref, globalns, globalns)
-
-
-def get_typed_annotation(annotation: Any, globalns: dict[str, Any]) -> Any:
+def get_typed_annotation(
+    annotation: Any,
+    globalns: dict[str, Any],
+    module: Any = None,
+    is_class: bool = False,
+) -> Any:
     """Get the typed annotation of a parameter."""
     if isinstance(annotation, str):
-        annotation = ForwardRef(annotation)
-        annotation = evaluate_forwardref(annotation, globalns, globalns)
+        if sys.version_info < (3, 9):
+            annotation = ForwardRef(annotation)
+        else:
+            annotation = ForwardRef(annotation, module=module, is_class=is_class)
+        annotation = evaluate_forwardref(annotation, globalns, {})
     return annotation
 
 
 def get_typed_return_annotation(obj: Callable[..., Any]) -> Any:
     """Get the typed return annotation of a callable object."""
     signature = inspect.signature(obj)
     annotation = signature.return_annotation
     if annotation is inspect.Signature.empty:
         return None
     globalns = getattr(obj, "__globals__", {})
-    return get_typed_annotation(annotation, globalns)
+    module = getattr(obj, "__module__", None)
+    is_class = inspect.isclass(obj)
+    return get_typed_annotation(annotation, globalns, module=module, is_class=is_class)
 
 
 def get_typed_parameters(obj: Callable[..., Any]) -> list[inspect.Parameter]:
     """Get the typed parameters of a callable object."""
     globalns = getattr(obj, "__globals__", {})
+    module = getattr(obj, "__module__", None)
+    is_class = inspect.isclass(obj)
     return [
         parameter.replace(
-            annotation=get_typed_annotation(parameter.annotation, globalns)
+            annotation=get_typed_annotation(
+                parameter.annotation,
+                globalns,
+                module=module,
+                is_class=is_class,
+            )
         )
         for name, parameter in inspect.signature(obj).parameters.items()
     ]
 
 
 _resource_origins = (
     get_origin(Iterator),
```

### Comparing `anydi-0.25.1/anydi/ext/django/_settings.py` & `anydi-0.25.2/anydi/ext/django/_settings.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/ext/django/_utils.py` & `anydi-0.25.2/anydi/ext/django/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/ext/django/apps.py` & `anydi-0.25.2/anydi/ext/django/apps.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/ext/django/middleware.py` & `anydi-0.25.2/anydi/ext/django/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/ext/django/ninja/__init__.py` & `anydi-0.25.2/anydi/ext/django/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/ext/django/ninja/_operation.py` & `anydi-0.25.2/anydi/ext/django/ninja/_operation.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/ext/django/ninja/_signature.py` & `anydi-0.25.2/anydi/ext/django/ninja/_signature.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/ext/fastapi.py` & `anydi-0.25.2/anydi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/anydi/ext/pytest_plugin.py` & `anydi-0.25.2/anydi/ext/pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import inspect
 from typing import Any, Callable, Iterator, cast
 
 import pytest
 
 from anydi import Container
+from anydi._utils import get_typed_parameters
 
 
 def pytest_configure(config: pytest.Config) -> None:
     config.addinivalue_line(
         "markers",
         "inject: mark test as needing dependency injection",
     )
@@ -59,22 +60,22 @@
 
 @pytest.fixture
 def _anydi_injected_parameter_iterator(
     request: pytest.FixtureRequest,
     _anydi_unresolved: list[str],
 ) -> Callable[[], Iterator[tuple[str, Any]]]:
     def _iterator() -> Iterator[tuple[str, inspect.Parameter]]:
-        for name, parameter in inspect.signature(request.function).parameters.items():
+        for parameter in get_typed_parameters(request.function):
             if (
                 ((interface := parameter.annotation) is parameter.empty)
                 or interface in _anydi_unresolved
-                or name in request.node.funcargs
+                or parameter.name in request.node.funcargs
             ):
                 continue
-            yield name, interface
+            yield parameter.name, interface
 
     return _iterator
 
 
 @pytest.fixture(autouse=True)
 def _anydi_inject(
     request: pytest.FixtureRequest,
```

### Comparing `anydi-0.25.1/anydi/ext/starlette/middleware.py` & `anydi-0.25.2/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.1/pyproject.toml` & `anydi-0.25.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.25.1"
+version = "0.25.2"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
```

### Comparing `anydi-0.25.1/PKG-INFO` & `anydi-0.25.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.25.1
+Version: 0.25.2
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
```


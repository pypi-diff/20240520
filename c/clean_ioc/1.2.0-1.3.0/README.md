# Comparing `tmp/clean_ioc-1.2.0.tar.gz` & `tmp/clean_ioc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-1.2.0.tar", max compression
+gzip compressed data, was "clean_ioc-1.3.0.tar", max compression
```

## Comparing `clean_ioc-1.2.0.tar` & `clean_ioc-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4195 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/CHANGES.rst
--rw-r--r--   0        0        0     1067 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/LICENSE
--rw-r--r--   0        0        0    17357 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/README.md
--rw-r--r--   0        0        0       20 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/__init__.py
--rw-r--r--   0        0        0     2118 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/bundles.py
--rw-r--r--   0        0        0    62229 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/core.py
--rw-r--r--   0        0        0       20 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/ext/fastapi/__init__.py
--rw-r--r--   0        0        0     2259 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/ext/fastapi/core.py
--rw-r--r--   0        0        0     1344 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/ext/fastapi/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/ext/fastapi/py.typed
--rw-r--r--   0        0        0     1262 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/factories.py
--rw-r--r--   0        0        0     2662 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0      563 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/list_reduction_filters.py
--rw-r--r--   0        0        0     1779 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/node_filters.py
--rw-r--r--   0        0        0        0 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/py.typed
--rw-r--r--   0        0        0     4807 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      962 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6920 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1828 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/utils.py
--rw-r--r--   0        0        0      564 2024-05-13 23:05:42.584916 clean_ioc-1.2.0/clean_ioc/value_factories.py
--rw-r--r--   0        0        0     2243 2024-05-13 23:05:42.588916 clean_ioc-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    18211 1970-01-01 00:00:00.000000 clean_ioc-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4195 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/CHANGES.rst
+-rw-r--r--   0        0        0     1067 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2470 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/README.md
+-rw-r--r--   0        0        0       20 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/bundles.py
+-rw-r--r--   0        0        0    61208 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/core.py
+-rw-r--r--   0        0        0       20 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     2259 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/ext/fastapi/core.py
+-rw-r--r--   0        0        0     1344 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/ext/fastapi/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/ext/fastapi/py.typed
+-rw-r--r--   0        0        0     1262 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/factories.py
+-rw-r--r--   0        0        0     2662 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0      563 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/list_reduction_filters.py
+-rw-r--r--   0        0        0     1779 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/node_filters.py
+-rw-r--r--   0        0        0        0 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/py.typed
+-rw-r--r--   0        0        0     6229 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      962 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6920 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1828 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/utils.py
+-rw-r--r--   0        0        0      564 2024-05-20 15:51:15.688923 clean_ioc-1.3.0/clean_ioc/value_factories.py
+-rw-r--r--   0        0        0     2271 2024-05-20 15:51:15.784923 clean_ioc-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 clean_ioc-1.3.0/PKG-INFO
```

### Comparing `clean_ioc-1.2.0/CHANGES.rst` & `clean_ioc-1.3.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/LICENSE` & `clean_ioc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/bundles.py` & `clean_ioc-1.3.0/clean_ioc/bundles.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/core.py` & `clean_ioc-1.3.0/clean_ioc/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import logging
 import types
 from collections import defaultdict, deque
 from collections.abc import Callable, Collection, Iterable, MutableSequence, Sequence
 from contextlib import contextmanager
 from dataclasses import dataclass
 from enum import IntEnum
-from functools import reduce
 from typing import (
     Any,
     ClassVar,
     Protocol,
     TypeVar,
     _GenericAlias,  # type: ignore
     get_type_hints,
@@ -132,23 +131,22 @@
 ) -> dict[str, Any]:
     kwargs = {}
     for arg_name, arg_dep in dependencies.items():
         kwargs[arg_name] = await arg_dep.resolve_async(context, dependency_node)
     return kwargs
 
 
-def default_registration_filter(r: _Registration) -> bool:
-    return not r.is_named
+def default_registration_filter(r: Registration) -> bool:
+    return r.name is None
 
 
-def default_dependency_value_factory(default_value: Any, _: DependencyContext) -> Any:
+def default_parameter_value_factory(default_value: Any, _: DependencyContext) -> Any:
     return default_value
 
 
-default_registration_list_reducing_filter = constant(True)
 default_parent_node_filter = constant(True)
 default_decorated_node_filter = constant(True)
 
 
 @dataclass
 class Tag:
     name: str
@@ -503,15 +501,14 @@
         if self.is_dependency_context:
             return DependencyContext(name=self.name, dependency_node=dependency_node)
 
         if self.generic_collection_type:
             regs = context.find_registrations(
                 service_type=self.service_type.__args__[0],  # type: ignore
                 registration_filter=self.settings.filter,
-                registration_list_reducing_filter=self.settings.list_reducing_filter,
                 parent_node=dependency_node,
             )
             sequence_node = DependencyNode(
                 service_type=self.service_type,
                 implementation=self.generic_collection_type,
                 lifespan=Lifespan.transient,
             )
@@ -544,15 +541,14 @@
         if self.is_dependency_context:
             return DependencyContext(name=self.name, dependency_node=dependency_node)
 
         if self.generic_collection_type:
             regs = context.find_registrations(
                 service_type=self.service_type.__args__[0],  # type: ignore
                 registration_filter=self.settings.filter,
-                registration_list_reducing_filter=self.settings.list_reducing_filter,
                 parent_node=dependency_node,
             )
             sequence_node = DependencyNode(
                 service_type=self.service_type,
                 implementation=self.generic_collection_type,
                 lifespan=Lifespan.transient,
             )
@@ -804,18 +800,14 @@
 
 
 class Registration(Protocol):
     service_type: type
     implementation: Callable
     lifespan: Lifespan
     name: str | None
-    is_named: bool
-    parent_node_filter: NodeFilter
-    tags: Iterable[Tag]
-    scoped_teardown: Callable | None
     generic_mapping: GenericTypeMap
 
     def has_tag(self, name: str, value: Any) -> bool: ...
 
 
 class _Registration(Registration):
     __slots__ = (
@@ -1207,15 +1199,14 @@
         service_type: type,
         registration_filter: Callable,
         parent_node: DependencyNode,
     ) -> _Registration:
         regs = self.find_registrations(
             service_type=service_type,
             registration_filter=registration_filter,
-            registration_list_reducing_filter=constant(True),
             parent_node=parent_node,
         )
         reg = next(iter(regs), None)
 
         if reg is None:
             if type(service_type) == _GenericAlias:
                 reg = self.try_generic_fallback(service_type, parent_node)
@@ -1223,27 +1214,20 @@
                 raise CannotResolveError()
         return reg
 
     def find_registrations(
         self,
         service_type: type,
         registration_filter: Callable[[_Registration], bool],
-        registration_list_reducing_filter: Callable[[_Registration, Iterable[_Registration]], bool],
         parent_node: DependencyNode,
     ) -> list[_Registration]:
         registrations = self.scope.find_registrations(
             service_type=service_type, parent_node=parent_node, filter=registration_filter
         )
-
-        def reducer(accumulator: list[_Registration], registration: _Registration) -> list[_Registration]:
-            if registration_list_reducing_filter(registration, accumulator):
-                accumulator.append(registration)
-            return accumulator
-
-        return reduce(reducer, registrations, [])
+        return registrations
 
     def find_decorators_that_apply(
         self, registration: _Registration, decorated_instance_node: DependencyNode
     ) -> list[Decorator]:
         return self.scope.find_decorators(registration=registration, decorated_instance_node=decorated_instance_node)
 
     def find_pre_configurations_that_apply(self, registration: _Registration):
@@ -1765,17 +1749,15 @@
 
     def new_scope(self) -> Scope:
         return ChildScope(self)
 
 
 @dataclass(kw_only=True)
 class DependencySettings:
-    value_factory: DependencyValueFactory = default_dependency_value_factory
+    value_factory: ParameterValueFactory = default_parameter_value_factory
     filter: RegistrationFilter = default_registration_filter
-    list_reducing_filter: RegistrationListReducingFilter = default_registration_list_reducing_filter
 
 
 DependencyConfig = dict[str, DependencySettings]
 RegistrationFilter = Callable[[_Registration], bool]
-RegistrationListReducingFilter = Callable[[_Registration, Iterable[_Registration]], bool]
 NodeFilter = Callable[[Node], bool]
-DependencyValueFactory = Callable[[Any, DependencyContext], Any]
+ParameterValueFactory = Callable[[Any, DependencyContext], Any]
```

### Comparing `clean_ioc-1.2.0/clean_ioc/ext/fastapi/core.py` & `clean_ioc-1.3.0/clean_ioc/ext/fastapi/core.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/ext/fastapi/dependencies.py` & `clean_ioc-1.3.0/clean_ioc/ext/fastapi/dependencies.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/factories.py` & `clean_ioc-1.3.0/clean_ioc/factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/functional_utils.py` & `clean_ioc-1.3.0/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/list_reduction_filters.py` & `clean_ioc-1.3.0/clean_ioc/list_reduction_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/node_filters.py` & `clean_ioc-1.3.0/clean_ioc/node_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 def registration_name_is(name: str):
     def inner(node: Node):
         return node.registration_name == name
 
     return predicate(inner)
 
 
-def has_registartion_tag(name: str, value: str | None = None):
+def has_registration_tag(name: str, value: str | None = None):
     def inner(node: Node):
         return node.has_registration_tag(name, value)
 
     return predicate(inner)
 
 
 def has_dependant_service_type(service_type: type):
```

### Comparing `clean_ioc-1.2.0/clean_ioc/registration_filters.py` & `clean_ioc-1.3.0/clean_ioc/registration_filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 import inspect
+from collections.abc import Iterable
 from typing import Callable, TypeVar
 
-from .core import Registration
+from .core import Lifespan, Registration
 from .functional_utils import constant, predicate
 
 all_registrations = constant(True)
 
 
+def create_filter(func: Callable[[Registration], bool]):
+    return predicate(func)
+
+
 def with_name(name: str | None):
     """
     Filter registrations equal the name
     """
 
-    def inner(r: Registration):
+    def _with_name(r: Registration):
         return r.name == name
 
-    return predicate(inner)
+    return predicate(_with_name)
 
 
 def name_starts_with(prefix: str):
     """
     Filter registrations where the name starts the prefix
     """
 
-    def inner(r: Registration):
+    def _name_starts_with(r: Registration):
         if r.name is not None:
             return r.name.startswith(prefix)
         return False
 
-    return predicate(inner)
+    return predicate(_name_starts_with)
 
 
 def name_ends_with(suffix: str):
     """
     Filter registrations where the name ends the suffix
     """
 
-    def inner(r: Registration):
+    def _name_ends_with(r: Registration):
         if r.name is not None:
             return r.name.endswith(suffix)
         return False
 
-    return predicate(inner)
+    return predicate(_name_ends_with)
 
 
-def _is_named(r: Registration):
-    """
-    Filter registrations that have a name
-    """
-    return r.is_named
-
-
-is_named = predicate(_is_named)
 is_not_named = with_name(None)
+is_not_named.__doc__ = "Filter for registrations that do not have a name"
+
+is_named = ~is_not_named
+is_named.__doc__ = "Filter for registrations that have a name"
 
 
 def with_implementation(implementation: type):
     """
     Filter to registrations that have the implementation
     """
 
-    def inner(r: Registration):
+    def _with_implementation(r: Registration):
         return r.implementation == implementation
 
-    return predicate(inner)
+    return predicate(_with_implementation)
 
 
 def with_implementation_matching_filter(type_filter: Callable[[type], bool]):
     """
     Returns a filter function that checks if the implementation of a given registration matches a specified type filter.
 
     Parameters:
@@ -81,21 +82,21 @@
     Example:
         >>> type_filter = lambda x: issubclass(x, int)
         >>> registration = Registration(implementation=123)
         >>> with_implementation_matching_filter(type_filter)(registration)
         True
     """
 
-    def inner(r: Registration):
+    def _with_implementation_matching_filter(r: Registration):
         if inspect.isfunction(r.implementation):
             return False
 
         return type_filter(r.implementation)  # type: ignore
 
-    return predicate(inner)
+    return predicate(_with_implementation_matching_filter)
 
 
 def has_generic_args_matching(pair: tuple[TypeVar | str, type]):
     """
     Filter registrations where generic type arg matches
     >>> TBar = TypeVar("TBar")
     >>> class Foo(Generic[TBar]):
@@ -105,18 +106,18 @@
     >>> class StringFoo(Foo[str]):
     ...    pass
     >>> container.register(Foo, IntFoo)
     >>> container.register(Foo, StringFoo)
     >>> container.resolve(Foo, filter=has_generic_args_matching((TBar, int))) # returns instance of IntFoo
     """
 
-    def inner(r: Registration):
+    def _has_generic_args_matching(r: Registration):
         return r.generic_mapping.get(pair[0]) == pair[1]
 
-    return predicate(inner)
+    return predicate(_has_generic_args_matching)
 
 
 def has_tag(name: str, value: str | None = None):
     """
     Check if a given registration has a specific tag.
 
     Parameters:
@@ -124,18 +125,18 @@
         value (str | None, optional): The value of the tag to check for. Defaults to None.
 
     Returns:
         Callable[[Registration], bool]: A filter function that takes a registration and returns True
         if the registration has the specified tag, False otherwise.
     """
 
-    def inner(r: Registration):
+    def _has_tag(r: Registration):
         return r.has_tag(name, value)
 
-    return predicate(inner)
+    return predicate(_has_tag)
 
 
 def has_tag_with_value_or_missing_tag(name: str, value: str):
     """
     Check if a given registration has a specific tag with a given value or if it does not have that tag.
 
     Parameters:
@@ -159,11 +160,47 @@
 
     Returns:
         Callable[[Registration], bool]: A filter function that takes a registration and returns True if
         the registration has the specified tag with a value that matches any of the given values, False otherwise.
     """
     predicates = [has_tag(name, v) for v in values]
 
-    def inner(r: Registration):
+    def _has_tag_with_value_in(r: Registration):
         return any([p(r) for p in predicates])
 
-    return predicate(inner)
+    return predicate(_has_tag_with_value_in)
+
+
+def has_lifespan(lifespan: Lifespan):
+    """
+    Check if a given registration has a specific lifespan.
+
+    Parameters:
+        lifespan (str): The lifespan to check for.
+
+    Returns:
+        Callable[[Registration], bool]: A filter function that takes a registration and returns True
+        if the registration has the specified lifespan, False otherwise.
+    """
+
+    def _has_lifespan(r: Registration):
+        return r.lifespan == lifespan
+
+    return predicate(_has_lifespan)
+
+
+def has_lifespan_in(lifespans: Iterable[Lifespan]):
+    """
+    Returns a predicate function that checks if the lifespan of a registration is in the given lifespans.
+
+    Args:
+        lifespans (Iterable[Lifespan]): The lifespans to check against.
+
+    Returns:
+        Callable[[Registration], bool]: A predicate function that returns True if the lifespan of a registration
+        is in the given lifespans, False otherwise.
+    """
+
+    def _has_lifespans(r: Registration):
+        return r.lifespan in lifespans
+
+    return predicate(_has_lifespans)
```

### Comparing `clean_ioc-1.2.0/clean_ioc/type_filters.py` & `clean_ioc-1.3.0/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/typing_utils.py` & `clean_ioc-1.3.0/clean_ioc/typing_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/utils.py` & `clean_ioc-1.3.0/clean_ioc/utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/clean_ioc/value_factories.py` & `clean_ioc-1.3.0/clean_ioc/value_factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-1.2.0/pyproject.toml` & `clean_ioc-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "1.2.0"
+version = "1.3.0"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://peter-daly.github.io/clean_ioc/"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://peter-daly.github.io/clean_ioc/"
 readme = "README.md"
@@ -29,16 +29,17 @@
 fastapi = "^0.101.0"
 httpx = "^0.26.0"
 pyright = "^1.1.362"
 ruff = "^0.4.3"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
-mkdocstrings = {version = "^0.24.0", extras = ["python"]}
+mkdocstrings = {version = "^0.25.0", extras = ["python"]}
 mkdocs-material = "^9.5.9"
+mkdocs-glightbox = "^0.4.0"
 
 
 [tool.poetry.group.dev]
 optional = true
 
 
 [tool.poetry.extras]
```


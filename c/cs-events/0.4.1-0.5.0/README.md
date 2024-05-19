# Comparing `tmp/cs_events-0.4.1.tar.gz` & `tmp/cs_events-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs_events-0.4.1.tar", max compression
+gzip compressed data, was "cs_events-0.5.0.tar", max compression
```

## Comparing `cs_events-0.4.1.tar` & `cs_events-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-03-27 01:32:35.282886 cs_events-0.4.1/LICENSE
--rw-r--r--   0        0        0     1323 2023-04-16 14:04:20.620131 cs_events-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6756 2023-03-27 01:05:01.123372 cs_events-0.4.1/README.md
--rw-r--r--   0        0        0      495 2023-04-16 14:04:20.626131 cs_events-0.4.1/src/events/__init__.py
--rw-r--r--   0        0        0     3655 2023-04-01 15:38:35.471687 cs_events-0.4.1/src/events/_collections.py
--rw-r--r--   0        0        0     7134 2023-04-01 15:37:38.747157 cs_events-0.4.1/src/events/_event.py
--rw-r--r--   0        0        0     6948 2023-04-16 14:01:05.944034 cs_events-0.4.1/src/events/_events.py
--rw-r--r--   0        0        0     7739 1970-01-01 00:00:00.000000 cs_events-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-06 00:41:51.879016 cs_events-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1370 2024-05-19 22:20:22.339646 cs_events-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6826 2024-04-27 23:59:00.416180 cs_events-0.5.0/README.md
+-rw-r--r--   0        0        0      664 2024-05-19 22:20:22.339646 cs_events-0.5.0/src/events/__init__.py
+-rw-r--r--   0        0        0     4540 2024-05-19 22:20:22.339646 cs_events-0.5.0/src/events/_collections.py
+-rw-r--r--   0        0        0     3768 2024-05-19 22:20:22.341148 cs_events-0.5.0/src/events/_common.py
+-rw-r--r--   0        0        0     3798 2024-05-19 22:20:22.341148 cs_events-0.5.0/src/events/_field.py
+-rw-r--r--   0        0        0     7441 2024-05-19 22:20:22.341148 cs_events-0.5.0/src/events/_property.py
+-rw-r--r--   0        0        0     7585 2024-05-19 22:20:22.341148 cs_events-0.5.0/src/events/_utils.py
+-rw-r--r--   0        0        0     7712 1970-01-01 00:00:00.000000 cs_events-0.5.0/PKG-INFO
```

### Comparing `cs_events-0.4.1/LICENSE` & `cs_events-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cs_events-0.4.1/pyproject.toml` & `cs_events-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cs-events"
-version = "0.4.1"
+version = "0.5.0"
 description = "C#-style event handling mechanism for Python"
 authors = ["Daniel Jeong <wise0704@outlook.com>"]
 keywords = ["python", "event", "c#"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/wise0704/python-cs-events"
 classifiers = [
@@ -16,24 +16,25 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries",
     "Typing :: Typed",
 ]
 packages = [
     { include = "events", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typing-extensions = { version = "^4.0.1", python = "<3.11" }
+typing-extensions = { version = "^4.0.1", python = "<3.12" }
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest = "^7.2.1"
 
 [tool.poetry.urls]
 "Issues" = "https://github.com/wise0704/python-cs-events/issues"
```

### Comparing `cs_events-0.4.1/README.md` & `cs_events-0.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -37,72 +37,72 @@
 
 Python does not support an addition of two `Callable` types.
 So the `Event[**TArgs]` class is provided to mimic delegates:
 
 ```python
 from events import Event
 
-changed = Event[str, object]()
+item_changed = Event[str, object]()
 ```
 
 > C# naming convention prefers present/past participles (`changing`/`changed`) instead of `on`+infinitive (`on_change`) for events.
 
 Handlers can subscribe to and unsubscribe from the event with the same syntax:
 
 ```python
-def changed_handler(key: str, value: object) -> None:
+def item_changed_handler(key: str, value: object) -> None:
     ...
 
-changed += changed_handler
-changed -= changed_handler
+item_changed += item_changed_handler
+item_changed -= item_changed_handler
 ```
 
 An event can be raised by simply invoking it with the arguments:
 
 ```python
-changed("state", obj)
+item_changed("info", obj)
 ```
 
 Since `Event` acts just like a delegate from C#, it is not required to be bound to a class or an instance object.
 This is the major difference to other packages that try to implement the C#-style event system, which usually revolve around a container object for events.
 
 An example class with event fields may look like this:
 
 ```python
 class EventExample:
     def __init__(self) -> None:
+        self.__value = ""
         self.updated: Event[str] = Event()
-        self.__value: str = ""
 
     def update(self, value: str) -> None:
         if self.__value != value:
             self.__value = value
             self.updated(value)
 
 obj = EventExample()
 obj.updated += lambda value: print(f"obj.{value=}")
 obj.update("new value")
 ```
 
-A class decorator `@events` is provided as a shortcut for event fields:
+A class decorator `@events` is provided as a shortcut for **event fields**:
 
 ```python
 from events import Event, events
 
 @events
 class EventFieldsExample:
     item_added: Event[object]
     item_removed: Event[object]
-    item_updated: Event[object, str]
+    item_updated: Event[str, object]
 ```
 
-C# also provides event properties with `add` and `remove` accessors:
+C# also provides **event properties** with `add` and `remove` accessors:
 
 ```C#
-public event EventHandler<T> Changed
+public event EventHandler<ItemChangedEventArgs> ItemChanged
 {
     add { ... }
     remove { ... }
 }
 ```
 
 This feature is useful for classes that do not actually own the events, but need to forward the subscriptions to the underlying object that do own the events.
@@ -110,62 +110,60 @@
 The `@event[**TArgs]` decorator and the `accessors[**TArgs]` type are provided to support this feature:
 
 ```python
 from events import accessors, event, EventHandler
 
 class EventPropertyExample:
     @event[str, object]
-    def changed() -> accessors[str, object]:
-        def add(self: Self, value: EventHandler[str, object]) -> None:
-            ...
-        def remove(self: Self, value: EventHandler[str, object]) -> None:
-            ...
+    def item_changed() -> accessors[str, object]:
+        def add(self: Self, value: EventHandler[str, object]) -> None: ...
+        def remove(self: Self, value: EventHandler[str, object]) -> None: ...
         return (add, remove)
 ```
 
 Furthermore, the `EventHandlerCollection` interface is provided to support the functionalities of `System.ComponentModel.EventHandlerList` class from C#, along with the two implementations `EventHandlerList` and `EventHandlerDict` using a linked list and a dictionary respectively. The behaviour of `EventHandlerList` is exactly the same as of its counterpart from C#.
 
 A typical usage of `EventHandlerList` in C# can be translated directly into the python code:
 
 ```python
 class EventPropertyExample:
-    __event_changed: Final = object()
+    __event_item_changed: Final = object()
+
+    def __init__(self) -> None:
+        self.__events = EventHandlerList()
 
     @event  # [str, object] is inferred
-    def changed():  # -> accessors[str, object] is inferred
+    def item_changed():  # -> accessors[str, object] is inferred
         def add(self: Self, value: EventHandler[str, object]) -> None:
-            self.__events.add_handler(self.__event_changed, value)
+            self.__events.add_handler(self.__event_item_changed, value)
 
         def remove(self: Self, value: EventHandler[str, object]) -> None:
-            self.__events.remove_handler(self.__event_changed, value)
+            self.__events.remove_handler(self.__event_item_changed, value)
 
         return (add, remove)
-    
-    def __init__(self) -> None:
-        self.__events = EventHandlerList()
-    
-    def perform_change(self, key: str, value: object) -> None:
-        handler = self.__events[self.__event_changed]
+
+    def _on_item_changed(self, key: str, value: object) -> None:
+        handler = self.__events[self.__event_item_changed]
         if handler:
             handler(key, value)
 ```
 
 The class decorator `@events` also provides a shortcut for event properties.
 The above code can be shortened to:
 
 ```python
 @events(collection="__events")
 class EventPropertyExample:
-    changed: event[str, object]
+    item_changed: event[str, object]
 
     def __init__(self) -> None:
         self.__events = EventHandlerList()
 
-    def perform_change(self, key: str, value: object) -> None:
-        self.__events.invoke("changed", key, value)
+    def _on_item_changed(self, key: str, value: object) -> None:
+        self.__events.invoke("item_changed", key, value)
 ```
 
 ## Installation
 
 Install using [`pip`](https://pypi.org/project/pip/):
 
 ```console
```

### Comparing `cs_events-0.4.1/src/events/_collections.py` & `cs_events-0.5.0/src/events/_collections.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,139 +1,168 @@
+import sys
+from abc import ABC, abstractmethod
 from collections.abc import Callable
-from typing import TYPE_CHECKING, Protocol, Union, runtime_checkable
+from typing import TYPE_CHECKING, Union
 
-from ._event import Event
+from ._common import Delegate
+from ._field import Event
+
+
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
 
 
 __all__ = [
     "EventHandlerCollection",
     "EventHandlerList",
     "EventHandlerDict",
 ]
 
 
-void = object
-
-
-@runtime_checkable
-class EventHandlerCollection(Protocol):
+class EventHandlerCollection(ABC):
     """
     Provides a collection of event handler delegates.
     """
 
-    __slots__ = ()
+    __slots__ = []
 
-    def __getitem__(self, key: object, /) -> Event[...] | None:
+    @abstractmethod
+    def __getitem__(self, key: object, /) -> Delegate | None:
         """
         Gets the event for the specified key.
 
         Args:
-         - key (object): A key to find in the list.
+            key (object): A key to find in the collection.
 
         Returns:
-            (Event[...]?): The event for the specified key, or ``None`` if an event does not exist.
+            Delegate | None: The event for the specified key, or `None` if an event does not exist.
         """
 
-        ...
+        raise NotImplementedError
 
-    def add_handler(self, key: object, value: Callable[..., void], /) -> None:
+    @abstractmethod
+    def add_handler(self, key: object, value: Callable, event_type: type[Delegate] = Event, /) -> None:
         """
-        Adds the delegate to the list.
+        Adds the delegate to the collection.
 
         Args:
-         - key (object): A key that owns the event.
-         - value ((...) -> void): A delegate to add to the list.
+            key(object): A key that owns the event.
+            value((...) -> Unknown): A delegate to add to the collection.
+            event_type (type[Delegate], optional): The type of the event. Defaults to `Event`.
         """
 
-        ...
+        raise NotImplementedError
 
-    def remove_handler(self, key: object, value: Callable[..., void], /) -> None:
+    def remove_handler(self, key: object, value: Callable, /) -> None:
         """
-        Removes the delegate from the list.
+        Removes the delegate from the collection.
 
         Args:
          - key (object): A key that owns the event.
-         - value ((...) -> void): A delegate to remove from the list.
+         - value ((...) -> Unknown): A delegate to remove from the collection.
         """
 
         if (e := self[key]) is not None:
             e -= value
 
     def invoke(self, key: object, /, *args, **kwargs) -> None:
         """
-        Invokes an event from the list.
+        Invokes an event from the collection.
 
         Equivalent to::
 
             e = events[key]
             if e is not None:
                 e(...)
 
         This method is provided as a shortcut to above,
         since python does not have null-conditional operators::
 
             events[key]?.__call__(...)  # C# style func?.Invoke(...)
-            events[key]?.(...)  # JavaScript style func?.(...)
+            events[key]?.(...)          # JS/TS style func?.(...)
 
         Args:
-         - key (object): A key that owns the event.
+            key (object): A key that owns the event.
         """
 
         if (e := self[key]) is not None:
             e(*args, **kwargs)
 
+    async def invoke_async(self, key: object, /, *args, **kwargs) -> None:
+        """
+        Asynchronously invokes an event from the collection.
+
+        Equivalent to::
+
+            e = events[key]
+            if e is not None:
+                await e(...)
+
+        Args:
+            key (object): A key that owns the event.
+        """
+
+        if (e := self[key]) is not None:
+            await e(*args, **kwargs)
+
 
 if TYPE_CHECKING:
-    ListEntry = tuple[object, Event[...], Union["ListEntry", None]]
+    ListEntry = tuple[object, Delegate, Union["ListEntry", None]]
 
 
 class EventHandlerList(EventHandlerCollection):
     """
     Provides a simple linked list of event handler delegates.
     """
 
-    __slots__ = ("__head")
+    __slots__ = ["__head"]
 
     def __init__(self) -> None:
         """
-        Initializes a new instance of the ``EventHandlerList`` class.
+        Initializes a new instance of the `EventHandlerList` class.
         """
 
         self.__head: ListEntry | None = None
 
-    def __getitem__(self, key: object, /) -> Event[...] | None:
+    @override
+    def __getitem__(self, key: object, /) -> Delegate | None:
         next = self.__head
         while next is not None:
             (k, e, next) = next
-            if k == key:  # use __eq__ instead of "is"
+            if k == key:
                 return e
         return None
 
-    def add_handler(self, key: object, value: Callable[..., void], /) -> None:
+    @override
+    def add_handler(self, key: object, value: Callable, event_type: type[Delegate] = Event, /) -> None:
         if (e := self[key]) is None:
-            self.__head = (key, Event(value), self.__head)
+            self.__head = (key, event_type(value), self.__head)
         else:
             e += value
 
 
 class EventHandlerDict(EventHandlerCollection):
     """
     Provides a simple dictionary of event handler delegates.
     """
 
-    __slots__ = ("__dict")
+    __slots__ = ["__dict"]
 
     def __init__(self) -> None:
         """
-        Initializes a new instance of the ``EventHandlerDict`` class.
+        Initializes a new instance of the `EventHandlerDict` class.
         """
 
-        self.__dict: dict[object, Event[...]] = {}
+        self.__dict: dict[object, Delegate] = {}
 
-    def __getitem__(self, key: object, /) -> Event[...] | None:
+    @override
+    def __getitem__(self, key: object, /) -> Delegate | None:
         return self.__dict.get(key)
 
-    def add_handler(self, key: object, value: Callable[..., void], /) -> None:
+    @override
+    def add_handler(self, key: object, value: Callable, event_type: type[Delegate] = Event, /) -> None:
         if (e := self[key]) is None:
-            self.__dict[key] = Event(value)
+            self.__dict[key] = event_type(value)
         else:
             e += value
```

### Comparing `cs_events-0.4.1/src/events/_event.py` & `cs_events-0.5.0/src/events/_property.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,240 +1,226 @@
 import sys
-from collections.abc import Callable, Collection, Iterator
-from typing import Generic, ParamSpec, final, overload
+from collections.abc import Callable
+from typing import Any, Generic, Literal, ParamSpec, TypeAlias, overload
 
+from ._common import void
+from ._field import AsyncEventHandler, EventHandler
 
-if sys.version_info >= (3, 11):
-    from typing import Self
+
+if sys.version_info >= (3, 12):
+    from typing import Self, override
 else:
-    from typing_extensions import Self
+    from typing_extensions import Self, override
 
 
 __all__ = [
-    "accessors",
+    "async_event",
     "event",
-    "Event",
-    "EventHandler",
 ]
 
 
-# Python does not provide a void type, which is a useful feature in callbacks,
-# and is clearly different from None.
-# Comparison with TS:
-#     function foo(): void {} <==> def foo() -> None: pass
-#     let bar: () => void;    <==> bar: Callable[[], Any]
-void = object
 P = ParamSpec("P")
-
-EventHandler = Callable[P, void]
-accessors = tuple[Callable[[object, EventHandler[P]], void], Callable[[object, EventHandler[P]], void]]
+add: TypeAlias = tuple[EventHandler[P], Literal[True]]
+remove: TypeAlias = tuple[EventHandler[P], Literal[False]]
 
 
-class Event(Collection[EventHandler[P]]):
+class event(Generic[P]):
     """
-    Represents an event delegate that handlers can subscribe to.
-
-    The type argument specifies the event data parameters::
-
-        event = Event[str, int]()
-        # accepts handlers (str, int) -> void
-
-    Handlers can subscribe to and unsubscribe from an event by::
-
-        event += event_handler
-        event -= event_handler
+    A decorator used to declare an event property in a publisher class.
 
-    An event can be raised by invoking itself with the necessary arguments::
+    The definition function must return a tuple of accessors `(add, remove)`
+    each of type `(Self, (**P) -> void) -> void`.
 
-        event(...)
+    The subscribe and unsubscribe operators::
 
-    Type Args:
-     - **P (ParamSpec): Event data parameter specification.
-    """
+        obj.event += handler
+        obj.event -= handler
 
-    __slots__ = ("__handlers")
+    will invoke the respective `add` and `remove` accessors with the arguments
+    `(obj, handler)`.
 
-    __handlers: list[EventHandler[P]]
+    An event property is not bound to an instance object, thus it must be
+    accessed as an attribute of an object in order for the accessors to be
+    invoked. The following code::
 
-    def __init__(self, *handlers: EventHandler[P]) -> None:
-        """
-        Initializes a new instance of the ``Event`` class.
+        e = obj.event
+        e += handler  # no reference to obj!
 
-        Args:
-         - *handlers ((**P) -> void): List of handlers to subscribe to the event.
-        """
+    has no effect on `obj.event` and will not call the `add` accessor,
+    since the argument `self` is not supplied.
 
-        self.__handlers = [*handlers]
+    Unlike event fields, an event property cannot be invoked directly.
+    Use the underlying event object that the accessors point to instead.
 
-    def __iadd__(self, value: EventHandler[P], /) -> Self:
-        """
-        Subscribes the handler to this event.
+    Example::
 
-        Args:
-         - value ((**P) -> void): An event handler.
+        class Example:
+            # Infer event handler type from the accessor parameter type
+            @event
+            def item_added():
+                def add(self: Self, value: EventHandler[int, object]) -> None:
+                    ...
+                def remove(self: Self, value: EventHandler[int, object]) -> None:
+                    ...
+                return (add, remove)
 
-        Returns:
-            (Self): This event.
-        """
+    Type Args:
+        **P: Event handler parameter specification.
+    """
 
-        self.__handlers.append(value)
-        return self
+    __slots__ = ["__add", "__remove"]
 
-    def __isub__(self, value: EventHandler[P], /) -> Self:
+    @overload
+    def __init__(self, definition: Callable[[], tuple[Callable[[Any, EventHandler[P]], void], Callable[[Any, EventHandler[P]], void]]], /) -> None:
         """
-        Unsubscribes the handler from this event.
-
-        If the handler has been added multiple times, removes only the last occurrence.
+        Initializes a new instance of the `event` class.
 
         Args:
-         - value ((**P) -> void): An event handler
-
-        Returns:
-            (Self): This event
+            definition (() -> tuple[(Self, (**P) -> void) -> void, (Self, (**P) -> void) -> void]):
+            An event definition returning a tuple of add and remove accessors.
         """
 
-        for i in range(len(self.__handlers) - 1, -1, -1):
-            if self.__handlers[i] is value:
-                del self.__handlers[i]
-                break
-        return self
-
-    def __contains__(self, obj: object, /) -> bool:
+    @overload
+    def __init__(self, accessors: tuple[Callable[[Any, EventHandler[P]], void], Callable[[Any, EventHandler[P]], void]], /) -> None:
         """
-        Returns whether the handler has been subscribed to this event.
+        Initializes a new instance of the `event` class.
 
         Args:
-         - obj (object): An event handler.
-
-        Returns:
-            (bool): ``True`` if handler is subscribed, ``False`` otherwise.
+            accessors (tuple[(Self, (**P) -> void) -> void, (Self, (**P) -> void) -> void]): A tuple of add and remove accessors.
         """
 
-        return obj in self.__handlers
-
-    def __iter__(self) -> Iterator[EventHandler[P]]:
-        """
-        Returns an iterator from the list of subscribed handlers.
+    def __init__(
+            self,
+            x: Callable[[], tuple[Callable[[Any, EventHandler[P]], void], Callable[[Any, EventHandler[P]], void]]]
+            | tuple[Callable[[Any, EventHandler[P]], void], Callable[[Any, EventHandler[P]], void]],
+            /
+    ) -> None:
+        (self.__add, self.__remove) = x() if callable(x) else x
 
-        Yields:
-            ((**P) -> void): A subscribed event handler.
-        """
+    def __get__(self, instance: object, cls: type, /) -> Self:
+        return self
 
-        return iter(self.__handlers)
+    def __set__(self, instance: object, value: add[P] | remove[P], /) -> None:
+        (handler, add) = value
+        if add:
+            self.__add(instance, handler)
+        else:
+            self.__remove(instance, handler)
 
-    def __len__(self) -> int:
+    def __iadd__(self, handler: EventHandler[P], /) -> add[P]:
         """
-        Returns the number of subscribed handlers.
+        Subscribes the handler to this event.
 
-        Returns:
-            (int): The number of subscribed event handlers.
+        Args:
+            handler ((**P) -> void): An event handler.
         """
 
-        return len(self.__handlers)
+        return (handler, True)
 
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> None:
+    def __isub__(self, handler: EventHandler[P], /) -> remove[P]:
         """
-        Raises this event.
+        Unsubscribes the handler from this event.
 
-        Handlers will be invoked in the order they subscribed.
+        Args:
+            handler ((**P) -> void): An event handler.
         """
 
-        for handler in [*self.__handlers]:  # apparently faster than list.copy(), list[:] or (*list, )
-            handler(*args, **kwargs)
+        return (handler, False)
 
 
-@final
-class event(Generic[P]):
+class async_event(event[P]):
     """
-    A decorator used to declare an event property in a publisher class.
+    A decorator used to declare an asynchronous event property in a publisher
+    class.
 
-    The definition function must return a tuple of accessors ``(add, remove)``
-    each of type ``(Self, (**P) -> void) -> void``.
+    The definition function must return a tuple of accessors `(add, remove)`
+    each of type `(Self, async (**P) -> void) -> void`.
 
     The subscribe and unsubscribe operators::
 
         obj.event += handler
         obj.event -= handler
 
-    will invoke the respective ``add`` and ``remove`` accessors with the arguments
-    ``(obj, handler)``.
+    will invoke the respective `add` and `remove` accessors with the arguments
+    `(obj, handler)`.
 
-    An event property is not bound to an instance object, thus it must be accessed as
-    an attribute of an object in order for the accessors to be invoked.
-    The following code::
+    An event property is not bound to an instance object, thus it must be
+    accessed as an attribute of an object in order for the accessors to be
+    invoked. The following code::
 
         e = obj.event
-        e += handler  # no effect on obj.event
+        e += handler  # no reference to obj!
 
-    has no effect on ``obj.event`` and will not call the ``add`` accessor,
-    since the argument ``self`` is not supplied.
+    has no effect on `obj.event` and will not call the `add` accessor,
+    since the argument `self` is not supplied.
 
     Unlike event fields, an event property cannot be invoked directly.
-    Use the underlying event that the accessors point to instead.
+    Use the underlying event object that the accessors point to instead.
 
     Example::
 
         class Example:
-            # Infer event type from the accessor parameter type
-            @event
+            # Infer event handler type from the accessor parameter type
+            @async_event
             def item_added():
-                def add(self: Self, value: EventHandler[int, object]) -> None:
-                    ...
-                def remove(self: Self, value: EventHandler[int, object]) -> None:
-                    ...
-                return (add, remove)
-
-            # Infer event type from the accessors type
-            @event
-            def item_removed() -> accessors[int, object]:
-                def add(self: Self, value) -> None:
-                    ...
-                def remove(self: Self, value) -> None:
-                    ...
-                return (add, remove)
-
-            # Explicit event type
-            @event[int, object]
-            def item_changed():
-                def add(self: Self, value) -> None:
+                def add(self: Self, value: AsyncEventHandler[int, object]) -> None:
                     ...
-                def remove(self: Self, value) -> None:
+                def remove(self: Self, value: AsyncEventHandler[int, object]) -> None:
                     ...
                 return (add, remove)
 
     Type Args:
-     - **P (ParamSpec): Event data parameter specification.
+        **P: Asynchronous event handler parameter specification.
     """
 
-    __slots__ = ("__add", "__remove")
+    __slots__ = []
 
     @overload
-    def __init__(self, definition: Callable[[], accessors[P]], /) -> None: ...
+    def __init__(self, definition: Callable[[], tuple[Callable[[Any, AsyncEventHandler[P]], void], Callable[[Any, AsyncEventHandler[P]], void]]], /) -> None:
+        """
+        Initializes a new instance of the `async_event` class.
 
-    @overload
-    def __init__(self, accessors: accessors[P], /) -> None: ...
+        Args:
+            definition (() -> tuple[(Self, async (**P) -> void) -> void, (Self, async (**P) -> void) -> void]):
+            An event definition returning a tuple of add and remove accessors.
+        """
 
-    def __init__(self, x: Callable[[], accessors[P]] | accessors[P], /) -> None:
+    @overload
+    def __init__(self, accessors: tuple[Callable[[Any, AsyncEventHandler[P]], void], Callable[[Any, AsyncEventHandler[P]], void]], /) -> None:
         """
-        Initializes a new instance of the ``event`` class.
+        Initializes a new instance of the `async_event` class.
 
         Args:
-         - definition (() -> accessors[P]): An event definition returning a tuple of add and remove accessors.
-         - accessors (accessors[P]): A tuple of add and remove accessors.
+            accessors (tuple[(Self, async (**P) -> void) -> void, (Self, async (**P) -> void) -> void]):
+            A tuple of add and remove accessors.
         """
-        (self.__add, self.__remove) = x() if callable(x) else x
 
+    def __init__(self, x, /) -> None:
+        super().__init__(x)
+
+    # __get__ definition is required for async_event to be recognized as a property
+    # although the base class already has both __get__ and __set__ definitions
+    @override
     def __get__(self, instance: object, cls: type, /) -> Self:
         return self
 
-    def __set__(self, instance: object, value: tuple[EventHandler[P], bool], /) -> None:
-        (handler, add) = value
-        if add:
-            self.__add(instance, handler)
-        else:
-            self.__remove(instance, handler)
+    @override
+    def __iadd__(self, handler: AsyncEventHandler[P]) -> add[P]:
+        """
+        Subscribes the handler to this event.
+
+        Args:
+            handler (async (**P) -> void): An asynchronous event handler.
+        """
+
+        return (handler, True)
 
-    def __iadd__(self, value: EventHandler[P], /) -> tuple[EventHandler[P], bool]:
-        return (value, True)
+    @override
+    def __isub__(self, handler: AsyncEventHandler[P]) -> remove[P]:
+        """
+        Unsubscribes the handler from this event.
+
+        Args:
+            handler (async (**P) -> void): An asynchronous event handler.
+        """
 
-    def __isub__(self, value: EventHandler[P], /) -> tuple[EventHandler[P], bool]:
-        return (value, False)
+        return (handler, False)
```

### Comparing `cs_events-0.4.1/src/events/_events.py` & `cs_events-0.5.0/src/events/_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import functools
 from collections.abc import Callable
-from typing import TypeVar, get_origin, get_type_hints, overload
+from typing import Any, TypeVar, get_origin, get_type_hints, overload
 
 from ._collections import EventHandlerCollection
-from ._event import Event, accessors, event
+from ._common import Delegate
+from ._field import AsyncEvent, Event
+from ._property import async_event, event
 
 
 __all__ = [
     "event_key",
     "events",
 ]
 
@@ -21,76 +23,85 @@
 
 @overload
 def events(*, collection: str | None = ...) -> Callable[[T], T]: ...
 
 
 def events(cls: T | None = None, /, *, collection: str | None = None) -> T | Callable[[T], T]:
     """
-    Adds event fields and/or properties based on the annotations defined in the class.
+    Adds event fields and/or properties based on the annotations defined in the
+    class.
 
-    ### Event Fields
+    ## Event Fields
 
-    Field annotations of type ``Event`` are turned into field assignments in a generated ``__init__`` method.
-    The ``__init__`` method will execute the original ``__init__`` method before the assignments if defined,
-    or call ``super().__init__`` otherwise.
+    Field annotations of type `Event` are turned into field assignments in a
+    generated `__init__` method.
+
+    The `__init__` method will execute the original `__init__` method before
+    the assignments if defined, or call `super().__init__` otherwise.
 
     Example::
 
         @events
         class EventFieldsExample:
             added: Event[object]
             removed: Event[object]
 
     is equivalent to::
 
         class EventFieldsExample:
+            added: Event[object]
+            removed: Event[object]
+
             def __init__(self, *args, **kwargs) -> None:
-                super().__init__(*args, **kwargs)
-                self.added: Event[object] = Event()
-                self.removed: Event[object] = Event()
-
-    ### Event Properties
-
-    Field annotations of type ``event`` are turned into event property definitions.
-    The add and remove accessors will simply call ``add_handler`` and ``remove_handler`` on the
-    specified collection, with the attribute name as the key by default.
-    The collection can be specified either by passing the attribute name of an ``EventHandlerCollection`` object
-    as the ``collection`` argument, or by a field annotation of a subtype of ``EventHandlerCollection``.
+                super().__init__(*args, **kwargs)  # or calls the original __init__(*args, **kwargs)
+                self.added = Event()
+                self.removed = Event()
+
+    ## Event Properties
+
+    Field annotations of type `event` are turned into event property
+    definitions. The add and remove accessors will simply call `add_handler()`
+    and `remove_handler()` on the specified collection, with the attribute name
+    as the key by default.
+
+    The collection can be specified either by passing the attribute name of an
+    `EventHandlerCollection` object as the `collection` argument, or by a field
+    annotation of a subtype of `EventHandlerCollection`.
 
     Example::
 
         @events(collection="__events")
         class EventPropertiesExample:
             closing: event[CancelEventArgs]
             closed: event[[]]
 
             def __init__(self) -> None:
                 self.__events = EventHandlerList()
 
-    is equivalent to::
+    is functionally equivalent to::
 
         class EventPropertiesExample:
+            def __init__(self) -> None:
+                self.__events = EventHandlerList()
+
             @event[CancelEventArgs]
             def closing():
-                def add(self, value):
+                def add(self, value, /):
                     self.__events.add_handler("closing", value)
-                def remove(self, value):
+                def remove(self, value, /):
                     self.__events.remove_handler("closing", value)
-                return add, remove
+                return (add, remove)
 
             @event[[]]
             def closed():
-                def add(self, value):
+                def add(self, value, /):
                     self.__events.add_handler("closed", value)
-                def remove(self, value):
+                def remove(self, value, /):
                     self.__events.remove_handler("closed", value)
-                return add, remove
-
-            def __init__(self) -> None:
-                self.__events = EventHandlerList()
+                return (add, remove)
 
     If your class defines a large number of events, the storage cost of one field per event might not be acceptable.
     For those situations, event properties can be used to store the events in another data structure.
 
     Event properties are slower than event fields due to the additional data structure.
     The trade-off is between memory and speed.
     If your class defines many events that are infrequently raised, you'll want to use event properties.
@@ -112,89 +123,96 @@
 def _events(cls: T, collection: str | None, /) -> T:
     if not isinstance(cls, type):
         raise TypeError("Argument 'cls' must be a class.")
 
     if collection and collection.startswith("__") and not collection.endswith("__"):
         collection = f"_{cls.__name__.lstrip('_')}{collection}"
 
-    fields: list[str] = [None]  # type: ignore
-    properties: list[str] = []
+    fields: list[tuple[str, str]] = []
+    properties: list[tuple[str, type[event], type[Delegate]]] = []
 
     for (attr, T) in get_type_hints(cls).items():
         T = get_origin(T) or T
         if T is Event:
-            fields.append(f"self.{attr} = Event()")
+            fields.append((attr, "Event"))
+        elif T is AsyncEvent:
+            fields.append((attr, "AsyncEvent"))
         elif T is event:
-            properties.append(attr)
+            properties.append((attr, event, Event))
+        elif T is async_event:
+            properties.append((attr, async_event, AsyncEvent))
         elif not collection and isinstance(T, type) and issubclass(T, EventHandlerCollection):
             collection = attr
 
-    if len(fields) > 1:
+    if fields:
         _fields(cls, fields)
 
     if properties:
         _properties(cls, properties, collection)
 
     return cls
 
 
-def _fields(cls: type, fields: list[str], /) -> None:
-    fields[0] = (
-        "def __init__(self, /, *args, **kwargs) -> None:"
-        "\n __orig_init__(self, *args, **kwargs)"
-    )
+def _fields(cls: type, fields: list[tuple[str, str]], /) -> None:
     globals = {
         "__builtins__": {},
         "__orig_init__": cls.__init__,
         "Event": Event,
+        "AsyncEvent": AsyncEvent,
     }
-    locals = {}
-    exec("\n ".join(fields), globals, locals)
+    locals: dict[str, Callable] = {}
+    exec(
+        "def __init__(self, /, *args, **kwargs) -> None:\n "
+        "__orig_init__(self, *args, **kwargs)\n " +
+        "\n ".join(
+            f"self.{attr} = {event_type}()" for (attr, event_type) in fields
+        ),
+        globals,
+        locals
+    )
 
-    f: Callable[..., None] = locals["__init__"]
+    __init__ = locals["__init__"]
 
     if "__init__" in cls.__dict__:
-        functools.update_wrapper(f, cls.__init__)
+        functools.update_wrapper(__init__, cls.__init__)
     else:
-        f.__module__ = cls.__module__
-        f.__qualname__ = f"{cls.__qualname__}.__init__"
+        __init__.__module__ = cls.__module__
+        __init__.__qualname__ = f"{cls.__qualname__}.__init__"
 
-    cls.__init__ = f
+    cls.__init__ = __init__
 
 
-def _properties(cls: type, properties: list[str], collection: str | None, /) -> None:
+def _properties(cls: type, properties: list[tuple[str, type[event], type[Delegate]]], collection: str | None, /) -> None:
     if not collection:
         raise ValueError(
             "Could not find an annotation of type "
             f"'{EventHandlerCollection.__qualname__}' in class '{cls.__qualname__}'."
         )
 
     # Assume collection is a valid variable name
-    locals = {}
+    locals: dict[str, Callable] = {}
     exec(
-        "def f(key, /):\n"
-        " def add(self, value, /):\n"
-        f"  self.{collection}.add_handler(key, value)\n"
-
-        " def remove(self, value, /):\n"
+        f"def f(key, event_type, /):\n"
+        f" def add(self, value, /):\n"
+        f"  self.{collection}.add_handler(key, value, event_type)\n"
+        f" def remove(self, value, /):\n"
         f"  self.{collection}.remove_handler(key, value)\n"
-
-        " return (add, remove)",
+        f" return (add, remove)",
         {"__builtins__": {}},
         locals
     )
-    f: Callable[[object], accessors[...]] = locals["f"]
+    f = locals["f"]
 
-    for name in properties:
-        setattr(cls, name, event(f(getattr(cls, name, name))))
+    for (name, property_type, event_type) in properties:
+        setattr(cls, name, property_type(f(getattr(cls, name, name), event_type)))
 
 
-def event_key(key: object, /) -> event[...]:
+def event_key(key: object, /) -> Any:
     """
-    Sets the key to use for event properties created with ``@events``.
+    Sets the key to use for event properties created with `@events`.
 
     Typically, empty objects are used as keys instead of allocating strings.
 
     Example::
 
         @events(collection="_events")
         class EventKeyExample:
@@ -204,14 +222,14 @@
             added: event[str] = event_key(__event_added)
             removed: event[str] = event_key(__event_removed)
 
             def __init__(self) -> None:
                 self._events = EventHandlerList()
 
     Args:
-     - key (object): A key for the event handler collection to use.
+        key (object): A key for the event handler collection to use.
 
     Returns:
-        (event[...]): A hint for the ``@events`` decorator to use the specified key instead.
+        Any: A hint for the `@events` decorator to use the specified key instead.
     """
 
-    return key  # type: ignore
+    return key
```

### Comparing `cs_events-0.4.1/PKG-INFO` & `cs_events-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-events
-Version: 0.4.1
+Version: 0.5.0
 Summary: C#-style event handling mechanism for Python
 Home-page: https://github.com/wise0704/python-cs-events
 License: MIT
 Keywords: python,event,c#
 Author: Daniel Jeong
 Author-email: wise0704@outlook.com
 Requires-Python: >=3.10,<4.0
@@ -12,20 +12,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Dist: typing-extensions (>=4.0.1,<5.0.0) ; python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.0.1,<5.0.0) ; python_version < "3.12"
 Project-URL: Issues, https://github.com/wise0704/python-cs-events/issues
 Project-URL: Repository, https://github.com/wise0704/python-cs-events
 Description-Content-Type: text/markdown
 
 # C#-Style Event Handling Mechanism for Python
 
 <p align="center">
@@ -65,72 +63,72 @@
 
 Python does not support an addition of two `Callable` types.
 So the `Event[**TArgs]` class is provided to mimic delegates:
 
 ```python
 from events import Event
 
-changed = Event[str, object]()
+item_changed = Event[str, object]()
 ```
 
 > C# naming convention prefers present/past participles (`changing`/`changed`) instead of `on`+infinitive (`on_change`) for events.
 
 Handlers can subscribe to and unsubscribe from the event with the same syntax:
 
 ```python
-def changed_handler(key: str, value: object) -> None:
+def item_changed_handler(key: str, value: object) -> None:
     ...
 
-changed += changed_handler
-changed -= changed_handler
+item_changed += item_changed_handler
+item_changed -= item_changed_handler
 ```
 
 An event can be raised by simply invoking it with the arguments:
 
 ```python
-changed("state", obj)
+item_changed("info", obj)
 ```
 
 Since `Event` acts just like a delegate from C#, it is not required to be bound to a class or an instance object.
 This is the major difference to other packages that try to implement the C#-style event system, which usually revolve around a container object for events.
 
 An example class with event fields may look like this:
 
 ```python
 class EventExample:
     def __init__(self) -> None:
+        self.__value = ""
         self.updated: Event[str] = Event()
-        self.__value: str = ""
 
     def update(self, value: str) -> None:
         if self.__value != value:
             self.__value = value
             self.updated(value)
 
 obj = EventExample()
 obj.updated += lambda value: print(f"obj.{value=}")
 obj.update("new value")
 ```
 
-A class decorator `@events` is provided as a shortcut for event fields:
+A class decorator `@events` is provided as a shortcut for **event fields**:
 
 ```python
 from events import Event, events
 
 @events
 class EventFieldsExample:
     item_added: Event[object]
     item_removed: Event[object]
-    item_updated: Event[object, str]
+    item_updated: Event[str, object]
 ```
 
-C# also provides event properties with `add` and `remove` accessors:
+C# also provides **event properties** with `add` and `remove` accessors:
 
 ```C#
-public event EventHandler<T> Changed
+public event EventHandler<ItemChangedEventArgs> ItemChanged
 {
     add { ... }
     remove { ... }
 }
 ```
 
 This feature is useful for classes that do not actually own the events, but need to forward the subscriptions to the underlying object that do own the events.
@@ -138,62 +136,60 @@
 The `@event[**TArgs]` decorator and the `accessors[**TArgs]` type are provided to support this feature:
 
 ```python
 from events import accessors, event, EventHandler
 
 class EventPropertyExample:
     @event[str, object]
-    def changed() -> accessors[str, object]:
-        def add(self: Self, value: EventHandler[str, object]) -> None:
-            ...
-        def remove(self: Self, value: EventHandler[str, object]) -> None:
-            ...
+    def item_changed() -> accessors[str, object]:
+        def add(self: Self, value: EventHandler[str, object]) -> None: ...
+        def remove(self: Self, value: EventHandler[str, object]) -> None: ...
         return (add, remove)
 ```
 
 Furthermore, the `EventHandlerCollection` interface is provided to support the functionalities of `System.ComponentModel.EventHandlerList` class from C#, along with the two implementations `EventHandlerList` and `EventHandlerDict` using a linked list and a dictionary respectively. The behaviour of `EventHandlerList` is exactly the same as of its counterpart from C#.
 
 A typical usage of `EventHandlerList` in C# can be translated directly into the python code:
 
 ```python
 class EventPropertyExample:
-    __event_changed: Final = object()
+    __event_item_changed: Final = object()
+
+    def __init__(self) -> None:
+        self.__events = EventHandlerList()
 
     @event  # [str, object] is inferred
-    def changed():  # -> accessors[str, object] is inferred
+    def item_changed():  # -> accessors[str, object] is inferred
         def add(self: Self, value: EventHandler[str, object]) -> None:
-            self.__events.add_handler(self.__event_changed, value)
+            self.__events.add_handler(self.__event_item_changed, value)
 
         def remove(self: Self, value: EventHandler[str, object]) -> None:
-            self.__events.remove_handler(self.__event_changed, value)
+            self.__events.remove_handler(self.__event_item_changed, value)
 
         return (add, remove)
-    
-    def __init__(self) -> None:
-        self.__events = EventHandlerList()
-    
-    def perform_change(self, key: str, value: object) -> None:
-        handler = self.__events[self.__event_changed]
+
+    def _on_item_changed(self, key: str, value: object) -> None:
+        handler = self.__events[self.__event_item_changed]
         if handler:
             handler(key, value)
 ```
 
 The class decorator `@events` also provides a shortcut for event properties.
 The above code can be shortened to:
 
 ```python
 @events(collection="__events")
 class EventPropertyExample:
-    changed: event[str, object]
+    item_changed: event[str, object]
 
     def __init__(self) -> None:
         self.__events = EventHandlerList()
 
-    def perform_change(self, key: str, value: object) -> None:
-        self.__events.invoke("changed", key, value)
+    def _on_item_changed(self, key: str, value: object) -> None:
+        self.__events.invoke("item_changed", key, value)
 ```
 
 ## Installation
 
 Install using [`pip`](https://pypi.org/project/pip/):
 
 ```console
```


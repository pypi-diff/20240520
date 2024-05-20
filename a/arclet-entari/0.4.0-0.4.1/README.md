# Comparing `tmp/arclet_entari-0.4.0.tar.gz` & `tmp/arclet_entari-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_entari-0.4.0.tar", last modified: Fri May  3 15:14:27 2024, max compression
+gzip compressed data, was "arclet_entari-0.4.1.tar", last modified: Mon May 20 09:40:42 2024, max compression
```

## Comparing `arclet_entari-0.4.0.tar` & `arclet_entari-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/LICENSE
--rw-r--r--   0        0        0      872 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/README.md
--rw-r--r--   0        0        0     2147 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/__init__.py
--rw-r--r--   0        0        0      228 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/__init__.py
--rw-r--r--   0        0        0      480 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/argv.py
--rw-r--r--   0        0        0     8556 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/main.py
--rw-r--r--   0        0        0     1142 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/model.py
--rw-r--r--   0        0        0      914 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/plugin.py
--rw-r--r--   0        0        0     5590 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/provider.py
--rw-r--r--   0        0        0     3532 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/core.py
--rw-r--r--   0        0        0    10616 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/event.py
--rw-r--r--   0        0        0      950 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/filter.py
--rw-r--r--   0        0        0     9684 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/message.py
--rw-r--r--   0        0        0     4772 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/plugin.py
--rw-r--r--   0        0        0    13585 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/session.py
--rw-r--r--   0        0        0     1821 2024-05-03 15:14:27.598539 arclet_entari-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 arclet_entari-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1111 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/README.md
+-rw-r--r--   0        0        0     2185 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/command/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/command/argv.py
+-rw-r--r--   0        0        0     8556 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/command/main.py
+-rw-r--r--   0        0        0     1191 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/command/model.py
+-rw-r--r--   0        0        0      914 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/command/plugin.py
+-rw-r--r--   0        0        0     5590 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/command/provider.py
+-rw-r--r--   0        0        0     4308 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/core.py
+-rw-r--r--   0        0        0    10616 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/event.py
+-rw-r--r--   0        0        0      950 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/filter.py
+-rw-r--r--   0        0        0     9777 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/message.py
+-rw-r--r--   0        0        0     4772 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/plugin.py
+-rw-r--r--   0        0        0    13671 2024-05-20 09:40:19.327387 arclet_entari-0.4.1/arclet/entari/session.py
+-rw-r--r--   0        0        0     1835 2024-05-20 09:40:42.775471 arclet_entari-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 arclet_entari-0.4.1/PKG-INFO
```

### Comparing `arclet_entari-0.4.0/LICENSE` & `arclet_entari-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.4.0/arclet/entari/__init__.py` & `arclet_entari-0.4.1/arclet/entari/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,7 +46,10 @@
 from .filter import is_direct_message as is_direct_message
 from .filter import is_public_message as is_public_message
 from .message import MessageChain as MessageChain
 from .plugin import Plugin as Plugin
 from .plugin import load_plugin as load_plugin
 from .plugin import load_plugins as load_plugins
 from .session import ContextSession as ContextSession
+
+WS = WebsocketsInfo
+WH = WebhookInfo
```

### Comparing `arclet_entari-0.4.0/arclet/entari/command/main.py` & `arclet_entari-0.4.1/arclet/entari/command/main.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.4.0/arclet/entari/command/model.py` & `arclet_entari-0.4.1/arclet/entari/command/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,31 @@
 
 
 @dataclass
 class Match(Generic[T]):
     """
     匹配项，表示参数是否存在于 `all_matched_args` 内
 
-    result (T): 匹配结果
-
-    available (bool): 匹配状态
+    Attributes:
+        result (T): 匹配结果
+        available (bool): 匹配状态
     """
 
     result: T
     available: bool
 
 
 class Query(Generic[T]):
     """
     查询项，表示参数是否可由 `Arparma.query` 查询并获得结果
 
-    result (T): 查询结果
-
-    available (bool): 查询状态
-
-    path (str): 查询路径
+    Attributes:
+        result (T): 查询结果
+        available (bool): 查询状态
+        path (str): 查询路径
     """
 
     result: T
     available: bool
     path: str
 
     def __init__(self, path: str, default: Union[T, type[Empty]] = Empty):
```

### Comparing `arclet_entari-0.4.0/arclet/entari/command/plugin.py` & `arclet_entari-0.4.1/arclet/entari/command/plugin.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.4.0/arclet/entari/command/provider.py` & `arclet_entari-0.4.1/arclet/entari/command/provider.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.4.0/arclet/entari/core.py` & `arclet_entari-0.4.1/arclet/entari/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import asyncio
 from contextlib import suppress
 
-from arclet.letoderea import Contexts, EventSystem, Provider, global_providers
+from arclet.letoderea import BaseAuxiliary, Contexts, EventSystem, Provider, ProviderFactory, global_providers
 from loguru import logger
 from satori.client import App
 from satori.client.account import Account
 from satori.client.session import Session
 from satori.config import Config
 from satori.model import Event
 
-from .event import event_parse
+from .event import MessageEvent, event_parse
 from .plugin import dispatchers
 from .session import ContextSession
 
 
 class SessionProvider(Provider[Session]):
     async def __call__(self, context: Contexts):
         if account := context.get("$account"):
@@ -37,14 +37,33 @@
     def __init__(self, *configs: Config):
         super().__init__(*configs)
         self.event_system = EventSystem()
         self.register(self.handle_event)
         self._ref_tasks = set()
         # self.lifecycle(self.handle_lifecycle)
 
+    def on(
+        self,
+        *events: type,
+        priority: int = 16,
+        auxiliaries: list[BaseAuxiliary] | None = None,
+        providers: list[Provider | type[Provider] | ProviderFactory | type[ProviderFactory]] | None = None,
+    ):
+        return self.event_system.on(*events, priority=priority, auxiliaries=auxiliaries, providers=providers)
+
+    def on_message(
+        self,
+        priority: int = 16,
+        auxiliaries: list[BaseAuxiliary] | None = None,
+        providers: list[Provider | type[Provider] | ProviderFactory | type[ProviderFactory]] | None = None,
+    ):
+        return self.event_system.on(
+            MessageEvent, priority=priority, auxiliaries=auxiliaries, providers=providers
+        )
+
     async def handle_event(self, account: Account, event: Event):
         async def event_parse_task(connection: Account, raw: Event):
             loop = asyncio.get_running_loop()
             with suppress(NotImplementedError):
                 ev = event_parse(connection, raw)
                 self.event_system.publish(ev)
                 for disp in dispatchers.values():
```

### Comparing `arclet_entari-0.4.0/arclet/entari/event.py` & `arclet_entari-0.4.1/arclet/entari/event.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.4.0/arclet/entari/filter.py` & `arclet_entari-0.4.1/arclet/entari/filter.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.4.0/arclet/entari/message.py` & `arclet_entari-0.4.1/arclet/entari/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,87 +100,87 @@
     @overload
     def __getitem__(self, args: type[TE1]) -> MessageChain[TE1]:
         """获取仅包含指定消息段类型的消息
 
         Args:
             args: 消息段类型
 
-        Return:
+        Returns:
             所有类型为 `args` 的消息段
         """
 
     @overload
     def __getitem__(self, args: tuple[type[TE1], int]) -> TE1:
         """索引指定类型的消息段
 
         Args:
             args: 消息段类型和索引
 
-        Return:
+        Returns:
             类型为 `args[0]` 的消息段第 `args[1]` 个
         """
 
     @overload
     def __getitem__(self, args: tuple[type[TE1], slice]) -> MessageChain[TE1]:
         """切片指定类型的消息段
 
         Args:
             args: 消息段类型和切片
 
-        Return:
+        Returns:
             类型为 `args[0]` 的消息段切片 `args[1]`
         """
 
     @overload
     def __getitem__(self, args: int) -> TE:
         """索引消息段
 
         Args:
             args: 索引
 
-        Return:
+        Returns:
             第 `args` 个消息段
         """
 
     @overload
     def __getitem__(self, args: slice) -> Self:
         """切片消息段
 
         Args:
             args: 切片
 
-        Return:
+        Returns:
             消息切片 `args`
         """
 
     def __getitem__(
         self,
         args: type[TE1] | tuple[type[TE1], int] | tuple[type[TE1], slice] | int | slice,
     ) -> TE | TE1 | MessageChain[TE1] | Self:
         arg1, arg2 = args if isinstance(args, tuple) else (args, None)
         if isinstance(arg1, int) and arg2 is None:
             return super().__getitem__(arg1)
         if isinstance(arg1, slice) and arg2 is None:
-            return MessageChain(super().__getitem__(arg1))
+            return MessageChain(super().__getitem__(arg1))  # type: ignore
         if TYPE_CHECKING:
             assert not isinstance(arg1, (slice, int))
         if issubclass(arg1, Element) and arg2 is None:
-            return MessageChain(seg for seg in self if isinstance(seg, arg1))
+            return MessageChain(seg for seg in self if isinstance(seg, arg1))  # type: ignore
         if issubclass(arg1, Element) and isinstance(arg2, int):
             return [seg for seg in self if isinstance(seg, arg1)][arg2]
         if issubclass(arg1, Element) and isinstance(arg2, slice):
-            return MessageChain([seg for seg in self if isinstance(seg, arg1)][arg2])
+            return MessageChain([seg for seg in self if isinstance(seg, arg1)][arg2])  # type: ignore
         raise ValueError("Incorrect arguments to slice")  # pragma: no cover
 
     def __contains__(self, value: str | Element | type[Element]) -> bool:
         """检查消息段是否存在
 
         Args:
             value: 消息段或消息段类型
-        Return:
+        Returns:
             消息内是否存在给定消息段或给定类型的消息段
         """
         if isinstance(value, type):
             return bool(next((seg for seg in self if isinstance(seg, value)), None))
         if isinstance(value, str):
             value = Text(value)
         return super().__contains__(value)
@@ -191,15 +191,15 @@
     def index(self, value: str | Element | type[Element], *args: SupportsIndex) -> int:
         """索引消息段
 
         Args:
             value: 消息段或者消息段类型
             args: start 与 end
 
-        Return:
+        Returns:
             索引 index
 
         Raise:
             ValueError: 消息段不存在
         """
         if isinstance(value, type):
             first_segment = next((seg for seg in self if isinstance(seg, value)), None)
@@ -213,35 +213,35 @@
     def get(self, type_: type[TE], count: int | None = None) -> MessageChain[TE]:
         """获取指定类型的消息段
 
         Args:
             type_: 消息段类型
             count: 获取个数
 
-        Return:
+        Returns:
             构建的新消息
         """
         if count is None:
             return self[type_]
 
         iterator, filtered = (seg for seg in self if isinstance(seg, type_)), MessageChain()
         for _ in range(count):
             seg = next(iterator, None)
             if seg is None:
                 break
             filtered.append(seg)
-        return filtered
+        return filtered  # type: ignore
 
     def count(self, value: type[Element] | str | Element) -> int:
         """计算指定消息段的个数
 
         Args:
             value: 消息段或消息段类型
 
-        Return:
+        Returns:
             个数
         """
         if isinstance(value, str):
             value = Text(value)
         return (
             len(self[value])  # type: ignore
             if isinstance(value, type)
@@ -250,64 +250,64 @@
 
     def only(self, value: type[Element] | str | Element) -> bool:
         """检查消息中是否仅包含指定消息段
 
         Args:
             value: 指定消息段或消息段类型
 
-        Return:
+        Returns:
             是否仅包含指定消息段
         """
         if isinstance(value, type):
             return all(isinstance(seg, value) for seg in self)
         if isinstance(value, str):
             value = Text(value)
         return all(seg == value for seg in self)
 
     def join(self, iterable: Iterable[TE1 | MessageChain[TE1]]) -> MessageChain[TE | TE1]:
         """将多个消息连接并将自身作为分割
 
         Args:
             iterable: 要连接的消息
 
-        Return:
+        Returns:
             连接后的消息
         """
         ret = MessageChain()
         for index, msg in enumerate(iterable):
             if index != 0:
                 ret.extend(self)
             if isinstance(msg, Element):
                 ret.append(msg)
             else:
                 ret.extend(msg.copy())
-        return ret
+        return ret  # type: ignore
 
     def copy(self) -> MessageChain[TE]:
         """深拷贝消息"""
         return deepcopy(self)
 
     def include(self, *types: type[Element]) -> MessageChain:
         """过滤消息
 
         Args:
             types: 包含的消息段类型
 
-        Return:
+        Returns:
             新构造的消息
         """
         return MessageChain(seg for seg in self if seg.__class__ in types)
 
     def exclude(self, *types: type[Element]) -> MessageChain:
         """过滤消息
 
         Args:
             types: 不包含的消息段类型
 
-        Return:
+        Returns:
             新构造的消息
         """
         return MessageChain(seg for seg in self if seg.__class__ not in types)
 
     def extract_plain_text(self) -> str:
         """提取消息内纯文本消息"""
```

### Comparing `arclet_entari-0.4.0/arclet/entari/plugin.py` & `arclet_entari-0.4.1/arclet/entari/plugin.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.4.0/arclet/entari/session.py` & `arclet_entari-0.4.1/arclet/entari/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,18 @@
         self,
         message: str | Iterable[str | Element],
         timeout: float = 120,
         timeout_message: str | Iterable[str | Element] = "等待超时",
     ) -> MessageChain:
         """发送提示消息, 并等待回复
 
-        参数:
+        Args:
             message: 要发送的消息
+            timeout: 等待超时时间
+            timeout_message: 超时后发送的消息
         """
         if self.context.type != EventType.MESSAGE_CREATED:
             raise RuntimeError("Event cannot be prompted!")
 
         await self.send(message)
 
         async def waiter(content: MessageChain, session: ContextSession):
@@ -100,41 +102,41 @@
 
     async def send_message(
         self,
         message: str | Iterable[str | Element],
     ) -> list[MessageObject]:
         """发送消息
 
-        参数:
+        Args:
             message: 要发送的消息
         """
         if not self.context.channel:
             raise RuntimeError("Event cannot be replied to!")
         return await self.account.session.send_message(self.context.channel, message)
 
     async def send_private_message(
         self,
         message: str | Iterable[str | Element],
     ) -> list[MessageObject]:
         """发送私聊消息
 
-        参数:
+        Args:
             message: 要发送的消息
         """
         if not self.context.user:
             raise RuntimeError("Event cannot be replied to!")
         return await self.account.session.send_private_message(self.context.user, message)
 
     async def update_message(
         self,
         message: str | Iterable[str | Element],
     ):
         """更新消息
 
-        参数:
+        Args:
             message: 要更新的消息
         """
         if not self.context.channel:
             raise RuntimeError("Event cannot be replied to!")
         if not self.context.message:
             raise RuntimeError("Event cannot update message")
         return await self.account.session.update_message(
```

### Comparing `arclet_entari-0.4.0/pyproject.toml` & `arclet_entari-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-entari"
-version = "0.4.0"
+version = "0.4.1"
 description = "Simple IM Framework based on satori-python"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "arclet-letoderea>=0.9.2",
     "arclet-alconna>=1.8.11",
@@ -95,13 +95,14 @@
     "Q",
 ]
 ignore = [
     "C901",
     "T201",
     "E731",
     "E402",
+    "PYI055",
 ]
 
 [tool.pyright]
 pythonVersion = "3.9"
 pythonPlatform = "All"
 typeCheckingMode = "basic"
```

### Comparing `arclet_entari-0.4.0/PKG-INFO` & `arclet_entari-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-entari
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple IM Framework based on satori-python
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -31,24 +31,37 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arclet-entari)](https://www.python.org/)
 ![Entari](https://img.shields.io/badge/Arclet-Entari-2564c2.svg)
 
 一个基于 `Satori` 协议的简易 IM framework
 
 ## 示例
 
+复读:
+
+```python
+from arclet.entari import ContextSession, Entari, WS
+
+app = Entari(WS(host="127.0.0.1", port=5140, path="satori"))
+
+
+@app.on_message()
+async def repeat(session: ContextSession):
+    await session.send(session.content)
+
+app.run()
+```
+
+指令 `add {a} {b}`: 
 ```python
-from arclet.entari import ContextSession, Entari, EntariCommands, WebsocketsInfo
+from arclet.entari import ContextSession, Entari, EntariCommands, WS
 
 command = EntariCommands()
 
 
 @command.on("add {a} {b}")
 async def add(a: int, b: int, session: ContextSession):
-    await session.send(f"{a + b =}")
+    await session.send(f"{a + b = }")
 
 
-app = Entari()
-app.apply(WebsocketsInfo(port=5500, token="XXX"))
-
+app = Entari(WS(port=5500, token="XXX"))
 app.run()
-
 ```
```


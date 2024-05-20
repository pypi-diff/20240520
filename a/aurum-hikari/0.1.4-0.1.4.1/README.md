# Comparing `tmp/aurum_hikari-0.1.4.tar.gz` & `tmp/aurum_hikari-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurum_hikari-0.1.4.tar", max compression
+gzip compressed data, was "aurum_hikari-0.1.4.1.tar", max compression
```

## Comparing `aurum_hikari-0.1.4.tar` & `aurum_hikari-0.1.4.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     1080 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/LICENSE
--rw-r--r--   0        0        0     3082 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/README.md
--rw-r--r--   0        0        0      479 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/__init__.py
--rw-r--r--   0        0        0      382 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/_about.py
--rw-r--r--   0        0        0     5346 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/client.py
--rw-r--r--   0        0        0      316 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/__init__.py
--rw-r--r--   0        0        0      198 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/decorators/__init__.py
--rw-r--r--   0        0        0     1099 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/decorators/sub_command.py
--rw-r--r--   0        0        0     2321 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/message_command.py
--rw-r--r--   0        0        0     9023 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/slash_command.py
--rw-r--r--   0        0        0     1671 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/sub_command.py
--rw-r--r--   0        0        0     2402 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/commands/user_command.py
--rw-r--r--   0        0        0        0 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/enum/__init__.py
--rw-r--r--   0        0        0      423 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/enum/sync_commands.py
--rw-r--r--   0        0        0        0 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/ext/__init__.py
--rw-r--r--   0        0        0      241 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/ext/plugins/__init__.py
--rw-r--r--   0        0        0     4227 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/ext/plugins/plugin.py
--rw-r--r--   0        0        0     3333 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/ext/plugins/plugin_manager.py
--rw-r--r--   0        0        0      292 2024-05-18 23:01:06.001518 aurum_hikari-0.1.4/aurum/includable.py
--rw-r--r--   0        0        0      220 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/interactions/__init__.py
--rw-r--r--   0        0        0     7214 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/interactions/interaction_context.py
--rw-r--r--   0        0        0        0 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/commands/__init__.py
--rw-r--r--   0        0        0     3035 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/commands/app_command.py
--rw-r--r--   0        0        0     4014 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/commands/command_handler.py
--rw-r--r--   0        0        0     1937 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/commands/context_menu_command.py
--rw-r--r--   0        0        0       75 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/consts.py
--rw-r--r--   0        0        0      290 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/exceptions/__init__.py
--rw-r--r--   0        0        0       67 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/exceptions/base_exception.py
--rw-r--r--   0        0        0      456 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/exceptions/commands_exceptions.py
--rw-r--r--   0        0        0     6407 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/internal/interaction_processor.py
--rw-r--r--   0        0        0      401 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/__init__.py
--rw-r--r--   0        0        0      147 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/locale.py
--rw-r--r--   0        0        0     1223 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/localization_provider_interface.py
--rw-r--r--   0        0        0      255 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/localized.py
--rw-r--r--   0        0        0      529 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/pass_localization_provider.py
--rw-r--r--   0        0        0      207 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/l10n/types.py
--rw-r--r--   0        0        0      219 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/options/__init__.py
--rw-r--r--   0        0        0      299 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/options/choice.py
--rw-r--r--   0        0        0     1715 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/options/option.py
--rw-r--r--   0        0        0        0 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/py.typed
--rw-r--r--   0        0        0      147 2024-05-18 23:01:06.005518 aurum_hikari-0.1.4/aurum/types.py
--rw-r--r--   0        0        0     1987 2024-05-18 23:01:19.581538 aurum_hikari-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 aurum_hikari-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/LICENSE
+-rw-r--r--   0        0        0     3473 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/README.md
+-rw-r--r--   0        0        0      427 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/__init__.py
+-rw-r--r--   0        0        0      430 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/_about.py
+-rw-r--r--   0        0        0     5346 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/client.py
+-rw-r--r--   0        0        0      316 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/commands/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/commands/decorators/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/commands/decorators/sub_command.py
+-rw-r--r--   0        0        0     2324 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/commands/message_command.py
+-rw-r--r--   0        0        0     5747 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/commands/slash_command.py
+-rw-r--r--   0        0        0     2594 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/commands/sub_command.py
+-rw-r--r--   0        0        0     2402 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/commands/user_command.py
+-rw-r--r--   0        0        0        0 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/enum/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-20 17:26:58.028502 aurum_hikari-0.1.4.1/aurum/enum/sync_commands.py
+-rw-r--r--   0        0        0        0 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/ext/__init__.py
+-rw-r--r--   0        0        0      241 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/ext/plugins/__init__.py
+-rw-r--r--   0        0        0     4227 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/ext/plugins/plugin.py
+-rw-r--r--   0        0        0     3333 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/ext/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      292 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/includable.py
+-rw-r--r--   0        0        0      220 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/interactions/__init__.py
+-rw-r--r--   0        0        0     7214 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/interactions/interaction_context.py
+-rw-r--r--   0        0        0        0 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/commands/__init__.py
+-rw-r--r--   0        0        0     3035 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/commands/app_command.py
+-rw-r--r--   0        0        0     4014 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/commands/command_handler.py
+-rw-r--r--   0        0        0     1937 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/commands/context_menu_command.py
+-rw-r--r--   0        0        0       75 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/consts.py
+-rw-r--r--   0        0        0      290 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/exceptions/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/exceptions/base_exception.py
+-rw-r--r--   0        0        0      456 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/exceptions/commands_exceptions.py
+-rw-r--r--   0        0        0     6465 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/interaction_processor.py
+-rw-r--r--   0        0        0        0 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1148 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/internal/utils/commands.py
+-rw-r--r--   0        0        0      401 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/l10n/__init__.py
+-rw-r--r--   0        0        0      147 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/l10n/locale.py
+-rw-r--r--   0        0        0     1323 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/l10n/localization_provider_interface.py
+-rw-r--r--   0        0        0      255 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/l10n/localized.py
+-rw-r--r--   0        0        0      529 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/l10n/pass_localization_provider.py
+-rw-r--r--   0        0        0      207 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/l10n/types.py
+-rw-r--r--   0        0        0      219 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/options/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/options/choice.py
+-rw-r--r--   0        0        0     1715 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/options/option.py
+-rw-r--r--   0        0        0        0 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/py.typed
+-rw-r--r--   0        0        0      147 2024-05-20 17:26:58.032502 aurum_hikari-0.1.4.1/aurum/types.py
+-rw-r--r--   0        0        0     1989 2024-05-20 17:27:18.652697 aurum_hikari-0.1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 aurum_hikari-0.1.4.1/PKG-INFO
```

### Comparing `aurum_hikari-0.1.4/LICENSE` & `aurum_hikari-0.1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/README.md` & `aurum_hikari-0.1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-![banner](static/banner.png)
-
 <div align="center">
-    <h1>Aurum</h1>
-    <p>
-        <a href="https://github.com/hikari-py/hikari">
-            <img alt="Static Badge" src="https://img.shields.io/badge/Powered%20by-hikari-E440C1">
-        </a>
-        <a href="https://pypi.org/project/aurum-hikari/">
-            <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/aurum-hikari">
-            <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/aurum-hikari">
-            <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/aurum-hikari">
-        </a>
-        <a href="https://github.com/ShinshiDevs/aurum-hikari">
-            <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/w/ShinshiDevs/aurum-hikari">
-            <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-closed/ShinshiDevs/aurum-hikari">
-            <img alt="GitHub License" src="https://img.shields.io/github/license/ShinshiDevs/aurum-hikari">
-        </a>
-    </p>
-    <p>
-        <a href="https://shinshidevs.github.io/aurum-hikari/">Documentation</a>
-        ·
-        <a href="https://github.com/ShinshiDevs/aurum-hikari/releases">Releases</a>
-        ·
-        <a href="https://pypi.org/project/aurum-hikari/">PyPI</a>
-        ·
-        <a href="./LICENSE">License</a>
-    </p>
-    <p>
-        <text>A flexible command & component handler.</text>
-    </p>
-    <p>
-        <text>
-            The main purpose of this library is to help you create a bot and implement its functionality. It makes the process simpler and easier.
-        </text>
-        <text>
-            Our goal is to provide you, as developers, with complete freedom of action and to highlight the benefits of Hikari.
-        </text>
-    </p>
+    <div>
+        <div align=left>
+            <h1>
+                <img src="docs/assets/logo.svg" width=25> Aurum
+            </h1>
+            <p>
+                <a href="https://shinshidevs.github.io/aurum-hikari/">Documentation</a>
+                ·
+                <a href="https://github.com/ShinshiDevs/aurum-hikari/releases">Releases</a>
+                ·
+                <a href="https://pypi.org/project/aurum-hikari/">PyPI</a>
+                ·
+                <a href="./LICENSE">License</a>
+            </p>
+            <p>
+                <a href="https://github.com/hikari-py/hikari">
+                    <img alt="Static Badge" src="https://img.shields.io/badge/Powered%20by-hikari-E440C1">
+                </a>
+                <a href="https://pypi.org/project/aurum-hikari/">
+                    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/aurum-hikari">
+                    <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/aurum-hikari">
+                    <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/aurum-hikari">
+                </a>
+                <a href="https://github.com/ShinshiDevs/aurum-hikari">
+                    <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/w/ShinshiDevs/aurum-hikari">
+                    <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-closed/ShinshiDevs/aurum-hikari">
+                    <img alt="GitHub License" src="https://img.shields.io/github/license/ShinshiDevs/aurum-hikari">
+                </a>
+            </p>
+            <p>
+                <text>A flexible command & component handler.</text>
+            </p>
+            <p>
+                <text>
+                    The main purpose of this library is to help you create a bot and implement its functionality. It makes the process simpler and easier.
+                </text>
+                <text>
+                    Our goal is to provide you, as developers, with complete freedom of action and to highlight the benefits of Hikari.
+                </text>
+            </p>
+        </div>
+    </div>
 </div>
 
 # Installation
 > [!NOTE]
 > Aurum requires Python 3.10 or higher.
 
 Run command:
```

### Comparing `aurum_hikari-0.1.4/aurum/client.py` & `aurum_hikari-0.1.4.1/aurum/client.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/commands/decorators/sub_command.py` & `aurum_hikari-0.1.4.1/aurum/commands/decorators/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/commands/message_command.py` & `aurum_hikari-0.1.4.1/aurum/commands/message_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         is_dm_enabled (bool): Whether the command can be used in direct messages.
         is_nsfw (bool): Indicates whether the command is age-restricted.
 
     Example:
         ```py
         class ReverseTextCommand(MessageCommand):
             def __init__(self) -> None:
-                super().__init__(name="Reverse", dm_enabled=True)
+                super().__init__(name="Reverse", is_dm_enabled=True)
 
             async def callback(self, context: InteractionContext, message: Message) -> None:
                 await context.create_response(message.content[::-1])
         ```
     """
 
     def __init__(
```

### Comparing `aurum_hikari-0.1.4/aurum/commands/sub_command.py` & `aurum_hikari-0.1.4.1/aurum/commands/sub_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 import typing
 from dataclasses import dataclass, field
 
+from hikari.commands import CommandOption, OptionType
+
+from aurum.internal.utils.commands import build_option
 from aurum.options import Option
 
 if typing.TYPE_CHECKING:
     from collections.abc import Awaitable, Callable, Sequence
 
+    from aurum.l10n import LocalizationProviderInterface
     from aurum.l10n.types import LocalizedOr
 
 
 @dataclass(slots=True, kw_only=True)
 class SubCommand:
     callback: Callable[..., Awaitable[typing.Any]]
 
@@ -47,7 +51,22 @@
                 callback=func,
                 name=name,
                 description=description or "No description",
                 options=options,
             )
 
         return decorator
+
+    def as_option(self, l10n: LocalizationProviderInterface) -> CommandOption:
+        options: Sequence[CommandOption]
+        if not self.sub_commands:
+            options = [build_option(option, l10n) for option in self.options]
+        else:
+            options = [sub_command.as_option(l10n) for sub_command in self.sub_commands.values()]
+        return CommandOption(
+            type=OptionType.SUB_COMMAND if not self.sub_commands else OptionType.SUB_COMMAND_GROUP,
+            name=str(self.name),
+            name_localizations=l10n.build_localized(self.name),
+            description=str(self.description),
+            description_localizations=l10n.build_localized(self.description or "No description"),
+            options=options,
+        )
```

### Comparing `aurum_hikari-0.1.4/aurum/commands/user_command.py` & `aurum_hikari-0.1.4.1/aurum/commands/user_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/ext/plugins/plugin.py` & `aurum_hikari-0.1.4.1/aurum/ext/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/ext/plugins/plugin_manager.py` & `aurum_hikari-0.1.4.1/aurum/ext/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/interactions/interaction_context.py` & `aurum_hikari-0.1.4.1/aurum/interactions/interaction_context.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/internal/commands/app_command.py` & `aurum_hikari-0.1.4.1/aurum/internal/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/internal/commands/command_handler.py` & `aurum_hikari-0.1.4.1/aurum/internal/commands/command_handler.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/internal/commands/context_menu_command.py` & `aurum_hikari-0.1.4.1/aurum/internal/commands/context_menu_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/internal/interaction_processor.py` & `aurum_hikari-0.1.4.1/aurum/internal/interaction_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from aurum.commands.message_command import MessageCommand
 from aurum.commands.slash_command import SlashCommand
 from aurum.commands.user_command import UserCommand
 from aurum.interactions.interaction_context import InteractionContext
 from aurum.internal.exceptions.commands_exceptions import UnknownCommandException
 
 if typing.TYPE_CHECKING:
-    from collections.abc import Callable, Sequence
+    from collections.abc import Awaitable, Callable, Sequence
 
     from hikari.impl import GatewayBot
     from hikari.interactions import (
         CommandInteractionOption,
         ComponentInteraction,
         PartialInteraction,
     )
@@ -104,19 +104,18 @@
                         options = options[0].options
                         if not command:
                             raise UnknownCommandException(
                                 option.name, sub_command_group.name, interaction.command_name
                             )
                 for option in options or ():
                     arguments[option.name] = self.resolve_command_argument(interaction, option)
-            return await (
-                command.callback(context, **arguments)
-                if isinstance(command, SlashCommand)
-                else command.callback(parent_command, context, **arguments)
-            )
+            callback: Callable[..., Awaitable[typing.Any]] = getattr(command, "callback")
+            if isinstance(command, SlashCommand):
+                return await callback(context, **arguments)
+            return await callback(parent_command, context, **arguments)
         if interaction.command_type is CommandType.MESSAGE:
             assert isinstance(command, MessageCommand)
             assert interaction.resolved
             return await command.callback(
                 context,
                 list(interaction.resolved.messages.values())[0],
             )
```

### Comparing `aurum_hikari-0.1.4/aurum/l10n/localization_provider_interface.py` & `aurum_hikari-0.1.4.1/aurum/l10n/localization_provider_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import typing
 
 if typing.TYPE_CHECKING:
     from hikari import CommandInteraction, ComponentInteraction
 
     from aurum.l10n.locale import Locale
-    from aurum.l10n.localized import Localized
+    from aurum.l10n.types import LocalizedOr
 
 
 class LocalizationProviderInterface(typing.Protocol):
     """Localization provider interface.
 
     It's used to localize commands, components, and provide a locale for interaction.
 
@@ -18,23 +18,24 @@
     or create your own.
     To create your own implementation, you need to inherit from this interface.
     """
 
     async def start(self) -> None:
         """Start the localization provider.
 
-        Note:
+        Warning:
             Important function, must be implemented.
         """
         ...
 
-    def build_localized(self, value: Localized) -> typing.Dict[str, str]:
+    def build_localized(self, value: LocalizedOr[str]) -> typing.Dict[str, str]:
         """Build [Localized object][aurum.l10n.localized.Localized] for Discord API.
 
-        Note:
-            Important function, must be implemented.
+        Warning:
+            - Important function, must be implemented.
+            - When str is passed to value, this function must return empty dictionary.
         """
         ...
 
     def get_locale(self, by: str | CommandInteraction | ComponentInteraction) -> Locale | None:
         """Get locale by name or interaction"""
         ...
```

### Comparing `aurum_hikari-0.1.4/aurum/l10n/pass_localization_provider.py` & `aurum_hikari-0.1.4.1/aurum/l10n/pass_localization_provider.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/aurum/options/option.py` & `aurum_hikari-0.1.4.1/aurum/options/option.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.4/pyproject.toml` & `aurum_hikari-0.1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 
 # Package information
 [tool.poetry]
 packages = [{ include = "aurum" }]
 name = "aurum-hikari"
-version = "v0.1.4"
+version = "v0.1.4.1"
 license = "MIT"
 authors = ["stefanlight <64615032+stefanlight8@users.noreply.github.com>"]
 description = "A flexible command & component handler"
 keywords = [
     "discord",
     "hikari",
     "commands",
```

### Comparing `aurum_hikari-0.1.4/PKG-INFO` & `aurum_hikari-0.1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurum-hikari
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: A flexible command & component handler
 License: MIT
 Keywords: discord,hikari,commands,components,command-handler,component-handler
 Author: stefanlight
 Author-email: 64615032+stefanlight8@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
@@ -23,53 +23,57 @@
 Classifier: Typing :: Typed
 Requires-Dist: hikari (>2.0.0.dev122)
 Project-URL: Issue Tracker, https://github.com/ShinshiDevs/aurum-hikari/issues
 Project-URL: documentation, https://shinshidevs.github.io/aurum-hikari/
 Project-URL: repository, https://github.com/ShinshiDevs/aurum-hikari
 Description-Content-Type: text/markdown
 
-![banner](static/banner.png)
-
 <div align="center">
-    <h1>Aurum</h1>
-    <p>
-        <a href="https://github.com/hikari-py/hikari">
-            <img alt="Static Badge" src="https://img.shields.io/badge/Powered%20by-hikari-E440C1">
-        </a>
-        <a href="https://pypi.org/project/aurum-hikari/">
-            <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/aurum-hikari">
-            <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/aurum-hikari">
-            <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/aurum-hikari">
-        </a>
-        <a href="https://github.com/ShinshiDevs/aurum-hikari">
-            <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/w/ShinshiDevs/aurum-hikari">
-            <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-closed/ShinshiDevs/aurum-hikari">
-            <img alt="GitHub License" src="https://img.shields.io/github/license/ShinshiDevs/aurum-hikari">
-        </a>
-    </p>
-    <p>
-        <a href="https://shinshidevs.github.io/aurum-hikari/">Documentation</a>
-        ·
-        <a href="https://github.com/ShinshiDevs/aurum-hikari/releases">Releases</a>
-        ·
-        <a href="https://pypi.org/project/aurum-hikari/">PyPI</a>
-        ·
-        <a href="./LICENSE">License</a>
-    </p>
-    <p>
-        <text>A flexible command & component handler.</text>
-    </p>
-    <p>
-        <text>
-            The main purpose of this library is to help you create a bot and implement its functionality. It makes the process simpler and easier.
-        </text>
-        <text>
-            Our goal is to provide you, as developers, with complete freedom of action and to highlight the benefits of Hikari.
-        </text>
-    </p>
+    <div>
+        <div align=left>
+            <h1>
+                <img src="docs/assets/logo.svg" width=25> Aurum
+            </h1>
+            <p>
+                <a href="https://shinshidevs.github.io/aurum-hikari/">Documentation</a>
+                ·
+                <a href="https://github.com/ShinshiDevs/aurum-hikari/releases">Releases</a>
+                ·
+                <a href="https://pypi.org/project/aurum-hikari/">PyPI</a>
+                ·
+                <a href="./LICENSE">License</a>
+            </p>
+            <p>
+                <a href="https://github.com/hikari-py/hikari">
+                    <img alt="Static Badge" src="https://img.shields.io/badge/Powered%20by-hikari-E440C1">
+                </a>
+                <a href="https://pypi.org/project/aurum-hikari/">
+                    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/aurum-hikari">
+                    <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/aurum-hikari">
+                    <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/aurum-hikari">
+                </a>
+                <a href="https://github.com/ShinshiDevs/aurum-hikari">
+                    <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/w/ShinshiDevs/aurum-hikari">
+                    <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-closed/ShinshiDevs/aurum-hikari">
+                    <img alt="GitHub License" src="https://img.shields.io/github/license/ShinshiDevs/aurum-hikari">
+                </a>
+            </p>
+            <p>
+                <text>A flexible command & component handler.</text>
+            </p>
+            <p>
+                <text>
+                    The main purpose of this library is to help you create a bot and implement its functionality. It makes the process simpler and easier.
+                </text>
+                <text>
+                    Our goal is to provide you, as developers, with complete freedom of action and to highlight the benefits of Hikari.
+                </text>
+            </p>
+        </div>
+    </div>
 </div>
 
 # Installation
 > [!NOTE]
 > Aurum requires Python 3.10 or higher.
 
 Run command:
```


# Comparing `tmp/pyprland-2.3.0.tar.gz` & `tmp/pyprland-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.3.0.tar", max compression
+gzip compressed data, was "pyprland-2.3.1.tar", max compression
```

## Comparing `pyprland-2.3.0.tar` & `pyprland-2.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.3.0/LICENSE
--rw-r--r--   0        0        0     5427 2024-05-18 15:13:31.365799 pyprland-2.3.0/README.md
--rw-r--r--   0        0        0       24 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/__init__.py
--rw-r--r--   0        0        0       38 2024-05-16 19:14:17.148810 pyprland-2.3.0/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      386 2024-05-16 19:14:17.148810 pyprland-2.3.0/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4848 2024-05-18 13:01:21.799747 pyprland-2.3.0/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     1462 2024-05-16 20:28:22.384986 pyprland-2.3.0/pyprland/adapters/units.py
--rw-r--r--   0        0        0    18462 2024-05-17 22:31:04.698344 pyprland-2.3.0/pyprland/command.py
--rw-r--r--   0        0        0     8470 2024-05-17 21:59:35.557745 pyprland-2.3.0/pyprland/common.py
--rw-r--r--   0        0        0     8086 2024-05-17 22:07:11.198968 pyprland-2.3.0/pyprland/ipc.py
--rw-r--r--   0        0        0       49 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      115 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1658 2024-05-16 20:12:25.826075 pyprland-2.3.0/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1370 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2723 2024-05-17 21:51:17.035559 pyprland-2.3.0/pyprland/plugins/gbar.py
--rw-r--r--   0        0        0     2655 2024-05-16 20:24:49.329951 pyprland-2.3.0/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     8084 2024-05-18 12:50:01.915976 pyprland-2.3.0/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1731 2024-05-16 20:31:35.359564 pyprland-2.3.0/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     2514 2024-05-18 12:40:23.740738 pyprland-2.3.0/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0    11159 2024-05-18 15:09:44.027753 pyprland-2.3.0/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     3817 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0     3121 2024-05-16 20:27:48.054173 pyprland-2.3.0/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    31607 2024-05-18 13:08:09.554633 pyprland-2.3.0/pyprland/plugins/scratchpads/__init__.py
--rw-r--r--   0        0        0     2842 2024-05-17 17:55:08.207991 pyprland-2.3.0/pyprland/plugins/scratchpads/animations.py
--rw-r--r--   0        0        0     2702 2024-05-18 12:34:55.300430 pyprland-2.3.0/pyprland/plugins/scratchpads/helpers.py
--rw-r--r--   0        0        0     4036 2024-05-18 13:07:36.207295 pyprland-2.3.0/pyprland/plugins/scratchpads/lookup.py
--rw-r--r--   0        0        0     5997 2024-05-18 13:08:46.975391 pyprland-2.3.0/pyprland/plugins/scratchpads/objects.py
--rw-r--r--   0        0        0     1103 2024-05-16 20:02:45.022300 pyprland-2.3.0/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4245 2024-05-18 12:58:41.979853 pyprland-2.3.0/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     4804 2024-05-16 20:40:18.898697 pyprland-2.3.0/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      570 2024-05-16 19:14:17.152144 pyprland-2.3.0/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1120 2024-05-16 19:55:58.745845 pyprland-2.3.0/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     5610 2024-05-17 21:59:53.718191 pyprland-2.3.0/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2496 2024-05-16 19:55:44.465502 pyprland-2.3.0/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0     1459 2024-05-17 22:24:00.284438 pyprland-2.3.0/pyprland/types.py
--rw-r--r--   0        0        0       42 2024-05-18 15:39:48.487505 pyprland-2.3.0/pyprland/version.py
--rw-r--r--   0        0        0     2124 2024-05-18 15:39:48.484172 pyprland-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 pyprland-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.3.1/LICENSE
+-rw-r--r--   0        0        0     5427 2024-05-18 15:13:31.365799 pyprland-2.3.1/README.md
+-rw-r--r--   0        0        0       24 2024-05-16 19:14:17.152144 pyprland-2.3.1/pyprland/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-16 19:14:17.148810 pyprland-2.3.1/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      386 2024-05-16 19:14:17.148810 pyprland-2.3.1/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4848 2024-05-19 09:02:05.262228 pyprland-2.3.1/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1462 2024-05-16 20:28:22.384986 pyprland-2.3.1/pyprland/adapters/units.py
+-rw-r--r--   0        0        0    18490 2024-05-18 23:11:38.369254 pyprland-2.3.1/pyprland/command.py
+-rw-r--r--   0        0        0     8853 2024-05-19 09:03:46.053494 pyprland-2.3.1/pyprland/common.py
+-rw-r--r--   0        0        0     8097 2024-05-19 00:15:04.411549 pyprland-2.3.1/pyprland/ipc.py
+-rw-r--r--   0        0        0       49 2024-05-16 19:14:17.152144 pyprland-2.3.1/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-16 19:14:17.152144 pyprland-2.3.1/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1658 2024-05-16 20:12:25.826075 pyprland-2.3.1/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1370 2024-05-16 19:14:17.152144 pyprland-2.3.1/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2723 2024-05-17 21:51:17.035559 pyprland-2.3.1/pyprland/plugins/gbar.py
+-rw-r--r--   0        0        0     2657 2024-05-19 00:11:17.726169 pyprland-2.3.1/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     8084 2024-05-18 12:50:01.915976 pyprland-2.3.1/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1731 2024-05-16 20:31:35.359564 pyprland-2.3.1/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     2519 2024-05-20 13:22:13.839156 pyprland-2.3.1/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0    11159 2024-05-18 15:09:44.027753 pyprland-2.3.1/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     3817 2024-05-16 19:14:17.152144 pyprland-2.3.1/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0     3121 2024-05-16 20:27:48.054173 pyprland-2.3.1/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    31614 2024-05-18 23:58:44.507673 pyprland-2.3.1/pyprland/plugins/scratchpads/__init__.py
+-rw-r--r--   0        0        0     2842 2024-05-17 17:55:08.207991 pyprland-2.3.1/pyprland/plugins/scratchpads/animations.py
+-rw-r--r--   0        0        0     2702 2024-05-18 12:34:55.300430 pyprland-2.3.1/pyprland/plugins/scratchpads/helpers.py
+-rw-r--r--   0        0        0     4036 2024-05-18 13:07:36.207295 pyprland-2.3.1/pyprland/plugins/scratchpads/lookup.py
+-rw-r--r--   0        0        0     6033 2024-05-18 23:57:10.361129 pyprland-2.3.1/pyprland/plugins/scratchpads/objects.py
+-rw-r--r--   0        0        0     1103 2024-05-16 20:02:45.022300 pyprland-2.3.1/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4245 2024-05-18 12:58:41.979853 pyprland-2.3.1/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     4804 2024-05-16 20:40:18.898697 pyprland-2.3.1/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      570 2024-05-16 19:14:17.152144 pyprland-2.3.1/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1120 2024-05-16 19:55:58.745845 pyprland-2.3.1/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     5610 2024-05-17 21:59:53.718191 pyprland-2.3.1/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2496 2024-05-16 19:55:44.465502 pyprland-2.3.1/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0     1459 2024-05-17 22:24:00.284438 pyprland-2.3.1/pyprland/types.py
+-rw-r--r--   0        0        0       42 2024-05-20 13:24:38.702217 pyprland-2.3.1/pyprland/version.py
+-rw-r--r--   0        0        0     2124 2024-05-20 13:24:38.695550 pyprland-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 pyprland-2.3.1/PKG-INFO
```

### Comparing `pyprland-2.3.0/LICENSE` & `pyprland-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/README.md` & `pyprland-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/adapters/menus.py` & `pyprland-2.3.1/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/adapters/units.py` & `pyprland-2.3.1/pyprland/adapters/units.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/command.py` & `pyprland-2.3.1/pyprland/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import itertools
 import json
 import os
 import sys
 import tomllib
 from collections.abc import Callable
 from functools import partial
-from typing import Any, Self
+from typing import Any, Self, cast
 
 from pyprland.common import IPC_FOLDER, get_logger, init_logger, merge, run_interactive_program
 from pyprland.ipc import get_event_stream, notify_error, notify_fatal, notify_info
 from pyprland.ipc import init as ipc_init
 from pyprland.plugins.interface import Plugin
 from pyprland.types import PyprError
 from pyprland.version import VERSION
@@ -172,15 +172,15 @@
         plugin.log.debug("%s%s", name, params)
 
     def colored_log_handler(self, plugin: Plugin, name: str, params: tuple[str]) -> None:
         """Log a handler method with color."""
         color = 33 if name.startswith("run_") else 30
         plugin.log.debug("\033[%s;1m%s%s\033[0m", color, name, params)
 
-    async def _run_plugin_handler(self, plugin: Plugin, full_name: str, params: tuple[str]) -> None:
+    async def _run_plugin_handler(self, plugin: Plugin, full_name: str, params: tuple[str, ...]) -> None:
         """Run a single handler on a plugin."""
         self.log_handler(plugin, full_name, params)
         try:
             await getattr(plugin, full_name)(*params)
         except AssertionError as e:
             self.log.exception("This could be a bug in Pyprland, if you think so, report on https://github.com/fdev31/pyprland/issues")
             await notify_error(f"Pypr integrity check failed on {plugin.name}::{full_name}: {e}")
@@ -342,15 +342,15 @@
     manager = Pyprland()
     manager.server = await asyncio.start_unix_server(manager.read_command, CONTROL)
 
     events_reader, events_writer = await get_event_stream_with_retry()
     if events_reader is None:
         manager.log.critical("Failed to open hyprland event stream: %s.", events_writer)
         await notify_fatal("Failed to open hyprland event stream")
-        raise PyprError from events_writer
+        raise PyprError from cast(Exception, events_writer)
 
     manager.event_reader = events_reader
 
     await manager.initialize()
 
     manager.log.debug("[ initialized ]".center(80, "="))
 
@@ -374,15 +374,15 @@
 
     def format_doc(txt: str) -> str:
         return txt.split("\n")[0]
 
     print(
         """Syntax: pypr [command]
 
-If the command is ommited, runs the daemon which will start every configured plugin.
+If the command is omitted, runs the daemon which will start every configured plugin.
 
 Available commands:
 """
     )
     builtins_docs = {
         "dumpjson": "Dump the configuration in JSON format.",
         "edit": "Edit the configuration file.",
```

### Comparing `pyprland-2.3.0/pyprland/common.py` & `pyprland-2.3.1/pyprland/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,41 @@
 __all__ = [
     "DEBUG",
     "apply_variables",
     "get_logger",
     "merge",
     "run_interactive_program",
     "state",
+    "init_logger",
+    "SharedState",
+    "prepare_for_quotes",
+    "apply_filter",
+    "CastBoolMixin",
+    "is_rotated",
 ]
 
+
 DEBUG = os.environ.get("DEBUG", False)
 
-HYPRLAND_INSTANCE_SIGNATURE = os.environ["HYPRLAND_INSTANCE_SIGNATURE"]
+HYPRLAND_INSTANCE_SIGNATURE = os.environ.get("HYPRLAND_INSTANCE_SIGNATURE", "NO_INSTANCE")
 
-MINIMUM_ADDR_LEN = 10
+MINIMUM_ADDR_LEN = 4
 
 try:
-    IPC_FOLDER = (
+    original_ipc_folder = (
         f'{os.environ["XDG_RUNTIME_DIR"]}/hypr/{HYPRLAND_INSTANCE_SIGNATURE}'
         if os.path.exists(f'{os.environ["XDG_RUNTIME_DIR"]}/hypr/{HYPRLAND_INSTANCE_SIGNATURE}')
         else f"/tmp/hypr/{HYPRLAND_INSTANCE_SIGNATURE}"  # noqa: S108
     )
+
+    IPC_FOLDER = f"/tmp/.hypr-{HYPRLAND_INSTANCE_SIGNATURE}"  # noqa: S108
+    # make a link from short path to original path
+    if not os.path.exists(IPC_FOLDER):
+        os.symlink(original_ipc_folder, IPC_FOLDER)
+
 except KeyError:
     print("This is a fatal error, assuming we are running documentation generation or testing in a sandbox, hence ignoring it")
     IPC_FOLDER = "/fake"
 
 
 def set_terminal_size(descriptor: int, rows: int, cols: int) -> None:
     """Set the terminal size."""
@@ -194,15 +207,15 @@
     active_monitor: str = ""  # monitor name
     active_window: str = ""  # window address
     variables: dict = field(default_factory=dict)
     monitors: list[str] = field(default_factory=list)
     hyprland_version: VersionInfo = field(default_factory=VersionInfo)
 
 
-state = SharedState()
+state: SharedState = SharedState()
 """
 Exposes most-commonly accessed attributes to avoid specific IPC requests
 - `active_monitor` monitor's name
 - `active_workspace` workspace's name
 - `active_window` window's address
 """
```

### Comparing `pyprland-2.3.0/pyprland/ipc.py` & `pyprland-2.3.1/pyprland/ipc.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,31 +155,35 @@
         name: (optional) monitor name
 
     Returns:
         dict() with the focused monitor properties
     """
     if name:
 
-        def match_fn(mon: MonitorInfo) -> bool:
+        def _match_fn(mon: MonitorInfo) -> bool:
             return mon["name"] == name
-
     else:
 
-        def match_fn(mon: MonitorInfo) -> bool:
+        def _match_fn(mon: MonitorInfo) -> bool:
             return cast(bool, mon.get("focused"))
 
     for monitor in await hyprctl_json("monitors", logger=logger):
-        if match_fn(cast(MonitorInfo, monitor)):
-            return monitor  # type: ignore
+        if _match_fn(cast(MonitorInfo, monitor)):
+            return cast(MonitorInfo, monitor)
     msg = "no focused monitor"
     raise RuntimeError(msg)
 
 
+def default_match_fn(value1: Any, value2: Any) -> bool:  # noqa: ANN401
+    """Default match function."""
+    return bool(value1 == value2)
+
+
 async def get_client_props(
-    logger: Logger | None = None, match_fn: Callable | None = None, clients: list[ClientInfo] | None = None, **kw
+    logger: Logger | None = None, match_fn: Callable = default_match_fn, clients: list[ClientInfo] | None = None, **kw
 ) -> ClientInfo | None:
     """Return the properties of a client that matches the given `match_fn` (or default to equality) given the keyword arguments.
 
     Eg.
         # will return the properties of the client with address "0x1234"
         get_client_props(logger, addr="0x1234")
 
@@ -208,19 +212,14 @@
         prop_value = addr
     elif klass:
         prop_name = "class"
         prop_value = klass
     else:
         prop_name, prop_value = next(iter(kw.items()))
 
-    if match_fn is None:
-
-        def match_fn(value1: Any, value2: Any) -> bool:  # noqa: ANN401
-            return bool(value1 == value2)
-
     for client in clients or await hyprctl_json("clients", logger=logger):
         assert isinstance(client, dict)
         if match_fn(client.get(prop_name), prop_value):
             return client  # type: ignore
     return None
```

### Comparing `pyprland-2.3.0/pyprland/plugins/expose.py` & `pyprland-2.3.1/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.3.1/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/gbar.py` & `pyprland-2.3.1/pyprland/plugins/gbar.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/interface.py` & `pyprland-2.3.1/pyprland/plugins/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     notify_info: Callable
     " `pyprland.ipc.notify_info` using the pluggin's logger "
 
     notify_error: Callable
     " `pyprland.ipc.notify_error` using the pluggin's logger "
 
     config: dict[str, Any]
-    " This plugin configuration section as a dict object "
+    " This plugin configuration section as a `dict` object "
 
     def __init__(self, name: str) -> None:
         """Create a new plugin `name` and the matching logger."""
         self.name = name
         """ the plugin name """
         self.log = get_logger(name)
         """ the logger to use for this plugin """
```

### Comparing `pyprland-2.3.0/pyprland/plugins/layout_center.py` & `pyprland-2.3.1/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/lost_windows.py` & `pyprland-2.3.1/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/magnify.py` & `pyprland-2.3.1/pyprland/plugins/magnify.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 class Extension(Plugin):  # pylint: disable=missing-class-docstring
     """Control workspace zooming."""
 
     zoomed = False
 
     cur_factor = 1.0
 
-    def ease_out_quad(self, step: int, start: int, end: int, duration: int) -> int:
+    def ease_out_quad(self, step: float, start: int, end: int, duration: int) -> float:
         """Easing function for animations."""
-        step //= duration
+        step /= duration
         return -end * step * (step - 2) + start
 
-    def animated_eased_zoom(self, start: int, end: int, duration: int) -> Iterable[int]:
+    def animated_eased_zoom(self, start: int, end: int, duration: int) -> Iterable[float]:
         """Add easing to an animation.
 
         This function is a generator that yields the next value of the animation
 
         Args:
             start (float): starting value
             end (float): ending value
```

### Comparing `pyprland-2.3.0/pyprland/plugins/monitors.py` & `pyprland-2.3.1/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/monitors_v0.py` & `pyprland-2.3.1/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/pyprland.py` & `pyprland-2.3.1/pyprland/plugins/pyprland.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/scratchpads/__init__.py` & `pyprland-2.3.1/pyprland/plugins/scratchpads/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
             await self._configure_windowrules(scratch)
 
     async def event_activewindowv2(self, addr: str) -> None:
         """Active windows hook."""
         full_address = "" if not addr or len(addr) < MINIMUM_ADDR_LEN else "0x" + addr
         for uid, scratch in self.scratches.items():
             if not scratch.client_info:
-                continue
+                continue  # type: ignore
             if scratch.have_address(full_address):
                 self.last_focused = scratch
                 self.cancel_task(uid)
             elif scratch.visible and scratch.conf.get("unfocus") == "hide":
                 last_shown = scratch.meta.last_shown
                 if last_shown + AFTER_SHOW_INHIBITION > time.time():
                     self.log.debug(
@@ -344,16 +344,15 @@
             return False
         self.log.debug("Lookup hack triggered")
         clients = cast(list[ClientInfo], await self.hyprctl_json("clients"))
         for pending_scratch in class_lookup_hack:
             match_by, match_value = pending_scratch.get_match_props()
             match_fn = get_match_fn(match_by, match_value)
             for client in clients:
-                assert isinstance(client, dict)
-                if match_fn(client[match_by], match_value):
+                if match_fn(client[match_by], match_value):  # type: ignore
                     self.scratches.register(pending_scratch, addr=client["address"][2:])
                     self.log.debug("client class found: %s", client)
                     await pending_scratch.update_client_info(client)
         return True
 
     async def event_openwindow(self, params: str) -> None:
         """Open windows hook."""
@@ -627,15 +626,15 @@
             else:
                 self.log.exception("Lost the client info for %s", scratch.uid)
 
     async def _animate_show(self, scratch: Scratch, monitor: MonitorInfo, relative_animation: bool) -> None:
         """Animate the show transition."""
         animation_type = get_animation_type(scratch)
         if animation_type:
-            offset = tuple(-1 * n for n in await self.get_offsets(scratch, monitor))
+            offset = cast(tuple[int, int], tuple(-1 * n for n in await self.get_offsets(scratch, monitor)))
             if relative_animation:
                 # Relative positioning
                 if "size" not in scratch.client_info:
                     await self.update_scratch_info(scratch)  # type: ignore
 
                 await self._slide_animation(animation_type, scratch, offset)
             else:
```

### Comparing `pyprland-2.3.0/pyprland/plugins/scratchpads/animations.py` & `pyprland-2.3.1/pyprland/plugins/scratchpads/animations.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/scratchpads/helpers.py` & `pyprland-2.3.1/pyprland/plugins/scratchpads/helpers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/scratchpads/lookup.py` & `pyprland-2.3.1/pyprland/plugins/scratchpads/lookup.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/scratchpads/objects.py` & `pyprland-2.3.1/pyprland/plugins/scratchpads/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ...ipc import notify_error
 from ...types import ClientInfo, MonitorInfo, VersionInfo
 from .helpers import OverridableConfig, get_match_fn
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
-    import pyprland.plugins.scratchpads.Extension as PyprlandPlugin
+    import pyprland.plugins.scratchpads as _scratchpads_extension_m
 
     class ClientPropGetter(Protocol):
         """type for the get_client_props function."""
 
         async def __call__(self, match_fn: Callable | None = None, clients: list[ClientInfo] | None = None, **kw) -> ClientInfo | None:
             pass
 
@@ -72,15 +72,15 @@
 
         self.conf = opts
 
     def have_address(self, addr: str) -> bool:
         """Check if the address is the same as the client."""
         return addr == self.full_address or addr in self.extra_addr
 
-    async def initialize(self, ex: "PyprlandPlugin") -> None:
+    async def initialize(self, ex: "_scratchpads_extension_m.Extension") -> None:
         """Initialize the scratchpad."""
         if self.meta.initialized:
             return
         self.meta.initialized = True
         await self.update_client_info()
         await ex.hyprctl(f"movetoworkspacesilent special:scratch_{self.uid},address:{self.full_address}")
         if "class_match" in self.conf:  # NOTE: legacy, to be removed
@@ -147,15 +147,15 @@
             client_info = await self.get_client_props(addr=self.full_address, clients=clients)
         if not isinstance(client_info, dict):
             if client_info is None:
                 self.log.error("The client window %s vanished", self.full_address)
                 msg = f"Client window {self.full_address} not found"
                 raise KeyError(msg)
             # Unexpected type:
-            self.log.error("client_info of %s must be a dict: %s", self.address, client_info)
+            self.log.error("client_info of %s must be a dict: %s", self.address, client_info)  # type: ignore
             msg = f"Not a dict: {client_info}"
             raise TypeError(msg)
 
         self.client_info.update(client_info)
 
     def __str__(self) -> str:
         return f"{self.uid} {self.address} : {self.client_info} / {self.conf}"
```

### Comparing `pyprland-2.3.0/pyprland/plugins/shift_monitors.py` & `pyprland-2.3.1/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.3.1/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/system_notifier.py` & `pyprland-2.3.1/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/toggle_dpms.py` & `pyprland-2.3.1/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/toggle_special.py` & `pyprland-2.3.1/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/wallpapers.py` & `pyprland-2.3.1/pyprland/plugins/wallpapers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.3.1/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyprland/types.py` & `pyprland-2.3.1/pyprland/types.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.0/pyproject.toml` & `pyprland-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyprland"
-version = "2.3.0"
+version = "2.3.1"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.3.0/PKG-INFO` & `pyprland-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.3.0
+Version: 2.3.1
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


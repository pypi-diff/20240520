# Comparing `tmp/simple_config_sync-0.1.13.tar.gz` & `tmp/simple_config_sync-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_config_sync-0.1.13.tar", last modified: Mon May 20 03:59:40 2024, max compression
+gzip compressed data, was "simple_config_sync-0.1.5.tar", last modified: Wed Mar 27 02:15:35 2024, max compression
```

## Comparing `simple_config_sync-0.1.13.tar` & `simple_config_sync-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,10 @@
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-05-20 03:59:40.564103 simple_config_sync-0.1.13/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      877 2024-05-20 03:59:40.564103 simple_config_sync-0.1.13/PKG-INFO
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      360 2024-05-07 03:26:05.000000 simple_config_sync-0.1.13/README.md
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      933 2024-05-20 02:44:33.000000 simple_config_sync-0.1.13/pyproject.toml
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       38 2024-05-20 03:59:40.564103 simple_config_sync-0.1.13/setup.cfg
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-05-20 03:59:40.562102 simple_config_sync-0.1.13/src/
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-05-20 03:59:40.562102 simple_config_sync-0.1.13/src/simple_config_sync/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       43 2024-04-16 22:04:22.000000 simple_config_sync-0.1.13/src/simple_config_sync/__init__.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       68 2024-04-14 20:37:08.000000 simple_config_sync-0.1.13/src/simple_config_sync/__main__.py
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-05-20 03:59:40.563103 simple_config_sync-0.1.13/src/simple_config_sync/core/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      193 2024-04-16 22:48:20.000000 simple_config_sync-0.1.13/src/simple_config_sync/core/__init__.py
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-05-20 03:59:40.564103 simple_config_sync-0.1.13/src/simple_config_sync/core/assets/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     1338 2024-04-16 23:22:06.000000 simple_config_sync-0.1.13/src/simple_config_sync/core/assets/tui.tcss
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      606 2024-05-20 03:21:54.000000 simple_config_sync-0.1.13/src/simple_config_sync/core/backup.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      222 2024-04-16 20:18:30.000000 simple_config_sync-0.1.13/src/simple_config_sync/core/cli.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     5625 2024-05-20 02:09:37.000000 simple_config_sync-0.1.13/src/simple_config_sync/core/config.py
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     4879 2024-05-20 03:15:40.000000 simple_config_sync-0.1.13/src/simple_config_sync/core/tui.py
-drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-05-20 03:59:40.564103 simple_config_sync-0.1.13/src/simple_config_sync.egg-info/
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      877 2024-05-20 03:59:40.000000 simple_config_sync-0.1.13/src/simple_config_sync.egg-info/PKG-INFO
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      602 2024-05-20 03:59:40.000000 simple_config_sync-0.1.13/src/simple_config_sync.egg-info/SOURCES.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)        1 2024-05-20 03:59:40.000000 simple_config_sync-0.1.13/src/simple_config_sync.egg-info/dependency_links.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      124 2024-05-20 03:59:40.000000 simple_config_sync-0.1.13/src/simple_config_sync.egg-info/entry_points.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       70 2024-05-20 03:59:40.000000 simple_config_sync-0.1.13/src/simple_config_sync.egg-info/requires.txt
--rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       19 2024-05-20 03:59:40.000000 simple_config_sync-0.1.13/src/simple_config_sync.egg-info/top_level.txt
+-rw-r--r--   0        0        0      360 2024-02-28 02:46:26.939911 simple_config_sync-0.1.5/README.md
+-rw-r--r--   0        0        0      762 2024-03-27 02:15:35.381741 simple_config_sync-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-26 07:16:06.313934 simple_config_sync-0.1.5/src/simple_config_sync/__init__.py
+-rw-r--r--   0        0        0      146 2024-02-27 03:13:57.975540 simple_config_sync-0.1.5/src/simple_config_sync/core/__init__.py
+-rw-r--r--   0        0        0     1203 2024-03-27 02:02:07.190528 simple_config_sync-0.1.5/src/simple_config_sync/core/assets/tui.tcss
+-rw-r--r--   0        0        0     4736 2024-03-27 02:13:20.351783 simple_config_sync-0.1.5/src/simple_config_sync/core/config.py
+-rw-r--r--   0        0        0      265 2024-02-27 17:11:02.534641 simple_config_sync-0.1.5/src/simple_config_sync/core/scripts.py
+-rw-r--r--   0        0        0     3268 2024-03-27 02:05:17.418826 simple_config_sync-0.1.5/src/simple_config_sync/core/tui.py
+-rw-r--r--   0        0        0        0 2024-02-26 07:16:06.312934 simple_config_sync-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 simple_config_sync-0.1.5/PKG-INFO
```

### Comparing `simple_config_sync-0.1.13/src/simple_config_sync/core/assets/tui.tcss` & `simple_config_sync-0.1.5/src/simple_config_sync/core/assets/tui.tcss`

 * *Files 22% similar despite different names*

```diff
@@ -12,86 +12,76 @@
 }
 
 Panel > * {
     width: 1fr;
     margin-bottom: 1;
 }
 
-UOption {
+Option {
     layout: grid;
     grid-size: 2;
     grid-gutter: 1;
     grid-columns: 16 1fr;
     margin: 1;
     width: 1fr;
     height: auto;
 }
 
-UOption #sync {
+Option #sync {
     width: 1fr;
 }
 
-UOption #content {
+Option #content {
     width: 1fr;
     height: auto;
 }
 
-UOption #info {
+Option #info {
     layout: horizontal;
     width: 1fr;
     height: auto;
 }
 
-UOption #info > * {
+Option #info > * {
     margin-right: 2;
     width: auto;
     height: auto;
 }
 
-UOption #info #name {
+Option #info #name {
     text-style: bold;
 }
 
-UOption #info #status {
-    text-style: bold;
-}
-
-UOption #info #status.added {
+Option #info #status.added {
     color: #0f0;
 }
 
-UOption #info #status.modified {
+Option #info #status.modified {
     color: #ff0;
 }
 
-UOption #info #status.deleted {
+Option #info #status.deleted {
     color: #f00;
 }
 
-UOption #depends {
-    width: 1fr;
-    height: auto;
-}
-
-ULinkList {
+Option #links {
     width: 1fr;
     height: auto;
 }
 
-ULink {
-    margin-left: 2;
+Link {
     height: auto;
 }
 
-ULink > * {
+Link > * {
     width: auto;
     margin-right: 2;
 }
 
-ULink .status {
+Link .hint {
     text-style: bold;
 }
 
 .text-blue,
 .text-primary {
     color: #00f;
 }
```

### Comparing `simple_config_sync-0.1.13/src/simple_config_sync/core/config.py` & `simple_config_sync-0.1.5/src/simple_config_sync/core/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,198 +1,177 @@
 import os
+import shutil
 from copy import deepcopy
-from functools import cached_property
 from pathlib import Path
-from typing import Literal, Protocol
+from typing import Literal
 
 import toml
 
-from .backup import backup, restore
+Status = Literal['added', 'modified', 'deleted', '']
 
-Status = Literal["added", "modified", "deleted", ""]
 
+default_config_path = Path('./config-sync.toml')
+default_lock_path = Path('./config-sync.lock')
 
-class OptionProtocol(Protocol):
-    def sync(self) -> None: ...
-    def uninstall(self, clean: bool = False) -> None: ...
 
+def load(config_path: Path | None = None, lock_path: Path | None = None) -> None:
+    config_path = config_path or default_config_path
+    lock_path = lock_path or default_lock_path
 
-class Link(OptionProtocol):
-    def __init__(self, d: dict) -> None:
-        self.d = d
+    if not config_path.exists():
+        raise FileNotFoundError(f'Could not find config file: {config_path}')
 
-    def __eq__(self, value: "Option") -> bool:
-        return self.d == value.d
+    config = toml.load(config_path)
+    lock_cfg = toml.load(lock_path) if lock_path.exists() else {}
 
-    def sync(self):
-        if not self.source.exists():
-            raise FileNotFoundError(f"Source file not found: {self.source}")
-        if self.target.exists():
-            self.clean_target()
-        self.target.parent.mkdir(parents=True, exist_ok=True)
-        self.target.symlink_to(self.source.resolve(), self.source.is_dir())
+    ops: dict = config.get('options', {})
+    lock_ops: dict = lock_cfg.get('options', {})
 
-    def uninstall(self) -> None:
-        if self.linked:
-            self.target.unlink()
-        restore(self.target)
+    options.clear()
+    options.update({k: SyncOp(ops.get(k), lock_ops.get(k)) for k in sorted(set(ops).union(lock_ops))})
+
+
+def make_lock_file(lock_path: Path | None = None) -> None:
+    lock_path = lock_path or default_lock_path
+
+    config = {'options': {}}
+    for k, op in options.items():
+        if op.status == 'deleted':
+            continue
+        config['options'][k] = op.d
+    with lock_path.open('w') as file:
+        toml.dump(config, file)
 
-    def clean_target(self) -> None:
-        if not self.target.exists():
+
+class Link(dict):
+    def install(self):
+        if self.linked:
             return
-        backup(self.target)
+        source = self.source
+        target = self.target
+        if target.is_symlink() or target.is_file():
+            target.unlink()
+        elif target.is_dir():
+            shutil.rmtree(target)
+        target.parent.mkdir(parents=True, exist_ok=True)
+        target.symlink_to(source.absolute(), source.is_dir())
+
+    def uninstall(self):
+        target = self.target
+        if target.exists() and target.is_symlink():
+            target.unlink()
 
     @property
-    def linked(self) -> bool:
-        if not self.target.exists() or not self.target.is_symlink():
-            return False
-        return self.source.resolve() == self.target.readlink()
-
-    @cached_property
     def source(self) -> Path:
-        return Path(os.path.expandvars(self.d.get("source", ""))).expanduser()
+        return Path(os.path.expandvars(self.get('source', ''))).expanduser()
 
-    @cached_property
+    @source.setter
+    def source(self, value: Path | str):
+        self['source'] = str(value)
+
+    @property
     def target(self) -> Path:
-        return Path(os.path.expandvars(self.d.get("target", ""))).expanduser()
+        return Path(os.path.expandvars(self.get('target', ''))).expanduser()
+
+    @target.setter
+    def target(self, value: Path | str):
+        self['target'] = str(value)
+
+    @property
+    def target_exists(self) -> bool:
+        target = self.target
+        return target.exists() or target.is_symlink()
 
+    @property
+    def linked(self) -> bool:
+        target = self.target
+        if not target.is_symlink():
+            return False
+        return target.readlink() == self.source.absolute()
 
-class Option(OptionProtocol):
-    def __init__(self, name: str, d: dict | None) -> None:
-        self.name = name
+
+class Option:
+    def __init__(self, d: dict | None = None):
         self.d = d or {}
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
-        return f"{self.__class__.__name__}({self.name})"
+        return f'{self.__class__.__name__}({self.description})'
 
     def __bool__(self) -> bool:
         return bool(self.d)
 
-    def __eq__(self, value: "Option") -> bool:
-        return self.name == value.name
-
-    def sync(self) -> None:
-        for link in self.links:
-            link.sync()
-
-    def uninstall(self, clean: bool = False) -> None:
-        for link in self.links:
-            link.uninstall()
-
     @property
     def group(self) -> str:
-        return self.d.get("group", "")
+        return self.d.get('group', '')
 
     @property
     def description(self) -> str:
-        return self.d.get("description", "")
+        return self.d.get('description', '')
 
     @property
     def links(self) -> list[Link]:
-        return [Link(i) for i in self.d.get("links", [])]
-
-    @property
-    def depends(self) -> dict[str, list]:
-        return self.d.get("depends", {})
+        return [Link(i) for i in self.d.get('links', [])]
 
     @property
     def synced(self) -> bool:
-        return self.d.get("synced", False)
+        return self.d.get('synced', True)
 
     @synced.setter
-    def synced(self, value: bool) -> None:
-        self.d["synced"] = value
+    def synced(self, value: bool):
+        self.d['synced'] = value
 
     @property
     def status(self) -> Status:
-        return self.d.get("status", "")
+        return self.d.get('status', '')
 
+    @property
+    def dependencies(self) -> list[str]:
+        return self.d.get('dependencies', [])
 
-class SyncOp(Option, OptionProtocol):
-    def __init__(self, name: str, op: dict | None = None, lock_op: dict | None = None):
+
+class SyncOp(Option):
+    def __init__(self, op: dict | None = None, lock_op: dict | None = None):
         assert op or lock_op
-        self.op = Option(name, op)
-        self.lock_op = Option(name, lock_op)
-        super().__init__(name, self._sync_op())
-
-    def _sync_op(self) -> dict:
-        synced: bool = bool(self.op and (self.lock_op and self.lock_op.synced))
-        if self.status == "deleted":
-            return deepcopy(self.lock_op.d) | {"synced": synced}
-        return deepcopy(self.op.d) | {"synced": synced}
+        self.op = Option(op)
+        self.lock_op = Option(lock_op)
+        super().__init__(self.sync_lock())
+        self.synced = self.lock_op.synced if self.lock_op else self.op.synced
+
+    def sync_lock(self):
+        if self.status == 'deleted':
+            return deepcopy(self.lock_op.d)
+        return deepcopy(self.op.d)
 
-    def sync(self) -> None:
-        if not self.synced:
+    def install(self):
+        for link in self.links:
+            link.install()
+
+    def uninstall(self):
+        self.status = 'deleted'
+        for link in self.lock_op.links:
+            link.uninstall()
+
+    def sync(self):
+        if self.status == 'deleted' or not self.synced:
             self.uninstall()
-            return
-        self.lock_op.uninstall()
-        self.op.sync()
-        self.synced = True
-
-    def uninstall(self, clean: bool = False) -> None:
-        self.lock_op.uninstall(clean=clean)
-        self.synced = False
+        else:
+            self.install()
 
     @property
     def status(self) -> Status:
         if not self.op:
-            return "deleted"
-        if not self.lock_op:
-            return "added"
+            return 'deleted'
+        if not self.lock_op or self.lock_op.status == 'deleted' or not self.lock_op.synced:
+            return 'added'
         if self.op.links != self.lock_op.links:
-            return "modified"
-        return ""
+            return 'modified'
+        return ''
 
     @status.setter
     def status(self, value: Status):
-        self.d["status"] = value
-
-
-class Config:
-    def __init__(self) -> None:
-        self.path = Path("config-sync.toml")
-        self.lock_path = Path("config-sync.lock")
-        self.opt_names: list[str] = []
-        self.lock_opt_names: list[str] = []
-        self.opts: list[SyncOp] = []
-
-    def load(self) -> None:
-        with open(self.path) as f:
-            d = toml.load(f)
-            opts: dict = d.get("options", {})
-        if self.lock_path.exists():
-            with open(self.lock_path) as f:
-                lock_d = toml.load(f)
-            lock_opts: dict = lock_d.get("options", {})
-        else:
-            lock_opts = {}
-        self.opt_names = list(opts.keys())
-        self.lock_opt_names = list(lock_opts.keys())
-        self.opts.clear()
-        self.opts.extend(SyncOp(i, opts[i], lock_opts.get(i)) for i in opts)
-        self.opts.extend(SyncOp(i, None, lock_opts[i]) for i in lock_opts if i not in opts)
-
-    def lock(self) -> None:
-        with open(self.lock_path, "w") as f:
-            toml.dump({"options": {i.name: i.d for i in self.opts if i.op}}, f)
-
-    def sync(self) -> None:
-        for op in filter(lambda x: x.status == "deleted", self.opts):
-            op.sync()
-        for op in filter(lambda x: x.status != "deleted", self.opts):
-            op.sync()
-        self.lock()
-        self.load()
-
-    def uninstall(self) -> None:
-        for op in self.opts:
-            if op.name not in self.lock_opt_names:
-                continue
-            op.uninstall()
-        self.lock()
-        self.load()
+        self.d['status'] = value
 
 
-config = Config()
+options: dict[str, SyncOp] = {}
```


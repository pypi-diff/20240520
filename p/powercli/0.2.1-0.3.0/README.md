# Comparing `tmp/powercli-0.2.1.tar.gz` & `tmp/powercli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powercli-0.2.1.tar", last modified: Sat Mar 30 23:06:35 2024, max compression
+gzip compressed data, was "powercli-0.3.0.tar", last modified: Sun May 19 22:54:14 2024, max compression
```

## Comparing `powercli-0.2.1.tar` & `powercli-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.832605 powercli-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-30 23:06:30.000000 powercli-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-30 23:06:35.832605 powercli-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-30 23:06:30.000000 powercli-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-30 23:06:30.000000 powercli-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 23:06:35.832605 powercli-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.824605 powercli-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.828605 powercli-0.2.1/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.828605 powercli-0.2.1/src/cli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/cli/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.828605 powercli-0.2.1/src/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/commands/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/commands/open_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/commands/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.828605 powercli-0.2.1/src/cli/models/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.828605 powercli-0.2.1/src/cli/output/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/output/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/output/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/output/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/output/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/output/status.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:30.000000 powercli-0.2.1/src/cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.832605 powercli-0.2.1/src/powercli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-30 23:06:35.000000 powercli-0.2.1/src/powercli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-30 23:06:35.000000 powercli-0.2.1/src/powercli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 23:06:35.000000 powercli-0.2.1/src/powercli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-30 23:06:35.000000 powercli-0.2.1/src/powercli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-30 23:06:35.000000 powercli-0.2.1/src/powercli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-30 23:06:35.000000 powercli-0.2.1/src/powercli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:06:35.832605 powercli-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-30 23:06:30.000000 powercli-0.2.1/tests/test_cli_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-30 23:06:30.000000 powercli-0.2.1/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-30 23:06:30.000000 powercli-0.2.1/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-30 23:06:30.000000 powercli-0.2.1/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.773433 powercli-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-19 22:54:04.000000 powercli-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-19 22:54:14.773433 powercli-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-19 22:54:04.000000 powercli-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-19 22:54:04.000000 powercli-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:54:14.773433 powercli-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.769433 powercli-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.769433 powercli-0.3.0/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.769433 powercli-0.3.0/src/cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/cli/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.769433 powercli-0.3.0/src/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/commands/open_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/commands/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.769433 powercli-0.3.0/src/cli/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.769433 powercli-0.3.0/src/cli/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/output/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/output/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/output/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/output/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/output/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:04.000000 powercli-0.3.0/src/cli/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.773433 powercli-0.3.0/src/powercli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-19 22:54:14.000000 powercli-0.3.0/src/powercli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-19 22:54:14.000000 powercli-0.3.0/src/powercli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:54:14.000000 powercli-0.3.0/src/powercli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 22:54:14.000000 powercli-0.3.0/src/powercli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-19 22:54:14.000000 powercli-0.3.0/src/powercli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 22:54:14.000000 powercli-0.3.0/src/powercli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:54:14.773433 powercli-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-19 22:54:04.000000 powercli-0.3.0/tests/test_cli_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 22:54:04.000000 powercli-0.3.0/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-19 22:54:04.000000 powercli-0.3.0/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-19 22:54:04.000000 powercli-0.3.0/tests/test_runner.py
```

### Comparing `powercli-0.2.1/LICENSE` & `powercli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/PKG-INFO` & `powercli-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powercli
-Version: 0.2.1
+Version: 0.3.0
 Summary: High-level CLI interaction
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `powercli-0.2.1/README.md` & `powercli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/pyproject.toml` & `powercli-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "powercli"
-version = "0.2.1"
+version = "0.3.0"
 description = "High-level CLI interaction"
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "rich >=13.7.1, <14",
```

### Comparing `powercli-0.2.1/src/cli/commands/commands.py` & `powercli-0.3.0/src/cli/commands/commands.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/src/cli/commands/install.py` & `powercli-0.3.0/src/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/src/cli/commands/run.py` & `powercli-0.3.0/src/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/src/cli/commands/runner.py` & `powercli-0.3.0/src/cli/commands/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import io
 import os
 import subprocess
 import typing
 from collections.abc import Callable
 from dataclasses import dataclass, field
 from functools import cached_property
-from pathlib import Path
 from typing import Any, Generic, TypeVar
 
 from ..models import CalledProcessError
 from .commands import CommandItem, CommandPreparer
 
 T1 = TypeVar("T1", bound=str)
 T2 = TypeVar("T2")
@@ -26,22 +25,25 @@
     # subprocess arguments
     text: bool = True
     check: bool = True
     shell: bool = False
     input: str | None = None
     stdout: int | None = None
     stderr: int | None = None
-    cwd: Path | str | None = None
 
     verbose_errors: bool = True
     kwargs: dict[str, Any] = field(default_factory=dict)
+    subprocess_kwargs: dict[str, Any] = field(default_factory=dict)
 
     def __post_init__(self) -> None:
-        for key, value in self.kwargs.items():
-            self.__setattr__(key, value)
+        for name, value in self.kwargs.items():
+            if hasattr(self, name):
+                self.__setattr__(name, value)
+            else:
+                self.subprocess_kwargs[name] = value
 
     @cached_property
     def command_parts(self) -> tuple[str, ...]:
         use_shell_command = self.shell or self.console
         command_preparer = CommandPreparer(
             self.items, use_shell_command, self.console, self.root, self.title
         )
@@ -86,15 +88,15 @@
             text=self.text,
             check=self.check,
             shell=self.shell,
             capture_output=capture_output,
             input=self.input,
             stdout=self.stdout,
             stderr=self.stderr,
-            cwd=self.cwd,
+            **self.subprocess_kwargs,
         )
 
     def run_in_console(self) -> subprocess.Popen[str]:
         self.prepare_console_command()
         return self.launch()
 
     def launch(self) -> subprocess.Popen[str]:
@@ -107,15 +109,15 @@
     def _launch(self) -> subprocess.Popen[str]:
         return subprocess.Popen(
             self.command_parts,
             text=self.text,
             shell=self.shell,
             stdout=self.stdout,
             stderr=self.stderr,
-            cwd=self.cwd,
+            **self.subprocess_kwargs,
         )
 
     def run_with_exception_handling(
         self, runner: Callable[..., T2], *args: Any, **kwargs: Any
     ) -> T2:
         try:
             return runner(*args, **kwargs)
```

### Comparing `powercli-0.2.1/src/cli/input.py` & `powercli-0.3.0/src/cli/input.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/src/cli/output/message.py` & `powercli-0.3.0/src/cli/output/message.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/src/cli/output/progress.py` & `powercli-0.3.0/src/cli/output/progress.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/src/cli/output/rich.py` & `powercli-0.3.0/src/cli/output/rich.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/src/cli/output/status.py` & `powercli-0.3.0/src/cli/output/status.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/src/powercli.egg-info/PKG-INFO` & `powercli-0.3.0/src/powercli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powercli
-Version: 0.2.1
+Version: 0.3.0
 Summary: High-level CLI interaction
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `powercli-0.2.1/src/powercli.egg-info/SOURCES.txt` & `powercli-0.3.0/src/powercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/tests/test_progress.py` & `powercli-0.3.0/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `powercli-0.2.1/tests/test_runner.py` & `powercli-0.3.0/tests/test_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,7 +69,14 @@
     cli.run_commands(*commands)
 
 
 def test_cwd() -> None:
     with Path.tempdir() as folder:
         extracted_folder_name = cli.capture_output("pwd", cwd=folder).split("/")[-1]
     assert extracted_folder_name == folder.name
+
+
+@given(value=text_strategy())
+@linux_only_test
+def test_extra_subprocess_kwarg(value: str) -> None:
+    env = {"name": value}
+    assert cli.capture_output("echo", "$name", shell=True, env=env) == value
```


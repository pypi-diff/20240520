# Comparing `tmp/fast_dev_cli-0.7.3.tar.gz` & `tmp/fast_dev_cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dev_cli-0.7.3.tar", max compression
+gzip compressed data, was "fast_dev_cli-0.8.0.tar", last modified: Mon May 20 07:05:09 2024, max compression
```

## Comparing `fast_dev_cli-0.7.3.tar` & `fast_dev_cli-0.8.0.tar`

### file list

```diff
@@ -1,8 +1,26 @@
--rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.7.3/LICENSE
--rw-r--r--   0        0        0     2171 2024-05-13 06:12:17.707278 fast_dev_cli-0.7.3/README.md
--rw-r--r--   0        0        0      392 2024-05-09 15:36:58.837450 fast_dev_cli-0.7.3/fast_dev_cli/__init__.py
--rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.7.3/fast_dev_cli/__main__.py
--rw-r--r--   0        0        0    22059 2024-05-13 06:44:01.994013 fast_dev_cli-0.7.3/fast_dev_cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.7.3/fast_dev_cli/py.typed
--rw-r--r--   0        0        0     1407 2024-05-13 06:33:12.556585 fast_dev_cli-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 fast_dev_cli-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2136 2024-05-17 06:28:04.843495 fast_dev_cli-0.8.0/README.md
+-rw-r--r--   0        0        0      392 2024-05-09 15:36:58.837450 fast_dev_cli-0.8.0/fast_dev_cli/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.8.0/fast_dev_cli/__main__.py
+-rw-r--r--   0        0        0    22414 2024-05-19 13:57:01.821992 fast_dev_cli-0.8.0/fast_dev_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.8.0/fast_dev_cli/py.typed
+-rw-r--r--   0        0        0     1702 2024-05-20 03:21:41.699055 fast_dev_cli-0.8.0/pdm_build.py
+-rw-r--r--   0        0        0     2876 2024-05-20 07:05:09.446580 fast_dev_cli-0.8.0/pyproject.toml
+-rwxr-xr-x   0        0        0      181 2024-05-17 04:21:44.094861 fast_dev_cli-0.8.0/scripts/check.sh
+-rwxr-xr-x   0        0        0       74 2024-05-17 04:24:01.151836 fast_dev_cli-0.8.0/scripts/format.sh
+-rwxr-xr-x   0        0        0       62 2024-05-17 14:51:31.973921 fast_dev_cli-0.8.0/scripts/test.sh
+-rw-r--r--   0        0        0        0 2024-04-16 15:22:43.200424 fast_dev_cli-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1545 2024-05-17 09:11:46.760828 fast_dev_cli-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     5021 2024-05-17 09:21:40.555737 fast_dev_cli-0.8.0/tests/test_bump.py
+-rw-r--r--   0        0        0     3526 2024-05-19 14:43:59.304589 fast_dev_cli-0.8.0/tests/test_fast_test.py
+-rw-r--r--   0        0        0     2663 2024-05-17 08:46:15.928913 fast_dev_cli-0.8.0/tests/test_functions.py
+-rw-r--r--   0        0        0      289 2024-03-06 06:15:44.376466 fast_dev_cli-0.8.0/tests/test_import.py
+-rw-r--r--   0        0        0     4202 2024-05-20 02:02:31.629015 fast_dev_cli-0.8.0/tests/test_lint.py
+-rw-r--r--   0        0        0     1524 2024-05-09 14:20:03.778791 fast_dev_cli-0.8.0/tests/test_runserver.py
+-rw-r--r--   0        0        0     1917 2024-05-17 08:03:03.771865 fast_dev_cli-0.8.0/tests/test_sync.py
+-rw-r--r--   0        0        0     1837 2024-04-18 04:09:13.722510 fast_dev_cli-0.8.0/tests/test_tag.py
+-rw-r--r--   0        0        0     8700 2024-05-17 09:10:59.763906 fast_dev_cli-0.8.0/tests/test_upgrade.py
+-rw-r--r--   0        0        0      189 2024-04-12 03:40:33.542620 fast_dev_cli-0.8.0/tests/test_upload.py
+-rw-r--r--   0        0        0      376 2024-05-17 08:40:12.960695 fast_dev_cli-0.8.0/tests/test_version.py
+-rw-r--r--   0        0        0     1564 2024-04-30 10:00:32.669252 fast_dev_cli-0.8.0/tests/utils.py
+-rw-r--r--   0        0        0     3485 1970-01-01 00:00:00.000000 fast_dev_cli-0.8.0/PKG-INFO
```

### Comparing `fast_dev_cli-0.7.3/LICENSE` & `fast_dev_cli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.7.3/README.md` & `fast_dev_cli-0.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -33,19 +33,18 @@
 
 Python 3.10+
 
 ## Installation
 
 <div class="termy">
 
-```console
-$ pip install "fast-dev-cli[all]"
----> 100%
-Successfully installed fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage
+```bash
+pip install "fast-dev-cli"
 ```
+*Will install: fast-dev-cli typer ruff mypy bumpversion pytest coverage*
 
 </div>
 
 ## Usage
 
 - Lint py code:
 ```bash
@@ -68,10 +67,10 @@
 fast sync
 ```
 - Upgrade main/dev dependencies to latest version
 ```bash
 fast upgrade
 ```
 - Start a fastapi server in development mode
-```
+```bash
 fast dev
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
                          _S_t_a_t_u_s_]_[_R_u_f_f_]_[_M_y_p_y_ _C_o_v_e_r_a_g_e_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
 Python 3.10+ ## Installation
-```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
-fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage ```
+```bash pip install "fast-dev-cli" ``` *Will install: fast-dev-cli typer ruff
+mypy bumpversion pytest coverage*
 ## Usage - Lint py code: ```bash fast lint /path/to/file-or-directory ``` -
 Check only ```bash fast check ``` - Bump up version in pyproject.toml ```bash
 fast bump ``` - Run unittest and report coverage ```bash fast test ``` - Export
 requirement file and install `pip install -r ` ```bash fast sync ``` - Upgrade
 main/dev dependencies to latest version ```bash fast upgrade ``` - Start a
-fastapi server in development mode ``` fast dev ```
+fastapi server in development mode ```bash fast dev ```
```

### Comparing `fast_dev_cli-0.7.3/fast_dev_cli/cli.py` & `fast_dev_cli-0.8.0/fast_dev_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,51 @@
 from __future__ import annotations
 
-import importlib.metadata
+import importlib.metadata as importlib_metadata
 import os
 import re
 import subprocess
 import sys
 from functools import cached_property
 from pathlib import Path
 from subprocess import CompletedProcess
-from typing import TYPE_CHECKING, Optional, Type
+from typing import TYPE_CHECKING, Literal, Optional, Type
+
+import typer
+from typer import Exit, Option, echo, secho
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:  # pragma: no cover
-    from strenum import StrEnum  # type:ignore[no-redef,assignment]
+    from enum import Enum
+
     from typing_extensions import Self
 
+    class StrEnum(str, Enum):
+        __str__ = str.__str__
+
+
 if TYPE_CHECKING:  # pragma: no cover
     from typer.models import OptionInfo
 
 
-__version__ = importlib.metadata.version(Path(__file__).parent.name)
+__version__ = "0.8.0"
 
 
 def parse_files(args: list[str] | tuple[str, ...]) -> list[str]:
     return [i for i in args if not i.startswith("-")]
 
 
-try:
-    import typer
-    from typer import Exit, Option, echo, secho
-
-    cli = typer.Typer()
-    if len(sys.argv) >= 2 and sys.argv[1] == "lint":
-        if not parse_files(sys.argv[2:]):
-            sys.argv.append(".")
-except ModuleNotFoundError:
-    import click
-    from click import echo, secho
-    from click.core import Group as _Group
-    from click.exceptions import Exit
-
-    def Option(default, *shortcuts, **kw):  # type:ignore[no-redef]
-        return default
-
-    def _command(self, *args, **kwargs):
-        from click.decorators import command
-
-        def decorator(f):
-            if kwargs.get("name") == "lint":
-                import functools
-
-                def auto_fill_args(func):
-                    @functools.wraps(func)
-                    def runner(*arguments: str, **kw):
-                        if "files" not in kw and not parse_files(arguments):
-                            arguments = (".",)
-                        return func(*arguments, **kw)
-
-                    return runner
-
-                f = auto_fill_args(f)
-                if sys.argv[2:]:
-                    f = click.argument("files", nargs=-1)(f)
-            cmd = command(*args, **kwargs)(f)
-            self.add_command(cmd)
-            return cmd
-
-        return decorator
-
-    _Group.command = _command  # type:ignore
-
-    @click.group()
-    def cli() -> None: ...  # pragma: no cover
-
+if len(sys.argv) >= 2 and sys.argv[1] == "lint":
+    if not parse_files(sys.argv[2:]):
+        sys.argv.append(".")
 
 TOML_FILE = "pyproject.toml"
+cli = typer.Typer()
 
 
 def load_bool(name: str, default=False) -> bool:
     if not (v := os.getenv(name)):
         return default
     return v.lower() not in ("0", "false", "off", "no", "n")
 
@@ -114,15 +79,23 @@
 def capture_cmd_output(command: list[str] | str, **kw) -> str:
     if isinstance(command, str) and not kw.get("shell"):
         command = command.split()
     r = subprocess.run(command, capture_output=True, **kw)
     return r.stdout.strip().decode()
 
 
-def get_current_version(verbose=False) -> str:
+def get_current_version(
+    verbose=False,
+    is_poetry: bool | None = None,
+    package_name=Path(__file__).parent.name,
+) -> str:
+    if is_poetry is None:
+        is_poetry = Project.manage_by_poetry()
+    if not is_poetry:
+        return importlib_metadata.version(package_name)
     cmd = ["poetry", "version", "-s"]
     if verbose:
         echo(f"--> {' '.join(cmd)}")
     return capture_cmd_output(cmd)
 
 
 def _ensure_bool(value: bool | "OptionInfo") -> bool:
@@ -162,21 +135,33 @@
 class BumpUp(DryRun):
     class PartChoices(StrEnum):
         patch = "patch"
         minor = "minor"
         major = "major"
 
     def __init__(
-        self: Self, commit: bool, part: str, filename=TOML_FILE, dry=False
+        self: Self, commit: bool, part: str, filename: str | None = None, dry=False
     ) -> None:
         self.commit = commit
         self.part = part
+        if filename is None:
+            filename = self.parse_filename()
         self.filename = filename
         super().__init__(dry=dry)
 
+    @staticmethod
+    def parse_filename() -> str:
+        if not Project.manage_by_poetry():
+            # version = { source = "file", path = "fast_dev_cli/cli.py" }
+            for line in Project.load_toml_text().splitlines():
+                if not line.startswith("version = "):
+                    continue
+                return line.split('path = "', 1)[-1].split('"')[0]
+        return TOML_FILE
+
     def get_part(self, s: str) -> str:
         choices: dict[str, str] = {}
         for i, p in enumerate(self.PartChoices, 1):
             v = str(p)
             choices.update({str(i): v, v: v})
         try:
             return choices[s]
@@ -243,15 +228,15 @@
             if not a.startswith("-"):
                 part = a
                 break
     return BumpUp(commit, part, dry="--dry" in args).run()
 
 
 class EnvError(Exception):
-    """Raise this when the project is expected to be managed by poetry, but toml file not found."""
+    """Raise when expected to be managed by poetry, but toml file not found."""
 
 
 class Project:
     path_depth = 5
 
     @staticmethod
     def work_dir(name: str, parent: Path, depth: int) -> Path | None:
@@ -273,14 +258,31 @@
         raise EnvError(f"{name} not found! Make sure this is a poetry project.")
 
     @classmethod
     def load_toml_text(cls: Type[Self]) -> str:
         toml_file = cls.get_work_dir().resolve() / TOML_FILE  # to be optimize
         return toml_file.read_text("utf8")
 
+    @classmethod
+    def manage_by_poetry(cls: Type[Self]) -> bool:
+        return "[tool.poetry]" in cls.load_toml_text()
+
+    @classmethod
+    def get_manage_tool(cls: Type[Self]) -> Literal["poetry", "pdm", ""]:
+        try:
+            text = cls.load_toml_text()
+        except EnvError:
+            pass
+        else:
+            if "[tool.poetry]" in text:
+                return "poetry"
+            elif "[tool.pdm]" in text:
+                return "pdm"
+        return ""
+
     @staticmethod
     def python_exec_dir() -> Path:
         return Path(sys.executable).parent
 
     @classmethod
     def get_root_dir(cls: Type[Self], cwd: Path | None = None) -> Path:
         root = cwd or Path.cwd()
@@ -393,14 +395,18 @@
     @classmethod
     def get_args(
         cls: Type[Self], toml_text: str | None = None
     ) -> tuple[list[str], list[str], list[list[str]], str]:
         if toml_text is None:
             toml_text = cls.load_toml_text()
         main_title = "[tool.poetry.dependencies]"
+        if main_title not in toml_text:
+            raise EnvError(
+                f"{main_title} not found! Make sure this is a poetry project."
+            )
         text = toml_text.split(main_title)[-1]
         dev_flag = "--group dev"
         new_flag, old_flag = cls.DevFlag.new, cls.DevFlag.old
         if (dev_title := getattr(new_flag, "value", new_flag)) not in text:
             dev_title = getattr(old_flag, "value", old_flag)  # For poetry<=1.2
             dev_flag = "--dev"
         others: list[list[str]] = []
@@ -510,32 +516,36 @@
     @staticmethod
     def check_lint_tool_installed() -> bool:
         return check_call("ruff --version")
 
     @classmethod
     def to_cmd(cls: Type[Self], paths=".", check_only=False) -> str:
         cmd = ""
-        tools = ["ruff check --extend-select=I --fix", "ruff format", "mypy"]
+        tools = ["ruff format", "ruff check --extend-select=I --fix", "mypy"]
         if check_only:
-            tools[1] += " --check"
+            tools[0] += " --check"
         if check_only or load_bool("NO_FIX"):
-            tools[0] = tools[0].replace(" --fix", "")
+            tools[1] = tools[1].replace(" --fix", "")
         if load_bool("SKIP_MYPY"):
             # Sometimes mypy is too slow
             tools = tools[:-1]
         lint_them = " && ".join("{0}{%d} {1}" % i for i in range(2, len(tools) + 2))
-        prefix = "poetry run "
+        prefix = ""
+        should_run_by_tool = False
         if is_venv():
-            if cls.check_lint_tool_installed():
-                prefix = ""
-            else:
+            if not cls.check_lint_tool_installed():
+                should_run_by_tool = True
                 if check_call("python -c 'import fast_dev_cli'"):
-                    command = 'python -m pip install -U "fast_dev_cli[all]"'
-                    tip = "You may need to run the following command to install lint tools"
+                    command = 'python -m pip install -U "fast_dev_cli"'
+                    tip = "You may need to run following command to install lint tools"
                     secho(f"{tip}:\n\n  {command}\n", fg="yellow")
+        else:
+            should_run_by_tool = True
+        if should_run_by_tool:
+            prefix = Project.get_manage_tool() + " run "
         cmd += lint_them.format(prefix, paths, *tools)
         return cmd
 
     def gen(self: Self) -> str:
         paths = " ".join(self.args) if self.args else "."
         return self.to_cmd(paths, self.check_only)
 
@@ -624,15 +634,16 @@
         cmd = f"sh {test_script.relative_to(root)}"
         if cwd != root:
             cmd = f"cd {root} && " + cmd
     else:
         cmd = 'coverage run -m pytest -s && coverage report --omit="tests/*" -m'
         if not is_venv() or not check_call("coverage --version"):
             sep = " && "
-            cmd = sep.join("poetry run " + i for i in cmd.split(sep))
+            tool = Project.get_manage_tool()
+            cmd = sep.join(f"{tool} run " + i for i in cmd.split(sep))
     exit_if_run_failed(cmd, dry=dry)
 
 
 @cli.command(name="test")
 def coverage_test(
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
     ignore_script: bool = Option(False, "--ignore-script", "-i"),
```


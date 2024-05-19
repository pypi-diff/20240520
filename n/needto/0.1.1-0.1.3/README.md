# Comparing `tmp/needto-0.1.1.tar.gz` & `tmp/needto-0.1.3.tar.gz`

## Comparing `needto-0.1.1.tar` & `needto-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.1/needto/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.1/needto/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.1/needto/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.1/needto/src/__init__.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 needto-0.1.1/needto/src/ai_client.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 needto-0.1.1/needto/src/cli.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.1/needto/src/config.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 needto-0.1.1/needto/src/utils.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.1/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 needto-0.1.1/README.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 needto-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.3/needto/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.3/needto/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.3/needto/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/ai_client.py
+-rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/cli.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/config.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/utils.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.3/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.3/PKG-INFO
```

### Comparing `needto-0.1.1/needto/src/ai_client.py` & `needto-0.1.3/needto/src/ai_client.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.1/needto/src/cli.py` & `needto-0.1.3/needto/src/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                     )
                 with open(selected_file_name, "w") as f:
                     f.write(file_content)
                 console.print(f"'{selected_file_name}' saved.", style="bold green")
                 break
 
         console.print("Leave blank to end conversation", style="blue bold")
-        if user_prompt := ("> ",):
+        if user_prompt := input("> "):
             print()
             parsed_answer = ai_client.ask(user_prompt)
         else:
             break
 
 
 @app.command(help=f"Open editor for '{config_manager.config_path}'.")
```

### Comparing `needto-0.1.1/needto/src/config.py` & `needto-0.1.3/needto/src/config.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.1/needto/src/utils.py` & `needto-0.1.3/needto/src/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 import typing
+import functools
 import click
 import sys
 from simple_term_menu import TerminalMenu
 import rich.console
 import rich.prompt
 
 EDITOR_TEMPLATE = """{command}
 
 # save this file to confirm the command or quit to skip it.
 # after save, you will {confirm_prompt} this command.
 """
 
 
+@functools.cache
+def stdin_is_atty():
+    return sys.stdin.isatty()
+
+
+@functools.cache
+def get_tty_file():
+    return open("/dev/tty")
+
+
 def prompt_menu(
     items: list[str],
     *,
     ask_for_edit=False,
     no_op_value="-- non of this options, want to explain more --",
     confirm_prompt="",
     preview_command: None | str | typing.Callable[[str], str] = None,
@@ -26,15 +37,15 @@
         preview_command=preview_command,
     ).show()
     selected_item: str = items_to_prompt[menu_entry_index]
 
     if selected_item == no_op_value:
         return
 
-    if ask_for_edit and sys.stdin.isatty():
+    if ask_for_edit and stdin_is_atty():
         if edited_text := click.edit(
             text=EDITOR_TEMPLATE.format(
                 command=selected_item, confirm_prompt=confirm_prompt.lower()
             )
         ):
             lines = [
                 line
@@ -42,16 +53,16 @@
                 if line.strip() and not line.strip().startswith("#")
             ]
             if len(lines) == 1:
                 selected_item = lines[0].strip()
         else:
             return
 
-    if not sys.stdin.isatty():
-        sys.stdin = open("/dev/tty")
+    if not stdin_is_atty():
+        sys.stdin = get_tty_file()
 
         if confirm_prompt and not rich.prompt.Confirm.ask(
             f"{confirm_prompt} '{selected_item}'", default=False
         ):
             return
 
     return selected_item
```

### Comparing `needto-0.1.1/.gitignore` & `needto-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `needto-0.1.1/LICENSE.txt` & `needto-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `needto-0.1.1/README.md` & `needto-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Needto
 
 [![PyPI - Version](https://img.shields.io/pypi/v/needto.svg)](https://pypi.org/project/needto)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/needto.svg)](https://pypi.org/project/needto)
 
------
 
 Needto have an AI assistant in your command line?
 
 `needto` is an AI-powered assistant for the command line, designed to help you with various tasks such as **finding and running commands**, **answering questions by analyzing command outputs**, and **writing code snippets**. It suggests solutions and makes it easy to apply them in your environment. With `needto`, you can select and run recommended commands safely.
 
 ## Installation
```

### Comparing `needto-0.1.1/pyproject.toml` & `needto-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `needto-0.1.1/PKG-INFO` & `needto-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: needto
-Version: 0.1.1
+Version: 0.1.3
 Summary: Ask AI for help you in your terminal.
 Project-URL: Documentation, https://github.com/danialkeimasi/needto#readme
 Project-URL: Issues, https://github.com/danialkeimasi/needto/issues
 Project-URL: Source, https://github.com/danialkeimasi/needto
 Author-email: Danial Keimasi <danialkeimasi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -25,15 +25,14 @@
 Description-Content-Type: text/markdown
 
 # Needto
 
 [![PyPI - Version](https://img.shields.io/pypi/v/needto.svg)](https://pypi.org/project/needto)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/needto.svg)](https://pypi.org/project/needto)
 
------
 
 Needto have an AI assistant in your command line?
 
 `needto` is an AI-powered assistant for the command line, designed to help you with various tasks such as **finding and running commands**, **answering questions by analyzing command outputs**, and **writing code snippets**. It suggests solutions and makes it easy to apply them in your environment. With `needto`, you can select and run recommended commands safely.
 
 ## Installation
```


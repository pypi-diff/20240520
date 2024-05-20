# Comparing `tmp/needto-0.1.3.tar.gz` & `tmp/needto-0.1.4.tar.gz`

## Comparing `needto-0.1.3.tar` & `needto-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.3/needto/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.3/needto/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.3/needto/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/__init__.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/ai_client.py
--rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/cli.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/config.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 needto-0.1.3/needto/src/utils.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.3/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.3/README.md
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 needto-0.1.4/needto/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 needto-0.1.4/needto/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 needto-0.1.4/needto/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/__init__.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/ai_client.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/cli.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/config.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 needto-0.1.4/needto/src/utils.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 needto-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 needto-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 needto-0.1.4/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 needto-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 needto-0.1.4/PKG-INFO
```

### Comparing `needto-0.1.3/needto/src/ai_client.py` & `needto-0.1.4/needto/src/ai_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 import sys
 import rich.console
 import rich.prompt
 from .config import config_manager
 
 import rich.console
 import json
@@ -53,15 +54,29 @@
         console = rich.console.Console()
         if print_prompt:
             print()
             console.print(prompt)
             print()
 
         self.messages.append({"role": "user", "content": prompt})
-        chat_completion = self.client.chat.completions.create(
-            messages=self.messages,
-            model=config_manager.values.model_name,
-            response_format={"type": "json_object"},
-        )
-        answer = chat_completion.choices[0].message.content
-        self.messages.append({"role": "system", "content": answer})
-        return json.loads(answer)
+
+        retry_count = 3
+        for _ in range(retry_count):
+            chat_completion = self.client.chat.completions.create(
+                messages=self.messages,
+                model=config_manager.values.model_name,
+                # response_format={"type": "json_object"},
+            )
+            answer = chat_completion.choices[0].message.content
+
+            try:
+                parsed_answer = json.loads(answer)
+            except json.JSONDecodeError:
+                self.messages.append(
+                    {
+                        "role": "user",
+                        "content": "Last response was not JSON. Always write JSON.",
+                    }
+                )
+            else:
+                self.messages.append({"role": "system", "content": answer})
+                return parsed_answer
```

### Comparing `needto-0.1.3/needto/src/cli.py` & `needto-0.1.4/needto/src/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import os
 import click
 import sys
 import typer
 import rich.console
 import rich.prompt
 import subprocess
-from rich.markdown import Markdown
 
 from .config import config_manager
 from .ai_client import AIClient
 from .utils import prompt_menu_and_print
 
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command(help="Find and run a command.")
 def do(prompt_list: list[str]):
     prompt = " ".join(prompt_list)
     console = rich.console.Console()
     system_prompt = """
     You are a CLI code generator. User will search for a command, you respond with a list of CLI commands.
-    Always answer in json in all your responses with these keys:
+    Don't write markdown.
+    Response should always be JSON stars with "{" and ends with "}" with these keys:
     "description" (str), "warning" (str only if necessary), "commands" (list of str).
+    Don't explain at begin or end of JSON.
     """
     console = rich.console.Console()
     ai_client = AIClient(system_prompt=system_prompt)
     parsed_answer = ai_client.ask(prompt)
 
     while True:
         console.print(parsed_answer["description"], style="bold blue")
@@ -58,22 +59,24 @@
 @app.command(help="Ask question, Send output of commands to AI to get help.")
 def ask(prompt_list: list[str]):
     prompt = " ".join(prompt_list)
     system_prompt = """
     You are a AI assistant. User will ask you something and you will help him find their answer.
     You can ask user to run commands and send the output of commands to you, to help you answer their questions.
     Don't recommend commands that can change the system state.
-    Always answer in json in all your responses with these keys:
-    "help" (markdown str), "commands_to_explore" (list of str only if necessary)
+    Don't write markdown.
+    Response should always be JSON stars with "{" and ends with "}" with these keys:
+    "help" (text), "commands_to_explore" (list of str only if necessary)
+    Don't explain at begin or end of JSON.
     """
     console = rich.console.Console()
     ai_client = AIClient(system_prompt=system_prompt)
     parsed_answer = ai_client.ask(prompt)
     while True:
-        console.print(Markdown(parsed_answer["help"]))
+        console.print(parsed_answer["help"])
         print()
 
         if commands := parsed_answer.get("commands_to_explore"):
             if command := prompt_menu_and_print(
                 commands, confirm_prompt="Run and send output of", ask_for_edit=True
             ):
                 try:
@@ -108,22 +111,24 @@
 
 @app.command(help="Write code.")
 def write(prompt_list: list[str]):
     prompt = " ".join(prompt_list)
     system_prompt = """
     You are a AI assistant. User will ask you to write a code.
     You can ask user to clarify what they need and then run the code.
-    Always answer in json in all your responses with these keys:
-    "help" (markdown str), "files_to_save": (object with name to content)
+    Don't write markdown.
+    Response should always be JSON stars with "{" and ends with "}" with these keys:
+    "help" (text), "files_to_save": (object with name to content)
+    Don't explain at begin or end of JSON.
     """
     console = rich.console.Console()
     ai_client = AIClient(system_prompt=system_prompt)
     parsed_answer = ai_client.ask(prompt)
     while True:
-        console.print(Markdown(parsed_answer["help"]))
+        console.print(parsed_answer["help"])
         files_to_save = parsed_answer.get("files_to_save", {})
         print()
         if files_to_save:
             if selected_file_name := prompt_menu_and_print(
                 list(files_to_save.keys()),
                 preview_command=lambda file_name: files_to_save.get(file_name, ""),
             ):
```

### Comparing `needto-0.1.3/needto/src/config.py` & `needto-0.1.4/needto/src/config.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.3/needto/src/utils.py` & `needto-0.1.4/needto/src/utils.py`

 * *Files identical despite different names*

### Comparing `needto-0.1.3/.gitignore` & `needto-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `needto-0.1.3/LICENSE.txt` & `needto-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `needto-0.1.3/README.md` & `needto-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `needto-0.1.3/pyproject.toml` & `needto-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `needto-0.1.3/PKG-INFO` & `needto-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: needto
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ask AI for help you in your terminal.
 Project-URL: Documentation, https://github.com/danialkeimasi/needto#readme
 Project-URL: Issues, https://github.com/danialkeimasi/needto/issues
 Project-URL: Source, https://github.com/danialkeimasi/needto
 Author-email: Danial Keimasi <danialkeimasi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```


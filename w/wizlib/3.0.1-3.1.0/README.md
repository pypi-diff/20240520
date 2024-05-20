# Comparing `tmp/wizlib-3.0.1.tar.gz` & `tmp/wizlib-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-3.0.1.tar", max compression
+gzip compressed data, was "wizlib-3.1.0.tar", max compression
```

## Comparing `wizlib-3.0.1.tar` & `wizlib-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1094 2024-05-19 00:07:31.324488 wizlib-3.0.1/README.md
--rw-r--r--   0        0        0      698 2024-05-19 00:07:42.820476 wizlib-3.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 00:07:31.411488 wizlib-3.0.1/wizlib/__init__.py
--rw-r--r--   0        0        0     3263 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/app.py
--rw-r--r--   0        0        0     4506 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/class_family.py
--rw-r--r--   0        0        0     1747 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/command.py
--rw-r--r--   0        0        0     2588 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/config_handler.py
--rw-r--r--   0        0        0       46 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/error.py
--rw-r--r--   0        0        0      446 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/handler.py
--rw-r--r--   0        0        0     1505 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/parser.py
--rw-r--r--   0        0        0     1754 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/rlinput.py
--rw-r--r--   0        0        0      663 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/stream_handler.py
--rw-r--r--   0        0        0      272 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/super_wrapper.py
--rw-r--r--   0        0        0     4241 2024-05-19 00:07:31.361488 wizlib-3.0.1/wizlib/ui/__init__.py
--rw-r--r--   0        0        0      943 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/ui/shell/__init__.py
--rw-r--r--   0        0        0     7419 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/ui/shell/line_editor.py
--rw-r--r--   0        0        0     2064 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/ui/shell_ui.py
--rw-r--r--   0        0        0      634 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/ui_handler.py
--rw-r--r--   0        0        0      156 2024-05-19 00:07:31.362488 wizlib-3.0.1/wizlib/util.py
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 wizlib-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-20 16:26:57.317283 wizlib-3.1.0/README.md
+-rw-r--r--   0        0        0      698 2024-05-20 16:27:09.054272 wizlib-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 16:26:57.410283 wizlib-3.1.0/wizlib/__init__.py
+-rw-r--r--   0        0        0     3350 2024-05-20 16:26:57.355283 wizlib-3.1.0/wizlib/app.py
+-rw-r--r--   0        0        0     4506 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/class_family.py
+-rw-r--r--   0        0        0     1708 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/command.py
+-rw-r--r--   0        0        0     2588 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/config_handler.py
+-rw-r--r--   0        0        0       46 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/error.py
+-rw-r--r--   0        0        0      446 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/handler.py
+-rw-r--r--   0        0        0     1505 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/parser.py
+-rw-r--r--   0        0        0      663 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/stream_handler.py
+-rw-r--r--   0        0        0      272 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/super_wrapper.py
+-rw-r--r--   0        0        0     4241 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/ui/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/ui/shell/__init__.py
+-rw-r--r--   0        0        0     7419 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/ui/shell/line_editor.py
+-rw-r--r--   0        0        0     2029 2024-05-20 16:26:57.356283 wizlib-3.1.0/wizlib/ui/shell_ui.py
+-rw-r--r--   0        0        0      634 2024-05-20 16:26:57.357283 wizlib-3.1.0/wizlib/ui_handler.py
+-rw-r--r--   0        0        0      156 2024-05-20 16:26:57.357283 wizlib-3.1.0/wizlib/util.py
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 wizlib-3.1.0/PKG-INFO
```

### Comparing `wizlib-3.0.1/README.md` & `wizlib-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/pyproject.toml` & `wizlib-3.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wizlib"
-version = "3.0.1"
+version = "3.1.0"
 description = "Framework for flexible and powerful command-line applications"
 authors = ["Steampunk Wizard <wizlib@steampunkwizard.ca>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `wizlib-3.0.1/wizlib/class_family.py` & `wizlib-3.1.0/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/wizlib/command.py` & `wizlib-3.1.0/wizlib/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     pass
 
 
 class WizCommand(ClassFamily, SuperWrapper):
     """Define all the args you want, but stdin always works."""
 
     status = ''
-    handlers = []  # TODO: Move to app
 
     @classmethod
     def add_args(self, parser):
         """Add arguments to the command's parser - override this.
         Add global arguments in the base class. Not wrapped."""
         pass
```

### Comparing `wizlib-3.0.1/wizlib/config_handler.py` & `wizlib-3.1.0/wizlib/config_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/wizlib/parser.py` & `wizlib-3.1.0/wizlib/parser.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/wizlib/stream_handler.py` & `wizlib-3.1.0/wizlib/stream_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/wizlib/ui/__init__.py` & `wizlib-3.1.0/wizlib/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/wizlib/ui/shell/__init__.py` & `wizlib-3.1.0/wizlib/ui/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/wizlib/ui/shell/line_editor.py` & `wizlib-3.1.0/wizlib/ui/shell/line_editor.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/wizlib/ui/shell_ui.py` & `wizlib-3.1.0/wizlib/ui/shell_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from enum import StrEnum
 import sys
 
 from readchar import readkey
 
-from wizlib.rlinput import rlinput
 from wizlib.ui import UI, Chooser, Emphasis
 from wizlib.ui.shell.line_editor import ShellLineEditor
 from wizlib.ui.shell import S
 
 INTERACTIVE = sys.stdin.isatty()
 
 COLOR = {
```

### Comparing `wizlib-3.0.1/wizlib/ui_handler.py` & `wizlib-3.1.0/wizlib/ui_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-3.0.1/PKG-INFO` & `wizlib-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 3.0.1
+Version: 3.1.0
 Summary: Framework for flexible and powerful command-line applications
 License: MIT
 Author: Steampunk Wizard
 Author-email: wizlib@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/markdown_exec-1.8.1.tar.gz` & `tmp/markdown_exec-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_exec-1.8.1.tar", last modified: Mon Apr 15 16:53:26 2024, max compression
+gzip compressed data, was "markdown_exec-1.8.2.tar", last modified: Mon May 20 18:15:57 2024, max compression
```

## Comparing `markdown_exec-1.8.1.tar` & `markdown_exec-1.8.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      754 2024-03-20 15:30:02.179261 markdown_exec-1.8.1/LICENSE
--rw-r--r--   0        0        0     3367 2024-03-20 15:30:04.979225 markdown_exec-1.8.1/README.md
--rw-r--r--   0        0        0     1844 2024-04-15 16:53:26.659226 markdown_exec-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     4366 2024-03-20 15:30:04.982558 markdown_exec-1.8.1/src/markdown_exec/__init__.py
--rw-r--r--   0        0        0     8090 2024-04-15 16:45:33.050727 markdown_exec-1.8.1/src/markdown_exec/ansi.css
--rw-r--r--   0        0        0     2840 2024-03-20 15:30:02.289260 markdown_exec-1.8.1/src/markdown_exec/debug.py
--rw-r--r--   0        0        0       51 2023-11-05 16:57:00.630087 markdown_exec-1.8.1/src/markdown_exec/formatters/__init__.py
--rw-r--r--   0        0        0     4761 2023-11-05 16:57:00.653419 markdown_exec-1.8.1/src/markdown_exec/formatters/base.py
--rw-r--r--   0        0        0      886 2023-11-05 16:57:00.653419 markdown_exec-1.8.1/src/markdown_exec/formatters/bash.py
--rw-r--r--   0        0        0      815 2023-11-05 16:57:00.670086 markdown_exec-1.8.1/src/markdown_exec/formatters/console.py
--rw-r--r--   0        0        0      276 2023-11-05 16:57:00.683419 markdown_exec-1.8.1/src/markdown_exec/formatters/markdown.py
--rw-r--r--   0        0        0      854 2023-11-05 16:57:00.706752 markdown_exec-1.8.1/src/markdown_exec/formatters/pycon.py
--rw-r--r--   0        0        0     2898 2024-01-05 17:48:17.990589 markdown_exec-1.8.1/src/markdown_exec/formatters/pyodide.py
--rw-r--r--   0        0        0     2406 2023-11-05 16:57:00.726752 markdown_exec-1.8.1/src/markdown_exec/formatters/python.py
--rw-r--r--   0        0        0      876 2023-11-05 16:57:00.726752 markdown_exec-1.8.1/src/markdown_exec/formatters/sh.py
--rw-r--r--   0        0        0     2046 2023-11-05 16:57:00.746751 markdown_exec-1.8.1/src/markdown_exec/formatters/tree.py
--rw-r--r--   0        0        0     2109 2023-11-05 16:57:00.760085 markdown_exec-1.8.1/src/markdown_exec/logger.py
--rw-r--r--   0        0        0     4701 2024-01-05 18:36:32.567651 markdown_exec-1.8.1/src/markdown_exec/mkdocs_plugin.py
--rw-r--r--   0        0        0     4291 2024-01-05 17:35:28.675090 markdown_exec-1.8.1/src/markdown_exec/processors.py
--rw-r--r--   0        0        0        0 2024-03-20 15:30:02.292593 markdown_exec-1.8.1/src/markdown_exec/py.typed
--rw-r--r--   0        0        0      849 2024-01-05 17:48:17.990589 markdown_exec-1.8.1/src/markdown_exec/pyodide.css
--rw-r--r--   0        0        0     3845 2024-01-05 17:48:17.993923 markdown_exec-1.8.1/src/markdown_exec/pyodide.js
--rw-r--r--   0        0        0     9459 2024-01-05 18:00:40.526407 markdown_exec-1.8.1/src/markdown_exec/rendering.py
--rw-r--r--   0        0        0      166 2024-03-20 15:30:02.299260 markdown_exec-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0      635 2024-03-20 15:30:04.982558 markdown_exec-1.8.1/tests/conftest.py
--rw-r--r--   0        0        0     1443 2023-11-05 16:57:00.873417 markdown_exec-1.8.1/tests/test_base_formatter.py
--rw-r--r--   0        0        0     2080 2023-11-05 16:57:00.893416 markdown_exec-1.8.1/tests/test_converter.py
--rw-r--r--   0        0        0     4337 2023-11-05 16:57:00.916749 markdown_exec-1.8.1/tests/test_python.py
--rw-r--r--   0        0        0     2027 2023-11-05 16:57:00.936749 markdown_exec-1.8.1/tests/test_shell.py
--rw-r--r--   0        0        0     2335 2023-11-05 16:57:00.983415 markdown_exec-1.8.1/tests/test_toc.py
--rw-r--r--   0        0        0      488 2023-11-05 16:57:00.983415 markdown_exec-1.8.1/tests/test_tree.py
--rw-r--r--   0        0        0      995 2023-11-05 16:57:01.013414 markdown_exec-1.8.1/tests/test_validator.py
--rw-r--r--   0        0        0     4954 1970-01-01 00:00:00.000000 markdown_exec-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-03-20 15:30:02.179261 markdown_exec-1.8.2/LICENSE
+-rw-r--r--   0        0        0     3367 2024-03-20 15:30:04.979225 markdown_exec-1.8.2/README.md
+-rw-r--r--   0        0        0     1844 2024-05-20 18:15:57.868931 markdown_exec-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4366 2024-03-20 15:30:04.982558 markdown_exec-1.8.2/src/markdown_exec/__init__.py
+-rw-r--r--   0        0        0     8090 2024-04-15 16:45:33.050727 markdown_exec-1.8.2/src/markdown_exec/ansi.css
+-rw-r--r--   0        0        0     2840 2024-03-20 15:30:02.289260 markdown_exec-1.8.2/src/markdown_exec/debug.py
+-rw-r--r--   0        0        0       51 2023-11-05 16:57:00.630087 markdown_exec-1.8.2/src/markdown_exec/formatters/__init__.py
+-rw-r--r--   0        0        0     4761 2023-11-05 16:57:00.653419 markdown_exec-1.8.2/src/markdown_exec/formatters/base.py
+-rw-r--r--   0        0        0      886 2023-11-05 16:57:00.653419 markdown_exec-1.8.2/src/markdown_exec/formatters/bash.py
+-rw-r--r--   0        0        0      815 2023-11-05 16:57:00.670086 markdown_exec-1.8.2/src/markdown_exec/formatters/console.py
+-rw-r--r--   0        0        0      276 2023-11-05 16:57:00.683419 markdown_exec-1.8.2/src/markdown_exec/formatters/markdown.py
+-rw-r--r--   0        0        0      854 2023-11-05 16:57:00.706752 markdown_exec-1.8.2/src/markdown_exec/formatters/pycon.py
+-rw-r--r--   0        0        0     2898 2024-01-05 17:48:17.990589 markdown_exec-1.8.2/src/markdown_exec/formatters/pyodide.py
+-rw-r--r--   0        0        0     3029 2024-05-20 18:13:12.803878 markdown_exec-1.8.2/src/markdown_exec/formatters/python.py
+-rw-r--r--   0        0        0      876 2023-11-05 16:57:00.726752 markdown_exec-1.8.2/src/markdown_exec/formatters/sh.py
+-rw-r--r--   0        0        0     2046 2023-11-05 16:57:00.746751 markdown_exec-1.8.2/src/markdown_exec/formatters/tree.py
+-rw-r--r--   0        0        0     2109 2023-11-05 16:57:00.760085 markdown_exec-1.8.2/src/markdown_exec/logger.py
+-rw-r--r--   0        0        0     4701 2024-01-05 18:36:32.567651 markdown_exec-1.8.2/src/markdown_exec/mkdocs_plugin.py
+-rw-r--r--   0        0        0     4291 2024-01-05 17:35:28.675090 markdown_exec-1.8.2/src/markdown_exec/processors.py
+-rw-r--r--   0        0        0        0 2024-03-20 15:30:02.292593 markdown_exec-1.8.2/src/markdown_exec/py.typed
+-rw-r--r--   0        0        0      849 2024-01-05 17:48:17.990589 markdown_exec-1.8.2/src/markdown_exec/pyodide.css
+-rw-r--r--   0        0        0     3845 2024-01-05 17:48:17.993923 markdown_exec-1.8.2/src/markdown_exec/pyodide.js
+-rw-r--r--   0        0        0     9459 2024-01-05 18:00:40.526407 markdown_exec-1.8.2/src/markdown_exec/rendering.py
+-rw-r--r--   0        0        0      166 2024-03-20 15:30:02.299260 markdown_exec-1.8.2/tests/__init__.py
+-rw-r--r--   0        0        0      635 2024-03-20 15:30:04.982558 markdown_exec-1.8.2/tests/conftest.py
+-rw-r--r--   0        0        0     1443 2023-11-05 16:57:00.873417 markdown_exec-1.8.2/tests/test_base_formatter.py
+-rw-r--r--   0        0        0     2080 2023-11-05 16:57:00.893416 markdown_exec-1.8.2/tests/test_converter.py
+-rw-r--r--   0        0        0     4787 2024-05-20 18:02:38.502897 markdown_exec-1.8.2/tests/test_python.py
+-rw-r--r--   0        0        0     2027 2023-11-05 16:57:00.936749 markdown_exec-1.8.2/tests/test_shell.py
+-rw-r--r--   0        0        0     2335 2023-11-05 16:57:00.983415 markdown_exec-1.8.2/tests/test_toc.py
+-rw-r--r--   0        0        0      488 2023-11-05 16:57:00.983415 markdown_exec-1.8.2/tests/test_tree.py
+-rw-r--r--   0        0        0      995 2023-11-05 16:57:01.013414 markdown_exec-1.8.2/tests/test_validator.py
+-rw-r--r--   0        0        0     4954 1970-01-01 00:00:00.000000 markdown_exec-1.8.2/PKG-INFO
```

### Comparing `markdown_exec-1.8.1/LICENSE` & `markdown_exec-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/README.md` & `markdown_exec-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/pyproject.toml` & `markdown_exec-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "pymdown-extensions>=9",
 ]
-version = "1.8.1"
+version = "1.8.2"
 
 [project.license]
 text = "ISC"
 
 [project.optional-dependencies]
 ansi = [
     "pygments-ansi-color",
```

### Comparing `markdown_exec-1.8.1/src/markdown_exec/__init__.py` & `markdown_exec-1.8.2/src/markdown_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/ansi.css` & `markdown_exec-1.8.2/src/markdown_exec/ansi.css`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/debug.py` & `markdown_exec-1.8.2/src/markdown_exec/debug.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/formatters/base.py` & `markdown_exec-1.8.2/src/markdown_exec/formatters/base.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/formatters/bash.py` & `markdown_exec-1.8.2/src/markdown_exec/formatters/bash.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/formatters/console.py` & `markdown_exec-1.8.2/src/markdown_exec/formatters/console.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/formatters/pycon.py` & `markdown_exec-1.8.2/src/markdown_exec/formatters/pycon.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/formatters/pyodide.py` & `markdown_exec-1.8.2/src/markdown_exec/formatters/pyodide.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/formatters/python.py` & `markdown_exec-1.8.2/src/markdown_exec/formatters/python.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Formatter for executing Python code."""
 
 from __future__ import annotations
 
+import re
+import sys
 import traceback
 from collections import defaultdict
 from functools import partial
 from io import StringIO
+from types import ModuleType
 from typing import Any
 
 from markdown_exec.formatters.base import ExecutionError, base_format
 from markdown_exec.rendering import code_block
 
 _sessions_globals: dict[str, dict] = defaultdict(dict)
 _sessions_counter: dict[str | None, int] = defaultdict(int)
@@ -47,14 +50,23 @@
     **extra: str,
 ) -> str:
     title = extra.get("title", None)
     code_block_id = _code_block_id(id, session, title)
     _code_blocks[code_block_id] = code.split("\n")
     exec_globals = _sessions_globals[session] if session else {}
 
+    # Other libraries expect functions to have a valid `__module__` attribute.
+    # To achieve this, we need to add a `__name__` attribute to the globals.
+    # We compute the name from the code block ID, replacing invalid characters with `_`.
+    # We also create a module object with the same name and add it to `sys.modules`,
+    # because that's what yet other libraries expect (`dataclasses` for example).
+    module_name = re.sub(r"[^a-zA-Z\d]+", "_", code_block_id)
+    exec_globals["__name__"] = module_name
+    sys.modules[module_name] = ModuleType(module_name)
+
     buffer = StringIO()
     exec_globals["print"] = partial(_buffer_print, buffer)
 
     try:
         compiled = compile(code, filename=code_block_id, mode="exec")
         exec(compiled, exec_globals)  # noqa: S102
     except Exception as error:  # noqa: BLE001
```

### Comparing `markdown_exec-1.8.1/src/markdown_exec/formatters/sh.py` & `markdown_exec-1.8.2/src/markdown_exec/formatters/sh.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/formatters/tree.py` & `markdown_exec-1.8.2/src/markdown_exec/formatters/tree.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/logger.py` & `markdown_exec-1.8.2/src/markdown_exec/logger.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/mkdocs_plugin.py` & `markdown_exec-1.8.2/src/markdown_exec/mkdocs_plugin.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/processors.py` & `markdown_exec-1.8.2/src/markdown_exec/processors.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/pyodide.css` & `markdown_exec-1.8.2/src/markdown_exec/pyodide.css`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/pyodide.js` & `markdown_exec-1.8.2/src/markdown_exec/pyodide.js`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/src/markdown_exec/rendering.py` & `markdown_exec-1.8.2/src/markdown_exec/rendering.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/tests/conftest.py` & `markdown_exec-1.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/tests/test_base_formatter.py` & `markdown_exec-1.8.2/tests/test_base_formatter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/tests/test_converter.py` & `markdown_exec-1.8.2/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/tests/test_python.py` & `markdown_exec-1.8.2/tests/test_python.py`

 * *Files 7% similar despite different names*

```diff
@@ -178,7 +178,28 @@
             ko
             ```
             """,
         ),
     )
     assert "ok" in html
     assert "ko" not in html
+
+
+def test_functions_have_a_module_attribute(md: Markdown) -> None:
+    """Assert functions have a `__module__` attribute.
+
+    Parameters:
+        md: A Markdown instance (fixture).
+    """
+    html = md.convert(
+        dedent(
+            """
+            ```python exec="1"
+            def func():
+                pass
+
+            print(f"`{func.__module__}`")
+            ```
+            """,
+        ),
+    )
+    assert "_code_block_n" in html
```

### Comparing `markdown_exec-1.8.1/tests/test_shell.py` & `markdown_exec-1.8.2/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/tests/test_toc.py` & `markdown_exec-1.8.2/tests/test_toc.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/tests/test_validator.py` & `markdown_exec-1.8.2/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.1/PKG-INFO` & `markdown_exec-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-exec
-Version: 1.8.1
+Version: 1.8.2
 Summary: Utilities to execute code blocks in Markdown files.
 Keywords: markdown,python,exec,shell,bash,mkdocs
 Author-Email: =?utf-8?q?Timoth=C3=A9e_Mazzucotelli?= <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```


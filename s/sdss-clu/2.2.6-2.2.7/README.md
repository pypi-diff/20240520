# Comparing `tmp/sdss_clu-2.2.6.tar.gz` & `tmp/sdss_clu-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_clu-2.2.6.tar", max compression
+gzip compressed data, was "sdss_clu-2.2.7.tar", max compression
```

## Comparing `sdss_clu-2.2.6.tar` & `sdss_clu-2.2.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1504 2024-03-26 19:03:07.836795 sdss_clu-2.2.6/LICENSE.md
--rw-r--r--   0        0        0     5038 2024-03-26 19:03:07.836795 sdss_clu-2.2.6/README.rst
--rw-r--r--   0        0        0     2957 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/pyproject.toml
--rw-r--r--   0        0        0      889 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/__init__.py
--rwxr-xr-x   0        0        0     9086 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/__main__.py
--rw-r--r--   0        0        0    16644 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/actor.py
--rw-r--r--   0        0        0    21380 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/base.py
--rw-r--r--   0        0        0    16877 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/client.py
--rw-r--r--   0        0        0    20416 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/command.py
--rw-r--r--   0        0        0     4135 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/device.py
--rw-r--r--   0        0        0     1347 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/exceptions.py
--rw-r--r--   0        0        0       41 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/__init__.py
--rw-r--r--   0        0        0    18808 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/actor.py
--rw-r--r--   0        0        0    13581 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/tron.py
--rw-r--r--   0        0        0        0 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/__init__.py
--rw-r--r--   0        0        0    15014 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/html.py
--rw-r--r--   0        0        0    17888 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/keys.py
--rw-r--r--   0        0        0    17508 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/messages.py
--rw-r--r--   0        0        0     9489 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/parser.py
--rwxr-xr-x   0        0        0      104 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/ply/__init__.py
--rwxr-xr-x   0        0        0    38405 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/ply/cpp.py
--rwxr-xr-x   0        0        0     2877 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/ply/ctokens.py
--rwxr-xr-x   0        0        0    45219 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/ply/lex.py
--rwxr-xr-x   0        0        0   140885 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/ply/yacc.py
--rwxr-xr-x   0        0        0     2314 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/ply/ygen.py
--rw-r--r--   0        0        0     5487 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/pvt.py
--rw-r--r--   0        0        0    19685 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/legacy/types/types.py
--rw-r--r--   0        0        0    11924 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/model.py
--rw-r--r--   0        0        0      309 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/parsers/__init__.py
--rw-r--r--   0        0        0    20583 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/parsers/click.py
--rw-r--r--   0        0        0     2685 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/parsers/json.py
--rw-r--r--   0        0        0    19724 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/protocol.py
--rw-r--r--   0        0        0     2805 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/store.py
--rw-r--r--   0        0        0     7820 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/testing.py
--rw-r--r--   0        0        0    16712 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/tools.py
--rw-r--r--   0        0        0     3648 2024-03-26 19:03:07.840795 sdss_clu-2.2.6/python/clu/websocket.py
--rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 sdss_clu-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-20 19:03:48.527713 sdss_clu-2.2.7/LICENSE.md
+-rw-r--r--   0        0        0     5038 2024-05-20 19:03:48.527713 sdss_clu-2.2.7/README.rst
+-rw-r--r--   0        0        0     3025 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/pyproject.toml
+-rw-r--r--   0        0        0      889 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/__init__.py
+-rwxr-xr-x   0        0        0     9086 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/__main__.py
+-rw-r--r--   0        0        0    16644 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/actor.py
+-rw-r--r--   0        0        0    21380 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/base.py
+-rw-r--r--   0        0        0    16877 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/client.py
+-rw-r--r--   0        0        0    20416 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/command.py
+-rw-r--r--   0        0        0     4135 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/device.py
+-rw-r--r--   0        0        0     1347 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/exceptions.py
+-rw-r--r--   0        0        0       41 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/__init__.py
+-rw-r--r--   0        0        0    18808 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/actor.py
+-rw-r--r--   0        0        0    13581 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/tron.py
+-rw-r--r--   0        0        0        0 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/__init__.py
+-rw-r--r--   0        0        0    15014 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/html.py
+-rw-r--r--   0        0        0    17888 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/keys.py
+-rw-r--r--   0        0        0    17508 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/messages.py
+-rw-r--r--   0        0        0     9489 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/parser.py
+-rwxr-xr-x   0        0        0      104 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/ply/__init__.py
+-rwxr-xr-x   0        0        0    38405 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/ply/cpp.py
+-rwxr-xr-x   0        0        0     2877 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/ply/ctokens.py
+-rwxr-xr-x   0        0        0    45219 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/ply/lex.py
+-rwxr-xr-x   0        0        0   140885 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/ply/yacc.py
+-rwxr-xr-x   0        0        0     2314 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/ply/ygen.py
+-rw-r--r--   0        0        0     5487 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/pvt.py
+-rw-r--r--   0        0        0    19685 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/legacy/types/types.py
+-rw-r--r--   0        0        0    11924 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/model.py
+-rw-r--r--   0        0        0      309 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/parsers/__init__.py
+-rw-r--r--   0        0        0    20640 2024-05-20 19:03:48.531714 sdss_clu-2.2.7/python/clu/parsers/click.py
+-rw-r--r--   0        0        0     2685 2024-05-20 19:03:48.535714 sdss_clu-2.2.7/python/clu/parsers/json.py
+-rw-r--r--   0        0        0    19724 2024-05-20 19:03:48.535714 sdss_clu-2.2.7/python/clu/protocol.py
+-rw-r--r--   0        0        0     2805 2024-05-20 19:03:48.535714 sdss_clu-2.2.7/python/clu/store.py
+-rw-r--r--   0        0        0     7820 2024-05-20 19:03:48.535714 sdss_clu-2.2.7/python/clu/testing.py
+-rw-r--r--   0        0        0    16712 2024-05-20 19:03:48.535714 sdss_clu-2.2.7/python/clu/tools.py
+-rw-r--r--   0        0        0     3648 2024-05-20 19:03:48.535714 sdss_clu-2.2.7/python/clu/websocket.py
+-rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 sdss_clu-2.2.7/PKG-INFO
```

### Comparing `sdss_clu-2.2.6/LICENSE.md` & `sdss_clu-2.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/README.rst` & `sdss_clu-2.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/pyproject.toml` & `sdss_clu-2.2.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-clu"
-version = "2.2.6"
+version = "2.2.7"
 description = "A new protocol for SDSS actors."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/sdss/clu"
 repository = "https://github.com/sdss/clu"
 documentation = "https://clu.readthedocs.io/en/latest/"
@@ -33,14 +33,15 @@
 jsonschema = "^4.0.1"
 sdsstools = "^1.0.0"
 prompt_toolkit = "^3.0.6"
 aiormq = "^6.6.4"
 unclick = "^0.1.0b5"
 websockets = {version = "^11.0.3", optional = true}
 click-default-group = "^1.2.2"
+click-aliases = "^1.0.4"
 
 [tool.poetry.group.dev.dependencies]
 ipython = ">=8.0.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 toml = ">=0.10.0"
 isort = ">=5.2.2"
@@ -72,26 +73,28 @@
 target-version = ['py311']
 fast = true
 extend-exclude = 'docs/sphinx/examples/.+\.py'
 
 [tool.ruff]
 line-length = 88
 target-version = 'py311'
+
+[tool.ruff.lint]
 select = ["E", "F", "I"]
-exclude = ["docs/sphinx/examples", "python/clu/legacy/types"]
+exclude = ["docs/sphinx/examples/*.py", "python/clu/legacy/types/*.py"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403", "E402"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["clu"]
 lines-after-imports = 2
 section-order = ["future", "standard-library", "typing", "third-party", "sdss", "first-party", "local-folder"]
 
-[tool.ruff.isort.sections]
+[tool.ruff.lint.isort.sections]
 typing = ["typing"]
 sdss = ["sdsstools"]
 
 [tool.pytest.ini_options]
 addopts = "--cov clu --cov-report xml --cov-report html --cov-report term -p no:warnings"
 asyncio_mode = "auto"
```

### Comparing `sdss_clu-2.2.6/python/clu/__init__.py` & `sdss_clu-2.2.7/python/clu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/__main__.py` & `sdss_clu-2.2.7/python/clu/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/actor.py` & `sdss_clu-2.2.7/python/clu/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/base.py` & `sdss_clu-2.2.7/python/clu/base.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/client.py` & `sdss_clu-2.2.7/python/clu/client.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/command.py` & `sdss_clu-2.2.7/python/clu/command.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/device.py` & `sdss_clu-2.2.7/python/clu/device.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/exceptions.py` & `sdss_clu-2.2.7/python/clu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/actor.py` & `sdss_clu-2.2.7/python/clu/legacy/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/tron.py` & `sdss_clu-2.2.7/python/clu/legacy/tron.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/html.py` & `sdss_clu-2.2.7/python/clu/legacy/types/html.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/keys.py` & `sdss_clu-2.2.7/python/clu/legacy/types/keys.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/messages.py` & `sdss_clu-2.2.7/python/clu/legacy/types/messages.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/parser.py` & `sdss_clu-2.2.7/python/clu/legacy/types/parser.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/ply/cpp.py` & `sdss_clu-2.2.7/python/clu/legacy/types/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/ply/ctokens.py` & `sdss_clu-2.2.7/python/clu/legacy/types/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/ply/lex.py` & `sdss_clu-2.2.7/python/clu/legacy/types/ply/lex.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/ply/yacc.py` & `sdss_clu-2.2.7/python/clu/legacy/types/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/ply/ygen.py` & `sdss_clu-2.2.7/python/clu/legacy/types/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/pvt.py` & `sdss_clu-2.2.7/python/clu/legacy/types/pvt.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/legacy/types/types.py` & `sdss_clu-2.2.7/python/clu/legacy/types/types.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/model.py` & `sdss_clu-2.2.7/python/clu/model.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/parsers/click.py` & `sdss_clu-2.2.7/python/clu/parsers/click.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import shlex
 import time
 
 from typing import Any, List, TypeVar
 
 import click
 from click.decorators import group, pass_obj
+from click_aliases import ClickAliasedGroup
 from unclick.core import command_to_json
 
 from sdsstools.logger import SDSSLogger
 
 from clu.command import Command
 
 from .. import actor
@@ -275,15 +276,15 @@
             # Cancel the oldest running one (although there should only be one)
             running_tasks[0].cancel()
 
             command.finish(text="Command has been scheduled for cancellation.")
             return True
 
 
-class CluGroup(click.Group):
+class CluGroup(ClickAliasedGroup):
     """Override :py:class:`click.Group`.
 
     Makes all child commands instances of `.CluCommand`.
 
     """
 
     def command(self, *args, **kwargs):
@@ -291,15 +292,15 @@
 
         if "cls" in kwargs:
             pass
         else:
             kwargs["cls"] = CluCommand
 
         def decorator(f):
-            cmd = click.decorators.command(*args, **kwargs)(f)
+            cmd = ClickAliasedGroup.command(self, *args, **kwargs)(f)
             self.add_command(cmd)
             return cmd
 
         return decorator
 
     def parse_args(self, ctx, args):  # pragma: no cover
         # Copy this method so that we can turn off the printing of the
```

### Comparing `sdss_clu-2.2.6/python/clu/parsers/json.py` & `sdss_clu-2.2.7/python/clu/parsers/json.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/protocol.py` & `sdss_clu-2.2.7/python/clu/protocol.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/store.py` & `sdss_clu-2.2.7/python/clu/store.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/testing.py` & `sdss_clu-2.2.7/python/clu/testing.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/tools.py` & `sdss_clu-2.2.7/python/clu/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/python/clu/websocket.py` & `sdss_clu-2.2.7/python/clu/websocket.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.2.6/PKG-INFO` & `sdss_clu-2.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-clu
-Version: 2.2.6
+Version: 2.2.7
 Summary: A new protocol for SDSS actors.
 Home-page: https://github.com/sdss/clu
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: websocket
 Requires-Dist: aio_pika (>=9.0.0,<10.0.0)
 Requires-Dist: aiormq (>=6.6.4,<7.0.0)
 Requires-Dist: click (>=8.0,<9.0)
+Requires-Dist: click-aliases (>=1.0.4,<2.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: jsonschema (>=4.0.1,<5.0.0)
 Requires-Dist: prompt_toolkit (>=3.0.6,<4.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Requires-Dist: unclick (>=0.1.0b5,<0.2.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0) ; extra == "websocket"
 Project-URL: Documentation, https://clu.readthedocs.io/en/latest/
```


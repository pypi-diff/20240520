# Comparing `tmp/aergia-0.1.0.tar.gz` & `tmp/aergia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aergia-0.1.0.tar", max compression
+gzip compressed data, was "aergia-0.2.0.tar", max compression
```

## Comparing `aergia-0.1.0.tar` & `aergia-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,26 @@
--rw-r--r--   0        0        0      570 2024-05-19 15:44:26.834212 aergia-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-18 08:48:05.330264 aergia-0.1.0/aergia/__init__.py
--rw-r--r--   0        0        0       43 2024-05-19 14:21:22.863021 aergia-0.1.0/aergia/__main__.py
--rw-r--r--   0        0        0        0 2024-05-18 15:02:43.450687 aergia-0.1.0/aergia/_cli/__init__.py
--rw-r--r--   0        0        0     3997 2024-05-19 09:43:20.741158 aergia-0.1.0/aergia/_cli/_command.py
--rw-r--r--   0        0        0      571 2024-05-19 13:42:23.816376 aergia-0.1.0/aergia/_cli/_output.py
--rw-r--r--   0        0        0     7936 2024-05-19 15:28:29.075376 aergia-0.1.0/aergia/_cli/_parser.py
--rw-r--r--   0        0        0       19 2024-05-19 15:32:22.778157 aergia-0.1.0/aergia/_config.py
--rw-r--r--   0        0        0       54 2024-05-19 14:13:54.766074 aergia-0.1.0/aergia/_logging.py
--rw-r--r--   0        0        0     1996 2024-05-19 15:32:19.885569 aergia-0.1.0/aergia/_storage.py
--rw-r--r--   0        0        0     1742 2024-05-19 14:54:36.540710 aergia-0.1.0/aergia/application.py
--rw-r--r--   0        0        0      914 2024-05-19 14:28:55.913175 aergia-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 aergia-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      570 2024-05-19 18:42:59.981661 aergia-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 18:42:59.981661 aergia-0.2.0/aergia/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-19 18:42:59.981661 aergia-0.2.0/aergia/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:42:59.981661 aergia-0.2.0/aergia/_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 19:48:05.263630 aergia-0.2.0/aergia/_cli/_command/__init__.py
+-rw-r--r--   0        0        0     2201 2024-05-20 20:12:19.556543 aergia-0.2.0/aergia/_cli/_command/_chat.py
+-rw-r--r--   0        0        0      591 2024-05-20 20:16:06.607902 aergia-0.2.0/aergia/_cli/_command/_code.py
+-rw-r--r--   0        0        0      739 2024-05-20 20:17:01.876657 aergia-0.2.0/aergia/_cli/_command/_execute.py
+-rw-r--r--   0        0        0     4409 2024-05-20 20:36:05.748998 aergia-0.2.0/aergia/_cli/_command/_image.py
+-rw-r--r--   0        0        0      413 2024-05-20 20:19:17.478536 aergia-0.2.0/aergia/_cli/_command/_info.py
+-rw-r--r--   0        0        0     1060 2024-05-20 20:11:41.467997 aergia-0.2.0/aergia/_cli/_command/_models.py
+-rw-r--r--   0        0        0     1244 2024-05-20 20:20:11.867292 aergia-0.2.0/aergia/_cli/_command/_parser.py
+-rw-r--r--   0        0        0      369 2024-05-20 20:14:50.754826 aergia-0.2.0/aergia/_cli/_command/_repl.py
+-rw-r--r--   0        0        0     1733 2024-05-20 20:18:38.381993 aergia-0.2.0/aergia/_cli/_command/_role.py
+-rw-r--r--   0        0        0     1238 2024-05-20 20:17:51.293338 aergia-0.2.0/aergia/_cli/_command/_session.py
+-rw-r--r--   0        0        0      379 2024-05-20 20:14:09.898196 aergia-0.2.0/aergia/_cli/_command/_tui.py
+-rw-r--r--   0        0        0     1811 2024-05-20 20:07:58.788858 aergia-0.2.0/aergia/_cli/_command/_utilities.py
+-rw-r--r--   0        0        0       84 2024-05-20 20:21:44.636581 aergia-0.2.0/aergia/_cli/_io.py
+-rw-r--r--   0        0        0       19 2024-05-19 18:42:59.981661 aergia-0.2.0/aergia/_config.py
+-rw-r--r--   0        0        0       54 2024-05-19 18:42:59.981661 aergia-0.2.0/aergia/_logging.py
+-rw-r--r--   0        0        0        0 2024-05-20 20:29:09.726966 aergia-0.2.0/aergia/_model/__init__.py
+-rw-r--r--   0        0        0     1600 2024-05-20 20:36:05.752998 aergia-0.2.0/aergia/_model/_data.py
+-rw-r--r--   0        0        0     3232 2024-05-20 20:36:50.493647 aergia-0.2.0/aergia/_model/_storage.py
+-rw-r--r--   0        0        0     1758 2024-05-20 20:22:16.113022 aergia-0.2.0/aergia/application.py
+-rw-r--r--   0        0        0     1007 2024-05-20 20:40:15.044583 aergia-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 aergia-0.2.0/PKG-INFO
```

### Comparing `aergia-0.1.0/README.md` & `aergia-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aergia-0.1.0/aergia/application.py` & `aergia-0.2.0/aergia/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import sys
 import logging
 
 from functools import wraps
-from aergia._cli._parser import make_parser
-from aergia._cli._output import stderr, stdout
-from aergia._cli._command import ExitCode
+from aergia._cli._command._parser import make_parser
+from aergia._cli._io import stderr, stdout
+from aergia._cli._command._utilities import ExitCode
 from aergia._logging import logger
 from rich.logging import RichHandler
 
 
 def _protect(func, *args, **kwargs):
     @wraps(func)
     def wrapper(*args, **kwargs):
```

### Comparing `aergia-0.1.0/pyproject.toml` & `aergia-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aergia"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Nicola Coretti <nico.coretti@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
@@ -31,7 +31,12 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 aergia = "aergia.application:main"
 ae = "aergia.application:main"
+
+[tool.pytest.ini_options]
+markers = [
+    "openai_api:  tests utilizing the openai api.",
+]
```

### Comparing `aergia-0.1.0/PKG-INFO` & `aergia-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aergia
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/Nicoretti/one-piece/python/aergia
 Keywords: ai,openai,llm,tui,cli,repl
 Author: Nicola Coretti
 Author-email: nico.coretti@gmail.com
 Requires-Python: >=3.10
 Classifier: Development Status :: 2 - Pre-Alpha
```


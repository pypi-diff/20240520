# Comparing `tmp/makolator-2.5.0.tar.gz` & `tmp/makolator-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makolator-2.5.0.tar", max compression
+gzip compressed data, was "makolator-2.6.0.tar", max compression
```

## Comparing `makolator-2.5.0.tar` & `makolator-2.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-05-11 17:22:18.766346 makolator-2.5.0/LICENSE
--rw-r--r--   0        0        0     1210 2024-05-11 17:22:18.766346 makolator-2.5.0/README.md
--rw-r--r--   0        0        0     5563 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/__init__.py
--rw-r--r--   0        0        0     1182 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/__main__.py
--rw-r--r--   0        0        0     9425 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/_inplace.py
--rw-r--r--   0        0        0     5451 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/_staticcode.py
--rw-r--r--   0        0        0     2283 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/_util.py
--rw-r--r--   0        0        0     4960 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/cli.py
--rw-r--r--   0        0        0     3167 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/config.py
--rw-r--r--   0        0        0     2004 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/datamodel.py
--rw-r--r--   0        0        0     2006 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/escape.py
--rw-r--r--   0        0        0     1215 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/exceptions.py
--rw-r--r--   0        0        0     2519 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/helper.py
--rw-r--r--   0        0        0     1902 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/info.py
--rw-r--r--   0        0        0    10229 2024-05-11 17:22:18.766346 makolator-2.5.0/makolator/makolator.py
--rw-r--r--   0        0        0     2434 2024-05-11 17:22:18.766346 makolator-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 makolator-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-20 13:35:25.096228 makolator-2.6.0/LICENSE
+-rw-r--r--   0        0        0     1210 2024-05-20 13:35:25.096228 makolator-2.6.0/README.md
+-rw-r--r--   0        0        0     5563 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/__init__.py
+-rw-r--r--   0        0        0     1182 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/__main__.py
+-rw-r--r--   0        0        0     9427 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/_inplace.py
+-rw-r--r--   0        0        0     5452 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/_staticcode.py
+-rw-r--r--   0        0        0     2283 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/_util.py
+-rw-r--r--   0        0        0     4960 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/cli.py
+-rw-r--r--   0        0        0     3167 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/config.py
+-rw-r--r--   0        0        0     2004 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/datamodel.py
+-rw-r--r--   0        0        0     2006 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/escape.py
+-rw-r--r--   0        0        0     1215 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/exceptions.py
+-rw-r--r--   0        0        0     2519 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/helper.py
+-rw-r--r--   0        0        0     1902 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/info.py
+-rw-r--r--   0        0        0    10402 2024-05-20 13:35:25.100228 makolator-2.6.0/makolator/makolator.py
+-rw-r--r--   0        0        0     2434 2024-05-20 13:35:25.100228 makolator-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 makolator-2.6.0/PKG-INFO
```

### Comparing `makolator-2.5.0/LICENSE` & `makolator-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/README.md` & `makolator-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/__init__.py` & `makolator-2.6.0/makolator/__init__.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/__main__.py` & `makolator-2.6.0/makolator/__main__.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/_inplace.py` & `makolator-2.6.0/makolator/_inplace.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                 msg = f"missing END tag for '{filepath!s}:{tinfo.lineno}'"
                 raise MakolatorError(msg)
 
             # search for "INPLACE END"
             endmatch = tend.match(line)
             if endmatch:
                 outputfile.write(self._fill_marker(endmatch))
-                LOGGER.info("Template '%s:%d'", str(outputfile), tinfo.lineno)
+                LOGGER.debug("Template '%s:%d'", str(outputfile), tinfo.lineno)
                 templates.append(Template("".join(tinfo.lines), lookup=lookup))
                 break
             else:
                 # propagate
                 outputfile.write(line)
 
             if line.startswith(pre):
@@ -191,15 +191,15 @@
             return InplaceInfo(lineno, indent, funcname, args, func, end)
         if not self.ignore_unknown:
             raise MakolatorError(f"{filepath!s}:{lineno} Function '{funcname}' is not found in templates.")
         return None
 
     def _fill_inplace(self, filepath: Path, outputfile, inplace: InplaceInfo, context: dict):
         # pylint: disable=too-many-locals
-        LOGGER.info("Inplace '%s:%d'", str(filepath), inplace.lineno)
+        LOGGER.debug("Inplace '%s:%d'", str(filepath), inplace.lineno)
         # determine args, kwargs
         try:
             # pylint: disable=eval-used
             args, kwargs = eval(f"_extract({inplace.args})", {"_extract": _extract})
         except Exception as exc:
             raise MakolatorError(
                 f"{filepath!s}:{inplace.lineno} Function invocation failed. "
```

### Comparing `makolator-2.5.0/makolator/_staticcode.py` & `makolator-2.6.0/makolator/_staticcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         if beginmatch:
             msg = f"missing END tag {info.name!r} for '{filepath!s}:{info.lineno}'"
             raise MakolatorError(msg)
 
         endmatch = end.match(line)
         if endmatch:
             # consume END
-            LOGGER.info("Static Code %r at '%s:%d'", info.name, str(filepath), info.lineno)
+            LOGGER.debug("Static Code %r at '%s:%d'", info.name, str(filepath), info.lineno)
             if info.name not in staticcodemap:
                 staticcodemap[info.name] = "".join(lines)
             else:
                 msg = f"duplicate static code {info.name!r} at '{filepath!s}:{info.lineno}'"
                 raise MakolatorError(msg)
             check_indent(filepath, lineno, info.indent, endmatch.group("indent"))
             break
```

### Comparing `makolator-2.5.0/makolator/_util.py` & `makolator-2.6.0/makolator/_util.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/cli.py` & `makolator-2.6.0/makolator/cli.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/config.py` & `makolator-2.6.0/makolator/config.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/datamodel.py` & `makolator-2.6.0/makolator/datamodel.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/escape.py` & `makolator-2.6.0/makolator/escape.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/exceptions.py` & `makolator-2.6.0/makolator/exceptions.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/helper.py` & `makolator-2.6.0/makolator/helper.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/info.py` & `makolator-2.6.0/makolator/info.py`

 * *Files identical despite different names*

### Comparing `makolator-2.5.0/makolator/makolator.py` & `makolator-2.6.0/makolator/makolator.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 """
 The Makolator.
 
 A simple API to an improved Mako.
 """
 
 import hashlib
-import logging
 import sys
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from shutil import rmtree
 from typing import Generator, List, Optional, Tuple
 
@@ -42,22 +41,20 @@
 from mako.template import Template
 from outputfile import Existing, open_
 from uniquer import uniquelist
 
 from . import escape, helper
 from ._inplace import InplaceRenderer
 from ._staticcode import StaticCode, read
-from ._util import Paths, humanify, norm_paths
+from ._util import LOGGER, Paths, humanify, norm_paths
 from .config import Config
 from .datamodel import Datamodel
 from .exceptions import MakolatorError
 from .info import Info
 
-LOGGER = logging.getLogger("makolator")
-
 HELPER = {
     "indent": helper.indent,
     "prefix": helper.prefix,
     "run": helper.run,
     "tex": escape.tex,
 }
 
@@ -130,31 +127,33 @@
             template_filepaths: Templates.
 
         Keyword Args:
             dest: Output File.
             context: Key-Value Pairs pairs forwarded to the template.
         """
         template_filepaths = norm_paths(template_filepaths)
-        LOGGER.debug("gen(%r, %s)", [str(filepath) for filepath in template_filepaths], dest)
+        LOGGER.debug("_gen(%r, %r)", [str(filepath) for filepath in template_filepaths], str(dest or "STDOUT"))
         tplfilepaths, lookup = self._create_template_lookup(
             template_filepaths, self.config.template_paths, required=True
         )
         templates = self._create_templates(tplfilepaths, lookup)
         context = context or {}
         comment_sep = self._get_comment_sep(dest)
         if dest is None:
             with read(dest, comment_sep, self.config) as staticcode:
-                self._render(next(templates), sys.stdout, None, context, staticcode)
+                template = next(templates)  # Load template
+                LOGGER.info("gen(%r, STDOUT)", template.filename)
+                self._render(template, sys.stdout, None, context, staticcode)
         else:
             # Mako takes care about proper newline handling. Therefore we deactivate
             # the universal newline mode, by setting newline="".
             with self.open_outputfile(dest, newline="") as output:
                 with read(dest, comment_sep, self.config) as staticcode:
                     template = next(templates)  # Load template
-                    LOGGER.info("Generate '%s'", dest)
+                    LOGGER.info("gen(%r, %r)", template.filename, str(dest))
                     self._render(template, output, dest, context, staticcode)
 
     def _render(self, template: Template, output, dest: Optional[Path], context: dict, staticcode: StaticCode):
         # pylint: disable=too-many-arguments
         context = Context(output, **self._get_render_context(dest, context, staticcode))
         template.render_context(context)
 
@@ -173,30 +172,30 @@
             dest: File to update.
 
         Keyword Args:
             context: Key-Value Pairs pairs forwarded to the template.
             ignore_unknown: Ignore unknown inplace markers, instead of raising an error.
         """
         template_filepaths = norm_paths(template_filepaths)
-        LOGGER.debug("inplace(%r, %s)", [str(filepath) for filepath in template_filepaths], filepath)
+        LOGGER.debug("_inplace(%r, %r)", [str(filepath) for filepath in template_filepaths], str(filepath))
         tplfilepaths, lookup = self._create_template_lookup(template_filepaths, self.config.template_paths)
         templates = tuple(self._create_templates(tplfilepaths, lookup))
         config = self.config
         context = context or {}
         comment_sep = self._get_comment_sep(filepath)
         eol = self._get_eol(filepath, config.inplace_eol_comment)
         inplace = InplaceRenderer(config, templates, ignore_unknown, eol)
         with self.open_outputfile(filepath, existing=Existing.KEEP_TIMESTAMP, newline="") as outputfile:
             with read(filepath, comment_sep, config) as staticcode:
+                LOGGER.info("inplace(%r, %r)", str(tplfilepaths[0]) if tplfilepaths else None, str(filepath))
                 context = self._get_render_context(filepath, context, staticcode)
                 inplace.render(lookup, filepath, outputfile, context)
 
     def _create_templates(self, tplfilepaths: List[Path], lookup: TemplateLookup) -> Generator[Template, None, None]:
         for tplfilepath in tplfilepaths:
-            LOGGER.info("Template '%s'", tplfilepath)
             yield lookup.get_template(tplfilepath.name)
         yield Template(
             """<%! from makolator import helper %>
 <%def name="run(*args, **kwargs)">\
 ${helper.run(*args, **kwargs)}\
 </%def>"""
         )
```

### Comparing `makolator-2.5.0/pyproject.toml` & `makolator-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makolator"
-version = "2.5.0"
+version = "2.6.0"
 description = "Extended Mako Templates for Python"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `makolator-2.5.0/PKG-INFO` & `makolator-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makolator
-Version: 2.5.0
+Version: 2.6.0
 Summary: Extended Mako Templates for Python
 License: MIT
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/gifnoc-0.3.2.tar.gz` & `tmp/gifnoc-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gifnoc-0.3.2.tar", max compression
+gzip compressed data, was "gifnoc-0.3.3.tar", max compression
```

## Comparing `gifnoc-0.3.2.tar` & `gifnoc-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2268 2024-03-13 17:48:39.575307 gifnoc-0.3.2/README.md
--rw-r--r--   0        0        0      431 2024-04-04 05:32:30.662546 gifnoc-0.3.2/gifnoc/__init__.py
--rw-r--r--   0        0        0     3261 2024-04-17 20:19:50.897932 gifnoc-0.3.2/gifnoc/__main__.py
--rw-r--r--   0        0        0     3547 2024-04-18 01:47:41.546298 gifnoc-0.3.2/gifnoc/acquire.py
--rw-r--r--   0        0        0     6497 2024-04-17 20:43:59.542425 gifnoc-0.3.2/gifnoc/arg.py
--rw-r--r--   0        0        0      126 2024-04-04 03:48:14.345716 gifnoc-0.3.2/gifnoc/config.py
--rw-r--r--   0        0        0     4420 2024-03-14 18:27:32.891465 gifnoc-0.3.2/gifnoc/docstrings.py
--rw-r--r--   0        0        0     6544 2024-04-17 20:19:50.897927 gifnoc-0.3.2/gifnoc/interface.py
--rw-r--r--   0        0        0     1347 2024-04-17 20:19:50.897737 gifnoc-0.3.2/gifnoc/merge.py
--rw-r--r--   0        0        0     3835 2024-04-17 20:16:50.868285 gifnoc-0.3.2/gifnoc/parse.py
--rw-r--r--   0        0        0     1362 2024-04-17 20:19:50.896918 gifnoc-0.3.2/gifnoc/proxy.py
--rw-r--r--   0        0        0     6717 2024-04-17 20:19:50.898068 gifnoc-0.3.2/gifnoc/registry.py
--rw-r--r--   0        0        0     1617 2024-04-04 03:48:14.390506 gifnoc-0.3.2/gifnoc/schema.py
--rw-r--r--   0        0        0      247 2024-03-08 22:39:08.607547 gifnoc-0.3.2/gifnoc/std/__init__.py
--rw-r--r--   0        0        0      822 2024-04-04 03:48:14.346765 gifnoc-0.3.2/gifnoc/std/_time.py
--rw-r--r--   0        0        0     3976 2024-04-17 20:19:50.897814 gifnoc-0.3.2/gifnoc/type_wrappers.py
--rw-r--r--   0        0        0     4259 2024-04-17 21:31:33.848158 gifnoc-0.3.2/gifnoc/utils.py
--rw-r--r--   0        0        0       18 2024-04-18 02:07:27.632643 gifnoc-0.3.2/gifnoc/version.py
--rw-r--r--   0        0        0      671 2024-04-18 02:07:27.608528 gifnoc-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 gifnoc-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2268 2024-03-13 17:48:39.575307 gifnoc-0.3.3/README.md
+-rw-r--r--   0        0        0      431 2024-04-04 05:32:30.662546 gifnoc-0.3.3/gifnoc/__init__.py
+-rw-r--r--   0        0        0     3769 2024-05-20 18:19:59.219349 gifnoc-0.3.3/gifnoc/__main__.py
+-rw-r--r--   0        0        0     3547 2024-04-18 01:47:41.546298 gifnoc-0.3.3/gifnoc/acquire.py
+-rw-r--r--   0        0        0     6497 2024-04-17 20:43:59.542425 gifnoc-0.3.3/gifnoc/arg.py
+-rw-r--r--   0        0        0      126 2024-04-04 03:48:14.345716 gifnoc-0.3.3/gifnoc/config.py
+-rw-r--r--   0        0        0     4420 2024-03-14 18:27:32.891465 gifnoc-0.3.3/gifnoc/docstrings.py
+-rw-r--r--   0        0        0     6544 2024-04-17 20:19:50.897927 gifnoc-0.3.3/gifnoc/interface.py
+-rw-r--r--   0        0        0     1347 2024-04-17 20:19:50.897737 gifnoc-0.3.3/gifnoc/merge.py
+-rw-r--r--   0        0        0     3835 2024-04-17 20:16:50.868285 gifnoc-0.3.3/gifnoc/parse.py
+-rw-r--r--   0        0        0     1362 2024-04-17 20:19:50.896918 gifnoc-0.3.3/gifnoc/proxy.py
+-rw-r--r--   0        0        0     6717 2024-04-17 20:19:50.898068 gifnoc-0.3.3/gifnoc/registry.py
+-rw-r--r--   0        0        0     1617 2024-04-04 03:48:14.390506 gifnoc-0.3.3/gifnoc/schema.py
+-rw-r--r--   0        0        0      247 2024-03-08 22:39:08.607547 gifnoc-0.3.3/gifnoc/std/__init__.py
+-rw-r--r--   0        0        0      822 2024-04-04 03:48:14.346765 gifnoc-0.3.3/gifnoc/std/_time.py
+-rw-r--r--   0        0        0     3976 2024-04-17 20:19:50.897814 gifnoc-0.3.3/gifnoc/type_wrappers.py
+-rw-r--r--   0        0        0     4259 2024-04-17 21:31:33.848158 gifnoc-0.3.3/gifnoc/utils.py
+-rw-r--r--   0        0        0       18 2024-05-20 18:23:19.283491 gifnoc-0.3.3/gifnoc/version.py
+-rw-r--r--   0        0        0      671 2024-05-20 18:23:19.259398 gifnoc-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 gifnoc-0.3.3/PKG-INFO
```

### Comparing `gifnoc-0.3.2/README.md` & `gifnoc-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/__main__.py` & `gifnoc-0.3.3/gifnoc/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 import argparse
 import json
 import os
 from importlib import import_module
 
 from apischema import serialize
 
-from .core import use
+from .interface import global_registry, use
 from .parse import EnvironMap, extensions
-from .registry import global_registry
 from .schema import deserialization_schema
 from .utils import get_at_path, type_at_path
 
 
-def command_dump(options, sources):
+def extract(options, sources):
     with use(*sources()) as cfg:
+        data = cfg.data
         if options.SUBPATH:
-            cfg = get_at_path(cfg, options.SUBPATH.split("."))
-        ser = serialize(cfg)
-        if options.format == "raw":
-            print(ser)
+            data = get_at_path(data, options.SUBPATH.split("."))
+        return data
+
+
+def command_dump(options, sources):
+    data = extract(options, sources)
+    ser = serialize(data)
+    if options.format == "raw":
+        print(ser)
+    else:
+        fmt = f".{options.format}"
+        if fmt not in extensions:
+            exit(f"Cannot dump to '{options.format}' format")
         else:
-            fmt = f".{options.format}"
-            if fmt not in extensions:
-                exit(f"Cannot dump to '{options.format}' format")
-            else:
-                print(extensions[fmt].dump(ser))
+            print(extensions[fmt].dump(ser))
+
+
+def command_check(options, sources):
+    try:
+        data = extract(options, sources)
+    except AttributeError:
+        print("nonexistent")
+        exit(2)
+    if data:
+        print("true")
+        exit(0)
+    elif not data:
+        print("false")
+        exit(1)
 
 
 def command_schema(options, sources):
     with use(*sources(require=False)) as cfg:
-        cfg_type = type(cfg)
+        cfg_type = type(cfg.data)
         if options.SUBPATH:
             cfg_type, _ = type_at_path(cfg_type, options.SUBPATH.split("."))
         schema = deserialization_schema(cfg_type)
         print(json.dumps(schema, indent=4))
 
 
 def main():
@@ -62,14 +81,17 @@
 
     subparsers = parser.add_subparsers(dest="command", required=True)
 
     dump = subparsers.add_parser("dump", help="Dump configuration.")
     dump.add_argument("SUBPATH", help="Subpath to dump", nargs="?", default=None)
     dump.add_argument("--format", "-f", help="Dump format", default="raw")
 
+    dump = subparsers.add_parser("check", help="Check configuration (true/false).")
+    dump.add_argument("SUBPATH", help="Subpath to check", nargs="?", default=None)
+
     schema = subparsers.add_parser("schema", help="Dump JSON schema.")
     schema.add_argument("SUBPATH", help="Subpath to get a schema for", nargs="?", default=None)
 
     options = parser.parse_args()
 
     from_env = os.environ.get("GIFNOC_MODULE", None)
     from_env = from_env.split(",") if from_env else []
```

### Comparing `gifnoc-0.3.2/gifnoc/acquire.py` & `gifnoc-0.3.3/gifnoc/acquire.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/arg.py` & `gifnoc-0.3.3/gifnoc/arg.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/docstrings.py` & `gifnoc-0.3.3/gifnoc/docstrings.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/interface.py` & `gifnoc-0.3.3/gifnoc/interface.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/merge.py` & `gifnoc-0.3.3/gifnoc/merge.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/parse.py` & `gifnoc-0.3.3/gifnoc/parse.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/proxy.py` & `gifnoc-0.3.3/gifnoc/proxy.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/registry.py` & `gifnoc-0.3.3/gifnoc/registry.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/schema.py` & `gifnoc-0.3.3/gifnoc/schema.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/std/_time.py` & `gifnoc-0.3.3/gifnoc/std/_time.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/type_wrappers.py` & `gifnoc-0.3.3/gifnoc/type_wrappers.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/gifnoc/utils.py` & `gifnoc-0.3.3/gifnoc/utils.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.2/pyproject.toml` & `gifnoc-0.3.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gifnoc"
-version = "0.3.2"
+version = "0.3.3"
 description = "Handle configuration for multiple libraries"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gifnoc-0.3.2/PKG-INFO` & `gifnoc-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gifnoc
-Version: 0.3.2
+Version: 0.3.3
 Summary: Handle configuration for multiple libraries
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


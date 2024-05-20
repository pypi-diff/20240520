# Comparing `tmp/toolfuse-0.1.23.tar.gz` & `tmp/toolfuse-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.23.tar", max compression
+gzip compressed data, was "toolfuse-0.1.24.tar", max compression
```

## Comparing `toolfuse-0.1.23.tar` & `toolfuse-0.1.24.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.23/LICENSE
--rw-r--r--   0        0        0     4594 2024-05-05 16:31:27.833089 toolfuse-0.1.23/README.md
--rw-r--r--   0        0        0      803 2024-05-09 18:37:40.377543 toolfuse-0.1.23/pyproject.toml
--rw-r--r--   0        0        0      435 2024-05-05 03:00:01.092317 toolfuse-0.1.23/toolfuse/__init__.py
--rw-r--r--   0        0        0    30555 2024-05-09 18:37:31.926716 toolfuse-0.1.23/toolfuse/base.py
--rw-r--r--   0        0        0      231 2024-05-09 18:34:01.339814 toolfuse-0.1.23/toolfuse/models.py
--rw-r--r--   0        0        0      996 2024-05-05 02:09:19.322511 toolfuse-0.1.23/toolfuse/multi.py
--rw-r--r--   0        0        0      543 2024-05-05 03:06:09.263475 toolfuse-0.1.23/toolfuse/util.py
--rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 toolfuse-0.1.23/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.24/LICENSE
+-rw-r--r--   0        0        0     4594 2024-05-05 16:31:27.833089 toolfuse-0.1.24/README.md
+-rw-r--r--   0        0        0      803 2024-05-20 20:55:38.506063 toolfuse-0.1.24/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-05-05 03:00:01.092317 toolfuse-0.1.24/toolfuse/__init__.py
+-rw-r--r--   0        0        0    30555 2024-05-20 20:56:34.273635 toolfuse-0.1.24/toolfuse/base.py
+-rw-r--r--   0        0        0      231 2024-05-20 20:55:10.878956 toolfuse-0.1.24/toolfuse/models.py
+-rw-r--r--   0        0        0      996 2024-05-05 02:09:19.322511 toolfuse-0.1.24/toolfuse/multi.py
+-rw-r--r--   0        0        0      543 2024-05-05 03:06:09.263475 toolfuse-0.1.24/toolfuse/util.py
+-rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 toolfuse-0.1.24/PKG-INFO
```

### Comparing `toolfuse-0.1.23/LICENSE` & `toolfuse-0.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.23/README.md` & `toolfuse-0.1.24/README.md`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.23/pyproject.toml` & `toolfuse-0.1.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.23"
+version = "0.1.24"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
```

### Comparing `toolfuse-0.1.23/toolfuse/base.py` & `toolfuse-0.1.24/toolfuse/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,34 +351,34 @@
 
         Returns:
             str: LLM context for the tool
         """
         return self.__doc__  # type: ignore
 
     @classmethod
-    def name(cls) -> str:
-        """Tool name
+    def type(cls) -> str:
+        """Tool type
 
         Returns:
-            str: Tool name
+            str: Tool type
         """
         return cls.__name__
 
     def ref(self) -> V1ToolRef:
         """Tool reference"""
         module = getmodule(self)
         if not module:
             raise ValueError("Tool not associated with a module")
         mod_parts = module.__name__.split(".")
         version = None
         try:
             version = pkgversion(mod_parts[0])
         except:
             pass
-        return V1ToolRef(module=module.__name__, name=self.name(), version=version)
+        return V1ToolRef(module=module.__name__, type=self.type(), version=version)
 
     def add_action(self, method: Callable) -> None:
         """
         Adds a new action to the tool using only the method provided. Name, schema,
         and description are derived automatically.
 
         Args:
@@ -528,15 +528,15 @@
 
         Attributes:
             Inherits all attributes from the Tool class and the user-defined class (cls).
 
         Methods:
             __init__(*args, **kwargs): Initializes the Combined class, the Tool part of the class,
                                        and registers methods from the user-defined class as actions.
-            name(): Returns the name of the class.
+            type(): Returns the type of the class.
             _register_methods_from_cls(): Registers public methods from the user-defined class as actions.
         """
 
         def __init__(self, *args, **kwargs):
             """
             Initializes the Combined class by initializing both the user-defined class part and the Tool class part.
             It also registers the methods from the user-defined class (cls) as actions within the Tool framework.
@@ -548,20 +548,20 @@
             cls.__init__(
                 self, *args, **kwargs  # type: ignore
             )  # Initialize the user-defined part of the combined class
             Tool.__init__(self)  # Initialize the Tool part of the combined class
             self._register_methods_from_cls()  # Register methods from cls as actions
 
         @classmethod
-        def name(cls) -> str:
+        def type(cls) -> str:
             """
-            Returns the name of the class.
+            Returns the type of the class.
 
             Returns:
-                str: The name of the class.
+                str: The type of the class.
             """
             return cls.__name__
 
         def _register_methods_from_cls(self):
             """
             Registers all public methods from the user-defined class (cls) as actions.
```

### Comparing `toolfuse-0.1.23/toolfuse/multi.py` & `toolfuse-0.1.24/toolfuse/multi.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.23/toolfuse/util.py` & `toolfuse-0.1.24/toolfuse/util.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.23/PKG-INFO` & `toolfuse-0.1.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.23
+Version: 0.1.24
 Summary: Tools for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


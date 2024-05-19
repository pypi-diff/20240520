# Comparing `tmp/ioxplugin-1.1.0.tar.gz` & `tmp/ioxplugin-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioxplugin-1.1.0.tar", last modified: Mon May 13 22:16:06 2024, max compression
+gzip compressed data, was "ioxplugin-1.1.1.tar", last modified: Sun May 19 23:53:32 2024, max compression
```

## Comparing `ioxplugin-1.1.0.tar` & `ioxplugin-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:16:06.274746 ioxplugin-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 22:16:06.274746 ioxplugin-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:16:06.270746 ioxplugin-1.1.0/ioxplugin/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53706 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/ast_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/iox_controller_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/iox_main_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/iox_node_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/iox_node_impl_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/iox_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/iox_to_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/iox_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/main_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/node_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/nodedef.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/oauth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/plugin_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/uom.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/ioxplugin/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:16:06.274746 ioxplugin-1.1.0/ioxplugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 22:16:06.000000 ioxplugin-1.1.0/ioxplugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-13 22:16:06.000000 ioxplugin-1.1.0/ioxplugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:16:06.000000 ioxplugin-1.1.0/ioxplugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 22:16:06.000000 ioxplugin-1.1.0/ioxplugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 22:16:06.000000 ioxplugin-1.1.0/ioxplugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:16:06.274746 ioxplugin-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:16:06.274746 ioxplugin-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/tests/ModbusControllerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/tests/ModbusDeviceNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/tests/ModbusProtocolHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/tests/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/tests/test_ioxplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 22:16:02.000000 ioxplugin-1.1.0/tests/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:53:32.272451 ioxplugin-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-19 23:53:32.272451 ioxplugin-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:53:32.268451 ioxplugin-1.1.1/ioxplugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50220 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/ast_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/iox_controller_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/iox_main_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/iox_node_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/iox_node_impl_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/iox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/iox_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/main_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/nodedef.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/oauth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/plugin_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/uom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/ioxplugin/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:53:32.268451 ioxplugin-1.1.1/ioxplugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-19 23:53:32.000000 ioxplugin-1.1.1/ioxplugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-19 23:53:32.000000 ioxplugin-1.1.1/ioxplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 23:53:32.000000 ioxplugin-1.1.1/ioxplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 23:53:32.000000 ioxplugin-1.1.1/ioxplugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 23:53:32.000000 ioxplugin-1.1.1/ioxplugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 23:53:32.272451 ioxplugin-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:53:32.268451 ioxplugin-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/tests/ModbusProtocolHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/tests/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/tests/test_ioxplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 23:53:28.000000 ioxplugin-1.1.1/tests/version.py
```

### Comparing `ioxplugin-1.1.0/PKG-INFO` & `ioxplugin-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.1.0
+Version: 1.1.1
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.1.0/ioxplugin/__init__.py` & `ioxplugin-1.1.1/ioxplugin/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 from .plugin import Plugin 
 from .plugin_meta import PluginMetaData 
 from .protocol import Protocol
 from .commands import Commands, CommandDetails, CommandParam 
 from .editor import EditorDetails, Editors
 from .iox_profile import ProfileWriter
-from .log import LOGGER
+from .log import LOGGER as PLUGIN_LOGGER
 from .main_gen import PluginMain
 from .new_project import create_project as CreateNewIoXPluginProject
 from .node_properties import NodeProperties, NodePropertyDetails
 from .nodedef import NodeDefDetails, NodeDefs, NodeProperties
 from .properties import Properties, PropertyDetails
 from .uom import UOMs, UOMDetails, UOMOption
 from .validator import getValidName
-from .iox_to_modbus import ModbusIoX
 from .iox_transport import IoXSerialTransport, IoXTCPTransport,IoXTransport
 from .oauth_service import OAuthService
 from ioxplugin import ast_util
```

### Comparing `ioxplugin-1.1.0/ioxplugin/ast_util.py` & `ioxplugin-1.1.1/ioxplugin/ast_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -990,15 +990,15 @@
 
 def astQueryAllMethod(commands):
     if commands == None or len(commands) <= 0:
         return None
 
     function_def = ast.FunctionDef(
         name='queryAll',
-        args=ast.arguments(args=[], vararg=None, kwonlyargs=[], kw_defaults=[], kwarg=None, defaults=[]),
+        args=ast.arguments(args=[ ast.arg(arg='self', annotation=None)], vararg=None, kwonlyargs=[], kw_defaults=[], kwarg=None, defaults=[]),
         body=[],
         decorator_list=[],
         returns=None
     )
 
     # Add a method call for each query to the function body
     for command in commands:
@@ -1134,127 +1134,14 @@
             )
         ],
         orelse=[]
     )
 
     return main_if
 
-def astDiscoverControllerCommand():
-    return_statement = ast.Return(
-        value = ast.Call(
-        func=ast.Attribute(
-            value=ast.Attribute(
-                value=ast.Name(id='self', ctx=ast.Load()),
-                attr='protocolHandler',
-                ctx=ast.Load()
-            ),
-            attr='discover',
-            ctx=ast.Load()
-        ),
-        args=[],
-        keywords=[]
-    )
-    )
-    body=[
-       return_statement 
-    ]
-    return body
-
-def astQueryAllControllerCommand():
-    body=[
-        # nodes = self.poly.getNodes()
-        ast.Assign(
-            targets=[ast.Name(id='nodes', ctx=ast.Store())],
-            value=ast.Call(
-                func=ast.Attribute(
-                    value=ast.Attribute(
-                        value=ast.Name(id='self', ctx=ast.Load()),
-                        attr='poly',
-                        ctx=ast.Load()
-                    ),
-                    attr='getNodes',
-                    ctx=ast.Load()
-                ),
-                args=[],
-                keywords=[]
-            )
-        ),
-        # if nodes == None or len(nodes) == 0:
-        ast.If(
-            test=ast.BoolOp(
-                op=ast.Or(),
-                values=[
-                    ast.Compare(
-                        left=ast.Name(id='nodes', ctx=ast.Load()),
-                        ops=[ast.Is()],
-                        comparators=[ast.Constant(value=None)]
-                    ),
-                    ast.Compare(
-                        left=ast.Call(
-                            func=ast.Name(id='len', ctx=ast.Load()),
-                            args=[ast.Name(id='nodes', ctx=ast.Load())],
-                            keywords=[]
-                        ),
-                        ops=[ast.Eq()],
-                        comparators=[ast.Constant(value=0)]
-                    )
-                ]
-            ),
-            body=[
-                # return True
-                ast.Return(value=ast.Constant(value=True))
-            ],
-            orelse=[]
-        ),
-        # for n in nodes:
-        ast.For(
-            target=ast.Name(id='n', ctx=ast.Store()),
-            iter=ast.Name(id='nodes', ctx=ast.Load()),
-            body=[
-                # node = nodes[n]
-                ast.Assign(
-                    targets=[ast.Name(id='node', ctx=ast.Store())],
-                    value=ast.Subscript(
-                        value=ast.Name(id='nodes', ctx=ast.Load()),
-                        slice=ast.Name(id='n', ctx=ast.Load()),
-                        ctx=ast.Load()
-                    )
-                ),
-                # if node == None:
-                ast.If(
-                    test=ast.Compare(
-                        left=ast.Name(id='node', ctx=ast.Load()),
-                        ops=[ast.Is()],
-                        comparators=[ast.Constant(value=None)]
-                    ),
-                    body=[
-                        # continue
-                        ast.Continue()
-                    ],
-                    orelse=[
-                        # node.queryAll()
-                        ast.Expr(
-                            value=ast.Call(
-                                func=ast.Attribute(
-                                    value=ast.Name(id='node', ctx=ast.Load()),
-                                    attr='queryAll',
-                                    ctx=ast.Load()
-                                ),
-                                args=[],
-                                keywords=[]
-                            )
-                        )
-                    ]
-                )
-            ],
-            orelse=[]
-        )
-    ]
-    return body
-
 def astSetPluginFunc():
     return ast.FunctionDef(
     name='setProtocolHandler',
     args=ast.arguments(
         posonlyargs=[],
         args=[
             ast.arg(arg='self', annotation=None),
@@ -1312,15 +1199,18 @@
                         ast.Constant(value=property)
                     ],
                     keywords=[]
                 )
             ),
             # Inner if statement
             ast.If(
-                test=ast.Name(id='val', ctx=ast.Load()),
+                test=ast.Compare(
+                left=ast.Name(id='val', ctx=ast.Load()),
+                ops=[ast.NotEq()],
+                comparators=[ast.Constant(value=None)]),
                 body=[
                     # Method call within the inner if statement
                     ast.Expr(
                         value=ast.Call(
                             func=ast.Attribute(
                                 value=ast.Name(id='self', ctx=ast.Load()),
                                 attr=update_method,
@@ -1402,15 +1292,15 @@
     ),
     ast.Return(value=ast.Constant(value=False))
     ]
     return body
 
 def astPHProcessCommandFunc(command_name, args):
 
-    arg_nodes = [ast.Constant(value=command_name)] 
+    arg_nodes = [ast.Name(id='self', ctx=ast.Load()),ast.Constant(value=command_name) ] 
     #for arg in args_array:
     #    arg_nodes.append(ast.Name(id=arg, ctx=ast.Load))
     # Create AST node for function call
     return_statement = ast.Return(
             value=ast.Call(
             func=ast.Name(id='self.protocolHandler.processCommand', ctx=ast.Load()),
             args= arg_nodes,
```

### Comparing `ioxplugin-1.1.0/ioxplugin/commands.py` & `ioxplugin-1.1.1/ioxplugin/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,17 @@
                 self.name = command['name']
             if 'params' in command:
                 params = command['params']
                 for param in params:
                     p = CommandParam(param)
                     self.params[p.id]=p
 
+            if self.id.lower() == "query":
+                self.id = "x_query"
+
         except Exception as ex:
             LOGGER.critical(str(ex))
             raise
 
     def toIoX(self, node_id:str)->(str,str):
         nls = ""
         cmd = ""
```

### Comparing `ioxplugin-1.1.0/ioxplugin/editor.py` & `ioxplugin-1.1.1/ioxplugin/editor.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/iox_controller_template.py` & `ioxplugin-1.1.1/ioxplugin/iox_controller_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,28 +13,28 @@
     def setProtocolHandler(self, protocolHandler):
         self.protocolHandler = protocolHandler
 
     def initOAuth(self):
         if self.protocolHandler and self.protocolHandler.plugin and self.protocolHandler.plugin.meta and self.protocolHandler.plugin.meta.getEnableOAUTH2():
             self.oauthService = OAuthService(self.polyglot)
 
-    def parameter_handler(self, params):
+    def parameterHandler(self, params):
         self.Parameters.load(params)
         return self.protocolHandler.processParams(self.Parameters)
 
     def configHandler(self, param):
         try:
             if os.path.exists(DATA_PATH):
                 self.protocolHandler.filesUploaded(DATA_PATH)
                 shutil.rmtree(DATA_PATH)
-                return
+            if param:
+                return self.protocolHandler.configChanged(param)
         except Exception as ex:
             LOGGER.warn(str(ex))
 
-        self.protocolHandler.configChanged(param)
         return True
 
     def start(self):
         LOGGER.info(f'Starting... ')
         try:
             self.poly.addNode(self)
             self.poly.setCustomParamsDoc()
@@ -69,35 +69,49 @@
         if 'shortPoll' in polltype:
             self.protocolHandler.shortPoll()
         elif 'longPoll' in polltype:
             self.protocolHandler.longPoll()
 
     def addAllNodes(self):
         config = self.poly.getConfig()
-        if config is None or config['nodes'] is None or len(config['nodes']
-            ) <= 0:
+        if config is None or config['nodes'] is None or len(config['nodes']) <= 0:
             config = {}
             config['nodes'] = []
-            for child in self.children:
+        for child in self.children:
+            try:
                 config['nodes'].append({'nodeDefId': child['id'], 'address':
-                    child['node_class'], 'name': child['name'],
-                    'primaryNode': child['parent']})
+                child['id'], 'name': child['name'],
+                'primaryNode': child['parent']})
+            except Exception as ex:
+                LOGGER.error(str(ex))
+                return
         for node in config['nodes']:
+            if node['nodeDefId'] == self.id:
+                continue
             if not self.__addNode(node):
                 return
         LOGGER.info(f'Done adding nodes ...')
 
+    def __getNodeClass(self, nodeDefId:str)->str:
+        for child in self.children:
+            if child['id'] == nodeDefId:
+                return child['node_class']
+        return None
+
     def __addNode(self, node_info) ->bool:
         if node_info is None:
             LOGGER.error('node cannot be null')
             return False
         try:
-            cls = globals()[node_info['address']]
-            node = cls(self.poly, node_info['primaryNode'], node_info[
-                'nodeDefId'], node_info['name'])
+            node_class = self.__getNodeClass(node_info['nodeDefId'])
+            if node_class == None:
+                return False 
+            node_address=self.protocolHandler.getNodeAddress(node_info['nodeDefId'])
+            cls = globals()[node_class]
+            node = cls(self.poly, self.protocolHandler, node_info['primaryNode'], node_address, node_info['name'])
             if node is None:
                 LOGGER.error(f'invalid noddef id ...')
                 return False
             else:
                 node_r = self.poly.addNode(node)
                 if node_r:
                     node_r.setProtocolHandler(self.protocolHandler)
@@ -170,27 +184,27 @@
     
     def updateStatus(self, value, force: bool):
         return self.setDriver("ST", value, 2, force)
 
     def getStatus(self):
         return self.getDriver("ST")
 
-    def Discover(self, command):
+    def discover(self, command):
         return self.protocolHandler.discover()
 
-    def Query(self, command):
+    def query(self, command):
         nodes = self.poly.getNodes()
         if nodes is None or len(nodes) == 0:
             return True
         for n in nodes:
             node = nodes[n]
             if node is None:
                 continue
             else:
-                node.queryAll()
+                node.query()
 
     ###
     # This is a list of commands that were defined in the nodedef
     ###
-    commands = {'discover': Discover, 'query': Query}
+    commands = {'Discover': discover, 'Query': query}
 
 '''
```

### Comparing `ioxplugin-1.1.0/ioxplugin/iox_main_template.py` & `ioxplugin-1.1.1/ioxplugin/iox_main_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 import udi_interface, os, sys, json, time
 import version
 from ioxplugin import Plugin
 from __PROTOCOL_HANDLER_FILE__ import __PROTOCOL_HANDLER_CLASS__
 
 PLUGIN_FILE_NAME = '__PLUGIN_FILE_NAME__'
-from __CONTROLLER_NODE_FILE__ import __CONTROLLER_NODE_CLASS__
 LOGGER = udi_interface.LOGGER
 if __name__ == '__main__':
     try:
         polyglot = udi_interface.Interface([])
         polyglot.start(version.ud_plugin_version)
         plugin = None
         if not os.path.exists(PLUGIN_FILE_NAME):
             polyglot.Notices['config']=f"{PLUGIN_FILE_NAME} does not exist. Uplaod it using file upload ..."
         else:
             plugin = Plugin(PLUGIN_FILE_NAME)
             plugin.toIoX()
             plugin.generateCode(path='./')
         
+        from __CONTROLLER_NODE_FILE__ import __CONTROLLER_NODE_CLASS__
         protocolHandler = __PROTOCOL_HANDLER_CLASS__(plugin)
         controller = __CONTROLLER_NODE_CLASS__(polyglot, protocolHandler)
         protocolHandler.setController(controller)
         controller.start()
         polyglot.runForever()
     except (KeyboardInterrupt, SystemExit):
         LOGGER.info('exiting ...')
```

### Comparing `ioxplugin-1.1.0/ioxplugin/iox_node_gen.py` & `ioxplugin-1.1.1/ioxplugin/iox_node_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
         self.nodedef = nodedef
         self.path = path
  
     def create_command_body(self, command:CommandDetails, command_name):
         if command == None:
             return None
         
-        if not command.hasParams():
-            if command_name == "Query" and command.id == "query":
-                return ast_util.astQueryAllControllerCommand()
-            if command_name == "Discover" and command.id == "discover":
-                return ast_util.astDiscoverControllerCommand()
+  #      if not command.hasParams() and self.nodedef.isController:
+  #          if command_name == "Query" and command.id == "query":
+  #              return ast_util.astQueryAllControllerCommand()
+  #          if command_name == "Discover" and command.id == "discover":
+  #              return ast_util.astDiscoverControllerCommand()
         
         out = []
         error = []
-        impl_args ={} 
+        impl_args ={}
 
         added_jparams=False
         is_property=command.init_prop != None
 
         params = command.getParams()
         for p in params:
             param = params[p] 
@@ -248,15 +248,14 @@
             )
             if not self.nodedef.isController:
                 class_def.body.append(method)
 
         if len (query_commands) > 0 and not self.nodedef.isController:
             class_def.body.append(ast_util.astQueryAllMethod(query_commands)) 
 
-
         #now make the commands
         for command in commands:
             cmd = self.nodedef.commands.acceptCommands[command['id']]
             pass_stmt = ast.Pass()
             command_name=getValidName(command['name'],False)
             body = self.create_command_body(cmd, command_name)
             if not isinstance(body, list):
```

### Comparing `ioxplugin-1.1.0/ioxplugin/iox_node_impl_gen.py` & `ioxplugin-1.1.1/tests/ModbusProtocolHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,13 @@
-import os
-from .log import LOGGER
 
-'''
-This class creates an implemenation class for the Node class
-Methods of this class should be implemented by developers
-'''
-IMPL_PH_TEMPLATE='''
 import udi_interface, os, sys, json, time
 LOGGER = udi_interface.LOGGER
 Custom = udi_interface.Custom
 
-class __PROTOCOL_HANDLER_CLASS__:
+class ModbusProtocolHandler:
     ##
     #Implementation and Protocol Handler class
     ##
 
     ##
     #The plugin has all the information that's stored in the json file.
     #The controller allows you to communicate with the underlying system (PG3).
@@ -246,26 +239,8 @@
     ###
     # If your plugin is an OAuth client, use this method to call APIs that 
     # automatically include all the tokens for authorization and authentication 
     ###
     def callOAuthApi(self, method='GET', url=None, params=None, body=None)->bool:
         return self.controller.callOAuthApi(method, url, params, body)
 
-    '''
-
-class IoXNodeImplGen():
-    def __init__(self, path:str, file_name:str, class_name:str):
-        if class_name == None or file_name == None or path == None:
-            LOGGER.critical("need path, filename, and class_name ")
-            raise Exception ("need path, filename, and class_name") 
-
-        self.file_path=f'{path}/{file_name}'
-        self.class_name = class_name
-        self.class_def = None
-
-    def create(self):
-        if os.path.exists(self.file_path): 
-            LOGGER.info(f"{self.file_path} already exists ... ignoring")
-            #do not redo if already exists
-            return
-        with open(self.file_path, 'w') as file:
-            file.write(IMPL_PH_TEMPLATE.replace("__PROTOCOL_HANDLER_CLASS__",self.class_name))
+
```

### Comparing `ioxplugin-1.1.0/ioxplugin/iox_profile.py` & `ioxplugin-1.1.1/ioxplugin/iox_profile.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/iox_transport.py` & `ioxplugin-1.1.1/ioxplugin/iox_transport.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 from .log import LOGGER
 
 class IoXTCPTransport():
     def __init__(self, comm_params):
         if comm_params == None:
             raise Exception ("Need communication parameters for TCP (host/port)")
+        self.name = "TCP"
         self.host = None
         self.port = None
         self.timeout = None
         self.keepAlive = None
         try:
             if 'host' in comm_params:
                 self.host = comm_params['host'] 
@@ -36,14 +37,15 @@
         pass
 
 class IoXSerialTransport():
     def __init__(self, comm_params):
         if comm_params == None:
             raise Exception ("Need communication parameters for serial (port/baudrate)")
 
+        self.name = "Serial"
         self.port = None
         self.baudrate = 115200
         self.timeout=1
         self.databits=serial.EIGHTBITS
         self.parity=serial.PARITY_NONE 
         self.stopbits=serial.STOPBITS_ONE
         self.flowcontrol=None
@@ -72,22 +74,22 @@
 
     def connect(self)->bool:
         #make a connection and return 
         pass
 
 class IoXTransport:
     def __init__(self, transport_params):
-        if comm_params == None:
+        if transport_params == None:
             raise Exception ("Need communication parameters for TCP (host/port)")
 
         if not transport_params['mode']:
             raise Exception ("Missing communication mode")
 
         self.is_connected=False
-        self.params=transport.params
+        self.params=transport_params
         self.mode=self.params['mode']
 
     def getMode(self):
         return self.mode
 
     def getTransport(self):
```

### Comparing `ioxplugin-1.1.0/ioxplugin/log.py` & `ioxplugin-1.1.1/ioxplugin/log.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/main_gen.py` & `ioxplugin-1.1.1/ioxplugin/main_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/new_project.py` & `ioxplugin-1.1.1/ioxplugin/new_project.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/node_properties.py` & `ioxplugin-1.1.1/ioxplugin/node_properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,17 @@
                 if nls_np:
                     nls += f"\n{nls_np}"
             sts += "\n</sts>"
             return sts, nls
         except Exception as ex:
             LOGGER.critical(str(ex))
 
+    '''
+        Returns a dictory of the form {property_id, protocol_data_object}
+    '''
     def getProtocolData(self):
         out = {}
         for np in self.node_properties:
             node_property:NodePropertyDetails = self.node_properties[np]
             out[node_property.id] = node_property.protocol_data
 
         return out
```

### Comparing `ioxplugin-1.1.0/ioxplugin/nodedef.py` & `ioxplugin-1.1.1/ioxplugin/nodedef.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,19 +144,19 @@
                     "is_settable": False
                 }
             ],
             "commands": {
                 "accepts": [
                     {
                         "id": "discover",
-                        "name": "Discover"
+                        "name": "discover"
                     },
                     {
                         "id": "query",
-                        "name": "Query"
+                        "name": "query"
                     }
                 ],
                 "sends": []
                 }
            }
```

### Comparing `ioxplugin-1.1.0/ioxplugin/oauth_service.py` & `ioxplugin-1.1.1/ioxplugin/oauth_service.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/plugin.py` & `ioxplugin-1.1.1/ioxplugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/plugin_meta.py` & `ioxplugin-1.1.1/ioxplugin/plugin_meta.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/properties.py` & `ioxplugin-1.1.1/ioxplugin/properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/protocol.py` & `ioxplugin-1.1.1/ioxplugin/protocol.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/uom.py` & `ioxplugin-1.1.1/ioxplugin/uom.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin/validator.py` & `ioxplugin-1.1.1/ioxplugin/validator.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.1.0/ioxplugin.egg-info/PKG-INFO` & `ioxplugin-1.1.1/ioxplugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.1.0
+Version: 1.1.1
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.1.0/ioxplugin.egg-info/SOURCES.txt` & `ioxplugin-1.1.1/ioxplugin.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 ioxplugin/commands.py
 ioxplugin/editor.py
 ioxplugin/iox_controller_template.py
 ioxplugin/iox_main_template.py
 ioxplugin/iox_node_gen.py
 ioxplugin/iox_node_impl_gen.py
 ioxplugin/iox_profile.py
-ioxplugin/iox_to_modbus.py
 ioxplugin/iox_transport.py
 ioxplugin/log.py
 ioxplugin/main_gen.py
 ioxplugin/new_project.py
 ioxplugin/node_properties.py
 ioxplugin/nodedef.py
 ioxplugin/oauth_service.py
@@ -25,14 +24,12 @@
 ioxplugin/uom.py
 ioxplugin/validator.py
 ioxplugin.egg-info/PKG-INFO
 ioxplugin.egg-info/SOURCES.txt
 ioxplugin.egg-info/dependency_links.txt
 ioxplugin.egg-info/requires.txt
 ioxplugin.egg-info/top_level.txt
-tests/ModbusControllerNode.py
-tests/ModbusDeviceNode.py
 tests/ModbusProtocolHandler.py
 tests/__init__.py
 tests/modbus.py
 tests/test_ioxplugin.py
 tests/version.py
```

### Comparing `ioxplugin-1.1.0/setup.py` & `ioxplugin-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ioxplugin',
-    version='1.1.0',
+    version='1.1.1',
     packages=find_packages(),
     description='IoX Plugin Helper Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Michel Kohanim',
     author_email='support@universal-devices.com',
     url='https://github.com/universaldevices/ioxplugin.git',
```

### Comparing `ioxplugin-1.1.0/tests/modbus.py` & `ioxplugin-1.1.1/tests/modbus.py`

 * *Files identical despite different names*


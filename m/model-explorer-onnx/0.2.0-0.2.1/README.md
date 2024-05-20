# Comparing `tmp/model_explorer_onnx-0.2.0.tar.gz` & `tmp/model_explorer_onnx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.2.0.tar", last modified: Sun May 19 03:41:57 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.2.1.tar", last modified: Mon May 20 19:00:56 2024, max compression
```

## Comparing `model_explorer_onnx-0.2.0.tar` & `model_explorer_onnx-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:41:57.994183 model_explorer_onnx-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 03:41:52.000000 model_explorer_onnx-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-19 03:41:57.994183 model_explorer_onnx-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-19 03:41:52.000000 model_explorer_onnx-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-19 03:41:52.000000 model_explorer_onnx-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 03:41:57.994183 model_explorer_onnx-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:41:57.990183 model_explorer_onnx-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:41:57.994183 model_explorer_onnx-0.2.0/src/model_explorer_onnx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:41:57.994183 model_explorer_onnx-0.2.0/src/model_explorer_onnx/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 03:41:52.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-19 03:41:52.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx/bin/onnxvis.py
--rw-r--r--   0 runner    (1001) docker     (127)    19296 2024-05-19 03:41:52.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:41:57.994183 model_explorer_onnx-0.2.0/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-19 03:41:57.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-19 03:41:57.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:41:57.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-19 03:41:57.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-19 03:41:57.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 03:41:57.000000 model_explorer_onnx-0.2.0/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.076603 model_explorer_onnx-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.076603 model_explorer_onnx-0.2.1/src/model_explorer_onnx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/src/model_explorer_onnx/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx/bin/onnxvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21334 2024-05-20 19:00:52.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:00:56.080603 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 19:00:56.000000 model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.2.0/LICENSE` & `model_explorer_onnx-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.2.0/PKG-INFO` & `model_explorer_onnx-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.2.0
+Version: 0.2.1
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Keywords: onnx,model-explorer,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `model_explorer_onnx-0.2.0/README.md` & `model_explorer_onnx-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.2.0/pyproject.toml` & `model_explorer_onnx-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.2.0"
+version = "0.2.1"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 keywords = ["onnx", "model-explorer", "visualization"]
 classifiers = [
```

### Comparing `model_explorer_onnx-0.2.0/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.2.1/src/model_explorer_onnx/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,77 @@
 from __future__ import annotations
 
+import json
 import logging
 from typing import Any, Literal, Sequence
 
 import ml_dtypes
 import model_explorer
 import numpy as np
 import onnx
 from model_explorer import graph_builder
 from onnxscript import ir
 
 logger = logging.getLogger(__name__)
 
-_TENSOR_DISPLAY_LIMIT = 1024
 _DEFAULT_OPSET_VERSION = 18
 
 
-def display_tensor(tensor: ir.TensorProtocol | None) -> str:
+class Settings:
+    def __init__(self, const_element_count_limit: int = 1024, **_: Any):
+        self.const_element_count_limit: int = const_element_count_limit
+
+
+def _tensor_to_numpy(tensor: ir.TensorProtocol) -> np.ndarray:
+    array = tensor.numpy()
+    if tensor.dtype == ir.DataType.BFLOAT16:
+        array = array.view(ml_dtypes.bfloat16)
+    elif tensor.dtype == ir.DataType.FLOAT8E4M3FN:
+        array = array.view(ml_dtypes.float8_e4m3fn)
+    elif tensor.dtype == ir.DataType.FLOAT8E4M3FNUZ:
+        array = array.view(ml_dtypes.float8_e4m3fnuz)
+    elif tensor.dtype == ir.DataType.FLOAT8E5M2:
+        array = array.view(ml_dtypes.float8_e5m2)
+    elif tensor.dtype == ir.DataType.FLOAT8E5M2FNUZ:
+        array = array.view(ml_dtypes.float8_e5m2fnuz)
+    return array
+
+
+def display_tensor_repr(tensor: ir.TensorProtocol | None) -> str:
     if tensor is None:
         return "Data not available"
-    if tensor.size > _TENSOR_DISPLAY_LIMIT or isinstance(tensor, ir.ExternalTensor):
-        return str(tensor)
+    return str(tensor)
+
+
+def can_display_tensor_json(
+    tensor: ir.TensorProtocol | None, settings: Settings
+) -> bool:
+    if tensor is None:
+        return False
+    if tensor.size > settings.const_element_count_limit:
+        return False
+    if isinstance(tensor, ir.ExternalTensor):
+        return False
+    return True
+
+
+def display_tensor_json(tensor: ir.TensorProtocol | None, settings: Settings) -> str:
     try:
-        array = tensor.numpy()
-        if tensor.dtype == ir.DataType.BFLOAT16:
-            array = array.view(ml_dtypes.bfloat16)
-        elif tensor.dtype == ir.DataType.FLOAT8E4M3FN:
-            array = array.view(ml_dtypes.float8_e4m3fn)
-        elif tensor.dtype == ir.DataType.FLOAT8E4M3FNUZ:
-            array = array.view(ml_dtypes.float8_e4m3fnuz)
-        elif tensor.dtype == ir.DataType.FLOAT8E5M2:
-            array = array.view(ml_dtypes.float8_e5m2)
-        elif tensor.dtype == ir.DataType.FLOAT8E5M2FNUZ:
-            array = array.view(ml_dtypes.float8_e5m2fnuz)
-        return np.array2string(array, separator=",")
+        array = _tensor_to_numpy(tensor)
+        size_limit = settings.const_element_count_limit
+        if size_limit < 0 or size_limit > array.size:
+            # Use separators=(',', ':') to remove spaces
+            return json.dumps(array.tolist(), separators=(",", ":"))
+        # Show the first `size_limit` elements if the tensor is too large
+        return json.dumps(
+            (array.flatten())[:size_limit].tolist(), separators=(",", ":")
+        )
     except Exception as e:
-        logger.warning("Failed to display tensor: %s", e)
-    return str(tensor)
+        logger.warning("Failed to display tensor (%s): %s", tensor, e)
+    return ""
 
 
 def format_shape(shape: ir.ShapeProtocol | None) -> str:
     return str(shape) if shape is not None else "[?]"
 
 
 def format_type(type: ir.TypeProtocol | None) -> str:
@@ -173,19 +204,27 @@
             if (
                 param_name := get_node_output_param_name(schema, output_index)
             ) is not None:
                 set_attr(metadata, "param_name", param_name)
         node.outputsMetadata.append(metadata)
 
 
-def add_node_attrs(onnx_node: ir.Node, node: graph_builder.GraphNode) -> None:
+def add_node_attrs(
+    onnx_node: ir.Node, node: graph_builder.GraphNode, settings: Settings
+) -> None:
     for attr in onnx_node.attributes.values():
         if isinstance(attr, ir.Attr):
             if attr.type == ir.AttributeType.TENSOR:
-                attr_value = display_tensor(attr.value)
+                if can_display_tensor_json(attr.value, settings=settings):
+                    set_attr(
+                        node,
+                        "__value",
+                        display_tensor_json(attr.value, settings=settings),
+                    )
+                attr_value = display_tensor_repr(attr.value)
             elif onnx_node.op_type == "Cast" and attr.name == "to":
                 attr_value = str(ir.DataType(attr.value))
             else:
                 attr_value = str(attr.value)
             set_attr(node, attr.name, attr_value)
         elif isinstance(attr, ir.RefAttr):
             set_attr(node, attr.name, f"@{attr.ref_attr_name}")
@@ -245,14 +284,15 @@
 
 def create_node(
     onnx_node: ir.Node,
     graph_inputs: set[ir.Value],
     namespace: str,
     all_function_ids: set[ir.OperatorIdentifier],
     opset_version: int,
+    settings: Settings,
 ) -> graph_builder.GraphNode | None:
     """Create a GraphNode from an ONNX node.
 
     Args:
         onnx_node: The ONNX node to convert.
         graph_inputs: The set of graph inputs.
         namespace: The namespace of the node.
@@ -270,15 +310,15 @@
             namespace = namespace + "/" + "/".join(embedded_namespace)
     node = graph_builder.GraphNode(
         id=onnx_node.name,
         label=create_op_label(onnx_node.domain, onnx_node.op_type),
         namespace=namespace,
     )
     add_incoming_edges(onnx_node, node, graph_inputs)
-    add_node_attrs(onnx_node, node)
+    add_node_attrs(onnx_node, node, settings=settings)
     add_inputs_metadata(onnx_node, node, opset_version=opset_version)
     add_outputs_metadata(onnx_node, node, opset_version=opset_version)
     if onnx_node.op_identifier() in all_function_ids:
         node.subgraphIds.append(get_function_graph_name(onnx_node.op_identifier()))
     return node
 
 
@@ -359,27 +399,34 @@
 
 
 def add_initializers(
     graph: graph_builder.Graph,
     initializers: Sequence[ir.Value],
     namespace: str,
     all_nodes: dict[str, graph_builder.GraphNode],
+    settings: Settings,
 ) -> None:
     for initializer in initializers:
         if not initializer.name:
             logger.warning(
                 "Initializer does not have a name. Skipping: %s", initializer
             )
             continue
         initializer_node_name = get_initializer_node_name(initializer)
         if initializer_node_name in all_nodes:
             # The initializer is also a graph input. Fill in the missing metadata.
             node = all_nodes[initializer_node_name]
             metadata = node.outputsMetadata[0]
-            set_attr(metadata, "value", display_tensor(initializer.const_value))
+            if can_display_tensor_json(initializer.const_value, settings=settings):
+                set_attr(
+                    node,
+                    "__value",
+                    display_tensor_json(initializer.const_value, settings=settings),
+                )
+            set_attr(metadata, "value", display_tensor_repr(initializer.const_value))
             continue
         node = graph_builder.GraphNode(
             id=initializer_node_name,
             label="Initializer",
             namespace=get_constant_namespace(initializer, namespace),
         )
         # Add metadata for the output tensor
@@ -388,26 +435,33 @@
                 "Initializer %s does not have a const value. Skipping.", initializer
             )
             graph.nodes.append(node)
             continue
         metadata = graph_builder.MetadataItem(id="0", attrs=[])
         set_attr(metadata, "__tensor_tag", initializer.name or "")
         set_type_shape_metadata(metadata, initializer.const_value)
-        set_attr(metadata, "value", display_tensor(initializer.const_value))
+        if can_display_tensor_json(initializer.const_value, settings=settings):
+            set_attr(
+                node,
+                "__value",
+                display_tensor_json(initializer.const_value, settings=settings),
+            )
+        set_attr(metadata, "value", display_tensor_repr(initializer.const_value))
         # Note if the initializer is unused
         if not initializer.uses():
             set_attr(metadata, "unused", "True")
         node.outputsMetadata.append(metadata)
         graph.nodes.append(node)
 
 
 def create_graph(
     onnx_graph: ir.Graph | ir.Function,
     all_function_ids: set[ir.OperatorIdentifier],
     opset_version: int,
+    settings: Settings,
 ) -> graph_builder.Graph | None:
     if isinstance(onnx_graph, ir.Function):
         graph_name = get_function_graph_name(onnx_graph.identifier())
     elif onnx_graph.name is None:
         logger.warning("Graph does not have a name. skipping graph: %s", onnx_graph)
         return None
     else:
@@ -422,27 +476,29 @@
             onnx_node.name = f"<node_{i}>"
         node = create_node(
             onnx_node,
             graph_inputs,  # type: ignore
             namespace=graph_name,
             all_function_ids=all_function_ids,
             opset_version=opset_version,
+            settings=settings,
         )  # type: ignore
         if node is None:
             continue
         graph.nodes.append(node)
         all_nodes[node.id] = node
 
     # Add initializers
     if isinstance(onnx_graph, ir.Graph):
         add_initializers(
             graph,
             list(onnx_graph.initializers.values()),
             graph_name,
             all_nodes=all_nodes,
+            settings=settings,
         )
 
     # Add outputs
     add_graph_io(graph, onnx_graph.outputs, type_="Output", all_nodes=all_nodes)
     return graph
 
 
@@ -456,15 +512,15 @@
         source_repo="https://github.com/justinchuby/model_explorer_onnx",
         fileExts=["onnx", "onnxtext", "onnxtxt", "textproto", "onnxjson", "json"],
     )
 
     def convert(
         self, model_path: str, settings: dict[str, Any]
     ) -> model_explorer.ModelExplorerGraphs:
-        del settings  # Unused
+        parsed_settings = Settings(**settings)
 
         # Do not load external data because the model file is copied to a temporary location
         # and the external data paths are not valid anymore.
         onnx_model = onnx.load(model_path, load_external_data=False)
         try:
             onnx_model = onnx.shape_inference.infer_shapes(onnx_model, data_prop=True)
         except Exception as e:
@@ -485,19 +541,25 @@
         if model.graph.name is None:
             model.graph.name = "<main>"
             logger.warning(
                 "Main graph of ONNX file '%s' does not have a name. Set name to '<main>'",
                 model_path,
             )
         main_graph = create_graph(
-            model.graph, all_function_ids, opset_version=opset_version
+            model.graph,
+            all_function_ids,
+            opset_version=opset_version,
+            settings=parsed_settings,
         )
         assert main_graph is not None, "Bug: Main graph should not be None"
         graphs.append(main_graph)
 
         for function in model.functions.values():
             function_graph = create_graph(
-                function, all_function_ids, opset_version=opset_version
+                function,
+                all_function_ids,
+                opset_version=opset_version,
+                settings=parsed_settings,
             )
             assert function_graph is not None
             graphs.append(function_graph)
         return {"graphs": graphs}
```

### Comparing `model_explorer_onnx-0.2.0/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.2.1/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.2.0
+Version: 0.2.1
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Keywords: onnx,model-explorer,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


# Comparing `tmp/hugr-0.2.0a1.tar.gz` & `tmp/hugr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugr-0.2.0a1.tar", max compression
+gzip compressed data, was "hugr-0.2.1.tar", max compression
```

## Comparing `hugr-0.2.0a1.tar` & `hugr-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1446 2024-05-13 10:18:47.630760 hugr-0.2.0a1/README.md
--rw-r--r--   0        0        0     1217 2024-05-13 10:18:47.630760 hugr-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0      234 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/py.typed
--rw-r--r--   0        0        0       62 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/__init__.py
--rw-r--r--   0        0        0    15478 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/ops.py
--rw-r--r--   0        0        0     1392 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/serial_hugr.py
--rw-r--r--   0        0        0      971 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/testing_hugr.py
--rw-r--r--   0        0        0     9457 2024-05-13 10:18:47.630760 hugr-0.2.0a1/src/hugr/serialization/tys.py
--rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 hugr-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1446 2024-05-20 13:15:05.927139 hugr-0.2.1/README.md
+-rw-r--r--   0        0        0     1215 2024-05-20 13:15:05.927139 hugr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-05-20 13:15:05.931139 hugr-0.2.1/src/hugr/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:15:05.931139 hugr-0.2.1/src/hugr/py.typed
+-rw-r--r--   0        0        0       62 2024-05-20 13:15:05.931139 hugr-0.2.1/src/hugr/serialization/__init__.py
+-rw-r--r--   0        0        0    15478 2024-05-20 13:15:05.931139 hugr-0.2.1/src/hugr/serialization/ops.py
+-rw-r--r--   0        0        0     1468 2024-05-20 13:15:05.931139 hugr-0.2.1/src/hugr/serialization/serial_hugr.py
+-rw-r--r--   0        0        0      971 2024-05-20 13:15:05.931139 hugr-0.2.1/src/hugr/serialization/testing_hugr.py
+-rw-r--r--   0        0        0     9457 2024-05-20 13:15:05.931139 hugr-0.2.1/src/hugr/serialization/tys.py
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 hugr-0.2.1/PKG-INFO
```

### Comparing `hugr-0.2.0a1/README.md` & `hugr-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hugr-0.2.0a1/pyproject.toml` & `hugr-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
 ]
 name = "hugr"
-version = "0.2.0a1"
+version = "0.2.1"
 description = "Quantinuum's common representation for quantum programs"
 #keywords = []
 authors = ["TKET development team <tket-support@cambridgequantum.com>"]
 maintainers = ["TKET development team <tket-support@cambridgequantum.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/CQCL/hugr"
```

### Comparing `hugr-0.2.0a1/src/hugr/serialization/ops.py` & `hugr-0.2.1/src/hugr/serialization/ops.py`

 * *Files identical despite different names*

### Comparing `hugr-0.2.0a1/src/hugr/serialization/serial_hugr.py` & `hugr-0.2.1/src/hugr/serialization/serial_hugr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Any, Literal
 
-from pydantic import BaseModel, Field, ConfigDict
+from pydantic import Field, ConfigDict
 
 from .ops import NodeID, OpType, classes as ops_classes
-from .tys import model_rebuild
+from .tys import model_rebuild, ConfiguredBaseModel
 import hugr
 
 Port = tuple[NodeID, int | None]  # (node, offset)
 Edge = tuple[Port, Port]
 
 
-class SerialHugr(BaseModel):
+class SerialHugr(ConfiguredBaseModel):
     """A serializable representation of a Hugr."""
 
     version: Literal["v1"] = "v1"
     nodes: list[OpType]
     edges: list[Edge]
+    metadata: list[dict[str, Any] | None] | None = None
     encoder: str | None = Field(
         default=None, description="The name of the encoder used to generate the Hugr."
     )
 
     def to_json(self) -> str:
         """Return a JSON representation of the Hugr."""
         self.encoder = f"hugr-py v{hugr.__version__}"
```

### Comparing `hugr-0.2.0a1/src/hugr/serialization/testing_hugr.py` & `hugr-0.2.1/src/hugr/serialization/testing_hugr.py`

 * *Files identical despite different names*

### Comparing `hugr-0.2.0a1/src/hugr/serialization/tys.py` & `hugr-0.2.1/src/hugr/serialization/tys.py`

 * *Files identical despite different names*

### Comparing `hugr-0.2.0a1/PKG-INFO` & `hugr-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugr
-Version: 0.2.0a1
+Version: 0.2.1
 Summary: Quantinuum's common representation for quantum programs
 Home-page: https://github.com/CQCL/hugr
 License: Apache-2.0
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 Maintainer: TKET development team
 Maintainer-email: tket-support@cambridgequantum.com
```


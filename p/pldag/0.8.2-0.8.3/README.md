# Comparing `tmp/pldag-0.8.2.tar.gz` & `tmp/pldag-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.2.tar", max compression
+gzip compressed data, was "pldag-0.8.3.tar", max compression
```

## Comparing `pldag-0.8.2.tar` & `pldag-0.8.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.2/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.2/README.md
--rw-r--r--   0        0        0    38933 2024-05-14 12:33:16.562246 pldag-0.8.2/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.2/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.2/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-05-14 12:33:36.777304 pldag-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.3/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.3/README.md
+-rw-r--r--   0        0        0    44814 2024-05-20 12:18:33.057582 pldag-0.8.3/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.3/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.3/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-05-20 12:31:45.429037 pldag-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.3/PKG-INFO
```

### Comparing `pldag-0.8.2/LICENSE` & `pldag-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.2/README.md` & `pldag-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.2/pldag/__init__.py` & `pldag-0.8.3/pldag/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from hashlib import sha1
 from itertools import groupby, repeat, starmap
 from functools import partial, lru_cache
-from typing import Dict, List, Set, Optional
+from typing import Dict, List, Set, Optional, Callable, Any
 from graphlib import TopologicalSorter
 
 from enum import Enum
 
 class NoSolutionsException(Exception):
     pass
 
@@ -310,24 +310,25 @@
             )
         )
     
     def id_from_alias(self, alias: str) -> Optional[str]:
         """Get the ID of the given alias"""
         return self._amap.get(alias, None)
     
-    def id_to_alias(self, id: str) -> List[str]:
+    def id_to_alias(self, id: str) -> Optional[str]:
         """Get the aliases of the given ID"""
-        return list(
+        return next(
             map(
                 lambda x: x[0],
                 filter(
                     lambda x: x[1] == id,
                     self._amap.items(),
                 )
-            )
+            ),
+            None
         )
     
     def copy(self) -> "PLDAG":
         """Copy the model"""
         model = PLDAG()
         model._amat = self._amat.copy()
         model._wmat = self._wmat.copy()
@@ -1088,8 +1089,172 @@
                             lambda i: complex(i,i),
                             solution
                         )
                     )
                 ),
                 solutions
             )
-        )
+        )
+    
+from dataclasses import dataclass, field
+    
+@dataclass
+class Variable:
+    id: str
+    bound: complex
+    properties: dict = field(default_factory=dict)
+    alias: Optional[str] = None
+
+@dataclass
+class Solution:
+    
+    variables: List[Variable]
+
+    def __getitem__(self, key: str) -> Variable:
+        return next(
+            filter(
+                lambda x: x.id == key,
+                self.variables
+            )
+        )
+    
+    def find(self, predicate: Callable[[Variable], bool]) -> List[str]:
+        return list(
+            filter(
+                predicate,
+                self.variables
+            )
+        )
+
+class Puan(PLDAG):
+
+    def __init__(self):
+        super().__init__()
+        self.data: dict = {}
+
+    def set_meta(self, id: str, props: dict):
+        self.data.setdefault(id, {}).update(props)
+
+    def del_meta(self, id: str, key: str):
+        self.data[id].pop(key, None)
+
+    def set_primitive(self, id: str, properties: dict = {}, bound: complex = complex(0,1)) -> str:
+        self.set_meta(id, properties)
+        return super().set_primitive(id, bound)
+    
+    def set_primitives(self, ids: List[str], properties: dict = {}, bound: complex = complex(0,1)) -> List[str]:
+        return list(
+            map(
+                lambda x: self.set_primitive(x, properties, bound),
+                ids
+            )
+        )
+
+    def set_gelineq(self, children: list, bias: int, negate: bool = False, alias: Optional[str] = None, weights: Optional[List[int]] = None, properties: dict = {}) -> str:
+        id = super().set_gelineq(children, bias, negate, alias, weights)
+        self.set_meta(id, properties)
+        return id
+    
+    def set_atmost(self, children: List[str], value: int, alias: Optional[str] = None, weights: Optional[List[int]] = None, properties: dict = {}) -> str:
+        id = super().set_atmost(children, value, alias, weights)
+        self.set_meta(id, properties)
+        return id
+    
+    def set_atleast(self, children: List[str], value: int, alias: Optional[str] = None, weights: Optional[List[int]] = None, properties: dict = {}) -> str:
+        id = super().set_atleast(children, value, alias, weights)
+        self.set_meta(id, properties)
+        return id
+    
+    def set_and(self, children: List[str], alias: Optional[str] = None, properties: dict = {}) -> str:
+        id = super().set_and(children, alias)
+        self.set_meta(id, properties)
+        return id
+    
+    def set_or(self, children: List[str], alias: Optional[str] = None, properties: dict = {}) -> str:
+        id = super().set_or(children, alias)
+        self.set_meta(id, properties)
+        return id
+    
+    def set_xor(self, children: List[str], alias: Optional[str] = None, properties: dict = {}) -> str:
+        id = super().set_xor(children, alias)
+        self.set_meta(id, properties)
+        return id
+    
+    def set_xnor(self, children: List[str], alias: Optional[str] = None, properties: dict = {}) -> str:
+        id = super().set_xnor(children, alias)
+        self.set_meta(id, properties)
+        return id
+    
+    def set_equal(self, references: List[str], alias: Optional[str] = None, properties: dict = {}) -> str:
+        id = super().set_equal(references, alias)
+        self.set_meta(id, properties)
+        return id
+    
+    def set_imply(self, antecedent: str, consequent: str, properties: dict = {}) -> str:
+        id = super().set_imply(antecedent, consequent)
+        self.set_meta(id, properties)
+        return id
+    
+    def find(self, predicate: Callable[[str, Any], bool]) -> Set[str]:
+        return set(
+            map(
+                lambda x: x[0],
+                filter(
+                    lambda x: any(
+                        starmap(
+                            predicate,
+                            x[1].items()
+                        )
+                    ),
+                    self.data.items()
+                )
+            )
+        )
+    
+    def solve(self, objectives: List[dict], assume: Dict[str, complex], solver: Solver) -> List[dict]:
+        return list(
+            map(
+                lambda solution: Solution(
+                    variables=list(
+                        starmap(
+                            lambda k,v: Variable(k, v, self.data.get(k, {}), self.id_to_alias(k) or None),
+                            solution.items()
+                        )
+                    )
+                ),
+                super().solve(objectives, assume, solver)
+            )
+        )
+    
+    def propagate(self, query: dict = {}, freeze: bool = True) -> Solution:
+        return Solution(
+            variables=list(
+                starmap(
+                    lambda k,v: Variable(k, v, self.data.get(k, {}), self.id_to_alias(k) or None),
+                    super().propagate(query, freeze).items()
+                )
+            )
+        )
+    
+    @staticmethod
+    def from_super(super_model: PLDAG) -> 'Puan':
+        new_model = Puan()
+        new_model._amat = super_model._amat
+        new_model._wmat = super_model._wmat
+        new_model._dvec = super_model._dvec
+        new_model._bvec = super_model._bvec
+        new_model._nvec = super_model._nvec
+        new_model._cvec = super_model._cvec
+        new_model._imap = super_model._imap
+        new_model._amap = super_model._amap
+        return new_model
+    
+    def sub(self, roots: List[str], max_iterations: int = 1000) -> 'Puan':
+        new_model = self.from_super(super().sub(roots, max_iterations))
+        new_model.data = dict(filter(lambda k: k[0] in new_model._imap, self.data.items()))
+        return new_model
+        
+    def cut(self, cuts: Dict[str, str]) -> "Puan":
+        new_model = self.from_super(super().cut(cuts))
+        new_model.data = dict(filter(lambda k: k[0] in new_model._imap, self.data))
+        return new_model
+
```

### Comparing `pldag-0.8.2/pldag/solver/glpk_solver.py` & `pldag-0.8.3/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.2/PKG-INFO` & `pldag-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.2
+Version: 0.8.3
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


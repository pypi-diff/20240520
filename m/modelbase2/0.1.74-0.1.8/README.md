# Comparing `tmp/modelbase2-0.1.74.tar.gz` & `tmp/modelbase2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbase2-0.1.74.tar", max compression
+gzip compressed data, was "modelbase2-0.1.8.tar", max compression
```

## Comparing `modelbase2-0.1.74.tar` & `modelbase2-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35079 2024-05-20 01:08:14.240697 modelbase2-0.1.74/LICENSE
--rw-r--r--   0        0        0     2666 2024-05-20 01:08:14.241696 modelbase2-0.1.74/pyproject.toml
--rw-r--r--   0        0        0      723 2024-05-20 01:08:14.241696 modelbase2-0.1.74/src/modelbase2/__init__.py
--rw-r--r--   0        0        0      690 2024-05-20 01:08:14.241696 modelbase2-0.1.74/src/modelbase2/core/__init__.py
--rw-r--r--   0        0        0     4564 2024-05-20 01:08:14.241696 modelbase2-0.1.74/src/modelbase2/core/algebraic_module_container.py
--rw-r--r--   0        0        0     4669 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/core/constant_container.py
--rw-r--r--   0        0        0     2452 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/core/data.py
--rw-r--r--   0        0        0      918 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/core/name_container.py
--rw-r--r--   0        0        0     4860 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/core/reaction_container.py
--rw-r--r--   0        0        0      857 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/core/utils.py
--rw-r--r--   0        0        0      736 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/core/variable_container.py
--rw-r--r--   0        0        0      217 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/ode/__init__.py
--rw-r--r--   0        0        0     2239 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/ode/integrator.py
--rw-r--r--   0        0        0     8450 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/ode/mca.py
--rw-r--r--   0        0        0    15618 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/ode/model.py
--rw-r--r--   0        0        0     4880 2024-05-20 01:08:14.242697 modelbase2-0.1.74/src/modelbase2/ode/simulator.py
--rw-r--r--   0        0        0        0 2024-05-20 01:08:14.273697 modelbase2-0.1.74/src/modelbase2/py.typed
--rw-r--r--   0        0        0      407 2024-05-20 01:08:14.243697 modelbase2-0.1.74/src/modelbase2/types.py
--rw-r--r--   0        0        0        0 2024-05-20 01:08:14.274696 modelbase2-0.1.74/src/modelbase2/utils/__init__.py
--rw-r--r--   0        0        0    12357 2024-05-20 01:08:14.243697 modelbase2-0.1.74/src/modelbase2/utils/plotting.py
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 modelbase2-0.1.74/setup.py
--rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 modelbase2-0.1.74/PKG-INFO
+-rw-r--r--   0        0        0    35079 2022-11-21 09:18:31.668037 modelbase2-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2596 2022-11-21 09:18:31.670037 modelbase2-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      723 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/__init__.py
+-rw-r--r--   0        0        0      690 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/__init__.py
+-rw-r--r--   0        0        0     4493 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/algebraic_module_container.py
+-rw-r--r--   0        0        0     4609 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/constant_container.py
+-rw-r--r--   0        0        0     2452 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/data.py
+-rw-r--r--   0        0        0      889 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/name_container.py
+-rw-r--r--   0        0        0     4832 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/reaction_container.py
+-rw-r--r--   0        0        0      857 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/utils.py
+-rw-r--r--   0        0        0      736 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/core/variable_container.py
+-rw-r--r--   0        0        0      217 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/__init__.py
+-rw-r--r--   0        0        0     2259 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/integrator.py
+-rw-r--r--   0        0        0     8378 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/mca.py
+-rw-r--r--   0        0        0    15494 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/model.py
+-rw-r--r--   0        0        0     4784 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/ode/simulator.py
+-rw-r--r--   0        0        0        0 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/py.typed
+-rw-r--r--   0        0        0      407 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/types.py
+-rw-r--r--   0        0        0        0 2022-11-21 09:18:31.670037 modelbase2-0.1.8/src/modelbase2/utils/__init__.py
+-rw-r--r--   0        0        0    12258 2022-11-21 09:18:31.671037 modelbase2-0.1.8/src/modelbase2/utils/plotting.py
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 modelbase2-0.1.8/setup.py
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 modelbase2-0.1.8/PKG-INFO
```

### Comparing `modelbase2-0.1.74/LICENSE` & `modelbase2-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.74/pyproject.toml` & `modelbase2-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelbase2"
-version = "0.1.74"
+version = "0.1.8"
 description = "A package to build metabolic models"
 license = "GPL-3.0-or-later"
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>", "Oliver Ebenhöh <oliver.ebenhoeh@hhu.de>"]
 maintainers = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 repository = "https://gitlab.com/qtb-hhu/modelbase-software"
 documentation = "https://modelbase.readthedocs.io/en/latest/"
 keywords = ["modelling", "ode", "metabolic"]
@@ -23,15 +23,15 @@
         "Operating System :: Unix",
         "Operating System :: MacOS",
         "Operating System :: OS Independent",
     ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9.0,<3.11"
 matplotlib = "^3.5.0"
 numpy = "^1.21.4"
 pandas = "^1.3.4"
 python-libsbml = "^5.19.2"
 scipy = "^1.7.2"
 black = "^22.3.0"
 sympy = "^1.9"
@@ -56,17 +56,14 @@
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
 line-length = 90
 target-version = ['py310']
 
-[tool.bandit]
-skips = ["B101", "B301", "B403", "B404", "B603", "B607"]
-
 [tool.isort]
 profile = "black"
 src_paths = ["src", "tests"]
 no_sections = true
 honor_noqa = true
 
 [tool.mypy]
@@ -74,15 +71,15 @@
 warn_return_any = true
 warn_unused_configs = true
 ignore_missing_imports = true
 disallow_untyped_defs = true
 exclude = "tests/*.py"
 
 [tool.pylint.messages_control]
-max-line-length = 100
+max-line-length = 120
 disable = [
   "no-self-use",
   "too-many-instance-attributes",
   "too-many-arguments",
   "too-many-locals",
   "too-many-branches",
   "too-many-public-methods",
```

### Comparing `modelbase2-0.1.74/src/modelbase2/__init__.py` & `modelbase2-0.1.8/src/modelbase2/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 __all__ = [
     "AlgebraicModule",
-    "Assimulo",
     "Constant",
     "DerivedConstant",
     "DerivedStoichiometry",
-    "Model",
     "Reaction",
-    "Simulator",
     "Variable",
+    "Assimulo",
+    "Model",
+    "Simulator",
     "mca",
 ]
 
 import logging
 from .core.data import (
     AlgebraicModule,
     Constant,
```

### Comparing `modelbase2-0.1.74/src/modelbase2/core/__init__.py` & `modelbase2-0.1.8/src/modelbase2/core/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 __all__ = [
-    "AlgebraicModule",
     "AlgebraicModuleContainer",
-    "Constant",
     "ConstantContainer",
+    "AlgebraicModule",
+    "Constant",
     "DerivedConstant",
     "DerivedStoichiometry",
-    "NameContainer",
     "Reaction",
-    "ReactionContainer",
     "Variable",
+    "NameContainer",
+    "ReactionContainer",
     "VariableContainer",
 ]
 
 from .algebraic_module_container import AlgebraicModuleContainer
 from .constant_container import ConstantContainer
 from .data import (
     AlgebraicModule,
```

### Comparing `modelbase2-0.1.74/src/modelbase2/core/algebraic_module_container.py` & `modelbase2-0.1.8/src/modelbase2/core/algebraic_module_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
 import logging
-from ..types import Array
+import numpy as np
 from .data import AlgebraicModule, ModuleFunction
 from dataclasses import dataclass, field
 from queue import Empty, SimpleQueue
 from typing import Iterable, Iterator, Optional, cast
+from ..types import Array
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class AlgebraicModuleContainer:
     modules: dict[str, AlgebraicModule] = field(default_factory=dict)
     module_order: list[str] = field(default_factory=list)
 
     def __iter__(self) -> Iterator[AlgebraicModule]:
         return iter(self.modules.values())
 
-    def _sort_algebraic_modules(
-        self, available_args: set[str], max_iterations: int = 10_000
-    ) -> None:
+    def _sort_algebraic_modules(self, available_args: set[str], max_iterations: int = 10_000) -> None:
         module_order = []
         modules_to_sort: SimpleQueue[tuple[str, AlgebraicModule]] = SimpleQueue()
         for k, v in self.modules.items():
             modules_to_sort.put((k, v))
 
         last_name = None
         i = 0
@@ -46,19 +45,15 @@
             if i > max_iterations:
                 raise ValueError(
                     "Exceeded max iterations on algebraic module sorting. Check if there are circular references."
                 )
         self.module_order = module_order
 
     def get_derived_variables(self) -> list[str]:
-        return [
-            variable
-            for module in self.modules.values()
-            for variable in module.derived_variables
-        ]
+        return [variable for module in self.modules.values() for variable in module.derived_variables]
 
     def add(
         self,
         module: AlgebraicModule,
         available_args: set[str],
         sort_modules: bool,
     ) -> None:
@@ -117,14 +112,12 @@
         args: dict[str, Array],
     ) -> dict[str, Array]:
         derived_variables: dict[str, Array] = {}
         for name in self.module_order:
             module = self.modules[name]
             # values = np.array(module.function(*(args[arg] for arg in module.args)), dtype=float)
             # values = values.reshape((len(module.derived_variables), -1))
-            _values = cast(
-                Iterable[Array], module.function(*(args[arg] for arg in module.args))
-            )
+            _values = cast(Iterable[Array], module.function(*(args[arg] for arg in module.args)))
             values = dict(zip(module.derived_variables, _values))
             derived_variables |= values
             args |= values
         return derived_variables
```

### Comparing `modelbase2-0.1.74/src/modelbase2/core/constant_container.py` & `modelbase2-0.1.8/src/modelbase2/core/constant_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 
     def remove_basic(self, name: str) -> None:
         del self.constants[name]
         del self.values[name]
 
     def update_basic(self, name: str, value: float, update_derived: bool = True) -> None:
         if name not in self.constants:
-            raise KeyError(
-                f"Constant {name} is not in the model. You have to add it first"
-            )
+            raise KeyError(f"Constant {name} is not in the model. You have to add it first")
         self.constants[name].value = value
         self.values[name] = value
         if name in self._derived_from_constants and update_derived:
             self._update_derived_constant_values()
 
     ###############################################################################
     # Derived
@@ -78,17 +76,15 @@
                     "Check if there are circular references."
                 )
         self._derived_constant_order = order
 
     def _update_derived_constant_values(self) -> None:
         for name in self._derived_constant_order:
             derived_constant = self.derived_constants[name]
-            value = derived_constant.function(
-                *(self.values[i] for i in derived_constant.args)
-            )
+            value = derived_constant.function(*(self.values[i] for i in derived_constant.args))
             self.values[name] = value
 
     def add_derived(self, constant: DerivedConstant, update_derived: bool = True) -> None:
         name = constant.name
         self.derived_constants[name] = constant
         for arg in constant.args:
             self._derived_from_constants.add(arg)
```

### Comparing `modelbase2-0.1.74/src/modelbase2/core/data.py` & `modelbase2-0.1.8/src/modelbase2/core/data.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.74/src/modelbase2/core/name_container.py` & `modelbase2-0.1.8/src/modelbase2/core/name_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 
 @dataclass
 class NameContainer:
     names: dict[str, str] = field(default_factory=dict)
 
     def add(self, name: str, element_type: str) -> None:
         if (old_type := self.names.get(name)) is not None:
-            raise KeyError(
-                f"Cannot add {element_type} {name}, as there already exists a {old_type} with that name."
-            )
+            raise KeyError(f"Cannot add {element_type} {name}, as there already exists a {old_type} with that name.")
 
         logger.info(f"Adding name {name}")
         self.names[name] = element_type
 
     def remove(self, name: str) -> None:
+
         logger.info(f"Removing name {name}")
         del self.names[name]
 
     def require_multiple(self, names: Iterable[str]) -> None:
         if bool(difference := set(names).difference(self.names)):
             raise KeyError(f"Names '{', '.join(difference)}' are missing.")
```

### Comparing `modelbase2-0.1.74/src/modelbase2/core/reaction_container.py` & `modelbase2-0.1.8/src/modelbase2/core/reaction_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 from __future__ import annotations
 
 import logging
 import numpy as np
 import pandas as pd
-from ..types import Array
 from .data import DerivedStoichiometry, RateFunction, Reaction, StoichiometryByVariable
 from dataclasses import dataclass, field
 from typing import Optional
+from ..types import Array
 
 logger = logging.getLogger()
 
 
 @dataclass
 class ReactionContainer:
     reactions: dict[str, Reaction] = field(default_factory=dict)
-    stoichiometries_by_variables: dict[str, StoichiometryByVariable] = field(
-        default_factory=dict
-    )
+    stoichiometries_by_variables: dict[str, StoichiometryByVariable] = field(default_factory=dict)
 
     def set_stoichiometry(self, variable: str, reaction: str, factor: float) -> None:
         self.stoichiometries_by_variables.setdefault(variable, {})[reaction] = factor
 
     def update_stoichiometry(self, name: str, reaction: Reaction) -> None:
         for variable, factor in reaction.stoichiometry.items():
             self.set_stoichiometry(variable, name, factor)
 
-    def update_derived_stoichiometry(
-        self, name: str, reaction: Reaction, constants: dict[str, float]
-    ) -> None:
+    def update_derived_stoichiometry(self, name: str, reaction: Reaction, constants: dict[str, float]) -> None:
         for variable, derived_stoich in reaction.derived_stoichiometry.items():
             factor = derived_stoich.function(*(constants[i] for i in derived_stoich.args))
             self.set_stoichiometry(variable, name, factor)
 
     def update_derived_stoichiometries(self, constants: dict[str, float]) -> None:
         for name, reaction in self.reactions.items():
             self.update_derived_stoichiometry(name, reaction, constants)
```

### Comparing `modelbase2-0.1.74/src/modelbase2/core/utils.py` & `modelbase2-0.1.8/src/modelbase2/core/utils.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.74/src/modelbase2/core/variable_container.py` & `modelbase2-0.1.8/src/modelbase2/core/variable_container.py`

 * *Files identical despite different names*

### Comparing `modelbase2-0.1.74/src/modelbase2/ode/integrator.py` & `modelbase2-0.1.8/src/modelbase2/ode/integrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import numpy as np
-from ..types import Array
+import pandas as pd
 from assimulo.problem import Explicit_Problem  # type: ignore
 from assimulo.solvers import CVode  # type: ignore
 from assimulo.solvers.sundials import CVodeError  # type: ignore
 from dataclasses import dataclass
 from typing import Callable, Optional, cast
+from ..types import Array
 
 
 @dataclass
 class AssmimuloSettings:
     atol: float = 1e-8
     rtol: float = 1e-8
     maxnef: int = 4
```

### Comparing `modelbase2-0.1.74/src/modelbase2/ode/mca.py` & `modelbase2-0.1.8/src/modelbase2/ode/mca.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,15 @@
     displacement: float = _DISPLACEMENT,
 ) -> DataFrame:
     """Get sensitivity of all rates to a change of the concentration of multiple variables.
 
     Also called epsilon-elasticities. Not in steady state!
     """
     stoichiometries = m.get_stoichiometries().columns
-    elasticities = np.full(
-        shape=(len(variables), len(stoichiometries)), fill_value=np.nan
-    )
+    elasticities = np.full(shape=(len(variables), len(stoichiometries)), fill_value=np.nan)
     for i, variable in enumerate(variables):
         elasticities[i] = get_variable_elasticity(
             m=m,
             variable=variable,
             y=y,
             displacement=displacement,
         )
@@ -103,17 +101,15 @@
     displacement: float = _DISPLACEMENT,
 ) -> DataFrame:
     """Get sensitivity of all rates to a change of multiple constant values.
 
     Also called pi-elasticities. Not in steady state!
     """
     stoichiometries = m.get_stoichiometries().columns
-    elasticities = np.full(
-        shape=(len(constants), len(stoichiometries)), fill_value=np.nan
-    )
+    elasticities = np.full(shape=(len(constants), len(stoichiometries)), fill_value=np.nan)
     for i, constant in enumerate(constants):
         elasticities[i] = get_constant_elasticity(
             m=m,
             constant=constant,
             y=y,
             displacement=displacement,
         )
@@ -154,20 +150,16 @@
         ss.append(np.fromiter(y_full.values(), dtype="float"))
         fluxes.append(m.get_fluxes(y_full, return_type="array"))
 
     conc_resp_coef = (ss[0] - ss[1]) / (2 * displacement * old_value)
     flux_resp_coef = (fluxes[0] - fluxes[1]) / (2 * displacement * old_value)
 
     return (
-        pd.Series(conc_resp_coef * y_ss_norm, index=list(y_full.keys())).replace(
-            [np.inf, -np.inf], np.nan
-        ),
-        pd.Series(flux_resp_coef * fluxes_norm, index=list(m.reactions)).replace(
-            [np.inf, -np.inf], np.nan
-        ),
+        pd.Series(conc_resp_coef * y_ss_norm, index=list(y_full.keys())).replace([np.inf, -np.inf], np.nan),
+        pd.Series(flux_resp_coef * fluxes_norm, index=list(m.reactions)).replace([np.inf, -np.inf], np.nan),
     )
 
 
 def get_response_coefficients(
     m: Model,
     constants: list[str],
     y0: dict[str, float],
```

### Comparing `modelbase2-0.1.74/src/modelbase2/ode/model.py` & `modelbase2-0.1.8/src/modelbase2/ode/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,25 +58,21 @@
             while True:
                 try:
                     name, args = to_sort.get_nowait()
                     print(name, args)
                 except Empty:
                     break
 
-            raise ValueError(
-                "Exceeded max iterations on sorting. Check if there are circular references."
-            )
+            raise ValueError("Exceeded max iterations on sorting. Check if there are circular references.")
     return order
 
 
 @dataclass
 class Model:
-    _algebraic_modules: AlgebraicModuleContainer = field(
-        default_factory=AlgebraicModuleContainer
-    )
+    _algebraic_modules: AlgebraicModuleContainer = field(default_factory=AlgebraicModuleContainer)
     _variables: VariableContainer = field(default_factory=VariableContainer)
     _constants: ConstantContainer = field(default_factory=ConstantContainer)
     _reactions: ReactionContainer = field(default_factory=ReactionContainer)
     _names: NameContainer = field(default_factory=NameContainer)
 
     def __add__(self, other: "Model") -> "Model":
         for name, variable in other.variables.items():
@@ -310,17 +306,15 @@
         old_module = self.remove_algebraic_module(name)
         if function is None:
             function = old_module.function
         if derived_variables is None:
             derived_variables = old_module.derived_variables
         if args is None:
             args = old_module.args
-        self.add_algebraic_module(
-            AlgebraicModule(name, function, derived_variables, args)
-        )
+        self.add_algebraic_module(AlgebraicModule(name, function, derived_variables, args))
 
         self._algebraic_modules.update(
             name,
             function,
             derived_variables,
             args,
             self._get_available_args(),
@@ -380,17 +374,15 @@
         return list(rhs.values())
 
     def _get_all_args(self, variables: dict[str, float], time: float) -> dict[str, float]:
         args = variables | self.constant_values | {"time": time}
         args |= self._algebraic_modules.get_values_float(args)
         return args
 
-    def get_derived_variables(
-        self, variables: dict[str, float], time: float = 0.0
-    ) -> dict[str, float]:
+    def get_derived_variables(self, variables: dict[str, float], time: float = 0.0) -> dict[str, float]:
         args = variables | self.constant_values | {"time": time}
         return self._algebraic_modules.get_values_float(args)
 
     @overload
     def get_fluxes(
         self,
         variables: dict[str, float],
@@ -439,17 +431,15 @@
         elif return_type == "series":
             return pd.Series(fluxes_dict)
         elif return_type == "array":
             return np.fromiter(fluxes_dict.values(), dtype="float")
         else:
             raise NotImplementedError(f"Unknown return type {return_type}")
 
-    def get_right_hand_side(
-        self, variables: dict[str, float], time: float = 0.0
-    ) -> dict[str, float]:
+    def get_right_hand_side(self, variables: dict[str, float], time: float = 0.0) -> dict[str, float]:
         fluxes = self.get_fluxes(variables, time=time)
         return self._reactions.get_right_hand_side_float(fluxes)
 
     def to_version_1(self) -> OldModel:
         old = OldModel()
 
         old.add_compounds(list(self.variables))
@@ -457,14 +447,12 @@
         old.add_parameters({k: v.value for k, v in self.constants.items()})
 
         for k in _sort_derived_compounds(self):
             dc = self.derived_constants[k]
             old.add_derived_parameter(k, dc.function, dc.args)
 
         for k, am in self.algebraic_modules.items():
-            old.add_algebraic_module_from_args(
-                k, am.function, am.derived_variables, am.args
-            )
+            old.add_algebraic_module_from_args(k, am.function, am.derived_variables, am.args)
 
         for r in self.reactions.values():
             old.add_reaction_from_args(r.name, r.function, r.stoichiometry, r.args)
         return old
```

### Comparing `modelbase2-0.1.74/src/modelbase2/ode/simulator.py` & `modelbase2-0.1.8/src/modelbase2/ode/simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import logging
 import numpy as np
 import pandas as pd
-from ..types import Array
 from .integrator import Assimulo
 from .model import Model
 from dataclasses import dataclass, field
 from typing import Any, Optional, Type
+from ..types import Array
 
 logger = logging.getLogger()
 
 
 @dataclass(repr=False)
 class SimulationResult:
     time: Array
@@ -86,20 +86,16 @@
             integration.time,
             dict(zip(self.model.stoichiometries, integration.values.T)),
             self.model.constant_values,
         )
         self.results.append(res)
         return res
 
-    def simulate_to_steady_state(
-        self, tolerance: float = 1e-6
-    ) -> Optional[dict[str, float]]:
-        if (
-            integration := self.integrator.integrate_to_steady_state(tolerance)
-        ) is not None:
+    def simulate_to_steady_state(self, tolerance: float = 1e-6) -> Optional[dict[str, float]]:
+        if (integration := self.integrator.integrate_to_steady_state(tolerance)) is not None:
             return dict(zip(self.model.stoichiometries, integration))
         else:
             logger.warning("Simulation failed")
             return None
 
     def get_results(self) -> pd.DataFrame:
         return concatenate_results(self.results)
@@ -109,34 +105,30 @@
 
     def _get_result_derived_variables(
         self,
         args: dict[str, Array],
     ) -> dict[str, Array]:
         return self.model._algebraic_modules.get_values_array(args)
 
-    def _get_result_all_variables(
-        self, result: SimulationResult, constants: dict[str, Array]
-    ) -> dict[str, Array]:
+    def _get_result_all_variables(self, result: SimulationResult, constants: dict[str, Array]) -> dict[str, Array]:
         args = result.values | constants | {"time": result.time}
         return result.values | self._get_result_derived_variables(args)
 
     def _get_result_fluxes(self, result: SimulationResult) -> dict[str, Array]:
         constants = self._get_result_constants(result)
         all_variables = self._get_result_all_variables(result, constants)
         args = all_variables | constants | {"time": result.time}
         return self.model._reactions.get_fluxes_array(args)
 
     def get_full_results(self) -> pd.DataFrame:
         full_results: list[SimulationResult] = []
         for result in self.results:
             full_results.append(
                 SimulationResult(
-                    values=self._get_result_all_variables(
-                        result, self._get_result_constants(result)
-                    ),
+                    values=self._get_result_all_variables(result, self._get_result_constants(result)),
                     time=result.time,
                     constants=result.constants,
                 )
             )
         return concatenate_results(full_results)
 
     def get_fluxes(self) -> pd.DataFrame:
```

### Comparing `modelbase2-0.1.74/src/modelbase2/utils/plotting.py` & `modelbase2-0.1.8/src/modelbase2/utils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import itertools as it
 import math
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from ..types import Axes, Figure
 from matplotlib.collections import QuadMesh
 from matplotlib.colors import LogNorm, Normalize, SymLogNorm
 from matplotlib.colors import colorConverter as _colorConverter
 from typing import Any, Iterable, Optional, Sized, Union
+from ..types import Figure, Axes
 
 
 def _get_plot_kwargs(
     figure_kwargs: Optional[dict[str, Any]],
     subplot_kwargs: Optional[dict[str, Any]],
     plot_kwargs: Optional[dict[str, Any]],
     grid_kwargs: Optional[dict[str, Any]],
@@ -187,18 +187,15 @@
     tick_kwargs: Optional[dict[str, Any]] = None,
     label_kwargs: Optional[dict[str, Any]] = None,
     title_kwargs: Optional[dict[str, Any]] = None,
 ) -> tuple[Figure, Axes]:
     """Plot simulation results as a grid."""
     if ncols is None:
         _, ncols = min(
-            (
-                (math.ceil(len(plot_groups) / i) * i - len(plot_groups), i)
-                for i in range(2, 6)
-            ),
+            ((math.ceil(len(plot_groups) / i) * i - len(plot_groups), i) for i in range(2, 6)),
             key=lambda x: (x[0], -x[1]),
         )
     nrows = math.ceil(len(plot_groups) / ncols)
     if figure_kwargs is None:
         figure_kwargs = {}
     figure_kwargs.setdefault("figsize", (5 * ncols, 4 * nrows))
     if legend_kwargs is None:
@@ -277,14 +274,15 @@
 
     # L = 0.2126 * R + 0.7152 * G + 0.0722 * B
     rel_luminance: list[float] = np.matmul(rsrgb, [0.2126, 0.7152, 0.0722])
     return rel_luminance[0]
 
 
 def get_norm(vmin: float, vmax: float) -> plt.Normalize:
+
     if vmax < 1000 and vmin > -1000:
         norm = Normalize(vmin=vmin, vmax=vmax)
     elif vmin <= 0:
         norm = SymLogNorm(linthresh=1, vmin=vmin, vmax=vmax, base=10)
     else:
         norm = LogNorm(vmin=vmin, vmax=vmax)
     return norm
@@ -346,20 +344,16 @@
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
 
     if annotate:
         text_kwargs = {"ha": "center", "va": "center"}
         hm.update_scalarmappable()  # So that get_facecolor is an array
         xpos, ypos = np.meshgrid(np.arange(len(columns)), np.arange(len(rows)))
-        for x, y, val, color in zip(
-            xpos.flat, ypos.flat, hm.get_array(), hm.get_facecolor()
-        ):
-            text_kwargs["color"] = (
-                "black" if relative_luminance(color) > 0.45 else "white"
-            )
+        for x, y, val, color in zip(xpos.flat, ypos.flat, hm.get_array(), hm.get_facecolor()):
+            text_kwargs["color"] = "black" if relative_luminance(color) > 0.45 else "white"
             if sci_annotation_bounds[0] < abs(val) <= sci_annotation_bounds[1]:
                 val_text = f"{val:.{annotation_style}}"
             else:
                 val_text = f"{val:.0e}"
             ax.text(x + 0.5, y + 0.5, val_text, **text_kwargs)
 
     if colorbar:
```

### Comparing `modelbase2-0.1.74/setup.py` & `modelbase2-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,24 +21,24 @@
  'scipy>=1.7.2,<2.0.0',
  'sympy>=1.9,<2.0',
  'tqdm>=4.62.3,<5.0.0',
  'typing-extensions>=4.0.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'modelbase2',
-    'version': '0.1.74',
+    'version': '0.1.8',
     'description': 'A package to build metabolic models',
     'long_description': 'None',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'Marvin van Aalst',
     'maintainer_email': 'marvin.vanaalst@gmail.com',
     'url': 'https://gitlab.com/qtb-hhu/modelbase-software',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9.0,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `modelbase2-0.1.74/PKG-INFO` & `modelbase2-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: modelbase2
-Version: 0.1.74
+Version: 0.1.8
 Summary: A package to build metabolic models
 Home-page: https://gitlab.com/qtb-hhu/modelbase-software
 License: GPL-3.0-or-later
 Keywords: modelling,ode,metabolic
 Author: Marvin van Aalst
 Author-email: marvin.vanaalst@gmail.com
 Maintainer: Marvin van Aalst
 Maintainer-email: marvin.vanaalst@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9.0,<3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: black (>=22.3.0,<23.0.0)
 Requires-Dist: ipywidgets (>=8.0.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
```


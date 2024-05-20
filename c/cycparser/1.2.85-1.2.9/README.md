# Comparing `tmp/cycparser-1.2.85.tar.gz` & `tmp/cycparser-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycparser-1.2.85.tar", max compression
+gzip compressed data, was "cycparser-1.2.9.tar", max compression
```

## Comparing `cycparser-1.2.85.tar` & `cycparser-1.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35079 2024-05-20 01:05:27.458856 cycparser-1.2.85/LICENSE
--rw-r--r--   0        0        0     1661 2024-05-20 01:05:27.459856 cycparser-1.2.85/pyproject.toml
--rw-r--r--   0        0        0     3512 2024-05-20 01:05:27.459856 cycparser-1.2.85/src/cycparser/__init__.py
--rw-r--r--   0        0        0     2827 2024-05-20 01:05:27.459856 cycparser-1.2.85/src/cycparser/data.py
--rw-r--r--   0        0        0     6585 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/defaults.py
--rw-r--r--   0        0        0     1994 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/parsing/__init__.py
--rw-r--r--   0        0        0     3434 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/parsing/compounds.py
--rw-r--r--   0        0        0     2545 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/parsing/enzymes.py
--rw-r--r--   0        0        0     2753 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/parsing/monomer_annotation.py
--rw-r--r--   0        0        0      502 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/parsing/monomer_sequences.py
--rw-r--r--   0        0        0     1390 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/parsing/protein_complexes.py
--rw-r--r--   0        0        0     6825 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/parsing/reactions.py
--rw-r--r--   0        0        0     2044 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/parsing/shared.py
--rw-r--r--   0        0        0        0 2024-05-20 01:05:27.496856 cycparser-1.2.85/src/cycparser/py.typed
--rw-r--r--   0        0        0      954 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/repairing/__init__.py
--rw-r--r--   0        0        0      289 2024-05-20 01:05:27.460856 cycparser-1.2.85/src/cycparser/repairing/fix_add_important_cpds.py
--rw-r--r--   0        0        0     8626 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/repairing/fix_create_compartment_variants.py
--rw-r--r--   0        0        0     2202 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/repairing/fix_create_reaction_variants.py
--rw-r--r--   0        0        0      455 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/repairing/fix_filter_garbage.py
--rw-r--r--   0        0        0     1144 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/repairing/fix_get_gpr_association.py
--rw-r--r--   0        0        0      520 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/repairing/fix_get_highest_compound_type.py
--rw-r--r--   0        0        0      525 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/repairing/fix_get_kinetic_data.py
--rw-r--r--   0        0        0     1170 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/repairing/fix_set_reaction_stoichiometry.py
--rw-r--r--   0        0        0     1778 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/repairing/fix_unify_reaction_direction.py
--rw-r--r--   0        0        0     2416 2024-05-20 01:05:27.461856 cycparser-1.2.85/src/cycparser/utils.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 cycparser-1.2.85/setup.py
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 cycparser-1.2.85/PKG-INFO
+-rw-r--r--   0        0        0    35079 2022-08-01 02:07:03.381614 cycparser-1.2.9/LICENSE
+-rw-r--r--   0        0        0     1901 2022-08-01 02:07:03.382614 cycparser-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3484 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/__init__.py
+-rw-r--r--   0        0        0     2827 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/data.py
+-rw-r--r--   0        0        0     6585 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/defaults.py
+-rw-r--r--   0        0        0     1928 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/__init__.py
+-rw-r--r--   0        0        0     3434 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/compounds.py
+-rw-r--r--   0        0        0     2510 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/enzymes.py
+-rw-r--r--   0        0        0     2747 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/monomer_annotation.py
+-rw-r--r--   0        0        0      502 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/monomer_sequences.py
+-rw-r--r--   0        0        0     1385 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/protein_complexes.py
+-rw-r--r--   0        0        0     6625 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/reactions.py
+-rw-r--r--   0        0        0     2038 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/shared.py
+-rw-r--r--   0        0        0        0 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/py.typed
+-rw-r--r--   0        0        0      954 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/repairing/__init__.py
+-rw-r--r--   0        0        0      289 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/repairing/fix_add_important_cpds.py
+-rw-r--r--   0        0        0     8538 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_create_compartment_variants.py
+-rw-r--r--   0        0        0     2188 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_create_reaction_variants.py
+-rw-r--r--   0        0        0      455 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_filter_garbage.py
+-rw-r--r--   0        0        0     1144 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_get_gpr_association.py
+-rw-r--r--   0        0        0      520 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_get_highest_compound_type.py
+-rw-r--r--   0        0        0      525 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_get_kinetic_data.py
+-rw-r--r--   0        0        0     1164 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_set_reaction_stoichiometry.py
+-rw-r--r--   0        0        0     1772 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_unify_reaction_direction.py
+-rw-r--r--   0        0        0     2416 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/utils.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 cycparser-1.2.9/setup.py
+-rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 cycparser-1.2.9/PKG-INFO
```

### Comparing `cycparser-1.2.85/LICENSE` & `cycparser-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.85/pyproject.toml` & `cycparser-1.2.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 [tool.poetry]
 name = "cycparser"
-version = "1.2.85"
+version = "1.2.9"
 description = ""
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = "^3.8"
 gitchangelog = "^3.0.4"
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.1.1"
 isort = "^5.10.0"
 flake8 = "^4.0.1"
 mypy = "^0.910"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 ipykernel = "^6.6.1"
 black = "^22.3.0"
 
-[tool.poetry.group.dev.dependencies]
-gitchangelog = "^3.0.4"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
-line-length = 90
-target-version = ['py311']
-
-[tool.bandit]
-skips = ["B101", "B301", "B403", "B404", "B603", "B607"]
+line-length = 110
+target-version = ['py38']
+include = '\.pyi?$'
+exclude = '''
+(
+  /(
+      \.eggs         # exclude a few common directories in the
+    | \.git          # root of the project
+    | \.hg
+    | \.mypy_cache
+    | \.tox
+    | \.venv
+    | _build
+    | buck-out
+    | build
+    | dist
+  )/
+  | foo.py           # also separately exclude a file named foo.py in
+                     # the root of the project
+)
+'''
 
 [tool.isort]
 profile = "black"
 sections = ["FUTURE", "STDLIB", "FIRSTPARTY", "THIRDPARTY", "LOCALFOLDER"]
 import_heading_stdlib = ""
 import_heading_framework = ""
 import_heading_firstparty = ""
@@ -48,15 +61,15 @@
 warn_return_any = true
 warn_unused_configs = true
 ignore_missing_imports = true
 disallow_untyped_defs = true
 exclude = "temp"
 
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

### Comparing `cycparser-1.2.85/src/cycparser/__init__.py` & `cycparser-1.2.9/src/cycparser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,27 +24,27 @@
     fix_unify_reaction_direction,
     get_gpr_associations,
     get_highest_compound_type,
     get_kinetic_data,
 )
 
 __all__ = [
-    "COMPARTMENT_MAP",
-    "COMPARTMENT_SUFFIXES",
+    "repair",
+    "parse_and_repair_pgdb",
     "Compound",
     "Cyc",
     "Enzyme",
     "KineticData",
-    "MANUAL_ADDITIONS",
     "Monomer",
     "MonomerAnnotation",
     "Reaction",
+    "COMPARTMENT_MAP",
+    "COMPARTMENT_SUFFIXES",
+    "MANUAL_ADDITIONS",
     "TYPE_MAP",
-    "parse_and_repair_pgdb",
-    "repair",
 ]
 
 
 def combine_sequence_and_annotation(
     sequences: Dict[str, str], annotation: Dict[str, MonomerAnnotation]
 ) -> Dict[str, Monomer]:
     return {
@@ -86,21 +86,17 @@
         compounds,
         compartment_map,
         compartment_suffixes,
     )
     reactions = fix_set_reaction_stoichiometry(reactions)
 
     # Post fixing
-    used_compartments: Set[str] = {
-        i.compartment for i in compounds.values() if i.compartment is not None
-    }
+    used_compartments: Set[str] = {i.compartment for i in compounds.values() if i.compartment is not None}
     compartments: Dict[str, str] = {i: compartment_suffixes[i] for i in used_compartments}
-    return Cyc(
-        compounds, reactions, compartments, gpr_annotations, kinetic_data, monomers
-    )
+    return Cyc(compounds, reactions, compartments, gpr_annotations, kinetic_data, monomers)
 
 
 def parse_and_repair_pgdb(
     pgdb_path: Path,
     compartment_map: Dict[str, str] | None = None,
     type_map: Dict[str, str] | None = None,
     manual_additions: Dict[str, Compound] | None = None,
```

### Comparing `cycparser-1.2.85/src/cycparser/data.py` & `cycparser-1.2.9/src/cycparser/data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, List, Set, Tuple
 
 __all__ = [
-    "Compound",
-    "Enzyme",
     "Monomer",
     "MonomerAnnotation",
+    "Compound",
     "Reaction",
+    "Enzyme",
 ]
 
 
 @dataclass
 class Compound:
     id: str
     base_id: str
```

### Comparing `cycparser-1.2.85/src/cycparser/defaults.py` & `cycparser-1.2.9/src/cycparser/defaults.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from .data import Compound
 
 __all__ = [
     "COMPARTMENT_MAP",
+    "TYPE_MAP",
     "COMPARTMENT_SUFFIXES",
     "MANUAL_ADDITIONS",
-    "TYPE_MAP",
 ]
 
 COMPARTMENT_MAP = {
     "CYTOSOL": "CYTOSOL",
     "IN": "CYTOSOL",
     "UNKNOWN-SPACE": "CYTOSOL",
     "SIDE-1": "CYTOSOL",
```

### Comparing `cycparser-1.2.85/src/cycparser/parsing/__init__.py` & `cycparser-1.2.9/src/cycparser/parsing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from .enzymes import parse_enzymes
 from .monomer_annotation import parse_monomer_annotation
 from .monomer_sequences import parse_sequences
 from .protein_complexes import parse_complexes
 from .reactions import parse_reactions
 
 __all__ = [
-    "parse_complexes",
+    "parse_pgdb",
     "parse_compounds",
     "parse_enzymes",
     "parse_monomer_annotation",
-    "parse_pgdb",
+    "parse_complexes",
     "parse_reactions",
     "parse_sequences",
 ]
 
 
 def remove_top_comments(file: List[str]) -> List[str]:
     """Remove the metainformation from a pgdb file."""
@@ -46,20 +46,14 @@
 
 
 def parse_pgdb(path: Path, type_map: Dict[str, str] | None = None) -> Result:
     if type_map is None:
         type_map = {}
 
     return Result(
-        compounds=parse_compounds(
-            read_file_and_remove_comments(path / "compounds.dat"), type_map
-        ),
-        reactions=parse_reactions(
-            read_file_and_remove_comments(path / "reactions.dat"), type_map
-        ),
-        monomer_annotation=parse_monomer_annotation(
-            read_file_and_remove_comments(path / "genes.dat")
-        ),
+        compounds=parse_compounds(read_file_and_remove_comments(path / "compounds.dat"), type_map),
+        reactions=parse_reactions(read_file_and_remove_comments(path / "reactions.dat"), type_map),
+        monomer_annotation=parse_monomer_annotation(read_file_and_remove_comments(path / "genes.dat")),
         complexes=parse_complexes(read_file_and_remove_comments(path / "proteins.dat")),
         enzymes=parse_enzymes(read_file_and_remove_comments(path / "enzrxns.dat")),
         sequences=parse_sequences(iter(read_file(path / "protseq.fsa"))),
     )
```

### Comparing `cycparser-1.2.85/src/cycparser/parsing/compounds.py` & `cycparser-1.2.9/src/cycparser/parsing/compounds.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.85/src/cycparser/parsing/enzymes.py` & `cycparser-1.2.9/src/cycparser/parsing/enzymes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 __all__ = ["parse_enzymes"]
 
 logger = logging.getLogger(__name__)
 Action = Callable[[Any, Any, Any], None]
 SubAction = Dict[str, Callable[[Any, Any, Any, Any], None]]
 
 
-def _set_cplx_or_monomer(
-    enzrxns: Dict[str, Enzyme], id_: str, cplx_or_monomer: str
-) -> None:
+def _set_cplx_or_monomer(enzrxns: Dict[str, Enzyme], id_: str, cplx_or_monomer: str) -> None:
     enzrxns[id_].cplx_or_monomer = cplx_or_monomer
 
 
 def _add_kcat(enzrxns: Dict[str, Enzyme], id_: str, substrate: str, kcat: str) -> None:
     try:
         enzrxns[id_].kinetic_data.kcat.setdefault(substrate, float(kcat))
     except ValueError:  # conversion failed
@@ -41,14 +39,15 @@
 
 
 def parse_enzymes(
     file: Iterable[str],
     actions: Dict[str, Action] | None = None,
     sub_actions: Dict[str, SubAction] | None = None,
 ) -> Dict[str, Enzyme]:
+
     if actions is None:
         actions = {
             "ENZYME": _set_cplx_or_monomer,
         }
     if sub_actions is None:
         sub_actions = {
             "^SUBSTRATE": {"KM": _add_km, "VMAX": _add_vmax, "KCAT": _add_kcat},
@@ -67,17 +66,15 @@
             logger.info(f"Malformed line in enzymes.dat {line}")
             continue
 
         if identifier == "UNIQUE-ID":
             id_ = content
             enzrxns[id_] = Enzyme(id=id_)
         elif identifier.startswith("^"):
-            if (
-                subaction := sub_actions.get(identifier, {}).get(last_identifier, None)
-            ) is not None:
+            if (subaction := sub_actions.get(identifier, {}).get(last_identifier, None)) is not None:
                 subaction(enzrxns, id_, content, last_content)
         else:
             if (action := actions.get(identifier, None)) is not None:
                 action(enzrxns, id_, content)
                 last_identifier = identifier
                 last_content = content
     return enzrxns
```

### Comparing `cycparser-1.2.85/src/cycparser/parsing/monomer_annotation.py` & `cycparser-1.2.9/src/cycparser/parsing/monomer_annotation.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 __all__ = ["parse_monomer_annotation"]
 
 logger = logging.getLogger(__name__)
 Action = Callable[[Any, Any, Any], None]
 
 
-def _set_gene_product(
-    genes: Dict[str, MonomerAnnotation], id_: str, product: str
-) -> None:
+def _set_gene_product(genes: Dict[str, MonomerAnnotation], id_: str, product: str) -> None:
     genes[id_].product = product
 
 
 def parse_monomer_annotation(
     file: Iterable[str],
     actions: Dict[str, Action] | None = None,
     db_to_resource: dict[str, str] | None = None,
```

### Comparing `cycparser-1.2.85/src/cycparser/parsing/protein_complexes.py` & `cycparser-1.2.9/src/cycparser/parsing/protein_complexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["parse_complexes"]
 Action = Callable[[Any, Any, Any], None]
 
 
-def _add_component(
-    complexes: Dict[str, Set[str]], complex_id: str, component: str
-) -> None:
+def _add_component(complexes: Dict[str, Set[str]], complex_id: str, component: str) -> None:
     complexes[complex_id].add(component)
 
 
 def parse_complexes(
     file: Iterable[str],
     actions: Dict[str, Action] | None = None,
 ) -> Dict[str, Set[str]]:
+
     if actions is None:
         actions = {
             "COMPONENTS": _add_component,
         }
 
     id_ = ""
     proteins: Dict[str, Set[str]] = {}
```

### Comparing `cycparser-1.2.85/src/cycparser/parsing/reactions.py` & `cycparser-1.2.9/src/cycparser/parsing/reactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,23 @@
     reactions[id_].pathways.add(pathway)
 
 
 def _add_enzrxn(reactions: Dict[str, Reaction], id_: str, enzrxn: str) -> None:
     reactions[id_].enzrxns.add(enzrxn)
 
 
-def _set_reaction_direction(
-    reactions: Dict[str, Reaction], id_: str, direction: str
-) -> None:
+def _set_reaction_direction(reactions: Dict[str, Reaction], id_: str, direction: str) -> None:
     reactions[id_].direction = direction
     if direction == "REVERSIBLE":
         reactions[id_].reversible = True
     else:
         reactions[id_].reversible = False
 
 
-def _add_reaction_location(
-    reactions: Dict[str, Reaction], id_: str, location: str
-) -> None:
+def _add_reaction_location(reactions: Dict[str, Reaction], id_: str, location: str) -> None:
     location = location.replace("CCI-", "CCO-")
     if location.startswith("CCO-"):
         reactions[id_].locations.append(location)
 
 
 def _set_substrate(
     reactions: Dict[str, Reaction],
@@ -77,32 +73,28 @@
     reactions: Dict[str, Reaction],
     id_: str,
     coefficient: str,
     substrate: str,
     type_map: Dict[str, str],
 ) -> None:
     try:
-        reactions[id_].substrates[
-            _rename(type_map.get(substrate, substrate)) + "_c"
-        ] = -float(coefficient)
+        reactions[id_].substrates[_rename(type_map.get(substrate, substrate)) + "_c"] = -float(coefficient)
     except ValueError:  # conversion failed
         pass
 
 
 def _set_product_coefficient(
     reactions: Dict[str, Reaction],
     id_: str,
     coefficient: str,
     product: str,
     type_map: Dict[str, str],
 ) -> None:
     try:
-        reactions[id_].products[_rename(type_map.get(product, product)) + "_c"] = float(
-            coefficient
-        )
+        reactions[id_].products[_rename(type_map.get(product, product)) + "_c"] = float(coefficient)
     except ValueError:  # conversion failed
         pass
 
 
 def _set_substrate_compartment(
     reactions: Dict[str, Reaction],
     id_: str,
@@ -169,25 +161,19 @@
             "RXN-LOCATIONS": _add_reaction_location,
         }
 
     if sub_actions is None:
         sub_actions = {
             "^COMPARTMENT": {
                 "LEFT": partial(_set_substrate_compartment, type_map=type_map),
-                "RIGHT": lambda a, b, c, d: _set_product_compartment(
-                    a, b, c, d, type_map=type_map
-                ),
+                "RIGHT": lambda a, b, c, d: _set_product_compartment(a, b, c, d, type_map=type_map),
             },
             "^COEFFICIENT": {
-                "LEFT": lambda a, b, c, d: _set_substrate_coefficient(
-                    a, b, c, d, type_map=type_map
-                ),
-                "RIGHT": lambda a, b, c, d: _set_product_coefficient(
-                    a, b, c, d, type_map=type_map
-                ),
+                "LEFT": lambda a, b, c, d: _set_substrate_coefficient(a, b, c, d, type_map=type_map),
+                "RIGHT": lambda a, b, c, d: _set_product_coefficient(a, b, c, d, type_map=type_map),
             },
         }
 
     id_ = ""
     reactions = {}
     last_identifier = ""
     last_content = ""
@@ -207,17 +193,15 @@
                 base_id=id_,
                 database_links={
                     "biocyc": set([id_]),
                     "metacyc.reaction": set([id_]),
                 },
             )
         elif identifier.startswith("^"):
-            if (
-                subaction := sub_actions.get(identifier, {}).get(last_identifier, None)
-            ) is not None:
+            if (subaction := sub_actions.get(identifier, {}).get(last_identifier, None)) is not None:
                 subaction(reactions, id_, content, last_content)
         else:
             if (action := actions.get(identifier, None)) is not None:
                 action(reactions, id_, content)
                 last_identifier = identifier
                 last_content = content
```

### Comparing `cycparser-1.2.85/src/cycparser/parsing/shared.py` & `cycparser-1.2.9/src/cycparser/parsing/shared.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from typing import Dict
 
 from ..data import Compound, Reaction
 
 __all__ = [
     "MALFORMED_LINE_STARTS",
-    "_add_database_link",
-    "_add_type",
     "_rename",
     "_set_gibbs0",
     "_set_name",
+    "_add_database_link",
+    "_add_type",
 ]
 
 # Often lines starting with these identifiers are malformed
 MALFORMED_LINE_STARTS = {
     "/",
     "COMMENT",
     "CITATIONS",
@@ -39,17 +39,15 @@
         .replace("</SUB>", "")
         .replace("&", "")
         .replace(";", "")
         .replace("|", "")
     )
 
 
-def _set_gibbs0(
-    dictionary: Dict[str, Reaction | Compound], id_: str, gibbs0: str
-) -> None:
+def _set_gibbs0(dictionary: Dict[str, Reaction | Compound], id_: str, gibbs0: str) -> None:
     try:
         dictionary[id_].gibbs0 = float(gibbs0)
     except ValueError:  # conversion failed
         pass
 
 
 def _set_name(dictionary: Dict[str, Reaction | Compound], id_: str, name: str) -> None:
```

### Comparing `cycparser-1.2.85/src/cycparser/repairing/__init__.py` & `cycparser-1.2.9/src/cycparser/repairing/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 __all__ = [
     "fix_add_important_compounds",
     "fix_create_compartment_variants",
     "fix_create_reaction_variants",
     "fix_filter_garbage_reactions",
     "fix_set_reaction_stoichiometry",
     "fix_unify_reaction_direction",
-    "get_gpr_associations",
     "get_highest_compound_type",
+    "get_gpr_associations",
     "get_kinetic_data",
 ]
 
 
 from .fix_add_important_cpds import fix_add_important_compounds
 from .fix_create_compartment_variants import fix_create_compartment_variants
 from .fix_create_reaction_variants import fix_create_reaction_variants
```

### Comparing `cycparser-1.2.85/src/cycparser/repairing/fix_create_compartment_variants.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_create_compartment_variants.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,16 @@
     split = re.split(r"(\-?CCO\-)", location)
     try:
         out_, in_ = split[2::2]
     except ValueError:
         out_ = split[2]
         in_ = "CYTOSOL"
     return {
-        "CCO-OUT": _map_compartment_to_model_compartments(
-            compartment=out_, compartment_map=compartment_map
-        ),
-        "CCO-IN": _map_compartment_to_model_compartments(
-            compartment=in_, compartment_map=compartment_map
-        ),
+        "CCO-OUT": _map_compartment_to_model_compartments(compartment=out_, compartment_map=compartment_map),
+        "CCO-IN": _map_compartment_to_model_compartments(compartment=in_, compartment_map=compartment_map),
     }
 
 
 def _add_compartment_compound_variant(
     *,
     cpd_id: str,
     compartment: str,
@@ -116,17 +112,15 @@
         compartment=compartment,
         compartment_suffixes=compartment_suffixes,
     )
     local.compartment = compartment
     return local
 
 
-def _get_sides(
-    side: str, location: str, compartment_map: Dict[str, str]
-) -> Dict[str, str]:
+def _get_sides(side: str, location: str, compartment_map: Dict[str, str]) -> Dict[str, str]:
     if "-CCO-" in location:
         return _split_location(location=location, compartment_map=compartment_map)
     else:
         return {
             side: _map_compartment_to_model_compartments(
                 compartment=location[4:],
                 compartment_map=compartment_map,
@@ -244,17 +238,15 @@
                     compartment_suffixes=compartment_suffixes,
                 )
                 new_reactions[local.id] = local
         else:
             if not bool(rxn.locations):
                 rxn.locations = ["CCO-EXTRACELLULAR-CCO-CYTOSOL"]
             for location in rxn.locations:
-                sides = _split_location(
-                    location=location, compartment_map=compartment_map
-                )
+                sides = _split_location(location=location, compartment_map=compartment_map)
                 if sides["CCO-IN"] == sides["CCO-OUT"]:
                     local = _create_compartment_reaction(
                         rxn=rxn,
                         compartment=sides["CCO-OUT"],
                         compounds=compounds,
                         compartment_suffixes=compartment_suffixes,
                     )
```

### Comparing `cycparser-1.2.85/src/cycparser/repairing/fix_create_reaction_variants.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_create_reaction_variants.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 ) -> Reaction:
     local = copy.copy(rxn)
     local.substrates = {compound_map.get(k, k): v for k, v in local.substrates.items()}
     local.products = {compound_map.get(k, k): v for k, v in local.products.items()}
     local.substrate_compartments = {
         compound_map.get(k, k): v for k, v in local.substrate_compartments.items()
     }
-    local.product_compartments = {
-        compound_map.get(k, k): v for k, v in local.product_compartments.items()
-    }
+    local.product_compartments = {compound_map.get(k, k): v for k, v in local.product_compartments.items()}
     local.id = f"{local.id}__var__{count}"
     local._var = count
     return local
 
 
 def fix_create_reaction_variants(
     rxns: Dict[str, Reaction],
```

### Comparing `cycparser-1.2.85/src/cycparser/repairing/fix_get_gpr_association.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_get_gpr_association.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.85/src/cycparser/repairing/fix_get_highest_compound_type.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_get_highest_compound_type.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.85/src/cycparser/repairing/fix_get_kinetic_data.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_get_kinetic_data.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.85/src/cycparser/repairing/fix_set_reaction_stoichiometry.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_set_reaction_stoichiometry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import annotations
 
 from typing import Dict
 
 from ..data import Reaction
 
 
-def fix_set_reaction_stoichiometry(
-    parse_reactions: Dict[str, Reaction]
-) -> Dict[str, Reaction]:
+def fix_set_reaction_stoichiometry(parse_reactions: Dict[str, Reaction]) -> Dict[str, Reaction]:
     """Set the stoichiometry from the information given by the substrates and products."""
     new_reactions = {}
     for rxn_id, reaction in parse_reactions.items():
         substrates = reaction.substrates
         products = reaction.products
 
         # Check for duplicates
```

### Comparing `cycparser-1.2.85/src/cycparser/repairing/fix_unify_reaction_direction.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_unify_reaction_direction.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,17 +21,15 @@
         rxn.gibbs0 = -rxn.gibbs0
     rxn.substrate_compartments, rxn.product_compartments = (
         rxn.product_compartments,
         rxn.substrate_compartments,
     )
 
 
-def fix_unify_reaction_direction(
-    parse_reactions: Dict[str, Reaction]
-) -> Dict[str, Reaction]:
+def fix_unify_reaction_direction(parse_reactions: Dict[str, Reaction]) -> Dict[str, Reaction]:
     """Set every reaction to be LEFT-TO-RIGHT and add bounds accordingly."""
     for reaction in parse_reactions.values():
         if reaction.reversible:
             reaction.bounds = (-1000, 1000)
         else:
             direction = reaction.direction
             if direction in (
```

### Comparing `cycparser-1.2.85/src/cycparser/utils.py` & `cycparser-1.2.9/src/cycparser/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import itertools as it
 from collections import defaultdict
 from typing import DefaultDict, Dict
 
 from .data import Compound, Reaction
 
 __all__ = [
-    "check_charge_balance",
     "check_compound_existence",
     "check_mass_balance",
+    "check_charge_balance",
     "reaction_is_bad",
 ]
 
 
 def check_compound_existence(rxn: Reaction, cpds: Dict[str, Compound]) -> bool:
     """Check if all compounds of a reaction exist."""
     for cpd in it.chain(rxn.substrates, rxn.products):
```

### Comparing `cycparser-1.2.85/setup.py` & `cycparser-1.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['gitchangelog>=3.0.4,<4.0.0']
 
 setup_kwargs = {
     'name': 'cycparser',
-    'version': '1.2.85',
+    'version': '1.2.9',
     'description': '',
     'long_description': 'None',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```


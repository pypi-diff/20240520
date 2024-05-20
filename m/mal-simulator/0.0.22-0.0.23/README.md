# Comparing `tmp/mal_simulator-0.0.22.tar.gz` & `tmp/mal_simulator-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mal_simulator-0.0.22.tar", last modified: Fri May  3 15:22:14 2024, max compression
+gzip compressed data, was "mal_simulator-0.0.23.tar", last modified: Mon May 20 12:45:45 2024, max compression
```

## Comparing `mal_simulator-0.0.22.tar` & `mal_simulator-0.0.23.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:22:14.623500 mal_simulator-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-03 15:22:14.623500 mal_simulator-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:22:14.623500 mal_simulator-0.0.22/mal_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-03 15:22:14.000000 mal_simulator-0.0.22/mal_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-03 15:22:14.000000 mal_simulator-0.0.22/mal_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:22:14.000000 mal_simulator-0.0.22/mal_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 15:22:14.000000 mal_simulator-0.0.22/mal_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 15:22:14.000000 mal_simulator-0.0.22/mal_simulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:22:14.623500 mal_simulator-0.0.22/malsim/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/malsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:22:14.623500 mal_simulator-0.0.22/malsim/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/malsim/agents/keyboard_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/malsim/agents/searchers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:22:14.623500 mal_simulator-0.0.22/malsim/sims/
--rw-r--r--   0 runner    (1001) docker     (127)    26613 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/malsim/sims/mal_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:22:14.623500 mal_simulator-0.0.22/malsim/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/malsim/wrappers/gym_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/malsim/wrappers/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-03 15:22:10.000000 mal_simulator-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:22:14.623500 mal_simulator-0.0.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:45.691626 mal_simulator-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 12:45:45.691626 mal_simulator-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:45.687626 mal_simulator-0.0.23/mal_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 12:45:45.000000 mal_simulator-0.0.23/mal_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 12:45:45.000000 mal_simulator-0.0.23/mal_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:45:45.000000 mal_simulator-0.0.23/mal_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-20 12:45:45.000000 mal_simulator-0.0.23/mal_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 12:45:45.000000 mal_simulator-0.0.23/mal_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:45.687626 mal_simulator-0.0.23/malsim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/malsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:45.687626 mal_simulator-0.0.23/malsim/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/malsim/agents/keyboard_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/malsim/agents/searchers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:45.687626 mal_simulator-0.0.23/malsim/sims/
+-rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/malsim/sims/mal_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:45:45.687626 mal_simulator-0.0.23/malsim/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/malsim/wrappers/gym_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/malsim/wrappers/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-20 12:45:41.000000 mal_simulator-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:45:45.691626 mal_simulator-0.0.23/setup.cfg
```

### Comparing `mal_simulator-0.0.22/LICENSE` & `mal_simulator-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `mal_simulator-0.0.22/PKG-INFO` & `mal_simulator-0.0.23/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mal-simulator
-Version: 0.0.22
+Version: 0.0.23
 Summary: A MAL compliant simulator.
-Author-email: Andrei Buhaiu <buhaiu@kth.se>, Jakob Nyberg <jaknyb@kth.se>, Nikolaos Kakouros <nkak@kth.se>
+Author-email: Andrei Buhaiu <buhaiu@kth.se>, Jakob Nyberg <jaknyb@kth.se>, Nikolaos Kakouros <nkak@kth.se>, Joakim Loxdal <loxdal@kth.se>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/mal-lang/mal-simulator
 Project-URL: Bug Tracker, https://github.com/mal-lang/mal-simulator/issues
 Project-URL: Repository, https://github.com/mal-lang/mal-simulator
 Keywords: mal
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,18 +16,19 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: py2neo>=2021.2.3
 Requires-Dist: python-jsonschema-objects>=0.4.1
-Requires-Dist: mal-toolbox>=0.0.35
+Requires-Dist: mal-toolbox>=0.0.39
 Requires-Dist: numpy>=1.21.4
 Requires-Dist: pettingzoo>=1.24.2
 Requires-Dist: gymnasium<1,>=0.29.1
+Requires-Dist: PyYAML>=6.0.1
 
 # Overview
 
 A MAL compliant simulator.
 
 # Installation 
 ```pip install mal-simulator```
```

### Comparing `mal_simulator-0.0.22/mal_simulator.egg-info/PKG-INFO` & `mal_simulator-0.0.23/mal_simulator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mal-simulator
-Version: 0.0.22
+Version: 0.0.23
 Summary: A MAL compliant simulator.
-Author-email: Andrei Buhaiu <buhaiu@kth.se>, Jakob Nyberg <jaknyb@kth.se>, Nikolaos Kakouros <nkak@kth.se>
+Author-email: Andrei Buhaiu <buhaiu@kth.se>, Jakob Nyberg <jaknyb@kth.se>, Nikolaos Kakouros <nkak@kth.se>, Joakim Loxdal <loxdal@kth.se>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/mal-lang/mal-simulator
 Project-URL: Bug Tracker, https://github.com/mal-lang/mal-simulator/issues
 Project-URL: Repository, https://github.com/mal-lang/mal-simulator
 Keywords: mal
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,18 +16,19 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: py2neo>=2021.2.3
 Requires-Dist: python-jsonschema-objects>=0.4.1
-Requires-Dist: mal-toolbox>=0.0.35
+Requires-Dist: mal-toolbox>=0.0.39
 Requires-Dist: numpy>=1.21.4
 Requires-Dist: pettingzoo>=1.24.2
 Requires-Dist: gymnasium<1,>=0.29.1
+Requires-Dist: PyYAML>=6.0.1
 
 # Overview
 
 A MAL compliant simulator.
 
 # Installation 
 ```pip install mal-simulator```
```

### Comparing `mal_simulator-0.0.22/malsim/__init__.py` & `mal_simulator-0.0.23/malsim/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- encoding: utf-8 -*-
-# MAL Simulator v0.0.22
+# MAL Simulator v0.0.23
 # Copyright 2024, Andrei Buhaiu.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
@@ -21,16 +21,16 @@
 from malsim.wrappers.gym_wrapper import AttackerEnv, DefenderEnv, register_envs
 
 """
 MAL Simulator
 """
 
 __title__ = "malsim"
-__version__ = "0.0.22"
-__authors__ = ["Andrei Buhaiu", "Jakob Nyberg", "Nikolaos Kakouros"]
+__version__ = "0.0.23"
+__authors__ = ["Andrei Buhaiu", "Jakob Nyberg", "Nikolaos Kakouros", "Joakim Loxdal"]
 __license__ = "Apache 2.0"
 __docformat__ = "restructuredtext en"
 
 __all__ = ("LazyWrapper", "AttackerEnv", "DefenderEnv", "register_envs")
 
 formatter = logging.Formatter('%(asctime)s %(name)-12s %(levelname)-8s %(message)s', datefmt='%m-%d %H:%M')
 file_handler = logging.FileHandler('tmp/malsim_log.txt', mode='w')
```

### Comparing `mal_simulator-0.0.22/malsim/agents/keyboard_input.py` & `mal_simulator-0.0.23/malsim/agents/keyboard_input.py`

 * *Files identical despite different names*

### Comparing `mal_simulator-0.0.22/malsim/agents/searchers.py` & `mal_simulator-0.0.23/malsim/agents/searchers.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 ) -> List[int]:
     attack_surface = mask[1]
     surface_indexes = list(np.flatnonzero(attack_surface))
     new_targets = [idx for idx in surface_indexes if idx not in discovered_targets]
     return new_targets, surface_indexes
 
 
+class PassiveAttacker:
+    def compute_action_from_dict(self, observation, mask):
+        return (0, None)
+
 class BreadthFirstAttacker:
     def __init__(self, agent_config: dict) -> None:
         self.targets: Deque[int] = deque([])
         self.current_target: int = None
         seed = (
             agent_config["seed"]
             if agent_config.get("seed", None)
```

### Comparing `mal_simulator-0.0.22/malsim/sims/mal_simulator.py` & `mal_simulator-0.0.23/malsim/sims/mal_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         }
         str_format = "{:<5} {:<}\n"
         table = "\n" + str_format.format("Index", "Asset Type")
         for entry in self._index_to_asset_type:
             table += str_format.format(self._asset_type_to_index[entry], entry)
         logger.debug(table)
 
-        self._index_to_step_name = [n.name for n in self.lang_graph.attack_steps]
+        self._index_to_step_name = [n.asset.name + ":" + n.name for n in self.lang_graph.attack_steps]
         self._step_name_to_index = {
             n: i for i, n in enumerate(self._index_to_step_name)
         }
 
         self._unholy_index_to_step_name = {
             n.attributes["name"] for n in self.lang_graph.attack_steps
         }
```

### Comparing `mal_simulator-0.0.22/malsim/wrappers/gym_wrapper.py` & `mal_simulator-0.0.23/malsim/wrappers/gym_wrapper.py`

 * *Files identical despite different names*

### Comparing `mal_simulator-0.0.22/malsim/wrappers/wrapper.py` & `mal_simulator-0.0.23/malsim/wrappers/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 
 from gymnasium.spaces.space import Space
 from pettingzoo.utils.env import ParallelEnv
 
-from maltoolbox.language import LanguageClassesFactory, LanguageGraph, specification
+from maltoolbox.language import LanguageClassesFactory, LanguageGraph
 from maltoolbox.attackgraph import AttackGraph
 from maltoolbox.model import Model
 
 from malsim.sims.mal_simulator import MalSimulator
 
 
 class LazyWrapper(ParallelEnv):
@@ -15,35 +15,33 @@
         lang_file = kwargs.pop("lang_file")
         model_file = kwargs.pop("model_file")
         if "attack_graph_file" in kwargs:
             attack_graph_file = kwargs.pop("attack_graph_file")
         else:
             attack_graph_file = ""
         agents = kwargs.pop("agents", {})
-        lang_spec = specification.load_language_specification_from_mar(
+        lang_spec = LanguageGraph.from_mar_archive(
             str(lang_file))
         lang_classes_factory = LanguageClassesFactory(lang_spec)
-        lang_classes_factory.create_classes()
 
         lang_graph = LanguageGraph(lang_spec)
 
-        model = Model("Test Model", lang_spec, lang_classes_factory)
-        model.load_from_file(model_file)
+        model = Model.load_from_file(model_file, lang_classes_factory)
 
         if attack_graph_file != "":
             # If we were provided with an attack graph file we load it.
             attack_graph = AttackGraph()
             attack_graph.load_from_file(filename = attack_graph_file,
                 model = model)
-            attack_graph.attach_attackers(model)
+            attack_graph.attach_attackers()
         else:
             # Otherwise we generate the attack graph based on the model
             # provided.
             attack_graph = AttackGraph(lang_spec, model)
-            attack_graph.attach_attackers(model)
+            attack_graph.attach_attackers()
 
         sim = MalSimulator(lang_graph,
             model,
             attack_graph,
             **kwargs)
 
         for agent_class, agent_id in agents.items():
```

### Comparing `mal_simulator-0.0.22/pyproject.toml` & `mal_simulator-0.0.23/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [project]
 name = "mal-simulator"
-version = "0.0.22"
+version = "0.0.23"
 authors = [
   { name="Andrei Buhaiu", email="buhaiu@kth.se" },
   { name="Jakob Nyberg", email="jaknyb@kth.se" },
-  { name="Nikolaos Kakouros", email="nkak@kth.se" }
+  { name="Nikolaos Kakouros", email="nkak@kth.se" },
+  { name="Joakim Loxdal", email="loxdal@kth.se" }
 
 ]
 description = "A MAL compliant simulator."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
   "py2neo>=2021.2.3",
   "python-jsonschema-objects>=0.4.1",
-  "mal-toolbox>=0.0.35",
+  "mal-toolbox>=0.0.39",
   "numpy>=1.21.4",
   "pettingzoo>=1.24.2",
-  "gymnasium>=0.29.1, <1"
+  "gymnasium>=0.29.1, <1",
+  "PyYAML>=6.0.1"
 ]
 license = {text = "Apache Software License"}
 keywords = ["mal"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
@@ -39,7 +41,10 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["malsim*"]
 
 [tool.setuptools.package-data]
 maltoolbox = ["tests*"]
+
+[tool.pytest.ini_options]
+pythonpath = ['.']
```


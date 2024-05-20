# Comparing `tmp/simpn-1.1.0.tar.gz` & `tmp/simpn-1.2.0.tar.gz`

## Comparing `simpn-1.1.0.tar` & `simpn-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 simpn-1.1.0/CHANGELOG.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/immutabletypes.py
--rw-r--r--   0        0        0    13797 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/prototypes.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/reporters.py
--rw-r--r--   0        0        0    32992 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/simulator.py
--rw-r--r--   0        0        0    18097 2020-02-02 00:00:00.000000 simpn-1.1.0/simpn/visualisation.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simpn-1.1.0/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 simpn-1.1.0/LICENSE
--rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 simpn-1.1.0/README.rst
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 simpn-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 simpn-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 simpn-1.2.0/CHANGELOG.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/immutabletypes.py
+-rw-r--r--   0        0        0    13797 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/prototypes.py
+-rw-r--r--   0        0        0    16831 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/prototypes_queueing.py
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/reporters.py
+-rw-r--r--   0        0        0    33413 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/simulator.py
+-rw-r--r--   0        0        0    18193 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/visualisation.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simpn-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 simpn-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 simpn-1.2.0/README.rst
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 simpn-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 simpn-1.2.0/PKG-INFO
```

### Comparing `simpn-1.1.0/simpn/prototypes.py` & `simpn-1.2.0/simpn/prototypes.py`

 * *Files identical despite different names*

### Comparing `simpn-1.1.0/simpn/reporters.py` & `simpn-1.2.0/simpn/reporters.py`

 * *Files identical despite different names*

### Comparing `simpn-1.1.0/simpn/simulator.py` & `simpn-1.2.0/simpn/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 from sortedcontainers import SortedList
+import simpn.visualisation as vis
 
 
 class SimVar:
     """
     A simulation variable SimVar has an identifier and a marking.
     A simulation variable can have multiple values. These values are available at particular times.
     For example, a variable van have the value 1 at time 0 (denoted as 1@0) and also 2@0.
@@ -81,14 +82,16 @@
             self._time = 0
             self.marking.clear()
             for token in self.checkpoints[name]:
                 self.add_token(token)
         else:
             raise LookupError("No checkpoint '" + name + "' at place '" + str(self) + "'.")
 
+    def get_visualisation(self):
+        return vis.PlaceViz(self)
 
 class SimVarQueue(SimVar):
     """
     A simulation variable that contains the queue of tokens from another SimVar.
     The identifier of this SimVar is <simvar_id>.queue, where simvar_id is the _id of the SimVar of which it contains the queue.
     Regular SimVar have a queue property that refers to their SimVarQueue variable.
     """
@@ -229,14 +232,16 @@
 
     def __str__(self):
         return self._id
 
     def __repr__(self):
         return self.__str__()
 
+    def get_visualisation(self):
+        return vis.TransitionViz(self)
 
 class SimToken:
     """
     A token SimToken, which is a possible value of a SimVar. A token has a value and the time at which this value is available in a SimVar.
     When the SimToken is used as the return value of an event behavior, the delay can be used. This represents the delay with which the value will be available.
     The value will then be available at <time of event> + <delay>.
 
@@ -344,28 +349,36 @@
         """
         Creates a new SimVar with the specified name as identifier. Adds the SimVar to the problem and returns it.
 
         :param name: a name for the SimVar.
         :param priority: a function that takes a token as input and returns a value that is used to sort the tokens in the order in which they will be processed (lower values first). The default is processing in the order of the time of the token.
         :return: a SimVar with the specified name as identifier.
         """
+        # Generate and add SimVar
+        result = SimVar(name, priority=priority)
+        self.add_prototype_var(result)
+        return result
+
+    def add_prototype_var(self, var):
+        """
+        Adds the SimVar to the problem. This function should only be used for prototypes.
+        """
         # Check name
+        name = var.get_id()
         if name in self.id2node:
             raise TypeError("Node with name " + name + " already exists. Names must be unique.")
         if name.endswith(SimVarQueue.QUEUE_SUFFIX):
             raise TypeError("Cannot create SimVar with name " + name + ". Names ending with " + SimVarQueue.QUEUE_SUFFIX + " are reserved for SimVar queues. They are automatically generated.")
         if name == SimVarTime.TIME_ID:
             raise TypeError("Cannot create SimVar with name " + name + ". " + SimVarTime.TIME_ID + " is reserved for the time variable. If you just want to get the time variable, use the .var() method instead.")
 
-        # Generate and add SimVar
-        result = SimVar(name, priority=priority)
-        self.places.append(result)
-        self.id2node[name] = result
+        # Add SimVar
+        self.places.append(var)
+        self.id2node[name] = var
 
-        return result
 
     def var(self, name):
         """
         Returns the SimVar with the given name.
         Raises an error if no such SimVar exists.
 
         :param name: the name of the SimVar.
```

### Comparing `simpn-1.1.0/simpn/visualisation.py` & `simpn-1.2.0/simpn/visualisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import igraph
 import os
+import traceback
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = "hide"
 import pygame
 from enum import Enum, auto
 
 
 MAX_SIZE = 1920, 1080
 # colors
@@ -249,18 +250,18 @@
             viznodes_with_edges.append(prototype_viznode)
             for event in prototype.events:
                 element_to_prototype[event.get_id()] = prototype.get_id()
             for place in prototype.places:
                 element_to_prototype[place.get_id()] = prototype.get_id()
         for var in self._problem.places:
             if var.get_id() not in element_to_prototype:
-                self._nodes[var.get_id()] = PlaceViz(var)
+                self._nodes[var.get_id()] = var.get_visualisation()
         for event in self._problem.events:
             if event.get_id() not in element_to_prototype:
-                event_viznode = TransitionViz(event)
+                event_viznode = event.get_visualisation()
                 self._nodes[event.get_id()] = event_viznode
                 viznodes_with_edges.append(event_viznode)                
         # Add visualization for edges.
         # If an edge is from or to a prototype element, it must be from or to the prototype itself.
         for viznode in viznodes_with_edges:
             for incoming in viznode._model_node.incoming:
                 node_id = incoming.get_id()
@@ -333,15 +334,15 @@
         for edge in self._edges:            
             graph.add_edge(edge.get_start_node().get_id(), edge.get_end_node().get_id())
         layout = graph.layout_sugiyama()
         layout.rotate(-90)
         layout.scale(NODE_SPACING)
         boundaries = layout.boundaries(border=STANDARD_NODE_WIDTH)
         layout.translate(-boundaries[0][0], -boundaries[0][1])
-        canvas_size = layout.boundaries(border=STANDARD_NODE_WIDTH)[1]
+        canvas_size = layout.boundaries(border=STANDARD_NODE_WIDTH*2)[1]
         self._size = (min(MAX_SIZE[0], canvas_size[0]), min(MAX_SIZE[1], canvas_size[1]))
         i = 0
         for v in graph.vs:
             xy = layout[i]
             xy  = (round(xy[0]/GRID_SPACING)*GRID_SPACING, round(xy[1]/GRID_SPACING)*GRID_SPACING)
             self._nodes[v["name"]].set_pos(xy)
             i += 1
@@ -423,13 +424,14 @@
             
             self.__running = True
             while self.__running:
                 for event in pygame.event.get():
                     self.__handle_event(event)
                 try:
                     self.__draw()
-                except:
+                except Exception:
                     print("Error while drawing the visualisation.")
+                    print(traceback.format_exc())
                     self.__running = False
                 clock.tick(30)
 
             pygame.quit()
```

### Comparing `simpn-1.1.0/.gitignore` & `simpn-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simpn-1.1.0/LICENSE` & `simpn-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpn-1.1.0/README.rst` & `simpn-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `simpn-1.1.0/pyproject.toml` & `simpn-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simpn"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Remco Dijkman", email="r.m.dijkman@tue.nl" },
 ]
 description = "A package for Discrete Event Simulation, using the theory of Petri Nets."
 readme = "README.rst"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `simpn-1.1.0/PKG-INFO` & `simpn-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: simpn
-Version: 1.1.0
+Version: 1.2.0
 Summary: A package for Discrete Event Simulation, using the theory of Petri Nets.
 Project-URL: Homepage, https://github.com/bpogroup/simpn
 Project-URL: Documentation, https://bpogroup.github.io/simpn/
 Author-email: Remco Dijkman <r.m.dijkman@tue.nl>
 License: Copyright (c) 2023 Remco Dijkman (Eindhoven University of Technology)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


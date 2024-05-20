# Comparing `tmp/fuel_efficiency-0.1.3.tar.gz` & `tmp/fuel_efficiency-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuel_efficiency-0.1.3.tar", max compression
+gzip compressed data, was "fuel_efficiency-0.1.4.tar", max compression
```

## Comparing `fuel_efficiency-0.1.3.tar` & `fuel_efficiency-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5316 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/__init__.py
--rw-r--r--   0        0        0     3622 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/a_star.py
--rw-r--r--   0        0        0     1949 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/context.py
--rw-r--r--   0        0        0     3164 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/dijkstra.py
--rw-r--r--   0        0        0      509 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/path_finding.py
--rw-r--r--   0        0        0        0 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/__init__.py
--rw-r--r--   0        0        0      974 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/down_hill.py
--rw-r--r--   0        0        0     2125 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/node.py
--rw-r--r--   0        0        0      971 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/plateau.py
--rw-r--r--   0        0        0     1812 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/position.py
--rw-r--r--   0        0        0      970 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/up_hill.py
--rw-r--r--   0        0        0      970 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/valley.py
--rw-r--r--   0        0        0     1569 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6090 1970-01-01 00:00:00.000000 fuel_efficiency-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5316 2024-05-20 16:22:36.029229 fuel_efficiency-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/algorithms/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/algorithms/a_star.py
+-rw-r--r--   0        0        0     1949 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/algorithms/context.py
+-rw-r--r--   0        0        0     3671 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/algorithms/dijkstra.py
+-rw-r--r--   0        0        0      697 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/algorithms/path_finding.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/entities/__init__.py
+-rw-r--r--   0        0        0      974 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/entities/down_hill.py
+-rw-r--r--   0        0        0     2125 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/entities/node.py
+-rw-r--r--   0        0        0      971 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/entities/plateau.py
+-rw-r--r--   0        0        0     1812 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/entities/position.py
+-rw-r--r--   0        0        0      970 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/entities/up_hill.py
+-rw-r--r--   0        0        0      970 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/fuel_efficiency/entities/valley.py
+-rw-r--r--   0        0        0     1679 2024-05-20 16:22:36.033229 fuel_efficiency-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6090 1970-01-01 00:00:00.000000 fuel_efficiency-0.1.4/PKG-INFO
```

### Comparing `fuel_efficiency-0.1.3/README.md` & `fuel_efficiency-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.3/fuel_efficiency/algorithms/a_star.py` & `fuel_efficiency-0.1.4/fuel_efficiency/algorithms/dijkstra.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,82 @@
 import heapq
-from typing import List
+import math
+from typing import List, Tuple
 
 from fuel_efficiency.algorithms.path_finding import PathfindingStrategy
 from fuel_efficiency.entities.node import Node
 from fuel_efficiency.entities.position import Position
 
 
-class AStarStrategy(PathfindingStrategy):
-    """
-    A class used to represent a Position (x,y)
+class DijkstraStrategy(PathfindingStrategy):
 
-    A ``Position(x,y)`` is a position on a grid with x axis and y axis.
-
-    This class uses ``dataclasses`` that provides a decorator and functions for automatically adding generated special
-    methods such as ``__init__()`` and ``__repr__()``
-
-    Attributes:
-        x (int): position value on x-axis
-        y (int): position value on x-axis
-    """
-
-    allowed_directions = [
+    cardinal_directions = [
+        Position(-1, -1),
         Position(-1, 0),
+        Position(-1, 1),
         Position(0, -1),
         Position(0, 1),
+        Position(1, -1),
         Position(1, 0),
+        Position(1, 1),
     ]
 
     def find_path(grid: List[List[Node]], start: Node, end: Node):
+
         rows, cols = len(grid), len(grid[0])
         distances = [[float('inf')] * cols for _ in range(rows)]
         distances[start.position.x][start.position.y] = grid[start.position.x][
             start.position.y
         ].weight
 
         previous = [[None] * cols for _ in range(rows)]
 
-        pq = [
-            (
-                grid[start.position.x][start.position.y].weight
-                + AStarStrategy.calculate_distance(start, end),
-                start,
-            )
-        ]
-
-        while pq:
-            current_distance, current_node = heapq.heappop(pq)
-            if current_node == end:
-                path = []
-                while current_node is not start:
-                    path.append(current_node)
-                    current_node = previous[current_node.position.x][
-                        current_node.position.y
-                    ]
-
-                return path[::-1]  # reversed path
+        pq = [(grid[start.position.x][start.position.y].weight, start)]
 
-            for neighbor in AStarStrategy.get_neighbors(grid, current_node):
-                new_distance = current_distance + neighbor.weight
+        if start != end:
+            while pq:
+                current_distance, current_node = heapq.heappop(pq)
+                if current_node == end:
+                    path = []
+                    while current_node is not start:
+                        path.append(current_node)
+                        current_node = previous[current_node.position.x][
+                            current_node.position.y
+                        ]
+                    return path[::-1]  # reversed path
 
-                if (
-                    new_distance
-                    < distances[neighbor.position.x][neighbor.position.y]
+                for neighbor in DijkstraStrategy.get_neighbors(
+                    grid, current_node
                 ):
-                    distances[neighbor.position.x][
-                        neighbor.position.y
-                    ] = new_distance
-                    previous[neighbor.position.x][
-                        neighbor.position.y
-                    ] = current_node
-                    heapq.heappush(
-                        pq,
-                        (
-                            new_distance
-                            + AStarStrategy.calculate_distance(neighbor, end),
-                            neighbor,
-                        ),
+                    new_distance = current_distance + (
+                        neighbor.weight
+                        * DijkstraStrategy.calculate_distance(
+                            current_node, neighbor
+                        )
                     )
 
+                    if (
+                        new_distance
+                        < distances[neighbor.position.x][neighbor.position.y]
+                    ):
+                        distances[neighbor.position.x][
+                            neighbor.position.y
+                        ] = new_distance
+                        previous[neighbor.position.x][
+                            neighbor.position.y
+                        ] = current_node
+                        heapq.heappush(pq, (new_distance, neighbor))
+
         return []
 
     def get_neighbors(grid: List[List[Node]], node: Node) -> List[Node]:
         neighbors_list = []
         grid_xlen = len(grid)
         grid_ylen = len(grid[0])
-        for direction in AStarStrategy.allowed_directions:
+        for direction in DijkstraStrategy.cardinal_directions:
             if (
                 ((node.position.x + direction.x) >= 0)
                 and ((node.position.y + direction.y) >= 0)
             ) and (
                 ((node.position.x + direction.x) < grid_xlen)
                 and ((node.position.y + direction.y) < grid_ylen)
             ):
@@ -97,11 +85,21 @@
                         node.position.y + direction.y
                     ]
                 )
 
         return neighbors_list
 
     def calculate_distance(node1: Node, node2: Node) -> float:
-        # Manhattan distance
-        return abs(node1.position.x - node2.position.x) + abs(
-            node1.position.y - node2.position.y
+        # Euclidean distance
+        return math.sqrt(
+            (node2.position.x - node1.position.x) ** 2
+            + (node2.position.y - node1.position.y) ** 2
         )
+
+    def calculate_fuel_consumption(
+        grid: List[List[Node]], start: Node, end: Node
+    ) -> Tuple[float, List[Node]]:
+        path = DijkstraStrategy.find_path(grid, start, end)
+        fuel_consumption = 0
+        for node in path:
+            fuel_consumption += node.weight
+        return fuel_consumption, path
```

### Comparing `fuel_efficiency-0.1.3/fuel_efficiency/algorithms/context.py` & `fuel_efficiency-0.1.4/fuel_efficiency/algorithms/context.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.3/fuel_efficiency/entities/down_hill.py` & `fuel_efficiency-0.1.4/fuel_efficiency/entities/down_hill.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.3/fuel_efficiency/entities/node.py` & `fuel_efficiency-0.1.4/fuel_efficiency/entities/node.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.3/fuel_efficiency/entities/plateau.py` & `fuel_efficiency-0.1.4/fuel_efficiency/entities/plateau.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.3/fuel_efficiency/entities/position.py` & `fuel_efficiency-0.1.4/fuel_efficiency/entities/position.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.3/fuel_efficiency/entities/up_hill.py` & `fuel_efficiency-0.1.4/fuel_efficiency/entities/up_hill.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.3/fuel_efficiency/entities/valley.py` & `fuel_efficiency-0.1.4/fuel_efficiency/entities/valley.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.3/pyproject.toml` & `fuel_efficiency-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fuel-efficiency"
-version = "0.1.3"
+version = "0.1.4"
 description = "Fuel efficiency challenge test"
 license = "Proprietary"
 authors = ["Guilherme Lima <guimarotto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fuel_efficiency"}]
 classifiers = [
     "Topic :: Software Development",
@@ -51,10 +51,12 @@
 lint = "blue --check --diff . && isort --check --diff ."
 docs = "mkdocs serve"
 pre_test = "task lint"
 test = "pytest -s -x --cov=fuel_efficiency -vv"
 test_entities = "pytest tests/test_entities.py -s -x -vv"
 test_entities_raise = "pytest tests/test_entities_raise.py -s -x -vv"
 test_algorithms = "pytest tests/test_algorithms.py -s -x -vv"
+test_astar = "pytest tests/test_astar.py -s -x -vv"
+test_dijkstra = "pytest tests/test_dijkstra.py -s -x -vv"
 post_test =  "coverage html"
 build = "poetry build"
 publish = "poetry publish"
```

### Comparing `fuel_efficiency-0.1.3/PKG-INFO` & `fuel_efficiency-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuel-efficiency
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fuel efficiency challenge test
 License: Proprietary
 Author: Guilherme Lima
 Author-email: guimarotto@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```


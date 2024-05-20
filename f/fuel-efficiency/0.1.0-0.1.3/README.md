# Comparing `tmp/fuel_efficiency-0.1.0.tar.gz` & `tmp/fuel_efficiency-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuel_efficiency-0.1.0.tar", max compression
+gzip compressed data, was "fuel_efficiency-0.1.3.tar", max compression
```

## Comparing `fuel_efficiency-0.1.0.tar` & `fuel_efficiency-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      476 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/algorithms/__init__.py
--rw-r--r--   0        0        0     3622 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/algorithms/a_star.py
--rw-r--r--   0        0        0     1949 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/algorithms/context.py
--rw-r--r--   0        0        0     3164 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/algorithms/dijkstra.py
--rw-r--r--   0        0        0      509 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/algorithms/path_finding.py
--rw-r--r--   0        0        0        0 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/entities/__init__.py
--rw-r--r--   0        0        0      974 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/entities/down_hill.py
--rw-r--r--   0        0        0     2125 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/entities/node.py
--rw-r--r--   0        0        0      971 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/entities/plateau.py
--rw-r--r--   0        0        0     1812 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/entities/position.py
--rw-r--r--   0        0        0      970 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/entities/up_hill.py
--rw-r--r--   0        0        0      970 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/fuel_efficiency/entities/valley.py
--rw-r--r--   0        0        0     1570 2024-05-20 12:39:32.750512 fuel_efficiency-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 fuel_efficiency-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5316 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/__init__.py
+-rw-r--r--   0        0        0     3622 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/a_star.py
+-rw-r--r--   0        0        0     1949 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/context.py
+-rw-r--r--   0        0        0     3164 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/dijkstra.py
+-rw-r--r--   0        0        0      509 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/algorithms/path_finding.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/__init__.py
+-rw-r--r--   0        0        0      974 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/down_hill.py
+-rw-r--r--   0        0        0     2125 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/node.py
+-rw-r--r--   0        0        0      971 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/plateau.py
+-rw-r--r--   0        0        0     1812 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/position.py
+-rw-r--r--   0        0        0      970 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/up_hill.py
+-rw-r--r--   0        0        0      970 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/fuel_efficiency/entities/valley.py
+-rw-r--r--   0        0        0     1569 2024-05-20 13:36:51.254993 fuel_efficiency-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6090 1970-01-01 00:00:00.000000 fuel_efficiency-0.1.3/PKG-INFO
```

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/algorithms/a_star.py` & `fuel_efficiency-0.1.3/fuel_efficiency/algorithms/a_star.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/algorithms/context.py` & `fuel_efficiency-0.1.3/fuel_efficiency/algorithms/context.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/algorithms/dijkstra.py` & `fuel_efficiency-0.1.3/fuel_efficiency/algorithms/dijkstra.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/entities/down_hill.py` & `fuel_efficiency-0.1.3/fuel_efficiency/entities/down_hill.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/entities/node.py` & `fuel_efficiency-0.1.3/fuel_efficiency/entities/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 
 @dataclass(slots=True, eq=False)
 class Node(Protocol):
     """
     A class used to represent a Node
 
-    A Node contain a ``Position(x,y)`` that is a position on a grid and a ``weight`` that represents the weight for a vehicle to move through different
-    terrains, that affects its fuel efficiency.
+    A Node contain a ``Position(x,y)`` that is a position on a grid and a ``weight`` that represents the weight for a
+    vehicle to move through different terrains, that affects its fuel efficiency.
 
     This class uses ``dataclasses`` that provides a decorator and functions for automatically adding generated special
     methods such as ``__init__()`` and ``__repr__()``
 
     Attributes:
         weight (float): position value on x-axis
         position (Position): position value on x-axis
```

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/entities/plateau.py` & `fuel_efficiency-0.1.3/fuel_efficiency/entities/plateau.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/entities/position.py` & `fuel_efficiency-0.1.3/fuel_efficiency/entities/position.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/entities/up_hill.py` & `fuel_efficiency-0.1.3/fuel_efficiency/entities/up_hill.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.0/fuel_efficiency/entities/valley.py` & `fuel_efficiency-0.1.3/fuel_efficiency/entities/valley.py`

 * *Files identical despite different names*

### Comparing `fuel_efficiency-0.1.0/pyproject.toml` & `fuel_efficiency-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "fuel-efficiency"
-version = "0.1.0"
-description = "Fueel efficiency challenge test"
+version = "0.1.3"
+description = "Fuel efficiency challenge test"
 license = "Proprietary"
 authors = ["Guilherme Lima <guimarotto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fuel_efficiency"}]
 classifiers = [
     "Topic :: Software Development",
     "Environment :: Console",
```


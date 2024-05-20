# Comparing `tmp/gmsh_scripts-0.4.3.tar.gz` & `tmp/gmsh_scripts-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmsh_scripts-0.4.3.tar", last modified: Wed May  8 17:53:22 2024, max compression
+gzip compressed data, was "gmsh_scripts-0.4.4.tar", last modified: Mon May 20 09:33:44 2024, max compression
```

## Comparing `gmsh_scripts-0.4.3.tar` & `gmsh_scripts-0.4.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:22.043471 gmsh_scripts-0.4.3/
--rw-rw-rw-   0        0        0    19460 2024-01-18 21:14:31.000000 gmsh_scripts-0.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     6170 2024-05-08 17:53:22.042474 gmsh_scripts-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5506 2024-02-27 20:31:22.000000 gmsh_scripts-0.4.3/README.md
--rw-rw-rw-   0        0        0      139 2024-05-08 17:47:31.000000 gmsh_scripts-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0      738 2024-05-08 17:53:22.053446 gmsh_scripts-0.4.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.373236 gmsh_scripts-0.4.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.510824 gmsh_scripts-0.4.3/src/gmsh_scripts/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/__init__.py
--rw-rw-rw-   0        0        0      442 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.669402 gmsh_scripts-0.4.3/src/gmsh_scripts/block/
--rw-rw-rw-   0        0        0      244 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/block/__init__.py
--rw-rw-rw-   0        0        0    32578 2024-05-08 17:33:49.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/block/block.py
--rw-rw-rw-   0        0        0    29630 2024-02-27 19:18:54.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/block/layer.py
--rw-rw-rw-   0        0        0    13353 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/block/matrix.py
--rw-rw-rw-   0        0        0     5716 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/block/polyhedron.py
--rw-rw-rw-   0        0        0    11729 2024-02-27 19:18:51.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/block/quarter_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.678379 gmsh_scripts-0.4.3/src/gmsh_scripts/boolean/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/boolean/__init__.py
--rw-rw-rw-   0        0        0     1601 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/boolean/boolean.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.698396 gmsh_scripts-0.4.3/src/gmsh_scripts/coordinate_system/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/coordinate_system/__init__.py
--rw-rw-rw-   0        0        0    20061 2024-01-19 11:07:34.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/coordinate_system/coordinate_system.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.816079 gmsh_scripts-0.4.3/src/gmsh_scripts/entity/
--rw-rw-rw-   0        0        0      379 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/entity/__init__.py
--rw-rw-rw-   0        0        0      767 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/entity/curve.py
--rw-rw-rw-   0        0        0      646 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/entity/curve_loop.py
--rw-rw-rw-   0        0        0    10085 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/entity/point.py
--rw-rw-rw-   0        0        0      763 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/entity/surface.py
--rw-rw-rw-   0        0        0      536 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/entity/surface_loop.py
--rw-rw-rw-   0        0        0      771 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/entity/volume.py
--rw-rw-rw-   0        0        0     4951 2024-01-19 10:40:45.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/factory.py
--rw-rw-rw-   0        0        0      328 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/load.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.834032 gmsh_scripts-0.4.3/src/gmsh_scripts/optimize/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/optimize/__init__.py
--rw-rw-rw-   0        0        0     3240 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/optimize/optimize.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.846998 gmsh_scripts-0.4.3/src/gmsh_scripts/parse/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/parse/__init__.py
--rw-rw-rw-   0        0        0    40863 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/parse/parse.py
--rw-rw-rw-   0        0        0     3345 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.855974 gmsh_scripts-0.4.3/src/gmsh_scripts/quadrate/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/quadrate/__init__.py
--rw-rw-rw-   0        0        0     1276 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/quadrate/quadrate.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.865946 gmsh_scripts-0.4.3/src/gmsh_scripts/refine/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/refine/__init__.py
--rw-rw-rw-   0        0        0      762 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/refine/refine.py
--rw-rw-rw-   0        0        0    20940 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/registry.py
--rw-rw-rw-   0        0        0     8196 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/run.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.877917 gmsh_scripts-0.4.3/src/gmsh_scripts/size/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/size/__init__.py
--rw-rw-rw-   0        0        0     5205 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/size/size.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.886891 gmsh_scripts-0.4.3/src/gmsh_scripts/smooth/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/smooth/__init__.py
--rw-rw-rw-   0        0        0     1773 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/smooth/smooth.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.898858 gmsh_scripts-0.4.3/src/gmsh_scripts/strategy/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/strategy/__init__.py
--rw-rw-rw-   0        0        0     8647 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/strategy/strategy.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.907835 gmsh_scripts-0.4.3/src/gmsh_scripts/structure/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/structure/__init__.py
--rw-rw-rw-   0        0        0     7321 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/structure/structure.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.919802 gmsh_scripts-0.4.3/src/gmsh_scripts/support/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/support/__init__.py
--rw-rw-rw-   0        0        0    31989 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/support/support.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:21.957702 gmsh_scripts-0.4.3/src/gmsh_scripts/transform/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/transform/__init__.py
--rw-rw-rw-   0        0        0    25233 2024-01-19 14:17:38.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/transform/transform.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:22.001583 gmsh_scripts-0.4.3/src/gmsh_scripts/utils/
--rw-rw-rw-   0        0        0       65 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/utils/__init__.py
--rw-rw-rw-   0        0        0      924 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/utils/obj2gmsh.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:22.039482 gmsh_scripts-0.4.3/src/gmsh_scripts/zone/
--rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/zone/__init__.py
--rw-rw-rw-   0        0        0    15868 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.3/src/gmsh_scripts/zone/zone.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:53:22.041479 gmsh_scripts-0.4.3/src/gmsh_scripts.egg-info/
--rw-rw-rw-   0        0        0     6170 2024-05-08 17:53:21.000000 gmsh_scripts-0.4.3/src/gmsh_scripts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2141 2024-05-08 17:53:21.000000 gmsh_scripts-0.4.3/src/gmsh_scripts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 17:53:21.000000 gmsh_scripts-0.4.3/src/gmsh_scripts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-08 17:53:21.000000 gmsh_scripts-0.4.3/src/gmsh_scripts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-08 17:53:21.000000 gmsh_scripts-0.4.3/src/gmsh_scripts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.462008 gmsh_scripts-0.4.4/
+-rw-rw-rw-   0        0        0    19460 2024-01-18 21:14:31.000000 gmsh_scripts-0.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     6170 2024-05-20 09:33:44.460996 gmsh_scripts-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5506 2024-02-27 20:31:22.000000 gmsh_scripts-0.4.4/README.md
+-rw-rw-rw-   0        0        0      139 2024-05-08 17:47:31.000000 gmsh_scripts-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0      738 2024-05-20 09:33:44.492036 gmsh_scripts-0.4.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:42.346994 gmsh_scripts-0.4.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:42.637982 gmsh_scripts-0.4.4/src/gmsh_scripts/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/__init__.py
+-rw-rw-rw-   0        0        0      442 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:43.196035 gmsh_scripts-0.4.4/src/gmsh_scripts/block/
+-rw-rw-rw-   0        0        0      244 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/block/__init__.py
+-rw-rw-rw-   0        0        0    32578 2024-05-08 17:33:49.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/block/block.py
+-rw-rw-rw-   0        0        0    27490 2024-05-20 09:23:27.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/block/layer.py
+-rw-rw-rw-   0        0        0    13353 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/block/matrix.py
+-rw-rw-rw-   0        0        0     5716 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/block/polyhedron.py
+-rw-rw-rw-   0        0        0    13918 2024-05-20 09:29:17.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/block/quarter_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:43.232942 gmsh_scripts-0.4.4/src/gmsh_scripts/boolean/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/boolean/__init__.py
+-rw-rw-rw-   0        0        0     1601 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/boolean/boolean.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:43.251885 gmsh_scripts-0.4.4/src/gmsh_scripts/coordinate_system/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/coordinate_system/__init__.py
+-rw-rw-rw-   0        0        0    20061 2024-01-19 11:07:34.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/coordinate_system/coordinate_system.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:43.779691 gmsh_scripts-0.4.4/src/gmsh_scripts/entity/
+-rw-rw-rw-   0        0        0      379 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/entity/__init__.py
+-rw-rw-rw-   0        0        0      767 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/entity/curve.py
+-rw-rw-rw-   0        0        0      646 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/entity/curve_loop.py
+-rw-rw-rw-   0        0        0    10085 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/entity/point.py
+-rw-rw-rw-   0        0        0      763 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/entity/surface.py
+-rw-rw-rw-   0        0        0      536 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/entity/surface_loop.py
+-rw-rw-rw-   0        0        0      771 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/entity/volume.py
+-rw-rw-rw-   0        0        0     4951 2024-01-19 10:40:45.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/factory.py
+-rw-rw-rw-   0        0        0      328 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/load.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:43.792656 gmsh_scripts-0.4.4/src/gmsh_scripts/optimize/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:32.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/optimize/__init__.py
+-rw-rw-rw-   0        0        0     3240 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/optimize/optimize.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:43.831205 gmsh_scripts-0.4.4/src/gmsh_scripts/parse/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/parse/__init__.py
+-rw-rw-rw-   0        0        0    40863 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/parse/parse.py
+-rw-rw-rw-   0        0        0     3345 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:43.971605 gmsh_scripts-0.4.4/src/gmsh_scripts/quadrate/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/quadrate/__init__.py
+-rw-rw-rw-   0        0        0     1276 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/quadrate/quadrate.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.067105 gmsh_scripts-0.4.4/src/gmsh_scripts/refine/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/refine/__init__.py
+-rw-rw-rw-   0        0        0      762 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/refine/refine.py
+-rw-rw-rw-   0        0        0    20940 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/registry.py
+-rw-rw-rw-   0        0        0     8196 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/run.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.082065 gmsh_scripts-0.4.4/src/gmsh_scripts/size/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/size/__init__.py
+-rw-rw-rw-   0        0        0     5205 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/size/size.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.115409 gmsh_scripts-0.4.4/src/gmsh_scripts/smooth/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/smooth/__init__.py
+-rw-rw-rw-   0        0        0     1773 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/smooth/smooth.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.169575 gmsh_scripts-0.4.4/src/gmsh_scripts/strategy/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/strategy/__init__.py
+-rw-rw-rw-   0        0        0     8647 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/strategy/strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.186650 gmsh_scripts-0.4.4/src/gmsh_scripts/structure/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/structure/__init__.py
+-rw-rw-rw-   0        0        0     7321 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/structure/structure.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.257244 gmsh_scripts-0.4.4/src/gmsh_scripts/support/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/support/__init__.py
+-rw-rw-rw-   0        0        0    31989 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/support/support.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.306299 gmsh_scripts-0.4.4/src/gmsh_scripts/transform/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/transform/__init__.py
+-rw-rw-rw-   0        0        0    25233 2024-01-19 14:17:38.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/transform/transform.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.427924 gmsh_scripts-0.4.4/src/gmsh_scripts/utils/
+-rw-rw-rw-   0        0        0       65 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/utils/__init__.py
+-rw-rw-rw-   0        0        0      924 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/utils/obj2gmsh.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.457028 gmsh_scripts-0.4.4/src/gmsh_scripts/zone/
+-rw-rw-rw-   0        0        0        0 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/zone/__init__.py
+-rw-rw-rw-   0        0        0    15868 2024-01-18 21:14:33.000000 gmsh_scripts-0.4.4/src/gmsh_scripts/zone/zone.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:33:44.459002 gmsh_scripts-0.4.4/src/gmsh_scripts.egg-info/
+-rw-rw-rw-   0        0        0     6170 2024-05-20 09:33:42.000000 gmsh_scripts-0.4.4/src/gmsh_scripts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2141 2024-05-20 09:33:42.000000 gmsh_scripts-0.4.4/src/gmsh_scripts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:33:42.000000 gmsh_scripts-0.4.4/src/gmsh_scripts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-20 09:33:42.000000 gmsh_scripts-0.4.4/src/gmsh_scripts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-20 09:33:42.000000 gmsh_scripts-0.4.4/src/gmsh_scripts.egg-info/top_level.txt
```

### Comparing `gmsh_scripts-0.4.3/LICENSE.txt` & `gmsh_scripts-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/PKG-INFO` & `gmsh_scripts-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsh-scripts
-Version: 0.4.3
+Version: 0.4.4
 Summary: Scripts for GMSH mesh generator
 Home-page: https://github.com/romanzes637/gmsh_scripts
 Author: Roman Pashkovsky
 Author-email: romapasky@gmail.com
 Project-URL: Bug Tracker, https://github.com/romanzes637/gmsh_scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gmsh-scripts Version: 0.4.3 Summary: Scripts for
+Metadata-Version: 2.1 Name: gmsh-scripts Version: 0.4.4 Summary: Scripts for
 GMSH mesh generator Home-page: https://github.com/romanzes637/gmsh_scripts
 Author: Roman Pashkovsky Author-email: romapasky@gmail.com Project-URL: Bug
 Tracker, https://github.com/romanzes637/gmsh_scripts/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
 Dist: gmsh Requires-Dist: numpy Requires-Dist: pyyaml Provides-Extra: viz
```

### Comparing `gmsh_scripts-0.4.3/README.md` & `gmsh_scripts-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/setup.cfg` & `gmsh_scripts-0.4.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6d73 682d 7363 7269 7074 730d   = gmsh-scripts.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 2e33  .version = 0.4.3
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 2e34  .version = 0.4.4
 00000030: 0d0a 6175 7468 6f72 203d 2052 6f6d 616e  ..author = Roman
 00000040: 2050 6173 686b 6f76 736b 790d 0a61 7574   Pashkovsky..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 726f 6d61  hor_email = roma
 00000060: 7061 736b 7940 676d 6169 6c2e 636f 6d0d  pasky@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2053  .description = S
 00000080: 6372 6970 7473 2066 6f72 2047 4d53 4820  cripts for GMSH 
 00000090: 6d65 7368 2067 656e 6572 6174 6f72 0d0a  mesh generator..
```

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/block/block.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/block/block.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/block/layer.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/block/layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,83 +189,36 @@
                     new_li = (i, j)
                     old_li = n2o_l2l_l2l[new_li]
                     new_item = old_layers[old_li[0]][old_li[1]]
                     new_layer_items.append(new_item)
                 new_layers.append(new_layer_items)
         return new_layers
 
-    # @staticmethod
-    # def parse_layers_block_map(m, default, new2old, item_types=()):
-    #     # Default value for all items if map is None
-    #     if m is None:
-    #         m = [default for _ in new2old]
-    #         return m
-    #     m = list(flatten(m)) if isinstance(m, list) else m
-    #     # Check on single item of type in item_types
-    #     for t in item_types:
-    #         if isinstance(t, list) and isinstance(m, list):  # list of ...
-    #             if all(isinstance(ti, mi) for ti in t for mi in m):
-    #                 m = [m for _ in new2old]
-    #                 return m
-    #         elif isinstance(m, t):  # non list types
-    #             m = [m for _ in new2old]
-    #             return m
-    #     # Old list to new list
-    #     if isinstance(m, list):
-    #         m = [m[x[0]] if x is not None else default for x in new2old]
-    #         return m
-    #     else:  # Something wrong
-    #         raise ValueError(m)
-
     @staticmethod
-    def parse_layers_block_map(m, default, new2old, item_types=(), center_mask=None):
+    def parse_layers_block_map(m, default, new2old, item_types=()):
         # Default value for all items if map is None
         if m is None:
-            n = [default for _ in new2old]
-            return n
+            m = [default for _ in new2old]
+            return m
         m = list(flatten(m)) if isinstance(m, list) else m
-        # Old list to new list
-        old2new = {}
-        for new, old in enumerate(new2old):
-            if old is not None:
-                old2new.setdefault(old[0], []).append(new)
         # Check on single item of type in item_types
         for t in item_types:
             if isinstance(t, list) and isinstance(m, list):  # list of ...
                 if all(isinstance(ti, mi) for ti in t for mi in m):
-                    max_old = max(x[0] for x in new2old if x is not None)
-                    m = [m for _ in range(max_old + 1)]
-                    break
+                    m = [m for _ in new2old]
+                    return m
             elif isinstance(m, t):  # non list types
-                max_old = max(x[0] for x in new2old if x is not None)
-                m = [m for _ in range(max_old + 1)]
-                break
-        n = [default for _ in new2old]
-        for mi, mm in enumerate(m):
-            nis = old2new[mi]
-            if len(nis) == 1 and center_mask is not None:  # center
-                mm = center_mask
-            if isinstance(mm, str):
-                if float in item_types:
-                    mm = [float(x) for x in mm.split(',')]
-                elif int in item_types:
-                    mm = [int(x) for x in mm.split(',')]
-                elif bool in item_types:
-                    mm = [bool(x) for x in mm.split(',')]
-                else:
-                    mm = [x for x in mm.split(',')]
-            else:
-                mm = [mm for _ in range(4)]
-            masks = [mm[2], mm[0], mm[1], mm[3]]  # NX, X, NY, Y -> NY, NX, X, Y
-            if len(nis) == len(masks):  # layers
-                for ni, mask in zip(nis, masks):
-                    n[ni] = mask
-            elif len(nis) == 1:  # center
-                n[nis[0]] = masks[0]
-        return n
+                m = [m for _ in new2old]
+                return m
+        # Old list to new list
+        if isinstance(m, list):
+            m = [m[x[0]] if x is not None else default for x in new2old]
+            return m
+        else:  # Something wrong
+            raise ValueError(m)
 
     @staticmethod
     def parse_layers_block_mask(m, default, new2old, item_types=(), center_mask=None):
         # Default value for all items if map is None
         if m is None:
             n = [default for _ in new2old]
             return n
```

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/block/matrix.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/block/matrix.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/block/polyhedron.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/block/polyhedron.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/boolean/boolean.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/boolean/boolean.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/coordinate_system/coordinate_system.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/coordinate_system/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/entity/curve.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/entity/curve.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/entity/curve_loop.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/entity/curve_loop.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/entity/point.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/entity/point.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/entity/surface.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/entity/surface.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/entity/surface_loop.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/entity/surface_loop.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/entity/volume.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/entity/volume.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/factory.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/factory.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/optimize/optimize.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/parse/parse.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/parse/parse.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/plot.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/plot.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/quadrate/quadrate.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/quadrate/quadrate.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/refine/refine.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/refine/refine.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/registry.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/registry.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/run.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/run.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/size/size.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/size/size.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/smooth/smooth.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/smooth/smooth.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/strategy/strategy.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/structure/structure.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/structure/structure.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/support/support.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/support/support.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/transform/transform.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/transform/transform.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/utils/obj2gmsh.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/utils/obj2gmsh.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts/zone/zone.py` & `gmsh_scripts-0.4.4/src/gmsh_scripts/zone/zone.py`

 * *Files identical despite different names*

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts.egg-info/PKG-INFO` & `gmsh_scripts-0.4.4/src/gmsh_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsh-scripts
-Version: 0.4.3
+Version: 0.4.4
 Summary: Scripts for GMSH mesh generator
 Home-page: https://github.com/romanzes637/gmsh_scripts
 Author: Roman Pashkovsky
 Author-email: romapasky@gmail.com
 Project-URL: Bug Tracker, https://github.com/romanzes637/gmsh_scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gmsh-scripts Version: 0.4.3 Summary: Scripts for
+Metadata-Version: 2.1 Name: gmsh-scripts Version: 0.4.4 Summary: Scripts for
 GMSH mesh generator Home-page: https://github.com/romanzes637/gmsh_scripts
 Author: Roman Pashkovsky Author-email: romapasky@gmail.com Project-URL: Bug
 Tracker, https://github.com/romanzes637/gmsh_scripts/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
 Dist: gmsh Requires-Dist: numpy Requires-Dist: pyyaml Provides-Extra: viz
```

### Comparing `gmsh_scripts-0.4.3/src/gmsh_scripts.egg-info/SOURCES.txt` & `gmsh_scripts-0.4.4/src/gmsh_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*


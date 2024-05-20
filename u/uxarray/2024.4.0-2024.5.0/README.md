# Comparing `tmp/uxarray-2024.4.0.tar.gz` & `tmp/uxarray-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxarray-2024.4.0.tar", last modified: Fri Apr 26 00:56:58 2024, max compression
+gzip compressed data, was "uxarray-2024.5.0.tar", last modified: Mon May 20 05:03:49 2024, max compression
```

## Comparing `uxarray-2024.4.0.tar` & `uxarray-2024.5.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.479817 uxarray-2024.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-26 00:56:37.000000 uxarray-2024.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-26 00:56:37.000000 uxarray-2024.4.0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-26 00:56:37.000000 uxarray-2024.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 00:56:37.000000 uxarray-2024.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-26 00:56:58.479817 uxarray-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-26 00:56:37.000000 uxarray-2024.4.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-26 00:56:37.000000 uxarray-2024.4.0/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-26 00:56:37.000000 uxarray-2024.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 00:56:58.479817 uxarray-2024.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 00:56:37.000000 uxarray-2024.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.467817 uxarray-2024.4.0/uxarray/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.467817 uxarray-2024.4.0/uxarray/conventions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/conventions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/conventions/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/conventions/ugrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.471817 uxarray-2024.4.0/uxarray/core/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/core/dataarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    12693 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/core/gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.471817 uxarray-2024.4.0/uxarray/grid/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/arcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26484 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/area.py
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    35388 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    44245 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)    34181 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)    10782 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/grid/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.475817 uxarray-2024.4.0/uxarray/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/_esmf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/_exodus.py
--rw-r--r--   0 runner    (1001) docker     (127)    17277 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/_mpas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/_scrip.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/_shapefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/_ugrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/_vertices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.475817 uxarray-2024.4.0/uxarray/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/plot/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/plot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/plot/dataarray_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/plot/dataset_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/plot/grid_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.475817 uxarray-2024.4.0/uxarray/remap/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/remap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/remap/dataarray_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/remap/dataset_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/remap/inverse_distance_weighted.py
--rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/remap/nearest_neighbor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.475817 uxarray-2024.4.0/uxarray/subset/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/subset/dataarray_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/subset/grid_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.475817 uxarray-2024.4.0/uxarray/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/utils/computing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-26 00:56:37.000000 uxarray-2024.4.0/uxarray/utils/numba_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:56:58.475817 uxarray-2024.4.0/uxarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-26 00:56:58.000000 uxarray-2024.4.0/uxarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-26 00:56:58.000000 uxarray-2024.4.0/uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 00:56:58.000000 uxarray-2024.4.0/uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-26 00:56:58.000000 uxarray-2024.4.0/uxarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-26 00:56:58.000000 uxarray-2024.4.0/uxarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.551735 uxarray-2024.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-20 05:03:38.000000 uxarray-2024.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-20 05:03:38.000000 uxarray-2024.5.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-20 05:03:38.000000 uxarray-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 05:03:38.000000 uxarray-2024.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-05-20 05:03:49.551735 uxarray-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-05-20 05:03:38.000000 uxarray-2024.5.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-05-20 05:03:38.000000 uxarray-2024.5.0/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-20 05:03:38.000000 uxarray-2024.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:03:49.551735 uxarray-2024.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 05:03:38.000000 uxarray-2024.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.539735 uxarray-2024.5.0/uxarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.539735 uxarray-2024.5.0/uxarray/conventions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/conventions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/conventions/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/conventions/ugrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.539735 uxarray-2024.5.0/uxarray/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/core/dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12693 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/core/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.543735 uxarray-2024.5.0/uxarray/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/arcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26458 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35388 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44198 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14865 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34181 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10782 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/grid/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.543735 uxarray-2024.5.0/uxarray/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/_esmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17277 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/_shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/_ugrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.547735 uxarray-2024.5.0/uxarray/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/plot/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/plot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/plot/dataarray_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/plot/dataset_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/plot/grid_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.547735 uxarray-2024.5.0/uxarray/remap/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/remap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/remap/dataarray_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/remap/dataset_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/remap/inverse_distance_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/remap/nearest_neighbor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.547735 uxarray-2024.5.0/uxarray/subset/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/subset/dataarray_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/subset/grid_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.547735 uxarray-2024.5.0/uxarray/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/utils/computing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-20 05:03:38.000000 uxarray-2024.5.0/uxarray/utils/numba_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:03:49.547735 uxarray-2024.5.0/uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-05-20 05:03:49.000000 uxarray-2024.5.0/uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-20 05:03:49.000000 uxarray-2024.5.0/uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:03:49.000000 uxarray-2024.5.0/uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 05:03:49.000000 uxarray-2024.5.0/uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 05:03:49.000000 uxarray-2024.5.0/uxarray.egg-info/top_level.txt
```

### Comparing `uxarray-2024.4.0/LICENSE` & `uxarray-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/PKG-INFO` & `uxarray-2024.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Xarray-styled package for reading and directly operating on unstructured grid datasets following UGRID conventions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -220,15 +220,14 @@
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: antimeridian
 Requires-Dist: cartopy
-Requires-Dist: cartopy
 Requires-Dist: dask[dataframe]
 Requires-Dist: datashader
 Requires-Dist: geoviews
 Requires-Dist: holoviews
 Requires-Dist: matplotlib
 Requires-Dist: matplotlib-inline
 Requires-Dist: netcdf4
```

### Comparing `uxarray-2024.4.0/README.md` & `uxarray-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/pyproject.toml` & `uxarray-2024.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 readme = "README.md"
 requires-python = ">=3.9"
 
 # minimal dependencies start
 dependencies = [
   "antimeridian",
   "cartopy",
-  "cartopy",
   "dask[dataframe]",
   "datashader",
   "geoviews",
   "holoviews",
   "matplotlib",
   "matplotlib-inline",
   "netcdf4",
@@ -68,7 +67,14 @@
 find = {}
 
 [tool.setuptools_scm]
 fallback_version = "9999"
 
 [tool.ruff]
 extend-exclude = ["test","benchmarks"]
+
+[tool.ruff.lint]
+ignore-init-module-imports = false
+
+[tool.ruff.lint.per-file-ignores]
+"docs/*" = ["E402", "F401"]
+"uxarray/plot/*" = ["E402", "F401"]
```

### Comparing `uxarray-2024.4.0/uxarray/__init__.py` & `uxarray-2024.5.0/uxarray/__init__.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/constants.py` & `uxarray-2024.5.0/uxarray/constants.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/conventions/descriptors.py` & `uxarray-2024.5.0/uxarray/conventions/descriptors.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/conventions/ugrid.py` & `uxarray-2024.5.0/uxarray/conventions/ugrid.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/core/api.py` & `uxarray-2024.5.0/uxarray/core/api.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/core/dataarray.py` & `uxarray-2024.5.0/uxarray/core/dataarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import xarray as xr
 import numpy as np
 
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Optional, Union, Hashable
 
 from uxarray.grid import Grid
 import uxarray.core.dataset
 
 if TYPE_CHECKING:
     from uxarray.core.dataset import UxDataset
 
@@ -241,19 +241,43 @@
         # data not mapped to faces or nodes
         else:
             raise ValueError(
                 f"Data Variable with size {self.values.size} does not match the number of faces "
                 f"({self.uxgrid.n_face}."
             )
 
-    def to_dataset(self) -> UxDataset:
-        """Converts a ``UxDataArray`` into a ``UxDataset`` with a single data
-        variable."""
-        xrds = super().to_dataset()
-        return uxarray.core.dataset.UxDataset(xrds, uxgrid=self.uxgrid)
+    def to_dataset(
+        self,
+        dim: Hashable = None,
+        *,
+        name: Hashable = None,
+        promote_attrs: bool = False,
+    ) -> UxDataset:
+        """Convert a UxDataArray to a UxDataset.
+
+        Parameters
+        ----------
+        dim : Hashable, optional
+            Name of the dimension on this array along which to split this array
+            into separate variables. If not provided, this array is converted
+            into a Dataset of one variable.
+        name : Hashable, optional
+            Name to substitute for this array's name. Only valid if ``dim`` is
+            not provided.
+        promote_attrs : bool, default: False
+            Set to True to shallow copy attrs of UxDataArray to returned UxDataset.
+
+        Returns
+        -------
+        uxds: UxDataSet
+        """
+        xrds = super().to_dataset(dim=dim, name=name, promote_attrs=promote_attrs)
+        uxds = uxarray.core.dataset.UxDataset(xrds, uxgrid=self.uxgrid)
+
+        return uxds
 
     def nearest_neighbor_remap(
         self,
         destination_obj: Union[Grid, UxDataArray, UxDataset],
         remap_to: str = "nodes",
         coord_type: str = "spherical",
     ):
```

### Comparing `uxarray-2024.4.0/uxarray/core/dataset.py` & `uxarray-2024.5.0/uxarray/core/dataset.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/core/gradient.py` & `uxarray-2024.5.0/uxarray/core/gradient.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/core/utils.py` & `uxarray-2024.5.0/uxarray/core/utils.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/grid/arcs.py` & `uxarray-2024.5.0/uxarray/grid/arcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 
-from uxarray.grid.coordinates import node_xyz_to_lonlat_rad, normalize_in_place
+# from uxarray.grid.coordinates import node_xyz_to_lonlat_rad, normalize_in_place
+
+from uxarray.grid.coordinates import _xyz_to_lonlat_rad, _normalize_xyz
 from uxarray.constants import ERROR_TOLERANCE
 
 
 def _to_list(obj):
     if not isinstance(obj, list):
         if isinstance(obj, np.ndarray):
             # Convert the NumPy array to a list using .tolist()
@@ -54,17 +56,21 @@
     In this case, the function handles scenarios where the GCA spans across more than 180 degrees, requiring specific operation.
 
     The function relies on the `_angle_of_2_vectors` and `is_between` functions to perform the necessary calculations.
 
     Please ensure that the input coordinates are in radians and adhere to the ERROR_TOLERANCE value for floating-point comparisons.
     """
     # Convert the cartesian coordinates to lonlat coordinates
-    pt_lonlat = node_xyz_to_lonlat_rad(_to_list(pt))
-    GCRv0_lonlat = node_xyz_to_lonlat_rad(_to_list(gca_cart[0]))
-    GCRv1_lonlat = node_xyz_to_lonlat_rad(_to_list(gca_cart[1]))
+    pt_lonlat = np.array(_xyz_to_lonlat_rad(pt[0], pt[1], pt[2]))
+    GCRv0_lonlat = np.array(
+        _xyz_to_lonlat_rad(gca_cart[0][0], gca_cart[0][1], gca_cart[0][2])
+    )
+    GCRv1_lonlat = np.array(
+        _xyz_to_lonlat_rad(gca_cart[1][0], gca_cart[1][1], gca_cart[1][2])
+    )
 
     # Convert the list to np.float64
     gca_cart[0] = np.array(gca_cart[0], dtype=np.float64)
     gca_cart[1] = np.array(gca_cart[1], dtype=np.float64)
 
     # First if the input GCR is exactly 180 degree, we throw an exception, since this GCR can have multiple planes
     angle = _angle_of_2_vectors(gca_cart[0], gca_cart[1])
@@ -280,22 +286,21 @@
     d_a_max = (n1[2] * dot_n1_n2 - n2[2]) / denom
 
     d_a_max = (
         np.clip(d_a_max, 0, 1)
         if np.isclose(d_a_max, [0, 1], atol=ERROR_TOLERANCE).any()
         else d_a_max
     )
-    lat_n1, lat_n2 = (
-        node_xyz_to_lonlat_rad(n1.tolist())[1],
-        node_xyz_to_lonlat_rad(n2.tolist())[1],
-    )
+
+    _, lat_n1 = _xyz_to_lonlat_rad(n1[0], n1[1], n1[2])
+    _, lat_n2 = _xyz_to_lonlat_rad(n2[0], n2[1], n2[2])
 
     if 0 < d_a_max < 1:
         node3 = (1 - d_a_max) * n1 + d_a_max * n2
-        node3 = np.array(normalize_in_place(node3.tolist()))
+        node3 = np.array(_normalize_xyz(node3[0], node3[1], node3[2]))
         d_lat_rad = np.arcsin(np.clip(node3[2], -1, 1))
 
         return (
             max(d_lat_rad, lat_n1, lat_n2)
             if extreme_type == "max"
             else min(d_lat_rad, lat_n1, lat_n2)
         )
```

### Comparing `uxarray-2024.4.0/uxarray/grid/area.py` & `uxarray-2024.5.0/uxarray/grid/area.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-from numba import njit, config
-from uxarray.constants import ENABLE_JIT_CACHE, ENABLE_JIT
 
-from uxarray.grid.coordinates import node_lonlat_rad_to_xyz
+from uxarray.grid.coordinates import _lonlat_rad_to_xyz
 
+from numba import njit, config
+from uxarray.constants import ENABLE_JIT_CACHE, ENABLE_JIT
 
 config.DISABLE_JIT = not ENABLE_JIT
 
 
 @njit(cache=ENABLE_JIT_CACHE)
 def calculate_face_area(
     x, y, z, quadrature_rule="gaussian", order=4, coords_type="spherical"
@@ -63,23 +63,22 @@
     # loop through all sub-triangles of face
     for j in range(0, num_triangles):
         node1 = np.array([x[0], y[0], z[0]], dtype=np.float64)
         node2 = np.array([x[j + 1], y[j + 1], z[j + 1]], dtype=np.float64)
         node3 = np.array([x[j + 2], y[j + 2], z[j + 2]], dtype=np.float64)
 
         if coords_type == "spherical":
-            node1 = np.array(
-                node_lonlat_rad_to_xyz([np.deg2rad(x[0]), np.deg2rad(y[0])])
-            )
-            node2 = np.array(
-                node_lonlat_rad_to_xyz([np.deg2rad(x[j + 1]), np.deg2rad(y[j + 1])])
-            )
-            node3 = np.array(
-                node_lonlat_rad_to_xyz([np.deg2rad(x[j + 2]), np.deg2rad(y[j + 2])])
-            )
+            node1 = _lonlat_rad_to_xyz(np.deg2rad(x[0]), np.deg2rad(y[0]))
+            node1 = np.asarray(node1)
+
+            node2 = _lonlat_rad_to_xyz(np.deg2rad(x[j + 1]), np.deg2rad(y[j + 1]))
+            node2 = np.asarray(node2)
+
+            node3 = _lonlat_rad_to_xyz(np.deg2rad(x[j + 2]), np.deg2rad(y[j + 2]))
+            node3 = np.asarray(node3)
 
         for p in range(len(dW)):
             if quadrature_rule == "gaussian":
                 for q in range(len(dW)):
                     dA = dG[0][p]
                     dB = dG[0][q]
                     jacobian = calculate_spherical_triangle_jacobian(
```

### Comparing `uxarray-2024.4.0/uxarray/grid/connectivity.py` & `uxarray-2024.5.0/uxarray/grid/connectivity.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/grid/geometry.py` & `uxarray-2024.5.0/uxarray/grid/geometry.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/grid/grid.py` & `uxarray-2024.5.0/uxarray/grid/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 from uxarray.io.utils import _parse_grid_type
 from uxarray.grid.area import get_all_face_area_from_coords
 from uxarray.grid.coordinates import (
     _populate_face_centroids,
     _populate_edge_centroids,
     _set_desired_longitude_range,
-    _populate_lonlat_coord,
-    _populate_cartesian_xyz_coord,
+    _populate_node_latlon,
+    _populate_node_xyz,
 )
 from uxarray.grid.connectivity import (
     _populate_edge_node_connectivity,
     _populate_face_edge_connectivity,
     _populate_n_nodes_per_face,
     _populate_node_face_connectivity,
     _populate_edge_face_connectivity,
@@ -550,57 +550,57 @@
     def node_lon(self) -> xr.DataArray:
         """Longitude of each node in degrees.
 
         Dimensions: ``(n_node, )``
         """
         if "node_lon" not in self._ds:
             _set_desired_longitude_range(self._ds)
-            _populate_lonlat_coord(self)
+            _populate_node_latlon(self)
         return self._ds["node_lon"]
 
     @property
     def node_lat(self) -> xr.DataArray:
         """Latitude of each node in degrees.
 
         Dimensions: ``(n_node, )``
         """
         if "node_lat" not in self._ds:
             _set_desired_longitude_range(self._ds)
-            _populate_lonlat_coord(self)
+            _populate_node_latlon(self)
         return self._ds["node_lat"]
 
     @property
     def node_x(self) -> xr.DataArray:
         """Cartesian x location of each node in meters.
 
         Dimensions: ``(n_node, )``
         """
         if "node_x" not in self._ds:
-            _populate_cartesian_xyz_coord(self)
+            _populate_node_xyz(self)
 
         return self._ds["node_x"]
 
     @property
     def node_y(self) -> xr.DataArray:
         """Cartesian y location of each node in meters.
 
         Dimensions: ``(n_node, )``
         """
         if "node_y" not in self._ds:
-            _populate_cartesian_xyz_coord(self)
+            _populate_node_xyz(self)
         return self._ds["node_y"]
 
     @property
     def node_z(self) -> xr.DataArray:
         """Cartesian z location of each node in meters.
 
         Dimensions: ``(n_node, )``
         """
         if "node_z" not in self._ds:
-            _populate_cartesian_xyz_coord(self)
+            _populate_node_xyz(self)
         return self._ds["node_z"]
 
     @property
     def edge_lon(self) -> xr.DataArray:
         """Longitude of the center of each edge in degrees.
 
         Dimensions: ``(n_edge, )``
```

### Comparing `uxarray-2024.4.0/uxarray/grid/integrate.py` & `uxarray-2024.5.0/uxarray/grid/integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from uxarray.constants import ERROR_TOLERANCE, INT_FILL_VALUE
 from uxarray.grid.intersections import gca_constLat_intersection
-from uxarray.grid.coordinates import node_xyz_to_lonlat_rad
+from uxarray.grid.coordinates import _xyz_to_lonlat_rad
 import pandas as pd
 
 DUMMY_EDGE_VALUE = [INT_FILL_VALUE, INT_FILL_VALUE, INT_FILL_VALUE]
 
 
 def _get_zonal_faces_weight_at_constLat(
     faces_edges_cart,
@@ -187,17 +187,19 @@
                     intersections_pts_list_cart.extend(intersections)
                 else:
                     intersections_pts_list_cart.append(intersections[0])
 
     # Handle unique intersections and check for convex or concave cases
     unique_intersections = np.unique(intersections_pts_list_cart, axis=0)
     if len(unique_intersections) == 2:
+        # TODO: vectorize?
         unique_intersection_lonlat = np.array(
-            [node_xyz_to_lonlat_rad(pt.tolist()) for pt in unique_intersections]
+            [_xyz_to_lonlat_rad(pt[0], pt[1], pt[2]) for pt in unique_intersections]
         )
+
         sorted_lonlat = np.sort(unique_intersection_lonlat, axis=0)
         pt_lon_min, pt_lon_max = sorted_lonlat[:, 0]
         return unique_intersections, pt_lon_min, pt_lon_max
     elif len(unique_intersections) != 0:
         raise ValueError(
             "UXarray doesn't support concave face with intersections points as currently, please modify your grids accordingly"
         )
@@ -261,15 +263,15 @@
         pt_lon_max,
     ) = _get_faces_constLat_intersection_info(
         face_edges_cart, latitude_cart, is_GCA_list, is_latlonface, is_directed
     )
 
     # Convert intersection points to longitude-latitude
     longitudes = np.array(
-        [node_xyz_to_lonlat_rad(pt.tolist())[0] for pt in unique_intersections]
+        [_xyz_to_lonlat_rad(*pt.tolist())[0] for pt in unique_intersections]
     )
 
     # Handle special wrap-around cases by checking the face bounds
     if face_lon_bound_left >= face_lon_bound_right:
         if not (
             (pt_lon_max >= np.pi and pt_lon_min >= np.pi)
             or (0 <= pt_lon_max <= np.pi and 0 <= pt_lon_min <= np.pi)
```

### Comparing `uxarray-2024.4.0/uxarray/grid/intersections.py` & `uxarray-2024.5.0/uxarray/grid/intersections.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/grid/neighbors.py` & `uxarray-2024.5.0/uxarray/grid/neighbors.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/grid/slice.py` & `uxarray-2024.5.0/uxarray/grid/slice.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/grid/utils.py` & `uxarray-2024.5.0/uxarray/grid/utils.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/grid/validation.py` & `uxarray-2024.5.0/uxarray/grid/validation.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/io/_esmf.py` & `uxarray-2024.5.0/uxarray/io/_esmf.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/io/_exodus.py` & `uxarray-2024.5.0/uxarray/io/_exodus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import xarray as xr
 import numpy as np
 from pathlib import PurePath
 from datetime import datetime
 
 from uxarray.grid.connectivity import _replace_fill_values
 from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
-from uxarray.grid.coordinates import _get_lonlat_from_xyz, _get_xyz_from_lonlat
+
+from uxarray.grid.coordinates import _lonlat_rad_to_xyz, _xyz_to_lonlat_deg
 
 from uxarray.conventions import ugrid
 
 
 # Exodus Number is one-based.
 def _read_exodus(ext_ds):
     """Exodus file reader.
@@ -96,15 +97,15 @@
     ds["face_node_connectivity"] = xr.DataArray(
         data=face_nodes,
         dims=ugrid.FACE_NODE_CONNECTIVITY_DIMS,
         attrs=ugrid.FACE_NODE_CONNECTIVITY_ATTRS,
     )
 
     # populate lon/lat coordinates
-    lon, lat = _get_lonlat_from_xyz(
+    lon, lat = _xyz_to_lonlat_deg(
         ds["node_x"].values, ds["node_y"].values, ds["node_z"].values
     )
 
     # populate dataset
     ds["node_lon"] = xr.DataArray(
         data=lon, dims=[ugrid.NODE_DIM], attrs=ugrid.NODE_LON_ATTRS
     )
@@ -177,15 +178,15 @@
         data=xr.DataArray(np.array(qa_records, dtype="str")),
         dims=["four", "num_qa_rec"],
     )
 
     # Set the dim to 3 as we will always have x/y/z for cartesian grid
     # Note: Don't get orig dimension from Mesh2 attribute topology dimension
     if "node_x" not in ds:
-        x, y, z = _get_xyz_from_lonlat(ds["node_lon"].values, ds["node_lat"].values)
+        x, y, z = _lonlat_rad_to_xyz(ds["node_lon"].values, ds["node_lat"].values)
         c_data = xr.DataArray([x, y, z])
     else:
         c_data = xr.DataArray(
             [
                 ds["node_x"].data.tolist(),
                 ds["node_y"].data.tolist(),
                 ds["node_z"].data.tolist(),
```

### Comparing `uxarray-2024.4.0/uxarray/io/_mpas.py` & `uxarray-2024.5.0/uxarray/io/_mpas.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/io/_scrip.py` & `uxarray-2024.5.0/uxarray/io/_scrip.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/io/_topology.py` & `uxarray-2024.5.0/uxarray/io/_topology.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/io/_ugrid.py` & `uxarray-2024.5.0/uxarray/io/_ugrid.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/io/_vertices.py` & `uxarray-2024.5.0/uxarray/io/_vertices.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/io/utils.py` & `uxarray-2024.5.0/uxarray/io/utils.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/plot/accessor.py` & `uxarray-2024.5.0/uxarray/plot/accessor.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/plot/dataarray_plot.py` & `uxarray-2024.5.0/uxarray/plot/dataarray_plot.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/plot/grid_plot.py` & `uxarray-2024.5.0/uxarray/plot/grid_plot.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/plot/utils.py` & `uxarray-2024.5.0/uxarray/plot/utils.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/remap/dataarray_accessor.py` & `uxarray-2024.5.0/uxarray/remap/dataarray_accessor.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/remap/dataset_accessor.py` & `uxarray-2024.5.0/uxarray/remap/dataset_accessor.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/remap/inverse_distance_weighted.py` & `uxarray-2024.5.0/uxarray/remap/inverse_distance_weighted.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/remap/nearest_neighbor.py` & `uxarray-2024.5.0/uxarray/remap/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/subset/dataarray_accessor.py` & `uxarray-2024.5.0/uxarray/subset/dataarray_accessor.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/subset/grid_accessor.py` & `uxarray-2024.5.0/uxarray/subset/grid_accessor.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/utils/computing.py` & `uxarray-2024.5.0/uxarray/utils/computing.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray/utils/numba_settings.py` & `uxarray-2024.5.0/uxarray/utils/numba_settings.py`

 * *Files identical despite different names*

### Comparing `uxarray-2024.4.0/uxarray.egg-info/PKG-INFO` & `uxarray-2024.5.0/uxarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Xarray-styled package for reading and directly operating on unstructured grid datasets following UGRID conventions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -220,15 +220,14 @@
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: antimeridian
 Requires-Dist: cartopy
-Requires-Dist: cartopy
 Requires-Dist: dask[dataframe]
 Requires-Dist: datashader
 Requires-Dist: geoviews
 Requires-Dist: holoviews
 Requires-Dist: matplotlib
 Requires-Dist: matplotlib-inline
 Requires-Dist: netcdf4
```

### Comparing `uxarray-2024.4.0/uxarray.egg-info/SOURCES.txt` & `uxarray-2024.5.0/uxarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

